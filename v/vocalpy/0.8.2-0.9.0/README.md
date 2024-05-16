# Comparing `tmp/vocalpy-0.8.2.tar.gz` & `tmp/vocalpy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalpy-0.8.2.tar", last modified: Thu Feb  8 02:26:37 2024, max compression
+gzip compressed data, was "vocalpy-0.9.0.tar", last modified: Thu May 16 03:55:53 2024, max compression
```

## Comparing `vocalpy-0.8.2.tar` & `vocalpy-0.9.0.tar`

### file list

```diff
@@ -1,146 +1,157 @@
--rw-r--r--   0        0        0      650 2024-01-26 17:19:50.207528 vocalpy-0.8.2/.all-contributorsrc
--rw-r--r--   0        0        0     1307 2023-09-19 17:23:06.009955 vocalpy-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      248 2023-08-20 18:48:42.054440 vocalpy-0.8.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      615 2023-08-20 18:48:42.054440 vocalpy-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      705 2024-01-17 01:58:19.551347 vocalpy-0.8.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0      332 2024-01-26 17:19:50.207528 vocalpy-0.8.2/.gitignore
--rw-r--r--   0        0        0      769 2023-08-20 18:48:42.054440 vocalpy-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      334 2023-09-29 20:50:59.859125 vocalpy-0.8.2/.readthedocs.yaml
--rw-r--r--   0        0        0     5556 2023-09-19 17:23:06.009955 vocalpy-0.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1867 2023-08-20 18:48:42.054440 vocalpy-0.8.2/CONTRIBUTING.md
--rw-r--r--   0        0        0     1540 2023-04-18 02:08:12.226241 vocalpy-0.8.2/LICENSE
--rw-r--r--   0        0        0    15000 2024-02-07 20:41:23.718786 vocalpy-0.8.2/README.md
--rw-r--r--   0        0        0     4084 2024-02-08 02:26:16.209193 vocalpy-0.8.2/docs/CHANGELOG.md
--rw-r--r--   0        0        0      634 2023-12-30 12:42:08.307677 vocalpy-0.8.2/docs/Makefile
--rw-r--r--   0        0        0    29965 2023-08-20 18:48:42.054440 vocalpy-0.8.2/docs/_static/vocalpy-logomark.png
--rw-r--r--   0        0        0   285798 2023-08-20 18:48:42.054440 vocalpy-0.8.2/docs/_static/vocalpy-primary.png
--rw-r--r--   0        0        0   194159 2023-08-20 18:48:42.054440 vocalpy-0.8.2/docs/_static/vocalpy-secondary.png
--rw-r--r--   0        0        0      612 2023-12-30 13:28:54.397449 vocalpy-0.8.2/docs/_templates/class.rst
--rw-r--r--   0        0        0     1177 2023-12-30 13:28:54.397449 vocalpy-0.8.2/docs/_templates/module.rst
--rw-r--r--   0        0        0     1396 2024-02-07 20:41:23.718786 vocalpy-0.8.2/docs/api/index.rst
--rw-r--r--   0        0        0     3157 2024-02-01 04:06:36.213088 vocalpy-0.8.2/docs/conf.py
--rw-r--r--   0        0        0    17033 2023-09-19 17:23:06.009955 vocalpy-0.8.2/docs/fa2023/FA2023_template.tex
--rw-r--r--   0        0        0  1735302 2023-09-19 18:23:52.210288 vocalpy-0.8.2/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf
--rw-r--r--   0        0        0     8966 2023-09-19 17:23:06.009955 vocalpy-0.8.2/docs/fa2023/fa2023.sty
--rw-r--r--   0        0        0  1008143 2023-08-20 18:48:42.058440 vocalpy-0.8.2/docs/fa2023/footer_logo_aia.png
--rw-r--r--   0        0        0   313241 2023-08-20 18:48:42.062440 vocalpy-0.8.2/docs/fa2023/footer_logo_eaa.jpg
--rw-r--r--   0        0        0    10783 2023-08-20 18:48:42.062440 vocalpy-0.8.2/docs/fa2023/forum-acusticum-2023.bib
--rw-r--r--   0        0        0    18787 2023-08-20 18:48:42.062440 vocalpy-0.8.2/docs/fa2023/header.png
--rw-r--r--   0        0        0    39228 2023-08-20 18:48:42.062440 vocalpy-0.8.2/docs/fa2023/header_onda.png
--rw-r--r--   0        0        0    17958 2024-02-03 13:05:38.608298 vocalpy-0.8.2/docs/fa2023/main.tex
--rw-r--r--   0        0        0   118445 2023-08-20 18:48:42.070440 vocalpy-0.8.2/docs/fa2023/voc-fig1-model.png
--rw-r--r--   0        0        0      141 2024-01-26 17:19:50.211528 vocalpy-0.8.2/docs/getting_started/index.md
--rw-r--r--   0        0        0     2503 2024-01-26 17:19:50.211528 vocalpy-0.8.2/docs/getting_started/installation.md
--rw-r--r--   0        0        0    10048 2024-02-07 20:41:23.718786 vocalpy-0.8.2/docs/getting_started/quickstart.md
--rw-r--r--   0        0        0     3554 2024-01-26 17:19:50.211528 vocalpy-0.8.2/docs/index.md
--rw-r--r--   0        0        0      800 2023-08-20 18:48:42.070440 vocalpy-0.8.2/docs/make.bat
--rw-r--r--   0        0        0      881 2023-09-19 17:23:06.009955 vocalpy-0.8.2/docs/nitpick-ignore.txt
--rw-r--r--   0        0        0     4147 2024-01-26 17:19:50.211528 vocalpy-0.8.2/docs/user/background.md
--rw-r--r--   0        0        0       41 2024-01-26 17:19:50.211528 vocalpy-0.8.2/docs/user/howto/index.md
--rw-r--r--   0        0        0      331 2024-01-26 17:19:50.211528 vocalpy-0.8.2/docs/user/index.md
--rw-r--r--   0        0        0     9538 2024-02-07 20:41:23.718786 vocalpy-0.8.2/docs/user/whatisvocalpy.md
--rw-r--r--   0        0        0     7308 2023-12-30 01:52:55.169763 vocalpy-0.8.2/noxfile.py
--rw-r--r--   0        0        0     1997 2024-02-08 02:26:16.189193 vocalpy-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    19133 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/scripts/attrs-sqlalchemy.ipynb
--rw-r--r--   0        0        0     5151 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/scripts/carpentries-sql-practice.ipynb
--rw-r--r--   0        0        0    46531 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/scripts/dataclass-orm.ipynb
--rw-r--r--   0        0        0    21715 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/scripts/dataset.ipynb
--rw-r--r--   0        0        0     3130 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/scripts/sqlite-python-tutorial.ipynb
--rw-r--r--   0        0        0    22868 2023-10-01 23:04:49.583877 vocalpy-0.8.2/src/scripts/vocalpy-sqlalchemy-orm.ipynb
--rw-r--r--   0        0        0      804 2024-02-08 02:26:16.201193 vocalpy-0.8.2/src/vocalpy/__about__.py
--rw-r--r--   0        0        0     1712 2024-02-07 20:41:23.718786 vocalpy-0.8.2/src/vocalpy/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 17:19:50.211528 vocalpy-0.8.2/src/vocalpy/_spectrogram/__init__.py
--rw-r--r--   0        0        0     7867 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/_spectrogram/data_type.py
--rw-r--r--   0        0        0       36 2024-02-02 04:13:39.394112 vocalpy-0.8.2/src/vocalpy/_vendor/__init__.py
--rw-r--r--   0        0        0     6910 2024-02-02 04:13:39.398112 vocalpy-0.8.2/src/vocalpy/_vendor/evfuncs.py
--rw-r--r--   0        0        0     1092 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/vocalpy/annotation.py
--rw-r--r--   0        0        0     1895 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/vocalpy/annotation_file.py
--rw-r--r--   0        0        0        0 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/vocalpy/annotator.py
--rw-r--r--   0        0        0     7761 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/audio.py
--rw-r--r--   0        0        0      635 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/vocalpy/audio_file.py
--rw-r--r--   0        0        0       78 2023-09-28 11:53:11.545674 vocalpy-0.8.2/src/vocalpy/constants.py
--rw-r--r--   0        0        0      177 2023-09-12 01:52:43.314986 vocalpy-0.8.2/src/vocalpy/dataset/__init__.py
--rw-r--r--   0        0        0       54 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/vocalpy/dataset/schema/__init__.py
--rw-r--r--   0        0        0     3136 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/vocalpy/dataset/schema/orm.py
--rw-r--r--   0        0        0     2085 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/dataset/schema/sequence.py
--rw-r--r--   0        0        0     8833 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/dataset/sequence.py
--rw-r--r--   0        0        0     2581 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/dataset_file.py
--rw-r--r--   0        0        0   240044 2024-01-26 17:19:50.215528 vocalpy-0.8.2/src/vocalpy/examples/BM003.wav
--rw-r--r--   0        0        0      118 2024-02-01 04:06:36.213088 vocalpy-0.8.2/src/vocalpy/examples/__init__.py
--rw-r--r--   0        0        0     3388 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/examples/_registry.py
--rw-r--r--   0        0        0   142638 2024-01-26 17:19:50.215528 vocalpy-0.8.2/src/vocalpy/examples/bells.wav
--rw-r--r--   0        0        0   126320 2024-01-26 17:19:50.215528 vocalpy-0.8.2/src/vocalpy/examples/flashcam.wav
--rw-r--r--   0        0        0   130946 2024-01-26 17:19:50.219528 vocalpy-0.8.2/src/vocalpy/examples/samba.wav
--rw-r--r--   0        0        0   100696 2024-01-26 17:19:50.219528 vocalpy-0.8.2/src/vocalpy/examples/simple.wav
--rw-r--r--   0        0        0       62 2024-01-26 17:19:50.219528 vocalpy-0.8.2/src/vocalpy/feature/__init__.py
--rw-r--r--   0        0        0    16755 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/feature/sat.py
--rw-r--r--   0        0        0        0 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/vocalpy/feature_extractor.py
--rw-r--r--   0        0        0     1918 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/vocalpy/feature_file.py
--rw-r--r--   0        0        0      126 2023-09-28 01:29:32.668511 vocalpy-0.8.2/src/vocalpy/metrics/__init__.py
--rw-r--r--   0        0        0       85 2023-09-28 01:29:32.668511 vocalpy-0.8.2/src/vocalpy/metrics/segmentation/__init__.py
--rw-r--r--   0        0        0    31255 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/metrics/segmentation/ir.py
--rw-r--r--   0        0        0     1159 2023-09-29 20:50:59.859125 vocalpy-0.8.2/src/vocalpy/paths.py
--rw-r--r--   0        0        0      309 2023-09-28 11:53:11.545674 vocalpy-0.8.2/src/vocalpy/plot/__init__.py
--rw-r--r--   0        0        0     7258 2023-09-12 01:52:43.314986 vocalpy-0.8.2/src/vocalpy/plot/annot.py
--rw-r--r--   0        0        0     4492 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/plot/spect.py
--rw-r--r--   0        0        0      376 2023-10-03 01:08:03.615357 vocalpy-0.8.2/src/vocalpy/segment/__init__.py
--rw-r--r--   0        0        0    13395 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/segment/ava.py
--rw-r--r--   0        0        0     3601 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/segment/meansquared.py
--rw-r--r--   0        0        0     5044 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/segmenter.py
--rw-r--r--   0        0        0     2448 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/sequence.py
--rw-r--r--   0        0        0      109 2024-01-26 17:19:50.219528 vocalpy-0.8.2/src/vocalpy/signal/__init__.py
--rw-r--r--   0        0        0     3807 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/signal/audio.py
--rw-r--r--   0        0        0      885 2024-01-26 17:19:50.219528 vocalpy-0.8.2/src/vocalpy/signal/filter.py
--rw-r--r--   0        0        0       64 2024-01-26 17:19:50.219528 vocalpy-0.8.2/src/vocalpy/spectral/__init__.py
--rw-r--r--   0        0        0     5533 2024-02-08 02:24:01.626046 vocalpy-0.8.2/src/vocalpy/spectral/sat.py
--rw-r--r--   0        0        0     2233 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/spectrogram.py
--rw-r--r--   0        0        0     1491 2023-08-20 18:48:42.070440 vocalpy-0.8.2/src/vocalpy/spectrogram_file.py
--rw-r--r--   0        0        0     8443 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/spectrogram_maker.py
--rw-r--r--   0        0        0      734 2024-01-26 17:19:50.219528 vocalpy-0.8.2/src/vocalpy/spectrogram_parameters.py
--rw-r--r--   0        0        0     1576 2024-02-07 20:41:23.722786 vocalpy-0.8.2/src/vocalpy/unit.py
--rw-r--r--   0        0        0      356 2023-09-28 11:53:11.545674 vocalpy-0.8.2/src/vocalpy/validators/__init__.py
--rw-r--r--   0        0        0      699 2023-09-28 11:53:11.545674 vocalpy-0.8.2/src/vocalpy/validators/attrs.py
--rw-r--r--   0        0        0     4567 2023-12-30 01:52:55.173763 vocalpy-0.8.2/src/vocalpy/validators/validators.py
--rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.8.2/tests/__init__.py
--rw-r--r--   0        0        0       24 2023-04-18 02:08:12.226241 vocalpy-0.8.2/tests/conftest.py
--rw-r--r--   0        0        0      112 2023-08-20 18:48:42.070440 vocalpy-0.8.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2744 2023-09-19 17:23:06.009955 vocalpy-0.8.2/tests/fixtures/annot.py
--rw-r--r--   0        0        0     5420 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/fixtures/audio.py
--rw-r--r--   0        0        0     1121 2023-09-19 19:34:56.374727 vocalpy-0.8.2/tests/fixtures/datasets.py
--rw-r--r--   0        0        0      208 2023-09-19 19:34:56.374727 vocalpy-0.8.2/tests/fixtures/segments.py
--rw-r--r--   0        0        0     6642 2024-01-26 17:19:50.223528 vocalpy-0.8.2/tests/fixtures/spect.py
--rw-r--r--   0        0        0     1265 2023-09-19 19:34:56.374727 vocalpy-0.8.2/tests/fixtures/test_data.py
--rw-r--r--   0        0        0     2147 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/scripts/generate_data_for_tests.py
--rw-r--r--   0        0        0        0 2024-01-26 17:19:50.223528 vocalpy-0.8.2/tests/test__spectrogram/__init__.py
--rw-r--r--   0        0        0     4186 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test__spectrogram/test_data_type.py
--rw-r--r--   0        0        0     2695 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_annotation_file.py
--rw-r--r--   0        0        0     8775 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_audio.py
--rw-r--r--   0        0        0      992 2023-08-20 18:48:42.074440 vocalpy-0.8.2/tests/test_audio_file.py
--rw-r--r--   0        0        0        0 2023-08-20 18:48:42.074440 vocalpy-0.8.2/tests/test_dataset/__init__.py
--rw-r--r--   0        0        0      988 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_dataset/test_sequence.py
--rw-r--r--   0        0        0        0 2024-01-26 17:19:50.223528 vocalpy-0.8.2/tests/test_examples/__init__.py
--rw-r--r--   0        0        0      863 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_examples/test__registry.py
--rw-r--r--   0        0        0        0 2023-12-30 01:52:55.173763 vocalpy-0.8.2/tests/test_feature/__init__.py
--rw-r--r--   0        0        0     3886 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_feature/test_sat.py
--rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.8.2/tests/test_metrics/__init__.py
--rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.8.2/tests/test_metrics/test_segmentation/__init__.py
--rw-r--r--   0        0        0    26736 2024-02-01 13:56:56.788699 vocalpy-0.8.2/tests/test_metrics/test_segmentation/test_ir.py
--rw-r--r--   0        0        0     2819 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_paths.py
--rw-r--r--   0        0        0     1308 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_segment/test_ava.py
--rw-r--r--   0        0        0      582 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_segment/test_meansquared.py
--rw-r--r--   0        0        0     2236 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_segmenter.py
--rw-r--r--   0        0        0      547 2023-08-20 18:48:42.074440 vocalpy-0.8.2/tests/test_sequence.py
--rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.8.2/tests/test_signal/__init__.py
--rw-r--r--   0        0        0      546 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_signal/test_audio.py
--rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.8.2/tests/test_signal/test_spectrogram.py
--rw-r--r--   0        0        0        0 2023-12-30 01:52:55.173763 vocalpy-0.8.2/tests/test_spectral/__init__.py
--rw-r--r--   0        0        0      544 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_spectral/test_sat.py
--rw-r--r--   0        0        0      989 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_spectrogram.py
--rw-r--r--   0        0        0     1500 2023-08-20 18:48:42.074440 vocalpy-0.8.2/tests/test_spectrogram_file.py
--rw-r--r--   0        0        0     4457 2024-02-07 20:41:23.722786 vocalpy-0.8.2/tests/test_spectrogram_maker.py
--rw-r--r--   0        0        0      848 2023-08-20 18:48:42.074440 vocalpy-0.8.2/tests/test_unit.py
--rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.8.2/tests/test_validators/__init__.py
--rw-r--r--   0        0        0     3272 2023-12-30 01:52:55.173763 vocalpy-0.8.2/tests/test_validators/test_validators.py
--rw-r--r--   0        0        0        0 2024-02-02 04:13:39.398112 vocalpy-0.8.2/tests/test_vendor/__init__.py
--rw-r--r--   0        0        0     1280 2024-02-02 04:13:39.398112 vocalpy-0.8.2/tests/test_vendor/test_evfuncs.py
--rw-r--r--   0        0        0    17188 1970-01-01 00:00:00.000000 vocalpy-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      650 2024-01-26 17:19:50.207528 vocalpy-0.9.0/.all-contributorsrc
+-rw-r--r--   0        0        0     1307 2023-09-19 17:23:06.009955 vocalpy-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2023-08-20 18:48:42.054440 vocalpy-0.9.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      615 2023-08-20 18:48:42.054440 vocalpy-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      705 2024-01-17 01:58:19.551347 vocalpy-0.9.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      463 2024-02-22 13:15:42.873235 vocalpy-0.9.0/.gitignore
+-rw-r--r--   0        0        0      769 2023-08-20 18:48:42.054440 vocalpy-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      334 2023-09-29 20:50:59.859125 vocalpy-0.9.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     5556 2023-09-19 17:23:06.009955 vocalpy-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1867 2023-08-20 18:48:42.054440 vocalpy-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1540 2023-04-18 02:08:12.226241 vocalpy-0.9.0/LICENSE
+-rw-r--r--   0        0        0    15851 2024-02-12 02:46:58.472428 vocalpy-0.9.0/README.md
+-rw-r--r--   0        0        0       46 2024-02-24 00:45:51.665844 vocalpy-0.9.0/codecov.yml
+-rw-r--r--   0        0        0     8562 2024-05-16 03:54:52.513377 vocalpy-0.9.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0      775 2024-02-22 13:15:42.873235 vocalpy-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0    29965 2023-08-20 18:48:42.054440 vocalpy-0.9.0/docs/_static/vocalpy-logomark.png
+-rw-r--r--   0        0        0   285798 2023-08-20 18:48:42.054440 vocalpy-0.9.0/docs/_static/vocalpy-primary.png
+-rw-r--r--   0        0        0   194159 2023-08-20 18:48:42.054440 vocalpy-0.9.0/docs/_static/vocalpy-secondary.png
+-rw-r--r--   0        0        0      612 2023-12-30 13:28:54.397449 vocalpy-0.9.0/docs/_templates/class.rst
+-rw-r--r--   0        0        0     1177 2023-12-30 13:28:54.397449 vocalpy-0.9.0/docs/_templates/module.rst
+-rw-r--r--   0        0        0     1279 2024-05-16 03:52:17.046400 vocalpy-0.9.0/docs/api/index.rst
+-rw-r--r--   0        0        0     3862 2024-04-02 23:44:46.834318 vocalpy-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0    17033 2023-09-19 17:23:06.009955 vocalpy-0.9.0/docs/fa2023/FA2023_template.tex
+-rw-r--r--   0        0        0  1735302 2023-09-19 18:23:52.210288 vocalpy-0.9.0/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf
+-rw-r--r--   0        0        0     8966 2023-09-19 17:23:06.009955 vocalpy-0.9.0/docs/fa2023/fa2023.sty
+-rw-r--r--   0        0        0  1008143 2023-08-20 18:48:42.058440 vocalpy-0.9.0/docs/fa2023/footer_logo_aia.png
+-rw-r--r--   0        0        0   313241 2023-08-20 18:48:42.062440 vocalpy-0.9.0/docs/fa2023/footer_logo_eaa.jpg
+-rw-r--r--   0        0        0    10783 2023-08-20 18:48:42.062440 vocalpy-0.9.0/docs/fa2023/forum-acusticum-2023.bib
+-rw-r--r--   0        0        0    18787 2023-08-20 18:48:42.062440 vocalpy-0.9.0/docs/fa2023/header.png
+-rw-r--r--   0        0        0    39228 2023-08-20 18:48:42.062440 vocalpy-0.9.0/docs/fa2023/header_onda.png
+-rw-r--r--   0        0        0    17958 2024-02-03 13:05:38.608298 vocalpy-0.9.0/docs/fa2023/main.tex
+-rw-r--r--   0        0        0   118445 2023-08-20 18:48:42.070440 vocalpy-0.9.0/docs/fa2023/voc-fig1-model.png
+-rw-r--r--   0        0        0      141 2024-01-26 17:19:50.211528 vocalpy-0.9.0/docs/getting_started/index.md
+-rw-r--r--   0        0        0     2503 2024-01-26 17:19:50.211528 vocalpy-0.9.0/docs/getting_started/installation.md
+-rw-r--r--   0        0        0    10248 2024-04-03 03:02:45.940030 vocalpy-0.9.0/docs/getting_started/quickstart.md
+-rw-r--r--   0        0        0     3554 2024-01-26 17:19:50.211528 vocalpy-0.9.0/docs/index.md
+-rw-r--r--   0        0        0      800 2023-08-20 18:48:42.070440 vocalpy-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0      881 2023-09-19 17:23:06.009955 vocalpy-0.9.0/docs/nitpick-ignore.txt
+-rw-r--r--   0        0        0     4147 2024-01-26 17:19:50.211528 vocalpy-0.9.0/docs/user/background.md
+-rw-r--r--   0        0        0       67 2024-04-03 03:02:45.940030 vocalpy-0.9.0/docs/user/howto/index.md
+-rw-r--r--   0        0        0    15636 2024-04-09 02:06:31.842592 vocalpy-0.9.0/docs/user/howto/segmentation-ir-metrics.md
+-rw-r--r--   0        0        0      343 2024-04-03 03:02:45.940030 vocalpy-0.9.0/docs/user/index.md
+-rw-r--r--   0        0        0    10030 2024-02-12 02:46:58.472428 vocalpy-0.9.0/docs/user/whatisvocalpy.md
+-rw-r--r--   0        0        0     8492 2024-02-24 00:45:51.665844 vocalpy-0.9.0/noxfile.py
+-rw-r--r--   0        0        0     2438 2024-05-16 03:55:24.713165 vocalpy-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.0/src/scripts/example_data/.gitkeep
+-rw-r--r--   0        0        0     6836 2024-02-22 13:15:42.873235 vocalpy-0.9.0/src/scripts/make_example_data.py
+-rw-r--r--   0        0        0      804 2024-05-16 03:55:24.705165 vocalpy-0.9.0/src/vocalpy/__about__.py
+-rw-r--r--   0        0        0     1866 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 17:19:50.211528 vocalpy-0.9.0/src/vocalpy/_spectrogram/__init__.py
+-rw-r--r--   0        0        0     9382 2024-04-09 12:04:39.858685 vocalpy-0.9.0/src/vocalpy/_spectrogram/data_type.py
+-rw-r--r--   0        0        0       36 2024-02-12 02:46:58.472428 vocalpy-0.9.0/src/vocalpy/_vendor/__init__.py
+-rw-r--r--   0        0        0     6910 2024-02-12 02:46:58.472428 vocalpy-0.9.0/src/vocalpy/_vendor/evfuncs.py
+-rw-r--r--   0        0        0     1092 2023-08-20 18:48:42.070440 vocalpy-0.9.0/src/vocalpy/annotation.py
+-rw-r--r--   0        0        0     1830 2024-04-09 12:04:39.858685 vocalpy-0.9.0/src/vocalpy/annotation_file.py
+-rw-r--r--   0        0        0        0 2023-08-20 18:48:42.070440 vocalpy-0.9.0/src/vocalpy/annotator.py
+-rw-r--r--   0        0        0      541 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/audio_file.py
+-rw-r--r--   0        0        0       78 2023-09-28 11:53:11.545674 vocalpy-0.9.0/src/vocalpy/constants.py
+-rw-r--r--   0        0        0     2479 2024-04-09 12:04:39.858685 vocalpy-0.9.0/src/vocalpy/dataset_file.py
+-rw-r--r--   0        0        0   240044 2024-01-26 17:19:50.215528 vocalpy-0.9.0/src/vocalpy/examples/BM003.wav
+-rw-r--r--   0        0        0      186 2024-02-22 13:15:42.873235 vocalpy-0.9.0/src/vocalpy/examples/__init__.py
+-rw-r--r--   0        0        0    10264 2024-04-09 12:04:39.858685 vocalpy-0.9.0/src/vocalpy/examples/_examples.py
+-rw-r--r--   0        0        0   142638 2024-01-26 17:19:50.215528 vocalpy-0.9.0/src/vocalpy/examples/bells.wav
+-rw-r--r--   0        0        0   126320 2024-01-26 17:19:50.215528 vocalpy-0.9.0/src/vocalpy/examples/flashcam.wav
+-rw-r--r--   0        0        0   130946 2024-01-26 17:19:50.219528 vocalpy-0.9.0/src/vocalpy/examples/samba.wav
+-rw-r--r--   0        0        0   100696 2024-01-26 17:19:50.219528 vocalpy-0.9.0/src/vocalpy/examples/simple.wav
+-rw-r--r--   0        0        0       95 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/__init__.py
+-rw-r--r--   0        0        0    20055 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/sat.py
+-rw-r--r--   0        0        0       95 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/__init__.py
+-rw-r--r--   0        0        0     6840 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/detect_peaks.py
+-rw-r--r--   0        0        0    17164 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/features.py
+-rw-r--r--   0        0        0    20246 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/fundamental.py
+-rw-r--r--   0        0        0     3940 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/signal.py
+-rw-r--r--   0        0        0     1690 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature/soundsig/sound.py
+-rw-r--r--   0        0        0     5185 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/feature_extractor.py
+-rw-r--r--   0        0        0     1869 2024-04-09 12:04:39.862685 vocalpy-0.9.0/src/vocalpy/feature_file.py
+-rw-r--r--   0        0        0     1401 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/features.py
+-rw-r--r--   0        0        0      126 2023-09-28 01:29:32.668511 vocalpy-0.9.0/src/vocalpy/metrics/__init__.py
+-rw-r--r--   0        0        0      172 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/metrics/segmentation/__init__.py
+-rw-r--r--   0        0        0    31339 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/metrics/segmentation/ir.py
+-rw-r--r--   0        0        0      882 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/params.py
+-rw-r--r--   0        0        0     1159 2023-09-29 20:50:59.859125 vocalpy-0.9.0/src/vocalpy/paths.py
+-rw-r--r--   0        0        0      309 2023-09-28 11:53:11.545674 vocalpy-0.9.0/src/vocalpy/plot/__init__.py
+-rw-r--r--   0        0        0     7258 2023-09-12 01:52:43.314986 vocalpy-0.9.0/src/vocalpy/plot/annot.py
+-rw-r--r--   0        0        0     5230 2024-04-09 12:04:39.862685 vocalpy-0.9.0/src/vocalpy/plot/spect.py
+-rw-r--r--   0        0        0      508 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/segment/__init__.py
+-rw-r--r--   0        0        0    20942 2024-04-09 12:04:39.862685 vocalpy-0.9.0/src/vocalpy/segment/ava.py
+-rw-r--r--   0        0        0     9565 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/segment/meansquared.py
+-rw-r--r--   0        0        0     5402 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/segmenter.py
+-rw-r--r--   0        0        0    22648 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/segments.py
+-rw-r--r--   0        0        0      928 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/sequence.py
+-rw-r--r--   0        0        0      109 2024-01-26 17:19:50.219528 vocalpy-0.9.0/src/vocalpy/signal/__init__.py
+-rw-r--r--   0        0        0     4370 2024-02-12 02:46:58.476428 vocalpy-0.9.0/src/vocalpy/signal/audio.py
+-rw-r--r--   0        0        0      644 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/signal/filter.py
+-rw-r--r--   0        0        0     7811 2024-04-03 03:02:45.944030 vocalpy-0.9.0/src/vocalpy/sound.py
+-rw-r--r--   0        0        0      219 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectral/__init__.py
+-rw-r--r--   0        0        0     6273 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectral/sat.py
+-rw-r--r--   0        0        0     6675 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectral/soundsig.py
+-rw-r--r--   0        0        0     3205 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectrogram.py
+-rw-r--r--   0        0        0     1442 2024-04-09 12:04:39.862685 vocalpy-0.9.0/src/vocalpy/spectrogram_file.py
+-rw-r--r--   0        0        0     9448 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/spectrogram_maker.py
+-rw-r--r--   0        0        0      734 2024-01-26 17:19:50.219528 vocalpy-0.9.0/src/vocalpy/spectrogram_parameters.py
+-rw-r--r--   0        0        0     1576 2024-03-06 03:50:43.265345 vocalpy-0.9.0/src/vocalpy/unit.py
+-rw-r--r--   0        0        0      356 2023-09-28 11:53:11.545674 vocalpy-0.9.0/src/vocalpy/validators/__init__.py
+-rw-r--r--   0        0        0      699 2023-09-28 11:53:11.545674 vocalpy-0.9.0/src/vocalpy/validators/attrs.py
+-rw-r--r--   0        0        0     4936 2024-05-16 03:52:17.046400 vocalpy-0.9.0/src/vocalpy/validators/validators.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-18 02:08:12.226241 vocalpy-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      224 2024-05-16 03:52:17.046400 vocalpy-0.9.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2744 2023-09-19 17:23:06.009955 vocalpy-0.9.0/tests/fixtures/annot.py
+-rw-r--r--   0        0        0     3351 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/fixtures/audio.py
+-rw-r--r--   0        0        0      134 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/fixtures/dask.py
+-rw-r--r--   0        0        0      834 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/fixtures/datasets.py
+-rw-r--r--   0        0        0      210 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/fixtures/paths.py
+-rw-r--r--   0        0        0      983 2024-02-24 00:45:51.669844 vocalpy-0.9.0/tests/fixtures/segments.py
+-rw-r--r--   0        0        0     2942 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/fixtures/spect.py
+-rw-r--r--   0        0        0     1278 2024-02-24 00:45:51.669844 vocalpy-0.9.0/tests/fixtures/test_data.py
+-rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/scripts/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/scripts/generate_ava_segment_test_data/__init__.py
+-rw-r--r--   0        0        0     9340 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/scripts/generate_ava_segment_test_data/generate_ava_segment_text_files_from_jourjine_et_al_2023.py
+-rw-r--r--   0        0        0     1126 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/scripts/generate_ava_segment_test_data/generate_test_audio_for_ava_segment_from_jourjine_etal_2023.py
+-rw-r--r--   0        0        0     7048 2024-02-24 00:45:51.669844 vocalpy-0.9.0/tests/scripts/generate_data_for_tests.py
+-rw-r--r--   0        0        0        0 2024-01-26 17:19:50.223528 vocalpy-0.9.0/tests/test__spectrogram/__init__.py
+-rw-r--r--   0        0        0     9635 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test__spectrogram/test_data_type.py
+-rw-r--r--   0        0        0     2719 2024-03-06 03:50:43.265345 vocalpy-0.9.0/tests/test_annotation_file.py
+-rw-r--r--   0        0        0      992 2024-03-06 03:50:43.265345 vocalpy-0.9.0/tests/test_audio_file.py
+-rw-r--r--   0        0        0        0 2024-01-26 17:19:50.223528 vocalpy-0.9.0/tests/test_examples/__init__.py
+-rw-r--r--   0        0        0      915 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/test_examples/test__examples.py
+-rw-r--r--   0        0        0        0 2023-12-30 01:52:55.173763 vocalpy-0.9.0/tests/test_feature/__init__.py
+-rw-r--r--   0        0        0     8644 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_feature/test_sat.py
+-rw-r--r--   0        0        0      206 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_feature_extractor.py
+-rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.9.0/tests/test_metrics/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.9.0/tests/test_metrics/test_segmentation/__init__.py
+-rw-r--r--   0        0        0    26736 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_metrics/test_segmentation/test_ir.py
+-rw-r--r--   0        0        0      895 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/test_params.py
+-rw-r--r--   0        0        0     2903 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_paths.py
+-rw-r--r--   0        0        0        0 2024-02-22 13:15:42.873235 vocalpy-0.9.0/tests/test_segment/__init__.py
+-rw-r--r--   0        0        0     3062 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/test_segment/test_ava.py
+-rw-r--r--   0        0        0     2276 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/test_segment/test_meansquared.py
+-rw-r--r--   0        0        0     3222 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_segmenter.py
+-rw-r--r--   0        0        0    23811 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_segments.py
+-rw-r--r--   0        0        0      487 2024-04-03 03:02:45.944030 vocalpy-0.9.0/tests/test_sequence.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.9.0/tests/test_signal/__init__.py
+-rw-r--r--   0        0        0      886 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_signal/test_audio.py
+-rw-r--r--   0        0        0        0 2023-04-18 02:08:12.226241 vocalpy-0.9.0/tests/test_signal/test_spectrogram.py
+-rw-r--r--   0        0        0     8822 2024-02-24 00:45:51.669844 vocalpy-0.9.0/tests/test_sound.py
+-rw-r--r--   0        0        0        0 2023-12-30 01:52:55.173763 vocalpy-0.9.0/tests/test_spectral/__init__.py
+-rw-r--r--   0        0        0     1187 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_spectral/test_sat.py
+-rw-r--r--   0        0        0     1007 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_spectrogram.py
+-rw-r--r--   0        0        0     1500 2024-03-06 03:50:43.265345 vocalpy-0.9.0/tests/test_spectrogram_file.py
+-rw-r--r--   0        0        0     4628 2024-05-16 03:52:17.050400 vocalpy-0.9.0/tests/test_spectrogram_maker.py
+-rw-r--r--   0        0        0      848 2024-03-06 03:50:43.265345 vocalpy-0.9.0/tests/test_unit.py
+-rw-r--r--   0        0        0        0 2023-09-28 01:29:32.668511 vocalpy-0.9.0/tests/test_validators/__init__.py
+-rw-r--r--   0        0        0     3272 2023-12-30 01:52:55.173763 vocalpy-0.9.0/tests/test_validators/test_validators.py
+-rw-r--r--   0        0        0        0 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_vendor/__init__.py
+-rw-r--r--   0        0        0     1280 2024-02-12 02:46:58.476428 vocalpy-0.9.0/tests/test_vendor/test_evfuncs.py
+-rw-r--r--   0        0        0    18176 1970-01-01 00:00:00.000000 vocalpy-0.9.0/PKG-INFO
```

### Comparing `vocalpy-0.8.2/.all-contributorsrc` & `vocalpy-0.9.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md` & `vocalpy-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md` & `vocalpy-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/.github/workflows/ci.yml` & `vocalpy-0.9.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/.pre-commit-config.yaml` & `vocalpy-0.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/CODE_OF_CONDUCT.md` & `vocalpy-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/CONTRIBUTING.md` & `vocalpy-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/LICENSE` & `vocalpy-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/README.md` & `vocalpy-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -53,28 +53,29 @@
 
 [^1]: For a curated collection, see <https://github.com/rhine3/bioacoustics-software>.
 
 ## Features
 
 ###  Data types for acoustic communication data: audio, spectrogram, annotations, features
 
