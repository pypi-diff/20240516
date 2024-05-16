# Comparing `tmp/nrtk_explorer-0.1.2.tar.gz` & `tmp/nrtk_explorer-0.2.0.tar.gz`

## Comparing `nrtk_explorer-0.1.2.tar` & `nrtk_explorer-0.2.0.tar`

### file list

```diff
@@ -1,117 +1,118 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/.codespellrc
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/.flake8
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    23511 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/MANIFEST.in
--rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/screenshot.png
--rw-r--r--   0        0        0  4643872 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/usage.png
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/.github/dependabot.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/.github/workflows/create_release.yaml
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/desktop/README.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/desktop/create_exe.bat
--rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/desktop/create_linux.sh
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/desktop/create_mac.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/desktop/requirements.txt
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/desktop/run.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/DEPLOY.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/Dockerfile
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/README.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/captain-definition
--rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/scripts/build_image.sh
--rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/scripts/build_server.sh
--rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/scripts/run_image.sh
--rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/scripts/run_server.sh
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/setup/apps.yml
--rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/setup/initialize.sh
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/bundles/docker/setup/requirements.txt
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/examples/jupyter/show.ipynb
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/__init__.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/__init__.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/applet.py
--rw-r--r--   0        0        0    14871 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/core.py
--rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/embeddings.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/filtering.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/jupyter.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/main.py
--rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/parameters.py
--rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/test/__init__.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/test/quasar.py
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/test/vuetify2.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/test/vuetify3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/ui/__init__.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/ui/collapsible_card.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/ui/image_list.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/app/ui/result_list.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/__init__.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/dataset.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/dimension_reducers.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/embeddings_extractor.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/filtering.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/images_manager.py
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/ml_models.py
--rw-r--r--   0        0        0     5629 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/nrtk_transforms.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/object_detector.py
--rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/transforms.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/assets/__init__.py
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/library/assets/imagenet_classes.txt
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/module/.gitignore
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/module/__init__.py
--rw-r--r--   0        0        0   725493 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/module/serve/styles.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/__init__.py
--rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
--rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
--rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
--rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
--rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
--rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
--rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
--rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
--rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
--rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
--rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
--rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
--rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
--rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
--rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
--rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
--rw-r--r--   0        0        0   237505 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/widgets/__init__.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/src/nrtk_explorer/widgets/nrtk_explorer.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/tests/requirements.txt
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/tests/test_embeddings.py
--rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/tests/test_filtering.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/tests/test_import.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/tests/test_object_detector.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/.editorconfig
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/.eslintrc.cjs
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/.gitignore
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/.prettierrc.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/env.d.ts
--rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/package-lock.json
--rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/tsconfig.app.json
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/tsconfig.json
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/tsconfig.node.json
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/vite.config.ts
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/public/styles.css
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/main.js
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/components/FilterOperatorWidget.vue
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/components/FilterOptionsWidget.vue
--rw-r--r--   0        0        0     7185 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/components/ImageDetection.vue
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/components/ParamWidget.vue
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/components/ParamsWidget.vue
--rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/components/ScatterPlot.vue
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/components/index.js
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/types/index.ts
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/vue-components/src/utilities/colors.ts
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/LICENSE
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/README.md
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/hatch_build.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 nrtk_explorer-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.codespellrc
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.flake8
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    28253 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0   458672 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/screenshot.png
+-rw-r--r--   0        0        0  4643872 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/usage.png
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.github/workflows/create_release.yaml
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/README.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/create_exe.bat
+-rwxr-xr-x   0        0        0      241 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/create_linux.sh
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/create_mac.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/requirements.txt
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/desktop/run.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/DEPLOY.md
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/Dockerfile
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/README.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/captain-definition
+-rwxr-xr-x   0        0        0      162 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/scripts/build_image.sh
+-rwxr-xr-x   0        0        0      226 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/scripts/build_server.sh
+-rwxr-xr-x   0        0        0       64 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/scripts/run_image.sh
+-rwxr-xr-x   0        0        0      174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/scripts/run_server.sh
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/setup/apps.yml
+-rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/setup/initialize.sh
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/bundles/docker/setup/requirements.txt
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/examples/jupyter/show.ipynb
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/__init__.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/__init__.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/applet.py
+-rw-r--r--   0        0        0     7167 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/core.py
+-rw-r--r--   0        0        0    14220 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/embeddings.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/filtering.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/jupyter.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/main.py
+-rw-r--r--   0        0        0     4052 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/parameters.py
+-rw-r--r--   0        0        0    16245 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/__init__.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/quasar.py
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/vuetify2.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/vuetify3.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/__init__.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/collapsible_card.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/image_list.py
+-rw-r--r--   0        0        0     5651 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/layout.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/result_list.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/__init__.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/dataset.py
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/dimension_reducers.py
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/embeddings_extractor.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/filtering.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/images_manager.py
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/ml_models.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/nrtk_transforms.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/object_detector.py
+-rw-r--r--   0        0        0     6203 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/transforms.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/assets/__init__.py
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/library/assets/imagenet_classes.txt
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/module/.gitignore
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/module/__init__.py
+-rw-r--r--   0        0        0   725513 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/module/serve/styles.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/__init__.py
+-rw-r--r--   0        0        0   187603 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg
+-rw-r--r--   0        0        0   140827 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg
+-rw-r--r--   0        0        0   125000 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg
+-rw-r--r--   0        0        0   126137 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg
+-rw-r--r--   0        0        0   133163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg
+-rw-r--r--   0        0        0   166027 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg
+-rw-r--r--   0        0        0   177458 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg
+-rw-r--r--   0        0        0   160631 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg
+-rw-r--r--   0        0        0   246520 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg
+-rw-r--r--   0        0        0   107022 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg
+-rw-r--r--   0        0        0   180893 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg
+-rw-r--r--   0        0        0   217261 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg
+-rw-r--r--   0        0        0   102589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg
+-rw-r--r--   0        0        0   269721 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg
+-rw-r--r--   0        0        0   265479 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg
+-rw-r--r--   0        0        0   146964 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg
+-rw-r--r--   0        0        0   237505 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/widgets/__init__.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/src/nrtk_explorer/widgets/nrtk_explorer.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/requirements.txt
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/test_embeddings.py
+-rw-r--r--   0        0        0     5658 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/test_filtering.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/test_import.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/tests/test_object_detector.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/.editorconfig
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/.eslintrc.cjs
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/.gitignore
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/.prettierrc.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/env.d.ts
+-rw-r--r--   0        0        0   316181 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/package-lock.json
+-rw-r--r--   0        0        0     1920 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/tsconfig.app.json
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/tsconfig.json
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/tsconfig.node.json
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/vite.config.ts
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/public/styles.css
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/main.js
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/FilterOperatorWidget.vue
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/FilterOptionsWidget.vue
+-rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/ImageDetection.vue
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/ParamWidget.vue
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/ParamsWidget.vue
+-rw-r--r--   0        0        0     9480 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/ScatterPlot.vue
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/components/index.js
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/types/index.ts
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/vue-components/src/utilities/colors.ts
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/README.md
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/hatch_build.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 nrtk_explorer-0.2.0/PKG-INFO
```

### Comparing `nrtk_explorer-0.1.2/CHANGELOG.md` & `nrtk_explorer-0.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,115 @@
 # CHANGELOG
 
 
 
