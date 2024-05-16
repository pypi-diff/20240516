# Comparing `tmp/lightly-1.5.3.tar.gz` & `tmp/lightly-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightly-1.5.3.tar", last modified: Wed Apr 17 09:28:59 2024, max compression
+gzip compressed data, was "lightly-1.5.4.tar", last modified: Thu May 16 12:54:12 2024, max compression
```

## Comparing `lightly-1.5.3.tar` & `lightly-1.5.4.tar`

### file list

```diff
@@ -1,471 +1,472 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.473692 lightly-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-17 09:28:50.000000 lightly-1.5.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-17 09:28:50.000000 lightly-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24439 2024-04-17 09:28:59.473692 lightly-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22857 2024-04-17 09:28:50.000000 lightly-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.409692 lightly-1.5.3/lightly/
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.409692 lightly-1.5.3/lightly/active_learning/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/active_learning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.409692 lightly-1.5.3/lightly/active_learning/config/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/active_learning/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/active_learning/config/selection_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.413692 lightly-1.5.3/lightly/api/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/_version_checking.py
--rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_collaboration.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_compute_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    20194 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    36969 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_download_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    13415 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_upload_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/api_workflow_upload_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/bitmask.py
--rw-r--r--   0 runner    (1001) docker     (127)    19947 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/swagger_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/swagger_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.413692 lightly-1.5.3/lightly/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/_cli_simclr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.417692 lightly-1.5.3/lightly/cli/config/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/config/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/config/lightly-serve.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/crop_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/download_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/embed_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/lightly_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/serve_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/train_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/cli/version_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.417692 lightly-1.5.3/lightly/data/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/_image.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/_image_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25874 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/_video.py
--rw-r--r--   0 runner    (1001) docker     (127)    55856 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/lightly_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/data/multi_view_collate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.417692 lightly-1.5.3/lightly/embedding/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/embedding/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/embedding/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/embedding/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.421692 lightly-1.5.3/lightly/loss/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/barlow_twins_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/dcl_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/dino_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/emp_ssl_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/hypersphere_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/mmcr_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/msn_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/negative_cosine_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/ntx_ent_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/pmsn_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.421692 lightly-1.5.3/lightly/loss/regularizer/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/regularizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/regularizer/co2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/swav_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/sym_neg_cos_sim_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/tico_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/vicreg_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    17701 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/vicregl_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/loss/wmse_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.421692 lightly-1.5.3/lightly/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/_momentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/barlowtwins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/byol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/moco.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.421692 lightly-1.5.3/lightly/models/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/heads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/heads_timm.py
--rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/ijepa.py
--rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/masked_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/masked_autoencoder_timm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/masked_causal_vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/masked_vision_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/masked_vision_transformer_timm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/masked_vision_transformer_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/modules/nn_memory_bank.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/nnclr.py
--rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/simclr.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/simsiam.py
--rw-r--r--   0 runner    (1001) docker     (127)    25558 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/models/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.421692 lightly-1.5.3/lightly/openapi_generated/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.425692 lightly-1.5.3/lightly/openapi_generated/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (127)    31210 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.429692 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22634 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/collaboration_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    94278 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/datasets_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   136811 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/datasources_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   300001 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/docker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    24023 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    52405 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/embeddings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/jobs_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/mappings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30243 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    58282 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/predictions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/quota_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    80830 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/samples_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/samplings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    51643 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/scores_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   160366 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/tags_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41806 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/teams_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api/versioning_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17712 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.465692 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)    29006 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/active_learning_score_types_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/active_learning_score_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/api_error_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/api_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/async_task_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/configuration_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/configuration_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_cf_bucket_activity_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_entity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_team_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/crop_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_azure_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_base_full_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_gcs_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_local_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_obs_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_s3_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/delegated_access_external_ids_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_authorization_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_authorization_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_license_information.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_storage_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_create_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_docker_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_task_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_authorization_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_datasource_input_expiration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
--rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/embedding_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/expiry_handling_strategy_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/file_name_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/file_output_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/image_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/internal_debug_latency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/internal_debug_latency_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_result_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_status_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_status_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/jobs_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/label_studio_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_docker_selection_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/profile_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/profile_me_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/profile_me_data_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/s3_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sama_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sama_task_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sampling_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sampling_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of_target_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4_all_of.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_input_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_strategy_type_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/service_account_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/shared_access_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_creator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/task_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/team_basic_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/team_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/team_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/update_team_membership_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/video_frame_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/openapi_generated/swagger_client/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.469692 lightly-1.5.3/lightly/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/aim_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/byol_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/dino_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/fast_siam_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/gaussian_blur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/ijepa_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/image_grid_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/jigsaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/mae_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/mmcr_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/moco_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/msn_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/multi_crop_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/multi_view_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/pirl_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/random_crop_and_flip_with_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/simclr_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/simsiam_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/smog_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/solarize.py
--rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/swav_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/vicreg_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/vicregl_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/transforms/wmse_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.473692 lightly-1.5.3/lightly/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.473692 lightly-1.5.3/lightly/utils/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/benchmarking/benchmark_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/benchmarking/knn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/benchmarking/knn_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/benchmarking/linear_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/benchmarking/metric_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/benchmarking/online_linear_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/benchmarking/topk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/bounding_box.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.473692 lightly-1.5.3/lightly/utils/cropping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/cropping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/cropping/crop_image_by_bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/cropping/read_yolo_label_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/dist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/embeddings_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/hipify.py
--rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/lars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/reordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-17 09:28:50.000000 lightly-1.5.3/lightly/utils/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 09:28:59.409692 lightly-1.5.3/lightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24439 2024-04-17 09:28:59.000000 lightly-1.5.3/lightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27421 2024-04-17 09:28:59.000000 lightly-1.5.3/lightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 09:28:59.000000 lightly-1.5.3/lightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-17 09:28:59.000000 lightly-1.5.3/lightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-17 09:28:59.000000 lightly-1.5.3/lightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-17 09:28:59.000000 lightly-1.5.3/lightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-17 09:28:50.000000 lightly-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 09:28:59.473692 lightly-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-17 09:28:50.000000 lightly-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.207729 lightly-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-16 12:54:00.000000 lightly-1.5.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 12:54:00.000000 lightly-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25843 2024-05-16 12:54:12.207729 lightly-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24261 2024-05-16 12:54:00.000000 lightly-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.139728 lightly-1.5.4/lightly/
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.139728 lightly-1.5.4/lightly/active_learning/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/active_learning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.139728 lightly-1.5.4/lightly/active_learning/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/active_learning/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/active_learning/config/selection_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.143728 lightly-1.5.4/lightly/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/_version_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17421 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11430 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_collaboration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_compute_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20194 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36969 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11584 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_download_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13415 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_upload_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/api_workflow_upload_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/bitmask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19947 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/swagger_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5582 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/swagger_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.143728 lightly-1.5.4/lightly/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/_cli_simclr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7439 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.147728 lightly-1.5.4/lightly/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/config/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/config/lightly-serve.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/crop_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/download_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/embed_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/lightly_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/serve_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/train_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/cli/version_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.147728 lightly-1.5.4/lightly/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_image_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25874 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55856 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13019 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/lightly_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/data/multi_view_collate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.147728 lightly-1.5.4/lightly/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/embedding/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/embedding/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/embedding/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.151728 lightly-1.5.4/lightly/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/barlow_twins_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/dcl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/dino_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/emp_ssl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/hypersphere_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/mmcr_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8522 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/msn_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/negative_cosine_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/ntx_ent_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5846 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/pmsn_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.151728 lightly-1.5.4/lightly/loss/regularizer/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/regularizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/regularizer/co2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/swav_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/sym_neg_cos_sim_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/tico_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4791 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/vicreg_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17701 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/vicregl_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/loss/wmse_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.151728 lightly-1.5.4/lightly/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3364 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/_momentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/barlowtwins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/byol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/moco.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.155728 lightly-1.5.4/lightly/models/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26726 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/heads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/heads_timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15110 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/ijepa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17520 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_autoencoder_timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_causal_vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_vision_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_vision_transformer_timm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/masked_vision_transformer_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6323 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/modules/nn_memory_bank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/nnclr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/simclr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/simsiam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25558 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/models/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.155728 lightly-1.5.4/lightly/openapi_generated/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.155728 lightly-1.5.4/lightly/openapi_generated/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    31348 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.159728 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22634 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/collaboration_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98546 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/datasets_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/datasources_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   308272 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/docker_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24023 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52405 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/embeddings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13183 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/jobs_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/mappings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30243 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61239 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/predictions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7024 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/quota_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81340 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/samples_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/samplings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51643 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/scores_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   160366 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/tags_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41806 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api/versioning_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17712 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.199729 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    29144 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_types_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/api_error_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/api_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/async_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_cf_bucket_activity_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_entity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_team_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/crop_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7328 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13223 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_base_full_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_local_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/delegated_access_external_ids_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_authorization_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_authorization_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_license_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_storage_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_create_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_docker_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3829 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_task_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_user_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_authorization_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9246 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5927 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_datasource_input_expiration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3404 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9651 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4207 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding2d_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/expiry_handling_strategy_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/file_name_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/file_output_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/image_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/internal_debug_latency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/internal_debug_latency_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_result_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_data_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4075 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/jobs_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_box_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_studio_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_docker_selection_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_me_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_me_data_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/questionnaire_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/s3_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sama_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sama_task_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5272 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_data_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_sort_by.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_write_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of_target_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_input_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/service_account_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/task_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_basic_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/update_team_membership_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/video_frame_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12981 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/openapi_generated/swagger_client/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.203729 lightly-1.5.4/lightly/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/aim_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/byol_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/dino_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/fast_siam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/gaussian_blur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/ijepa_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/image_grid_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/jigsaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/mae_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/mmcr_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/moco_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6627 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/msn_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/multi_crop_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/multi_view_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/pirl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/random_crop_and_flip_with_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/simclr_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/simsiam_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/smog_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/solarize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6436 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/swav_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/vicreg_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/vicregl_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/transforms/wmse_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.203729 lightly-1.5.4/lightly/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.207729 lightly-1.5.4/lightly/utils/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/benchmark_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/knn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/knn_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6081 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/linear_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/metric_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/online_linear_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/benchmarking/topk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/bounding_box.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.207729 lightly-1.5.4/lightly/utils/cropping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/cropping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/cropping/crop_image_by_bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/cropping/read_yolo_label_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/embeddings_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/hipify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11598 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/lars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/reordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-16 12:54:00.000000 lightly-1.5.4/lightly/utils/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:54:12.139728 lightly-1.5.4/lightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25843 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27514 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 12:54:12.000000 lightly-1.5.4/lightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-16 12:54:00.000000 lightly-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:54:12.207729 lightly-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-16 12:54:00.000000 lightly-1.5.4/setup.py
```

### Comparing `lightly-1.5.3/LICENSE.txt` & `lightly-1.5.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/PKG-INFO` & `lightly-1.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.5.3
+Version: 1.5.4
 Summary: A deep learning package for self-supervised learning
 Author: Lightly Team
 Author-email: team@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
