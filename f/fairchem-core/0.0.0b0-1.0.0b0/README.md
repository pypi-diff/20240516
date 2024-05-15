# Comparing `tmp/fairchem_core-0.0.0b0.tar.gz` & `tmp/fairchem_core-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fairchem_core-0.0.0b0.tar", last modified: Fri May 10 00:27:08 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `fairchem_core-0.0.0b0.tar` & `fairchem_core-1.0.0b0.tar`

### file list

```diff
@@ -1,11 +1,160 @@
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-10 00:27:08.490449 fairchem_core-0.0.0b0/
--rw-r--r--   0 lbluque    (501) staff       (20)      201 2024-05-10 00:27:08.489701 fairchem_core-0.0.0b0/PKG-INFO
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-10 00:27:08.484533 fairchem_core-0.0.0b0/fairchem/
--rw-r--r--   0 lbluque    (501) staff       (20)        0 2024-05-09 23:33:00.000000 fairchem_core-0.0.0b0/fairchem/__init__.py
-drwxr-xr-x   0 lbluque    (501) staff       (20)        0 2024-05-10 00:27:08.489035 fairchem_core-0.0.0b0/fairchem_core.egg-info/
--rw-r--r--   0 lbluque    (501) staff       (20)      201 2024-05-10 00:27:08.000000 fairchem_core-0.0.0b0/fairchem_core.egg-info/PKG-INFO
--rw-r--r--   0 lbluque    (501) staff       (20)      183 2024-05-10 00:27:08.000000 fairchem_core-0.0.0b0/fairchem_core.egg-info/SOURCES.txt
--rw-r--r--   0 lbluque    (501) staff       (20)        1 2024-05-10 00:27:08.000000 fairchem_core-0.0.0b0/fairchem_core.egg-info/dependency_links.txt
--rw-r--r--   0 lbluque    (501) staff       (20)        9 2024-05-10 00:27:08.000000 fairchem_core-0.0.0b0/fairchem_core.egg-info/top_level.txt
--rw-r--r--   0 lbluque    (501) staff       (20)      271 2024-05-10 00:26:53.000000 fairchem_core-0.0.0b0/pyproject.toml
--rw-r--r--   0 lbluque    (501) staff       (20)       38 2024-05-10 00:27:08.490532 fairchem_core-0.0.0b0/setup.cfg
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/LICENSE.md
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/README.md
+-rw-r--r--   0        0        0    23925 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/TRAIN.md
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/__init__.py
+-rw-r--r--   0        0        0     3131 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/_cli.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/__init__.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/data_parallel.py
+-rw-r--r--   0        0        0     6410 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/distutils.py
+-rw-r--r--   0        0        0     4647 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/flags.py
+-rw-r--r--   0        0        0     8508 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/gp_utils.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/hpo_utils.py
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/logger.py
+-rw-r--r--   0        0        0    10091 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/registry.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/transforms.py
+-rw-r--r--   0        0        0     5568 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/tutorial_utils.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/typing.py
+-rw-r--r--   0        0        0    46096 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/relaxation/__init__.py
+-rw-r--r--   0        0        0     8893 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/relaxation/ase_utils.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/relaxation/ml_relaxation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/relaxation/optimizers/__init__.py
+-rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/common/relaxation/optimizers/lbfgs_torch.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/__init__.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/_utils.py
+-rw-r--r--   0        0        0    22877 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/ase_datasets.py
+-rw-r--r--   0        0        0    10559 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/lmdb_database.py
+-rw-r--r--   0        0        0     9231 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/lmdb_dataset.py
+-rw-r--r--   0        0        0     8889 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/oc22_lmdb_dataset.py
+-rw-r--r--   0        0        0     7692 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/target_metadata_guesser.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/embeddings/__init__.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/embeddings/atomic_radii.py
+-rw-r--r--   0        0        0    19518 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/embeddings/continuous_embeddings.py
+-rw-r--r--   0        0        0   103170 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/embeddings/khot_embeddings.py
+-rw-r--r--   0        0        0    83734 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/datasets/embeddings/qmof_khot_embeddings.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/__init__.py
+-rw-r--r--   0        0        0     3955 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/base.py
+-rw-r--r--   0        0        0    15683 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/dimenet_plus_plus.py
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/model_registry.py
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/pretrained_models.yml
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/schnet.py
+-rw-r--r--   0        0        0    21697 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/Jd.pt
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/LICENSE
+-rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/README.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/__init__.py
+-rwxr-xr-x   0        0        0     6269 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/activation.py
+-rwxr-xr-x   0        0        0     4929 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/drop.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/edge_rot_mat.py
+-rw-r--r--   0        0        0    24723 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/equiformer_v2_oc20.py
+-rwxr-xr-x   0        0        0     1636 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/gaussian_rbf.py
+-rw-r--r--   0        0        0     5219 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/input_block.py
+-rwxr-xr-x   0        0        0    15514 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/layer_norm.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/module_list.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/radial_function.py
+-rw-r--r--   0        0        0    14060 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/so2_ops.py
+-rw-r--r--   0        0        0    25597 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/so3.py
+-rwxr-xr-x   0        0        0    28205 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/transformer_block.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/wigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/trainers/__init__.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/trainers/energy_trainer.py
+-rwxr-xr-x   0        0        0     2688 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/trainers/forces_trainer.py
+-rwxr-xr-x   0        0        0     6597 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/equiformer_v2/trainers/lr_scheduler.py
+-rw-r--r--   0        0        0    21697 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/escn/Jd.pt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/escn/__init__.py
+-rw-r--r--   0        0        0    34315 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/escn/escn.py
+-rw-r--r--   0        0        0    18749 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/escn/so3.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/__init__.py
+-rw-r--r--   0        0        0    20379 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/gemnet.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/initializers.py
+-rw-r--r--   0        0        0     9378 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/layers/__init__.py
+-rw-r--r--   0        0        0     6440 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/layers/atom_update_block.py
+-rw-r--r--   0        0        0     2933 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/layers/base_layers.py
+-rw-r--r--   0        0        0    10311 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/layers/basis_utils.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/layers/efficient.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/layers/embedding_block.py
+-rw-r--r--   0        0        0    10560 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/layers/interaction_block.py
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/layers/radial_basis.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet/layers/spherical_basis.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/README.md
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/__init__.py
+-rw-r--r--   0        0        0    22217 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/gemnet.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/initializers.py
+-rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/layers/__init__.py
+-rw-r--r--   0        0        0     7859 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/layers/atom_update_block.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/layers/base_layers.py
+-rw-r--r--   0        0        0    10315 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/layers/basis_utils.py
+-rw-r--r--   0        0        0     4941 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/layers/efficient.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/layers/embedding_block.py
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/layers/interaction_block.py
+-rw-r--r--   0        0        0     6425 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/layers/radial_basis.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_gp/layers/spherical_basis.py
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/README.md
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/__init__.py
+-rw-r--r--   0        0        0    48537 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/gemnet_oc.py
+-rw-r--r--   0        0        0     2737 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/initializers.py
+-rw-r--r--   0        0        0    10429 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/interaction_indices.py
+-rw-r--r--   0        0        0    14313 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/__init__.py
+-rw-r--r--   0        0        0     5823 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/atom_update_block.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/base_layers.py
+-rw-r--r--   0        0        0    11214 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/basis_utils.py
+-rw-r--r--   0        0        0     9301 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/efficient.py
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/embedding_block.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/force_scaler.py
+-rw-r--r--   0        0        0    23486 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/interaction_block.py
+-rw-r--r--   0        0        0     7672 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/radial_basis.py
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/gemnet_oc/layers/spherical_basis.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/painn/README.md
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/painn/__init__.py
+-rw-r--r--   0        0        0    21471 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/painn/painn.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/painn/utils.py
+-rw-r--r--   0        0        0    21697 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/scn/Jd.pt
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/scn/README.md
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/scn/__init__.py
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/scn/sampling.py
+-rw-r--r--   0        0        0    29135 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/scn/scn.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/scn/smearing.py
+-rw-r--r--   0        0        0    13992 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/scn/spherical_harmonics.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/utils/__init__.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/utils/activations.py
+-rw-r--r--   0        0        0    10312 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/models/utils/basis.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/__init__.py
+-rw-r--r--   0        0        0     9871 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/evaluator.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/exponential_moving_average.py
+-rw-r--r--   0        0        0     3278 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/loss.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/normalizer.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/scheduler.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/transforms.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/scaling/__init__.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/scaling/compat.py
+-rw-r--r--   0        0        0     8403 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/scaling/fit.py
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/scaling/scale_factor.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/modules/scaling/util.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/preprocessing/__init__.py
+-rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/preprocessing/atoms_to_graphs.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/__init__.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/download_data.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/gif_maker_parallelized.py
+-rw-r--r--   0        0        0     3649 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/make_challenge_submission_file.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/make_lmdb_sizes.py
+-rw-r--r--   0        0        0     4830 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/make_submission_file.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/preprocess_ef.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/preprocess_relaxed.py
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/uncompress.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/hpo/README.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/hpo/__init__.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/hpo/run_tune.py
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/hpo/run_tune_pbt.py
+-rwxr-xr-x   0        0        0      194 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/hpo/slurm/start-head.sh
+-rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/hpo/slurm/start-worker.sh
+-rwxr-xr-x   0        0        0     1662 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/scripts/hpo/slurm/submit-ray-cluster.sbatch
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/tasks/__init__.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/tasks/task.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/trainers/__init__.py
+-rw-r--r--   0        0        0    32091 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/trainers/base_trainer.py
+-rw-r--r--   0        0        0    26599 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/src/fairchem/core/trainers/ocp_trainer.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/.gitignore
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     5204 2020-02-02 00:00:00.000000 fairchem_core-1.0.0b0/PKG-INFO
```