-#### The `vocalpy.Audio` data type
+#### The `vocalpy.Sound` data type
 
 - Works with a wide array of audio formats, thanks to [soundfile](https://github.com/bastibe/python-soundfile).
 - Also works with the cbin audio format saved by the LabView app EvTAF used by many neuroscience labs studying birdsong,
   thanks to [evfuncs](https://github.com/NickleDave/evfuncs).
 
 ```python
->>> import vocalpy as voc
->>> data_dir = ('tests/data-for-tests/source/audio_wav_annot_birdsongrec/Bird0/Wave/')
->>> wav_paths = voc.paths.from_dir(data_dir, 'wav')
->>> audios = [voc.Audio.read(wav_path) for wav_path in wav_paths]
->>> print(audios[0])
-vocalpy.Audio(data=array([3.0517...66210938e-04]), samplerate=32000, channels=1), 
-path=tests/data-for-tests/source/audio_wav_annot_birdsongrec/Bird0/Wave/0.wav)
+>> > import vocalpy as voc
+>> > data_dir = ('tests/data-for-tests/source/audio_wav_annot_birdsongrec/Bird0/Wave/')
+>> > wav_paths = voc.paths.from_dir(data_dir, 'wav')
+>> > audios = [voc.Sound.read(wav_path) for wav_path in wav_paths]
+>> > print(audios[0])
+vocalpy.Sound(data=array([3.0517...66210938e-04]), samplerate=32000, channels=1),
+path = tests / data -
+for -tests / source / audio_wav_annot_birdsongrec / Bird0 / Wave / 0.wav)
 ```
 
 #### The `vocalpy.Spectrogram` data type
 
 - Save expensive-to-compute spectrograms to array files, so you don't regenerate them over and over again
 
 ```python
@@ -103,49 +104,60 @@
 ```
 
 ### Classes for common steps in your pipelines and workflows
 
 #### A `Segmenter` for segmentation into sequences of units
 
 ```python
->>> import evfuncs
->>> import vocalpy as voc
->>> data_dir = ('tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/')
->>> cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
->>> audios = [voc.Audio.read(cbin_path) for cbin_path in cbin_paths]
->>> segment_params = {'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006}
->>> segmenter = voc.Segmenter(callback=evfuncs.segment_song, segment_params=segment_params)
->>> seqs = segmenter.segment(audios, parallelize=True)
-[########################################] | 100% Completed | 122.91 ms
->>> print(seqs[1])
-Sequence(units=[Unit(onset=2.19075, offset=2.20428125, label='-', audio=None, spectrogram=None), 
-Unit(onset=2.35478125, offset=2.38815625, label='-', audio=None, spectrogram=None), Unit(onset=2.8410625, offset=2.86715625, label='-', audio=None, spectrogram=None), 
-Unit(onset=3.48234375, offset=3.49371875, label='-', audio=None, spectrogram=None), Unit(onset=3.57021875, offset=3.60296875, label='-', audio=None, spectrogram=None), 
-Unit(onset=3.64403125, offset=3.67721875, label='-', audio=None, spectrogram=None), Unit(onset=3.72228125, offset=3.74478125, label='-', audio=None, spectrogram=None), 
-Unit(onset=3.8036875, offset=3.8158125, label='-', audio=None, spectrogram=None), Unit(onset=3.82328125, offset=3.83646875, label='-', audio=None, spectrogram=None), 
-Unit(onset=4.13759375, offset=4.16346875, label='-', audio=None, spectrogram=None), Unit(onset=4.80278125, offset=4.814, label='-', audio=None, spectrogram=None), 
-Unit(onset=4.908125, offset=4.922875, label='-', audio=None, spectrogram=None), Unit(onset=4.9643125, offset=4.992625, label='-', audio=None, spectrogram=None), 
-Unit(onset=5.039625, offset=5.0506875, label='-', audio=None, spectrogram=None), Unit(onset=5.10165625, offset=5.1385, label='-', audio=None, spectrogram=None), 
-Unit(onset=5.146875, offset=5.16203125, label='-', audio=None, spectrogram=None), Unit(onset=5.46390625, offset=5.49409375, label='-', audio=None, spectrogram=None), 
-Unit(onset=6.14503125, offset=6.1565625, label='-', audio=None, spectrogram=None), Unit(onset=6.31003125, offset=6.346125, label='-', audio=None, spectrogram=None), 
-Unit(onset=6.38996875, offset=6.4018125, label='-', audio=None, spectrogram=None), Unit(onset=6.46053125, offset=6.4796875, label='-', audio=None, spectrogram=None), 
-Unit(onset=6.83525, offset=6.8643125, label='-', audio=None, spectrogram=None)], method='segment_song', 
-segment_params={'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006}, 
-audio=vocalpy.Audio(data=None, samplerate=None, channels=None), path=tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/gy6or6_baseline_230312_0809.141.cbin), spectrogram=None)
+>> > import evfuncs
+>> > import vocalpy as voc
+>> > data_dir = ('tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/')
+>> > cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
+>> > audios = [voc.Sound.read(cbin_path) for cbin_path in cbin_paths]
+>> > segment_params = {'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006}
+>> > segmenter = voc.Segmenter(callback=evfuncs.segment_song, segment_params=segment_params)
+>> > seqs = segmenter.segment(audios, parallelize=True)
+[  ########################################] | 100% Completed | 122.91 ms
+>> > print(seqs[1])
+Sequence(units=[Unit(onset=2.19075, offset=2.20428125, label='-', audio=None, spectrogram=None),
+                Unit(onset=2.35478125, offset=2.38815625, label='-', audio=None, spectrogram=None),
+                Unit(onset=2.8410625, offset=2.86715625, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.48234375, offset=3.49371875, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.57021875, offset=3.60296875, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.64403125, offset=3.67721875, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.72228125, offset=3.74478125, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.8036875, offset=3.8158125, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.82328125, offset=3.83646875, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.13759375, offset=4.16346875, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.80278125, offset=4.814, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.908125, offset=4.922875, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.9643125, offset=4.992625, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.039625, offset=5.0506875, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.10165625, offset=5.1385, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.146875, offset=5.16203125, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.46390625, offset=5.49409375, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.14503125, offset=6.1565625, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.31003125, offset=6.346125, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.38996875, offset=6.4018125, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.46053125, offset=6.4796875, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.83525, offset=6.8643125, label='-', audio=None, spectrogram=None)], method='segment_song',
+         segment_params={'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006},
+         audio=vocalpy.Sound(data=None, samplerate=None, channels=None), path=tests / data -
+for -tests / source / audio_cbin_annot_notmat / gy6or6 / 032312 / gy6or6_baseline_230312_0809.141.cbin), spectrogram=None)
 ```
  
 #### A `SpectrogramMaker` for computing spectrograms
 
 ```python
->>> import vocalpy as voc
->>> wav_paths = voc.paths.from_dir('wav')
->>> audios = [voc.Audio(wav_path) for wav_path in wav_paths]
->>> spect_params = {'fft_size': 512, 'step_size': 64}
->>> spect_maker = voc.SpectrogramMaker(spect_params=spect_params)
->>> spects = spect_maker.make(audios, parallelize=True)
+>> > import vocalpy as voc
+>> > wav_paths = voc.paths.from_dir('wav')
+>> > audios = [voc.Sound(wav_path) for wav_path in wav_paths]
+>> > spect_params = {'fft_size': 512, 'step_size': 64}
+>> > spect_maker = voc.SpectrogramMaker(spect_params=spect_params)
+>> > spects = spect_maker.make(audios, parallelize=True)
 ```
 
 ### `Dataset`s you flexibly build from pipelines and convert to databases
 
 - The `vocalpy.dataset` module contains classes that represent common types of datasets 
 - You make these classes with outputs of your pipelines, e.g. a `list` of `vocalpy.Sequence`s 
   or `vocalpy.Spectrogram`s
@@ -159,39 +171,43 @@
     [recommended by the US Library of Congress for archival data](https://www.sqlite.org/locrsf.html),
     and it's [built into Python](https://docs.python.org/3/library/sqlite3.html) 
     -- no need to install separate database software like MySQL
 
 #### A `SequenceDataset` for common analyses of sequences of units
 
 ```python
->>> import evfuncs
->>> import vocalpy as voc
->>> data_dir = 'tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/'
->>> cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
->>> audios = [voc.Audio.read(cbin_path) for cbin_path in cbin_paths]
->>> segment_params = {
-    'threshold': 1500,
-    'min_syl_dur': 0.01,
-    'min_silent_dur': 0.006,
+>> > import evfuncs
+>> > import vocalpy as voc
+>> > data_dir = 'tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/'
+>> > cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
+>> > audios = [voc.Sound.read(cbin_path) for cbin_path in cbin_paths]
+>> > segment_params = {
+  'threshold': 1500,
+  'min_syl_dur': 0.01,
+  'min_silent_dur': 0.006,
 }
->>> segmenter = voc.Segmenter(
-    callback=evfuncs.segment_song, 
-    segment_params=segment_params
+>> > segmenter = voc.Segmenter(
+  callback=evfuncs.segment_song,
+  segment_params=segment_params
 )
->>> seqs = segmenter.segment(audios)
->>> seq_dataset = voc.dataset.SequenceDataset(sequences=seqs)
->>> seq_dataset.to_sqlite(db_name='gy6or6-032312.db', replace=True)
->>> print(seq_dataset)
+>> > seqs = segmenter.segment(audios)
+>> > seq_dataset = voc.dataset.SequenceDataset(sequences=seqs)
+>> > seq_dataset.to_sqlite(db_name='gy6or6-032312.db', replace=True)
+>> > print(seq_dataset)
 SequenceDataset(sequences=[Sequence(units=[Unit(onset=2.18934375, offset=2.21, label='-', audio=None, spectrogram=None),
-Unit(onset=2.346125, offset=2.373125, label='-', audio=None, spectrogram=None), Unit(onset=2.50471875, offset=2.51546875,
-label='-', audio=None, spectrogram=None), Unit(onset=2.81909375, offset=2.84740625, label='-', audio=None, spectrogram=None),
-...
->>> # test that we can load the dataset
->>> seq_dataset_loaded = voc.dataset.SequenceDataset.from_sqlite(db_name='gy6or6-032312.db')
->>> seq_dataset_loaded == seq_dataset
+                                           Unit(onset=2.346125, offset=2.373125, label='-', audio=None,
+                                                spectrogram=None), Unit(onset=2.50471875, offset=2.51546875,
+                                                                        label='-', audio=None, spectrogram=None),
+                                           Unit(onset=2.81909375, offset=2.84740625, label='-', audio=None,
+                                                spectrogram=None),
+                                           ...
+                                           >> >  # test that we can load the dataset
+                                          >> > seq_dataset_loaded = voc.dataset.SequenceDataset.from_sqlite(
+  db_name='gy6or6-032312.db')
+                                                                    >> > seq_dataset_loaded == seq_dataset
 True
 ```
 
 
 ## Installation
 #### With `pip`
 ```
```

### Comparing `vocalpy-0.8.2/docs/_static/vocalpy-logomark.png` & `vocalpy-0.9.0/docs/_static/vocalpy-logomark.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/_static/vocalpy-primary.png` & `vocalpy-0.9.0/docs/_static/vocalpy-primary.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/_static/vocalpy-secondary.png` & `vocalpy-0.9.0/docs/_static/vocalpy-secondary.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/_templates/class.rst` & `vocalpy-0.9.0/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/_templates/module.rst` & `vocalpy-0.9.0/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/api/index.rst` & `vocalpy-0.9.0/docs/api/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -14,31 +14,34 @@
 
 Data types for acoustic communication data.
 
 .. autosummary::
    :toctree: generated
    :template: class.rst
 
-   Audio
+   Sound
    Spectrogram
    Annotation
+   Segments
+   Features
 
 
 Classes for Pipelines
 ---------------------
 
-Classes for common steps in your pipelines and workflows
+Classes for common steps in pipelines.
 
 .. autosummary::
    :toctree: generated
    :template: class.rst
 
    Segmenter
    SpectrogramMaker
-   SpectrogramParameters
+   FeatureExtractor
+   Params
 
 Signal processing
 -----------------
 
 .. autosummary::
    :toctree: generated
    :template: module.rst
@@ -67,25 +70,14 @@
    :template: module.rst
    :recursive:
 
    metrics
    metrics.segmentation
    metrics.segmentation.ir
 
-Datasets
---------
-
-.. autosummary::
-   :template: class
-   :toctree: generated
-
-   dataset.SequenceDataset
-   Sequence
-   Unit
-
 Visualization
 -------------
 .. autosummary::
    :toctree: generated
    :template: module.rst
    :recursive:
```

### Comparing `vocalpy-0.8.2/docs/conf.py` & `vocalpy-0.9.0/docs/conf.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,15 +21,17 @@
 srcpath = os.path.abspath(pathlib.Path(os.path.dirname(__file__)) / "..")
 sys.path.insert(0, srcpath)
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
+    'matplotlib.sphinxext.plot_directive',
     'myst_nb',
+    'numpydoc',
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.coverage',
     'sphinx_copybutton',
     'sphinx.ext.doctest',
     'sphinx.ext.intersphinx',
     'sphinx.ext.todo',
@@ -38,14 +40,17 @@
     'sphinx.ext.ifconfig',
     'sphinx.ext.viewcode',
     'sphinx_design',
     'sphinxext.opengraph',
     'sphinx_tabs.tabs',
 ]
 
+numpydoc_use_plots = True
+
+
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 source_suffix = ['.rst', '.md']
 
@@ -84,22 +89,47 @@
 }
 
 html_static_path = ['_static']
 
 # -- Extension configuration -------------------------------------------------
 autosummary_ignore_module_all = False
 
+# -- doctest -----------------------------------------------------------------
+
+doctest_global_setup = """
+import numpy as np
+import vocalpy as voc
+
+np.random.seed(42)
+np.set_printoptions(precision=3, linewidth=64, edgeitems=2, threshold=200)
+"""
+
+plot_pre_code = (
+    doctest_global_setup
+    + """
+import matplotlib
+matplotlib.rcParams['figure.constrained_layout.use'] = True
+"""
+)
+plot_include_source = True
+plot_html_show_source_link = False
+plot_formats = [("png", 100), ("pdf", 100)]
+plot_html_show_formats = False
+
+font_size = 12
+
 # -- Options for intersphinx extension ---------------------------------------
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "librosa": ("https://librosa.org/doc/0.10.0", None),
     "python": ("https://docs.python.org/3/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable/", None),
+    "soundfile": ("https://python-soundfile.readthedocs.io/en/latest/", None),
 }
 
 # -- Options for nitpicky mode
 
 # ensure that all references in the docs resolve.
 nitpicky = True
 nitpick_ignore = []