+## v0.2.0 (2024-05-16)
+
+### Ci
+
+* ci: fixture in semantic release script ([`5ce57e5`](https://github.com/Kitware/nrtk-explorer/commit/5ce57e57b18eb0c77677dc61694d6a3f52588c9e))
+
+### Feature
+
+* feat: support hot-reload for ui
+
+If starting app with `nrtk_explorer --hot-reload`,
+then a button appears in the upper right to reload
+the ui modules and re-run Engine.ui method. ([`42ae90d`](https://github.com/Kitware/nrtk-explorer/commit/42ae90d33325b2251a8d7585776ee6ebc129c6db))
+
+### Fix
+
+* fix(nrtk_transforms): support new nrtk PybsmPerturber api
+
+(cherry picked from commit efaf36a602b3383ab7a7374ec698b49a6e80d5b9) ([`edea3f8`](https://github.com/Kitware/nrtk-explorer/commit/edea3f83206799c2db8536c8a4038bcc89234ca3))
+
+* fix: change object_detector output
+
+(cherry picked from commit 633e5f46b22eaf594f3eab657b124f75386fff45) ([`fec5df0`](https://github.com/Kitware/nrtk-explorer/commit/fec5df0712d4743498d1f62fd56f46d94feaa22f))
+
+* fix(ImageDetection): fallback to Unknown name when uncatagorized
+
+Horse drawn trolly thing has category ID of 0.
+
+(cherry picked from commit f12cd7b2432b2b7fa957602e8dc34196bb183643) ([`75a236f`](https://github.com/Kitware/nrtk-explorer/commit/75a236f5b8309e1ab0839c50ba89eead09a5a6a7))
+
+* fix(object_detector): maintain input paths order of output predictions
+
+Caused annotations to be overlaid on the wrong
+images in image list view.
+
+(cherry picked from commit fcc8f0a278acf9cd8837185b8f046c75c315246a) ([`1b2fdb3`](https://github.com/Kitware/nrtk-explorer/commit/1b2fdb3615063be6e92a548ec0a6ab27751a001d))
+
+* fix(benchmarks): allow using a external COCO ds
+
+(cherry picked from commit 34b2fdbeff7b724c542ac053d4d19fca6114939c) ([`3e7e56e`](https://github.com/Kitware/nrtk-explorer/commit/3e7e56ed3f53e0baf2649336844e669f4213bcf8))
+
+* fix(nrtk-explorer): multi platform paths
+
+(cherry picked from commit 0131172a2480a3e75bdb353741561e31d1625bcd) ([`cc631d7`](https://github.com/Kitware/nrtk-explorer/commit/cc631d718476286a19222debc0382295e54885a2))
+
+* fix(nrtk_transforms): support new nrtk PybsmPerturber api ([`efaf36a`](https://github.com/Kitware/nrtk-explorer/commit/efaf36a602b3383ab7a7374ec698b49a6e80d5b9))
+
+* fix: change object_detector output ([`633e5f4`](https://github.com/Kitware/nrtk-explorer/commit/633e5f46b22eaf594f3eab657b124f75386fff45))
+
+* fix(ImageDetection): fallback to Unknown name when uncatagorized
+
+Horse drawn trolly thing has category ID of 0. ([`f12cd7b`](https://github.com/Kitware/nrtk-explorer/commit/f12cd7b2432b2b7fa957602e8dc34196bb183643))
+
+* fix(object_detector): maintain input paths order of output predictions
+
+Caused annotations to be overlaid on the wrong
+images in image list view. ([`fcc8f0a`](https://github.com/Kitware/nrtk-explorer/commit/fcc8f0a278acf9cd8837185b8f046c75c315246a))
+
+* fix(benchmarks): allow using a external COCO ds ([`34b2fdb`](https://github.com/Kitware/nrtk-explorer/commit/34b2fdbeff7b724c542ac053d4d19fca6114939c))
+
+* fix(nrtk-explorer): multi platform paths ([`0131172`](https://github.com/Kitware/nrtk-explorer/commit/0131172a2480a3e75bdb353741561e31d1625bcd))
+
+### Refactor
+
+* refactor(layout): factor out sections to functions ([`dfa9a85`](https://github.com/Kitware/nrtk-explorer/commit/dfa9a857675766fae6fdb66d3b4d68346607dea9))
+
+### Unknown
+
+* Merge main to release ([`e32828d`](https://github.com/Kitware/nrtk-explorer/commit/e32828d8011151e63093864411b037488275fa21))
+
+* Bump ubelt from 1.3.4 to 1.3.5
+
+Bumps [ubelt](https://github.com/Erotemic/ubelt) from 1.3.4 to 1.3.5.
+- [Release notes](https://github.com/Erotemic/ubelt/releases)
+- [Changelog](https://github.com/Erotemic/ubelt/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/Erotemic/ubelt/compare/v1.3.4...v1.3.5)
+
+---
+updated-dependencies:
+- dependency-name: ubelt
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`87a292d`](https://github.com/Kitware/nrtk-explorer/commit/87a292df21262e9f1f723a5a9be82d3fa3f89acc))
+
+* Bump scikit-learn from 1.4.1.post1 to 1.4.2
+
+Bumps [scikit-learn](https://github.com/scikit-learn/scikit-learn) from 1.4.1.post1 to 1.4.2.
+- [Release notes](https://github.com/scikit-learn/scikit-learn/releases)
+- [Commits](https://github.com/scikit-learn/scikit-learn/compare/1.4.1.post1...1.4.2)
+
+---
+updated-dependencies:
+- dependency-name: scikit-learn
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`a8a4862`](https://github.com/Kitware/nrtk-explorer/commit/a8a4862075cc57dc891ef40e6d46f9fbac29a267))
+
+* Auto-merge release back to main ([`12ea17d`](https://github.com/Kitware/nrtk-explorer/commit/12ea17d04d5790f9b5abea53684b34d2faab8b46))
+
+
 ## v0.1.2 (2024-04-19)
 
 ### Fix
 
 * fix(nrtk-explorer): fix readme ([`968e42e`](https://github.com/Kitware/nrtk-explorer/commit/968e42e38d0b9a15d62b4a27681aa1df300abde4))
 
 * fix(workflow): do not install uneeded deps ([`a29260f`](https://github.com/Kitware/nrtk-explorer/commit/a29260f2abcbc81d19c607d1f8c143bd435d4073))
```

### Comparing `nrtk_explorer-0.1.2/CONTRIBUTING.rst` & `nrtk_explorer-0.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/screenshot.png` & `nrtk_explorer-0.2.0/screenshot.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/usage.png` & `nrtk_explorer-0.2.0/usage.png`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/.github/workflows/ci.yml` & `nrtk_explorer-0.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/.github/workflows/create_release.yaml` & `nrtk_explorer-0.2.0/.github/workflows/create_release.yaml`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/bundles/desktop/README.md` & `nrtk_explorer-0.2.0/bundles/desktop/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/bundles/docker/DEPLOY.md` & `nrtk_explorer-0.2.0/bundles/docker/DEPLOY.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/bundles/docker/README.md` & `nrtk_explorer-0.2.0/bundles/docker/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/examples/jupyter/show.ipynb` & `nrtk_explorer-0.2.0/examples/jupyter/show.ipynb`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/applet.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/applet.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/core.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/embeddings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,359 +1,380 @@
-r"""
-Define your classes and create the instances that you need to expose
-"""
-
-import logging
-from typing import Iterable
-
-from trame.ui.quasar import QLayout
-from trame.widgets import quasar
-from trame.widgets import html
-from trame_server.utils.namespace import Translator
+from nrtk_explorer.widgets.nrtk_explorer import ScatterPlot
+from nrtk_explorer.library import embeddings_extractor
+from nrtk_explorer.library import dimension_reducers
 from nrtk_explorer.library import images_manager
-from nrtk_explorer.library.filtering import FilterProtocol
-
-from nrtk_explorer.app.embeddings import EmbeddingsApp
-from nrtk_explorer.app.transforms import TransformsApp
-from nrtk_explorer.app.filtering import FilteringApp
 from nrtk_explorer.app.applet import Applet
-from nrtk_explorer.app.ui.collapsible_card import collapsible_card
 import nrtk_explorer.test_data
-from pathlib import Path
-
-import os
 
+import asyncio
 import json
-import random
-
+import os
 
-logger = logging.getLogger(__name__)
-logger.setLevel(logging.INFO)
+from trame.widgets import quasar, html
+from trame.ui.quasar import QLayout
+from trame.app import get_server, asynchronous
 
-html.Template.slot_names.add("before")
-html.Template.slot_names.add("after")
 
-HORIZONTAL_SPLIT_DEFAULT_VALUE = 17
-VERTICAL_SPLIT_DEFAULT_VALUE = 40
+os.environ["TRAME_DISABLE_V3_WARNING"] = "1"
 
 DIR_NAME = os.path.dirname(nrtk_explorer.test_data.__file__)
-DEFAULT_DATASETS = [
-    f"{DIR_NAME}/coco-od-2017/test_val2017.json",
+DATASET_DIRS = [
+    f"{DIR_NAME}/OIRDS_v1_0/oirds.json",
+    f"{DIR_NAME}/OIRDS_v1_0/oirds_test.json",
+    f"{DIR_NAME}/OIRDS_v1_0/oirds_train.json",
 ]
 
 
-def image_id_to_meta(image_id):
-    return f"{image_id}_meta"
-
-
-def image_id_to_result(image_id):
-    return f"{image_id}_result"
-
-
-def parse_dataset_dirs(datasets):
-    return [{"label": Path(ds).name, "value": ds} for ds in datasets]
-
-
-# ---------------------------------------------------------
-# Engine class
-# ---------------------------------------------------------
-
-
-class Engine(Applet):
-    def __init__(self, server=None):
+class EmbeddingsApp(Applet):
+    def __init__(self, server):
         super().__init__(server)
 
-        self.server.cli.add_argument(
-            "--dataset",
-            nargs="+",
-            default=DEFAULT_DATASETS,
-            help="Path of the json file describing the image dataset",
-        )
-
-        known_args, _ = self.server.cli.parse_known_args()
-        self.input_paths = known_args.dataset
-        self.state.current_dataset = str(Path(self.input_paths[0]).resolve())
-
-        self.context["image_objects"] = {}
-        self.context["images_manager"] = images_manager.ImagesManager()
-        self.context["annotations"] = {}
-
         self._ui = None
+        self._on_select_fn = None
+        self.reducer = dimension_reducers.DimReducerManager()
+        self.is_standalone_app = self.server.state.parent is None
+        if self.is_standalone_app:
+            self.context.images_manager = images_manager.ImagesManager()
+
+        if self.state.current_dataset is None:
+            self.state.current_dataset = DATASET_DIRS[0]
+        self.features = None
 
-        self.state.collapse_dataset = False
-        self.state.collapse_embeddings = False
-        self.state.collapse_filter = False
-        self.state.collapse_transforms = False
-        self.state.client_only(
-            "collapse_dataset", "collapse_embeddings", "collapse_filter", "collapse_transforms"
-        )
-
-        self.state.horizontal_split = HORIZONTAL_SPLIT_DEFAULT_VALUE
-        self.state.vertical_split = VERTICAL_SPLIT_DEFAULT_VALUE
-        self.state.client_only("horizontal_split", "vertical_split")
-
-        transforms_translator = Translator()
-        transforms_translator.add_translation(
-            "feature_extraction_model", "current_transforms_model"
-        )
-
-        self._transforms_app = TransformsApp(
-            server=self.server.create_child_server(translator=transforms_translator)
-        )
-
-        embeddings_translator = Translator()
-        embeddings_translator.add_translation(
-            "feature_extraction_model", "current_embeddings_model"
-        )
-
-        self._embeddings_app = EmbeddingsApp(
-            server=self.server.create_child_server(translator=embeddings_translator),
-        )
+        self.state.client_only("camera_position")
+        self.state.feature_extraction_model = "resnet50.a1_in1k"
 
-        filtering_translator = Translator()
-        filtering_translator.add_translation("categories", "annotation_categories")
-        self._filtering_app = FilteringApp(
-            server=self.server.create_child_server(translator=filtering_translator),
-        )
-
-        self._embeddings_app.set_on_select(self._transforms_app.on_selected_images_change)
-        self._transforms_app.set_on_transform(self._embeddings_app.on_run_transformations)
-        self._embeddings_app.set_on_hover(self._transforms_app.on_image_hovered)
-        self._transforms_app.set_on_hover(self._embeddings_app.on_image_hovered)
-        self._filtering_app.set_on_apply_filter(self.on_filter_apply)
-
-        # Set state variable
-        self.state.trame__title = "nrtk_explorer"
-
-        # Bind instance methods to controller
-        self.ctrl.on_server_reload = self.ui
-        self.ctrl.add("on_server_ready")(self.on_server_ready)
-
-        self.state.num_images_max = 0
-        self.state.num_images_disabled = True
-        self.state.random_sampling = False
-        self.state.random_sampling_disabled = True
-        self.state.images_id = []
-
-        # Generate UI
-        self.ui()
-        self.context.images_manager = images_manager.ImagesManager()
+        self.server.controller.add("on_server_ready")(self.on_server_ready)
+        self.transformed_images_cache = {}
 
     def on_server_ready(self, *args, **kwargs):
         # Bind instance methods to state change
-        self.state.change("current_dataset")(self.on_dataset_change)
-        self.state.change("num_images")(self.on_num_images_change)
-        self.state.change("random_sampling")(self.on_random_sampling_change)
-
-        self.on_dataset_change()
-
-    def on_dataset_change(self, **kwargs):
-        # Reset cache
-        self.context.images_manager = images_manager.ImagesManager()
+        self.on_current_dataset_change()
+        self.on_feature_extraction_model_change()
+        self.state.change("current_dataset")(self.on_current_dataset_change)
+        self.state.change("feature_extraction_model")(self.on_feature_extraction_model_change)
+
+    def on_feature_extraction_model_change(self, **kwargs):
+        feature_extraction_model = self.state.feature_extraction_model
+        self.extractor = embeddings_extractor.EmbeddingsExtractor(
+            model_name=feature_extraction_model, manager=self.context.images_manager
+        )
 
+    def on_current_dataset_change(self, **kwargs):
+        self.state.num_elements_disabled = True
         with open(self.state.current_dataset) as f:
             dataset = json.load(f)
+            self.images = dataset["images"]
+            self.state.num_elements_max = len(self.images)
+        self.state.num_elements_disabled = False
+
+        if self.is_standalone_app:
+            self.context.images_manager = images_manager.ImagesManager()
+
+    def on_run_clicked(self):
+        self.state.is_loading = True
+        asynchronous.create_task(self.compute(self.compute_source_points))
+
+    async def compute(self, method):
+        # We need to yield twice for the is_loading=True to commit to the trame state
+        # before this routine ends
+        await asyncio.sleep(0)
+        await asyncio.sleep(0)
+        await method()
+        with self.state:
+            self.state.is_loading = False
+
+    async def compute_source_points(self):
+        self.features = self.extractor.extract(
+            paths=self.context.paths,
+            batch_size=int(self.state.model_batch_size),
+        )
 
-        self.state.num_images_max = len(dataset["images"])
-        self.state.random_sampling_disabled = False
-        self.state.num_images_disabled = False
-
-        self.reload_images()
-
-    def on_filter_apply(self, filter: FilterProtocol[Iterable[int]], **kwargs):
-        selected_indices = []
-
-        for index, image_id in enumerate(self.state.images_ids):
-            image_annotations_categories = map(
-                lambda annotation: annotation["category_id"],
-                self.context["annotations"].get(f"img_{image_id}", []),
+        if self.state.tab == "PCA":
+            self.state.points_sources = self.reducer.reduce(
+                name="PCA",
+                fit_features=self.features,
+                features=self.features,
+                dims=self.state.dimensionality,
+                whiten=self.state.pca_whiten,
+                solver=self.state.pca_solver,
             )
 
-            include = filter.evaluate(image_annotations_categories)
-
-            if include:
-                selected_indices.append(index)
+        elif self.state.tab == "UMAP":
+            args = {}
+            if self.state.umap_random_seed:
+                args["random_state"] = int(self.state.umap_random_seed_value)
+
+            if self.state.umap_n_neighbors:
+                args["n_neighbors"] = int(self.state.umap_n_neighbors_number)
+
+            self.state.points_sources = self.reducer.reduce(
+                name="UMAP",
+                dims=self.state.dimensionality,
+                fit_features=self.features,
+                features=self.features,
+                **args,
+            )
 
-        self._embeddings_app.on_select(selected_indices)
+        # Unselect current selection of images
+        if self._on_select_fn:
+            self._on_select_fn([])
+
+        self.state.points_transformations = []
+        self.state.user_selected_points_indices = []
+        self.state.camera_position = []
+
+    def on_run_transformations(self, transformed_image_ids):
+        # Fillup the cache with the transformed images
+        for img_id in transformed_image_ids:
+            img = self.context.image_objects[img_id]
+            img = self.context.images_manager.prepare_for_model(img)
+            self.transformed_images_cache[img_id] = img
+
+        transformation_features = self.extractor.extract(
+            paths=transformed_image_ids,
+            content=self.transformed_images_cache,
+            batch_size=int(self.state.model_batch_size),
+        )
 
-    def on_num_images_change(self, **kwargs):
-        self.reload_images()
+        if self.state.tab == "PCA":
+            self.state.points_transformations = self.reducer.reduce(
+                name="PCA",
+                fit_features=self.features,
+                features=transformation_features,
+                dims=self.state.dimensionality,
+                whiten=self.state.pca_whiten,
+                solver=self.state.pca_solver,
+            )
 
-    def on_random_sampling_change(self, **kwargs):
-        self.reload_images()
+        elif self.state.tab == "UMAP":
+            args = {}
+            if self.state.umap_random_seed:
+                args["random_state"] = int(self.state.umap_random_seed_value)
+
+            if self.state.umap_n_neighbors:
+                args["n_neighbors"] = int(self.state.umap_n_neighbors_number)
+
+            self.state.points_transformations = self.reducer.reduce(
+                name="UMAP",
+                dims=self.state.dimensionality,
+                fit_features=self.features,
+                features=transformation_features,
+                **args,
+            )
 
-    def reload_images(self):
-        with open(self.state.current_dataset) as f:
-            dataset = json.load(f)
+    def set_on_select(self, fn):
+        self._on_select_fn = fn
 
-        categories = {}
-        for category in dataset["categories"]:
-            categories[category["id"]] = category
-
-        images = dataset["images"]
-
-        selected_images = []
-        if self.state.num_images:
-            if self.state.random_sampling:
-                selected_images = random.sample(images, self.state.num_images)
+    def on_select(self, indices):
+        self.state.user_selected_points_indices = indices
+        self.state.points_transformations = []
+        ids = [self.state.images_ids[i] for i in indices]
+        if self._on_select_fn:
+            self._on_select_fn(ids)
+
+    def on_move(self, camera_position):
+        self.state.camera_position = camera_position
+
+    def set_on_hover(self, fn):
+        self._on_hover_fn = fn
+
+    def on_hover(self, point):
+        self.state.highlighted_point = point
+        image_id = -1
+        if point is not None and point in self.state.user_selected_points_indices:
+            image_id = self.state.images_ids[int(point)]
+        if self._on_hover_fn:
+            self._on_hover_fn(image_id)
+
+    def on_image_hovered(self, id_, is_transformation):
+        # If the point is in the list of selected points, we set it as the highlighted point
+        if id_ in self.state.images_ids:
+            index = self.state.images_ids.index(id_)
+            if is_transformation:
+                index_selected = self.state.user_selected_points_indices.index(index)
+                self.state.highlighted_point = len(self.state.points_sources) + index_selected
             else:
-                selected_images = images[: self.state.num_images]
+                self.state.highlighted_point = index
         else:
-            selected_images = images
+            # If the point is not in the list of selected points, we set it to a negative point
+            self.state.highlighted_point = -1
+
+    def visualization_widget(self):
+        ScatterPlot(
+            cameraMove="camera_position=$event",
+            cameraPosition=("camera_position",),
+            highlightedPoint=("highlighted_point", -1),
+            hover=(self.on_hover, "[$event]"),
+            points=("points_sources", []),
+            transformedPoints=("points_transformations", []),
+            select=(self.on_select, "[$event]"),
+            selectedPoints=("user_selected_points_indices", []),
+        )
 
-        paths = list()
-        for image in selected_images:
-            paths.append(
-                os.path.join(
-                    os.path.dirname(self.state.current_dataset),
-                    image["file_name"],
+    def settings_widget(self):
+        with html.Div(trame_server=self.server, classes="col"):
+            with html.Div(classes="q-gutter-y-md"):
+                quasar.QBtnToggle(
+                    v_model=("dimensionality", "3"),
+                    toggler_color="primary",
+                    flat=True,
+                    spread=True,
+                    options=(
+                        [
+                            {"label": "2D", "value": "2"},
+                            {"label": "3D", "value": "3"},
+                        ],
+                    ),
                 )
+
+            quasar.QSelect(
+                label="Embeddings Model",
+                v_model=("feature_extraction_model",),
+                options=(
+                    [
+                        {"label": "ResNet50", "value": "resnet50.a1_in1k"},
+                        {"label": "EfficientNet_b0", "value": "efficientnet_b0.ra_in1k"},
+                        {
+                            "label": "MobileNetV3Large",
+                            "value": "mobilenetv3_large_100.ra_in1k",
+                        },
+                    ],
+                ),
+                filled=True,
+                emit_value=True,
+                map_options=True,
+            )
+            quasar.QInput(
+                v_model=("model_batch_size", 32),
+                filled=True,
+                stack_label=True,
+                label="Batch Size",
+                type="number",
             )
 
-        self.context.paths = paths
-        self.state.annotation_categories = categories
-        self.state.images_ids = [img["id"] for img in selected_images]
+        with html.Div(classes="col"):
+            with quasar.QTabs(
+                v_model=("tab", "PCA"),
+                dense=True,
+                narrow_indicator=True,
+                active_color="primary",
+                indicator_color="primary",
+                align="justify",
+            ):
+                quasar.QTab(name="PCA", label="pca")
+                quasar.QTab(name="UMAP", label="umap")
+            quasar.QSeparator()
+            with quasar.QTabPanels(v_model=("tab", "PCA")):
+                with quasar.QTabPanel(name="PCA"):
+                    quasar.QToggle(
+                        v_model=("pca_whiten", False),
+                        label="Whiten",
+                        left_label=True,
+                    )
+                    quasar.QSelect(
+                        v_model=("pca_solver", "auto"),
+                        label="SVD Solver",
+                        toggler_color="primary",
+                        options=(
+                            [
+                                "auto",
+                                "full",
+                                "arpack",
+                                "randomized",
+                            ],
+                        ),
+                    )
+
+                with quasar.QTabPanel(name="UMAP"):
+                    quasar.QToggle(
+                        v_model=("umap_n_neighbors", False),
+                        label="Number of neighbors",
+                        left_label=True,
+                    )
+                    quasar.QInput(
+                        v_model=("umap_n_neighbors_number", 15),
+                        disable=("!umap_n_neighbors",),
+                        filled=True,
+                        stack_label=True,
+                        label="Neighbors amount",
+                        type="number",
+                    )
+                    quasar.QToggle(
+                        v_model=("umap_random_seed", True),
+                        label="Random seed",
+                        left_label=True,
+                    )
+                    quasar.QInput(
+                        v_model=("umap_random_seed_value", 1),
+                        disable=("!umap_random_seed",),
+                        filled=True,
+                        stack_label=True,
+                        label="Seed value",
+                        type="number",
+                    )
+
+    def compute_ui(self):
+        with html.Div(trame_server=self.server):
+            quasar.QBtn(
+                label="Compute",
+                loading=("is_loading", False),
+                click=self.on_run_clicked,
+                flat=True,
+            )
 
-    def ui(self, *args, **kwargs):
+    # This is only used within when this module (file) is executed as an Standalone app.
+    @property
+    def ui(self):
         if self._ui is None:
-            with QLayout(
-                self.server, view="lhh LpR lff", classes="shadow-2 rounded-borders bg-grey-2"
-            ) as layout:
-                # # Toolbar
+            with QLayout(self.server) as layout:
                 with quasar.QHeader():
                     with quasar.QToolbar(classes="shadow-4"):
-                        quasar.QToolbarTitle("NRTK_EXPLORER")
+                        quasar.QToolbarTitle("Embeddings")
+                        quasar.QBtn("Reset")
+
+                with quasar.QDrawer(
+                    v_model=("leftDrawerOpen", True),
+                    side="left",
+                    elevated=True,
+                ):
+                    with html.Div(classes="column justify-center", style="padding:1rem"):
+                        with html.Div(classes="col"):
+                            quasar.QSeparator()
+                            quasar.QSelect(
+                                label="Dataset",
+                                v_model=("current_dataset",),
+                                options=(
+                                    [
+                                        {"label": "oirds_test", "value": DATASET_DIRS[0]},
+                                        {"label": "oirds_train", "value": DATASET_DIRS[1]},
+                                    ],
+                                ),
+                                filled=True,
+                                emit_value=True,
+                                map_options=True,
+                            )
+                    self.settings_widget()
+                    self.compute_ui()
 
-                # # Main content
+                # Main content
                 with quasar.QPageContainer():
                     with quasar.QPage():
-                        with quasar.QSplitter(
-                            model_value=("horizontal_split",),
-                            classes="inherit-height",
-                            before_class="inherit-height zero-height scroll",
-                            after_class="inherit-height zero-height",
-                        ):
-                            with html.Template(v_slot_before=True):
-                                with html.Div(classes="q-pa-md q-gutter-md"):
-                                    (
-                                        dataset_title_slot,
-                                        dataset_content_slot,
-                                        dataset_actions_slot,
-                                    ) = collapsible_card("collapse_dataset")
-
-                                    with dataset_title_slot:
-                                        html.Span("Dataset Selection", classes="text-h6")
-
-                                    with dataset_content_slot:
-                                        quasar.QSelect(
-                                            label="Dataset",
-                                            v_model=("current_dataset",),
-                                            options=(parse_dataset_dirs(self.input_paths),),
-                                            filled=True,
-                                            emit_value=True,
-                                            map_options=True,
-                                            dense=True,
-                                        )
-                                        quasar.QSlider(
-                                            v_model=("num_images", 15),
-                                            min=(0,),
-                                            max=("num_images_max", 25),
-                                            disable=("num_images_disabled", True),
-                                            step=(1,),
-                                        )
-                                        html.P(
-                                            "{{num_images}}/{{num_images_max}} images",
-                                            classes="text-caption text-center",
-                                        )
-
-                                        quasar.QToggle(
-                                            v_model=("random_sampling", False),
-                                            dense=False,
-                                            label="Random selection",
-                                        )
-
-                                    (
-                                        embeddings_title_slot,
-                                        embeddings_content_slot,
-                                        embeddings_actions_slot,
-                                    ) = collapsible_card("collapse_embeddings")
-
-                                    with embeddings_title_slot:
-                                        html.Span("Embeddings", classes="text-h6")
-
-                                    with embeddings_content_slot:
-                                        self._embeddings_app.settings_widget()
-
-                                    with embeddings_actions_slot:
-                                        self._embeddings_app.compute_ui()
-
-                                    filter_title_slot, filter_content_slot, filter_actions_slot = (
-                                        collapsible_card("collapse_filter")
-                                    )
-
-                                    with filter_title_slot:
-                                        html.Span("Category Filter", classes="text-h6")
-
-                                    with filter_content_slot:
-                                        self._filtering_app.filter_operator_ui()
-                                        self._filtering_app.filter_options_ui()
-
-                                    with filter_actions_slot:
-                                        self._filtering_app.filter_apply_ui()
-
-                                    (
-                                        transforms_title_slot,
-                                        transforms_content_slot,
-                                        transforms_actions_slot,
-                                    ) = collapsible_card("collapse_transforms")
-
-                                    with transforms_title_slot:
-                                        html.Span("Transform Settings", classes="text-h6")
-
-                                    with transforms_content_slot:
-                                        self._transforms_app.settings_widget()
-
-                                    with transforms_actions_slot:
-                                        self._transforms_app.apply_ui()
-
-                            with html.Template(v_slot_after=True):
-                                with quasar.QSplitter(
-                                    v_model=("vertical_split",),
-                                    limits=("[0,100]",),
-                                    horizontal=True,
-                                    classes="inherit-height zero-height",
-                                    before_class="q-pa-md",
-                                    after_class="q-pa-md",
-                                ):
-                                    with html.Template(v_slot_before=True):
-                                        self._embeddings_app.visualization_widget()
-
-                                    with html.Template(v_slot_after=True):
-                                        with html.Div(classes="row q-col-gutter-md"):
-                                            with html.Div(classes="col-6"):
-                                                with quasar.QCard(flat=True, bordered=True):
-                                                    with quasar.QCardSection():
-                                                        html.Span(
-                                                            "Original Dataset", classes="text-h5"
-                                                        )
-
-                                                    with quasar.QCardSection():
-                                                        self._transforms_app.original_dataset_widget()
-
-                                            with html.Div(classes="col-6"):
-                                                with quasar.QCard(
-                                                    flat=True,
-                                                    bordered=True,
-                                                    style="background-color: #ffcdd2;",
-                                                ):
-                                                    with quasar.QCardSection():
-                                                        html.Span(
-                                                            "Transformed Dataset",
-                                                            classes="text-h5",
-                                                        )
+                        with html.Div(classes="row", style="min-height: inherit;"):
+                            with html.Div(classes="col q-pa-md"):
+                                self.visualization_widget()
 
-                                                    with quasar.QCardSection():
-                                                        self._transforms_app.transformed_dataset_widget()
+                self._ui = layout
+        return self._ui
 
-            self._ui = layout
 
-        return self._ui
+def embeddings(server=None, *args, **kwargs):
+    server = get_server()
+    server.client_type = "vue3"
+
+    embeddings_app = EmbeddingsApp(server)
+    embeddings_app.ui
+
+    server.start(**kwargs)
+
+
+if __name__ == "__main__":
+    embeddings()
```

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/filtering.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/jupyter.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/parameters.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/parameters.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/transforms.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from trame.widgets import quasar
 from trame.widgets import html
 from trame.app import get_server
 
 import nrtk_explorer.library.transforms as trans
 import nrtk_explorer.library.nrtk_transforms as nrtk_trans
 from nrtk_explorer.library import images_manager, object_detector
-from nrtk_explorer.app.ui.image_list import image_list_component
+from nrtk_explorer.app import ui
 from nrtk_explorer.app.applet import Applet
 from nrtk_explorer.app.parameters import ParametersApp
 from nrtk_explorer.library.ml_models import (
     ClassificationResNet50,
     ClassificationAlexNet,
     ClassificationVgg16,
 )
@@ -153,17 +153,17 @@
         """Compute annotations for the given image ids using the object detector model."""
         if len(ids) == 0:
             return
 
         for id_ in ids:
             self.context["annotations"][id_] = []
 
-        prediction = self.detector.eval(paths=ids, content=self.context.image_objects)
+        predictions = self.detector.eval(paths=ids, content=self.context.image_objects)
 
-        for id_, annotations in zip(ids, prediction):
+        for id_, annotations in predictions:
             image_annotations = self.context["annotations"].setdefault(id_, [])
             for prediction in annotations:
                 category_id = 0
                 for cat_id, cat in self.state.annotation_categories.items():
                     if cat["name"] == prediction["label"]:
                         category_id = cat_id
 
@@ -346,19 +346,19 @@
 
     def apply_ui(self):
         with html.Div(trame_server=self.server):
             self._parameters_app.transform_apply_ui()
 
     def original_dataset_widget(self):
         with html.Div(trame_server=self.server):
-            image_list_component("source_image_ids", self.on_hover)
+            ui.image_list_component("source_image_ids", self.on_hover)
 
     def transformed_dataset_widget(self):
         with html.Div(trame_server=self.server):
-            image_list_component("transformed_image_ids", self.on_hover, is_transformation=True)
+            ui.image_list_component("transformed_image_ids", self.on_hover, is_transformation=True)
 
     # This is only used within when this module (file) is executed as an Standalone app.
     @property
     def ui(self):
         if self._ui is None:
             with QLayout(
                 self.server, view="lhh LpR lff", classes="shadow-2 rounded-borders bg-grey-2"
```

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/test/quasar.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/quasar.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/test/vuetify2.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/vuetify2.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/test/vuetify3.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/test/vuetify3.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/ui/collapsible_card.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/collapsible_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from trame.widgets import quasar
 from trame.widgets import html
 
 
-def collapsible_card(collapse_key):
+def card(collapse_key):
     with quasar.QCard():
         with quasar.QCardSection():
             with html.Div(classes="row items-center no-wrap"):
                 title_slot = html.Div(classes="col")
 
                 with html.Div(classes="col-auto"):
                     quasar.QBtn(
```

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/app/ui/image_list.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/app/ui/image_list.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/library/dimension_reducers.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/library/dimension_reducers.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/library/embeddings_extractor.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/library/embeddings_extractor.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/library/filtering.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/library/filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/library/images_manager.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/library/images_manager.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/library/ml_models.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/library/ml_models.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/library/nrtk_transforms.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/library/nrtk_transforms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Any, Optional, Dict, Tuple
 
+import numpy as np
+from PIL import Image as ImageModule
 from PIL.Image import Image
-
-from nrtk_explorer.library.transforms import ImageTransform, ParameterDescription
-
+from pybsm.otf import darkCurrentFromDensity
 from nrtk.impls.perturb_image.generic.cv2.blur import GaussianBlurPerturber
 from nrtk.impls.perturb_image.pybsm.perturber import PybsmPerturber, PybsmSensor, PybsmScenario
-import pybsm
 
-import numpy as np
-from PIL import Image as ImageModule
+from nrtk_explorer.library.transforms import ImageTransform, ParameterDescription
 
 
 class NrtkGaussianBlurTransform(ImageTransform):
     def __init__(self, perturber: Optional[GaussianBlurPerturber] = None):
         if perturber is None:
             perturber = GaussianBlurPerturber()
 
@@ -44,15 +42,16 @@
         input_array = np.asarray(input)
         output_array = self._perturber.perturb(input_array)
 
         return ImageModule.fromarray(output_array)
 
 
 # Taken from the nrtk package tests
-def createSampleSensorandScenario() -> Tuple[PybsmSensor, PybsmScenario]:
+# https://github.com/Kitware/nrtk/blob/main/tests/impls/perturb_image/pybsm/test_pybsm_pertuber.py#L21
+def createSampleSensorAndScenario() -> Tuple[PybsmSensor, PybsmScenario]:
 
     name = "L32511x"
 
     # telescope focal length (m)
     f = 4
     # Telescope diameter (m)
     D = 275e-3
@@ -72,15 +71,15 @@
     wx = p
     wy = p
     # integration time (s) - this is a maximum, the actual integration time will be
     # determined by the well fill percentage
     intTime = 30.0e-3
 
     # dark current density of 1 nA/cm2 guess, guess mid range for a silicon camera
-    darkCurrent = pybsm.darkCurrentFromDensity(1e-5, wx, wy)
+    darkCurrent = darkCurrentFromDensity(1e-5, wx, wy)
 
     # rms read noise (rms electrons)
     readNoise = 25.0
 
     # maximum ADC level (electrons)
     maxN = 96000.0
 
@@ -140,29 +139,28 @@
 
     return sensor, scenario
 
 
 class NrtkPybsmTransform(ImageTransform):
     def __init__(self, perturber: Optional[PybsmPerturber] = None):
         if perturber is None:
-            sensor, scenario = createSampleSensorandScenario()
+            sensor, scenario = createSampleSensorAndScenario()
             perturber = PybsmPerturber(sensor=sensor, scenario=scenario)
 
         self._perturber: PybsmPerturber = perturber
 
     def get_parameters(self) -> dict[str, Any]:
         return {
             "D": self._perturber.sensor.D,
             "f": self._perturber.sensor.f,
         }
 
     def set_parameters(self, params: Dict[str, Any]):
         self._perturber.sensor.D = params["D"]
         self._perturber.sensor.f = params["f"]
-        self._perturber.metrics = pybsm.niirs(self._perturber.sensor, self._perturber.scenario)
 
     def get_parameters_description(self) -> Dict[str, ParameterDescription]:
         aperture_description: ParameterDescription = {
             "type": "float",
             "label": "Effective Aperture (m)",
             "default": None,
             "description": None,
```

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/library/object_detector.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/library/object_detector.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import transformers
 
 from functools import reduce
 from typing import Optional
 
 from nrtk_explorer.library import images_manager
 
-Annotations = list[list[dict]]
+Annotations = list[tuple[str, dict]]
 
 
 class ObjectDetector:
     """Object detection using Hugging Face's transformers library"""
 
     def __init__(
         self,
@@ -52,27 +52,33 @@
 
     def eval(
         self,
         paths: list[str],
         content: Optional[dict] = None,
         batch_size: int = 32,
     ) -> Annotations:
-        """Compute object recognition, return it in a dictionary of COCO format"""
+        """Compute object recognition, return it in a list of tuples in the form of [(path, annotations dict in COCO Format)]"""
         if len(paths) == 0:
             return []
 
         images: dict = {}
 
-        # Group images by size (shape)
+        # Some models require all the images in a batch to be the same size,
+        # otherwise crash or UB.
         for path in paths:
             img = None
             if content and path in content:
                 img = content[path]
             else:
                 img = self.manager.load_image(path)
 
-            images.setdefault(img.size, []).append(img)
+            images.setdefault(img.size, [[], []])
+            images[img.size][0].append(path)
+            images[img.size][1].append(img)
 
         # Call by each group
-        predictions = [self.pipeline(group, batch_size=batch_size) for group in images.values()]
+        predictions = [
+            list(zip(group[0], self.pipeline(group[1], batch_size=batch_size)))
+            for group in images.values()
+        ]
         # Flatten the list of predictions
         return reduce(operator.iadd, predictions)
```

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/library/transforms.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/library/transforms.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/library/assets/imagenet_classes.txt` & `nrtk_explorer-0.2.0/src/nrtk_explorer/library/assets/imagenet_classes.txt`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js` & `nrtk_explorer-0.2.0/src/nrtk_explorer/module/serve/nrtk_explorer.umd.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -221,16 +221,20 @@
                             }),
                             D = r.retrieve(L).filter(N => o(N, L));
                         let R = document.createElement("ul");
                         R.style.padding = "0", R.style.margin = "0", D.forEach(N => {
                             const B = document.createElement("li");
                             if (N.data != null) {
                                 const P = l.annotations[N.data],
-                                    F = l.categories[P.category_id];
-                                B.textContent = `(${P.id}): ${F.name}`;
+                                    {
+                                        name: F
+                                    } = l.categories[P.category_id] ?? {
+                                        name: "Unknown"
+                                    };
+                                B.textContent = `(${P.id}): ${F}`;
                                 const U = n[P.category_id % n.length];
                                 B.style.textShadow = `rgba(${U.join(",")},0.6) 1px 1px 3px`, R.appendChild(B)
                             }
                         }), h.value.replaceChildren(R)
                     }
                 }
```

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000016228.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000104612.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000109798.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000181666.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000184791.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000238866.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000356427.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000370677.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000474028.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000491497.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000511321.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000514508.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000515445.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000516316.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000551215.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/000000555705.jpg`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json` & `nrtk_explorer-0.2.0/src/nrtk_explorer/test_data/coco-od-2017/test_val2017.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/src/nrtk_explorer/widgets/nrtk_explorer.py` & `nrtk_explorer-0.2.0/src/nrtk_explorer/widgets/nrtk_explorer.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/tests/test_embeddings.py` & `nrtk_explorer-0.2.0/tests/test_embeddings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 from nrtk_explorer.library import embeddings_extractor
 from nrtk_explorer.library import dimension_reducers
 from nrtk_explorer.library import images_manager
 import nrtk_explorer.test_data
 
 from tabulate import tabulate
 from itertools import product
+from pathlib import Path
 
 import json
 import os
 import pytest
 import timeit
 
 CURRENT_DIR_NAME = os.path.dirname(nrtk_explorer.test_data.__file__)
-DATASET = f"{CURRENT_DIR_NAME}/coco-od-2017/test_val2017.json"
+inc_ds_path = Path(f"{CURRENT_DIR_NAME}/coco-od-2017/test_val2017.json")
 
 
-def image_paths_impl():
-    with open(DATASET) as f:
+def image_paths_impl(file_name):
+    with open(file_name) as f:
         dataset = json.load(f)
     images = dataset["images"]
 
     paths = list()
     for image_metadata in images:
-        paths.append(os.path.join(os.path.dirname(DATASET), image_metadata["file_name"]))
+        paths.append(os.path.join(os.path.dirname(file_name), image_metadata["file_name"]))
+
     return paths
 
 
 @pytest.fixture
-def image_paths():
-    return image_paths_impl()
+def image_paths(request):
+    return image_paths_impl(inc_ds_path)
+
+
+@pytest.fixture
+def image_paths_external(request):
+    return image_paths_impl(request.config.getoption("--benchmark-dataset-file"))
 
 
 def test_features_small(image_paths):
     extractor = embeddings_extractor.EmbeddingsExtractor()
     features = extractor.extract(image_paths[:10])
     assert len(features) == 10
     print(features)
@@ -41,19 +48,19 @@
 def test_features_zero(image_paths):
     extractor = embeddings_extractor.EmbeddingsExtractor()
     features = extractor.extract([])
     assert features is None
     print(features)
 
 
-@pytest.mark.slow
-def test_features_all(image_paths):
+@pytest.mark.benchmark
+def test_features_all(image_paths_external):
     extractor = embeddings_extractor.EmbeddingsExtractor()
-    features = extractor.extract(image_paths)
-    assert len(features) == len(image_paths)
+    features = extractor.extract(image_paths_external)
+    assert len(features) == len(image_paths_external)
     print(f"Number of features: {len(features)}")
 
 
 def test_pca_2d(image_paths):
     extractor = embeddings_extractor.EmbeddingsExtractor()
     features = extractor.extract(image_paths[:10])
     model = dimension_reducers.PCAReducer(2)
@@ -101,65 +108,64 @@
     extractor = embeddings_extractor.EmbeddingsExtractor()
     features = extractor.extract(image_paths[:10])
     mgr = dimension_reducers.DimReducerManager()
     old_points = mgr.reduce(fit_features=features, features=features, name="PCA", dims=3)
     assert len(old_points) > 0
     assert len(old_points[0]) == 3
 
-    # breakpoint()
     new_points = mgr.reduce(fit_features=features, features=features, name="PCA", dims=3)
     assert id(old_points) == id(new_points)
 
     new_points_2d = mgr.reduce(fit_features=features, features=features, name="PCA", dims=2)
     assert id(old_points) != id(new_points_2d)
 
 
-@pytest.mark.slow
-def test_features_extractor_benchmark(image_paths):
+@pytest.mark.benchmark
+def test_features_extractor_benchmark(image_paths_external):
     repetitions = 3
     sampling = [10, 100]
     batch_size = [1, 8, 16, 32]
     setups = list(product(sampling, batch_size))
     setups.append([500, 1])
     setups.append([500, 64])
     table = list()
 
     # Pre-load images
     manager = images_manager.ImagesManager()
-    for path in image_paths[: max(sampling)]:
+    for path in image_paths_external[: max(sampling)]:
         manager.load_image_for_model(path)
 
     for n, batch_size in setups:
         extractor = embeddings_extractor.EmbeddingsExtractor(manager=manager)
         output = timeit.repeat(
-            stmt=lambda: extractor.extract(image_paths[:n], batch_size=batch_size),
+            stmt=lambda: extractor.extract(image_paths_external[:n], batch_size=batch_size),
             number=repetitions,
             repeat=5,
         )
         table.append([n, batch_size, min(output) / 10 / n])
 
     print(tabulate(table, headers=["#Samples", "batch_size", "ExecTime(sec)"], tablefmt="github"))
 
 
-@pytest.mark.slow
-def test_reducer_manager_benchmark(image_paths):
+@pytest.mark.benchmark
+def test_reducer_manager_benchmark(image_paths_external):
     setups = [
         ("PCA", 10, True, 100),
         ("PCA", 10, False, 100),
         ("PCA", 100, True, 10),
         ("PCA", 100, False, 10),
         ("UMAP", 10, True, 100),
         ("UMAP", 10, False, 100),
         ("UMAP", 100, True, 10),
         ("UMAP", 100, False, 10),
     ]
 
     mgr = dimension_reducers.DimReducerManager()
     extractor = embeddings_extractor.EmbeddingsExtractor()
-    features = extractor.extract(image_paths)
+    features = extractor.extract(image_paths_external)
 
     # Short benchmarks cached
     for name, n, cache, iterations in setups:
         output = timeit.timeit(
             lambda: mgr.reduce(
                 fit_features=features[:n], features=features, name=name, cache=cache
             ),
@@ -167,29 +173,29 @@
         )
 
         print(
             f"{name} dims reductions of {n} images cached={cache} mean(FullExecTime)={output / iterations}s"
         )
 
 
-@pytest.mark.slow
-def test_pca_3d_large(image_paths):
+@pytest.mark.benchmark
+def test_pca_3d_large(image_paths_external):
     extractor = embeddings_extractor.EmbeddingsExtractor()
-    features = extractor.extract(image_paths)
+    features = extractor.extract(image_paths_external)
     model = dimension_reducers.PCAReducer(3)
     points = model.reduce(features)
     assert len(points) > 0
     assert len(points[0]) == 3
     print(f"Number of images: {len(points)}")
     print(points)
 
 
-@pytest.mark.slow
-def test_umap_3d_large(image_paths):
+@pytest.mark.benchmark
+def test_umap_3d_large(image_paths_external):
     extractor = embeddings_extractor.EmbeddingsExtractor()
-    features = extractor.extract(image_paths)
+    features = extractor.extract(image_paths_external)
     model = dimension_reducers.UMAPReducer(3)
     points = model.reduce(features)
     assert len(points) > 0
     assert len(points[0]) == 3
     print(f"Number of images: {len(points)}")
     print(points)
```

### Comparing `nrtk_explorer-0.1.2/tests/test_filtering.py` & `nrtk_explorer-0.2.0/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/tests/test_object_detector.py` & `nrtk_explorer-0.2.0/tests/test_object_detector.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/package-lock.json` & `nrtk_explorer-0.2.0/vue-components/package-lock.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/package.json` & `nrtk_explorer-0.2.0/vue-components/package.json`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/vite.config.ts` & `nrtk_explorer-0.2.0/vue-components/vite.config.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/src/components/FilterOperatorWidget.vue` & `nrtk_explorer-0.2.0/vue-components/src/components/FilterOperatorWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/src/components/FilterOptionsWidget.vue` & `nrtk_explorer-0.2.0/vue-components/src/components/FilterOptionsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/src/components/ImageDetection.vue` & `nrtk_explorer-0.2.0/vue-components/src/components/ImageDetection.vue`

 * *Files 2% similar despite different names*

```diff
@@ -226,16 +226,16 @@
     list.style.padding = '0'
     list.style.margin = '0'
 
     hits.forEach((hit) => {
       const item = document.createElement('li')
       if (hit.data != undefined) {
         const annotation = props.annotations[hit.data]
-        const category = props.categories[annotation.category_id]
-        item.textContent = `(${annotation.id}): ${category.name}`
+        const { name } = props.categories[annotation.category_id] ?? { name: 'Unknown' }
+        item.textContent = `(${annotation.id}): ${name}`
         const color = CATEGORY_COLORS[annotation.category_id % CATEGORY_COLORS.length]
         item.style.textShadow = `rgba(${color.join(',')},0.6) 1px 1px 3px`
         list.appendChild(item)
       }
     })
 
     labelContainer.value.replaceChildren(list)
```

### Comparing `nrtk_explorer-0.1.2/vue-components/src/components/ParamWidget.vue` & `nrtk_explorer-0.2.0/vue-components/src/components/ParamWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/src/components/ParamsWidget.vue` & `nrtk_explorer-0.2.0/vue-components/src/components/ParamsWidget.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/src/components/ScatterPlot.vue` & `nrtk_explorer-0.2.0/vue-components/src/components/ScatterPlot.vue`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/src/types/index.ts` & `nrtk_explorer-0.2.0/vue-components/src/types/index.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/vue-components/src/utilities/colors.ts` & `nrtk_explorer-0.2.0/vue-components/src/utilities/colors.ts`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/LICENSE` & `nrtk_explorer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/README.md` & `nrtk_explorer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/hatch_build.py` & `nrtk_explorer-0.2.0/hatch_build.py`

 * *Files identical despite different names*

### Comparing `nrtk_explorer-0.1.2/pyproject.toml` & `nrtk_explorer-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="nrtk-explorer"
-version="0.1.2"
+version="0.2.0"
 description="Model Visualizer"
 authors = [
   {name = "Alessandro Genova", email = "alessandro.genova@kitware.com"},
   {name = "Vicente Adolfo Bolea Sanchez", email = "vicente.bolea@kitware.com"},
 ]
 readme = "README.md"
 keywords = [
@@ -26,15 +26,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 dependencies = [
     "nrtk",
     "numpy",
     "Pillow",
-    "scikit-learn==1.4.1.post1",
+    "scikit-learn==1.4.2",
     "smqtk-classifier==0.19.0",
     "accelerate",
     "smqtk-core==0.19.0",
     "smqtk-dataprovider==0.18.0",
     "smqtk-descriptors==0.19.0",
     "smqtk-detection[torch,centernet]==0.20.1",
     "smqtk-image-io==0.17.1",
@@ -43,15 +43,15 @@
     "timm",
     "torch",
     "torchvision",
     "trame",
     "trame-client>=2.15.0",
     "trame-quasar",
     "trame-server>=2.15.0",
-    "ubelt==1.3.4",
+    "ubelt==1.3.5",
     "umap-learn",
     "tabulate",
 ]
 
 [project.optional-dependencies]
 dev = [
   "black",
@@ -124,15 +124,15 @@
   [ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh"
   nvm install 20
   node -v
   npm -v
   python -m venv .venv
   source .venv/bin/activate
   pip install -U pip
-  python -m pip install "build<0.10.0" "python-semantic-release" "setuptools" "wheel"
+  python -m pip install "build<0.10.0" python-semantic-release setuptools wheel
   python -m build .
 """
 
 [tool.semantic_release.branches.main]
 match = "(release)"
 prerelease_token = "rc"
 prerelease = false
```

### Comparing `nrtk_explorer-0.1.2/PKG-INFO` & `nrtk_explorer-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nrtk-explorer
-Version: 0.1.2
+Version: 0.2.0
 Summary: Model Visualizer
 Author-email: Alessandro Genova <alessandro.genova@kitware.com>, Vicente Adolfo Bolea Sanchez <vicente.bolea@kitware.com>
 License-File: LICENSE
 Keywords: Application,Framework,Interactive,Python,Web
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: License :: Other/Proprietary License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: accelerate
 Requires-Dist: nrtk
 Requires-Dist: numpy
 Requires-Dist: pillow
-Requires-Dist: scikit-learn==1.4.1.post1
+Requires-Dist: scikit-learn==1.4.2
 Requires-Dist: smqtk-classifier==0.19.0
 Requires-Dist: smqtk-core==0.19.0
 Requires-Dist: smqtk-dataprovider==0.18.0
 Requires-Dist: smqtk-descriptors==0.19.0
 Requires-Dist: smqtk-detection[centernet,torch]==0.20.1
 Requires-Dist: smqtk-image-io==0.17.1
 Requires-Dist: tabulate
@@ -30,15 +30,15 @@
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: trame
 Requires-Dist: trame-client>=2.15.0
 Requires-Dist: trame-quasar
 Requires-Dist: trame-server>=2.15.0
 Requires-Dist: transformers
-Requires-Dist: ubelt==1.3.4
+Requires-Dist: ubelt==1.3.5
 Requires-Dist: umap-learn
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: tabulate; extra == 'dev'
```