@@ -310,27 +310,27 @@
 
 - Linear: [SimCLR](https://arxiv.org/abs/2002.05709)
 - Finetune: [SimCLR](https://arxiv.org/abs/2002.05709)
 - KNN: [InstDisc](https://arxiv.org/abs/1805.01978)
 
 See the [benchmarking scripts](./benchmarks/imagenet/resnet50/) for details.
 
-| Model           | Backbone | Batch Size | Epochs | Linear Top1 | Finetune Top1 | kNN Top1 | Tensorboard                                                        | Checkpoint                                                                                                                                                              |
-| --------------- | -------- | ---------- | ------ | ----------- | ------------- | -------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| BarlowTwins     | Res50    | 256        | 100    | 62.9        | 72.6          | 45.6     | [link](https://tensorboard.dev/experiment/NxyNRiQsQjWZ82I9b0PvKg/) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_barlowtwins_2023-08-18_00-11-03/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt) |
-| BYOL            | Res50    | 256        | 100    | 62.5        | 74.5          | 46.0     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_byol_2024-02-14_16-10-09/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
-| DINO            | Res50    | 128        | 100    | 68.2        | 72.5          | 49.9     | [link](https://tensorboard.dev/experiment/DvKHX9sNSWWqDrRksllPLA)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dino_2023-06-06_13-59-48/pretrain/version_0/checkpoints/epoch%3D99-step%3D1000900.ckpt)       |
-| MAE             | ViT-B/16 | 256        | 100    | 46.0        | 81.3          | 11.2     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_vitb16_mae_2024-02-25_19-57-30/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)           |
-| MoCoV2          | Res50    | 256        | 100    | 61.5        | 74.3          | 41.8     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_mocov2_2024-02-18_10-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
-| SimCLR\*        | Res50    | 256        | 100    | 63.2        | 73.9          | 44.8     | [link](https://tensorboard.dev/experiment/Ugol97adQdezgcVibDYMMA)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-06-22_09-11-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
-| SimCLR\* + DCL  | Res50    | 256        | 100    | 65.1        | 73.5          | 49.6     | [link](https://tensorboard.dev/experiment/k4ZonZ77QzmBkc0lXswQlg/) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dcl_2023-07-04_16-51-40/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)         |
-| SimCLR\* + DCLW | Res50    | 256        | 100    | 64.5        | 73.2          | 48.5     | [link](https://tensorboard.dev/experiment/TrALnpwFQ4OkZV3uvaX7wQ/) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dclw_2023-07-07_14-57-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
-| SwAV            | Res50    | 256        | 100    | 67.2        | 75.4          | 49.5     | [link](https://tensorboard.dev/experiment/Ipx4Oxl5Qkqm5Sl5kWyKKg)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
-| TiCo            | Res50    | 256        | 100    | 49.7        | 72.7          | 26.6     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_tico_2024-01-07_18-40-57/pretrain/version_0/checkpoints/epoch%3D99-step%3D250200.ckpt)        |
-| VICReg          | Res50    | 256        | 100    | 63.0        | 73.7          | 46.3     | [link](https://tensorboard.dev/experiment/qH5uywJbTJSzgCEfxc7yUw)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_vicreg_2023-09-11_10-53-08/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
+| Model           | Backbone | Batch Size | Epochs | Linear Top1 | Finetune Top1 | kNN Top1 | Tensorboard                                                                                                                                                                    | Checkpoint                                                                                                                                                              |
+| --------------- | -------- | ---------- | ------ | ----------- | ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| BarlowTwins     | Res50    | 256        | 100    | 62.9        | 72.6          | 45.6     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_barlowtwins_2023-08-18_00-11-03/pretrain/version_0/events.out.tfevents.1692310273.Machine2.569794.0) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_barlowtwins_2023-08-18_00-11-03/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt) |
+| BYOL            | Res50    | 256        | 100    | 62.5        | 74.5          | 46.0     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_byol_2024-02-14_16-10-09/pretrain/version_0/events.out.tfevents.1707923418.Machine2.3205.0)          | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_byol_2024-02-14_16-10-09/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
+| DINO            | Res50    | 128        | 100    | 68.2        | 72.5          | 49.9     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dino_2023-06-06_13-59-48/pretrain/version_0/events.out.tfevents.1686052799.Machine2.482599.0)        | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dino_2023-06-06_13-59-48/pretrain/version_0/checkpoints/epoch%3D99-step%3D1000900.ckpt)       |
+| MAE             | ViT-B/16 | 256        | 100    | 46.0        | 81.3          | 11.2     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_vitb16_mae_2024-02-25_19-57-30/pretrain/version_0/events.out.tfevents.1708887459.Machine2.1092409.0)          | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_vitb16_mae_2024-02-25_19-57-30/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)           |
+| MoCoV2          | Res50    | 256        | 100    | 61.5        | 74.3          | 41.8     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_mocov2_2024-02-18_10-29-14/pretrain/version_0/events.out.tfevents.1708248562.Machine2.439033.0)      | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_mocov2_2024-02-18_10-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
+| SimCLR\*        | Res50    | 256        | 100    | 63.2        | 73.9          | 44.8     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-06-22_09-11-13/pretrain/version_0/events.out.tfevents.1687417883.Machine2.33270.0)       | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-06-22_09-11-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
+| SimCLR\* + DCL  | Res50    | 256        | 100    | 65.1        | 73.5          | 49.6     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dcl_2023-07-04_16-51-40/pretrain/version_0/events.out.tfevents.1688482310.Machine2.247807.0)         | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dcl_2023-07-04_16-51-40/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)         |
+| SimCLR\* + DCLW | Res50    | 256        | 100    | 64.5        | 73.2          | 48.5     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dclw_2023-07-07_14-57-13/pretrain/version_0/events.out.tfevents.1688734645.Machine2.3176.0)          | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dclw_2023-07-07_14-57-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
+| SwAV            | Res50    | 256        | 100    | 67.2        | 75.4          | 49.5     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/events.out.tfevents.1684996168.Machine2.1445108.0)       | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
+| TiCo            | Res50    | 256        | 100    | 49.7        | 72.7          | 26.6     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_tico_2024-01-07_18-40-57/pretrain/version_0/events.out.tfevents.1704649265.Machine2.1604956.0)       | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_tico_2024-01-07_18-40-57/pretrain/version_0/checkpoints/epoch%3D99-step%3D250200.ckpt)        |
+| VICReg          | Res50    | 256        | 100    | 63.0        | 73.7          | 46.3     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_vicreg_2023-09-11_10-53-08/pretrain/version_0/events.out.tfevents.1694422401.Machine2.556563.0)      | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_vicreg_2023-09-11_10-53-08/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
 
 _\*We use square root learning rate scaling instead of linear scaling as it yields
 better results for smaller batch sizes. See Appendix B.1 in the [SimCLR paper](https://arxiv.org/abs/2002.05709)._
 
 ### ImageNet100
 
 [ImageNet100 benchmarks detailed results](https://docs.lightly.ai/self-supervised-learning/getting_started/benchmarks.html#imagenet100)
```

### Comparing `lightly-1.5.3/README.md` & `lightly-1.5.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -272,27 +272,27 @@
 
 - Linear: [SimCLR](https://arxiv.org/abs/2002.05709)
 - Finetune: [SimCLR](https://arxiv.org/abs/2002.05709)
 - KNN: [InstDisc](https://arxiv.org/abs/1805.01978)
 
 See the [benchmarking scripts](./benchmarks/imagenet/resnet50/) for details.
 
-| Model           | Backbone | Batch Size | Epochs | Linear Top1 | Finetune Top1 | kNN Top1 | Tensorboard                                                        | Checkpoint                                                                                                                                                              |
-| --------------- | -------- | ---------- | ------ | ----------- | ------------- | -------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| BarlowTwins     | Res50    | 256        | 100    | 62.9        | 72.6          | 45.6     | [link](https://tensorboard.dev/experiment/NxyNRiQsQjWZ82I9b0PvKg/) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_barlowtwins_2023-08-18_00-11-03/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt) |
-| BYOL            | Res50    | 256        | 100    | 62.5        | 74.5          | 46.0     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_byol_2024-02-14_16-10-09/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
-| DINO            | Res50    | 128        | 100    | 68.2        | 72.5          | 49.9     | [link](https://tensorboard.dev/experiment/DvKHX9sNSWWqDrRksllPLA)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dino_2023-06-06_13-59-48/pretrain/version_0/checkpoints/epoch%3D99-step%3D1000900.ckpt)       |
-| MAE             | ViT-B/16 | 256        | 100    | 46.0        | 81.3          | 11.2     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_vitb16_mae_2024-02-25_19-57-30/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)           |
-| MoCoV2          | Res50    | 256        | 100    | 61.5        | 74.3          | 41.8     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_mocov2_2024-02-18_10-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
-| SimCLR\*        | Res50    | 256        | 100    | 63.2        | 73.9          | 44.8     | [link](https://tensorboard.dev/experiment/Ugol97adQdezgcVibDYMMA)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-06-22_09-11-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
-| SimCLR\* + DCL  | Res50    | 256        | 100    | 65.1        | 73.5          | 49.6     | [link](https://tensorboard.dev/experiment/k4ZonZ77QzmBkc0lXswQlg/) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dcl_2023-07-04_16-51-40/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)         |
-| SimCLR\* + DCLW | Res50    | 256        | 100    | 64.5        | 73.2          | 48.5     | [link](https://tensorboard.dev/experiment/TrALnpwFQ4OkZV3uvaX7wQ/) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dclw_2023-07-07_14-57-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
-| SwAV            | Res50    | 256        | 100    | 67.2        | 75.4          | 49.5     | [link](https://tensorboard.dev/experiment/Ipx4Oxl5Qkqm5Sl5kWyKKg)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
-| TiCo            | Res50    | 256        | 100    | 49.7        | 72.7          | 26.6     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_tico_2024-01-07_18-40-57/pretrain/version_0/checkpoints/epoch%3D99-step%3D250200.ckpt)        |
-| VICReg          | Res50    | 256        | 100    | 63.0        | 73.7          | 46.3     | [link](https://tensorboard.dev/experiment/qH5uywJbTJSzgCEfxc7yUw)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_vicreg_2023-09-11_10-53-08/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
+| Model           | Backbone | Batch Size | Epochs | Linear Top1 | Finetune Top1 | kNN Top1 | Tensorboard                                                                                                                                                                    | Checkpoint                                                                                                                                                              |
+| --------------- | -------- | ---------- | ------ | ----------- | ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| BarlowTwins     | Res50    | 256        | 100    | 62.9        | 72.6          | 45.6     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_barlowtwins_2023-08-18_00-11-03/pretrain/version_0/events.out.tfevents.1692310273.Machine2.569794.0) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_barlowtwins_2023-08-18_00-11-03/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt) |
+| BYOL            | Res50    | 256        | 100    | 62.5        | 74.5          | 46.0     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_byol_2024-02-14_16-10-09/pretrain/version_0/events.out.tfevents.1707923418.Machine2.3205.0)          | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_byol_2024-02-14_16-10-09/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
+| DINO            | Res50    | 128        | 100    | 68.2        | 72.5          | 49.9     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dino_2023-06-06_13-59-48/pretrain/version_0/events.out.tfevents.1686052799.Machine2.482599.0)        | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dino_2023-06-06_13-59-48/pretrain/version_0/checkpoints/epoch%3D99-step%3D1000900.ckpt)       |
+| MAE             | ViT-B/16 | 256        | 100    | 46.0        | 81.3          | 11.2     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_vitb16_mae_2024-02-25_19-57-30/pretrain/version_0/events.out.tfevents.1708887459.Machine2.1092409.0)          | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_vitb16_mae_2024-02-25_19-57-30/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)           |
+| MoCoV2          | Res50    | 256        | 100    | 61.5        | 74.3          | 41.8     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_mocov2_2024-02-18_10-29-14/pretrain/version_0/events.out.tfevents.1708248562.Machine2.439033.0)      | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_mocov2_2024-02-18_10-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
+| SimCLR\*        | Res50    | 256        | 100    | 63.2        | 73.9          | 44.8     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-06-22_09-11-13/pretrain/version_0/events.out.tfevents.1687417883.Machine2.33270.0)       | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-06-22_09-11-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
+| SimCLR\* + DCL  | Res50    | 256        | 100    | 65.1        | 73.5          | 49.6     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dcl_2023-07-04_16-51-40/pretrain/version_0/events.out.tfevents.1688482310.Machine2.247807.0)         | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dcl_2023-07-04_16-51-40/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)         |
+| SimCLR\* + DCLW | Res50    | 256        | 100    | 64.5        | 73.2          | 48.5     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dclw_2023-07-07_14-57-13/pretrain/version_0/events.out.tfevents.1688734645.Machine2.3176.0)          | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dclw_2023-07-07_14-57-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
+| SwAV            | Res50    | 256        | 100    | 67.2        | 75.4          | 49.5     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/events.out.tfevents.1684996168.Machine2.1445108.0)       | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
+| TiCo            | Res50    | 256        | 100    | 49.7        | 72.7          | 26.6     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_tico_2024-01-07_18-40-57/pretrain/version_0/events.out.tfevents.1704649265.Machine2.1604956.0)       | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_tico_2024-01-07_18-40-57/pretrain/version_0/checkpoints/epoch%3D99-step%3D250200.ckpt)        |
+| VICReg          | Res50    | 256        | 100    | 63.0        | 73.7          | 46.3     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_vicreg_2023-09-11_10-53-08/pretrain/version_0/events.out.tfevents.1694422401.Machine2.556563.0)      | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_vicreg_2023-09-11_10-53-08/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
 
 _\*We use square root learning rate scaling instead of linear scaling as it yields
 better results for smaller batch sizes. See Appendix B.1 in the [SimCLR paper](https://arxiv.org/abs/2002.05709)._
 
 ### ImageNet100
 
 [ImageNet100 benchmarks detailed results](https://docs.lightly.ai/self-supervised-learning/getting_started/benchmarks.html#imagenet100)
```

### Comparing `lightly-1.5.3/lightly/__init__.py` & `lightly-1.5.4/lightly/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 __name__ = "lightly"
-__version__ = "1.5.3"
+__version__ = "1.5.4"
 
 
 import os
 
 if os.getenv("LIGHTLY_DID_VERSION_CHECK", "False") == "False":
     os.environ["LIGHTLY_DID_VERSION_CHECK"] = "True"
     import multiprocessing
```

### Comparing `lightly-1.5.3/lightly/active_learning/config/selection_config.py` & `lightly-1.5.4/lightly/active_learning/config/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/__init__.py` & `lightly-1.5.4/lightly/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/_version_checking.py` & `lightly-1.5.4/lightly/api/_version_checking.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_artifacts.py` & `lightly-1.5.4/lightly/api/api_workflow_artifacts.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_client.py` & `lightly-1.5.4/lightly/api/api_workflow_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_collaboration.py` & `lightly-1.5.4/lightly/api/api_workflow_collaboration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_compute_worker.py` & `lightly-1.5.4/lightly/api/api_workflow_compute_worker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_datasets.py` & `lightly-1.5.4/lightly/api/api_workflow_datasets.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_datasources.py` & `lightly-1.5.4/lightly/api/api_workflow_datasources.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_download_dataset.py` & `lightly-1.5.4/lightly/api/api_workflow_download_dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_export.py` & `lightly-1.5.4/lightly/api/api_workflow_export.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_predictions.py` & `lightly-1.5.4/lightly/api/api_workflow_predictions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_selection.py` & `lightly-1.5.4/lightly/api/api_workflow_selection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_tags.py` & `lightly-1.5.4/lightly/api/api_workflow_tags.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_upload_embeddings.py` & `lightly-1.5.4/lightly/api/api_workflow_upload_embeddings.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/api_workflow_upload_metadata.py` & `lightly-1.5.4/lightly/api/api_workflow_upload_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/bitmask.py` & `lightly-1.5.4/lightly/api/bitmask.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/download.py` & `lightly-1.5.4/lightly/api/download.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/patch.py` & `lightly-1.5.4/lightly/api/patch.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/swagger_api_client.py` & `lightly-1.5.4/lightly/api/swagger_api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/swagger_rest_client.py` & `lightly-1.5.4/lightly/api/swagger_rest_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/api/utils.py` & `lightly-1.5.4/lightly/api/utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/cli/_cli_simclr.py` & `lightly-1.5.4/lightly/cli/_cli_simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/cli/_helpers.py` & `lightly-1.5.4/lightly/cli/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/cli/config/config.yaml` & `lightly-1.5.4/lightly/cli/config/config.yaml`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/cli/crop_cli.py` & `lightly-1.5.4/lightly/cli/crop_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/cli/download_cli.py` & `lightly-1.5.4/lightly/cli/download_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/cli/embed_cli.py` & `lightly-1.5.4/lightly/cli/embed_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/cli/lightly_cli.py` & `lightly-1.5.4/lightly/cli/lightly_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/cli/serve_cli.py` & `lightly-1.5.4/lightly/cli/serve_cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import sys
 from pathlib import Path
 
 import hydra
 
 from lightly.api import serve
+from lightly.api.serve import validate_input_mount, validate_lightly_mount
 from lightly.cli._helpers import fix_hydra_arguments
 from lightly.utils.hipify import bcolors
 
 
 @hydra.main(**fix_hydra_arguments(config_path="config", config_name="lightly-serve"))
 def lightly_serve(cfg):
     """Use lightly-serve to serve your data for interactive exploration.
@@ -24,23 +25,34 @@
 
     Examples:
         >>> lightly-serve input_mount=data/ lightly_mount=lightly/ port=3456
 
 
     """
     if not cfg.input_mount:
-        print("Please provide a valid input mount. Use --help for more information.")
+        print(
+            "Please provide a valid 'input_mount' argument. Use --help for more "
+            "information."
+        )
         sys.exit(1)
 
     if not cfg.lightly_mount:
-        print("Please provide a valid Lightly mount. Use --help for more information.")
+        print(
+            "Please provide a valid 'lightly_mount' argument. Use --help for more "
+            "information."
+        )
         sys.exit(1)
 
+    input_mount = Path(cfg.input_mount)
+    validate_input_mount(input_mount=input_mount)
+    lightly_mount = Path(cfg.lightly_mount)
+    validate_lightly_mount(lightly_mount=lightly_mount)
+
     httpd = serve.get_server(
-        paths=[Path(cfg.input_mount), Path(cfg.lightly_mount)],
+        paths=[input_mount, lightly_mount],
         host=cfg.host,
         port=cfg.port,
     )
     print(
         f"Starting server, listening at '{bcolors.OKBLUE}{httpd.server_name}:{httpd.server_port}{bcolors.ENDC}'"
     )
     print(
```

### Comparing `lightly-1.5.3/lightly/cli/train_cli.py` & `lightly-1.5.4/lightly/cli/train_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/cli/version_cli.py` & `lightly-1.5.4/lightly/cli/version_cli.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/core.py` & `lightly-1.5.4/lightly/core.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/__init__.py` & `lightly-1.5.4/lightly/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/_helpers.py` & `lightly-1.5.4/lightly/data/_helpers.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/_image.py` & `lightly-1.5.4/lightly/data/_image.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/_image_loaders.py` & `lightly-1.5.4/lightly/data/_image_loaders.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/_utils.py` & `lightly-1.5.4/lightly/data/_utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/_video.py` & `lightly-1.5.4/lightly/data/_video.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/collate.py` & `lightly-1.5.4/lightly/data/collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/dataset.py` & `lightly-1.5.4/lightly/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/lightly_subset.py` & `lightly-1.5.4/lightly/data/lightly_subset.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/data/multi_view_collate.py` & `lightly-1.5.4/lightly/data/multi_view_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/embedding/_base.py` & `lightly-1.5.4/lightly/embedding/_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/embedding/callbacks.py` & `lightly-1.5.4/lightly/embedding/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/embedding/embedding.py` & `lightly-1.5.4/lightly/embedding/embedding.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/__init__.py` & `lightly-1.5.4/lightly/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/barlow_twins_loss.py` & `lightly-1.5.4/lightly/loss/barlow_twins_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/dcl_loss.py` & `lightly-1.5.4/lightly/loss/dcl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/dino_loss.py` & `lightly-1.5.4/lightly/loss/dino_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/emp_ssl_loss.py` & `lightly-1.5.4/lightly/loss/emp_ssl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/hypersphere_loss.py` & `lightly-1.5.4/lightly/loss/hypersphere_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/mmcr_loss.py` & `lightly-1.5.4/lightly/loss/mmcr_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/msn_loss.py` & `lightly-1.5.4/lightly/loss/msn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/negative_cosine_similarity.py` & `lightly-1.5.4/lightly/loss/negative_cosine_similarity.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/ntx_ent_loss.py` & `lightly-1.5.4/lightly/loss/ntx_ent_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/pmsn_loss.py` & `lightly-1.5.4/lightly/loss/pmsn_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/regularizer/co2.py` & `lightly-1.5.4/lightly/loss/regularizer/co2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/swav_loss.py` & `lightly-1.5.4/lightly/loss/swav_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/sym_neg_cos_sim_loss.py` & `lightly-1.5.4/lightly/loss/sym_neg_cos_sim_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/tico_loss.py` & `lightly-1.5.4/lightly/loss/tico_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/vicreg_loss.py` & `lightly-1.5.4/lightly/loss/vicreg_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/vicregl_loss.py` & `lightly-1.5.4/lightly/loss/vicregl_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/loss/wmse_loss.py` & `lightly-1.5.4/lightly/loss/wmse_loss.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/__init__.py` & `lightly-1.5.4/lightly/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/_momentum.py` & `lightly-1.5.4/lightly/models/_momentum.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/barlowtwins.py` & `lightly-1.5.4/lightly/models/barlowtwins.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/batchnorm.py` & `lightly-1.5.4/lightly/models/batchnorm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/byol.py` & `lightly-1.5.4/lightly/models/byol.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/moco.py` & `lightly-1.5.4/lightly/models/moco.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/__init__.py` & `lightly-1.5.4/lightly/models/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/heads.py` & `lightly-1.5.4/lightly/models/modules/heads.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/heads_timm.py` & `lightly-1.5.4/lightly/models/modules/heads_timm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/ijepa.py` & `lightly-1.5.4/lightly/models/modules/ijepa.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/masked_autoencoder.py` & `lightly-1.5.4/lightly/models/modules/masked_autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/masked_autoencoder_timm.py` & `lightly-1.5.4/lightly/models/modules/masked_autoencoder_timm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/masked_causal_vision_transformer.py` & `lightly-1.5.4/lightly/models/modules/masked_causal_vision_transformer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/masked_vision_transformer.py` & `lightly-1.5.4/lightly/models/modules/masked_vision_transformer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/masked_vision_transformer_timm.py` & `lightly-1.5.4/lightly/models/modules/masked_vision_transformer_timm.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/masked_vision_transformer_torchvision.py` & `lightly-1.5.4/lightly/models/modules/masked_vision_transformer_torchvision.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/memory_bank.py` & `lightly-1.5.4/lightly/models/modules/memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/modules/nn_memory_bank.py` & `lightly-1.5.4/lightly/models/modules/nn_memory_bank.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/nnclr.py` & `lightly-1.5.4/lightly/models/nnclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/resnet.py` & `lightly-1.5.4/lightly/models/resnet.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/simclr.py` & `lightly-1.5.4/lightly/models/simclr.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/simsiam.py` & `lightly-1.5.4/lightly/models/simsiam.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/utils.py` & `lightly-1.5.4/lightly/models/utils.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/models/zoo.py` & `lightly-1.5.4/lightly/models/zoo.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/__init__.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 from lightly.openapi_generated.swagger_client.models.selection_config_v3_entry_strategy_all_of import SelectionConfigV3EntryStrategyAllOf
 from lightly.openapi_generated.swagger_client.models.selection_config_v3_entry_strategy_all_of_target_range import SelectionConfigV3EntryStrategyAllOfTargetRange
 from lightly.openapi_generated.swagger_client.models.selection_config_v4 import SelectionConfigV4
 from lightly.openapi_generated.swagger_client.models.selection_config_v4_all_of import SelectionConfigV4AllOf
 from lightly.openapi_generated.swagger_client.models.selection_config_v4_entry import SelectionConfigV4Entry
 from lightly.openapi_generated.swagger_client.models.selection_config_v4_entry_input import SelectionConfigV4EntryInput
 from lightly.openapi_generated.swagger_client.models.selection_config_v4_entry_strategy import SelectionConfigV4EntryStrategy
+from lightly.openapi_generated.swagger_client.models.selection_config_v4_entry_strategy_all_of import SelectionConfigV4EntryStrategyAllOf
 from lightly.openapi_generated.swagger_client.models.selection_input_predictions_name import SelectionInputPredictionsName
 from lightly.openapi_generated.swagger_client.models.selection_input_type import SelectionInputType
 from lightly.openapi_generated.swagger_client.models.selection_strategy_threshold_operation import SelectionStrategyThresholdOperation
 from lightly.openapi_generated.swagger_client.models.selection_strategy_type import SelectionStrategyType
 from lightly.openapi_generated.swagger_client.models.selection_strategy_type_v3 import SelectionStrategyTypeV3
 from lightly.openapi_generated.swagger_client.models.service_account_basic_data import ServiceAccountBasicData
 from lightly.openapi_generated.swagger_client.models.set_embeddings_is_processed_flag_by_id_body_request import SetEmbeddingsIsProcessedFlagByIdBodyRequest
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/__init__.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/collaboration_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/collaboration_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/datasets_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/datasets_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -632,26 +632,28 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_datasets(self, shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> List[DatasetData]:  # noqa: E501
+    def get_datasets(self, shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exclude_playground : Annotated[Optional[StrictBool], Field(description="if set, excludes playground datasets. Typically set to true when querying for team assets")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> List[DatasetData]:  # noqa: E501
         """get_datasets  # noqa: E501
 
         Get all datasets for a user  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_datasets(shared, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
+        >>> thread = api.get_datasets(shared, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
         >>> result = thread.get()
 
         :param shared: if set, only returns the datasets which have been shared with the user
         :type shared: bool
+        :param exclude_playground: if set, excludes playground datasets. Typically set to true when querying for team assets
+        :type exclude_playground: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param page_size: pagination size/limit of the number of samples to return
         :type page_size: int
         :param page_offset: pagination offset
@@ -666,29 +668,31 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[DatasetData]
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the get_datasets_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.get_datasets_with_http_info(shared, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, **kwargs)  # noqa: E501
+        return self.get_datasets_with_http_info(shared, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_datasets_with_http_info(self, shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_datasets_with_http_info(self, shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exclude_playground : Annotated[Optional[StrictBool], Field(description="if set, excludes playground datasets. Typically set to true when querying for team assets")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """get_datasets  # noqa: E501
 
         Get all datasets for a user  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_datasets_with_http_info(shared, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
+        >>> thread = api.get_datasets_with_http_info(shared, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
         >>> result = thread.get()
 
         :param shared: if set, only returns the datasets which have been shared with the user
         :type shared: bool
+        :param exclude_playground: if set, excludes playground datasets. Typically set to true when querying for team assets
+        :type exclude_playground: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param page_size: pagination size/limit of the number of samples to return
         :type page_size: int
         :param page_offset: pagination offset
@@ -718,14 +722,15 @@
         :rtype: tuple(List[DatasetData], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'shared',
+            'exclude_playground',
             'get_assets_of_team',
             'get_assets_of_team_inclusive_self',
             'page_size',
             'page_offset'
         ]
         _all_params.extend(
             [
@@ -758,14 +763,20 @@
         _query_params = []
         if _params.get('shared') is not None:  # noqa: E501
             _query_params.append((
                 'shared',
                 _params['shared'].value if hasattr(_params['shared'], 'value') else _params['shared']
             ))
 
+        if _params.get('exclude_playground') is not None:  # noqa: E501
+            _query_params.append((
+                'excludePlayground',
+                _params['exclude_playground'].value if hasattr(_params['exclude_playground'], 'value') else _params['exclude_playground']
+            ))
+
         if _params.get('get_assets_of_team') is not None:  # noqa: E501
             _query_params.append((
                 'getAssetsOfTeam',
                 _params['get_assets_of_team'].value if hasattr(_params['get_assets_of_team'], 'value') else _params['get_assets_of_team']
             ))
 
         if _params.get('get_assets_of_team_inclusive_self') is not None:  # noqa: E501
@@ -822,28 +833,30 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_datasets_enriched(self, shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, limit : Annotated[Optional[StrictInt], Field(description="DEPRECATED, use pageSize instead. if set, only returns the newest up until limit")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> List[DatasetDataEnriched]:  # noqa: E501
+    def get_datasets_enriched(self, shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, limit : Annotated[Optional[StrictInt], Field(description="DEPRECATED, use pageSize instead. if set, only returns the newest up until limit")] = None, exclude_playground : Annotated[Optional[StrictBool], Field(description="if set, excludes playground datasets. Typically set to true when querying for team assets")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> List[DatasetDataEnriched]:  # noqa: E501
         """get_datasets_enriched  # noqa: E501
 
-        Get all datasets for a user but enriched with additional information as nTags, nEmbeddings, samples  # noqa: E501
+        Get all datasets for a user but enriched with additional information as nTags, nEmbeddings, samples.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_datasets_enriched(shared, limit, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
+        >>> thread = api.get_datasets_enriched(shared, limit, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
         >>> result = thread.get()
 
         :param shared: if set, only returns the datasets which have been shared with the user
         :type shared: bool
         :param limit: DEPRECATED, use pageSize instead. if set, only returns the newest up until limit
         :type limit: int
+        :param exclude_playground: if set, excludes playground datasets. Typically set to true when querying for team assets
+        :type exclude_playground: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param page_size: pagination size/limit of the number of samples to return
         :type page_size: int
         :param page_offset: pagination offset
@@ -858,31 +871,33 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[DatasetDataEnriched]
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the get_datasets_enriched_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.get_datasets_enriched_with_http_info(shared, limit, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, **kwargs)  # noqa: E501
+        return self.get_datasets_enriched_with_http_info(shared, limit, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_datasets_enriched_with_http_info(self, shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, limit : Annotated[Optional[StrictInt], Field(description="DEPRECATED, use pageSize instead. if set, only returns the newest up until limit")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_datasets_enriched_with_http_info(self, shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, limit : Annotated[Optional[StrictInt], Field(description="DEPRECATED, use pageSize instead. if set, only returns the newest up until limit")] = None, exclude_playground : Annotated[Optional[StrictBool], Field(description="if set, excludes playground datasets. Typically set to true when querying for team assets")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """get_datasets_enriched  # noqa: E501
 
-        Get all datasets for a user but enriched with additional information as nTags, nEmbeddings, samples  # noqa: E501
+        Get all datasets for a user but enriched with additional information as nTags, nEmbeddings, samples.   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_datasets_enriched_with_http_info(shared, limit, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
+        >>> thread = api.get_datasets_enriched_with_http_info(shared, limit, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
         >>> result = thread.get()
 
         :param shared: if set, only returns the datasets which have been shared with the user
         :type shared: bool
         :param limit: DEPRECATED, use pageSize instead. if set, only returns the newest up until limit
         :type limit: int
+        :param exclude_playground: if set, excludes playground datasets. Typically set to true when querying for team assets
+        :type exclude_playground: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param page_size: pagination size/limit of the number of samples to return
         :type page_size: int
         :param page_offset: pagination offset
@@ -913,14 +928,15 @@
         """
 
         _params = locals()
 
         _all_params = [
             'shared',
             'limit',
+            'exclude_playground',
             'get_assets_of_team',
             'get_assets_of_team_inclusive_self',
             'page_size',
             'page_offset'
         ]
         _all_params.extend(
             [
@@ -959,14 +975,20 @@
 
         if _params.get('limit') is not None:  # noqa: E501
             _query_params.append((
                 'limit',
                 _params['limit'].value if hasattr(_params['limit'], 'value') else _params['limit']
             ))
 
+        if _params.get('exclude_playground') is not None:  # noqa: E501
+            _query_params.append((
+                'excludePlayground',
+                _params['exclude_playground'].value if hasattr(_params['exclude_playground'], 'value') else _params['exclude_playground']
+            ))
+
         if _params.get('get_assets_of_team') is not None:  # noqa: E501
             _query_params.append((
                 'getAssetsOfTeam',
                 _params['get_assets_of_team'].value if hasattr(_params['get_assets_of_team'], 'value') else _params['get_assets_of_team']
             ))
 
         if _params.get('get_assets_of_team_inclusive_self') is not None:  # noqa: E501
@@ -1170,30 +1192,32 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_datasets_enriched_query_by_name(self, dataset_name : constr(strict=True, min_length=1), shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exact : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which match the name exactly (not just by prefix)")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> List[DatasetDataEnriched]:  # noqa: E501
+    def get_datasets_enriched_query_by_name(self, dataset_name : constr(strict=True, min_length=1), shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exact : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which match the name exactly (not just by prefix)")] = None, exclude_playground : Annotated[Optional[StrictBool], Field(description="if set, excludes playground datasets. Typically set to true when querying for team assets")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> List[DatasetDataEnriched]:  # noqa: E501
         """get_datasets_enriched_query_by_name  # noqa: E501
 
         Query for datasets  enriched with additional information by their name prefix unless exact flag is set  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_datasets_enriched_query_by_name(dataset_name, shared, exact, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
+        >>> thread = api.get_datasets_enriched_query_by_name(dataset_name, shared, exact, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
         >>> result = thread.get()
 
         :param dataset_name: (required)
         :type dataset_name: str
         :param shared: if set, only returns the datasets which have been shared with the user
         :type shared: bool
         :param exact: if set, only returns the datasets which match the name exactly (not just by prefix)
         :type exact: bool
+        :param exclude_playground: if set, excludes playground datasets. Typically set to true when querying for team assets
+        :type exclude_playground: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param page_size: pagination size/limit of the number of samples to return
         :type page_size: int
         :param page_offset: pagination offset
@@ -1208,33 +1232,35 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[DatasetDataEnriched]
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the get_datasets_enriched_query_by_name_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.get_datasets_enriched_query_by_name_with_http_info(dataset_name, shared, exact, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, **kwargs)  # noqa: E501
+        return self.get_datasets_enriched_query_by_name_with_http_info(dataset_name, shared, exact, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_datasets_enriched_query_by_name_with_http_info(self, dataset_name : constr(strict=True, min_length=1), shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exact : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which match the name exactly (not just by prefix)")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_datasets_enriched_query_by_name_with_http_info(self, dataset_name : constr(strict=True, min_length=1), shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exact : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which match the name exactly (not just by prefix)")] = None, exclude_playground : Annotated[Optional[StrictBool], Field(description="if set, excludes playground datasets. Typically set to true when querying for team assets")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """get_datasets_enriched_query_by_name  # noqa: E501
 
         Query for datasets  enriched with additional information by their name prefix unless exact flag is set  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_datasets_enriched_query_by_name_with_http_info(dataset_name, shared, exact, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
+        >>> thread = api.get_datasets_enriched_query_by_name_with_http_info(dataset_name, shared, exact, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
         >>> result = thread.get()
 
         :param dataset_name: (required)
         :type dataset_name: str
         :param shared: if set, only returns the datasets which have been shared with the user
         :type shared: bool
         :param exact: if set, only returns the datasets which match the name exactly (not just by prefix)
         :type exact: bool
+        :param exclude_playground: if set, excludes playground datasets. Typically set to true when querying for team assets
+        :type exclude_playground: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param page_size: pagination size/limit of the number of samples to return
         :type page_size: int
         :param page_offset: pagination offset
@@ -1266,14 +1292,15 @@
 
         _params = locals()
 
         _all_params = [
             'dataset_name',
             'shared',
             'exact',
+            'exclude_playground',
             'get_assets_of_team',
             'get_assets_of_team_inclusive_self',
             'page_size',
             'page_offset'
         ]
         _all_params.extend(
             [
@@ -1315,14 +1342,20 @@
 
         if _params.get('exact') is not None:  # noqa: E501
             _query_params.append((
                 'exact',
                 _params['exact'].value if hasattr(_params['exact'], 'value') else _params['exact']
             ))
 
+        if _params.get('exclude_playground') is not None:  # noqa: E501
+            _query_params.append((
+                'excludePlayground',
+                _params['exclude_playground'].value if hasattr(_params['exclude_playground'], 'value') else _params['exclude_playground']
+            ))
+
         if _params.get('get_assets_of_team') is not None:  # noqa: E501
             _query_params.append((
                 'getAssetsOfTeam',
                 _params['get_assets_of_team'].value if hasattr(_params['get_assets_of_team'], 'value') else _params['get_assets_of_team']
             ))
 
         if _params.get('get_assets_of_team_inclusive_self') is not None:  # noqa: E501
@@ -1379,30 +1412,32 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_datasets_query_by_name(self, dataset_name : constr(strict=True, min_length=1), shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exact : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which match the name exactly (not just by prefix)")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> List[DatasetData]:  # noqa: E501
+    def get_datasets_query_by_name(self, dataset_name : constr(strict=True, min_length=1), shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exact : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which match the name exactly (not just by prefix)")] = None, exclude_playground : Annotated[Optional[StrictBool], Field(description="if set, excludes playground datasets. Typically set to true when querying for team assets")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> List[DatasetData]:  # noqa: E501
         """get_datasets_query_by_name  # noqa: E501
 
         Query for datasets by their name prefix unless exact flag is set  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_datasets_query_by_name(dataset_name, shared, exact, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
+        >>> thread = api.get_datasets_query_by_name(dataset_name, shared, exact, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
         >>> result = thread.get()
 
         :param dataset_name: (required)
         :type dataset_name: str
         :param shared: if set, only returns the datasets which have been shared with the user
         :type shared: bool
         :param exact: if set, only returns the datasets which match the name exactly (not just by prefix)
         :type exact: bool
+        :param exclude_playground: if set, excludes playground datasets. Typically set to true when querying for team assets
+        :type exclude_playground: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param page_size: pagination size/limit of the number of samples to return
         :type page_size: int
         :param page_offset: pagination offset
@@ -1417,33 +1452,35 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[DatasetData]
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the get_datasets_query_by_name_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.get_datasets_query_by_name_with_http_info(dataset_name, shared, exact, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, **kwargs)  # noqa: E501
+        return self.get_datasets_query_by_name_with_http_info(dataset_name, shared, exact, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_datasets_query_by_name_with_http_info(self, dataset_name : constr(strict=True, min_length=1), shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exact : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which match the name exactly (not just by prefix)")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_datasets_query_by_name_with_http_info(self, dataset_name : constr(strict=True, min_length=1), shared : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which have been shared with the user")] = None, exact : Annotated[Optional[StrictBool], Field(description="if set, only returns the datasets which match the name exactly (not just by prefix)")] = None, exclude_playground : Annotated[Optional[StrictBool], Field(description="if set, excludes playground datasets. Typically set to true when querying for team assets")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """get_datasets_query_by_name  # noqa: E501
 
         Query for datasets by their name prefix unless exact flag is set  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_datasets_query_by_name_with_http_info(dataset_name, shared, exact, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
+        >>> thread = api.get_datasets_query_by_name_with_http_info(dataset_name, shared, exact, exclude_playground, get_assets_of_team, get_assets_of_team_inclusive_self, page_size, page_offset, async_req=True)
         >>> result = thread.get()
 
         :param dataset_name: (required)
         :type dataset_name: str
         :param shared: if set, only returns the datasets which have been shared with the user
         :type shared: bool
         :param exact: if set, only returns the datasets which match the name exactly (not just by prefix)
         :type exact: bool
+        :param exclude_playground: if set, excludes playground datasets. Typically set to true when querying for team assets
+        :type exclude_playground: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param page_size: pagination size/limit of the number of samples to return
         :type page_size: int
         :param page_offset: pagination offset
@@ -1475,14 +1512,15 @@
 
         _params = locals()
 
         _all_params = [
             'dataset_name',
             'shared',
             'exact',
+            'exclude_playground',
             'get_assets_of_team',
             'get_assets_of_team_inclusive_self',
             'page_size',
             'page_offset'
         ]
         _all_params.extend(
             [
@@ -1524,14 +1562,20 @@
 
         if _params.get('exact') is not None:  # noqa: E501
             _query_params.append((
                 'exact',
                 _params['exact'].value if hasattr(_params['exact'], 'value') else _params['exact']
             ))
 
+        if _params.get('exclude_playground') is not None:  # noqa: E501
+            _query_params.append((
+                'excludePlayground',
+                _params['exclude_playground'].value if hasattr(_params['exclude_playground'], 'value') else _params['exclude_playground']
+            ))
+
         if _params.get('get_assets_of_team') is not None:  # noqa: E501
             _query_params.append((
                 'getAssetsOfTeam',
                 _params['get_assets_of_team'].value if hasattr(_params['get_assets_of_team'], 'value') else _params['get_assets_of_team']
             ))
 
         if _params.get('get_assets_of_team_inclusive_self') is not None:  # noqa: E501
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/datasources_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/datasources_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/docker_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/docker_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1728,14 +1728,148 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def get_default_or_register_worker(self, **kwargs) -> DockerWorkerRegistryEntryData:  # noqa: E501
+        """get_default_or_register_worker  # noqa: E501
+
+        Return a free default worker or register a new worker if no default worker exists.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_default_or_register_worker(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: DockerWorkerRegistryEntryData
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            raise ValueError("Error! Please call the get_default_or_register_worker_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
+        return self.get_default_or_register_worker_with_http_info(**kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_default_or_register_worker_with_http_info(self, **kwargs) -> ApiResponse:  # noqa: E501
+        """get_default_or_register_worker  # noqa: E501
+
+        Return a free default worker or register a new worker if no default worker exists.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_default_or_register_worker_with_http_info(async_req=True)
+        >>> result = thread.get()
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the 
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(DockerWorkerRegistryEntryData, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_default_or_register_worker" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['auth0Bearer', 'ApiKeyAuth']  # noqa: E501
+
+        _response_types_map = {
+            '200': "DockerWorkerRegistryEntryData",
+            '400': "ApiErrorResponse",
+            '403': "ApiErrorResponse",
+            '404': "ApiErrorResponse",
+        }
+
+        return self.api_client.call_api(
+            '/v1/docker/worker/default', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def get_docker_license_information(self, **kwargs) -> DockerLicenseInformation:  # noqa: E501
         """get_docker_license_information  # noqa: E501
 
         Requests license information to run the container.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
@@ -3430,59 +3564,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_docker_runs_scheduled_by_dataset_id(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], state : Optional[DockerRunScheduledState] = None, **kwargs) -> List[DockerRunScheduledData]:  # noqa: E501
+    def get_docker_runs_scheduled_by_dataset_id(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], state : Optional[DockerRunScheduledState] = None, states : Optional[conlist(DockerRunScheduledState)] = None, **kwargs) -> List[DockerRunScheduledData]:  # noqa: E501
         """get_docker_runs_scheduled_by_dataset_id  # noqa: E501
 
-        Get all scheduled docker runs by dataset id. If no state is specified, returns runs which have not yet finished (neither DONE or CANCELED).  # noqa: E501
+        Get all scheduled docker runs by dataset id. If no state(s) is specified, returns runs which have not yet finished (neither DONE or CANCELED).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_docker_runs_scheduled_by_dataset_id(dataset_id, state, async_req=True)
+        >>> thread = api.get_docker_runs_scheduled_by_dataset_id(dataset_id, state, states, async_req=True)
         >>> result = thread.get()
 
         :param dataset_id: ObjectId of the dataset (required)
         :type dataset_id: str
         :param state:
         :type state: DockerRunScheduledState
+        :param states:
+        :type states: List[DockerRunScheduledState]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[DockerRunScheduledData]
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the get_docker_runs_scheduled_by_dataset_id_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.get_docker_runs_scheduled_by_dataset_id_with_http_info(dataset_id, state, **kwargs)  # noqa: E501
+        return self.get_docker_runs_scheduled_by_dataset_id_with_http_info(dataset_id, state, states, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_docker_runs_scheduled_by_dataset_id_with_http_info(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], state : Optional[DockerRunScheduledState] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_docker_runs_scheduled_by_dataset_id_with_http_info(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], state : Optional[DockerRunScheduledState] = None, states : Optional[conlist(DockerRunScheduledState)] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """get_docker_runs_scheduled_by_dataset_id  # noqa: E501
 
-        Get all scheduled docker runs by dataset id. If no state is specified, returns runs which have not yet finished (neither DONE or CANCELED).  # noqa: E501
+        Get all scheduled docker runs by dataset id. If no state(s) is specified, returns runs which have not yet finished (neither DONE or CANCELED).  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_docker_runs_scheduled_by_dataset_id_with_http_info(dataset_id, state, async_req=True)
+        >>> thread = api.get_docker_runs_scheduled_by_dataset_id_with_http_info(dataset_id, state, states, async_req=True)
         >>> result = thread.get()
 
         :param dataset_id: ObjectId of the dataset (required)
         :type dataset_id: str
         :param state:
         :type state: DockerRunScheduledState
+        :param states:
+        :type states: List[DockerRunScheduledState]
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
         :type _preload_content: bool, optional
@@ -3504,15 +3642,16 @@
         :rtype: tuple(List[DockerRunScheduledData], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'dataset_id',
-            'state'
+            'state',
+            'states'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -3544,14 +3683,21 @@
         _query_params = []
         if _params.get('state') is not None:  # noqa: E501
             _query_params.append((
                 'state',
                 _params['state'].value if hasattr(_params['state'], 'value') else _params['state']
             ))
 
+        if _params.get('states') is not None:  # noqa: E501
+            _query_params.append((
+                'states',
+                _params['states'].value if hasattr(_params['states'], 'value') else _params['states']
+            ))
+            _collection_formats['states'] = 'multi'
+
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
         # process the form parameters
         _form_params = []
         _files = {}
         # process the body parameter
         _body_params = None
@@ -3583,30 +3729,32 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_docker_runs_scheduled_by_state_and_labels(self, state : Optional[DockerRunScheduledState] = None, labels : Optional[conlist(StrictStr)] = None, version : Optional[StrictStr] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, **kwargs) -> List[DockerRunScheduledData]:  # noqa: E501
+    def get_docker_runs_scheduled_by_state_and_labels(self, state : Optional[DockerRunScheduledState] = None, labels : Optional[conlist(StrictStr)] = None, version : Optional[StrictStr] = None, include_unlockable_runs : Annotated[Optional[StrictBool], Field(description="Unlockable runs are runs which can't be locked due to e.g another run with the same datasetId being locked/processed. This safeguards two workers processing the same dataset. Only has an effect if querying for runs with state=OPEN ")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, **kwargs) -> List[DockerRunScheduledData]:  # noqa: E501
         """get_docker_runs_scheduled_by_state_and_labels  # noqa: E501
 
         Get all scheduled docker runs of the user. Additionally, you can filter by state.  Furthermore, you can filter by only providing labels and only return scheduled runs whose runsOn labels are included in the provided labels. Runs are filtered by the provided version parameter. Version parameter set to * returns all configs   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_docker_runs_scheduled_by_state_and_labels(state, labels, version, get_assets_of_team, get_assets_of_team_inclusive_self, async_req=True)
+        >>> thread = api.get_docker_runs_scheduled_by_state_and_labels(state, labels, version, include_unlockable_runs, get_assets_of_team, get_assets_of_team_inclusive_self, async_req=True)
         >>> result = thread.get()
 
         :param state:
         :type state: DockerRunScheduledState
         :param labels:
         :type labels: List[str]
         :param version:
         :type version: str
+        :param include_unlockable_runs: Unlockable runs are runs which can't be locked due to e.g another run with the same datasetId being locked/processed. This safeguards two workers processing the same dataset. Only has an effect if querying for runs with state=OPEN 
+        :type include_unlockable_runs: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -3617,33 +3765,35 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[DockerRunScheduledData]
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the get_docker_runs_scheduled_by_state_and_labels_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.get_docker_runs_scheduled_by_state_and_labels_with_http_info(state, labels, version, get_assets_of_team, get_assets_of_team_inclusive_self, **kwargs)  # noqa: E501
+        return self.get_docker_runs_scheduled_by_state_and_labels_with_http_info(state, labels, version, include_unlockable_runs, get_assets_of_team, get_assets_of_team_inclusive_self, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_docker_runs_scheduled_by_state_and_labels_with_http_info(self, state : Optional[DockerRunScheduledState] = None, labels : Optional[conlist(StrictStr)] = None, version : Optional[StrictStr] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_docker_runs_scheduled_by_state_and_labels_with_http_info(self, state : Optional[DockerRunScheduledState] = None, labels : Optional[conlist(StrictStr)] = None, version : Optional[StrictStr] = None, include_unlockable_runs : Annotated[Optional[StrictBool], Field(description="Unlockable runs are runs which can't be locked due to e.g another run with the same datasetId being locked/processed. This safeguards two workers processing the same dataset. Only has an effect if querying for runs with state=OPEN ")] = None, get_assets_of_team : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user")] = None, get_assets_of_team_inclusive_self : Annotated[Optional[StrictBool], Field(description="if this flag is true, we get the relevant asset of the team of the user including the assets of the user")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """get_docker_runs_scheduled_by_state_and_labels  # noqa: E501
 
         Get all scheduled docker runs of the user. Additionally, you can filter by state.  Furthermore, you can filter by only providing labels and only return scheduled runs whose runsOn labels are included in the provided labels. Runs are filtered by the provided version parameter. Version parameter set to * returns all configs   # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_docker_runs_scheduled_by_state_and_labels_with_http_info(state, labels, version, get_assets_of_team, get_assets_of_team_inclusive_self, async_req=True)
+        >>> thread = api.get_docker_runs_scheduled_by_state_and_labels_with_http_info(state, labels, version, include_unlockable_runs, get_assets_of_team, get_assets_of_team_inclusive_self, async_req=True)
         >>> result = thread.get()
 
         :param state:
         :type state: DockerRunScheduledState
         :param labels:
         :type labels: List[str]
         :param version:
         :type version: str
+        :param include_unlockable_runs: Unlockable runs are runs which can't be locked due to e.g another run with the same datasetId being locked/processed. This safeguards two workers processing the same dataset. Only has an effect if querying for runs with state=OPEN 
+        :type include_unlockable_runs: bool
         :param get_assets_of_team: if this flag is true, we get the relevant asset of the team of the user rather than the assets of the user
         :type get_assets_of_team: bool
         :param get_assets_of_team_inclusive_self: if this flag is true, we get the relevant asset of the team of the user including the assets of the user
         :type get_assets_of_team_inclusive_self: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
@@ -3671,14 +3821,15 @@
 
         _params = locals()
 
         _all_params = [
             'state',
             'labels',
             'version',
+            'include_unlockable_runs',
             'get_assets_of_team',
             'get_assets_of_team_inclusive_self'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
@@ -3722,14 +3873,20 @@
 
         if _params.get('version') is not None:  # noqa: E501
             _query_params.append((
                 'version',
                 _params['version'].value if hasattr(_params['version'], 'value') else _params['version']
             ))
 
+        if _params.get('include_unlockable_runs') is not None:  # noqa: E501
+            _query_params.append((
+                'includeUnlockableRuns',
+                _params['include_unlockable_runs'].value if hasattr(_params['include_unlockable_runs'], 'value') else _params['include_unlockable_runs']
+            ))
+
         if _params.get('get_assets_of_team') is not None:  # noqa: E501
             _query_params.append((
                 'getAssetsOfTeam',
                 _params['get_assets_of_team'].value if hasattr(_params['get_assets_of_team'], 'value') else _params['get_assets_of_team']
             ))
 
         if _params.get('get_assets_of_team_inclusive_self') is not None:  # noqa: E501
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/embeddings2d_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/embeddings_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/embeddings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/jobs_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/mappings_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/mappings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/meta_data_configurations_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/predictions_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/predictions_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import re  # noqa: F401
 import io
 import warnings
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, conint, conlist, constr, validator
+from pydantic import Field, StrictBool, conint, conlist, constr, validator
 
 from typing import List, Optional
 
 from lightly.openapi_generated.swagger_client.models.create_entity_response import CreateEntityResponse
 from lightly.openapi_generated.swagger_client.models.prediction_singleton import PredictionSingleton
 from lightly.openapi_generated.swagger_client.models.prediction_task_schema import PredictionTaskSchema
 from lightly.openapi_generated.swagger_client.models.prediction_task_schemas import PredictionTaskSchemas
@@ -707,28 +707,34 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_predictions_by_dataset_id(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], prediction_uuid_timestamp : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Deprecated, currently ignored. The timestamp of when the actual predictions were created. This is used as a peg to version predictions. E.g one could upload predictions on day 1 and then create new predictions with an improved model on day 30. One can then upload the new predictions to the same dataset. ")] = None, task_name : Annotated[Optional[constr(strict=True, min_length=1)], Field(description="If provided, only gets all prediction singletons of all samples of a dataset that were yielded by a specific prediction task name")] = None, **kwargs) -> List[List]:  # noqa: E501
+    def get_predictions_by_dataset_id(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], prediction_uuid_timestamp : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Deprecated, currently ignored. The timestamp of when the actual predictions were created. This is used as a peg to version predictions. E.g one could upload predictions on day 1 and then create new predictions with an improved model on day 30. One can then upload the new predictions to the same dataset. ")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, lean : Annotated[Optional[StrictBool], Field(description="if lean is set to true, all prediction singletons are returned without their \"heavy\" part. This is useful for large datasets where the full prediction singletons are not needed. e.g SEGMENTATION does not need to return the RLE ")] = None, task_name : Annotated[Optional[constr(strict=True, min_length=1)], Field(description="If provided, only gets all prediction singletons of all samples of a dataset that were yielded by a specific prediction task name")] = None, **kwargs) -> List[List]:  # noqa: E501
         """get_predictions_by_dataset_id  # noqa: E501
 
         Get all prediction singletons of all samples of a dataset ordered by the sample mapping  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_predictions_by_dataset_id(dataset_id, prediction_uuid_timestamp, task_name, async_req=True)
+        >>> thread = api.get_predictions_by_dataset_id(dataset_id, prediction_uuid_timestamp, page_size, page_offset, lean, task_name, async_req=True)
         >>> result = thread.get()
 
         :param dataset_id: ObjectId of the dataset (required)
         :type dataset_id: str
         :param prediction_uuid_timestamp: Deprecated, currently ignored. The timestamp of when the actual predictions were created. This is used as a peg to version predictions. E.g one could upload predictions on day 1 and then create new predictions with an improved model on day 30. One can then upload the new predictions to the same dataset. 
         :type prediction_uuid_timestamp: int
+        :param page_size: pagination size/limit of the number of samples to return
+        :type page_size: int
+        :param page_offset: pagination offset
+        :type page_offset: int
+        :param lean: if lean is set to true, all prediction singletons are returned without their \"heavy\" part. This is useful for large datasets where the full prediction singletons are not needed. e.g SEGMENTATION does not need to return the RLE 
+        :type lean: bool
         :param task_name: If provided, only gets all prediction singletons of all samples of a dataset that were yielded by a specific prediction task name
         :type task_name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
@@ -737,31 +743,37 @@
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: List[List]
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the get_predictions_by_dataset_id_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
-        return self.get_predictions_by_dataset_id_with_http_info(dataset_id, prediction_uuid_timestamp, task_name, **kwargs)  # noqa: E501
+        return self.get_predictions_by_dataset_id_with_http_info(dataset_id, prediction_uuid_timestamp, page_size, page_offset, lean, task_name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_predictions_by_dataset_id_with_http_info(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], prediction_uuid_timestamp : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Deprecated, currently ignored. The timestamp of when the actual predictions were created. This is used as a peg to version predictions. E.g one could upload predictions on day 1 and then create new predictions with an improved model on day 30. One can then upload the new predictions to the same dataset. ")] = None, task_name : Annotated[Optional[constr(strict=True, min_length=1)], Field(description="If provided, only gets all prediction singletons of all samples of a dataset that were yielded by a specific prediction task name")] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def get_predictions_by_dataset_id_with_http_info(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], prediction_uuid_timestamp : Annotated[Optional[conint(strict=True, ge=0)], Field(description="Deprecated, currently ignored. The timestamp of when the actual predictions were created. This is used as a peg to version predictions. E.g one could upload predictions on day 1 and then create new predictions with an improved model on day 30. One can then upload the new predictions to the same dataset. ")] = None, page_size : Annotated[Optional[conint(strict=True, ge=1)], Field(description="pagination size/limit of the number of samples to return")] = None, page_offset : Annotated[Optional[conint(strict=True, ge=0)], Field(description="pagination offset")] = None, lean : Annotated[Optional[StrictBool], Field(description="if lean is set to true, all prediction singletons are returned without their \"heavy\" part. This is useful for large datasets where the full prediction singletons are not needed. e.g SEGMENTATION does not need to return the RLE ")] = None, task_name : Annotated[Optional[constr(strict=True, min_length=1)], Field(description="If provided, only gets all prediction singletons of all samples of a dataset that were yielded by a specific prediction task name")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """get_predictions_by_dataset_id  # noqa: E501
 
         Get all prediction singletons of all samples of a dataset ordered by the sample mapping  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_predictions_by_dataset_id_with_http_info(dataset_id, prediction_uuid_timestamp, task_name, async_req=True)
+        >>> thread = api.get_predictions_by_dataset_id_with_http_info(dataset_id, prediction_uuid_timestamp, page_size, page_offset, lean, task_name, async_req=True)
         >>> result = thread.get()
 
         :param dataset_id: ObjectId of the dataset (required)
         :type dataset_id: str
         :param prediction_uuid_timestamp: Deprecated, currently ignored. The timestamp of when the actual predictions were created. This is used as a peg to version predictions. E.g one could upload predictions on day 1 and then create new predictions with an improved model on day 30. One can then upload the new predictions to the same dataset. 
         :type prediction_uuid_timestamp: int
+        :param page_size: pagination size/limit of the number of samples to return
+        :type page_size: int
+        :param page_offset: pagination offset
+        :type page_offset: int
+        :param lean: if lean is set to true, all prediction singletons are returned without their \"heavy\" part. This is useful for large datasets where the full prediction singletons are not needed. e.g SEGMENTATION does not need to return the RLE 
+        :type lean: bool
         :param task_name: If provided, only gets all prediction singletons of all samples of a dataset that were yielded by a specific prediction task name
         :type task_name: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
@@ -786,14 +798,17 @@
         """
 
         _params = locals()
 
         _all_params = [
             'dataset_id',
             'prediction_uuid_timestamp',
+            'page_size',
+            'page_offset',
+            'lean',
             'task_name'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -826,14 +841,32 @@
         _query_params = []
         if _params.get('prediction_uuid_timestamp') is not None:  # noqa: E501
             _query_params.append((
                 'predictionUUIDTimestamp',
                 _params['prediction_uuid_timestamp'].value if hasattr(_params['prediction_uuid_timestamp'], 'value') else _params['prediction_uuid_timestamp']
             ))
 
+        if _params.get('page_size') is not None:  # noqa: E501
+            _query_params.append((
+                'pageSize',
+                _params['page_size'].value if hasattr(_params['page_size'], 'value') else _params['page_size']
+            ))
+
+        if _params.get('page_offset') is not None:  # noqa: E501
+            _query_params.append((
+                'pageOffset',
+                _params['page_offset'].value if hasattr(_params['page_offset'], 'value') else _params['page_offset']
+            ))
+
+        if _params.get('lean') is not None:  # noqa: E501
+            _query_params.append((
+                'lean',
+                _params['lean'].value if hasattr(_params['lean'], 'value') else _params['lean']
+            ))
+
         if _params.get('task_name') is not None:  # noqa: E501
             _query_params.append((
                 'taskName',
                 _params['task_name'].value if hasattr(_params['task_name'], 'value') else _params['task_name']
             ))
 
         # process the header parameters
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/quota_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/quota_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/samples_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/samples_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1523,15 +1523,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_sample_by_id(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], sample_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the sample")], sample_update_request : Annotated[SampleUpdateRequest, Field(..., description="The updated sample to set")], enable_dataset_update : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
+    def update_sample_by_id(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], sample_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the sample")], sample_update_request : Annotated[SampleUpdateRequest, Field(..., description="The updated sample to set")], enable_dataset_update : Annotated[Optional[StrictBool], Field(description="Deprecated, is ignored! If we should also update the dataset with the new sample information (like total size)")] = None, **kwargs) -> None:  # noqa: E501
         """update_sample_by_id  # noqa: E501
 
         update a specific sample of a dataset  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_sample_by_id(dataset_id, sample_id, sample_update_request, enable_dataset_update, async_req=True)
@@ -1539,15 +1539,15 @@
 
         :param dataset_id: ObjectId of the dataset (required)
         :type dataset_id: str
         :param sample_id: ObjectId of the sample (required)
         :type sample_id: str
         :param sample_update_request: The updated sample to set (required)
         :type sample_update_request: SampleUpdateRequest
-        :param enable_dataset_update:
+        :param enable_dataset_update: Deprecated, is ignored! If we should also update the dataset with the new sample information (like total size)
         :type enable_dataset_update: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1558,15 +1558,15 @@
         """
         kwargs['_return_http_data_only'] = True
         if '_preload_content' in kwargs:
             raise ValueError("Error! Please call the update_sample_by_id_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data")
         return self.update_sample_by_id_with_http_info(dataset_id, sample_id, sample_update_request, enable_dataset_update, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_sample_by_id_with_http_info(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], sample_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the sample")], sample_update_request : Annotated[SampleUpdateRequest, Field(..., description="The updated sample to set")], enable_dataset_update : Optional[StrictBool] = None, **kwargs) -> ApiResponse:  # noqa: E501
+    def update_sample_by_id_with_http_info(self, dataset_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the dataset")], sample_id : Annotated[constr(strict=True), Field(..., description="ObjectId of the sample")], sample_update_request : Annotated[SampleUpdateRequest, Field(..., description="The updated sample to set")], enable_dataset_update : Annotated[Optional[StrictBool], Field(description="Deprecated, is ignored! If we should also update the dataset with the new sample information (like total size)")] = None, **kwargs) -> ApiResponse:  # noqa: E501
         """update_sample_by_id  # noqa: E501
 
         update a specific sample of a dataset  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.update_sample_by_id_with_http_info(dataset_id, sample_id, sample_update_request, enable_dataset_update, async_req=True)
@@ -1574,15 +1574,15 @@
 
         :param dataset_id: ObjectId of the dataset (required)
         :type dataset_id: str
         :param sample_id: ObjectId of the sample (required)
         :type sample_id: str
         :param sample_update_request: The updated sample to set (required)
         :type sample_update_request: SampleUpdateRequest
-        :param enable_dataset_update:
+        :param enable_dataset_update: Deprecated, is ignored! If we should also update the dataset with the new sample information (like total size)
         :type enable_dataset_update: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the ApiResponse.data will
                                  be set to none and raw_data will store the 
                                  HTTP response body without reading/decoding.
                                  Default is True.
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/samplings_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/samplings_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/scores_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/scores_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/tags_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/tags_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/teams_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/teams_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api/versioning_api.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api/versioning_api.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api_client.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/api_response.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/api_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/configuration.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/exceptions.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/__init__.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,15 @@
 from lightly.openapi_generated.swagger_client.models.selection_config_v3_entry_strategy_all_of import SelectionConfigV3EntryStrategyAllOf
 from lightly.openapi_generated.swagger_client.models.selection_config_v3_entry_strategy_all_of_target_range import SelectionConfigV3EntryStrategyAllOfTargetRange
 from lightly.openapi_generated.swagger_client.models.selection_config_v4 import SelectionConfigV4
 from lightly.openapi_generated.swagger_client.models.selection_config_v4_all_of import SelectionConfigV4AllOf
 from lightly.openapi_generated.swagger_client.models.selection_config_v4_entry import SelectionConfigV4Entry
 from lightly.openapi_generated.swagger_client.models.selection_config_v4_entry_input import SelectionConfigV4EntryInput
 from lightly.openapi_generated.swagger_client.models.selection_config_v4_entry_strategy import SelectionConfigV4EntryStrategy
+from lightly.openapi_generated.swagger_client.models.selection_config_v4_entry_strategy_all_of import SelectionConfigV4EntryStrategyAllOf
 from lightly.openapi_generated.swagger_client.models.selection_input_predictions_name import SelectionInputPredictionsName
 from lightly.openapi_generated.swagger_client.models.selection_input_type import SelectionInputType
 from lightly.openapi_generated.swagger_client.models.selection_strategy_threshold_operation import SelectionStrategyThresholdOperation
 from lightly.openapi_generated.swagger_client.models.selection_strategy_type import SelectionStrategyType
 from lightly.openapi_generated.swagger_client.models.selection_strategy_type_v3 import SelectionStrategyTypeV3
 from lightly.openapi_generated.swagger_client.models.service_account_basic_data import ServiceAccountBasicData
 from lightly.openapi_generated.swagger_client.models.set_embeddings_is_processed_flag_by_id_body_request import SetEmbeddingsIsProcessedFlagByIdBodyRequest
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/active_learning_score_types_v2_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_types_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/active_learning_score_v2_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/active_learning_score_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/api_error_code.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/api_error_code.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/api_error_response.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/api_error_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/async_task_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/async_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request_user.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/auth0_on_sign_up_request_user.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/configuration_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/configuration_entry.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/configuration_set_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_set_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/configuration_value_data_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_cf_bucket_activity_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_cf_bucket_activity_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_entity_response.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_entity_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_sample_with_write_urls_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/create_team_membership_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/create_team_membership_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/creator.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/crop_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/crop_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_creator.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_data_enriched.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dataset_update_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dataset_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_azure_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_azure_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_base.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_base_full_path.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_base_full_path.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_gcs_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_gcs_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_local.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_local.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_local_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_local_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_obs_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_obs_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_s3_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class DatasourceConfigS3DelegatedAccess(DatasourceConfigBase):
     """
     DatasourceConfigS3DelegatedAccess
     """
     full_path: StrictStr = Field(..., alias="fullPath", description="path includes the bucket name and the path within the bucket where you have stored your information")
     s3_region: S3Region = Field(..., alias="s3Region")
-    s3_external_id: constr(strict=True, min_length=10) = Field(..., alias="s3ExternalId", description="The external ID specified when creating the role.")
+    s3_external_id: constr(strict=True, min_length=10) = Field(..., alias="s3ExternalId", description="The external ID specified when creating the role. More information can be found here: - https://docs.aws.amazon.com/IAM/latest/UserGuide/confused-deputy.html - https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_iam-condition-keys.html#ck_externalid ")
     s3_arn: constr(strict=True, min_length=12) = Field(..., alias="s3ARN", description="The ARN of the role you created")
     s3_server_side_encryption_kms_key: Optional[constr(strict=True, min_length=1)] = Field(None, alias="s3ServerSideEncryptionKMSKey", description="If set, Lightly Worker will automatically set the headers to use server side encryption https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingKMSEncryption.html with this value as the appropriate KMS key arn. This will encrypt the files created by Lightly (crops, frames, thumbnails) in the S3 bucket. ")
     __properties = ["id", "purpose", "type", "thumbSuffix", "fullPath", "s3Region", "s3ExternalId", "s3ARN", "s3ServerSideEncryptionKMSKey"]
 
     @validator('s3_external_id')
     def s3_external_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_s3_delegated_access_all_of.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from lightly.openapi_generated.swagger_client.models.s3_region import S3Region
 
 class DatasourceConfigS3DelegatedAccessAllOf(BaseModel):
     """
     DatasourceConfigS3DelegatedAccessAllOf
     """
     s3_region: S3Region = Field(..., alias="s3Region")
-    s3_external_id: constr(strict=True, min_length=10) = Field(..., alias="s3ExternalId", description="The external ID specified when creating the role.")
+    s3_external_id: constr(strict=True, min_length=10) = Field(..., alias="s3ExternalId", description="The external ID specified when creating the role. More information can be found here: - https://docs.aws.amazon.com/IAM/latest/UserGuide/confused-deputy.html - https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_iam-condition-keys.html#ck_externalid ")
     s3_arn: constr(strict=True, min_length=12) = Field(..., alias="s3ARN", description="The ARN of the role you created")
     s3_server_side_encryption_kms_key: Optional[constr(strict=True, min_length=1)] = Field(None, alias="s3ServerSideEncryptionKMSKey", description="If set, Lightly Worker will automatically set the headers to use server side encryption https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingKMSEncryption.html with this value as the appropriate KMS key arn. This will encrypt the files created by Lightly (crops, frames, thumbnails) in the S3 bucket. ")
     __properties = ["s3Region", "s3ExternalId", "s3ARN", "s3ServerSideEncryptionKMSKey"]
 
     @validator('s3_external_id')
     def s3_external_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_config_verify_data_errors.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_processed_until_timestamp_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_purpose.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_purpose.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_metadata_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/datasource_raw_samples_predictions_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/delegated_access_external_ids_inner.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/delegated_access_external_ids_inner.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from typing import Optional
 from pydantic import Extra,  BaseModel, Field, StrictStr, constr, validator
 
 class DelegatedAccessExternalIdsInner(BaseModel):
     """
     DelegatedAccessExternalIdsInner
     """
-    external_id: constr(strict=True, min_length=10) = Field(..., alias="externalId", description="The external ID specified when creating the role.")
+    external_id: constr(strict=True, min_length=10) = Field(..., alias="externalId", description="The external ID specified when creating the role. More information can be found here: - https://docs.aws.amazon.com/IAM/latest/UserGuide/confused-deputy.html - https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_iam-condition-keys.html#ck_externalid ")
     user_id: Optional[StrictStr] = Field(None, alias="userId")
     team_id: Optional[StrictStr] = Field(None, alias="teamId")
     __properties = ["externalId", "userId", "teamId"]
 
     @validator('external_id')
     def external_id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/dimensionality_reduction_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_authorization_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_authorization_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_authorization_response.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_authorization_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_license_information.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_license_information.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_created_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_storage_location.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_storage_location.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_artifact_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_create_entry_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_create_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_docker_load.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_docker_load.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data_base.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_entry_data_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_log_level.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,17 +28,18 @@
     DockerRunLogLevel
     """
 
     """
     allowed enum values
     """
     VERBOSE = 'VERBOSE'
+    NOTSET = 'NOTSET'
     DEBUG = 'DEBUG'
     INFO = 'INFO'
-    WARN = 'WARN'
+    WARNING = 'WARNING'
     ERROR = 'ERROR'
     CRITICAL = 'CRITICAL'
 
     @classmethod
     def from_json(cls, json_str: str) -> 'DockerRunLogLevel':
         """Create an instance of DockerRunLogLevel from a JSON string"""
         return DockerRunLogLevel(json.loads(json_str))
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_priority.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_scheduled_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_state.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_state.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 
     """
     allowed enum values
     """
     STARTED = 'STARTED'
     INITIALIZING = 'INITIALIZING'
     LOADING_DATASET = 'LOADING_DATASET'
+    LOADING_METADATA = 'LOADING_METADATA'
     LOADING_PREDICTION = 'LOADING_PREDICTION'
     CHECKING_CORRUPTNESS = 'CHECKING_CORRUPTNESS'
     INITIALIZING_OBJECT_CROPS = 'INITIALIZING_OBJECT_CROPS'
-    LOADING_METADATA = 'LOADING_METADATA'
     COMPUTING_METADATA = 'COMPUTING_METADATA'
     TRAINING = 'TRAINING'
     EMBEDDING = 'EMBEDDING'
     EMBEDDING_OBJECT_CROPS = 'EMBEDDING_OBJECT_CROPS'
     PRETAGGING = 'PRETAGGING'
     COMPUTING_ACTIVE_LEARNING_SCORES = 'COMPUTING_ACTIVE_LEARNING_SCORES'
     SAMPLING = 'SAMPLING'
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_run_update_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,24 +16,25 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import Extra,  BaseModel, Field, StrictStr
+from pydantic import Extra,  BaseModel, Field, StrictStr, conint
 from lightly.openapi_generated.swagger_client.models.docker_run_state import DockerRunState
 
 class DockerRunUpdateRequest(BaseModel):
     """
     DockerRunUpdateRequest
     """
     state: DockerRunState = Field(...)
     message: Optional[StrictStr] = None
-    __properties = ["state", "message"]
+    ts: Optional[conint(strict=True, ge=0)] = Field(None, description="unix timestamp in milliseconds")
+    __properties = ["state", "message", "ts"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
         use_enum_values = True
         extra = Extra.forbid
@@ -71,11 +72,12 @@
         # raise errors for additional fields in the input
         for _key in obj.keys():
             if _key not in cls.__properties:
                 raise ValueError("Error due to additional fields (not defined in DockerRunUpdateRequest) in the input: " + str(obj))
 
         _obj = DockerRunUpdateRequest.parse_obj({
             "state": obj.get("state"),
-            "message": obj.get("message")
+            "message": obj.get("message"),
+            "ts": obj.get("ts")
         })
         return _obj
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_task_description.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_task_description.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_user_stats.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_user_stats.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_authorization_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_authorization_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v2_create_request_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v3_create_request_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_v4_create_request_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request_base.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_omni_vx_create_request_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v0_data_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_data_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_datasource.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_datasource.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_object_level.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_docker_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v2_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_data_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_datasource_input_expiration.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_datasource_input_expiration.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_corruptness_check.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_datasource.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_docker_training.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_checkpoint_callback.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_collate.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_criterion.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_loader.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_model.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_optimizer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v3_lightly_trainer.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_data_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_docker.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_v4_docker.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data_base.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_config_vx_data_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_registry_entry_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import Extra,  BaseModel, Field, StrictStr, conint, conlist, constr, validator
+from pydantic import Extra,  BaseModel, Field, StrictBool, StrictStr, conint, conlist, constr, validator
 from lightly.openapi_generated.swagger_client.models.docker_worker_state import DockerWorkerState
 from lightly.openapi_generated.swagger_client.models.docker_worker_type import DockerWorkerType
 
 class DockerWorkerRegistryEntryData(BaseModel):
     """
     DockerWorkerRegistryEntryData
     """
@@ -32,16 +32,17 @@
     user_id: StrictStr = Field(..., alias="userId")
     name: constr(strict=True, min_length=3) = Field(...)
     worker_type: DockerWorkerType = Field(..., alias="workerType")
     state: DockerWorkerState = Field(...)
     created_at: conint(strict=True, ge=0) = Field(..., alias="createdAt", description="unix timestamp in milliseconds")
     last_modified_at: conint(strict=True, ge=0) = Field(..., alias="lastModifiedAt", description="unix timestamp in milliseconds")
     labels: conlist(StrictStr) = Field(..., description="The labels used for specifying the run-worker-relationship")
+    is_default: StrictBool = Field(..., alias="isDefault", description="If true, this worker was created by the API/System and not by a user. ")
     docker_version: Optional[StrictStr] = Field(None, alias="dockerVersion")
-    __properties = ["id", "userId", "name", "workerType", "state", "createdAt", "lastModifiedAt", "labels", "dockerVersion"]
+    __properties = ["id", "userId", "name", "workerType", "state", "createdAt", "lastModifiedAt", "labels", "isDefault", "dockerVersion"]
 
     @validator('id')
     def id_validate_regular_expression(cls, value):
         """Validates the regular expression"""
         if not re.match(r"^[a-f0-9]{24}$", value):
             raise ValueError(r"must validate the regular expression /^[a-f0-9]{24}$/")
         return value
@@ -100,11 +101,12 @@
             "user_id": obj.get("userId"),
             "name": obj.get("name"),
             "worker_type": obj.get("workerType"),
             "state": obj.get("state"),
             "created_at": obj.get("createdAt"),
             "last_modified_at": obj.get("lastModifiedAt"),
             "labels": obj.get("labels"),
+            "is_default": obj.get("isDefault") if obj.get("isDefault") is not None else False,
             "docker_version": obj.get("dockerVersion")
         })
         return _obj
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_state.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/docker_worker_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/docker_worker_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding2d_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/embedding2d_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding2d_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/embedding_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/embedding_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/expiry_handling_strategy_v3.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/expiry_handling_strategy_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/file_name_format.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/file_name_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/file_output_format.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/file_output_format.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/filename_and_read_url.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/image_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/image_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/initial_tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/internal_debug_latency.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/internal_debug_latency.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/internal_debug_latency_mongodb.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/internal_debug_latency_mongodb.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_result_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_result_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_state.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_state.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_status_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_status_data_result.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_data_result.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_status_meta.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_meta.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/job_status_upload_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/jobs_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/jobs_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/label_box_data_row.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_box_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_box_v4_data_row.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/label_studio_task.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_studio_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/label_studio_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_docker_selection_method.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_docker_selection_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_model_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_model_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v2.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/lightly_trainer_precision_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_classification_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_instance_segmentation_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_keypoint_detection_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_object_detection_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_singleton_semantic_segmentation_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_base.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_category_keypoints_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_keypoint_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schema_simple_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/prediction_task_schemas.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/prediction_task_schemas.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/profile_basic_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/profile_me_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_me_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/profile_me_data_settings.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/profile_me_data_settings.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/questionnaire_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/questionnaire_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/s3_region.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/s3_region.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sama_task.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sama_task.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sama_task_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sama_task_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_data_modes.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_data_modes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_meta_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_meta_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_partial_mode.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_sort_by.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_sort_by.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_update_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sample_write_urls.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sample_write_urls.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sampling_config.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_config_stopping_condition.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sampling_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sampling_method.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sampling_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/sector.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/sector.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_base.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_base.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_entry.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_entry_strategy.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_input.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     SelectionConfigV3EntryStrategy
     """
     type: SelectionStrategyTypeV3 = Field(...)
     stopping_condition_minimum_distance: Optional[Union[StrictFloat, StrictInt]] = None
     threshold: Optional[Union[StrictFloat, StrictInt]] = None
     operation: Optional[SelectionStrategyThresholdOperation] = None
     target: Optional[Dict[str, Any]] = None
-    num_nearest_neighbors: Optional[Union[confloat(ge=2, strict=True), conint(ge=2, strict=True)]] = Field(None, alias="numNearestNeighbors", description="It is the number of nearest datapoints used to compute the typicality of each sample. ")
+    num_nearest_neighbors: Optional[conint(strict=True, ge=2)] = Field(None, alias="numNearestNeighbors", description="It is the number of nearest datapoints used to compute the typicality of each sample. ")
     stopping_condition_minimum_typicality: Optional[Union[confloat(gt=0, strict=True), conint(gt=0, strict=True)]] = Field(None, alias="stoppingConditionMinimumTypicality", description="It is the minimal allowed typicality of the selected samples. When the typicality of the selected samples reaches this, the selection stops. It should be  a number between 0 and 1. ")
     strength: Optional[Union[confloat(le=1000000000, ge=-1000000000, strict=True), conint(le=1000000000, ge=-1000000000, strict=True)]] = Field(None, description="The relative strength of this strategy compared to other strategies. The default value is 1.0, which is set in the worker for backwards compatibility. The minimum and maximum values of +-10^9 are used to prevent numerical issues. ")
     stopping_condition_max_sum: Optional[Union[confloat(ge=0.0, strict=True), conint(ge=0, strict=True)]] = Field(None, alias="stoppingConditionMaxSum", description="When the sum of inputs reaches this, the selection stops. Only compatible with the WEIGHTS strategy. Similar to the stopping_condition_minimum_distance for the DIVERSITY strategy. ")
     target_range: Optional[SelectionConfigV3EntryStrategyAllOfTargetRange] = Field(None, alias="targetRange")
     __properties = ["type", "stopping_condition_minimum_distance", "threshold", "operation", "target", "numNearestNeighbors", "stoppingConditionMinimumTypicality", "strength", "stoppingConditionMaxSum", "targetRange"]
 
     class Config:
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from lightly.openapi_generated.swagger_client.models.selection_strategy_type_v3 import SelectionStrategyTypeV3
 
 class SelectionConfigV3EntryStrategyAllOf(BaseModel):
     """
     SelectionConfigV3EntryStrategyAllOf
     """
     type: SelectionStrategyTypeV3 = Field(...)
-    num_nearest_neighbors: Optional[Union[confloat(ge=2, strict=True), conint(ge=2, strict=True)]] = Field(None, alias="numNearestNeighbors", description="It is the number of nearest datapoints used to compute the typicality of each sample. ")
+    num_nearest_neighbors: Optional[conint(strict=True, ge=2)] = Field(None, alias="numNearestNeighbors", description="It is the number of nearest datapoints used to compute the typicality of each sample. ")
     stopping_condition_minimum_typicality: Optional[Union[confloat(gt=0, strict=True), conint(gt=0, strict=True)]] = Field(None, alias="stoppingConditionMinimumTypicality", description="It is the minimal allowed typicality of the selected samples. When the typicality of the selected samples reaches this, the selection stops. It should be  a number between 0 and 1. ")
     strength: Optional[Union[confloat(le=1000000000, ge=-1000000000, strict=True), conint(le=1000000000, ge=-1000000000, strict=True)]] = Field(None, description="The relative strength of this strategy compared to other strategies. The default value is 1.0, which is set in the worker for backwards compatibility. The minimum and maximum values of +-10^9 are used to prevent numerical issues. ")
     stopping_condition_max_sum: Optional[Union[confloat(ge=0.0, strict=True), conint(ge=0, strict=True)]] = Field(None, alias="stoppingConditionMaxSum", description="When the sum of inputs reaches this, the selection stops. Only compatible with the WEIGHTS strategy. Similar to the stopping_condition_minimum_distance for the DIVERSITY strategy. ")
     target_range: Optional[SelectionConfigV3EntryStrategyAllOfTargetRange] = Field(None, alias="targetRange")
     __properties = ["type", "numNearestNeighbors", "stoppingConditionMinimumTypicality", "strength", "stoppingConditionMaxSum", "targetRange"]
 
     class Config:
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of_target_range.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of_target_range.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4_all_of.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_all_of.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_input.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_input.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,34 +16,45 @@
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, Optional, Union
-from pydantic import Extra,  BaseModel, Field, StrictFloat, StrictInt, confloat, conint
+from pydantic import Extra,  BaseModel, Field, StrictFloat, StrictInt, StrictStr, confloat, conint, validator
 from lightly.openapi_generated.swagger_client.models.selection_config_v3_entry_strategy_all_of_target_range import SelectionConfigV3EntryStrategyAllOfTargetRange
 from lightly.openapi_generated.swagger_client.models.selection_strategy_threshold_operation import SelectionStrategyThresholdOperation
 from lightly.openapi_generated.swagger_client.models.selection_strategy_type_v3 import SelectionStrategyTypeV3
 
 class SelectionConfigV4EntryStrategy(BaseModel):
     """
     SelectionConfigV4EntryStrategy
     """
     type: SelectionStrategyTypeV3 = Field(...)
     stopping_condition_minimum_distance: Optional[Union[StrictFloat, StrictInt]] = None
     threshold: Optional[Union[StrictFloat, StrictInt]] = None
     operation: Optional[SelectionStrategyThresholdOperation] = None
     target: Optional[Dict[str, Any]] = None
-    num_nearest_neighbors: Optional[Union[confloat(ge=2, strict=True), conint(ge=2, strict=True)]] = Field(None, alias="numNearestNeighbors", description="It is the number of nearest datapoints used to compute the typicality of each sample. ")
+    num_nearest_neighbors: Optional[conint(strict=True, ge=2)] = Field(None, alias="numNearestNeighbors", description="It is the number of nearest datapoints used to compute the typicality of each sample. ")
     stopping_condition_minimum_typicality: Optional[Union[confloat(gt=0, strict=True), conint(gt=0, strict=True)]] = Field(None, alias="stoppingConditionMinimumTypicality", description="It is the minimal allowed typicality of the selected samples. When the typicality of the selected samples reaches this, the selection stops. It should be  a number between 0 and 1. ")
     strength: Optional[Union[confloat(le=1000000000, ge=-1000000000, strict=True), conint(le=1000000000, ge=-1000000000, strict=True)]] = Field(None, description="The relative strength of this strategy compared to other strategies. The default value is 1.0, which is set in the worker for backwards compatibility. The minimum and maximum values of +-10^9 are used to prevent numerical issues. ")
     stopping_condition_max_sum: Optional[Union[confloat(ge=0.0, strict=True), conint(ge=0, strict=True)]] = Field(None, alias="stoppingConditionMaxSum", description="When the sum of inputs reaches this, the selection stops. Only compatible with the WEIGHTS strategy. Similar to the stopping_condition_minimum_distance for the DIVERSITY strategy. ")
     target_range: Optional[SelectionConfigV3EntryStrategyAllOfTargetRange] = Field(None, alias="targetRange")
-    __properties = ["type", "stopping_condition_minimum_distance", "threshold", "operation", "target", "numNearestNeighbors", "stoppingConditionMinimumTypicality", "strength", "stoppingConditionMaxSum", "targetRange"]
+    distribution: Optional[StrictStr] = Field(None, description="The distribution of the balance selection strategy. If TARGET is selected, the target prop of the selection strategy needs to be set as well.")
+    __properties = ["type", "stopping_condition_minimum_distance", "threshold", "operation", "target", "numNearestNeighbors", "stoppingConditionMinimumTypicality", "strength", "stoppingConditionMaxSum", "targetRange", "distribution"]
+
+    @validator('distribution')
+    def distribution_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('TARGET', 'UNIFORM', 'INPUT'):
+            raise ValueError("must be one of enum values ('TARGET', 'UNIFORM', 'INPUT')")
+        return value
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
         use_enum_values = True
         extra = Extra.forbid
@@ -92,11 +103,12 @@
             "threshold": obj.get("threshold"),
             "operation": obj.get("operation"),
             "target": obj.get("target"),
             "num_nearest_neighbors": obj.get("numNearestNeighbors"),
             "stopping_condition_minimum_typicality": obj.get("stoppingConditionMinimumTypicality"),
             "strength": obj.get("strength"),
             "stopping_condition_max_sum": obj.get("stoppingConditionMaxSum"),
-            "target_range": SelectionConfigV3EntryStrategyAllOfTargetRange.from_dict(obj.get("targetRange")) if obj.get("targetRange") is not None else None
+            "target_range": SelectionConfigV3EntryStrategyAllOfTargetRange.from_dict(obj.get("targetRange")) if obj.get("targetRange") is not None else None,
+            "distribution": obj.get("distribution")
         })
         return _obj
```

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_input_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_input_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/selection_strategy_type_v3.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/selection_strategy_type_v3.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/service_account_basic_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/service_account_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_config_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_config_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/shared_access_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/shared_access_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_active_learning_scores_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_operation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_arithmetics_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_bit_mask_response.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_arithmetics.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_initial.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_metadata.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_operation_method.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_rename.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_sampler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_samples.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_scatterplot.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_data_upsize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_change_entry.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_change_entry.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_create_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_create_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_creator.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_creator.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_update_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_update_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/tag_upsize_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/task_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/task_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/team_basic_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_basic_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/team_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/team_role.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/team_role.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/trigger2d_embedding_job_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/update_docker_worker_registry_entry_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/update_team_membership_request.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/update_team_membership_request.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/user_type.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/user_type.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/video_frame_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/video_frame_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/models/write_csv_url_data.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/openapi_generated/swagger_client/rest.py` & `lightly-1.5.4/lightly/openapi_generated/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/__init__.py` & `lightly-1.5.4/lightly/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/aim_transform.py` & `lightly-1.5.4/lightly/transforms/aim_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/byol_transform.py` & `lightly-1.5.4/lightly/transforms/byol_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/dino_transform.py` & `lightly-1.5.4/lightly/transforms/dino_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/fast_siam_transform.py` & `lightly-1.5.4/lightly/transforms/fast_siam_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/gaussian_blur.py` & `lightly-1.5.4/lightly/transforms/gaussian_blur.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/ijepa_transform.py` & `lightly-1.5.4/lightly/transforms/ijepa_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/image_grid_transform.py` & `lightly-1.5.4/lightly/transforms/image_grid_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/jigsaw.py` & `lightly-1.5.4/lightly/transforms/jigsaw.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/mae_transform.py` & `lightly-1.5.4/lightly/transforms/mae_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/mmcr_transform.py` & `lightly-1.5.4/lightly/transforms/mmcr_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/moco_transform.py` & `lightly-1.5.4/lightly/transforms/moco_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/msn_transform.py` & `lightly-1.5.4/lightly/transforms/msn_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/multi_crop_transform.py` & `lightly-1.5.4/lightly/transforms/multi_crop_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/multi_view_transform.py` & `lightly-1.5.4/lightly/transforms/multi_view_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/pirl_transform.py` & `lightly-1.5.4/lightly/transforms/pirl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/random_crop_and_flip_with_grid.py` & `lightly-1.5.4/lightly/transforms/random_crop_and_flip_with_grid.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/rotation.py` & `lightly-1.5.4/lightly/transforms/rotation.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/simclr_transform.py` & `lightly-1.5.4/lightly/transforms/simclr_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/simsiam_transform.py` & `lightly-1.5.4/lightly/transforms/simsiam_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/smog_transform.py` & `lightly-1.5.4/lightly/transforms/smog_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/solarize.py` & `lightly-1.5.4/lightly/transforms/solarize.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/swav_transform.py` & `lightly-1.5.4/lightly/transforms/swav_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/vicreg_transform.py` & `lightly-1.5.4/lightly/transforms/vicreg_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/vicregl_transform.py` & `lightly-1.5.4/lightly/transforms/vicregl_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/transforms/wmse_transform.py` & `lightly-1.5.4/lightly/transforms/wmse_transform.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/benchmarking/benchmark_module.py` & `lightly-1.5.4/lightly/utils/benchmarking/benchmark_module.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
-from typing import List, Optional
+from typing import Any, List, Optional, Tuple
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
 from pytorch_lightning import LightningModule
 from torch import Tensor
 from torch.utils.data import DataLoader
 
 from lightly.utils.benchmarking.knn import knn_predict
+from lightly.utils.dist import gather as lightly_gather
 
 
 class BenchmarkModule(LightningModule):
     """A PyTorch Lightning Module for automated kNN callback
 
     At the end of every training epoch we create a feature bank by feeding the
     `dataloader_kNN` passed to the module through the backbone.
@@ -80,15 +81,15 @@
         >>> # you can get the peak accuracy using
         >>> print(model.max_accuracy)
 
     """
 
     def __init__(
         self,
-        dataloader_kNN: DataLoader,
+        dataloader_kNN: DataLoader[Any],
         num_classes: int,
         knn_k: int = 200,
         knn_t: float = 0.1,
     ):
         super().__init__()
         self.backbone = nn.Module()
         self.max_accuracy = 0.0
@@ -108,54 +109,50 @@
         with torch.no_grad():
             for data in self.dataloader_kNN:
                 img, target, _ = data
                 img = img.to(self.device)
                 target = target.to(self.device)
                 feature = self.backbone(img).squeeze()
                 feature = F.normalize(feature, dim=1)
-                if (
-                    dist.is_available()
-                    and dist.is_initialized()
-                    and dist.get_world_size() > 0
-                ):
-                    # gather features and targets from all processes
-                    feature = torch.cat(dist.gather(feature), 0)
-                    target = torch.cat(dist.gather(target), 0)
                 train_features.append(feature)
                 train_targets.append(target)
         self._train_features = torch.cat(train_features, dim=0).t().contiguous()
         self._train_targets = torch.cat(train_targets, dim=0).t().contiguous()
 
-    def validation_step(self, batch, batch_idx) -> None:
+    def validation_step(
+        self, batch: Tuple[List[Tensor], Tensor, List[str]], batch_idx: int
+    ) -> None:
         # we can only do kNN predictions once we have a feature bank
         if self._train_features is not None and self._train_targets is not None:
             images, targets, _ = batch
             feature = self.backbone(images).squeeze()
             feature = F.normalize(feature, dim=1)
             predicted_labels = knn_predict(
                 feature,
                 self._train_features,
                 self._train_targets,
                 self.num_classes,
                 self.knn_k,
                 self.knn_t,
             )
+
             if dist.is_initialized() and dist.get_world_size() > 0:
                 # gather predictions and targets from all processes
-                predicted_labels = torch.cat(dist.gather(predicted_labels), 0)
-                targets = torch.cat(dist.gather(targets), 0)
+
+                predicted_labels = torch.cat(lightly_gather(predicted_labels), dim=0)
+                targets = torch.cat(lightly_gather(targets), dim=0)
 
             self._val_predicted_labels.append(predicted_labels.cpu())
             self._val_targets.append(targets.cpu())
 
     def on_validation_epoch_end(self) -> None:
         if self._val_predicted_labels and self._val_targets:
             predicted_labels = torch.cat(self._val_predicted_labels, dim=0)
             targets = torch.cat(self._val_targets, dim=0)
             top1 = (predicted_labels[:, 0] == targets).float().sum()
             acc = top1 / len(targets)
             if acc > self.max_accuracy:
-                self.max_accuracy = acc.item()
+                self.max_accuracy = float(acc.item())
             self.log("kNN_accuracy", acc * 100.0, prog_bar=True)
 
         self._val_predicted_labels.clear()
         self._val_targets.clear()
```

### Comparing `lightly-1.5.3/lightly/utils/benchmarking/knn.py` & `lightly-1.5.4/lightly/utils/benchmarking/knn.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/benchmarking/knn_classifier.py` & `lightly-1.5.4/lightly/utils/benchmarking/knn_classifier.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/benchmarking/linear_classifier.py` & `lightly-1.5.4/lightly/utils/benchmarking/linear_classifier.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/benchmarking/metric_callback.py` & `lightly-1.5.4/lightly/utils/benchmarking/metric_callback.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/benchmarking/online_linear_classifier.py` & `lightly-1.5.4/lightly/utils/benchmarking/online_linear_classifier.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/benchmarking/topk.py` & `lightly-1.5.4/lightly/utils/benchmarking/topk.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/bounding_box.py` & `lightly-1.5.4/lightly/utils/bounding_box.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/cropping/crop_image_by_bounding_boxes.py` & `lightly-1.5.4/lightly/utils/cropping/crop_image_by_bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/cropping/read_yolo_label_file.py` & `lightly-1.5.4/lightly/utils/cropping/read_yolo_label_file.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/debug.py` & `lightly-1.5.4/lightly/utils/debug.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/dependency.py` & `lightly-1.5.4/lightly/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/dist.py` & `lightly-1.5.4/lightly/utils/dist.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import Optional, Tuple
+from typing import Any, Callable, Optional, Tuple, TypeVar
 
 import torch
 import torch.distributed as dist
+from torch.autograd.function import FunctionCtx
 
 
 class GatherLayer(torch.autograd.Function):
     """Gather tensors from all processes, supporting backward propagation.
 
     This code was taken and adapted from here:
-    https://github.com/Spijkervet/SimCLR
+    https://github.com/vturrisi/solo-learn/blob/b69b4bd27472593919956d9ac58902a301537a4d/solo/utils/misc.py#L187
 
     """
 
     @staticmethod
-    def forward(ctx, input: torch.Tensor) -> Tuple[torch.Tensor, ...]:
-        ctx.save_for_backward(input)
+    def forward(ctx, input: torch.Tensor) -> Tuple[torch.Tensor, ...]:  # type: ignore
         output = [torch.empty_like(input) for _ in range(dist.get_world_size())]
         dist.all_gather(output, input)
         return tuple(output)
 
     @staticmethod
-    def backward(ctx, *grads: torch.Tensor) -> torch.Tensor:
-        (input,) = ctx.saved_tensors
-        grad_out = torch.empty_like(input)
-        grad_out[:] = grads[dist.get_rank()]
+    def backward(ctx, *grads) -> torch.Tensor:  # type: ignore
+        all_gradients = torch.stack(grads)
+        dist.all_reduce(all_gradients)
+        grad_out = all_gradients[dist.get_rank()]
         return grad_out
 
 
 def rank() -> int:
     """Returns the rank of the current process."""
     return dist.get_rank() if dist.is_initialized() else 0
 
@@ -35,15 +35,15 @@
 def world_size() -> int:
     """Returns the current world size (number of distributed processes)."""
     return dist.get_world_size() if dist.is_initialized() else 1
 
 
 def gather(input: torch.Tensor) -> Tuple[torch.Tensor]:
     """Gathers this tensor from all processes. Supports backprop."""
-    return GatherLayer.apply(input)
+    return GatherLayer.apply(input)  # type: ignore[no-any-return]
 
 
 def eye_rank(n: int, device: Optional[torch.device] = None) -> torch.Tensor:
     """Returns an (n, n * world_size) zero matrix with the diagonal for the rank
     of this process set to 1.
 
     Example output where n=3, the current process has rank 1, and there are
@@ -66,30 +66,33 @@
     rows = torch.arange(n, device=device, dtype=torch.long)
     cols = rows + rank() * n
     diag_mask = torch.zeros((n, n * world_size()), dtype=torch.bool)
     diag_mask[(rows, cols)] = True
     return diag_mask
 
 
-def rank_zero_only(fn):
+R = TypeVar("R")
+
+
+def rank_zero_only(fn: Callable[..., R]) -> Callable[..., Optional[R]]:
     """Decorator that only runs the function on the process with rank 0.
 
     Example:
         >>> @rank_zero_only
         >>> def print_rank_zero(message: str):
         >>>     print(message)
         >>>
         >>> print_rank_zero("Hello from rank 0!")
-
     """
 
-    def wrapped(*args, **kwargs):
+    def wrapped(*args: Any, **kwargs: Any) -> Optional[R]:
         if rank() == 0:
             return fn(*args, **kwargs)
+        return None
 
     return wrapped
 
 
 @rank_zero_only
-def print_rank_zero(*args, **kwargs) -> None:
+def print_rank_zero(*args: Any, **kwargs: Any) -> None:  # type: ignore[misc]
     """Equivalent to print, but only runs on the process with rank 0."""
     print(*args, **kwargs)
```

### Comparing `lightly-1.5.3/lightly/utils/embeddings_2d.py` & `lightly-1.5.4/lightly/utils/embeddings_2d.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/hipify.py` & `lightly-1.5.4/lightly/utils/hipify.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/io.py` & `lightly-1.5.4/lightly/utils/io.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/lars.py` & `lightly-1.5.4/lightly/utils/lars.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/reordering.py` & `lightly-1.5.4/lightly/utils/reordering.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/scheduler.py` & `lightly-1.5.4/lightly/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly/utils/version_compare.py` & `lightly-1.5.4/lightly/utils/version_compare.py`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/lightly.egg-info/PKG-INFO` & `lightly-1.5.4/lightly.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightly
-Version: 1.5.3
+Version: 1.5.4
 Summary: A deep learning package for self-supervised learning
 Author: Lightly Team
 Author-email: team@lightly.ai
 License: MIT
 Project-URL: Homepage, https://www.lightly.ai
 Project-URL: Web-App, https://app.lightly.ai
 Project-URL: Documentation, https://docs.lightly.ai
@@ -310,27 +310,27 @@
 
 - Linear: [SimCLR](https://arxiv.org/abs/2002.05709)
 - Finetune: [SimCLR](https://arxiv.org/abs/2002.05709)
 - KNN: [InstDisc](https://arxiv.org/abs/1805.01978)
 
 See the [benchmarking scripts](./benchmarks/imagenet/resnet50/) for details.
 
-| Model           | Backbone | Batch Size | Epochs | Linear Top1 | Finetune Top1 | kNN Top1 | Tensorboard                                                        | Checkpoint                                                                                                                                                              |
-| --------------- | -------- | ---------- | ------ | ----------- | ------------- | -------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| BarlowTwins     | Res50    | 256        | 100    | 62.9        | 72.6          | 45.6     | [link](https://tensorboard.dev/experiment/NxyNRiQsQjWZ82I9b0PvKg/) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_barlowtwins_2023-08-18_00-11-03/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt) |
-| BYOL            | Res50    | 256        | 100    | 62.5        | 74.5          | 46.0     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_byol_2024-02-14_16-10-09/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
-| DINO            | Res50    | 128        | 100    | 68.2        | 72.5          | 49.9     | [link](https://tensorboard.dev/experiment/DvKHX9sNSWWqDrRksllPLA)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dino_2023-06-06_13-59-48/pretrain/version_0/checkpoints/epoch%3D99-step%3D1000900.ckpt)       |
-| MAE             | ViT-B/16 | 256        | 100    | 46.0        | 81.3          | 11.2     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_vitb16_mae_2024-02-25_19-57-30/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)           |
-| MoCoV2          | Res50    | 256        | 100    | 61.5        | 74.3          | 41.8     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_mocov2_2024-02-18_10-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
-| SimCLR\*        | Res50    | 256        | 100    | 63.2        | 73.9          | 44.8     | [link](https://tensorboard.dev/experiment/Ugol97adQdezgcVibDYMMA)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-06-22_09-11-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
-| SimCLR\* + DCL  | Res50    | 256        | 100    | 65.1        | 73.5          | 49.6     | [link](https://tensorboard.dev/experiment/k4ZonZ77QzmBkc0lXswQlg/) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dcl_2023-07-04_16-51-40/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)         |
-| SimCLR\* + DCLW | Res50    | 256        | 100    | 64.5        | 73.2          | 48.5     | [link](https://tensorboard.dev/experiment/TrALnpwFQ4OkZV3uvaX7wQ/) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dclw_2023-07-07_14-57-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
-| SwAV            | Res50    | 256        | 100    | 67.2        | 75.4          | 49.5     | [link](https://tensorboard.dev/experiment/Ipx4Oxl5Qkqm5Sl5kWyKKg)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
-| TiCo            | Res50    | 256        | 100    | 49.7        | 72.7          | 26.6     | -                                                                  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_tico_2024-01-07_18-40-57/pretrain/version_0/checkpoints/epoch%3D99-step%3D250200.ckpt)        |
-| VICReg          | Res50    | 256        | 100    | 63.0        | 73.7          | 46.3     | [link](https://tensorboard.dev/experiment/qH5uywJbTJSzgCEfxc7yUw)  | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_vicreg_2023-09-11_10-53-08/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
+| Model           | Backbone | Batch Size | Epochs | Linear Top1 | Finetune Top1 | kNN Top1 | Tensorboard                                                                                                                                                                    | Checkpoint                                                                                                                                                              |
+| --------------- | -------- | ---------- | ------ | ----------- | ------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| BarlowTwins     | Res50    | 256        | 100    | 62.9        | 72.6          | 45.6     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_barlowtwins_2023-08-18_00-11-03/pretrain/version_0/events.out.tfevents.1692310273.Machine2.569794.0) | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_barlowtwins_2023-08-18_00-11-03/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt) |
+| BYOL            | Res50    | 256        | 100    | 62.5        | 74.5          | 46.0     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_byol_2024-02-14_16-10-09/pretrain/version_0/events.out.tfevents.1707923418.Machine2.3205.0)          | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_byol_2024-02-14_16-10-09/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
+| DINO            | Res50    | 128        | 100    | 68.2        | 72.5          | 49.9     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dino_2023-06-06_13-59-48/pretrain/version_0/events.out.tfevents.1686052799.Machine2.482599.0)        | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dino_2023-06-06_13-59-48/pretrain/version_0/checkpoints/epoch%3D99-step%3D1000900.ckpt)       |
+| MAE             | ViT-B/16 | 256        | 100    | 46.0        | 81.3          | 11.2     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_vitb16_mae_2024-02-25_19-57-30/pretrain/version_0/events.out.tfevents.1708887459.Machine2.1092409.0)          | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_vitb16_mae_2024-02-25_19-57-30/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)           |
+| MoCoV2          | Res50    | 256        | 100    | 61.5        | 74.3          | 41.8     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_mocov2_2024-02-18_10-29-14/pretrain/version_0/events.out.tfevents.1708248562.Machine2.439033.0)      | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_mocov2_2024-02-18_10-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
+| SimCLR\*        | Res50    | 256        | 100    | 63.2        | 73.9          | 44.8     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-06-22_09-11-13/pretrain/version_0/events.out.tfevents.1687417883.Machine2.33270.0)       | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_simclr_2023-06-22_09-11-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
+| SimCLR\* + DCL  | Res50    | 256        | 100    | 65.1        | 73.5          | 49.6     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dcl_2023-07-04_16-51-40/pretrain/version_0/events.out.tfevents.1688482310.Machine2.247807.0)         | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dcl_2023-07-04_16-51-40/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)         |
+| SimCLR\* + DCLW | Res50    | 256        | 100    | 64.5        | 73.2          | 48.5     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dclw_2023-07-07_14-57-13/pretrain/version_0/events.out.tfevents.1688734645.Machine2.3176.0)          | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_dclw_2023-07-07_14-57-13/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
+| SwAV            | Res50    | 256        | 100    | 67.2        | 75.4          | 49.5     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/events.out.tfevents.1684996168.Machine2.1445108.0)       | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_swav_2023-05-25_08-29-14/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)        |
+| TiCo            | Res50    | 256        | 100    | 49.7        | 72.7          | 26.6     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_tico_2024-01-07_18-40-57/pretrain/version_0/events.out.tfevents.1704649265.Machine2.1604956.0)       | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_tico_2024-01-07_18-40-57/pretrain/version_0/checkpoints/epoch%3D99-step%3D250200.ckpt)        |
+| VICReg          | Res50    | 256        | 100    | 63.0        | 73.7          | 46.3     | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_vicreg_2023-09-11_10-53-08/pretrain/version_0/events.out.tfevents.1694422401.Machine2.556563.0)      | [link](https://lightly-ssl-checkpoints.s3.amazonaws.com/imagenet_resnet50_vicreg_2023-09-11_10-53-08/pretrain/version_0/checkpoints/epoch%3D99-step%3D500400.ckpt)      |
 
 _\*We use square root learning rate scaling instead of linear scaling as it yields
 better results for smaller batch sizes. See Appendix B.1 in the [SimCLR paper](https://arxiv.org/abs/2002.05709)._
 
 ### ImageNet100
 
 [ImageNet100 benchmarks detailed results](https://docs.lightly.ai/self-supervised-learning/getting_started/benchmarks.html#imagenet100)
```

### Comparing `lightly-1.5.3/lightly.egg-info/SOURCES.txt` & `lightly-1.5.4/lightly.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -350,14 +350,15 @@
 lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of.py
 lightly/openapi_generated/swagger_client/models/selection_config_v3_entry_strategy_all_of_target_range.py
 lightly/openapi_generated/swagger_client/models/selection_config_v4.py
 lightly/openapi_generated/swagger_client/models/selection_config_v4_all_of.py
 lightly/openapi_generated/swagger_client/models/selection_config_v4_entry.py
 lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_input.py
 lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy.py
+lightly/openapi_generated/swagger_client/models/selection_config_v4_entry_strategy_all_of.py
 lightly/openapi_generated/swagger_client/models/selection_input_predictions_name.py
 lightly/openapi_generated/swagger_client/models/selection_input_type.py
 lightly/openapi_generated/swagger_client/models/selection_strategy_threshold_operation.py
 lightly/openapi_generated/swagger_client/models/selection_strategy_type.py
 lightly/openapi_generated/swagger_client/models/selection_strategy_type_v3.py
 lightly/openapi_generated/swagger_client/models/service_account_basic_data.py
 lightly/openapi_generated/swagger_client/models/set_embeddings_is_processed_flag_by_id_body_request.py
```

### Comparing `lightly-1.5.3/lightly.egg-info/requires.txt` & `lightly-1.5.4/lightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lightly-1.5.3/setup.py` & `lightly-1.5.4/setup.py`

 * *Files identical despite different names*