```

### Comparing `vocalpy-0.8.2/docs/fa2023/FA2023_template.tex` & `vocalpy-0.9.0/docs/fa2023/FA2023_template.tex`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf` & `vocalpy-0.9.0/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/fa2023/fa2023.sty` & `vocalpy-0.9.0/docs/fa2023/fa2023.sty`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/fa2023/footer_logo_aia.png` & `vocalpy-0.9.0/docs/fa2023/footer_logo_aia.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/fa2023/footer_logo_eaa.jpg` & `vocalpy-0.9.0/docs/fa2023/footer_logo_eaa.jpg`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/fa2023/forum-acusticum-2023.bib` & `vocalpy-0.9.0/docs/fa2023/forum-acusticum-2023.bib`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/fa2023/header.png` & `vocalpy-0.9.0/docs/fa2023/header.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/fa2023/header_onda.png` & `vocalpy-0.9.0/docs/fa2023/header_onda.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/fa2023/main.tex` & `vocalpy-0.9.0/docs/fa2023/main.tex`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/fa2023/voc-fig1-model.png` & `vocalpy-0.9.0/docs/fa2023/voc-fig1-model.png`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/getting_started/installation.md` & `vocalpy-0.9.0/docs/getting_started/installation.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/getting_started/quickstart.md` & `vocalpy-0.9.0/docs/getting_started/quickstart.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 jupytext:
   text_representation:
     extension: .md
     format_name: myst
     format_version: 0.13
-    jupytext_version: 1.15.2
+    jupytext_version: 1.16.1
 kernelspec:
   display_name: Python 3 (ipykernel)
   language: python
   name: python3
 ---
 
 (quickstart)=
@@ -21,106 +21,100 @@
 
 +++
 
 ## Set up
 
 +++
 
-First we download some example data, from the [Bengalese Finch song repository](https://nickledave.github.io/bfsongrepo/).
+First we import `vocalpy`.
 
 ```{code-cell} ipython3
-:tags: [hide-output]
-!curl -sSL https://raw.githubusercontent.com/vocalpy/vak/main/src/scripts/download_autoannotate_data.py | python3 -
+import vocalpy as voc
 ```
 
-And then we'll move that data into a `./data` directory.
+Then we get some example data, from the [Bengalese Finch song repository](https://nickledave.github.io/bfsongrepo/).
 
 ```{code-cell} ipython3
-import pathlib
-```
-
-```{code-cell} ipython3
-pathlib.Path('./data').mkdir(exist_ok=True,parents=True)
-```
+:tags: [hide-output]
 
-```{code-cell} ipython3
-pathlib.Path('./bfsongrepo').rename('./data/bfsongrepo')
-```
-
-Now that we've got some data to work with, we can import `vocalpy`
-
-```{code-cell} ipython3
-import vocalpy as voc
+sounds = voc.example('bfsongrepo', return_type='sound')
 ```
 
 ## Data types for acoustic communication
 
 +++
 
 Let's look at the data types that VocalPy provides for acoustic comunication.
 
 +++
 
-We load all the wav files from a directory using a convenience function that VocalPy gives us in its `paths`, `vocalpy.paths.from_dir`:
+### Data type for sound: `vocalpy.Sound`
 
-```{code-cell} ipython3
-data_dir = ('data/bfsongrepo/gy6or6/032312/')
++++
 
-wav_paths = voc.paths.from_dir(data_dir, 'wav')
-```
+Calling `vocalpy.example('bfsongrepo')` gave us back a list of of `vocalpy.Sound` instances.
+Let's inspect one of them.
 
-### Data type for audio: `vocalpy.Audio`
+```{code-cell} ipython3
+a_sound = sounds[0]
+print(a_sound)
+```
 
-+++
+We can see that it has three attributes:
 
-Next we load all the wav files into the data type that VocalPy provides for audio, `vocalpy.Audio`, using the method `vocalpy.Audio.read`:
+1. `data`, the audio signal itself, with two dimensions: (channels, samples)
 
 ```{code-cell} ipython3
-audios = [
-    voc.Audio.read(wav_path) for wav_path in wav_paths
-]
+print(a_sound.data)
 ```
 
-Let's inspect one of the `vocalpy.Audio` instances
+2. `samplerate`, the sampling rate for the audio
 
 ```{code-cell} ipython3
-an_audio = audios[0]
-print(an_audio)
+print(a_sound.samplerate)
 ```
 
-We can see that it has four attributes:
+and finally,  
 
-1. `data`, the audio signal itself
+3. `path`, the path to the file that the sound was read from
 
 ```{code-cell} ipython3
-print(an_audio.data)
+print(a_sound.path)
 ```
 
-2. `samplerate`, the sampling rate for the audio
+A `Sound` also has three properties, derived from its data:
+1. `channels`, the number of channels
+2. `samples`, the number of samples, and
+3. `duration`, the number of samples divided by the sampling rate.
 
 ```{code-cell} ipython3
-print(an_audio.samplerate)
+print(
+    f"This sound comes from an audio file with {a_sound.channels} channel, "
+    f"{a_sound.samples} samples, and a duration of {a_sound.duration:.3f} seconds"
+)
 ```
 
-3. `channels`, the number of channels
+One of the reasons VocalPy provides this data type, and the others we're about to show you here, is that it helps you write more succinct code that's easier to read: for you, when you come back to your code months from now, and for others that want to read the code you share.
 
-```{code-cell} ipython3
-print(an_audio.channels)
-```
++++
 
-and finally,  
+When you are working with your own data, instead of example data built into VocalPy, you will do something like:  
 
-4. `path`, the path to the file that the audio was read from
+1. Load all the sound files from a directory using a convenience function that VocalPy gives us in its `paths` module, `vocalpy.paths.from_dir`
+2. Load all the wav files into the data type that VocalPy provides for sound, `vocalpy.Sound`, using the method `vocalpy.Sound.read`:
 
-```{code-cell} ipython3
-print(an_audio.path)
+This is shown in the snippet below.
+```python
+data_dir = ('data/bfsongrepo/gy6or6/032312/')
+wav_paths = voc.paths.from_dir(data_dir, 'wav')
+sounds = [
+    voc.Sound.read(wav_path) for wav_path in wav_paths
+]
 ```
 
-One of the reasons VocalPy provides this data type, and the others we're about to show you here, is that it helps you write more succinct code that's easier to read: for you, when you come back to your code months from now, and for others that want to read the code you share.
-
 +++
 
 ## Classes for steps in pipelines for processing data in acoustic communication
 
 +++
 
 In addition to data types for acoustic communication, VocalPy provides you with classes that represent steps in pipelines for processing that data. These classes are also written with readability and reproducibility in mind.
@@ -128,174 +122,163 @@
 +++
 
 Let's use one of those classes, `SpectrogramMaker`, to make a spectrogram from each one of the wav files that we loaded above.
 
 We'll write a brief snippet to do so, and then we'll explain what we did.
 
 ```{code-cell} ipython3
-spect_params = {'fft_size': 512, 'step_size': 64}
-callback = voc.signal.spectrogram.spectrogram
-spect_maker = voc.SpectrogramMaker(callback=callback, spect_params=spect_params)
-spects = spect_maker.make(audios, parallelize=True)
+params = {'n_fft': 512, 'hop_length': 64}
+callback = voc.spectrogram
+spect_maker = voc.SpectrogramMaker(callback=callback, params=params)
+spects = spect_maker.make(sounds, parallelize=True)
 ```
 
 Notice a couple of things about this snippet:
 - In line 1, you declare the parameters that you use to generate spectrograms explicitly, as a dictionary. This helps with reproducibility by encouraging you to document those parameters
-- In line 2, you also decide what code you will use to generate the spectrograms, by using what's called a "callback", because the `SpectrogramMaker` will call this function for you.
-- In line 3, you create an instance of the `SpectrogramMaker` class with the function you want to use to generate spectrograms, and the parameters to use with that function.
+- In line 2, you also decide what function you will use to generate the spectrograms. Here we use the helper function `vocalpy.spectrogram`.
+- In line 3, you create an instance of the `SpectrogramMaker` class with the function you want to use to generate spectrograms, and the parameters to use with that function. We refer to the function we pass in as a `callback`, because the `SpectrogramMaker` will "call back" to this function when it makes a spectrogram.
 - In line 4, you make the spectrograms, with a single call to the method `vocalpy.SpectrogramMaker.make`. You pass in the audio we loaded earlier, and you tell VocalPy that you want to parallelize the generation of the spectrograms. This is done for you, using the library `dask`.
 
 +++
 
 ### Data type: `vocalpy.Spectrogram`
 
 +++
 
 As you might have guessed, when we call `SpectrogramMaker.make`, we get back a list of spectrograms.
 
-This is the next data type we'll look at. 
+This is the next data type we'll look at.
 
 +++
 
 We inspect the first spectrogram we loaded.
 
 ```{code-cell} ipython3
 a_spect = spects[0]
 print(a_spect)
 ```
 
 As before, we'll walk through the attributes of this class.
 But since the whole point of a spectrogram is to let us see sound, let's actually look at the spectrogram, instead of staring at arrays of numbers.
 
-We'll make a new spectrogram where we log transform the data so it's easier to visualize.
-
-+++
-
-We import NumPy so we can do a quick-and-dirty transform.
-
-```{code-cell} ipython3
-import numpy as np
-```
-
-```{code-cell} ipython3
-a_spect_log = voc.Spectrogram(data=np.log(a_spect.data),
-                              frequencies=a_spect.frequencies,
-                              times=a_spect.times)
-```
-
-Then we'll plot the log-transformed spectrogram using a function built into the `vocalpy.plot` module.
+We do so by calling `vocalpy.plot.spectrogram`.
 
 ```{code-cell} ipython3
 voc.plot.spectrogram(
-    a_spect_log,
+    a_spect,
     tlim = [2.6, 4],
     flim=[500,12500],
-    pcolormesh_kwargs={'vmin':-25, 'vmax': -10}
 )
 ```
 
 We see that we have a spectrogram of Bengalese finch song.
 
 Now that we know what we're working with, let's actually inspect the attributes of the `vocalpy.Spectrogram` instance.
 
 +++
 
 There are five attributes we care about here.
 
-1. `data`: this is the spectrogram itself -- as with the other data types,like `vocalpy.Audio`, the attribute name `data` indiciates this main data we care about
+1. `data`: this is the spectrogram itself -- as with the other data types,like `vocalpy.Sound`, the attribute name `data` indiciates this main data we care about
 
 ```{code-cell} ipython3
 print(a_spect.data)
 ```
 
 Let's look at the shape of `data`. It's really just a NumPy array, so we inspect the array's `shape` attribute.
 
 ```{code-cell} ipython3
 print(a_spect.data.shape)
 ```
 
-We see that we have a matrix with some number of rows and columns. These correspond to the next two attributes we will look at.
+We see that we have an array with dimensions (channels, frequencies, times). The last two dimensions correspond to the next two attributes we will look at.
 
 +++
 
-2. `frequencies`, a vector of the number of frequency bins
+2. `frequencies`, a vector of the frequency for each row of the spectrogram.
 
 ```{code-cell} ipython3
 print(a_spect.frequencies[:10])
 ```
 
 ```{code-cell} ipython3
 print(a_spect.frequencies.shape)
 ```
 
 (We see it is equal to the number of rows.)
 
-3. `times`, a vector of time bin centers
+3. `times`, a vector of the time for each column in the spectrogram.
 
 ```{code-cell} ipython3
 print(a_spect.times[:10])
 ```
 
 ```{code-cell} ipython3
 print(a_spect.times.shape)
 ```
 
-Just like with the `Audio` class, VocalPy gives us the ability to conveniently read and write spectrograms from files. This saves us from generating spectrograms over and over. Computing spectrograms can be computionally expensive, if your audio has a high sampling rate or you are using methods like multi-taper spectrograms. Saving spectrograms from files also makes it easier for you to share your data in the exact form you used it, so that it's easier to replicate your analyses.
+Just like with the `Sound` class, VocalPy gives us the ability to conveniently read and write spectrograms from files. This saves us from generating spectrograms over and over. Computing spectrograms can be computionally expensive, if your audio has a high sampling rate or you are using methods like multi-taper spectrograms. Saving spectrograms from files also makes it easier for you to share your data in the exact form you used it, so that it's easier to replicate your analyses.
 
 +++
 
 To see this in action, let's write our spectrograms to files.
 
 ```{code-cell} ipython3
 import pathlib
 
+DATA_DIR = pathlib.Path('./data')
+DATA_DIR.mkdir(exist_ok=True)
+
 for spect in spects:
     spect.write(
-        spect.audio_path.parent / (spect.audio_path.name + '.spect.npz')
+        DATA_DIR / (spect.audio_path.name + '.spect.npz')
     )
 ```
 
 Notice that the extension is `'npz'`; this is a file format that NumPy uses to save mulitple arrays in a single file. By convention we include the file extension of the source audio, and another "extension" that incidicates this is a spectrogram, so that the file name ends with `'.wav.spect.npz'`.
 
 +++
 
 We can confirm that reading and writing spectrograms to disk works as we expect using the method `vocalpy.Spectrogram.read`
 
 ```{code-cell} ipython3
-spect_paths = voc.paths.from_dir(data_dir, '.wav.spect.npz')
+spect_paths = voc.paths.from_dir(DATA_DIR, '.spect.npz')
 ```
 
 ```{code-cell} ipython3
 spects_loaded = [
     voc.Spectrogram.read(spect_path)
     for spect_path in spect_paths
 ]
 ```
 
 We compare with the equality operator to confirm we loaded what we saved.
 
+Before doing so, we sort the original ``spects`` by the ``audio_path`` of the sound they were generated from, and the ``spects_loaded`` by the path they were loaded from. In this case, doing so puts both lists in the same order, because we used the audio file's filename as part of the spectrogram file's filename. (It might not work more generally, if you name your files differently.)
+
 ```{code-cell} ipython3
-# this happens to work 
-# because VocalPy always gives us back `sorted` lists,
-# but it wouldn't work in the more general case--
-# we'd need to pair by filename first or something
+spects = sorted(spects, key=lambda spect: spect.audio_path)
+spects_loaded = sorted(spects_loaded, key=lambda spect: spect.path)
 for spect, spect_loaded in zip(spects, spects_loaded):
     assert spect == spect_loaded
 ```
 
 ### Data type: `vocalpy.Annotation`
 
 +++
 
 The last data type we'll look at is for annotations. Such annotations are important for analysis of aocustic communication and behavior. Under the hood, VocalPy uses the pyOpenSci package [crowsetta](https://github.com/vocalpy/crowsetta).
 
 ```{code-cell} ipython3
 import vocalpy as voc
 
-csv_paths = voc.paths.from_dir(data_dir, '.wav.csv')
+# We get back the paths to all the files in this example dataset, 
+# but only keep the ones that are csv files, because those are the annotations.
+# This filters out the wav files.
+csv_paths = [path for path in voc.example('bfsongrepo') if path.name.endswith('csv')]
 ```
 
 ```{code-cell} ipython3
 annots = [voc.Annotation.read(notmat_path, format='simple-seq') 
           for notmat_path in csv_paths]
 ```
 
@@ -305,18 +288,15 @@
 print(annots[1])
 ```
 
 We plot the spectrogram along with the annotations.
 
 ```{code-cell} ipython3
 voc.plot.annotated_spectrogram(
-    spect=voc.Spectrogram(data=np.log(spects[1].data),
-                    frequencies=spects[1].frequencies,
-                    times=spects[1].times),
+    spect=spects[1],
     annot=annots[1],
     tlim = [3.2, 3.9],
     flim=[500,12500],
-    pcolormesh_kwargs={'vmin':-25, 'vmax': -10}
 );
 ```
 
-This crash course in VocalPy has introduced you to the key features and goals of the library. To learn more, please check out [the documentation](https://vocalpy.readthedocs.io/en/latest/) and read our Forum Acusticum 2023 Proceedings Paper, ["Introducing VocalPy"](https://github.com/vocalpy/vocalpy/blob/main/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf). We are actively developing the library to meet your needs and would love to hear your feedback in [our forum](https://forum.vocalpy.org/)
+This crash course in VocalPy has introduced you to the key features and goals of the library. To learn more, please check out [the documentation](https://vocalpy.readthedocs.io/en/latest/) and read our Forum Acusticum 2023 Proceedings Paper, ["Introducing VocalPy"](https://github.com/vocalpy/vocalpy/blob/main/docs/fa2023/Introducing_VocalPy__a_core_Python_package_for_researchers_studying_animal_acoustic_communication.pdf). We are actively developing the library to meet your needs and would love to hear your feedback in [our forum](https://forum.vocalpy.org/).
```

### Comparing `vocalpy-0.8.2/docs/index.md` & `vocalpy-0.9.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/make.bat` & `vocalpy-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/nitpick-ignore.txt` & `vocalpy-0.9.0/docs/nitpick-ignore.txt`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/user/background.md` & `vocalpy-0.9.0/docs/user/background.md`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/docs/user/whatisvocalpy.md` & `vocalpy-0.9.0/docs/user/whatisvocalpy.md`

 * *Files 10% similar despite different names*

```diff
@@ -26,41 +26,40 @@
 
 For more on acoustic communication research in general, please see the {ref}`background` page.
 
 ## Features
 
 ###  Data types for acoustic communication data: audio, spectrograms, annotations
 
-#### The `vocalpy.Audio` data type
+#### The `vocalpy.Sound` data type
 
 - Works with a wide array of audio formats, thanks to [soundfile](https://github.com/bastibe/python-soundfile).
 - Also works with the cbin audio format saved by the LabView app EvTAF used by many neuroscience labs studying birdsong,
   thanks to [evfuncs](https://github.com/NickleDave/evfuncs).
 
 ```python
 >>> import vocalpy as voc
 >>> data_dir = ('tests/data-for-tests/source/audio_wav_annot_birdsongrec/Bird0/Wave/')
 >>> wav_paths = voc.paths.from_dir(data_dir, 'wav')
->>> audios = [voc.Audio.read(wav_path) for wav_path in wav_paths]
->>> print(audios[0])
-vocalpy.Audio(data=array([3.0517...66210938e-04]), samplerate=32000, channels=1), 
-path=tests/data-for-tests/source/audio_wav_annot_birdsongrec/Bird0/Wave/0.wav)
+>>> sounds = [voc.Sound.read(wav_path) for wav_path in wav_paths]
+>>> print(sounds[0])
+vocalpy.Sound(data=array([3.0517...66210938e-04]), samplerate=32000, path ="tests/data-for-tests/source/audio_wav_annot_birdsongrec/Bird0/Wave/0.wav")
 ```
 
 #### The `vocalpy.Spectrogram` data type
 
 - Save expensive-to-compute spectrograms to array files, so you don't regenerate them over and over again
 
 ```python
 >>> import vocalpy as voc
 >>> data_dir = ('tests/data-for-tests/generated/spect_npz/')
 >>> spect_paths = voc.paths.from_dir(data_dir, 'wav.npz')
 >>> spects = [voc.Spectrogram.read(spect_path) for spect_path in spect_paths]
 >>> print(spects[0])
-vocalpy.Spectrogram(data=array([[3.463...7970774e-14]]), frequencies=array([    0....7.5, 16000. ]), times=array([0.008,...7.648, 7.65 ]), 
+vocalpy.Spectrogram(data=array([[3.463...7970774e-14]]), frequencies=array([0....7.5, 16000. ]), times=array([0.008,...7.648, 7.65 ]), 
 path=PosixPath('tests/data-for-tests/generated/spect_npz/0.wav.npz'), audio_path=None)
 ```
 
 #### The `vocalpy.Annotation` data type
 
 - Load many different annotation formats using the pyOpenSci package [crowsetta](https://crowsetta.readthedocs.io/en/latest/)
 
@@ -80,45 +79,55 @@
 #### A `Segmenter` for segmentation into sequences of units
 
 ```python
 >>> import evfuncs
 >>> import vocalpy as voc
 >>> data_dir = ('tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/')
 >>> cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
->>> audios = [voc.Audio.read(cbin_path) for cbin_path in cbin_paths]
+>>> sounds = [voc.Sound.read(cbin_path) for cbin_path in cbin_paths]
 >>> segment_params = {'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006}
 >>> segmenter = voc.Segmenter(callback=evfuncs.segment_song, segment_params=segment_params)
->>> seqs = segmenter.segment(audios, parallelize=True)
-[########################################] | 100% Completed | 122.91 ms
+>>> seqs = segmenter.segment(sounds, parallelize=True)
+[  ########################################] | 100% Completed | 122.91 ms
 >>> print(seqs[1])
-Sequence(units=[Unit(onset=2.19075, offset=2.20428125, label='-', audio=None, spectrogram=None), 
-Unit(onset=2.35478125, offset=2.38815625, label='-', audio=None, spectrogram=None), Unit(onset=2.8410625, offset=2.86715625, label='-', audio=None, spectrogram=None), 
-Unit(onset=3.48234375, offset=3.49371875, label='-', audio=None, spectrogram=None), Unit(onset=3.57021875, offset=3.60296875, label='-', audio=None, spectrogram=None), 
-Unit(onset=3.64403125, offset=3.67721875, label='-', audio=None, spectrogram=None), Unit(onset=3.72228125, offset=3.74478125, label='-', audio=None, spectrogram=None), 
-Unit(onset=3.8036875, offset=3.8158125, label='-', audio=None, spectrogram=None), Unit(onset=3.82328125, offset=3.83646875, label='-', audio=None, spectrogram=None), 
-Unit(onset=4.13759375, offset=4.16346875, label='-', audio=None, spectrogram=None), Unit(onset=4.80278125, offset=4.814, label='-', audio=None, spectrogram=None), 
-Unit(onset=4.908125, offset=4.922875, label='-', audio=None, spectrogram=None), Unit(onset=4.9643125, offset=4.992625, label='-', audio=None, spectrogram=None), 
-Unit(onset=5.039625, offset=5.0506875, label='-', audio=None, spectrogram=None), Unit(onset=5.10165625, offset=5.1385, label='-', audio=None, spectrogram=None), 
-Unit(onset=5.146875, offset=5.16203125, label='-', audio=None, spectrogram=None), Unit(onset=5.46390625, offset=5.49409375, label='-', audio=None, spectrogram=None), 
-Unit(onset=6.14503125, offset=6.1565625, label='-', audio=None, spectrogram=None), Unit(onset=6.31003125, offset=6.346125, label='-', audio=None, spectrogram=None), 
-Unit(onset=6.38996875, offset=6.4018125, label='-', audio=None, spectrogram=None), Unit(onset=6.46053125, offset=6.4796875, label='-', audio=None, spectrogram=None), 
-Unit(onset=6.83525, offset=6.8643125, label='-', audio=None, spectrogram=None)], method='segment_song', 
-segment_params={'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006}, 
-audio=vocalpy.Audio(data=None, samplerate=None, channels=None), path=tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/gy6or6_baseline_230312_0809.141.cbin), spectrogram=None)
+Sequence(units=[Unit(onset=2.19075, offset=2.20428125, label='-', audio=None, spectrogram=None),
+                Unit(onset=2.35478125, offset=2.38815625, label='-', audio=None, spectrogram=None),
+                Unit(onset=2.8410625, offset=2.86715625, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.48234375, offset=3.49371875, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.57021875, offset=3.60296875, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.64403125, offset=3.67721875, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.72228125, offset=3.74478125, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.8036875, offset=3.8158125, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.82328125, offset=3.83646875, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.13759375, offset=4.16346875, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.80278125, offset=4.814, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.908125, offset=4.922875, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.9643125, offset=4.992625, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.039625, offset=5.0506875, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.10165625, offset=5.1385, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.146875, offset=5.16203125, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.46390625, offset=5.49409375, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.14503125, offset=6.1565625, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.31003125, offset=6.346125, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.38996875, offset=6.4018125, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.46053125, offset=6.4796875, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.83525, offset=6.8643125, label='-', audio=None, spectrogram=None)], method='segment_song',
+         segment_params={'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006},
+         audio=vocalpy.Sound(data=None, samplerate=None, path="tests/data-for-tests/source/audio_cbin_annot_notmat / gy6or6 / 032312 / gy6or6_baseline_230312_0809.141.cbin"), spectrogram=None)
 ```
   
 #### A `SpectrogramMaker` for computing spectrograms
 
 ```python
 >>> import vocalpy as voc
 >>> wav_paths = voc.paths.from_dir('wav')
->>> audios = [voc.Audio(wav_path) for wav_path in wav_paths]
+>>> sounds = [voc.Sound(wav_path) for wav_path in wav_paths]
 >>> spect_params = {'fft_size': 512, 'step_size': 64}
 >>> spect_maker = voc.SpectrogramMaker(spect_params=spect_params)
->>> spects = spect_maker.make(audios, parallelize=True)
+>>> spects = spect_maker.make(sounds, parallelize=True)
 ```
 
 ### `Dataset`s you flexibly build from pipelines and convert to databases
 
 - The `vocalpy.dataset` module contains classes that represent common types of datasets 
 - You make these classes with outputs of your pipelines, e.g. a `list` of `vocalpy.Sequence`s 
   or `vocalpy.Spectrogram`s
@@ -136,30 +145,31 @@
 #### A `SequenceDataset` for common analyses of sequences of units
 
 ```python
 >>> import evfuncs
 >>> import vocalpy as voc
 >>> data_dir = 'tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/'
 >>> cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
->>> audios = [voc.Audio.read(cbin_path) for cbin_path in cbin_paths]
+>>> sounds = [voc.Sound.read(cbin_path) for cbin_path in cbin_paths]
 >>> segment_params = {
     'threshold': 1500,
     'min_syl_dur': 0.01,
     'min_silent_dur': 0.006,
 }
 >>> segmenter = voc.Segmenter(
-    callback=evfuncs.segment_song, 
+    callback=evfuncs.segment_song,
     segment_params=segment_params
 )
->>> seqs = segmenter.segment(audios)
+>>> seqs = segmenter.segment(sounds)
 >>> seq_dataset = voc.dataset.SequenceDataset(sequences=seqs)
 >>> seq_dataset.to_sqlite(db_name='gy6or6-032312.db', replace=True)
 >>> print(seq_dataset)
 SequenceDataset(sequences=[Sequence(units=[Unit(onset=2.18934375, offset=2.21, label='-', audio=None, spectrogram=None),
-Unit(onset=2.346125, offset=2.373125, label='-', audio=None, spectrogram=None), Unit(onset=2.50471875, offset=2.51546875,
-label='-', audio=None, spectrogram=None), Unit(onset=2.81909375, offset=2.84740625, label='-', audio=None, spectrogram=None),
-...
+                                           Unit(onset=2.346125, offset=2.373125, label='-', audio=None, spectrogram=None), 
+                                           Unit(onset=2.50471875, offset=2.51546875, label='-', audio=None, spectrogram=None),
+                                           Unit(onset=2.81909375, offset=2.84740625, label='-', audio=None, spectrogram=None),
+                                           ...
 >>> # test that we can load the dataset
 >>> seq_dataset_loaded = voc.dataset.SequenceDataset.from_sqlite(db_name='gy6or6-032312.db')
 >>> seq_dataset_loaded == seq_dataset
 True
 ```
```

### Comparing `vocalpy-0.8.2/noxfile.py` & `vocalpy-0.9.0/noxfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -103,27 +103,15 @@
     if dist_p.exists():
         shutil.rmtree(dist_p)
 
     session.install("flit")
     session.run("flit", "build")
 
 
-# ---- the bottom half of the noxfile, the rest of the sessions have to do with data for tests -------------------------
-# either generating, downloading, or archiving
-
-DATA_FOR_TESTS_DIR = pathlib.Path("./tests/data-for-tests/")
-SOURCE_TEST_DATA_DIR = DATA_FOR_TESTS_DIR / "source"
-SOURCE_TEST_DATA_DIRS = [
-    dir_ for dir_
-    in sorted(pathlib.Path(SOURCE_TEST_DATA_DIR).glob('*/'))
-    if dir_.is_dir()
-]
-
-
-# ---- used by sessions that "clean up" data for tests
+# ---- used by sessions that "clean up" data, for example data and for tests
 def clean_dir(dir_path):
     """
     "clean" a directory by removing all files
     (that are not hidden)
     without removing the directory itself
     """
     dir_path = pathlib.Path(dir_path)
@@ -134,14 +122,38 @@
         else:
             if content.name.startswith('.'):
                 # e.g., .gitkeep file we don't want to delete
                 continue
             content.unlink()
 
 
+@nox.session(name='make-example-data')
+def make_example_data(session: nox.Session) -> None:
+    """
+    Make example data.
+    Runs scripts in
+    """
+    clean_dir("./src/scripts/example_data/")
+    session.run("python", "./src/scripts/make_example_data.py")
+
+# ---- sessions that have to do with data for tests --------------------------------------------------------------------
+# either generating, downloading, or archiving
+
+DATA_FOR_TESTS_DIR = pathlib.Path("./tests/data-for-tests/")
+# THIS PATH NEEDS TO BE RELATIVE TO PROJECT ROOT OR WE BREAK TESTS ON CI THAT USE TAR'ED TEST DATA
+# i.e., keep as is, don't use the constant in tests.fixtures that involve paths relative to fixtures dir
+SOURCE_TEST_DATA_DIR = DATA_FOR_TESTS_DIR / "source"
+SOURCE_TEST_DATA_DIRS = [
+    dir_ for dir_
+    in sorted(pathlib.Path(SOURCE_TEST_DATA_DIR).glob('*/'))
+    if dir_.is_dir()
+]
+
+
+
 @nox.session(name='test-data-clean-source')
 def test_data_clean_source(session) -> None:
     """
     Clean (remove) 'source' test data, used by TEST_DATA_GENERATE_SCRIPT.
     """
     clean_dir(SOURCE_TEST_DATA_DIR)
 
@@ -183,43 +195,56 @@
     session.log(f'Downloading: {SOURCE_TEST_DATA_URL}')
     copy_url(url=SOURCE_TEST_DATA_URL, path=SOURCE_TEST_DATA_TAR)
     session.log(f'Extracting downloaded tar: {SOURCE_TEST_DATA_TAR}')
     with tarfile.open(SOURCE_TEST_DATA_TAR, "r:gz") as tf:
         tf.extractall(path='.')
 
 
+TEST_DATA_GENERATE_AVA_SEGMENTS_SCRIPT = './tests/scripts/generate_ava_segment_test_data/generate_ava_segment_text_files_from_jourjine_et_al_2023.py'
+
+
+@nox.session(name='test-data-generate-ava-segments', python="3.10")
+def test_data_generate_ava_segments(session) -> None:
+    """Produce generated test data for ava segments"""
+    session.install("joblib==1.3.2")
+    session.install("numpy==1.26.3")
+    session.install("scipy==1.12.0")
+    session.run("python", TEST_DATA_GENERATE_AVA_SEGMENTS_SCRIPT)
+
 
 TEST_DATA_GENERATE_SCRIPT = './tests/scripts/generate_data_for_tests.py'
 
 
 @nox.session(name='test-data-generate', python="3.10")
 def test_data_generate(session) -> None:
     """
     Produce 'generated' test data, by running TEST_DATA_GENERATE_SCRIPT on 'source' test data.
     """
     session.install(".[test]")
     session.run("python", TEST_DATA_GENERATE_SCRIPT)
 
 
-# TODO: fix this url!
+# THIS PATH NEEDS TO BE RELATIVE TO PROJECT ROOT OR WE BREAK TESTS ON CI THAT USE TAR'ED TEST DATA
+# i.e., keep as is, don't use the constant in tests.fixtures that involve paths relative to fixtures dir
 GENERATED_TEST_DATA_DIR = DATA_FOR_TESTS_DIR / "generated"
 GENERATED_TEST_DATA_SUBDIRS = [
     dir_ for dir_
-    in sorted(pathlib.Path(GENERATED_TEST_DATA_DIR).glob('*/'))
+    in GENERATED_TEST_DATA_DIR.iterdir()
     if dir_.is_dir()
 ]
 GENERATED_TEST_DATA_TAR = GENERATED_TEST_DATA_DIR / 'generated_test_data.tar.gz'
 
 
 @nox.session(name='test-data-clean-generated')
 def test_data_clean_generated(session) -> None:
     """
     Clean (remove) 'generated' test data.
     """
-    clean_dir(GENERATED_TEST_DATA_DIR)
+    for dir_ in GENERATED_TEST_DATA_SUBDIRS:
+        clean_dir(dir_)
 
 
 @nox.session(name='test-data-tar-generated')
 def test_data_tar_generated(session) -> None:
     """
     Make a .tar.gz file of all 'generated' test data.
     """
```

### Comparing `vocalpy-0.8.2/pyproject.toml` & `vocalpy-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "vocalpy"
 authors = [
     {name = "David Nicholson", email = "nickledave@users.noreply.github.com"}
 ]
 description = "A core package for acoustic communication research in Python"
-version = "0.8.2"
+version = "0.9.0"
 classifiers = [
         'License :: OSI Approved :: BSD License',
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
@@ -21,22 +21,23 @@
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "attrs >=23.1.0",
     "crowsetta >=5.0.2",
-    "dask >=2.10.1",
+    "dask[dataframe] >=2.10.1",
+    "h5netcdf >= 1.3.0",
     "librosa >= 0.10.0.post2",
     "matplotlib >=3.7.1",
     "numpy >=1.22.0",
     "pandas >= 1.4.0",
+    "pooch >= 1.8.1",
     "scipy >=1.8.0",
     "SoundFile >=0.12.1",
-    "SQLAlchemy >=2.0.12",
     "xarray >= 2023.11.0",
 ]
 
 [project.urls]
 Home = "https://github.com/vocalpy/vocalpy"
 Docs = "https://vocalpy.readthedocs.io"
 
@@ -47,14 +48,16 @@
     "pytest-xdist >=3.2.0",
 ]
 doc = [
     "ipython != 8.7.0",
     "jupyterlab >=3.0.3",
     "jupytext >=1.13.8",
     "myst-nb >=0.15.0",
+    "numpydoc >=1.6.0",
+    "seaborn >=0.13.2",
     "Sphinx >=3.4.3",
     "sphinx-autobuild >= 2021.3.14",
     "sphinx-book-theme >=0.3.2",
     "sphinx-copybutton >=0.4.0",
     "sphinx-design >=0.2.0",
     "sphinxext-opengraph  >=0.5.1",
     "sphinx-tabs >= 3.3.1",
@@ -65,15 +68,26 @@
     "ipython >=8.0.0",
     "nox >= 2022.1.7",
     "vocalpy[doc, test]"
 ]
 
 [tool.pytest.ini_options]
 filterwarnings = [
-    'ignore:Deprecated call to `pkg_resources.declare_namespace',
-    'ignore:pkg_resources is deprecated as an API',
+    'ignore:Deprecated call to `pkg_resources.declare_namespace:DeprecationWarning:pkg_resources',
+    'ignore:pkg_resources is deprecated as an API:DeprecationWarning:',
+    'ignore:\nPyarrow will become a required dependency::',
+    'ignore:use `parametric:DeprecationWarning:multimethod',
+    'ignore:base implementation will eventually ignore',
+    'ignore:The current Dask DataFrame'
 ]
 
 [tool.flit.sdist]
 exclude = [
     "tests/data-for-tests"
 ]
+
+[tool.coverage.run]
+omit = [
+    "src/scripts/",
+    "tests/scripts/",
+    "noxfile.py",
+]
```

### Comparing `vocalpy-0.8.2/src/vocalpy/__about__.py` & `vocalpy-0.9.0/src/vocalpy/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     base_dir = None
 
 
 __title__ = "vocalpy"
 __summary__ = "A core package for acoustic communication research in Python"
 __uri__ = "https://github.com/vocalpy/vocalpy"
 
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 if base_dir is not None and os.path.exists(os.path.join(base_dir, ".commit")):
     with open(os.path.join(base_dir, ".commit")) as fp:
         __commit__ = fp.read().strip()
 else:
     __commit__ = None
```

### Comparing `vocalpy-0.8.2/src/vocalpy/__init__.py` & `vocalpy-0.9.0/src/vocalpy/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,34 @@
 """A core package for acoustic communication research in Python."""
-from . import (
-    _vendor,
-    constants,
-    dataset,
-    examples,
-    feature,
-    metrics,
-    paths,
-    plot,
-    segment,
-    signal,
-    spectral,
-    validators,
-)
+from . import _vendor, constants, examples, feature, metrics, paths, plot, segment, signal, spectral, validators
 from .__about__ import (
     __author__,
     __commit__,
     __copyright__,
     __email__,
     __license__,
     __summary__,
     __title__,
     __uri__,
     __version__,
 )
 from ._spectrogram.data_type import Spectrogram
 from .annotation import Annotation
 from .annotation_file import AnnotationFile
-from .audio import Audio
 from .audio_file import AudioFile
 from .dataset_file import DatasetFile, DatasetFileType, DatasetFileTypeEnum
 from .examples import example
+from .feature_extractor import FeatureExtractor
 from .feature_file import FeatureFile
+from .features import Features
+from .params import Params
 from .segmenter import Segmenter
+from .segments import Segment, Segments
 from .sequence import Sequence
+from .sound import Sound
 from .spectrogram import spectrogram
 from .spectrogram_file import SpectrogramFile
 from .spectrogram_maker import SpectrogramMaker
 from .spectrogram_parameters import SpectrogramParameters
 from .unit import Unit
 
 __all__ = [
@@ -48,28 +39,32 @@
     "__license__",
     "__summary__",
     "__title__",
     "__uri__",
     "__version__",
     "Annotation",
     "AnnotationFile",
-    "Audio",
+    "Sound",
     "AudioFile",
     "constants",
-    "dataset",
     "DatasetFile",
     "DatasetFileType",
     "DatasetFileTypeEnum",
+    "FeatureExtractor",
     "FeatureFile",
+    "Features",
     "example",
     "examples",
     "feature",
     "paths",
     "plot",
+    "Params",
+    "Segment",
     "Segmenter",
+    "Segments",
     "Sequence",
     "metrics",
     "segment",
     "signal",
     "spectral",
     "spectrogram",
     "Spectrogram",
```

### Comparing `vocalpy-0.8.2/src/vocalpy/_spectrogram/data_type.py` & `vocalpy-0.9.0/src/vocalpy/_spectrogram/data_type.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,27 +21,28 @@
 
     Attributes
     ----------
     data : numpy.ndarray
         The spectrogram itself, typically a matrix
         :math:`f \times t` where there are :math:`f`
         frequency bins and :math:`t` time bins.
-        Must have at least 2 dimensions.
+        Must have either 2 dimensions (frequencies, times)
+        or 3 dimensions (channels, frequencies, times).
     frequencies : numpy.ndarray
         A vector of size :math:`f` where values are frequencies
         at center of frequency bins in spectrogram.
     times : numpy.ndarray
         Vector of size :math:`t` where values are times
         at center of time bins in spectrogram.
     path : pathlib.Path, optional
         Path to .npz file that spectrogram was loaded from.
         Optional, added automatically by the :meth:`~vocalpy.Spectrogram.read` method.
     audio_path : pathlib.Path, optional
         Path to audio file from which spectrogram was generated.
-        Optional, default None. Can be specified as argument
+        Optional, default is None. Can be specified as argument
         to :meth:`~vocalpy.Spectrogram.read` method.
 
     Examples
     --------
     An example of creating a spectrogram with toy data,
     to demonstrate the expected dimensions of the arrays.
 
@@ -53,27 +54,28 @@
     >>> print(spect)
     Spectrogram(data=array([[0.354... 0.81988536]]), frequencies=array([    0....000.        ]), times=array([0.0000...3.121875e-02]))  # noqa: E501
 
     An example of reading a spectrogram from an npz file.
 
     >>> spect = voc.Spectrogram.read("llb3_0066_2018_04_23_17_31_55.wav.npz")
     >>> spect
-    Spectrogram(s=array([[0.561... 0.        ]]), f=array([[    0...50.        ]]), t=array([[0.000...6053968e+01]]),
+    Spectrogram(data=array([[0.561... 0.        ]]), fequencies=array([[    0...50.        ]]), times=array([[0.000...6053968e+01]]),
     spect_path=PosixPath('llb3_0066_2018_04_23_17_31_55.wav.mat'), audio_path=None)
     """
     data: npt.NDArray = attrs.field()
 
     @data.validator
     def validate_data(self, attribute, value):
         if not isinstance(value, np.ndarray):
             raise TypeError(f"Spectrogram array `data` should be a numpy array, " f"but type was {type(value)}.")
 
-        if value.ndim < 2:
+        if value.ndim not in (2, 3):
             raise ValueError(
-                f"Spectrogram array `data` should have at least 2 dimensions, "
+                "Spectrogram array `data` must have either 2 dimensions (frequencies, times) "
+                "or 3 dimensions (channels, frequencies, times), "
                 f"but number of dimensions was {value.ndim}."
             )
 
     frequencies: npt.NDArray = attrs.field(validator=validators.attrs.is_1d_ndarray)
     times: npt.NDArray = attrs.field(validator=validators.attrs.is_1d_ndarray)
 
     path: pathlib.Path = attrs.field(
@@ -84,22 +86,25 @@
     audio_path: pathlib.Path = attrs.field(
         converter=attrs.converters.optional(pathlib.Path),
         validator=attrs.validators.optional(attrs.validators.instance_of(pathlib.Path)),
         default=None,
     )
 
     def __attrs_post_init__(self):
-        if not self.data.shape[0] == self.frequencies.shape[0]:
+        if self.data.ndim == 2:
+            # "canonicalize" to always have 3 dimensions, (channels, frequencies, times)
+            self.data = self.data[np.newaxis, ...]
+
+        if not self.data.shape[1] == self.frequencies.shape[0]:
             raise ValueError(
                 "Number of rows in spectrogram `data` should match number of elements in "
                 f"`frequencies vector, but `data` has {self.data.shape[0]} rows and there are "
                 f"{self.frequencies.shape[0]} elements in `frequencies`."
             )
-
-        if not self.data.shape[1] == self.times.shape[0]:
+        if not self.data.shape[2] == self.times.shape[0]:
             raise ValueError(
                 "Number of columns in spectrogram `data` should match number of elements in "
                 f"`times` vector, but `data` has {self.data.shape[1]} columns and there are "
                 f"{self.times.shape[0]} elements in `times`."
             )
 
     def __repr__(self):
@@ -139,32 +144,32 @@
         if other.__class__ is not self.__class__:
             return NotImplemented
         return not self.__eq__(other)
 
     @classmethod
     def read(cls, path: str | pathlib.Path, audio_path: str | pathlib.Path | None = None):
         """Read spectrogram and associated arrays from a Numpy npz file
-            at the given ``path``.
+        at the given ``path``.
 
-            Parameters
-            ----------
-            path : str, pathlib.Path
-                The path to the file containing the spectrogram ``s``
-                and associated arrays ``f`` and ``t``.
+        Parameters
+        ----------
+        path : str, pathlib.Path
+            The path to the file containing the spectrogram ``s``
+            and associated arrays ``f`` and ``t``.
         audio_path : str or pathlib.Path, optional
             Path to audio file from which spectrogram was generated.
             Optional, default None. Note this argument is not validated
             (to guarantee that the spectrogram was actually generated
             from the specified audio path.)
 
-            Returns
-            -------
-            spect : vocalpy.Spectrogram
-                An instance of :class:`vocalpy.Spectrogram`
-                containing the arrays loaded from ``path``.
+        Returns
+        -------
+        spect : vocalpy.Spectrogram
+            An instance of :class:`vocalpy.Spectrogram`
+            containing the arrays loaded from ``path``.
         """
         path = pathlib.Path(path)
         if not path.exists():
             raise FileNotFoundError(f"File with spectrogram not found at path specified:\n{path}")
 
         if not path.suffix == VALID_SPECT_FILE_EXTENSION:
             raise ValueError(
@@ -179,26 +184,59 @@
             try:
                 kwargs[key] = np.array(spect_file_dict[key])
             except KeyError as e:
                 raise KeyError(f"Did not find key '{key}' in path: {path}") from e
 
         return cls(path=path, audio_path=audio_path, **kwargs)
 
-    def write(self, path: [str, pathlib.Path]):
+    def write(self, path: [str, pathlib.Path]) -> SpectrogramFile:
         """Write this :class:`vocalpy.Spectrogram`
-        to a Numpy .npz file at the given ``path``.
+        to a Numpy npz file at the given ``path``.
 
         Parameters
         ----------
         path : str, pathlib.Path
             The path to where the path should be saved
             containing the spectrogram ``data``
             and associated arrays ``frequencies`` and ``times``.
+            If this path does not already end with the extension
+            ".npz", that extension will be added
+            (by :func:`numpy.savez`).
+
+        Returns
+        -------
+        spectrogram_file : SpectrogramFile
+            An instance of :class:`SpectrogramFile`
+            representing the saved spectrogram.
         """
-        # TODO: deal with extension here
         path = pathlib.Path(path)
         np.savez(path, data=self.data, frequencies=self.frequencies, times=self.times)
         if self.audio_path:
             source_audio_file = AudioFile(path=self.audio_path)
         else:
             source_audio_file = None
         return SpectrogramFile(path=path, source_audio_file=source_audio_file)
+
+    def __iter__(self):
+        for channel in self.data:
+            yield Spectrogram(
+                data=channel[np.newaxis, ...],
+                frequencies=self.frequencies,
+                times=self.times,
+                path=self.path,
+            )
+
+    def __getitem__(self, key):
+        if isinstance(key, (int, slice)):
+            try:
+                return Spectrogram(
+                    data=self.data[key],
+                    frequencies=self.frequencies,
+                    times=self.times,
+                    path=self.path,
+                )
+            except IndexError as e:
+                raise IndexError(
+                    f"Invalid integer or slice for Spectrogram with {self.data.shape[0]} channels: {key}"
+                ) from e
+        else:
+            raise TypeError(f"Spectrogram can be indexed with integer or slice, but type was: {type(key)}")
```

### Comparing `vocalpy-0.8.2/src/vocalpy/_vendor/evfuncs.py` & `vocalpy-0.9.0/src/vocalpy/_vendor/evfuncs.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/annotation.py` & `vocalpy-0.9.0/src/vocalpy/annotation.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/annotation_file.py` & `vocalpy-0.9.0/src/vocalpy/annotation_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,19 @@
 
 @attrs.define
 class AnnotationFile:
     """Class that represents an annotation file,
     as part of a dataset used to study
     animal acoustic communication.
 
-    Used by the :class:`vocalpy.Dataset` class.
-
     Attributes
     ----------
     path : pathlib.Path
         The path to the annotation file.
-    annotates : vocalpy.dataset.AudioFile or vocalpy.dataset.SpectrogramFile
+    annotates : vocalpy.AudioFile or vocalpy.SpectrogramFile
         The file that this annotation file annotates.
     """
 
     path: pathlib.Path = attrs.field()
     annotates: AudioFile | SpectrogramFile | list[AudioFile] | list[SpectrogramFile] | None = attrs.field()
 
     @annotates.validator
```

### Comparing `vocalpy-0.8.2/src/vocalpy/audio_file.py` & `vocalpy-0.9.0/src/vocalpy/audio_file.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 """Class that represents an audio file,
 as part of a dataset used to study
 animal acoustic communication.
-
-Used by the :class:`vocalpy.Dataset` class.
 """
 from __future__ import annotations
 
 import pathlib
 
 import attrs
 
 
 @attrs.define
 class AudioFile:
     """Class that represents an audio file,
     as part of a dataset used to study
     animal acoustic communication.
 
-    Used by the :class:`vocalpy.Dataset` class.
-
     Attributes
     ----------
     path : pathlib.Path
         The path to the audio file.
     """
 
     path: pathlib.Path = attrs.field(converter=pathlib.Path, validator=attrs.validators.instance_of(pathlib.Path))
```

### Comparing `vocalpy-0.8.2/src/vocalpy/dataset_file.py` & `vocalpy-0.9.0/src/vocalpy/dataset_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 DatasetFileType = Union[AnnotationFile, AudioFile, FeatureFile, SpectrogramFile]
 
 
 @attrs.define
 class DatasetFile:
     """A class that represents any file in a dataset.
-    Used when building a :class:`vocalpy.Dataset`.
 
     Attributes
     ----------
     file : AudioFile, SpectrogramFile, AnnotationFile, or FeatureFile
         An instance of one of the specific file types.
         This is the only required argument when instantiating a
         :class:`vocalpy.DatasetFile`; other attributes are determined
@@ -60,16 +59,15 @@
         The path to the file, taken from ``file.path``.
 
     Examples
     --------
     >>> import vocalpy as voc
     >>> audio_paths = voc.paths.from_dir('./dir', 'wav')
     >>> audio_files = [voc.AudioFile(path=path) for path in audio_paths]
-    >>> dataset_files = [voc.DatasetFile(file=audio_file) for audio_file in audio_files]
-    >>> dataset = voc.Dataset(files=dataset_files)
+    >>> dataset_files = [voc.DatasetFile(file=audio_file) for sound_file in audio_files]
     """
 
     file: DatasetFileType = attrs.field(
         validator=attrs.validators.instance_of((AnnotationFile, AudioFile, FeatureFile, SpectrogramFile))
     )
 
     def __attrs_post_init__(self):
```

### Comparing `vocalpy-0.8.2/src/vocalpy/examples/BM003.wav` & `vocalpy-0.9.0/src/vocalpy/examples/BM003.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/examples/bells.wav` & `vocalpy-0.9.0/src/vocalpy/examples/bells.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/examples/flashcam.wav` & `vocalpy-0.9.0/src/vocalpy/examples/flashcam.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/examples/samba.wav` & `vocalpy-0.9.0/src/vocalpy/examples/samba.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/examples/simple.wav` & `vocalpy-0.9.0/src/vocalpy/examples/simple.wav`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/feature/sat.py` & `vocalpy-0.9.0/src/vocalpy/feature/sat.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 import librosa
 import numpy as np
 import numpy.typing as npt
 import xarray as xr
 
 if TYPE_CHECKING:
-    from .. import Audio, Spectrogram
+    from .. import Features, Segment, Sound, Spectrogram
 
-from .. import spectral
+from .. import spectral, validators
 
 # get small number to avoid potential divide by zero errors
 EPS = np.finfo(np.double).eps
 
 
 def goodness_of_pitch(cepstrogram: npt.NDArray, quefrencies: npt.NDArray, max_F0: float = 1830.0) -> npt.NDArray:
     """Calculate goodness of pitch
@@ -32,15 +32,15 @@
     between ``quefrencies`` greater than ``1 / max_F0``
     and less than ``int(np.floor(len(cepstrogram) / 2))``.
 
     Parameters
     ----------
     cepstrogram : numpy.ndarray
         Cepstrogram returned by :func:`vocalpy.spectral.sat`,
-        matrix with dimensions (quefrencies, time bins).
+        matrix with dimensions (channels, quefrencies, time bins).
     quefrencies : numpy.ndarray
         The quefrencies for the cepstrogram.
     max_F0 : float
         Maximum frequency to consider,
         that becomes the lowest ``quefrency``
         used when computing goodness of pitch.
 
@@ -71,31 +71,30 @@
     quefrency_cutoff = 1 / max_F0
     if quefrency_cutoff > quefrencies.max():
         raise ValueError(
             f"`max_F0` of {max_F0} gives a quefrency cut-off of {quefrency_cutoff}, "
             f"but this is greater than the max value in `quefrencies`: {quefrencies.max()}"
         )
     min_quef_idx = np.min(np.argwhere(quefrencies > quefrency_cutoff)) - 1
-    max_quef_idx = int(np.floor(len(cepstrogram) / 2))
-    return np.max(cepstrogram[min_quef_idx:max_quef_idx, :], axis=0)
+    max_quef_idx = int(np.floor(cepstrogram.shape[1] / 2))
+    return np.max(cepstrogram[:, min_quef_idx:max_quef_idx, :], axis=1)
 
 
 def mean_frequency(power_spectrogram: Spectrogram, min_freq: float = 380.0, max_freq: float = 11025.0) -> npt.NDArray:
     """Calculate mean frequency.
 
     Finds the mean for each column in ``power_spectrogram``,
     between the frequencies specified by ``min_freq`` and ``max_freq``.
     To find the mean, the frequencies are weighted by their power
     in ``power_spectrogram`` and then divided by the sum of that power.
 
     Parameters
     ----------
     power_spectrogram : vocalpy.Spectrogram
-        Spectrogram, returned by
-        :func:`vocalpy.spectral.sat`.
+        Spectrogram, returned by :func:`vocalpy.spectral.sat`.
     min_freq : float
         The minimum frequency to consider in ``power_spectrogram``.
     max_freq : float
         The maximum frequency to consider in ``power_spectrogram``.
         Returned by :func`:vocalpy.spectral.sat`, computing using the
         ``freq_range`` argument to that function.
 
@@ -121,18 +120,18 @@
        by Therese Koch, specifically the acoustics module
 
     See Also
     --------
     pitch
     """
     freq_inds = (power_spectrogram.frequencies > min_freq) & (power_spectrogram.frequencies < max_freq)
-    P = power_spectrogram.data[freq_inds, :]
-    P[P == 0.0] = EPS
+    P = power_spectrogram.data[:, freq_inds, :]
+    P[P == 0.0] += np.finfo(P.dtype).eps
     frequencies = power_spectrogram.frequencies[freq_inds]
-    return np.sum(P * frequencies[:, np.newaxis], axis=0) / np.sum(P, axis=0)
+    return np.sum(P * frequencies[:, np.newaxis], axis=1) / np.sum(P, axis=1)
 
 
 def frequency_modulation(dSdt: npt.NDArray, dSdf: npt.NDArray) -> npt.NDArray:
     """Calculate frequency modulation.
 
     Parameters
     ----------
@@ -161,15 +160,15 @@
     .. [1] `Sound Analysis Tools <http://soundanalysispro.com/matlab-sat>`_ for Matlab (SAT) by Ofer Tchernichovski
     .. [2] `birdsonganalysis <https://github.com/PaulEcoffet/birdsonganalysis>`_  by Paul Ecoffet
     .. [3] `avn <https://github.com/theresekoch/avn/blob/main/avn/acoustics.py>`_
        by Therese Koch, specifically the acoustics module
     .. [4] Bradbury, Jack W., and Sandra Lee Vehrencamp. Principles of animal communication. Vol. 132.
        Sunderland, MA: Sinauer Associates, 1998.
     """
-    return np.arctan(np.max(dSdt, axis=0) / (np.max(dSdf, axis=0) + EPS))
+    return np.arctan(np.max(dSdt, axis=1) / (np.max(dSdf, axis=1) + np.finfo(dSdt.dtype).eps))
 
 
 def amplitude_modulation(dSdt: npt.NDArray) -> npt.NDArray:
     """Calculates the amplitude modulation.
 
     Parameters
     ----------
@@ -195,15 +194,15 @@
     .. [1] `Sound Analysis Tools <http://soundanalysispro.com/matlab-sat>`_ for Matlab (SAT) by Ofer Tchernichovski
     .. [2] `birdsonganalysis <https://github.com/PaulEcoffet/birdsonganalysis>`_  by Paul Ecoffet
     .. [3] `avn <https://github.com/theresekoch/avn/blob/main/avn/acoustics.py>`_
        by Therese Koch, specifically the acoustics module
     .. [4] Bradbury, Jack W., and Sandra Lee Vehrencamp. Principles of animal communication. Vol. 132.
        Sunderland, MA: Sinauer Associates, 1998.
     """
-    return np.sum(dSdt, axis=0)
+    return np.sum(dSdt, axis=1)
 
 
 def entropy(power_spectrogram: Spectrogram, min_freq: float = 380.0, max_freq: float = 11025.0) -> npt.NDArray:
     """Calculate Wiener entropy
 
     Computes the Wiener entropy for each column in ``power_spectrogram``,
     between the frequencies specified by ``min_freq`` and ``max_freq``.
@@ -243,20 +242,20 @@
     ----------
     .. [1] `Sound Analysis Tools <http://soundanalysispro.com/matlab-sat>`_ for Matlab (SAT) by Ofer Tchernichovski
     .. [2] `birdsonganalysis <https://github.com/PaulEcoffet/birdsonganalysis>`_  by Paul Ecoffet
     .. [3] `avn <https://github.com/theresekoch/avn/blob/main/avn/acoustics.py>`_
        by Therese Koch, specifically the acoustics module
     """
     freq_inds = (power_spectrogram.frequencies > min_freq) & (power_spectrogram.frequencies < max_freq)
-    P = power_spectrogram.data[freq_inds, :]
-    P[P == 0.0] = EPS
+    P = power_spectrogram.data[:, freq_inds, :]
+    P[P == 0.0] += np.finfo(P.dtype).eps
     # calculate entropy for current frame
-    sum_log = np.sum(np.log(P), axis=0)
-    log_sum = np.log(np.sum(P, axis=0) / (P.shape[0] - 1))
-    return sum_log / (P.shape[0] - 1) - log_sum
+    sum_log = np.sum(np.log(P), axis=1)
+    log_sum = np.log(np.sum(P, axis=1) / (P.shape[1] - 1))
+    return sum_log / (P.shape[1] - 1) - log_sum
 
 
 def amplitude(
     power_spectrogram: Spectrogram, min_freq: float = 380.0, max_freq: float = 11025.0, baseline: float = 70.0
 ) -> npt.NDArray:
     """Calculate amplitude.
 
@@ -295,35 +294,35 @@
     ----------
     .. [1] `Sound Analysis Tools <http://soundanalysispro.com/matlab-sat>`_ for Matlab (SAT) by Ofer Tchernichovski
     .. [2] `birdsonganalysis <https://github.com/PaulEcoffet/birdsonganalysis>`_  by Paul Ecoffet
     .. [3] `avn <https://github.com/theresekoch/avn/blob/main/avn/acoustics.py>`_
        by Therese Koch, specifically the acoustics module
     """
     freq_inds = (power_spectrogram.frequencies > min_freq) & (power_spectrogram.frequencies < max_freq)
-    P = power_spectrogram.data[freq_inds, :]
-    P[P == 0.0] = EPS
-    return 10 * np.log10(np.sum(P, axis=0)) + baseline
+    P = power_spectrogram.data[:, freq_inds, :]
+    P[P == 0.0] += np.finfo(P.dtype).eps
+    return 10 * np.log10(np.sum(P, axis=1)) + baseline
 
 
 def pitch(
-    audio: Audio,
+    sound: Sound,
     fmin: float = 380.0,
     fmax_yin: float = 8000.0,
     frame_length: int = 400,
     hop_length: int = 40,
     trough_threshold: float = 0.1,
 ):
     """Estimates the fundamental frequency (or pitch) using the YIN algorithm [1]_.
 
     The pitch is computed using :func:`librosa.yin`.
 
     Parameters
     ----------
-    audio : vocalpy.Audio
-        A :class:`vocalpy.Audio` instance.
+    sound : vocalpy.Sound
+        A :class:`vocalpy.Sound` instance. Multi-channel is supported.
     fmin : float
         Minimum frequency in Hertz.
         The recommended minimum is ``librosa.note_to_hz('C2')`` (~65 Hz)
         though lower values may be feasible.
     fmax_yin : float
         Maximum frequency in Hertz.
         Default is 8000.
@@ -358,45 +357,101 @@
            The Journal of the Acoustical Society of America 111.4 (2002): 1917-1930.
     .. [2] `Sound Analysis Tools <http://soundanalysispro.com/matlab-sat>`_ for Matlab (SAT) by Ofer Tchernichovski
     .. [3] `birdsonganalysis <https://github.com/PaulEcoffet/birdsonganalysis>`_  by Paul Ecoffet
     .. [4] `avn <https://github.com/theresekoch/avn/blob/main/avn/acoustics.py>`_
            by Therese Koch, specifically the acoustics module
     """
     return librosa.yin(
-        audio.data,
+        sound.data,
         fmin=fmin,
         fmax=fmax_yin,
-        sr=audio.samplerate,
+        sr=sound.samplerate,
         frame_length=frame_length,
         hop_length=hop_length,
         trough_threshold=trough_threshold,
     )
 
 
+def _get_cepstral(spectra1: npt.NDArray, n_fft: int, samplerate: int) -> tuple[npt.NDArray, npt.NDArray]:
+    """Get cepstrogram and quefrencies from a spectrogram
+
+    Helper function used by :func:`similarity_features` to compute
+    :func:`goodness_of_pitch` feature.
+
+    Parameters
+    ----------
+    spectra1
+    n_fft : int
+    sound : Sound
+
+    Returns
+    -------
+    cepstrogram : numpy.ndarray
+    quefrencies : numpy.ndarray
+    """
+    # ---- make "cepstrogram" and quefrencies
+    spectra1_for_cepstrum = np.copy(spectra1)
+    # next line is a fancy way of adding eps to zero values
+    # so we don't get the enigmatic divide-by-zero error, and we don't get np.inf values
+    # see https://github.com/numpy/numpy/issues/21560
+    spectra1_for_cepstrum[spectra1_for_cepstrum == 0.0] += np.finfo(spectra1_for_cepstrum.dtype).eps
+    cepstrogram = np.fft.ifft(np.log(np.abs(spectra1_for_cepstrum)), n=n_fft, axis=1).real
+    quefrencies = np.array(np.arange(n_fft)) / samplerate
+    return cepstrogram, quefrencies
+
+
+def _get_spectral_derivatives(
+    spectra1: npt.NDArray, spectra2: npt.NDArray, max_freq_idx: int
+) -> tuple[npt.NDArray, npt.NDArray]:
+    """Get derivatives of spectrogram with respect to time and frequency.
+
+    Helper function used by :func:`similarity_features` to compute
+    :func:`amplitude_modulation` and :func:`frequency_modulation` feature
+
+    Parameters
+    ----------
+    spectra1
+    spectra2
+    max_freq_idx : int
+
+    Returns
+    -------
+    dSdt : numpy.ndarray
+    dSdf : numpy.ndarray
+    """
+    spectra1 = spectra1[:, :max_freq_idx, :]
+    spectra2 = spectra2[:, :max_freq_idx, :]
+    # time derivative of spectrum
+    dSdt = (-spectra1.real * spectra2.real) - (spectra1.imag * spectra2.imag)
+    # frequency derivative of spectrum
+    dSdf = (spectra1.imag * spectra2.real) - (spectra1.real * spectra2.imag)
+    return dSdt, dSdf
+
+
 def similarity_features(
-    audio: Audio,
+    source: Sound | Segment,
     n_fft=400,
     hop_length=40,
     freq_range=0.5,
     min_freq: float = 380.0,
     amp_baseline: float = 70.0,
-    max_F0: int = 1830.0,
+    max_F0: float = 1830.0,
     fmax_yin: float = 8000.0,
     trough_threshold: float = 0.1,
-) -> xr.DataSet:
-    """Extract all features used to compute similarity with SAT.
-
-    Calls :func:`vocalpy.spectral.sat` to get spectral representations
-    of the :class:`vocalpy.Audio`, then extracts all features
-    from those spectral representations.
+) -> Features:
+    """Extract all features used to compute similarity with
+    the Sound Analysis Toolbox for Matlab (SAT).
 
     Parameters
     ----------
-    audio : vocalpy.Audio
-        Audio loaded from a file.
+    source : Sound or Segment
+        A :class:`Sound` loaded from a file,
+        or a :class:`Segment` produced by an algorithm
+        in :mod:`vocalpy.segment`.
+        Multi-channel sounds are supported.
     n_fft : int
         FFT window size.
     hop_length : int
         Number of audio samples between adjacent STFT columns.
     freq_range : float
         Range of frequencies to use, given as a value
         between zero and one.
@@ -423,30 +478,59 @@
 
     Returns
     -------
     features : xarray.Dataset
         An xarray.Dataset where the data variables are the features,
         and the coordinate is the time for each time bin.
     """
-    # pitch, goodness, AM, FM, entropy
-    power_spectrogram, cepstrogram, quefrencies, max_freq, dSdt, dSdf = spectral.sat(
-        audio, n_fft, hop_length, freq_range
-    )
-    amp_ = amplitude(power_spectrogram, min_freq, max_freq, amp_baseline)
+    validators.is_sound_or_segment(source)
+
+    if not 0.0 < freq_range <= 1.0:
+        raise ValueError(
+            f"`freq_range` must be a float greater than zero and less than or equal to 1.0, but was: {freq_range}. "
+            f"Please specify a value between zero and one inclusive specifying the percentage of the frequencies "
+            f"to use when extracting features with a frequency range"
+        )
+
+    power_spectrogram, spectra1, spectra2 = spectral.sat._sat_multitaper(source, n_fft, hop_length)
+
+    # in SAT, freq_range means "use first `freq_range` percent of frequencies". Next line finds that range.
+    f = power_spectrogram.frequencies
+    max_freq_idx = int(np.floor(f.shape[0] * freq_range))
+    max_freq = f[max_freq_idx]
+
+    # ---- now extract features
+    # -------- features that require sound
     pitch_ = pitch(
-        audio, min_freq, fmax_yin, frame_length=n_fft, hop_length=hop_length, trough_threshold=trough_threshold
+        source, min_freq, fmax_yin, frame_length=n_fft, hop_length=hop_length, trough_threshold=trough_threshold
     )
+
+    # -------- features that require power spectrogram and max_freq
+    amp_ = amplitude(power_spectrogram, min_freq, max_freq, amp_baseline)
+    entropy_ = entropy(power_spectrogram, min_freq, max_freq)
+
+    # -------- features that require cepstrogram
+    cepstrogram, quefrencies = _get_cepstral(spectra1, n_fft, source.samplerate)
     goodness_ = goodness_of_pitch(cepstrogram, quefrencies, max_F0)
+
+    # -------- features that spectral derivatives
+    dSdt, dSdf = _get_spectral_derivatives(spectra1, spectra2, max_freq_idx)
     FM = frequency_modulation(dSdt, dSdf)
     AM = amplitude_modulation(dSdt)
-    entropy_ = entropy(power_spectrogram, min_freq, max_freq)
-    return xr.Dataset(
+
+    channels = np.arange(source.data.shape[0])
+    data = xr.Dataset(
         {
-            "amplitude": (["time"], amp_),
-            "pitch": (["time"], pitch_),
-            "goodness_of_pitch": (["time"], goodness_),
-            "frequency_modulation": (["time"], FM),
-            "amplitude_modulation": (["time"], AM),
-            "entropy": (["time"], entropy_),
+            "amplitude": (["channel", "time"], amp_),
+            "pitch": (["channel", "time"], pitch_),
+            "goodness_of_pitch": (["channel", "time"], goodness_),
+            "frequency_modulation": (["channel", "time"], FM),
+            "amplitude_modulation": (["channel", "time"], AM),
+            "entropy": (["channel", "time"], entropy_),
         },
-        coords={"time": power_spectrogram.times},
+        coords={"channel": channels, "time": power_spectrogram.times},
     )
+
+    from .. import Features  # avoid circular import
+
+    features = Features(data=data)
+    return features
```

### Comparing `vocalpy-0.8.2/src/vocalpy/feature_file.py` & `vocalpy-0.9.0/src/vocalpy/feature_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,14 @@
     """Class that represents a file containing
     features extracted from data,
     e.g., acoustic parameters.
 
     The features file is part of a dataset used to study
     animal acoustic communication.
 
-    Used by the :class:`vocalpy.Dataset` class.
-
     Attributes
     ----------
     path : pathlib.Path
         The path to the annotation file.
     source_file : AudioFile, SpectrogramFile, or AnnotationFile
         The file that features were extracted from.
         A feature file can have either a single `source_file`
```

### Comparing `vocalpy-0.8.2/src/vocalpy/metrics/segmentation/ir.py` & `vocalpy-0.9.0/src/vocalpy/metrics/segmentation/ir.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,27 +283,27 @@
     This is also sometimes known as a "collar" [2]_ or "forgiveness collar" [3]_.
     The value for the tolerance can be determined by visual inspection
     of the distribution; see for example [4]_.
 
     References
     ----------
     .. [1] Kemp, T., Schmidt, M., Whypphal, M., & Waibel, A. (2000, June).
-    Strategies for automatic segmentation of audio data.
-    In 2000 ieee international conference on acoustics, speech, and signal processing.
-    proceedings (cat. no. 00ch37100) (Vol. 3, pp. 1423-1426). IEEE.
+       Strategies for automatic segmentation of audio data.
+       In 2000 ieee international conference on acoustics, speech, and signal processing.
+       proceedings (cat. no. 00ch37100) (Vol. 3, pp. 1423-1426). IEEE.
 
     .. [2] Jordán, P. G., & Giménez, A. O. (2023).
-    Advances in Binary and Multiclass Audio Segmentation with Deep Learning Techniques.
+       Advances in Binary and Multiclass Sound Segmentation with Deep Learning Techniques.
 
     .. [3] NIST. (2009). The 2009 (RT-09) Rich Transcription Meeting Recognition Evaluation Plan.
-    https://web.archive.org/web/20100606041157if_/http://www.itl.nist.gov/iad/mig/thyps/rt/2009/docs/rt09-meeting-eval-plan-v2.pdf
+       https://web.archive.org/web/20100606041157if_/http://www.itl.nist.gov/iad/mig/thyps/rt/2009/docs/rt09-meeting-eval-plan-v2.pdf
 
     .. [4] Du, P., & Troyer, T. W. (2006).
-    A segmentation algorithm for zebra finch song at the note level.
-    Neurocomputing, 69(10-12), 1375-1379.
+       A segmentation algorithm for zebra finch song at the note level.
+       Neurocomputing, 69(10-12), 1375-1379.
     """
     if metric not in {"precision", "recall", "fscore"}:
         raise ValueError(f'``metric`` must be one of: {{"precision", "recall", "fscore"}} but was: {metric}')
 
     # If we have no boundaries, we get no score.
     if len(reference) == 0 or len(hypothesis) == 0:
         return 0.0, 0, IRMetricData(hits_ref=np.array([]), hits_hyp=np.array([]), diffs=np.array([]))
@@ -433,27 +433,27 @@
     This is also sometimes known as a "collar" [2]_ or "forgiveness collar" [3]_.
     The value for the tolerance can be determined by visual inspection
     of the distribution; see for example [4]_.
 
     References
     ----------
     .. [1] Kemp, T., Schmidt, M., Whypphal, M., & Waibel, A. (2000, June).
-    Strategies for automatic segmentation of audio data.
-    In 2000 ieee international conference on acoustics, speech, and signal processing.
-    proceedings (cat. no. 00ch37100) (Vol. 3, pp. 1423-1426). IEEE.
+       Strategies for automatic segmentation of audio data.
+       In 2000 ieee international conference on acoustics, speech, and signal processing.
+       proceedings (cat. no. 00ch37100) (Vol. 3, pp. 1423-1426). IEEE.
 
     .. [2] Jordán, P. G., & Giménez, A. O. (2023).
-    Advances in Binary and Multiclass Audio Segmentation with Deep Learning Techniques.
+       Advances in Binary and Multiclass Sound Segmentation with Deep Learning Techniques.
 
     .. [3] NIST. (2009). The 2009 (RT-09) Rich Transcription Meeting Recognition Evaluation Plan.
-    https://web.archive.org/web/20100606041157if_/http://www.itl.nist.gov/iad/mig/thyps/rt/2009/docs/rt09-meeting-eval-plan-v2.pdf
+       https://web.archive.org/web/20100606041157if_/http://www.itl.nist.gov/iad/mig/thyps/rt/2009/docs/rt09-meeting-eval-plan-v2.pdf
 
     .. [4] Du, P., & Troyer, T. W. (2006).
-    A segmentation algorithm for zebra finch song at the note level.
-    Neurocomputing, 69(10-12), 1375-1379.
+       A segmentation algorithm for zebra finch song at the note level.
+       Neurocomputing, 69(10-12), 1375-1379.
     """
     return precision_recall_fscore(hypothesis, reference, "precision", tolerance, decimals)
 
 
 def recall(
     hypothesis: npt.NDArray,
     reference: npt.NDArray,
@@ -559,27 +559,27 @@
     This is also sometimes known as a "collar" [2]_ or "forgiveness collar" [3]_.
     The value for the tolerance can be determined by visual inspection
     of the distribution; see for example [4]_.
 
     References
     ----------
     .. [1] Kemp, T., Schmidt, M., Whypphal, M., & Waibel, A. (2000, June).
-    Strategies for automatic segmentation of audio data.
-    In 2000 ieee international conference on acoustics, speech, and signal processing.
-    proceedings (cat. no. 00ch37100) (Vol. 3, pp. 1423-1426). IEEE.
+       Strategies for automatic segmentation of audio data.
+       In 2000 ieee international conference on acoustics, speech, and signal processing.
+       proceedings (cat. no. 00ch37100) (Vol. 3, pp. 1423-1426). IEEE.
 
     .. [2] Jordán, P. G., & Giménez, A. O. (2023).
-    Advances in Binary and Multiclass Audio Segmentation with Deep Learning Techniques.
+       Advances in Binary and Multiclass Sound Segmentation with Deep Learning Techniques.
 
     .. [3] NIST. (2009). The 2009 (RT-09) Rich Transcription Meeting Recognition Evaluation Plan.
-    https://web.archive.org/web/20100606041157if_/http://www.itl.nist.gov/iad/mig/thyps/rt/2009/docs/rt09-meeting-eval-plan-v2.pdf
+       https://web.archive.org/web/20100606041157if_/http://www.itl.nist.gov/iad/mig/thyps/rt/2009/docs/rt09-meeting-eval-plan-v2.pdf
 
     .. [4] Du, P., & Troyer, T. W. (2006).
-    A segmentation algorithm for zebra finch song at the note level.
-    Neurocomputing, 69(10-12), 1375-1379.
+       A segmentation algorithm for zebra finch song at the note level.
+       Neurocomputing, 69(10-12), 1375-1379.
     """
     return precision_recall_fscore(hypothesis, reference, "recall", tolerance, decimals)
 
 
 def fscore(
     hypothesis: npt.NDArray,
     reference: npt.NDArray,
@@ -682,27 +682,27 @@
     This is also sometimes known as a "collar" [2]_ or "forgiveness collar" [3]_.
     The value for the tolerance can be determined by visual inspection
     of the distribution; see for example [4]_.
 
     References
     ----------
     .. [1] Kemp, T., Schmidt, M., Whypphal, M., & Waibel, A. (2000, June).
-    Strategies for automatic segmentation of audio data.
-    In 2000 ieee international conference on acoustics, speech, and signal processing.
-    proceedings (cat. no. 00ch37100) (Vol. 3, pp. 1423-1426). IEEE.
+       Strategies for automatic segmentation of audio data.
+       In 2000 ieee international conference on acoustics, speech, and signal processing.
+       proceedings (cat. no. 00ch37100) (Vol. 3, pp. 1423-1426). IEEE.
 
     .. [2] Jordán, P. G., & Giménez, A. O. (2023).
-    Advances in Binary and Multiclass Audio Segmentation with Deep Learning Techniques.
+       Advances in Binary and Multiclass Sound Segmentation with Deep Learning Techniques.
 
     .. [3] NIST. (2009). The 2009 (RT-09) Rich Transcription Meeting Recognition Evaluation Plan.
-    https://web.archive.org/web/20100606041157if_/http://www.itl.nist.gov/iad/mig/thyps/rt/2009/docs/rt09-meeting-eval-plan-v2.pdf
+       https://web.archive.org/web/20100606041157if_/http://www.itl.nist.gov/iad/mig/thyps/rt/2009/docs/rt09-meeting-eval-plan-v2.pdf
 
     .. [4] Du, P., & Troyer, T. W. (2006).
-    A segmentation algorithm for zebra finch song at the note level.
-    Neurocomputing, 69(10-12), 1375-1379.
+       A segmentation algorithm for zebra finch song at the note level.
+       Neurocomputing, 69(10-12), 1375-1379.
     """
     return precision_recall_fscore(hypothesis, reference, "fscore", tolerance, decimals)
 
 
 def concat_starts_and_stops(starts: npt.NDArray, stops: npt.NDArray) -> npt.NDArray:
     """Concatenate arrays of start and stop times
     into a single array of boundary times.
```

### Comparing `vocalpy-0.8.2/src/vocalpy/paths.py` & `vocalpy-0.9.0/src/vocalpy/paths.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/plot/annot.py` & `vocalpy-0.9.0/src/vocalpy/plot/annot.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/plot/spect.py` & `vocalpy-0.9.0/src/vocalpy/plot/spect.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Functions for plotting spectrograms"""
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
+import numpy as np
 
 from .._spectrogram.data_type import Spectrogram
 from ..annotation import Annotation
 from .annot import annotation
 
 
 def spectrogram(
@@ -33,21 +34,33 @@
         Default is None, in which case entire range of f will be plotted.
     ax : matplotlib.axes.Axes
         axes on which to plot spectrogram
     pcolormesh_kwargs : dict
         keyword arguments passed to :meth:`matplotlib.axes.Axes.pcolormesh`
         method used to plot spectrogram. Default is None.
     """
+    if spect.data.shape[0] > 1:
+        raise ValueError(
+            f"Spectrogram data has more than one channel. Number of channels was: {spect.data.shape[0]}."
+            "This happens when spectral representations are generated from multi-channel audio. "
+            "Plotting multiple channels is not currently supported. "
+            "To plot individual channels, either index into the spectrogram "
+            "to get a new spectrogram of a specific channel:\n"
+            ">>> spect0 = spect[0]  # gets channel 0\n"
+            "Or iterate through the spectrogram to get all the channels:\n"
+            ">>> per_channel_spects = [channel_spect for channel_spect in spect]"
+        )
+
     if ax is None:
         fig, ax = plt.subplots()
 
     if pcolormesh_kwargs is None:
         pcolormesh_kwargs = {}
 
-    ax.pcolormesh(spect.times, spect.frequencies, spect.data, **pcolormesh_kwargs)
+    ax.pcolormesh(spect.times, spect.frequencies, np.squeeze(spect.data, axis=0), **pcolormesh_kwargs)
 
     if tlim is not None:
         ax.set_xlim(tlim)
 
     if flim is not None:
         ax.set_ylim(flim)
```

### Comparing `vocalpy-0.8.2/src/vocalpy/segmenter.py` & `vocalpy-0.9.0/src/vocalpy/segmenter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 """Class that represents the segmenting step in a pipeline."""
 from __future__ import annotations
 
-from typing import Callable
+import collections.abc
+import inspect
+from typing import TYPE_CHECKING, Callable, Mapping
 
 import dask
 import dask.diagnostics
 
-from .audio import Audio
 from .audio_file import AudioFile
-from .sequence import Sequence
-from .spectrogram_maker import validate_audio
-from .unit import Unit
+from .params import Params
+from .sound import Sound
+from .spectrogram_maker import validate_sound
+
+if TYPE_CHECKING:
+    from .segments import Segments
+
 
 DEFAULT_SEGMENT_PARAMS = {
     "threshold": 5000,
     "min_dur": 0.02,
     "min_silent_dur": 0.002,
 }
 
@@ -25,123 +30,124 @@
     Attributes
     ----------
     callback : callable, optional
         The function or :class:`Callable` class instance
         that is used to segment.
         If not specified, defaults to
         :func:`vocalpy.segment.meansquared`.
-    method : str, optional.
-        The name of the function to use to segment.
-    segment_params : dict, optional.
+    params : Mapping or Params, optional.
+        Parameters passed to ``callback``.
+        A :class:`Mapping` of keyword arguments,
+        or one of the :class:`Params` classes that
+        represents parameters, e.g.,
+        class:`vocalpy.segment.MeanSquaredParams`.
         If not specified, defaults to
         :const:`vocalpy.segmenter.DEFAULT_SEGMENT_PARAMS`.
     """
 
-    def __init__(self, callback: Callable | None = None, method: str | None = None, segment_params: dict | None = None):
+    def __init__(self, callback: Callable | None = None, params: Mapping | Params | None = None):
         """Initialize a new :class:`vocalpy.Segmenter` instance.
 
         Parameters
         ----------
         callback : callable, optional
             The function or :class:`Callable` class instance
             that is used to segment.
             If not specified, defaults to
             :func:`vocalpy.segment.meansquared`.
-        method : str, optional.
-            The name of the function to use to segment.
-        segment_params : dict, optional.
+        params : Mapping or Params, optional.
+            Parameters passed to ``callback``.
+            A :class:`Mapping` of keyword arguments,
+            or one of the :class:`Params` classes that
+            represents parameters, e.g.,
+            class:`vocalpy.segment.MeanSquaredParams`.
             If not specified, defaults to
             :data:`vocalpy.segmenter.DEFAULT_SEGMENT_PARAMS`.
         """
-        if callback and method:
-            raise ValueError("Cannot specify both `callback` and `method`, only one or the other.")
-
-        if method:
-            import vocalpy.signal.segment
-
-            # TODO: fix this
-            try:
-                callback = getattr(vocalpy.segment, method)
-            except AttributeError:
-                raise AttributeError(f"Method was '{method}' but `vocalpy.segment` has no function named `{method}`")
-
         if callback is None:
-            from vocalpy.segment import meansquared as default_segment_func
+            from vocalpy.segment import meansquared
 
-            callback = default_segment_func
+            callback = meansquared
+            # if callback was None and we use the default,
+            # **and** params is None, we set these default params
+            if params is None:
+                params = DEFAULT_SEGMENT_PARAMS
+        else:
+            # if we *don't* use the default callback **and** params is None,
+            # then we instead get the defaults for the specified callback
+            if params is None:
+                params = {}
+                signature = inspect.signature(callback)
+                for name, param in signature.parameters.items():
+                    if param.default is not inspect._empty:
+                        params[name] = param.default
 
-        if callback is not None and not callable(callback):
+        if not callable(callback):
             raise ValueError(f"`callback` should be callable, but `callable({callback})` returns False")
 
         self.callback = callback
 
-        if segment_params is None:
-            segment_params = DEFAULT_SEGMENT_PARAMS
-        if not isinstance(segment_params, dict):
-            raise TypeError(f"`segment_params` should be a `dict` but type was: {type(segment_params)}")
+        if not isinstance(params, (collections.abc.Mapping, Params)):
+            raise TypeError(f"`params` should be a `Mapping` or `Params` but type was: {type(params)}")
 
-        self.segment_params = segment_params
+        if isinstance(params, Params):
+            # coerce to dict
+            params = {**params}
+
+        signature = inspect.signature(callback)
+        if not all([param in signature.parameters for param in params]):
+            invalid_params = [param for param in params if param not in signature.parameters]
+            raise ValueError(
+                f"Invalid params for callback: {invalid_params}\n" f"Callback parameters are: {signature.parameters}"
+            )
+
+        self.params = params
 
     def segment(
         self,
-        audio: Audio | AudioFile | list[Audio | AudioFile],
+        sound: Sound | AudioFile | list[Sound | AudioFile],
         parallelize: bool = True,
-    ) -> Sequence | None | list[Sequence | None]:
-        """Segment audio into sequences.
+    ) -> Segments | list[Segments]:
+        """Segment sound.
 
         Parameters
         ----------
-        audio : vocalpy.Audio or list of Audio
-            A `class`:vocalpy.Audio` instance
-            or list of :class:`vocalpy.Audio` instances
+        sound : vocalpy.Sound or list of Sound
+            A `class`:vocalpy.Sound` instance
+            or list of :class:`vocalpy.Sound` instances
             to segment.
         parallelize : bool
             If True, parallelize segmentation using :mod:`dask`.
 
         Returns
         -------
-        seq : vocalpy.Sequence, None, or list of vocalpy.Sequence or None
-            If a single :class:`~vocalpy.Audio` instance is passed in,
-            a single :class:`~vocalpy.Sequence` instance will be returned.
-            If a list of :class:`~vocalpy.Audio` instances is passed in,
-            a list of :class:`~vocalpy.Sequence` instances will be returned.
+        segments : vocalpy.Segments, list
+            If a :class:`~vocalpy.Sound` is passed in,
+            a single set of :class:`~vocalpy.Segments` will be returned.
+            If a list of :class:`~vocalpy.Sound` is passed in,
+            a list of :class:`~vocalpy.Segments` will be returned.
         """
-        validate_audio(audio)
+        validate_sound(sound)
 
         # define nested function so vars are in scope and ``dask`` can call it
-        def _to_sequence(audio_: Audio):
-            if isinstance(audio_, AudioFile):
-                audio_ = Audio.read(audio_.path)
-            out = self.callback(audio_, **self.segment_params)
-            if out is None:
-                return out
-            else:
-                onsets, offsets = out
-
-            units = []
-            for onset, offset in zip(onsets, offsets):
-                units.append(Unit(onset=onset, offset=offset))
-
-            return Sequence(
-                units=units,
-                # note we make a new audio instance **without** data loaded
-                audio=Audio(path=audio_.path),
-                method=self.callback.__name__,
-                segment_params=self.segment_params,
-            )
+        def _to_segments(sound_: Sound | AudioFile) -> Segments:
+            if isinstance(sound_, AudioFile):
+                sound_ = Sound.read(sound_.path)
+            segments = self.callback(sound_, **self.params)
+            return segments
 
-        if isinstance(audio, (Audio, AudioFile)):
-            return _to_sequence(audio)
+        if isinstance(sound, (Sound, AudioFile)):
+            return _to_segments(sound)
 
-        seqs = []
-        for audio_ in audio:
+        segments = []
+        for sound_ in sound:
             if parallelize:
-                seqs.append(dask.delayed(_to_sequence(audio_)))
+                segments.append(dask.delayed(_to_segments)(sound_))
             else:
-                seqs.append(_to_sequence(audio_))
+                segments.append(_to_segments(sound_))
 
         if parallelize:
-            graph = dask.delayed()(seqs)
+            graph = dask.delayed()(segments)
             with dask.diagnostics.ProgressBar():
                 return graph.compute()
         else:
-            return seqs
+            return segments
```

### Comparing `vocalpy-0.8.2/src/vocalpy/spectrogram.py` & `vocalpy-0.9.0/src/vocalpy/spectrogram.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,87 @@
 """Convenience function that generates a spectrogram."""
 from __future__ import annotations
 
+from typing import Mapping
+
 import librosa
 import numpy as np
 
+from . import spectral
 from ._spectrogram.data_type import Spectrogram
-from .audio import Audio
+from .params import Params
+from .sound import Sound
+
+METHODS = [
+    "librosa-db",
+    "sat-multitaper",
+    "soundsig-spectro",
+]
 
 
-# TODO: add 'SAT' method and 'biosound' method
-def spectrogram(audio: Audio, n_fft: int = 512, hop_length: int = 64, method="librosa-db", **kwargs) -> Spectrogram:
+def spectrogram(
+    sound: Sound, n_fft: int = 512, hop_length: int = 64, method="librosa-db", params: Mapping | Params | None = None
+) -> Spectrogram:
     """Get a spectrogram from audio.
 
-    This is a convenience function that takes an instance of :class:`vocalpy.Audio`
+    This is a convenience function that takes an instance of :class:`vocalpy.Sound`
     and returns an instance of :class:`vocalpy.Spectrogram`. The
     :attr:`vocalpy.Spectrogram.data` will be a spectral representation
     computed according to the specified `method`.
 
     Methods
     =======
-    * `'librosa-db`': equivalent to calling ``S = librosa.STFT(audio.data)``
-       and then ``S = librosa.amplitude_to_db(np.abs(S))``.
+    * `'librosa-db`': dB-scaled spectrogram
+      Equivalent to calling ``S = librosa.STFT(sound.data)``
+      and then ``S = librosa.amplitude_to_db(np.abs(S))``.
+    * ``'sat-multitaper``: multi-taper spectrogram computed the same way
+      that the Sound Analysis Toolbox for Matlab (SAT) does.
+    * ``'soundsig-spectro``: dB-scaled spectrogram
+      computed with Gaussian window; replicates the result of
+      the method ``soundsig.BioSound.spectroCalc`` in the
+      ``soundsig`` package.
 
     Parameters
     ----------
-    audio : vocalpy.Audio
+    sound : vocalpy.Sound
         Audio used to compute spectrogram.
     n_fft : int
         Length of the frame used for the Fast Fourier Transform,
         in number of audio samples. Default is 512.
     hop_length : int
         Number of audio samples to "hop" for each frame
         whe computing the Fast Fourier Transform.
         Smaller values increase the number of columns in the spectrogram,
         without affecting the frequency resolution of the STFT.
     method : str
         Name  of method.
         Default is `'librosa-db'`.
+    params : vocalpy.Params, mapping, None
+        A dictionary-like mapping from function parameter names
+        to argument values.
 
     Returns
     -------
     spect : vocalpy.Spectrogram
         A :class:`vocalpy.Spectrogram` instance
         computed according to `method`
     """
-    if not isinstance(audio, Audio):
-        raise TypeError(f"audio must be an instance of `vocalpy.Audio` but was: {type(audio)}")
+    if not isinstance(sound, Sound):
+        raise TypeError(f"audio must be an instance of `vocalpy.Sound` but was: {type(sound)}")
+
+    if method not in METHODS:
+        raise ValueError(f"Invalid `method`: {method}.\n" f"Valid methods are: {METHODS}\n")
+
     if method == "librosa-db":
-        S = librosa.stft(audio.data, n_fft=n_fft, hop_length=hop_length)
+        S = librosa.stft(sound.data, n_fft=n_fft, hop_length=hop_length)
         S = librosa.amplitude_to_db(np.abs(S))
-        t = librosa.frames_to_time(frames=np.arange(S.shape[-1]), sr=audio.samplerate, hop_length=hop_length)
-        f = librosa.fft_frequencies(sr=audio.samplerate, n_fft=n_fft)
-        return Spectrogram(
-            data=S,
-            frequencies=f,
-            times=t,
-            audio_path=audio.path,
-        )
+        t = librosa.frames_to_time(frames=np.arange(S.shape[-1]), sr=sound.samplerate, hop_length=hop_length)
+        f = librosa.fft_frequencies(sr=sound.samplerate, n_fft=n_fft)
+        spect = Spectrogram(data=S, frequencies=f, times=t, audio_path=sound.path)
+    elif method == "sat-multitaper":
+        spect: Spectrogram = spectral.sat_multitaper(sound, n_fft, hop_length)
+    elif method == "soundsig-spectro":
+        spect: Spectrogram = spectral.soundsig_spectro(sound, n_fft, hop_length, **params)
     else:
         raise ValueError(f"Unknown method: {method}")
+
+    return spect
```

### Comparing `vocalpy-0.8.2/src/vocalpy/spectrogram_file.py` & `vocalpy-0.9.0/src/vocalpy/spectrogram_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,14 @@
 
     A spectrogram file contains the array
     containing the computed spectrogram
     as well as two associated arrays,
     one representing the time bins
     and one representing the frequency bins.
 
-    Used by the :class:`vocalpy.Dataset` class.
-
     Attributes
     ----------
     path : pathlib.Path
         The path to the spectrogram file.
     spectrogram_parameters : vocalpy.dataset.SpectrogramParameters
         The parameters used to compute the spectrogram.
     source_audio_file : vocalpy.dataset.AudioFile
```

### Comparing `vocalpy-0.8.2/src/vocalpy/spectrogram_maker.py` & `vocalpy-0.9.0/src/vocalpy/spectrogram_maker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Class that represents the step in a pipeline that makes spectrograms from audio."""
 from __future__ import annotations
 
+import collections.abc
+import inspect
 import pathlib
-from typing import Callable, List, Sequence, Union
+from typing import Callable, List, Mapping, Sequence, Union
 
 import dask
 import dask.diagnostics
 
 import vocalpy.constants
 
 from ._spectrogram.data_type import Spectrogram
-from .audio import Audio
 from .audio_file import AudioFile
+from .params import Params
+from .sound import Sound
 from .spectrogram_file import SpectrogramFile
 
 
 def default_spect_fname_func(audio_path: Union[str, pathlib.Path]):
     """Default function for naming spectrogram files.
     Adds the extension `.spect.npz` to an audio path.
 
@@ -23,15 +26,15 @@
     ----------
     audio_path : str, pathlib.Path
         A path to an audio file.
 
     Returns
     -------
     spect_fname : pathlib.Path
-        Audio filename with extension added.
+        Sound filename with extension added.
         Default extension is :data:`vocalpy.constants.SPECT_FILE_EXT`.
 
     Notes
     -----
     Adding an extension to the audio path
     (instead of changing it)
     makes it possible to recover the audio path
@@ -40,188 +43,211 @@
     makes it less likely that the spectrogram file
     will overwrite an existing `.npz` file.
     """
     audio_path = pathlib.Path(audio_path)
     return audio_path.name + vocalpy.constants.SPECT_FILE_EXT
 
 
-def validate_audio(audio: Audio | AudioFile | Sequence[Audio | AudioFile]) -> None:
-    if not isinstance(audio, (Audio, AudioFile, list, tuple)):
+def validate_sound(sound: Sound | AudioFile | Sequence[Sound | AudioFile]) -> None:
+    if not isinstance(sound, (Sound, AudioFile, list, tuple)):
         raise TypeError(
-            "`audio` must be a `vocalpy.Audio` instance, "
+            "`sound` must be a `vocalpy.Sound` instance, "
             "a `vocalpy.AudioFile` instance, "
             "or a list/tuple of such instances, "
-            f"but type was : {type(audio)}"
+            f"but type was : {type(sound)}"
         )
 
-    if isinstance(audio, list) or isinstance(audio, tuple):
+    if isinstance(sound, list) or isinstance(sound, tuple):
         if not (
-            all([isinstance(item, Audio) for item in audio]) or all([isinstance(item, AudioFile) for item in audio])
+            all([isinstance(item, Sound) for item in sound]) or all([isinstance(item, AudioFile) for item in sound])
         ):
-            types_in_audio = set([type(audio) for audio in audio])
+            types_in_sound = set([type(sound) for sound in sound])
             raise TypeError(
-                "If `audio` is a list or tuple, "
-                "then items in `audio` must either "
-                "all be instances of `vocalpy.Audio`"
+                "If `sound` is a list or tuple, "
+                "then items in `sound` must either "
+                "all be instances of `vocalpy.Sound`"
                 "or all be instances of `vocalpy.AudioFile`."
-                f"Instead found the following types: {types_in_audio}."
-                f"Please make sure only `vocalpy.Audio instances are in the list/tuple."
+                f"Instead found the following types: {types_in_sound}."
+                f"Please make sure only `vocalpy.Sound instances are in the list/tuple."
             )
 
 
-DEFAULT_SPECT_PARAMS = {"fft_size": 512, "step_size": 64}
+DEFAULT_SPECT_PARAMS = {"n_fft": 512, "hop_length": 64}
 
 
 class SpectrogramMaker:
     """Class that represents the step in a pipeline that makes spectrograms from audio.
 
     Attributes
     ----------
     callback : Callable
-        Callable that takes audio and returns spectrograms.
-        Default is :func:`vocalpy.signal.spectrogram.spectrogram`.
-    spect_params : dict
+        Callable that accepts a :class:`Sound`
+        and returns a :class:`Spectrogram`.
+        Default is :func:`vocalpy.spectrogram`.
+    params : dict
         Parameters for making spectrograms.
         Passed as keyword arguments to ``callback``.
     """
 
-    def __init__(self, callback: Callable | None = None, spect_params: dict | None = None):
+    def __init__(self, callback: Callable | None = None, params: Mapping | Params | None = None):
         if callback is None:
             import vocalpy.spectrogram
 
             callback = vocalpy.spectrogram
+            # if callback was None and we use the default,
+            # **and** params is None, we set these default params
+            if params is None:
+                params = DEFAULT_SPECT_PARAMS
+        else:
+            # if we *don't* use the default callback **and** params is None,
+            # then we instead get the defaults for the specified callback
+            if params is None:
+                params = {}
+                signature = inspect.signature(callback)
+                for name, param in signature.parameters.items():
+                    if param.default is not inspect._empty:
+                        params[name] = param.default
+
         if not callable(callback):
             raise ValueError(f"`callback` should be callable, but `callable({callback})` returns False")
         self.callback = callback
 
-        if spect_params is None:
-            spect_params = DEFAULT_SPECT_PARAMS
-        if not isinstance(spect_params, dict):
-            raise TypeError(f"`spect_params` should be a `dict` but type was: {type(spect_params)}")
-        self.spect_params = spect_params
+        if not isinstance(params, (collections.abc.Mapping, Params)):
+            raise TypeError(f"`params` should be a `Mapping` or `Params` but type was: {type(params)}")
+
+        if isinstance(params, Params):
+            # coerce to dict
+            params = {**params}
+
+        signature = inspect.signature(callback)
+        if not all([param in signature.parameters for param in params]):
+            invalid_params = [param for param in params if param not in signature.parameters]
+            raise ValueError(
+                f"Invalid params for callback: {invalid_params}\n" f"Callback parameters are: {signature.parameters}"
+            )
+
+        self.params = params
 
     def make(
         self,
-        audio: Audio | AudioFile | Sequence[Audio | AudioFile],
+        sound: Sound | AudioFile | Sequence[Sound | AudioFile],
         parallelize: bool = True,
     ) -> Spectrogram | List[Spectrogram]:
         """Make spectrogram(s) from audio.
 
         Makes the spectrograms with `self.callback`
         using the parameters `self.params`.
 
-        Takes as input :class:`vocalpy.Audio` or :class:`vocalpy.AudioFile`,
-        a sequence of either, or a :class:`vocalpy.Dataset` with an
-        ``audio_files`` attribute,
+        Takes as input :class:`vocalpy.Sound` or :class:`vocalpy.AudioFile`,
+        or a sequence of either
         and returns either a :class:`vocalpy.Spectrogram`
-        (given a single :class:`vocalpy.Audio` or :class:`vocalpy.AudioFile` instance)
+        (given a single :class:`vocalpy.Sound` or :class:`vocalpy.AudioFile` instance)
         or a list of :class:`vocalpy.Spectrogram` instances (given a sequence).
 
         Parameters
         ----------
-        audio: vocalpy.Audio, vocalpy.AudioFile, or a sequence of either
+        sound: vocalpy.Sound, vocalpy.AudioFile, or a sequence of either
             Source of audio used to make spectrograms.
 
         Returns
         -------
         spectrogram : vocalpy.Spectrogram or list of vocalpy.Spectrogram
         """
-        validate_audio(audio)
+        validate_sound(sound)
 
         # define nested function so vars are in scope and ``dask`` can call it
-        def _to_spect(audio_):
-            """Make a ``Spectrogram`` from an ``Audio`` instance,
+        def _to_spect(sound_):
+            """Make a ``Spectrogram`` from an ``Sound`` instance,
             using self.callback"""
-            if isinstance(audio_, AudioFile):
-                audio_ = Audio.read(audio_.path)
-            spect = self.callback(audio_, **self.spect_params)
-            spect.audio_path = audio_.path
+            if isinstance(sound_, AudioFile):
+                sound_ = Sound.read(sound_.path)
+            spect = self.callback(sound_, **self.params)
+            spect.audio_path = sound_.path
             return spect
 
-        if isinstance(audio, (Audio, AudioFile)):
-            return _to_spect(audio)
+        if isinstance(sound, (Sound, AudioFile)):
+            return _to_spect(sound)
 
         spects = []
-        for audio_ in audio:
+        for sound_ in sound:
             if parallelize:
-                spects.append(dask.delayed(_to_spect(audio_)))
+                spects.append(dask.delayed(_to_spect)(sound_))
             else:
-                spects.append(_to_spect(audio_))
+                spects.append(_to_spect(sound_))
 
         if parallelize:
             graph = dask.delayed()(spects)
             with dask.diagnostics.ProgressBar():
                 return graph.compute()
         else:
             return spects
 
     def write(
         self,
-        audio: Audio | AudioFile | Sequence[Audio | AudioFile],
+        sound: Sound | AudioFile | Sequence[Sound | AudioFile],
         dir_path: str | pathlib.Path,
         parallelize: bool = True,
         namer: Callable = default_spect_fname_func,
     ) -> SpectrogramFile | List[SpectrogramFile]:
         """Make spectrogram(s) from audio, and write to file.
         Writes directly to file without returning the spectrograms,
         so that datasets can be generated that are too big
         to fit in memory.
 
         Makes the spectrograms with `self.callback`
         using the parameters `self.params`.
 
-        Takes as input :class:`vocalpy.Audio` or :class:`vocalpy.AudioFile`,
-        a sequence of either, or a :class:`vocalpy.Dataset` with an
-        ``audio_files`` attribute,
+        Takes as input :class:`vocalpy.Sound` or :class:`vocalpy.AudioFile`,
+        or a sequence of either,
         and returns either a :class:`vocalpy.SpectrogramFile`
-        (given a single :class:`vocalpy.Audio` or :class:`vocalpy.AudioFile` instance)
+        (given a single :class:`vocalpy.Sound` or :class:`vocalpy.AudioFile` instance)
         or a list of :class:`vocalpy.Spectrogram` instances (given a sequence).
 
         Parameters
         ----------
-        audio: vocalpy.Audio, vocalpy.AudioFile, a sequence of either, or a Dataset
+        sound: vocalpy.Sound, vocalpy.AudioFile, a sequence of either, or a Dataset
             Source of audio used to make spectrograms.
         dir_path : string, pathlib.Path
             The directory where the spectrogram files should be saved.
         namer : callable
             Function or class that determines spectrogram file name
             from audio file name. Default is
             :func:`vocalpy.domain_model.services.spectrogram_maker.default_spect_name_func`.
 
         Returns
         -------
         spectrogram_file : SpectrogramFile, list of SpectrogramFile
             The file(s) containing the spectrogram(s).
         """
-        validate_audio(audio)
+        validate_sound(sound)
         dir_path = pathlib.Path(dir_path)
         if not dir_path.exists() or not dir_path.is_dir():
             raise NotADirectoryError(f"`dir_path` not found or not recognized as a directory:\n{dir_path}")
 
         # define nested function so vars are in scope and ``dask`` can call it
-        def _to_spect_file(audio_):
-            """Compute a `Spectrogram` from an `Audio` instance,
+        def _to_spect_file(sound_):
+            """Compute a `Spectrogram` from an `Sound` instance,
             using self.callback"""
-            if isinstance(audio_, AudioFile):
-                audio_ = Audio.read(audio_.path)
-            spect = self.callback(audio_, **self.spect_params)
-            spect_fname = namer(audio_.path)
+            if isinstance(sound_, AudioFile):
+                sound_ = Sound.read(sound_.path)
+            spect = self.callback(sound_, **self.params)
+            spect_fname = namer(sound_.path)
             spect_path = dir_path / spect_fname
             spect_file = spect.write(spect_path)
             return spect_file
 
-        if isinstance(audio, (Audio, AudioFile)):
-            return _to_spect_file(audio)
+        if isinstance(sound, (Sound, AudioFile)):
+            return _to_spect_file(sound)
 
         spect_files = []
-        for audio_ in audio:
+        for sound_ in sound:
             if parallelize:
-                spect_files.append(dask.delayed(_to_spect_file(audio_)))
+                spect_files.append(dask.delayed(_to_spect_file(sound_)))
             else:
-                spect_files.append(_to_spect_file(audio_))
+                spect_files.append(_to_spect_file(sound_))
 
         if parallelize:
             graph = dask.delayed()(spect_files)
             with dask.diagnostics.ProgressBar():
                 return graph.compute()
         else:
             return spect_files
```

### Comparing `vocalpy-0.8.2/src/vocalpy/spectrogram_parameters.py` & `vocalpy-0.9.0/src/vocalpy/spectrogram_parameters.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/unit.py` & `vocalpy-0.9.0/src/vocalpy/unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import attrs
 
 from ._spectrogram.data_type import Spectrogram
-from .audio import Audio
+from .sound import Sound
 
 DEFAULT_LABEL = "-"
 
 
 @attrs.define
 class Unit:
     """A unit in a sequence,
@@ -16,29 +16,29 @@
     onset : float
         Onset time of unit, in seconds.
     offset : float
         Offset time of unit, in seconds.
     label : str
         A string label applied by an annotator to the unit.
         Default is determined by :data:`vocalpy.unit.DEFAULT_LABEL`.
-    audio : vocalpy.Audio, optional
+    sound : vocalpy.Sound, optional
         The audio for this unit.
         Optional, default is None.
     spectrogram : vocalpy.Spectrogram, optional
         The spectrogram for this unit.
         Optional, default is None.
     """
 
     onset = attrs.field(validator=attrs.validators.optional(attrs.validators.instance_of(float)))
     offset = attrs.field(validator=attrs.validators.optional(attrs.validators.instance_of(float)))
 
     label: str = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str)), default=DEFAULT_LABEL
     )
-    audio: Audio = attrs.field(validator=attrs.validators.optional(attrs.validators.instance_of(Audio)), default=None)
+    sound: Sound = attrs.field(validator=attrs.validators.optional(attrs.validators.instance_of(Sound)), default=None)
     spectrogram: Spectrogram = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(Spectrogram)), default=None
     )
 
     def __attrs_post_init__(self):
         if self.offset < self.onset:
             raise ValueError(
```

### Comparing `vocalpy-0.8.2/src/vocalpy/validators/attrs.py` & `vocalpy-0.9.0/src/vocalpy/validators/attrs.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/src/vocalpy/validators/validators.py` & `vocalpy-0.9.0/src/vocalpy/validators/validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-"""Validation functions.
-
-.. autosummary::
-   :toctree: generated
-"""
+"""Validation functions."""
 from __future__ import annotations
 
+from typing import TYPE_CHECKING
+
 import numpy as np
 import numpy.typing as npt
 
-__all__ = [
-    "have_same_dtype",
-    "is_1d_ndarray",
-    "is_valid_boundaries_array",
-]
+if TYPE_CHECKING:
+    from vocalpy import Segment, Sound
+
+
+__all__ = ["have_same_dtype", "is_1d_ndarray", "is_valid_boundaries_array", "is_sound_or_segment"]
 
 
 def is_1d_ndarray(y: npt.NDArray, name: str | None = None) -> bool:
     """Validates that ``y`` is a
     1-dimensional :class:`numpy.ndarray`.
 
     Parameters
@@ -142,7 +140,18 @@
             names = f"{name1} and {name2} "
         else:
             names = ""
 
         raise ValueError(f"Two arrays {names}must have the same dtype, but dtypes were: {arr1.dtype} and {arr2.dtype}")
 
     return True
+
+
+def is_sound_or_segment(source: Sound | Segment) -> bool:
+    from vocalpy import Segment, Sound
+
+    if not isinstance(source, (Sound, Segment)):
+        raise TypeError(
+            f"`source` must be an instance of either a `Sound` or a `Segment`, but type was: {type(source)}"
+        )
+
+    return True
```

### Comparing `vocalpy-0.8.2/tests/fixtures/annot.py` & `vocalpy-0.9.0/tests/fixtures/annot.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/tests/test_annotation_file.py` & `vocalpy-0.9.0/tests/test_annotation_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,16 @@
         for attr_name, attr_type, attr_val in zip(
             ("path", "annotates"), (pathlib.Path, vocalpy.AudioFile), (annot_path, audio_file)
         ):
             assert hasattr(annot_file, attr_name)
             assert isinstance(getattr(annot_file, attr_name), attr_type)
             assert getattr(annot_file, attr_name) == attr_val
 
-    def test_init_list_of_wav(self, annot_file_koumura, audio_list_wav):
-        audio_files = [vocalpy.AudioFile(path=wav_path) for wav_path in audio_list_wav]
+    def test_init_list_of_wav(self, annot_file_koumura, birdsongrec_wav_list):
+        audio_files = [vocalpy.AudioFile(path=wav_path) for wav_path in birdsongrec_wav_list]
         annot_file = vocalpy.AnnotationFile(path=annot_file_koumura, annotates=audio_files)
         assert isinstance(annot_file, vocalpy.AnnotationFile)
         for attr_name, attr_type, attr_val in zip(
             ("path", "annotates"), (pathlib.Path, list), (annot_file_koumura, audio_files)
         ):
             assert hasattr(annot_file, attr_name)
             assert isinstance(getattr(annot_file, attr_name), attr_type)
@@ -40,14 +40,14 @@
         for attr_name, attr_type, attr_val in zip(
             ("path", "annotates"), (pathlib.Path, list), (annot_file_yarden, spect_files)
         ):
             assert hasattr(annot_file, attr_name)
             assert isinstance(getattr(annot_file, attr_name), attr_type)
             assert getattr(annot_file, attr_name) == attr_val
 
-    def test_raises(self, annot_file_koumura, audio_list_wav, spect_list_mat):
-        audio_files = [vocalpy.AudioFile(path=wav_path) for wav_path in audio_list_wav]
+    def test_raises(self, annot_file_koumura, birdsongrec_wav_list, spect_list_mat):
+        audio_files = [vocalpy.AudioFile(path=wav_path) for wav_path in birdsongrec_wav_list]
         spect_files = [vocalpy.SpectrogramFile(path=mat_spect_path) for mat_spect_path in spect_list_mat]
         mixed_list = audio_files + spect_files
 
         with pytest.raises(TypeError):
             vocalpy.AnnotationFile(path=annot_file_koumura, annotates=mixed_list)
```

### Comparing `vocalpy-0.8.2/tests/test_audio.py` & `vocalpy-0.9.0/tests/test_sound.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,223 +1,233 @@
 import numpy as np
 import pytest
 import soundfile
 
 import vocalpy
 
+from .fixtures.audio import MULTICHANNEL_FLY_WAV, BIRDSONGREC_WAV_LIST
+
+
 RNG = np.random.default_rng()
 
+def assert_sound_is_instance_with_expected_attrs(
+        sound, data, samplerate, channels, audio_format
+):
+    """Assertions helper we use in TestSound methods"""
+    assert isinstance(sound, vocalpy.Sound)
+
+    for attr_name, attr_val in zip(("data", "samplerate", "channels"), (data, samplerate, channels)):
+        assert hasattr(sound, attr_name)
+        if attr_name == "data":
+            if audio_format == "cbin":
+                # add channel dim to data, needed for cbin audio
+                attr_val = (attr_val.astype(np.float64) / 32768.0)
+            if attr_val.ndim == 1:
+                attr_val = attr_val[np.newaxis, ...]
+            np.testing.assert_allclose(
+                getattr(sound, attr_name), attr_val
+            )
+        else:
+            assert getattr(sound, attr_name) == attr_val
 
-@pytest.mark.parametrize(
-    "data, expected_channels",
-    [
-        (RNG.normal(size=(int(32000 * 2.17))), 1),
-        (RNG.normal(size=(int(32000 * 2.17))), 1),
-        (RNG.normal(size=(int(32000 * 2.17), 1)), 1),
-        (RNG.normal(size=(int(32000 * 2.17), 1)), 1),
-        (RNG.normal(size=(int(32000 * 2.17), 2)), 2),
-        (RNG.normal(size=(int(32000 * 2.17), 2)), 2),
-        (RNG.normal(size=(int(48000 * 2.17), 2)), 2),
-        (RNG.normal(size=(int(48000 * 2.17), 2)), 2),
-        (RNG.normal(size=(int(48000 * 2.17), 6)), 6),
-        (RNG.normal(size=(int(48000 * 2.17), 6)), 6),
-    ],
-)
-def test_get_channels_from_data(data, expected_channels):
-    channels = vocalpy.audio.get_channels_from_data(data)
-    assert channels == expected_channels
+    assert sound.samples == sound.data.shape[1]
+    assert sound.duration == sound.data.shape[1] / sound.samplerate
 
 
-class TestAudio:
+class TestSound:
     @pytest.mark.parametrize(
         "data, samplerate, channels",
         [
             (RNG.normal(size=(int(32000 * 2.17))), 32000, 1),
-            (RNG.normal(size=(int(32000 * 2.17), 1)), 32000, 1),
-            (RNG.normal(size=(int(32000 * 2.17), 2)), 32000, 2),
-            (RNG.normal(size=(int(48000 * 2.17), 2)), 48000, 2),
-            (RNG.normal(size=(int(48000 * 2.17), 6)), 48000, 6),
+            (RNG.normal(size=(1, int(32000 * 2.17))), 32000, 1),
+            (RNG.normal(size=(2, int(32000 * 2.17))), 32000, 2),
+            (RNG.normal(size=(2, int(48000 * 2.17))), 48000, 2),
+            (RNG.normal(size=(6, int(48000 * 2.17))), 48000, 6),
         ],
     )
     def test_init(self, data, samplerate, channels):
-        """Test that we can initialize a :class:`vocalpy.Audio` instance."""
-        audio = vocalpy.Audio(data=data, samplerate=samplerate)
+        """Test that we can initialize a :class:`vocalpy.Sound` instance."""
+        sound = vocalpy.Sound(data=data, samplerate=samplerate)
 
-        assert isinstance(audio, vocalpy.Audio)
-
-        for attr_name, attr_val in zip(("data", "samplerate", "channels"), (data, samplerate, channels)):
-            assert hasattr(audio, attr_name)
-            assert getattr(audio, attr_name) is attr_val
+        assert_sound_is_instance_with_expected_attrs(
+            sound, data, samplerate, channels, audio_format="wav"
+        )
 
     @pytest.mark.parametrize(
         "data, samplerate, expected_exception",
         [
             # `data` is not a numpy array
             (RNG.normal(size=(int(32000 * 2.17))).tolist(), 32000, TypeError),
             # `data` is zero dimensional
             (np.array(2), 32000, ValueError),
             # `data` has more than 2 dimensions
             (RNG.normal(size=(int(32000 * 2.17)))[:, np.newaxis, np.newaxis], 32000, ValueError),
             # `samplerate` is not an int
             # this raises a ValueError because the converter can't cast the string to an int
-            (RNG.normal(size=(int(32000 * 2.17), 1)), "f", ValueError),
+            (RNG.normal(size=(1, int(32000 * 2.17))), "f", TypeError),
             # `samplerate` is less than zero
-            (RNG.normal(size=(int(32000 * 2.17), 1)), -32000, ValueError),
+            (RNG.normal(size=(1, int(32000 * 2.17))), -32000, ValueError),
         ],
     )
     def test_init_raises(self, data, samplerate, expected_exception):
-        """Test that :class:`vocalpy.Audio` raises expected errors"""
+        """Test that :class:`vocalpy.Sound` raises expected errors"""
         with pytest.raises(expected_exception):
-            vocalpy.Audio(data=data, samplerate=samplerate)
+            vocalpy.Sound(data=data, samplerate=samplerate)
 
-    @pytest.mark.parametrize(
-        "data, samplerate, channels",
-        [
-            (RNG.normal(size=(int(32000 * 2.17))), 32000, 1),
-            (RNG.normal(size=(int(32000 * 2.17), 1)), 32000, 1),
-            (RNG.normal(size=(int(32000 * 2.17), 2)), 32000, 2),
-            (RNG.normal(size=(int(48000 * 2.17), 2)), 48000, 2),
-            (RNG.normal(size=(int(48000 * 2.17), 6)), 48000, 6),
-        ],
-    )
-    def test_asdict(self, data, samplerate, channels):
-        audio = vocalpy.Audio(data=data, samplerate=samplerate)
-        assert isinstance(audio, vocalpy.Audio)
-
-        asdict = audio.asdict()
-        assert isinstance(asdict, dict)
-
-        for attr_name, attr_val in zip(("data", "samplerate", "channels"), (data, samplerate, channels)):
-            assert attr_name in asdict
-            assert asdict[attr_name] is attr_val
+    def test_init_warns(self):
+        """Test that we get a warning if number channels > number of samples"""
+        with pytest.warns():
+            vocalpy.Sound(data=RNG.normal(size=(int(32000 * 2.17), 1)), samplerate=32000)
 
     @pytest.mark.parametrize(
         "data, samplerate",
         [
             (RNG.normal(size=(int(32000 * 2.17))), 32000),
-            (RNG.normal(size=(int(32000 * 2.17), 1)), 32000),
-            (RNG.normal(size=(int(32000 * 2.17), 2)), 32000),
-            (RNG.normal(size=(int(48000 * 2.17), 2)), 48000),
-            (RNG.normal(size=(int(48000 * 2.17), 6)), 48000),
+            (RNG.normal(size=(1, int(32000 * 2.17))), 32000),
+            (RNG.normal(size=(2, int(32000 * 2.17))), 32000),
+            (RNG.normal(size=(2, int(48000 * 2.17))), 48000),
+            (RNG.normal(size=(6, int(48000 * 2.17))), 48000),
         ],
     )
     def test___eq__(self, data, samplerate):
-        audio = vocalpy.Audio(data=data, samplerate=samplerate)
-        other = vocalpy.Audio(data=data.copy(), samplerate=samplerate)
-        assert audio == other
+        sound = vocalpy.Sound(data=data, samplerate=samplerate)
+        other = vocalpy.Sound(data=data.copy(), samplerate=samplerate)
+        assert sound == other
 
     @pytest.mark.parametrize(
         "data, samplerate",
         [
             (RNG.normal(size=(int(32000 * 2.17))), 32000),
-            (RNG.normal(size=(int(32000 * 2.17), 1)), 32000),
-            (RNG.normal(size=(int(32000 * 2.17), 2)), 32000),
-            (RNG.normal(size=(int(48000 * 2.17), 2)), 48000),
-            (RNG.normal(size=(int(48000 * 2.17), 6)), 48000),
+            (RNG.normal(size=(1, int(32000 * 2.17))), 32000),
+            (RNG.normal(size=(2, int(32000 * 2.17))), 32000),
+            (RNG.normal(size=(2, int(48000 * 2.17))), 48000),
+            (RNG.normal(size=(6, int(48000 * 2.17))), 48000),
         ],
     )
     def test___ne__(self, data, samplerate):
-        audio = vocalpy.Audio(data=data, samplerate=samplerate)
-        other = vocalpy.Audio(data=data.copy() + 0.001, samplerate=samplerate)
-        assert audio != other
-
-    def test_read(self, a_wav_path, tmp_path):
-        """Test that :meth:`vocalpy.Audio.read` works as expected.
-
-        To do this we make an audio file "by hand".
-        """
-        data, samplerate = soundfile.read(a_wav_path)
-        if data.ndim == 1:
+        sound = vocalpy.Sound(data=data, samplerate=samplerate)
+        other = vocalpy.Sound(data=data.copy() + 0.001, samplerate=samplerate)
+        assert sound != other
+
+    @staticmethod
+    def load_an_audio_path(an_audio_path):
+        if an_audio_path.name.endswith("cbin"):
+            data, samplerate = vocalpy._vendor.evfuncs.load_cbin(an_audio_path)
             channels = 1
-        else:
+            audio_format = "cbin"
+        elif an_audio_path.name.endswith("wav"):
+            data, samplerate = soundfile.read(an_audio_path, always_2d=True)
             channels = data.shape[1]
-
-        # to make sure round-tripping works as we'd expect,
-        # we first write what we read with soundfile to a temporary file
-        # then use `vocalpy.Audio` to read that temporary file
-        # and test that it matches what we read directly from the original file
-        tmp_wav_path = tmp_path / a_wav_path.name
-        soundfile.write(tmp_wav_path, data, samplerate)
-
-        audio = vocalpy.Audio.read(tmp_wav_path)
-        assert isinstance(audio, vocalpy.Audio)
-        for attr_name, attr_val in zip(("data", "samplerate", "channels"), (data, samplerate, channels)):
-            assert hasattr(audio, attr_name)
-            if isinstance(attr_val, np.ndarray):
-                np.testing.assert_allclose(getattr(audio, attr_name), attr_val)
-            else:
-                assert getattr(audio, attr_name) == attr_val
-
-    def test_write(self, a_wav_path, tmp_path):
-        """Test that :meth:`vocalpy.Audio.write` works as expected.
-
-        To do this we make a spectrogram file "by hand".
-        """
-        data, samplerate = soundfile.read(a_wav_path)
-        if data.ndim == 1:
-            channels = 1
+            data = np.transpose(data, (1, 0))
+            audio_format = "wav"
         else:
-            channels = data.shape[1]
+            raise ValueError(
+                f"Unrecognized format: {an_audio_path.suffix}"
+            )
+        return data, samplerate, channels, audio_format
+
+    def test_read(self, an_audio_path):
+        """Test that :meth:`vocalpy.Sound.read` works as expected."""
+        data, samplerate, channels, audio_format = self.load_an_audio_path(an_audio_path)
+
+        sound = vocalpy.Sound.read(an_audio_path)
+        assert_sound_is_instance_with_expected_attrs(
+            sound, data, samplerate, channels, audio_format
+        )
+
+    def test_write(self, an_audio_path, tmp_path):
+        """Test that :meth:`vocalpy.Sound.write` works as expected.
+
+        To do this we instantiate a Sound instance directly,
+        write it to a file, read it, and then test that the loaded
+        data is what we expect.
+        """
+        data, samplerate, channels, audio_format = self.load_an_audio_path(an_audio_path)
 
-        # to make sure round-tripping works as we'd expect,
-        # we first write what we read with soundfile to a temporary file
-        # then use `vocalpy.Audio` to read that temporary file
-        # and test that it matches what we read directly from the original file
-        audio = vocalpy.Audio(data=data, samplerate=samplerate)
-        tmp_wav_path = tmp_path / a_wav_path.name
+        if audio_format == "cbin":
+            # we have to normalize cbin
+            # https://stackoverflow.com/a/42544738/4906855
+            data_float_normal = data.astype(np.float64) / 32768.0
+            sound = vocalpy.Sound(data=data_float_normal, samplerate=samplerate)
+        else:
+            sound = vocalpy.Sound(data=data, samplerate=samplerate)
+        tmp_wav_path = tmp_path / (an_audio_path.stem + ".wav")
         assert not tmp_wav_path.exists()
 
-        audio.write(tmp_wav_path)
+        sound.write(tmp_wav_path)
 
         assert tmp_wav_path.exists()
 
-        audio_loaded = vocalpy.Audio.read(tmp_wav_path)
-        assert isinstance(audio_loaded, vocalpy.Audio)
-        for attr_name, attr_val in zip(("data", "samplerate", "channels"), (data, samplerate, channels)):
-            assert hasattr(audio_loaded, attr_name)
-            if isinstance(attr_val, np.ndarray):
-                np.testing.assert_allclose(getattr(audio_loaded, attr_name), attr_val)
-            else:
-                assert getattr(audio_loaded, attr_name) == attr_val
+        sound_loaded = vocalpy.Sound.read(tmp_wav_path)
 
-    def test_lazy(self, a_wav_path):
-        """Test that :meth:`vocalpy.Audio.read` works as expected.
+        assert_sound_is_instance_with_expected_attrs(
+            sound_loaded, data, samplerate, channels, audio_format
+        )
+
+    def test_write_raises(self, a_cbin_path, tmp_path):
+        sound = vocalpy.Sound.read(a_cbin_path)
+        tmp_cbin_path = tmp_path / a_cbin_path.name
+        with pytest.raises(ValueError):
+            sound.write(tmp_cbin_path)
 
-        To do this we make an audio file "by hand".
-        """
-        data, samplerate = soundfile.read(a_wav_path)
-        if data.ndim == 1:
-            channels = 1
-        else:
-            channels = data.shape[1]
+    @pytest.mark.parametrize(
+        'a_wav_path',
+        [
+            # audio with one channel
+            BIRDSONGREC_WAV_LIST[0],
+            # audio with more than one channel
+            MULTICHANNEL_FLY_WAV,
+        ]
+    )
+    def test___iter__(self, a_wav_path):
+        sound = vocalpy.Sound.read(a_wav_path)
+        sound_channels = [
+            sound_ for sound_ in sound
+        ]
+        assert all(
+            [isinstance(sound_, vocalpy.Sound)
+             for sound_ in sound_channels]
+        )
+        for channel, sound_channel in enumerate(sound_channels):
+            np.testing.assert_allclose(
+                sound_channel.data, sound.data[channel][np.newaxis, ...]
+            )
+        assert len(sound_channels) == sound.data.shape[0]
 
-        audio = vocalpy.Audio(path=a_wav_path)
-        assert audio._data is None
-        assert audio._samplerate is None
-        assert audio._channels is None
-
-        _ = audio.data  # triggers lazy-load
-        assert np.array_equal(audio._data, data)
-        assert audio._samplerate == samplerate
-        assert audio._channels == channels
-
-    def test_open(self, a_wav_path):
-        data, samplerate = soundfile.read(a_wav_path)
-        if data.ndim == 1:
-            channels = 1
-        else:
-            channels = data.shape[1]
+    @pytest.mark.parametrize(
+        'a_wav_path, key',
+        [
+            # audio with one channel
+            (BIRDSONGREC_WAV_LIST[0], 0),
+            # audio with more than one channel
+            (MULTICHANNEL_FLY_WAV, slice(None, 2)),
+        ]
+    )
+    def test___getitem__(self, a_wav_path, key):
+        sound = vocalpy.Sound.read(a_wav_path)
+        sound_channel = sound[key]
+        assert isinstance(sound_channel, vocalpy.Sound)
+        if isinstance(key, int):
+            assert sound_channel.data.shape[0] == 1
+            np.testing.assert_allclose(
+                sound_channel.data, sound.data[key][np.newaxis, ...]
+            )
+        elif isinstance(key, slice):
+            sliced = sound.data[key]
+            assert sound_channel.data.shape[0] == sliced.shape[0]
+            np.testing.assert_allclose(
+                sound_channel.data, sliced
+            )
 
-        audio = vocalpy.Audio(path=a_wav_path)
-        assert audio._data is None
-        assert audio._samplerate is None
-        assert audio._channels is None
-
-        with audio.open():
-            assert np.array_equal(audio._data, data)
-            assert audio._samplerate == samplerate
-            assert audio._channels == channels
-
-        # check that attributes go back to none after we __exit__ the context
-        assert audio._data is None
-        assert audio._samplerate is None
-        assert audio._channels is None
+    @pytest.mark.parametrize(
+        'a_wav_path, key',
+        [
+            # audio with one channel
+            (BIRDSONGREC_WAV_LIST[0], 1),
+            # audio with more than one channel
+            (MULTICHANNEL_FLY_WAV, 5),
+        ]
+    )
+    def test___getitem__raises(self, a_wav_path, key):
+        sound = vocalpy.Sound.read(a_wav_path)
+        with pytest.raises(IndexError):
+            _ = sound[key]
```

### Comparing `vocalpy-0.8.2/tests/test_audio_file.py` & `vocalpy-0.9.0/tests/test_audio_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/tests/test_metrics/test_segmentation/test_ir.py` & `vocalpy-0.9.0/tests/test_metrics/test_segmentation/test_ir.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/tests/test_spectrogram_file.py` & `vocalpy-0.9.0/tests/test_spectrogram_file.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/tests/test_spectrogram_maker.py` & `vocalpy-0.9.0/tests/test_spectrogram_maker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,122 +1,126 @@
+import inspect
+
 import pytest
 
 import vocalpy
 
-from .fixtures.audio import AUDIO_LIST_WAV
+from .fixtures.audio import BIRDSONGREC_WAV_LIST
 from .fixtures.spect import SPECT_LIST_NPZ
 
 
 @pytest.mark.parametrize(
-    "audio_format",
-    [
-        "wav",
-        "cbin",
-    ],
+    'a_wav_path',
+    BIRDSONGREC_WAV_LIST[:3]
 )
-def test_default_spect_fname_func(specific_audio_dir, audio_format):
-    audio_dir = specific_audio_dir(audio_format)
-    audio_paths = sorted(audio_dir.glob(f"*{audio_format}"))
-
-    for audio_path in audio_paths:
-        spect_fname = vocalpy.spectrogram_maker.default_spect_fname_func(audio_path)
-        assert spect_fname == audio_path.name + vocalpy.constants.SPECT_FILE_EXT
+def test_default_spect_fname_func(a_wav_path):
+    spect_fname = vocalpy.spectrogram_maker.default_spect_fname_func(a_wav_path)
+    assert spect_fname == a_wav_path.name + vocalpy.constants.SPECT_FILE_EXT
 
 
 @pytest.mark.parametrize(
-    "audio",
+    "sound",
     [
-        vocalpy.Audio.read(AUDIO_LIST_WAV[0]),
-        vocalpy.AudioFile(path=AUDIO_LIST_WAV[0]),
-        [vocalpy.Audio.read(path) for path in AUDIO_LIST_WAV[:3]],
-        [vocalpy.AudioFile(path=path) for path in AUDIO_LIST_WAV[:3]],
+        vocalpy.Sound.read(BIRDSONGREC_WAV_LIST[0]),
+        vocalpy.AudioFile(path=BIRDSONGREC_WAV_LIST[0]),
+        [vocalpy.Sound.read(path) for path in BIRDSONGREC_WAV_LIST[:3]],
+        [vocalpy.AudioFile(path=path) for path in BIRDSONGREC_WAV_LIST[:3]],
     ],
 )
-def test_validate_audio(audio):
-    assert vocalpy.spectrogram_maker.validate_audio(audio) is None
+def test_validate_sound(sound):
+    assert vocalpy.spectrogram_maker.validate_sound(sound) is None
 
 
 @pytest.mark.parametrize(
     "not_audio, expected_exception",
     [
         (vocalpy.Spectrogram.read(SPECT_LIST_NPZ[0]), TypeError),
         (dict(), TypeError),
         ([vocalpy.Spectrogram.read(path) for path in SPECT_LIST_NPZ[:3]], TypeError),
         (
-            [vocalpy.Audio.read(path) for path in AUDIO_LIST_WAV[:3]]
-            + [vocalpy.AudioFile(path=path) for path in AUDIO_LIST_WAV[:3]],
+            [vocalpy.Sound.read(path) for path in BIRDSONGREC_WAV_LIST[:3]]
+            + [vocalpy.AudioFile(path=path) for path in BIRDSONGREC_WAV_LIST[:3]],
             TypeError,
         ),
     ],
 )
-def test_validate_audio_not_audio_raises(not_audio, expected_exception):
+def test_validate_sound_not_audio_raises(not_audio, expected_exception):
     with pytest.raises(expected_exception=expected_exception):
-        vocalpy.spectrogram_maker.validate_audio(not_audio)
+        vocalpy.spectrogram_maker.validate_sound(not_audio)
 
 
 class TestSpectrogramMaker:
     @pytest.mark.parametrize(
-        "callback, spect_params",
+        "callback, params, expected_callback, expected_params",
         [
-            (None, None),
+            (None,
+             None,
+             vocalpy.spectrogram,
+             vocalpy.spectrogram_maker.DEFAULT_SPECT_PARAMS
+             ),
+            (vocalpy.spectrogram,
+             None,
+             vocalpy.spectrogram,
+             {name: param.default
+              for name, param in inspect.signature(vocalpy.spectrogram).parameters.items()
+              if param.default is not inspect._empty}
+             )
         ],
     )
-    def test_init(self, callback, spect_params):
-        spect_maker = vocalpy.SpectrogramMaker(callback=callback, spect_params=spect_params)
+    def test_init(self, callback, params, expected_callback, expected_params):
+        spect_maker = vocalpy.SpectrogramMaker(callback=callback, params=params)
         assert isinstance(spect_maker, vocalpy.SpectrogramMaker)
-        if callback is None and spect_params is None:
-            assert spect_maker.callback is vocalpy.spectrogram
-            assert spect_maker.spect_params == vocalpy.spectrogram_maker.DEFAULT_SPECT_PARAMS
-        else:
-            assert spect_maker.callback is callback
-            assert spect_maker.spect_params == spect_params
+        assert spect_maker.callback is expected_callback
+        assert spect_maker.params == expected_params
 
     @pytest.mark.parametrize(
-        "audio",
+        "sound",
         [
-            vocalpy.Audio.read(AUDIO_LIST_WAV[0]),
-            vocalpy.AudioFile(path=AUDIO_LIST_WAV[0]),
-            [vocalpy.Audio.read(path) for path in AUDIO_LIST_WAV[:3]],
-            [vocalpy.AudioFile(path=path) for path in AUDIO_LIST_WAV[:3]],
+            vocalpy.Sound.read(BIRDSONGREC_WAV_LIST[0]),
+            vocalpy.AudioFile(path=BIRDSONGREC_WAV_LIST[0]),
+            [vocalpy.Sound.read(path) for path in BIRDSONGREC_WAV_LIST[:3]],
+            [vocalpy.AudioFile(path=path) for path in BIRDSONGREC_WAV_LIST[:3]],
         ],
     )
-    def test_make(self, audio):
+    def test_make(self, sound, parallel):
         spect_maker = vocalpy.SpectrogramMaker()
-        out = spect_maker.make(audio)
-        if isinstance(audio, (vocalpy.Audio, vocalpy.AudioFile)):
+
+        out = spect_maker.make(sound, parallelize=parallel)
+
+        if isinstance(sound, (vocalpy.Sound, vocalpy.AudioFile)):
             assert isinstance(out, vocalpy.Spectrogram)
-        elif isinstance(audio, list):
+        elif isinstance(sound, list):
             assert all([isinstance(spect, vocalpy.Spectrogram) for spect in out])
 
     @pytest.mark.parametrize(
-        "audio",
+        "sound",
         [
-            vocalpy.Audio.read(AUDIO_LIST_WAV[0]),
-            vocalpy.AudioFile(path=AUDIO_LIST_WAV[0]),
-            [vocalpy.Audio.read(path) for path in AUDIO_LIST_WAV[:3]],
-            [vocalpy.AudioFile(path=path) for path in AUDIO_LIST_WAV[:3]],
+            vocalpy.Sound.read(BIRDSONGREC_WAV_LIST[0]),
+            vocalpy.AudioFile(path=BIRDSONGREC_WAV_LIST[0]),
+            [vocalpy.Sound.read(path) for path in BIRDSONGREC_WAV_LIST[:3]],
+            [vocalpy.AudioFile(path=path) for path in BIRDSONGREC_WAV_LIST[:3]],
         ],
     )
-    def test_write(self, audio, tmp_path):
+    def test_write(self, sound, tmp_path):
         spect_maker = vocalpy.SpectrogramMaker()
 
-        out = spect_maker.write(audio, dir_path=tmp_path)
+        out = spect_maker.write(sound, dir_path=tmp_path)
 
-        if isinstance(audio, (vocalpy.Audio, vocalpy.AudioFile)):
+        if isinstance(sound, (vocalpy.Sound, vocalpy.AudioFile)):
             assert isinstance(out, vocalpy.SpectrogramFile)
             path = out.path
             assert path.exists()
-            if isinstance(audio, vocalpy.Audio):
-                assert out.source_audio_file.path == audio.path
-            elif isinstance(audio, vocalpy.AudioFile):
-                assert out.source_audio_file.path == audio.path
+            if isinstance(sound, vocalpy.Sound):
+                assert out.source_audio_file.path == sound.path
+            elif isinstance(sound, vocalpy.AudioFile):
+                assert out.source_audio_file.path == sound.path
 
-        elif isinstance(audio, list):
+        elif isinstance(sound, list):
             assert isinstance(out, list)
             assert all([isinstance(spect_file, vocalpy.SpectrogramFile) for spect_file in out])
             for spect_file in out:
                 path = spect_file.path
                 assert path.exists()
-                if isinstance(audio, vocalpy.Audio):
-                    assert spect_file.source_audio_file.path == audio.path
-                elif isinstance(audio, vocalpy.AudioFile):
-                    assert spect_file.source_audio_file.path == audio.path
+                if isinstance(sound, vocalpy.Sound):
+                    assert spect_file.source_audio_file.path == sound.path
+                elif isinstance(sound, vocalpy.AudioFile):
+                    assert spect_file.source_audio_file.path == sound.path
```

### Comparing `vocalpy-0.8.2/tests/test_unit.py` & `vocalpy-0.9.0/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/tests/test_validators/test_validators.py` & `vocalpy-0.9.0/tests/test_validators/test_validators.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/tests/test_vendor/test_evfuncs.py` & `vocalpy-0.9.0/tests/test_vendor/test_evfuncs.py`

 * *Files identical despite different names*

### Comparing `vocalpy-0.8.2/PKG-INFO` & `vocalpy-0.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 Metadata-Version: 2.1
 Name: vocalpy
-Version: 0.8.2
+Version: 0.9.0
 Summary: A core package for acoustic communication research in Python
 Author-email: David Nicholson <nickledave@users.noreply.github.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: attrs >=23.1.0
 Requires-Dist: crowsetta >=5.0.2
-Requires-Dist: dask >=2.10.1
+Requires-Dist: dask[dataframe] >=2.10.1
+Requires-Dist: h5netcdf >= 1.3.0
 Requires-Dist: librosa >= 0.10.0.post2
 Requires-Dist: matplotlib >=3.7.1
 Requires-Dist: numpy >=1.22.0
 Requires-Dist: pandas >= 1.4.0
+Requires-Dist: pooch >= 1.8.1
 Requires-Dist: scipy >=1.8.0
 Requires-Dist: SoundFile >=0.12.1
-Requires-Dist: SQLAlchemy >=2.0.12
 Requires-Dist: xarray >= 2023.11.0
 Requires-Dist: twine >=3.7.1 ; extra == "dev"
 Requires-Dist: black >=21.12b0 ; extra == "dev"
 Requires-Dist: ipython >=8.0.0 ; extra == "dev"
 Requires-Dist: nox >= 2022.1.7 ; extra == "dev"
 Requires-Dist: vocalpy[doc, test] ; extra == "dev"
 Requires-Dist: ipython != 8.7.0 ; extra == "doc"
 Requires-Dist: jupyterlab >=3.0.3 ; extra == "doc"
 Requires-Dist: jupytext >=1.13.8 ; extra == "doc"
 Requires-Dist: myst-nb >=0.15.0 ; extra == "doc"
+Requires-Dist: numpydoc >=1.6.0 ; extra == "doc"
+Requires-Dist: seaborn >=0.13.2 ; extra == "doc"
 Requires-Dist: Sphinx >=3.4.3 ; extra == "doc"
 Requires-Dist: sphinx-autobuild >= 2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-book-theme >=0.3.2 ; extra == "doc"
 Requires-Dist: sphinx-copybutton >=0.4.0 ; extra == "doc"
 Requires-Dist: sphinx-design >=0.2.0 ; extra == "doc"
 Requires-Dist: sphinxext-opengraph  >=0.5.1 ; extra == "doc"
 Requires-Dist: sphinx-tabs >= 3.3.1 ; extra == "doc"
@@ -104,28 +107,29 @@
 
 [^1]: For a curated collection, see <https://github.com/rhine3/bioacoustics-software>.
 
 ## Features
 
 ###  Data types for acoustic communication data: audio, spectrogram, annotations, features
 
-#### The `vocalpy.Audio` data type
+#### The `vocalpy.Sound` data type
 
 - Works with a wide array of audio formats, thanks to [soundfile](https://github.com/bastibe/python-soundfile).
 - Also works with the cbin audio format saved by the LabView app EvTAF used by many neuroscience labs studying birdsong,
   thanks to [evfuncs](https://github.com/NickleDave/evfuncs).
 
 ```python
->>> import vocalpy as voc
->>> data_dir = ('tests/data-for-tests/source/audio_wav_annot_birdsongrec/Bird0/Wave/')
->>> wav_paths = voc.paths.from_dir(data_dir, 'wav')
->>> audios = [voc.Audio.read(wav_path) for wav_path in wav_paths]
->>> print(audios[0])
-vocalpy.Audio(data=array([3.0517...66210938e-04]), samplerate=32000, channels=1), 
-path=tests/data-for-tests/source/audio_wav_annot_birdsongrec/Bird0/Wave/0.wav)
+>> > import vocalpy as voc
+>> > data_dir = ('tests/data-for-tests/source/audio_wav_annot_birdsongrec/Bird0/Wave/')
+>> > wav_paths = voc.paths.from_dir(data_dir, 'wav')
+>> > audios = [voc.Sound.read(wav_path) for wav_path in wav_paths]
+>> > print(audios[0])
+vocalpy.Sound(data=array([3.0517...66210938e-04]), samplerate=32000, channels=1),
+path = tests / data -
+for -tests / source / audio_wav_annot_birdsongrec / Bird0 / Wave / 0.wav)
 ```
 
 #### The `vocalpy.Spectrogram` data type
 
 - Save expensive-to-compute spectrograms to array files, so you don't regenerate them over and over again
 
 ```python
@@ -154,49 +158,60 @@
 ```
 
 ### Classes for common steps in your pipelines and workflows
 
 #### A `Segmenter` for segmentation into sequences of units
 
 ```python
->>> import evfuncs
->>> import vocalpy as voc
->>> data_dir = ('tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/')
->>> cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
->>> audios = [voc.Audio.read(cbin_path) for cbin_path in cbin_paths]
->>> segment_params = {'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006}
->>> segmenter = voc.Segmenter(callback=evfuncs.segment_song, segment_params=segment_params)
->>> seqs = segmenter.segment(audios, parallelize=True)
-[########################################] | 100% Completed | 122.91 ms
->>> print(seqs[1])
-Sequence(units=[Unit(onset=2.19075, offset=2.20428125, label='-', audio=None, spectrogram=None), 
-Unit(onset=2.35478125, offset=2.38815625, label='-', audio=None, spectrogram=None), Unit(onset=2.8410625, offset=2.86715625, label='-', audio=None, spectrogram=None), 
-Unit(onset=3.48234375, offset=3.49371875, label='-', audio=None, spectrogram=None), Unit(onset=3.57021875, offset=3.60296875, label='-', audio=None, spectrogram=None), 
-Unit(onset=3.64403125, offset=3.67721875, label='-', audio=None, spectrogram=None), Unit(onset=3.72228125, offset=3.74478125, label='-', audio=None, spectrogram=None), 
-Unit(onset=3.8036875, offset=3.8158125, label='-', audio=None, spectrogram=None), Unit(onset=3.82328125, offset=3.83646875, label='-', audio=None, spectrogram=None), 
-Unit(onset=4.13759375, offset=4.16346875, label='-', audio=None, spectrogram=None), Unit(onset=4.80278125, offset=4.814, label='-', audio=None, spectrogram=None), 
-Unit(onset=4.908125, offset=4.922875, label='-', audio=None, spectrogram=None), Unit(onset=4.9643125, offset=4.992625, label='-', audio=None, spectrogram=None), 
-Unit(onset=5.039625, offset=5.0506875, label='-', audio=None, spectrogram=None), Unit(onset=5.10165625, offset=5.1385, label='-', audio=None, spectrogram=None), 
-Unit(onset=5.146875, offset=5.16203125, label='-', audio=None, spectrogram=None), Unit(onset=5.46390625, offset=5.49409375, label='-', audio=None, spectrogram=None), 
-Unit(onset=6.14503125, offset=6.1565625, label='-', audio=None, spectrogram=None), Unit(onset=6.31003125, offset=6.346125, label='-', audio=None, spectrogram=None), 
-Unit(onset=6.38996875, offset=6.4018125, label='-', audio=None, spectrogram=None), Unit(onset=6.46053125, offset=6.4796875, label='-', audio=None, spectrogram=None), 
-Unit(onset=6.83525, offset=6.8643125, label='-', audio=None, spectrogram=None)], method='segment_song', 
-segment_params={'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006}, 
-audio=vocalpy.Audio(data=None, samplerate=None, channels=None), path=tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/gy6or6_baseline_230312_0809.141.cbin), spectrogram=None)
+>> > import evfuncs
+>> > import vocalpy as voc
+>> > data_dir = ('tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/')
+>> > cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
+>> > audios = [voc.Sound.read(cbin_path) for cbin_path in cbin_paths]
+>> > segment_params = {'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006}
+>> > segmenter = voc.Segmenter(callback=evfuncs.segment_song, segment_params=segment_params)
+>> > seqs = segmenter.segment(audios, parallelize=True)
+[  ########################################] | 100% Completed | 122.91 ms
+>> > print(seqs[1])
+Sequence(units=[Unit(onset=2.19075, offset=2.20428125, label='-', audio=None, spectrogram=None),
+                Unit(onset=2.35478125, offset=2.38815625, label='-', audio=None, spectrogram=None),
+                Unit(onset=2.8410625, offset=2.86715625, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.48234375, offset=3.49371875, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.57021875, offset=3.60296875, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.64403125, offset=3.67721875, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.72228125, offset=3.74478125, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.8036875, offset=3.8158125, label='-', audio=None, spectrogram=None),
+                Unit(onset=3.82328125, offset=3.83646875, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.13759375, offset=4.16346875, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.80278125, offset=4.814, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.908125, offset=4.922875, label='-', audio=None, spectrogram=None),
+                Unit(onset=4.9643125, offset=4.992625, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.039625, offset=5.0506875, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.10165625, offset=5.1385, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.146875, offset=5.16203125, label='-', audio=None, spectrogram=None),
+                Unit(onset=5.46390625, offset=5.49409375, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.14503125, offset=6.1565625, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.31003125, offset=6.346125, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.38996875, offset=6.4018125, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.46053125, offset=6.4796875, label='-', audio=None, spectrogram=None),
+                Unit(onset=6.83525, offset=6.8643125, label='-', audio=None, spectrogram=None)], method='segment_song',
+         segment_params={'threshold': 1500, 'min_syl_dur': 0.01, 'min_silent_dur': 0.006},
+         audio=vocalpy.Sound(data=None, samplerate=None, channels=None), path=tests / data -
+for -tests / source / audio_cbin_annot_notmat / gy6or6 / 032312 / gy6or6_baseline_230312_0809.141.cbin), spectrogram=None)
 ```
  
 #### A `SpectrogramMaker` for computing spectrograms
 
 ```python
->>> import vocalpy as voc
->>> wav_paths = voc.paths.from_dir('wav')
->>> audios = [voc.Audio(wav_path) for wav_path in wav_paths]
->>> spect_params = {'fft_size': 512, 'step_size': 64}
->>> spect_maker = voc.SpectrogramMaker(spect_params=spect_params)
->>> spects = spect_maker.make(audios, parallelize=True)
+>> > import vocalpy as voc
+>> > wav_paths = voc.paths.from_dir('wav')
+>> > audios = [voc.Sound(wav_path) for wav_path in wav_paths]
+>> > spect_params = {'fft_size': 512, 'step_size': 64}
+>> > spect_maker = voc.SpectrogramMaker(spect_params=spect_params)
+>> > spects = spect_maker.make(audios, parallelize=True)
 ```
 
 ### `Dataset`s you flexibly build from pipelines and convert to databases
 
 - The `vocalpy.dataset` module contains classes that represent common types of datasets 
 - You make these classes with outputs of your pipelines, e.g. a `list` of `vocalpy.Sequence`s 
   or `vocalpy.Spectrogram`s
@@ -210,39 +225,43 @@
     [recommended by the US Library of Congress for archival data](https://www.sqlite.org/locrsf.html),
     and it's [built into Python](https://docs.python.org/3/library/sqlite3.html) 
     -- no need to install separate database software like MySQL
 
 #### A `SequenceDataset` for common analyses of sequences of units
 
 ```python
->>> import evfuncs
->>> import vocalpy as voc
->>> data_dir = 'tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/'
->>> cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
->>> audios = [voc.Audio.read(cbin_path) for cbin_path in cbin_paths]
->>> segment_params = {
-    'threshold': 1500,
-    'min_syl_dur': 0.01,
-    'min_silent_dur': 0.006,
+>> > import evfuncs
+>> > import vocalpy as voc
+>> > data_dir = 'tests/data-for-tests/source/audio_cbin_annot_notmat/gy6or6/032312/'
+>> > cbin_paths = voc.paths.from_dir(data_dir, 'cbin')
+>> > audios = [voc.Sound.read(cbin_path) for cbin_path in cbin_paths]
+>> > segment_params = {
+  'threshold': 1500,
+  'min_syl_dur': 0.01,
+  'min_silent_dur': 0.006,
 }
->>> segmenter = voc.Segmenter(
-    callback=evfuncs.segment_song, 
-    segment_params=segment_params
+>> > segmenter = voc.Segmenter(
+  callback=evfuncs.segment_song,
+  segment_params=segment_params
 )
->>> seqs = segmenter.segment(audios)
->>> seq_dataset = voc.dataset.SequenceDataset(sequences=seqs)
->>> seq_dataset.to_sqlite(db_name='gy6or6-032312.db', replace=True)
->>> print(seq_dataset)
+>> > seqs = segmenter.segment(audios)
+>> > seq_dataset = voc.dataset.SequenceDataset(sequences=seqs)
+>> > seq_dataset.to_sqlite(db_name='gy6or6-032312.db', replace=True)
+>> > print(seq_dataset)
 SequenceDataset(sequences=[Sequence(units=[Unit(onset=2.18934375, offset=2.21, label='-', audio=None, spectrogram=None),
-Unit(onset=2.346125, offset=2.373125, label='-', audio=None, spectrogram=None), Unit(onset=2.50471875, offset=2.51546875,
-label='-', audio=None, spectrogram=None), Unit(onset=2.81909375, offset=2.84740625, label='-', audio=None, spectrogram=None),
-...
->>> # test that we can load the dataset
->>> seq_dataset_loaded = voc.dataset.SequenceDataset.from_sqlite(db_name='gy6or6-032312.db')
->>> seq_dataset_loaded == seq_dataset
+                                           Unit(onset=2.346125, offset=2.373125, label='-', audio=None,
+                                                spectrogram=None), Unit(onset=2.50471875, offset=2.51546875,
+                                                                        label='-', audio=None, spectrogram=None),
+                                           Unit(onset=2.81909375, offset=2.84740625, label='-', audio=None,
+                                                spectrogram=None),
+                                           ...
+                                           >> >  # test that we can load the dataset
+                                          >> > seq_dataset_loaded = voc.dataset.SequenceDataset.from_sqlite(
+  db_name='gy6or6-032312.db')
+                                                                    >> > seq_dataset_loaded == seq_dataset
 True
 ```
 
 
 ## Installation
 #### With `pip`
 ```
```

