# Comparing `tmp/mezcla-1.3.9.8.tar.gz` & `tmp/mezcla-1.3.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mezcla-1.3.9.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "mezcla-1.3.9.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `mezcla-1.3.9.8.tar` & `mezcla-1.3.9.9.tar`

### file list

```diff
@@ -1,217 +1,222 @@
--rw-r--r--   0        0        0      542 2023-08-31 03:42:59.481246 mezcla-1.3.9.8/.coveragerc
--rw-r--r--   0        0        0       67 2023-12-24 15:54:09.621229 mezcla-1.3.9.8/.github/CODEOWNERS
--rw-r--r--   0        0        0      129 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/.github/workflows/act-event.json
--rw-r--r--   0        0        0     3483 2024-01-15 00:49:02.193320 mezcla-1.3.9.8/.github/workflows/act.yml
--rw-r--r--   0        0        0     3955 2024-01-15 00:49:02.193320 mezcla-1.3.9.8/.github/workflows/debug.yml
--rw-r--r--   0        0        0      134 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/.github/workflows/github-event.json
--rw-r--r--   0        0        0     3220 2024-01-21 19:54:26.784324 mezcla-1.3.9.8/.github/workflows/github.yml
--rw-r--r--   0        0        0      137 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/.github/workflows/skip-docker.json
--rw-r--r--   0        0        0      137 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/.github/workflows/use-docker.json
--rw-r--r--   0        0        0     2142 2023-12-30 00:23:53.702664 mezcla-1.3.9.8/.gitignore
--rw-r--r--   0        0        0     6279 2024-01-15 05:24:19.324758 mezcla-1.3.9.8/Dockerfile
--rw-r--r--   0        0        0     7370 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/LICENSE.txt
--rw-r--r--   0        0        0      777 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/README.txt
--rw-r--r--   0        0        0      380 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/TODO.txt
--rw-r--r--   0        0        0      250 2024-01-05 07:20:43.100049 mezcla-1.3.9.8/_temp-user-docker.env
-lrwxr-xr-x   0        0        0        0 2023-11-24 09:48:13.530022 mezcla-1.3.9.8/local-workflows.sh -> tools/local-workflows.sh
--rw-r--r--   0        0        0      265 2023-11-14 05:21:22.635259 mezcla-1.3.9.8/mezcla/TODO.md
--rwxr-xr-x   0        0        0     2294 2024-01-26 18:16:38.774012 mezcla-1.3.9.8/mezcla/__init__.py
--rwxr-xr-x   0        0        0     1376 2023-11-01 04:13:50.848523 mezcla-1.3.9.8/mezcla/__main__.py
--rwxr-xr-x   0        0        0    10872 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/analyze_tfidf.py
--rwxr-xr-x   0        0        0    18007 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/mezcla/audio.py
--rwxr-xr-x   0        0        0     5052 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/bash_ast.py
--rwxr-xr-x   0        0        0    16055 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/bert_multi_classification.py
--rwxr-xr-x   0        0        0    25718 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/bert_text_classification.py
--rwxr-xr-x   0        0        0     8307 2023-12-03 22:09:20.600466 mezcla-1.3.9.8/mezcla/bing_search.py
--rwxr-xr-x   0        0        0     9241 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/check_html_javascript.py
--rwxr-xr-x   0        0        0    14896 2023-12-26 16:42:45.496986 mezcla-1.3.9.8/mezcla/compute_tfidf.py
--rwxr-xr-x   0        0        0     6042 2024-01-15 00:49:02.193320 mezcla-1.3.9.8/mezcla/convert_emoticons.py
--rwxr-xr-x   0        0        0    22554 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/cut.py
--rwxr-xr-x   0        0        0     4795 2023-11-01 04:13:50.848523 mezcla-1.3.9.8/mezcla/data_utils.py
--rwxr-xr-x   0        0        0    52402 2024-01-25 16:54:38.559622 mezcla-1.3.9.8/mezcla/debug.py
--rw-r--r--   0        0        0    25047 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/docs/audio_uml.svg
--rwxr-xr-x   0        0        0        0 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/__init__.py
--rwxr-xr-x   0        0        0    12874 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/alt_sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     3644 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/brownlee_ml_metrics.py
--rwxr-xr-x   0        0        0     2419 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/consume_all_memory.py
--rwxr-xr-x   0        0        0     5008 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/download_user_gist.py
--rw-r--r--   0        0        0      118 2023-09-04 18:41:17.983055 mezcla-1.3.9.8/mezcla/examples/dummy-image.png
--rwxr-xr-x   0        0        0     6477 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/dump_checkpoints.py
--rw-r--r--   0        0        0     2738 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/encoded-iris.csv
--rwxr-xr-x   0        0        0     8811 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/feature_importance.py
--rw-r--r--   0        0        0    40044 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/fuzzy-testing-1-2-3.wav
--rwxr-xr-x   0        0        0    54100 2024-01-26 18:09:16.447448 mezcla-1.3.9.8/mezcla/examples/hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     4660 2024-01-19 03:03:32.491569 mezcla-1.3.9.8/mezcla/examples/hugging_face_speechrec.py
--rwxr-xr-x   0        0        0     5622 2024-01-19 03:03:32.491569 mezcla-1.3.9.8/mezcla/examples/hugging_face_translation.py
--rwxr-xr-x   0        0        0    10347 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/inspect_checkpoint.py
--rw-r--r--   0        0        0     4607 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/iris.csv
--rw-r--r--   0        0        0    23345 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0     8279 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/plot_forest_importances.py
--rw-r--r--   0        0        0       20 2024-01-06 00:44:03.632067 mezcla-1.3.9.8/mezcla/examples/resources/translate_es_1.txt
--rw-r--r--   0        0        0     1809 2024-01-06 00:44:03.636067 mezcla-1.3.9.8/mezcla/examples/resources/translate_es_25.txt
--rw-r--r--   0        0        0   105004 2024-01-06 00:44:03.652066 mezcla-1.3.9.8/mezcla/examples/resources/us1.wav
--rw-r--r--   0        0        0    89644 2024-01-06 00:44:03.656066 mezcla-1.3.9.8/mezcla/examples/resources/us10.wav
--rw-r--r--   0        0        0   159725 2023-10-18 18:09:25.714553 mezcla-1.3.9.8/mezcla/examples/sd-spooky-pacman.png
--rwxr-xr-x   0        0        0    13004 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/sklearn_plot_precision_recall.py
--rwxr-xr-x   0        0        0     2060 2023-11-01 04:13:50.848523 mezcla-1.3.9.8/mezcla/examples/template.py
--rwxr-xr-x   0        0        0     3155 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/tensorflow_matrix_multiply.py
--rwxr-xr-x   0        0        0    11077 2024-01-26 18:09:55.810980 mezcla-1.3.9.8/mezcla/examples/tests/test_hf_stable_diffusion.py
--rwxr-xr-x   0        0        0     4608 2024-01-19 03:03:32.491569 mezcla-1.3.9.8/mezcla/examples/tests/test_hugging_face_speechrec.py
--rw-r--r--   0        0        0     5783 2024-01-06 00:44:03.672066 mezcla-1.3.9.8/mezcla/examples/tests/test_hugging_face_translation.py
--rwxr-xr-x   0        0        0     3617 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/examples/tracemalloc_display.py
--rwxr-xr-x   0        0        0     2884 2024-01-19 07:54:05.986709 mezcla-1.3.9.8/mezcla/examples/youtube_transcript.py
--rwxr-xr-x   0        0        0     5645 2023-11-01 04:13:50.848523 mezcla-1.3.9.8/mezcla/extract_document_text.py
--rwxr-xr-x   0        0        0     8648 2023-12-03 22:09:20.600466 mezcla-1.3.9.8/mezcla/file_utils.py
--rwxr-xr-x   0        0        0     3071 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/filter_random.py
--rwxr-xr-x   0        0        0     2999 2024-01-09 20:36:43.793404 mezcla-1.3.9.8/mezcla/format_profile.py
--rwxr-xr-x   0        0        0    32976 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/gensim_test.py
--rwxr-xr-x   0        0        0    37589 2024-01-13 02:28:41.693389 mezcla-1.3.9.8/mezcla/glue_helpers.py
--rwxr-xr-x   0        0        0    51307 2024-01-22 00:45:49.084147 mezcla-1.3.9.8/mezcla/html_utils.py
--rwxr-xr-x   0        0        0     5800 2024-01-19 07:54:05.990709 mezcla-1.3.9.8/mezcla/ipython_utils.py
--rwxr-xr-x   0        0        0     5718 2024-01-15 00:49:02.193320 mezcla-1.3.9.8/mezcla/kenlm_example.py
--rwxr-xr-x   0        0        0    17985 2023-10-18 18:09:25.714553 mezcla-1.3.9.8/mezcla/keras_param_search.py
--rwxr-xr-x   0        0        0    50921 2024-01-15 00:49:02.197319 mezcla-1.3.9.8/mezcla/main.py
--rwxr-xr-x   0        0        0     9307 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/merge_files.py
--rwxr-xr-x   0        0        0    11717 2023-08-31 03:42:59.485246 mezcla-1.3.9.8/mezcla/merge_notes.py
--rwxr-xr-x   0        0        0      608 2023-11-01 04:13:50.852523 mezcla-1.3.9.8/mezcla/mezcla
--rwxr-xr-x   0        0        0    16406 2024-01-15 05:24:19.324758 mezcla-1.3.9.8/mezcla/misc_utils.py
--rwxr-xr-x   0        0        0    10129 2023-11-14 05:21:22.671258 mezcla-1.3.9.8/mezcla/my_regex.py
--rwxr-xr-x   0        0        0    20913 2024-01-03 00:35:10.169127 mezcla-1.3.9.8/mezcla/ngram_tfidf.py
--rwxr-xr-x   0        0        0     1323 2024-01-16 02:27:06.071998 mezcla-1.3.9.8/mezcla/os_utils.py
--rwxr-xr-x   0        0        0    31564 2023-10-18 18:09:25.718553 mezcla-1.3.9.8/mezcla/pandas_sklearn.py
--rwxr-xr-x   0        0        0      915 2023-11-28 07:16:12.304850 mezcla-1.3.9.8/mezcla/plot_utils.py
--rwxr-xr-x   0        0        0     3202 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/python_ast.py
--rwxr-xr-x   0        0        0     7345 2023-11-14 05:21:22.671258 mezcla-1.3.9.8/mezcla/randomize_lines.py
--rwxr-xr-x   0        0        0     9144 2023-11-28 07:16:12.308850 mezcla-1.3.9.8/mezcla/rgb_color_name.py
--rwxr-xr-x   0        0        0    40735 2023-11-01 04:13:50.852523 mezcla-1.3.9.8/mezcla/run_albert_classifier.py
--rwxr-xr-x   0        0        0    39709 2023-11-01 04:13:50.856523 mezcla-1.3.9.8/mezcla/run_bert_classifier.py
--rw-r--r--   0        0        0    24045 2023-12-24 15:54:09.737228 mezcla-1.3.9.8/mezcla/samples/pima-indians-diabetes.csv
--rwxr-xr-x   0        0        0    17400 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/show_bert_representation.py
--rwxr-xr-x   0        0        0     2930 2023-11-01 04:13:50.856523 mezcla-1.3.9.8/mezcla/simple_main_example.py
--rwxr-xr-x   0        0        0    22751 2024-01-02 05:22:19.331782 mezcla-1.3.9.8/mezcla/spacy_nlp.py
--rwxr-xr-x   0        0        0     3168 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/mezcla/spell.py
--rwxr-xr-x   0        0        0     2416 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/sys_version_info_hack.py
--rwxr-xr-x   0        0        0    54405 2024-01-21 19:54:26.788324 mezcla-1.3.9.8/mezcla/system.py
--rw-r--r--   0        0        0   908397 2023-12-24 15:54:09.741228 mezcla-1.3.9.8/mezcla/temp/compound_CID_3672.xml
--rw-r--r--   0        0        0     1124 2024-01-06 00:44:03.672066 mezcla-1.3.9.8/mezcla/temp/plot.py
--rwxr-xr-x   0        0        0    45776 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     6183 2024-01-07 21:34:17.251121 mezcla-1.3.9.8/mezcla/template.py
--rw-r--r--   0        0        0     7370 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/LICENSE.txt
--rw-r--r--   0        0        0      140 2023-11-18 22:02:14.296885 mezcla-1.3.9.8/mezcla/tests/README.md
--rw-r--r--   0        0        0      462 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/TODO.md
--rw-r--r--   0        0        0     1082 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/adhoc-tests.batspp
--rwxr-xr-x   0        0        0     1900 2023-11-01 04:13:50.856523 mezcla-1.3.9.8/mezcla/tests/conftest.py
--rw-r--r--   0        0        0     1306 2023-12-24 15:54:09.741228 mezcla-1.3.9.8/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt
--rw-r--r--   0        0        0    21583 2023-12-24 15:54:09.753228 mezcla-1.3.9.8/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb
--rw-r--r--   0        0        0    28841 2024-01-06 00:44:03.672066 mezcla-1.3.9.8/mezcla/tests/jupyter/test_audio_py.ipynb
--rw-r--r--   0        0        0    44701 2023-12-24 15:54:09.753228 mezcla-1.3.9.8/mezcla/tests/jupyter/test_audio_py_experimental.ipynb
--rw-r--r--   0        0        0    23692 2024-01-06 00:44:03.672066 mezcla-1.3.9.8/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb
--rw-r--r--   0        0        0    29559 2023-12-24 15:54:09.753228 mezcla-1.3.9.8/mezcla/tests/jupyter/test_hugging_face_translation.ipynb
--rw-r--r--   0        0        0    58860 2024-01-06 00:44:03.672066 mezcla-1.3.9.8/mezcla/tests/jupyter/test_template.ipynb
--rw-r--r--   0        0        0     1176 2023-11-28 07:16:12.308850 mezcla-1.3.9.8/mezcla/tests/misc-tests.batspp
--rwxr-xr-x   0        0        0     3898 2023-11-24 09:48:13.530022 mezcla-1.3.9.8/mezcla/tests/misc_doctests.py
--rw-r--r--   0        0        0     3283 2024-01-13 02:28:41.693389 mezcla-1.3.9.8/mezcla/tests/misc_tests.py
--rw-r--r--   0        0        0      312 2023-11-18 22:02:14.296885 mezcla-1.3.9.8/mezcla/tests/regression.batspp
--rw-r--r--   0        0        0     1453 2023-12-17 23:19:18.562278 mezcla-1.3.9.8/mezcla/tests/resources/argentinian-attraction-snippets.txt
--rw-r--r--   0        0        0      810 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/cars-csv-len-3.txt
--rw-r--r--   0        0        0      113 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/cars-fields-2-3-4.txt
--rw-r--r--   0        0        0      602 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/cars-tsv-len-3.txt
--rw-r--r--   0        0        0      659 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/cars.csv
--rw-r--r--   0        0        0      655 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/cars.tsv
--rw-r--r--   0        0        0      603 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/example_text.txt
--rw-r--r--   0        0        0     2573 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/example_text_tags.txt
--rw-r--r--   0        0        0     2440 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/iris_output.txt
--rw-r--r--   0        0        0   324207 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/random-10pct-tweet-emotions.tsv
--rw-r--r--   0        0        0     1152 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/simple-window-dimensions.html
--rw-r--r--   0        0        0     5577 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/spanish-accents.docx
--rw-r--r--   0        0        0    12530 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/spanish-accents.pdf
--rw-r--r--   0        0        0      141 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/spanish-accents.txt
--rw-r--r--   0        0        0      415 2024-01-06 00:44:03.672066 mezcla-1.3.9.8/mezcla/tests/resources/spell-py-ar.list
--rw-r--r--   0        0        0      391 2024-01-06 00:44:03.672066 mezcla-1.3.9.8/mezcla/tests/resources/spell-py-en.list
--rw-r--r--   0        0        0      294 2024-01-06 00:44:03.672066 mezcla-1.3.9.8/mezcla/tests/resources/spell-py-es.list
--rw-r--r--   0        0        0      472 2024-01-06 00:44:03.672066 mezcla-1.3.9.8/mezcla/tests/resources/spell-py-ru.list
--rw-r--r--   0        0        0     2780 2023-12-24 15:54:09.753228 mezcla-1.3.9.8/mezcla/tests/resources/test.arpa
--rw-r--r--   0        0        0       65 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/resources/word-POS.freq
--rw-r--r--   0        0        0      254 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/simple-script-tests.test
--rwxr-xr-x   0        0        0     5509 2023-11-28 07:16:12.308850 mezcla-1.3.9.8/mezcla/tests/template.py
--rwxr-xr-x   0        0        0     1766 2024-01-07 21:34:17.303120 mezcla-1.3.9.8/mezcla/tests/test___init__.py
--rwxr-xr-x   0        0        0     5942 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/mezcla/tests/test_audio.py
--rwxr-xr-x   0        0        0      969 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_bert_multi_classification.py
--rwxr-xr-x   0        0        0     2343 2023-10-23 22:16:11.253304 mezcla-1.3.9.8/mezcla/tests/test_bing_search.py
--rwxr-xr-x   0        0        0     7559 2023-12-17 23:19:18.586278 mezcla-1.3.9.8/mezcla/tests/test_compute_tfidf.py
--rwxr-xr-x   0        0        0     4712 2024-01-16 02:27:06.071998 mezcla-1.3.9.8/mezcla/tests/test_convert_emoticons.py
--rwxr-xr-x   0        0        0     2905 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_cut.py
--rwxr-xr-x   0        0        0     2464 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_data_utils.py
--rwxr-xr-x   0        0        0    17872 2024-01-13 02:28:41.693389 mezcla-1.3.9.8/mezcla/tests/test_debug.py
--rwxr-xr-x   0        0        0     5469 2024-01-09 03:21:48.239009 mezcla-1.3.9.8/mezcla/tests/test_extract_document_text.py
--rwxr-xr-x   0        0        0     4429 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_file_utils.py
--rwxr-xr-x   0        0        0     2939 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_filter_random.py
--rwxr-xr-x   0        0        0    17414 2024-01-09 03:21:48.243009 mezcla-1.3.9.8/mezcla/tests/test_format_profile.py
--rwxr-xr-x   0        0        0     3449 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_gensim_test.py
--rwxr-xr-x   0        0        0    16307 2023-10-18 18:09:25.718553 mezcla-1.3.9.8/mezcla/tests/test_glue_helpers.py
--rwxr-xr-x   0        0        0    13525 2024-01-25 16:53:18.472738 mezcla-1.3.9.8/mezcla/tests/test_html_utils.py
--rwxr-xr-x   0        0        0     2023 2023-10-18 18:09:25.718553 mezcla-1.3.9.8/mezcla/tests/test_ipython_utils.py
--rwxr-xr-x   0        0        0    11821 2024-01-13 01:35:04.957349 mezcla-1.3.9.8/mezcla/tests/test_kenlm_example.py
--rwxr-xr-x   0        0        0     3473 2023-12-24 15:54:09.753228 mezcla-1.3.9.8/mezcla/tests/test_keras_param_search.py
--rwxr-xr-x   0        0        0     9925 2023-10-18 18:09:25.718553 mezcla-1.3.9.8/mezcla/tests/test_main.py
--rwxr-xr-x   0        0        0     2725 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_merge_files.py
--rwxr-xr-x   0        0        0     1291 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_merge_notes.py
--rwxr-xr-x   0        0        0     6844 2024-01-15 05:24:19.324758 mezcla-1.3.9.8/mezcla/tests/test_misc_utils.py
--rwxr-xr-x   0        0        0     4204 2024-01-19 03:06:09.373515 mezcla-1.3.9.8/mezcla/tests/test_my_regex.py
--rwxr-xr-x   0        0        0     5098 2023-12-26 16:42:45.500985 mezcla-1.3.9.8/mezcla/tests/test_ngram_tfidf.py
--rwxr-xr-x   0        0        0     1400 2024-01-16 02:27:06.075998 mezcla-1.3.9.8/mezcla/tests/test_os_utils.py
--rwxr-xr-x   0        0        0     8297 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_pandas_sklearn.py
--rwxr-xr-x   0        0        0     1183 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_plot_utils.py
--rwxr-xr-x   0        0        0     2156 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_python_ast.py
--rwxr-xr-x   0        0        0     1735 2023-11-14 05:21:22.671258 mezcla-1.3.9.8/mezcla/tests/test_randomize_lines.py
--rwxr-xr-x   0        0        0     2389 2024-01-07 21:34:17.463118 mezcla-1.3.9.8/mezcla/tests/test_rgb_color_name.py
--rwxr-xr-x   0        0        0      895 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_run_albert_classifier.py
--rwxr-xr-x   0        0        0      930 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_run_bert_classifier.py
--rwxr-xr-x   0        0        0     1602 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_show_bert_representation.py
--rwxr-xr-x   0        0        0     2372 2023-10-23 22:16:11.253304 mezcla-1.3.9.8/mezcla/tests/test_simple_main_example.py
--rwxr-xr-x   0        0        0     5511 2023-12-31 20:01:51.814975 mezcla-1.3.9.8/mezcla/tests/test_spacy_nlp.py
--rwxr-xr-x   0        0        0    12822 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/mezcla/tests/test_spell.py
--rwxr-xr-x   0        0        0      882 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_sys_version_info_hack.py
--rwxr-xr-x   0        0        0    36569 2024-01-19 03:03:32.491569 mezcla-1.3.9.8/mezcla/tests/test_system.py
--rwxr-xr-x   0        0        0     2231 2024-01-07 21:34:17.463118 mezcla-1.3.9.8/mezcla/tests/test_template.py
--rwxr-xr-x   0        0        0     5752 2023-11-05 02:06:02.889022 mezcla-1.3.9.8/mezcla/tests/test_text_categorizer.py
--rwxr-xr-x   0        0        0     8905 2024-01-07 21:34:17.463118 mezcla-1.3.9.8/mezcla/tests/test_text_processing.py
--rwxr-xr-x   0        0        0     7361 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_text_utils.py
--rwxr-xr-x   0        0        0    23029 2023-10-18 18:09:25.718553 mezcla-1.3.9.8/mezcla/tests/test_tpo_common.py
--rwxr-xr-x   0        0        0      715 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_train_language_model.py
--rwxr-xr-x   0        0        0     2041 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/test_train_text_categorizer.py
--rwxr-xr-x   0        0        0     4172 2023-12-24 15:54:09.757228 mezcla-1.3.9.8/mezcla/tests/test_transpose_data.py
--rw-r--r--   0        0        0      435 2023-12-24 15:54:09.757228 mezcla-1.3.9.8/mezcla/tests/test_transpose_lines.input
--rwxr-xr-x   0        0        0     3411 2024-01-16 02:27:06.075998 mezcla-1.3.9.8/mezcla/tests/test_unittest_wrapper.py
--rwxr-xr-x   0        0        0     2355 2024-01-07 21:34:17.495117 mezcla-1.3.9.8/mezcla/tests/test_xml_utils.py
--rwxr-xr-x   0        0        0      676 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/tfidf/test_corpus.py
--rwxr-xr-x   0        0        0      697 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/tfidf/test_dockeyword.py
--rwxr-xr-x   0        0        0      688 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/tfidf/test_document.py
--rwxr-xr-x   0        0        0      697 2023-08-31 03:42:59.489246 mezcla-1.3.9.8/mezcla/tests/tfidf/test_preprocess.py
--rwxr-xr-x   0        0        0    36563 2023-11-05 02:06:02.889022 mezcla-1.3.9.8/mezcla/text_categorizer.py
--rwxr-xr-x   0        0        0    28318 2024-01-07 21:34:17.527117 mezcla-1.3.9.8/mezcla/text_processing.py
--rwxr-xr-x   0        0        0    13108 2023-08-31 03:42:59.493246 mezcla-1.3.9.8/mezcla/text_utils.py
--rwxr-xr-x   0        0        0      375 2023-12-17 23:19:18.586278 mezcla-1.3.9.8/mezcla/tfidf/__init__.py
--rwxr-xr-x   0        0        0      777 2023-11-25 08:02:17.308369 mezcla-1.3.9.8/mezcla/tfidf/config.py
--rwxr-xr-x   0        0        0    19427 2023-12-26 16:42:45.512985 mezcla-1.3.9.8/mezcla/tfidf/corpus.py
--rwxr-xr-x   0        0        0     3146 2023-12-17 23:19:18.586278 mezcla-1.3.9.8/mezcla/tfidf/dockeyword.py
--rwxr-xr-x   0        0        0     7925 2023-12-17 23:19:18.586278 mezcla-1.3.9.8/mezcla/tfidf/document.py
--rwxr-xr-x   0        0        0    18886 2024-01-03 04:39:46.958772 mezcla-1.3.9.8/mezcla/tfidf/preprocess.py
--rw-r--r--   0        0        0     3961 2023-12-17 23:19:18.630277 mezcla-1.3.9.8/mezcla/tfidf/tests/misc_test.py
--rwxr-xr-x   0        0        0    60411 2024-01-07 21:34:17.527117 mezcla-1.3.9.8/mezcla/tpo_common.py
--rwxr-xr-x   0        0        0     5272 2023-12-24 15:54:09.757228 mezcla-1.3.9.8/mezcla/train_language_model.py
--rwxr-xr-x   0        0        0     5149 2023-08-31 03:42:59.493246 mezcla-1.3.9.8/mezcla/train_text_categorizer.py
--rwxr-xr-x   0        0        0     6673 2023-10-18 18:09:25.722553 mezcla-1.3.9.8/mezcla/transpose_data.py
--rwxr-xr-x   0        0        0    22511 2024-01-19 03:03:32.495569 mezcla-1.3.9.8/mezcla/unittest_wrapper.py
--rwxr-xr-x   0        0        0     3543 2023-08-31 03:42:59.493246 mezcla-1.3.9.8/mezcla/xml_utils.py
--rw-r--r--   0        0        0      432 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/non-binary-requirements.txt
--rw-r--r--   0        0        0      803 2024-01-26 18:16:38.774012 mezcla-1.3.9.8/pyproject.toml
--rw-r--r--   0        0        0      750 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/required-packages.txt
--rw-r--r--   0        0        0     3663 2024-01-26 17:49:27.934394 mezcla-1.3.9.8/requirements.txt
-lrwxr-xr-x   0        0        0        0 2023-11-24 09:48:13.530022 mezcla-1.3.9.8/run_tests.bash -> tools/run_tests.bash
--rwxr-xr-x   0        0        0     1943 2024-01-26 18:16:38.774012 mezcla-1.3.9.8/setup.py
--rwxr-xr-x   0        0        0    45023 2023-08-31 03:42:59.493246 mezcla-1.3.9.8/temp/simple_batspp.py
--rwxr-xr-x   0        0        0     3002 2024-01-10 03:38:56.034061 mezcla-1.3.9.8/tools/local-workflows.sh
--rwxr-xr-x   0        0        0     2410 2024-01-09 03:21:48.243009 mezcla-1.3.9.8/tools/run_tests.bash
--rw-r--r--   0        0        0      612 2023-08-31 03:42:59.493246 mezcla-1.3.9.8/tox.ini
--rw-r--r--   0        0        0     1087 1970-01-01 00:00:00.000000 mezcla-1.3.9.8/PKG-INFO
+-rw-r--r--   0        0        0      542 2023-06-18 00:28:36.095854 mezcla-1.3.9.9/.coveragerc
+-rw-r--r--   0        0        0       67 2023-12-23 00:35:49.550955 mezcla-1.3.9.9/.github/CODEOWNERS
+-rw-r--r--   0        0        0      129 2024-01-10 03:17:12.006045 mezcla-1.3.9.9/.github/workflows/act-event.json
+-rw-r--r--   0        0        0     3483 2024-01-12 23:59:44.940873 mezcla-1.3.9.9/.github/workflows/act.yml
+-rw-r--r--   0        0        0     3955 2024-01-12 23:59:44.940873 mezcla-1.3.9.9/.github/workflows/debug.yml
+-rw-r--r--   0        0        0      134 2024-01-10 03:17:12.010045 mezcla-1.3.9.9/.github/workflows/github-event.json
+-rw-r--r--   0        0        0     3220 2024-01-20 01:04:29.190369 mezcla-1.3.9.9/.github/workflows/github.yml
+-rw-r--r--   0        0        0      137 2024-01-10 03:17:12.010045 mezcla-1.3.9.9/.github/workflows/skip-docker.json
+-rw-r--r--   0        0        0      137 2024-01-10 03:17:12.010045 mezcla-1.3.9.9/.github/workflows/use-docker.json
+-rw-r--r--   0        0        0     2150 2024-02-05 02:22:35.674201 mezcla-1.3.9.9/.gitignore
+-rw-r--r--   0        0        0     6279 2024-01-15 02:08:46.605161 mezcla-1.3.9.9/Dockerfile
+-rw-r--r--   0        0        0     7370 2023-06-18 00:28:36.095854 mezcla-1.3.9.9/LICENSE.txt
+-rw-r--r--   0        0        0      883 2024-02-15 05:46:43.319262 mezcla-1.3.9.9/README.txt
+-rw-r--r--   0        0        0      380 2023-06-18 00:28:36.095854 mezcla-1.3.9.9/TODO.txt
+-rw-r--r--   0        0        0      250 2024-01-06 01:21:58.419999 mezcla-1.3.9.9/_temp-user-docker.env
+lrwxr-xr-x   0        0        0        0 2023-11-20 19:32:27.964661 mezcla-1.3.9.9/local-workflows.sh -> tools/local-workflows.sh
+-rw-r--r--   0        0        0      265 2023-11-19 20:31:47.986747 mezcla-1.3.9.9/mezcla/TODO.md
+-rwxr-xr-x   0        0        0     2294 2024-02-27 21:18:43.570553 mezcla-1.3.9.9/mezcla/__init__.py
+-rwxr-xr-x   0        0        0     1376 2023-10-28 05:49:57.823956 mezcla-1.3.9.9/mezcla/__main__.py
+-rwxr-xr-x   0        0        0    10872 2023-07-03 03:15:57.247954 mezcla-1.3.9.9/mezcla/analyze_tfidf.py
+-rwxr-xr-x   0        0        0    18007 2024-01-10 03:53:41.456581 mezcla-1.3.9.9/mezcla/audio.py
+-rwxr-xr-x   0        0        0     5052 2023-08-04 17:22:24.731552 mezcla-1.3.9.9/mezcla/bash_ast.py
+-rwxr-xr-x   0        0        0    16055 2023-06-18 00:28:36.099855 mezcla-1.3.9.9/mezcla/bert_multi_classification.py
+-rwxr-xr-x   0        0        0    25718 2023-07-03 03:15:57.251955 mezcla-1.3.9.9/mezcla/bert_text_classification.py
+-rwxr-xr-x   0        0        0     8307 2023-12-05 06:09:36.641882 mezcla-1.3.9.9/mezcla/bing_search.py
+-rwxr-xr-x   0        0        0     9241 2023-07-03 03:15:57.251955 mezcla-1.3.9.9/mezcla/check_html_javascript.py
+-rwxr-xr-x   0        0        0    14896 2023-12-25 20:30:57.995670 mezcla-1.3.9.9/mezcla/compute_tfidf.py
+-rwxr-xr-x   0        0        0     6042 2024-01-14 21:22:54.323127 mezcla-1.3.9.9/mezcla/convert_emoticons.py
+-rwxr-xr-x   0        0        0    22554 2023-08-04 17:22:24.731552 mezcla-1.3.9.9/mezcla/cut.py
+-rwxr-xr-x   0        0        0     4795 2023-11-07 23:03:56.570514 mezcla-1.3.9.9/mezcla/data_utils.py
+-rwxr-xr-x   0        0        0    52432 2024-02-10 06:04:37.816315 mezcla-1.3.9.9/mezcla/debug.py
+-rw-r--r--   0        0        0    25047 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/docs/audio_uml.svg
+-rwxr-xr-x   0        0        0     4842 2024-02-18 01:07:01.707066 mezcla-1.3.9.9/mezcla/evaluate_example_tests.py
+-rwxr-xr-x   0        0        0        0 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/__init__.py
+-rwxr-xr-x   0        0        0    12874 2023-07-03 03:15:57.251955 mezcla-1.3.9.9/mezcla/examples/alt_sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     3644 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/examples/brownlee_ml_metrics.py
+-rwxr-xr-x   0        0        0     2419 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/consume_all_memory.py
+-rwxr-xr-x   0        0        0     5008 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/download_user_gist.py
+-rw-r--r--   0        0        0      118 2023-09-03 04:28:25.907636 mezcla-1.3.9.9/mezcla/examples/dummy-image.png
+-rwxr-xr-x   0        0        0     6477 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/dump_checkpoints.py
+-rw-r--r--   0        0        0     2738 2023-06-18 00:28:36.103855 mezcla-1.3.9.9/mezcla/examples/encoded-iris.csv
+-rwxr-xr-x   0        0        0     8811 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/examples/feature_importance.py
+-rw-r--r--   0        0        0    40044 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/fuzzy-testing-1-2-3.wav
+-rwxr-xr-x   0        0        0    54141 2024-02-24 00:18:03.430170 mezcla-1.3.9.9/mezcla/examples/hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     4660 2024-01-19 02:56:58.191707 mezcla-1.3.9.9/mezcla/examples/hugging_face_speechrec.py
+-rwxr-xr-x   0        0        0     6011 2024-02-18 02:09:14.186107 mezcla-1.3.9.9/mezcla/examples/hugging_face_translation.py
+-rwxr-xr-x   0        0        0    10347 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/inspect_checkpoint.py
+-rw-r--r--   0        0        0     4607 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/iris.csv
+-rw-r--r--   0        0        0    23345 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0     8279 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/plot_forest_importances.py
+-rw-r--r--   0        0        0       20 2024-01-06 01:21:58.419999 mezcla-1.3.9.9/mezcla/examples/resources/translate_es_1.txt
+-rw-r--r--   0        0        0     1809 2024-01-06 01:21:58.419999 mezcla-1.3.9.9/mezcla/examples/resources/translate_es_25.txt
+-rw-r--r--   0        0        0   105004 2024-01-06 01:21:58.423999 mezcla-1.3.9.9/mezcla/examples/resources/us1.wav
+-rw-r--r--   0        0        0    89644 2024-01-06 01:21:58.423999 mezcla-1.3.9.9/mezcla/examples/resources/us10.wav
+-rw-r--r--   0        0        0   159725 2023-09-24 17:55:32.838498 mezcla-1.3.9.9/mezcla/examples/sd-spooky-pacman.png
+-rwxr-xr-x   0        0        0    13004 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/examples/sklearn_plot_precision_recall.py
+-rwxr-xr-x   0        0        0     2072 2024-02-13 23:48:53.709200 mezcla-1.3.9.9/mezcla/examples/template.py
+-rwxr-xr-x   0        0        0     3155 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/examples/tensorflow_matrix_multiply.py
+-rwxr-xr-x   0        0        0    13881 2024-01-26 22:05:20.253359 mezcla-1.3.9.9/mezcla/examples/tests/test_hf_stable_diffusion.py
+-rwxr-xr-x   0        0        0     4608 2024-01-19 02:57:22.956854 mezcla-1.3.9.9/mezcla/examples/tests/test_hugging_face_speechrec.py
+-rw-r--r--   0        0        0     5783 2024-01-06 01:21:58.439999 mezcla-1.3.9.9/mezcla/examples/tests/test_hugging_face_translation.py
+-rw-r--r--   0        0        0     4272 2024-02-05 06:18:22.947788 mezcla-1.3.9.9/mezcla/examples/tests/test_youtube_transcript.py
+-rwxr-xr-x   0        0        0     3617 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/examples/tracemalloc_display.py
+-rwxr-xr-x   0        0        0     3351 2024-02-13 23:49:45.739212 mezcla-1.3.9.9/mezcla/examples/youtube_transcript.py
+-rwxr-xr-x   0        0        0     5645 2023-10-28 05:49:57.827956 mezcla-1.3.9.9/mezcla/extract_document_text.py
+-rwxr-xr-x   0        0        0     8648 2023-12-05 06:09:36.641882 mezcla-1.3.9.9/mezcla/file_utils.py
+-rwxr-xr-x   0        0        0     3071 2023-06-18 00:28:36.107855 mezcla-1.3.9.9/mezcla/filter_random.py
+-rwxr-xr-x   0        0        0     2836 2024-02-25 21:50:11.199678 mezcla-1.3.9.9/mezcla/format_profile.py
+-rwxr-xr-x   0        0        0    32976 2023-07-03 03:15:57.255955 mezcla-1.3.9.9/mezcla/gensim_test.py
+-rwxr-xr-x   0        0        0    38023 2024-02-14 01:20:37.557523 mezcla-1.3.9.9/mezcla/glue_helpers.py
+-rwxr-xr-x   0        0        0    51316 2024-01-26 22:07:19.425573 mezcla-1.3.9.9/mezcla/html_utils.py
+-rwxr-xr-x   0        0        0     5800 2024-01-19 07:25:16.197480 mezcla-1.3.9.9/mezcla/ipython_utils.py
+-rwxr-xr-x   0        0        0     5718 2024-01-13 00:02:35.064560 mezcla-1.3.9.9/mezcla/kenlm_example.py
+-rwxr-xr-x   0        0        0    17985 2023-10-16 22:30:24.461638 mezcla-1.3.9.9/mezcla/keras_param_search.py
+-rwxr-xr-x   0        0        0    52196 2024-02-25 23:17:36.844026 mezcla-1.3.9.9/mezcla/main.py
+-rwxr-xr-x   0        0        0     9307 2023-06-18 00:28:36.115856 mezcla-1.3.9.9/mezcla/merge_files.py
+-rwxr-xr-x   0        0        0    11040 2024-02-05 02:23:37.860124 mezcla-1.3.9.9/mezcla/merge_notes.py
+-rwxr-xr-x   0        0        0      608 2023-10-28 05:49:57.831956 mezcla-1.3.9.9/mezcla/mezcla
+-rwxr-xr-x   0        0        0    16908 2024-01-29 02:43:05.206522 mezcla-1.3.9.9/mezcla/misc_utils.py
+-rwxr-xr-x   0        0        0    10273 2024-01-29 02:46:17.354076 mezcla-1.3.9.9/mezcla/my_regex.py
+-rwxr-xr-x   0        0        0    23846 2024-02-24 00:35:11.471795 mezcla-1.3.9.9/mezcla/ngram_tfidf.py
+-rwxr-xr-x   0        0        0     1323 2024-01-16 02:17:35.819701 mezcla-1.3.9.9/mezcla/os_utils.py
+-rwxr-xr-x   0        0        0    31564 2023-10-16 22:30:24.461638 mezcla-1.3.9.9/mezcla/pandas_sklearn.py
+-rwxr-xr-x   0        0        0      915 2023-11-28 08:56:45.997810 mezcla-1.3.9.9/mezcla/plot_utils.py
+-rwxr-xr-x   0        0        0     3202 2023-07-21 06:17:43.311676 mezcla-1.3.9.9/mezcla/python_ast.py
+-rwxr-xr-x   0        0        0     7345 2023-11-19 20:31:47.994747 mezcla-1.3.9.9/mezcla/randomize_lines.py
+-rwxr-xr-x   0        0        0     9144 2023-11-28 08:56:46.001810 mezcla-1.3.9.9/mezcla/rgb_color_name.py
+-rwxr-xr-x   0        0        0    40735 2023-10-28 05:49:57.835956 mezcla-1.3.9.9/mezcla/run_albert_classifier.py
+-rwxr-xr-x   0        0        0    39709 2023-10-28 05:49:57.835956 mezcla-1.3.9.9/mezcla/run_bert_classifier.py
+-rw-r--r--   0        0        0    24045 2023-12-23 00:35:49.666955 mezcla-1.3.9.9/mezcla/samples/pima-indians-diabetes.csv
+-rwxr-xr-x   0        0        0    17400 2023-06-18 00:28:36.119856 mezcla-1.3.9.9/mezcla/show_bert_representation.py
+-rwxr-xr-x   0        0        0     2930 2023-10-28 05:49:57.835956 mezcla-1.3.9.9/mezcla/simple_main_example.py
+-rwxr-xr-x   0        0        0    22899 2024-02-09 05:58:53.199379 mezcla-1.3.9.9/mezcla/spacy_nlp.py
+-rwxr-xr-x   0        0        0     3168 2024-01-10 03:13:25.131399 mezcla-1.3.9.9/mezcla/spell.py
+-rwxr-xr-x   0        0        0     2416 2023-06-18 00:28:36.119856 mezcla-1.3.9.9/mezcla/sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    54669 2024-01-27 06:59:58.811207 mezcla-1.3.9.9/mezcla/system.py
+-rw-r--r--   0        0        0   908397 2023-12-23 00:35:49.678955 mezcla-1.3.9.9/mezcla/temp/compound_CID_3672.xml
+-rw-r--r--   0        0        0     1124 2024-01-06 01:21:58.439999 mezcla-1.3.9.9/mezcla/temp/plot.py
+-rwxr-xr-x   0        0        0    45776 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/temp/simple_batspp.py
+-rwxr-xr-x   0        0        0     6257 2024-02-18 02:10:12.834939 mezcla-1.3.9.9/mezcla/template.py
+-rw-r--r--   0        0        0     7370 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/LICENSE.txt
+-rw-r--r--   0        0        0      140 2023-11-19 20:31:47.994747 mezcla-1.3.9.9/mezcla/tests/README.md
+-rw-r--r--   0        0        0      462 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/TODO.md
+-rw-r--r--   0        0        0     1082 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/adhoc-tests.batspp
+-rwxr-xr-x   0        0        0     1900 2023-10-28 05:49:57.835956 mezcla-1.3.9.9/mezcla/tests/conftest.py
+-rw-r--r--   0        0        0     1306 2023-12-23 00:35:49.678955 mezcla-1.3.9.9/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt
+-rw-r--r--   0        0        0    21583 2023-12-23 00:35:49.678955 mezcla-1.3.9.9/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb
+-rw-r--r--   0        0        0    28841 2024-01-06 01:21:58.439999 mezcla-1.3.9.9/mezcla/tests/jupyter/test_audio_py.ipynb
+-rw-r--r--   0        0        0    44701 2023-12-23 00:35:49.682955 mezcla-1.3.9.9/mezcla/tests/jupyter/test_audio_py_experimental.ipynb
+-rw-r--r--   0        0        0    23692 2024-01-06 01:21:58.439999 mezcla-1.3.9.9/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb
+-rw-r--r--   0        0        0    29559 2023-12-23 00:35:49.682955 mezcla-1.3.9.9/mezcla/tests/jupyter/test_hugging_face_translation.ipynb
+-rw-r--r--   0        0        0    58860 2024-01-06 01:21:58.443999 mezcla-1.3.9.9/mezcla/tests/jupyter/test_template.ipynb
+-rw-r--r--   0        0        0     1176 2023-11-28 08:56:46.001810 mezcla-1.3.9.9/mezcla/tests/misc-tests.batspp
+-rwxr-xr-x   0        0        0     3898 2023-11-23 07:44:42.985055 mezcla-1.3.9.9/mezcla/tests/misc_doctests.py
+-rw-r--r--   0        0        0     3283 2024-01-13 02:25:33.199045 mezcla-1.3.9.9/mezcla/tests/misc_tests.py
+-rw-r--r--   0        0        0      312 2023-11-19 20:31:47.994747 mezcla-1.3.9.9/mezcla/tests/regression.batspp
+-rw-r--r--   0        0        0     1453 2023-12-13 03:20:36.066992 mezcla-1.3.9.9/mezcla/tests/resources/argentinian-attraction-snippets.txt
+-rw-r--r--   0        0        0      810 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars-csv-len-3.txt
+-rw-r--r--   0        0        0      113 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars-fields-2-3-4.txt
+-rw-r--r--   0        0        0      602 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars-tsv-len-3.txt
+-rw-r--r--   0        0        0      659 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars.csv
+-rw-r--r--   0        0        0      655 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/cars.tsv
+-rw-r--r--   0        0        0      603 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/example_text.txt
+-rw-r--r--   0        0        0     2573 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/example_text_tags.txt
+-rw-r--r--   0        0        0     2440 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/iris_output.txt
+-rw-r--r--   0        0        0   324207 2023-08-15 23:14:53.434294 mezcla-1.3.9.9/mezcla/tests/resources/random-10pct-tweet-emotions.tsv
+-rw-r--r--   0        0        0     1152 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/simple-window-dimensions.html
+-rw-r--r--   0        0        0     5577 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.docx
+-rw-r--r--   0        0        0    12530 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.pdf
+-rw-r--r--   0        0        0      141 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.txt
+-rw-r--r--   0        0        0      415 2024-01-06 01:21:58.451999 mezcla-1.3.9.9/mezcla/tests/resources/spell-py-ar.list
+-rw-r--r--   0        0        0      391 2024-01-06 01:21:58.451999 mezcla-1.3.9.9/mezcla/tests/resources/spell-py-en.list
+-rw-r--r--   0        0        0      294 2024-01-06 01:21:58.451999 mezcla-1.3.9.9/mezcla/tests/resources/spell-py-es.list
+-rw-r--r--   0        0        0      472 2024-01-06 01:21:58.451999 mezcla-1.3.9.9/mezcla/tests/resources/spell-py-ru.list
+-rw-r--r--   0        0        0     2780 2023-12-23 00:35:49.682955 mezcla-1.3.9.9/mezcla/tests/resources/test.arpa
+-rwxr-xr-x   0        0        0    14631 2024-02-25 21:50:57.298231 mezcla-1.3.9.9/mezcla/tests/resources/word-POS.freq
+-rwxr-xr-x   0        0        0    11479 2024-02-25 21:44:14.241332 mezcla-1.3.9.9/mezcla/tests/resources/word.freq
+-rw-r--r--   0        0        0      254 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/simple-script-tests.test
+-rwxr-xr-x   0        0        0     5120 2024-02-26 23:37:28.019883 mezcla-1.3.9.9/mezcla/tests/template.py
+-rwxr-xr-x   0        0        0     1766 2024-01-10 03:13:25.131399 mezcla-1.3.9.9/mezcla/tests/test___init__.py
+-rwxr-xr-x   0        0        0     5942 2024-01-10 03:13:25.131399 mezcla-1.3.9.9/mezcla/tests/test_audio.py
+-rwxr-xr-x   0        0        0      969 2023-06-18 00:28:36.123857 mezcla-1.3.9.9/mezcla/tests/test_bert_multi_classification.py
+-rwxr-xr-x   0        0        0     2343 2023-10-24 00:05:30.113456 mezcla-1.3.9.9/mezcla/tests/test_bing_search.py
+-rwxr-xr-x   0        0        0     7559 2023-12-13 03:20:36.066992 mezcla-1.3.9.9/mezcla/tests/test_compute_tfidf.py
+-rwxr-xr-x   0        0        0     4681 2024-01-29 02:49:52.352507 mezcla-1.3.9.9/mezcla/tests/test_convert_emoticons.py
+-rwxr-xr-x   0        0        0     2905 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_cut.py
+-rwxr-xr-x   0        0        0     2464 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_data_utils.py
+-rwxr-xr-x   0        0        0    17872 2024-01-13 02:25:33.199045 mezcla-1.3.9.9/mezcla/tests/test_debug.py
+-rwxr-xr-x   0        0        0     2654 2024-02-18 00:52:35.708230 mezcla-1.3.9.9/mezcla/tests/test_evaluate_example_tests.py
+-rwxr-xr-x   0        0        0     5469 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_extract_document_text.py
+-rwxr-xr-x   0        0        0     4429 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_file_utils.py
+-rwxr-xr-x   0        0        0     2939 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_filter_random.py
+-rwxr-xr-x   0        0        0    17414 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_format_profile.py
+-rwxr-xr-x   0        0        0     3449 2023-07-03 03:15:57.263955 mezcla-1.3.9.9/mezcla/tests/test_gensim_test.py
+-rwxr-xr-x   0        0        0    17227 2024-02-11 07:09:18.051172 mezcla-1.3.9.9/mezcla/tests/test_glue_helpers.py
+-rwxr-xr-x   0        0        0    13525 2024-01-19 07:26:02.648020 mezcla-1.3.9.9/mezcla/tests/test_html_utils.py
+-rwxr-xr-x   0        0        0     2023 2023-10-16 22:30:24.465638 mezcla-1.3.9.9/mezcla/tests/test_ipython_utils.py
+-rwxr-xr-x   0        0        0    11821 2024-01-10 05:20:11.597430 mezcla-1.3.9.9/mezcla/tests/test_kenlm_example.py
+-rwxr-xr-x   0        0        0     3473 2023-12-24 04:34:38.391312 mezcla-1.3.9.9/mezcla/tests/test_keras_param_search.py
+-rwxr-xr-x   0        0        0    10850 2024-02-15 05:50:30.569406 mezcla-1.3.9.9/mezcla/tests/test_main.py
+-rwxr-xr-x   0        0        0     2725 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_merge_files.py
+-rwxr-xr-x   0        0        0     1291 2023-06-18 00:28:36.127857 mezcla-1.3.9.9/mezcla/tests/test_merge_notes.py
+-rwxr-xr-x   0        0        0     9528 2024-02-16 17:38:36.156177 mezcla-1.3.9.9/mezcla/tests/test_misc_utils.py
+-rwxr-xr-x   0        0        0     4204 2024-01-19 07:24:28.075538 mezcla-1.3.9.9/mezcla/tests/test_my_regex.py
+-rwxr-xr-x   0        0        0     5098 2023-12-25 20:30:57.995670 mezcla-1.3.9.9/mezcla/tests/test_ngram_tfidf.py
+-rwxr-xr-x   0        0        0     1400 2024-01-16 02:25:00.658659 mezcla-1.3.9.9/mezcla/tests/test_os_utils.py
+-rwxr-xr-x   0        0        0     8297 2023-07-03 03:15:57.263955 mezcla-1.3.9.9/mezcla/tests/test_pandas_sklearn.py
+-rwxr-xr-x   0        0        0     1183 2023-07-03 03:15:57.263955 mezcla-1.3.9.9/mezcla/tests/test_plot_utils.py
+-rwxr-xr-x   0        0        0     2156 2023-08-08 20:42:24.883287 mezcla-1.3.9.9/mezcla/tests/test_python_ast.py
+-rwxr-xr-x   0        0        0     1735 2023-11-19 20:31:47.998747 mezcla-1.3.9.9/mezcla/tests/test_randomize_lines.py
+-rwxr-xr-x   0        0        0     2389 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_rgb_color_name.py
+-rwxr-xr-x   0        0        0      895 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_run_albert_classifier.py
+-rwxr-xr-x   0        0        0      930 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_run_bert_classifier.py
+-rwxr-xr-x   0        0        0     1602 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_show_bert_representation.py
+-rwxr-xr-x   0        0        0     2372 2023-10-24 00:05:30.113456 mezcla-1.3.9.9/mezcla/tests/test_simple_main_example.py
+-rwxr-xr-x   0        0        0     5511 2023-12-31 19:50:34.708502 mezcla-1.3.9.9/mezcla/tests/test_spacy_nlp.py
+-rwxr-xr-x   0        0        0    12822 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_spell.py
+-rwxr-xr-x   0        0        0      882 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_sys_version_info_hack.py
+-rwxr-xr-x   0        0        0    36834 2024-02-16 17:38:36.156177 mezcla-1.3.9.9/mezcla/tests/test_system.py
+-rwxr-xr-x   0        0        0     2231 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_template.py
+-rwxr-xr-x   0        0        0     5752 2023-11-07 23:03:56.586514 mezcla-1.3.9.9/mezcla/tests/test_text_categorizer.py
+-rwxr-xr-x   0        0        0     8905 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_text_processing.py
+-rwxr-xr-x   0        0        0     7361 2023-08-06 02:05:25.411349 mezcla-1.3.9.9/mezcla/tests/test_text_utils.py
+-rwxr-xr-x   0        0        0    25913 2024-02-16 17:38:36.160177 mezcla-1.3.9.9/mezcla/tests/test_tpo_common.py
+-rwxr-xr-x   0        0        0      715 2023-06-18 00:28:36.131858 mezcla-1.3.9.9/mezcla/tests/test_train_language_model.py
+-rwxr-xr-x   0        0        0     2041 2023-08-15 23:14:53.434294 mezcla-1.3.9.9/mezcla/tests/test_train_text_categorizer.py
+-rwxr-xr-x   0        0        0     4172 2023-12-23 00:35:49.682955 mezcla-1.3.9.9/mezcla/tests/test_transpose_data.py
+-rw-r--r--   0        0        0      435 2023-12-23 00:35:49.686955 mezcla-1.3.9.9/mezcla/tests/test_transpose_lines.input
+-rwxr-xr-x   0        0        0     5709 2024-02-26 23:45:37.397580 mezcla-1.3.9.9/mezcla/tests/test_unittest_wrapper.py
+-rwxr-xr-x   0        0        0     2355 2024-01-10 03:13:25.135399 mezcla-1.3.9.9/mezcla/tests/test_xml_utils.py
+-rwxr-xr-x   0        0        0      676 2023-06-18 00:29:02.186396 mezcla-1.3.9.9/mezcla/tests/tfidf/test_corpus.py
+-rwxr-xr-x   0        0        0      697 2023-06-18 00:29:02.186396 mezcla-1.3.9.9/mezcla/tests/tfidf/test_dockeyword.py
+-rwxr-xr-x   0        0        0      688 2023-06-18 00:29:02.186396 mezcla-1.3.9.9/mezcla/tests/tfidf/test_document.py
+-rwxr-xr-x   0        0        0      697 2023-06-18 00:29:02.186396 mezcla-1.3.9.9/mezcla/tests/tfidf/test_preprocess.py
+-rwxr-xr-x   0        0        0    36563 2023-11-07 23:03:56.586514 mezcla-1.3.9.9/mezcla/text_categorizer.py
+-rwxr-xr-x   0        0        0    28563 2024-02-24 00:24:18.170215 mezcla-1.3.9.9/mezcla/text_processing.py
+-rwxr-xr-x   0        0        0    13236 2024-02-18 02:11:59.716346 mezcla-1.3.9.9/mezcla/text_utils.py
+-rwxr-xr-x   0        0        0      375 2023-12-13 03:20:36.066992 mezcla-1.3.9.9/mezcla/tfidf/__init__.py
+-rwxr-xr-x   0        0        0      777 2023-11-25 07:31:25.091092 mezcla-1.3.9.9/mezcla/tfidf/config.py
+-rwxr-xr-x   0        0        0    19427 2023-12-25 20:30:57.995670 mezcla-1.3.9.9/mezcla/tfidf/corpus.py
+-rwxr-xr-x   0        0        0     3146 2023-12-13 03:20:36.070992 mezcla-1.3.9.9/mezcla/tfidf/dockeyword.py
+-rwxr-xr-x   0        0        0     7925 2023-12-13 03:20:36.070992 mezcla-1.3.9.9/mezcla/tfidf/document.py
+-rwxr-xr-x   0        0        0    19704 2024-02-24 01:15:02.034525 mezcla-1.3.9.9/mezcla/tfidf/preprocess.py
+-rw-r--r--   0        0        0     3961 2023-12-13 03:20:36.070992 mezcla-1.3.9.9/mezcla/tfidf/tests/misc_test.py
+-rwxr-xr-x   0        0        0    60411 2024-01-10 03:13:25.139399 mezcla-1.3.9.9/mezcla/tpo_common.py
+-rwxr-xr-x   0        0        0     5272 2023-12-23 00:35:49.686955 mezcla-1.3.9.9/mezcla/train_language_model.py
+-rwxr-xr-x   0        0        0     5149 2023-08-15 23:14:53.434294 mezcla-1.3.9.9/mezcla/train_text_categorizer.py
+-rwxr-xr-x   0        0        0     6673 2023-10-16 22:30:24.473638 mezcla-1.3.9.9/mezcla/transpose_data.py
+-rwxr-xr-x   0        0        0    27371 2024-02-26 23:42:50.612807 mezcla-1.3.9.9/mezcla/unittest_wrapper.py
+-rwxr-xr-x   0        0        0     3543 2023-06-18 00:28:36.139858 mezcla-1.3.9.9/mezcla/xml_utils.py
+-rw-r--r--   0        0        0      432 2024-01-10 03:13:25.139399 mezcla-1.3.9.9/non-binary-requirements.txt
+-rw-r--r--   0        0        0      803 2024-02-27 21:18:43.570553 mezcla-1.3.9.9/pyproject.toml
+-rw-r--r--   0        0        0      750 2024-01-10 03:13:25.139399 mezcla-1.3.9.9/required-packages.txt
+-rw-r--r--   0        0        0     3737 2024-02-05 04:51:35.245886 mezcla-1.3.9.9/requirements.txt
+lrwxr-xr-x   0        0        0        0 2023-11-20 19:32:33.112667 mezcla-1.3.9.9/run_tests.bash -> tools/run_tests.bash
+-rwxr-xr-x   0        0        0     1943 2024-02-27 21:18:43.570553 mezcla-1.3.9.9/setup.py
+-rwxr-xr-x   0        0        0    45023 2023-06-18 00:28:36.139858 mezcla-1.3.9.9/temp/simple_batspp.py
+-rw-r--r--   0        0        0     1382 2024-02-24 23:00:50.169992 mezcla-1.3.9.9/tools/_temp_test_settings.bash
+-rwxr-xr-x   0        0        0     3002 2024-01-10 03:26:05.393620 mezcla-1.3.9.9/tools/local-workflows.sh
+-rwxr-xr-x   0        0        0     3770 2024-02-24 23:04:45.025995 mezcla-1.3.9.9/tools/run_tests.bash
+-rw-r--r--   0        0        0      612 2023-06-18 00:28:36.139858 mezcla-1.3.9.9/tox.ini
+-rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 mezcla-1.3.9.9/PKG-INFO
```

### Comparing `mezcla-1.3.9.8/.coveragerc` & `mezcla-1.3.9.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/.github/workflows/act.yml` & `mezcla-1.3.9.9/.github/workflows/act.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/.github/workflows/debug.yml` & `mezcla-1.3.9.9/.github/workflows/debug.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/.github/workflows/github.yml` & `mezcla-1.3.9.9/.github/workflows/github.yml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/.gitignore` & `mezcla-1.3.9.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 # Backup file
 **/*.bak
 **/backup/
 
 # Old or archived files
 **/old
-**/archive
+## OLD: **/archive
 
 # Output, log-file directories, etc.
 **/log-files
 **/output-files
 **/downloads
 **/cache
```

### Comparing `mezcla-1.3.9.8/Dockerfile` & `mezcla-1.3.9.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/LICENSE.txt` & `mezcla-1.3.9.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/README.txt` & `mezcla-1.3.9.9/README.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 ﻿Note: This is an upgrade of the misc-utility repository with Python 2 support being phased out.
 
 Miscellaneous Python scripts developed over the course of several independent consulting projects. This also includes some code samples I adapted from publicly available source. (The code is not proprietary in nature. For example, it was not "borrowed" from proprietary source files, nor based on proprietary processes.)
 
 Spoiler alter: this is not "Pythonic python": I'm more into R&D than production programming. Nonetheless, there's a some useful scripts here, so I made the repository available. It is public in the spirit of open source software. 
- 
+
+This is a companion script to shell-scripts from Github:
+     https://github.com/tomasohara/shell-scripts
+
 This repository is licensed under the GNU Lesser General Public Version 3 (LGPLv3). See LICENSE.txt.
 
 Tom O'Hara
 May 2021
```

### Comparing `mezcla-1.3.9.8/mezcla/__init__.py` & `mezcla-1.3.9.9/mezcla/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from mezcla import *
     debug.trace(TL.DEFAULT, "Hey")
     debug.trace(TL.DETAILED, "Joe")
 
 Tom O'Hara
 Feb 2022
 """
-version = "1.3.9.8"
+version = "1.3.9.9"
 __VERSION__ = version
 __version__ = __VERSION__
 
 # Standard module(s)
 import sys
 
 # Note: requires python 3 or higher
```

### Comparing `mezcla-1.3.9.8/mezcla/__main__.py` & `mezcla-1.3.9.9/mezcla/__main__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/analyze_tfidf.py` & `mezcla-1.3.9.9/mezcla/analyze_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/audio.py` & `mezcla-1.3.9.9/mezcla/audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/bash_ast.py` & `mezcla-1.3.9.9/mezcla/bash_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/bert_multi_classification.py` & `mezcla-1.3.9.9/mezcla/bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/bert_text_classification.py` & `mezcla-1.3.9.9/mezcla/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/bing_search.py` & `mezcla-1.3.9.9/mezcla/bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/check_html_javascript.py` & `mezcla-1.3.9.9/mezcla/check_html_javascript.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/compute_tfidf.py` & `mezcla-1.3.9.9/mezcla/compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/convert_emoticons.py` & `mezcla-1.3.9.9/mezcla/convert_emoticons.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/cut.py` & `mezcla-1.3.9.9/mezcla/cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/data_utils.py` & `mezcla-1.3.9.9/mezcla/data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/debug.py` & `mezcla-1.3.9.9/mezcla/debug.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 # note: INDENT0 is left margin and INDENT1 is normal indent
 INDENT0 = ""
 INDENT1 = "    "
 INDENT = INDENT1
 MISSING_LINE = "???"
 
 # Globals
-max_trace_value_len = 512
+max_trace_value_len = 1024
 
 #...............................................................................
 # Utility functions
 
 def docstring_parameter(**kwargs):
     """Decorator to reformat docstring using specified KWARGS"""
     # based on https://stackoverflow.com/questions/10307696/how-to-put-a-variable-into-python-docstring/71377925#71377925
@@ -542,15 +542,15 @@
         for expression, value in zip_longest(expressions, values):
             try:
                 # Exclude kwarg params
                 match = re.search(r"^(\w+)=", str(expression))
                 if (match and match.group(1) in kwargs):
                     continue
                 assertion((not ((value is not None) and (expression is None))),
-                          "Warning: Likely problem resolving expression text (try reworking trace_expr call)")
+                          f"Warning: Likely problem resolving expression text (try reworking trace_expr call at {filename}:{line_number})")
                 value_spec = format_value(repr(value) if use_repr else value,
                                           max_len=max_len)
                 trace(level, f"{expression}={value_spec}{delim}", no_eol=no_eol)
             except:
                 trace_fmtd(ALWAYS, "Exception tracing values in trace_expr: {exc}",
                        exc=sys.exc_info())
```

### Comparing `mezcla-1.3.9.8/mezcla/docs/audio_uml.svg` & `mezcla-1.3.9.9/mezcla/docs/audio_uml.svg`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/alt_sklearn_plot_precision_recall.py` & `mezcla-1.3.9.9/mezcla/examples/alt_sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/brownlee_ml_metrics.py` & `mezcla-1.3.9.9/mezcla/examples/brownlee_ml_metrics.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/consume_all_memory.py` & `mezcla-1.3.9.9/mezcla/examples/consume_all_memory.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/download_user_gist.py` & `mezcla-1.3.9.9/mezcla/examples/download_user_gist.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/dump_checkpoints.py` & `mezcla-1.3.9.9/mezcla/examples/dump_checkpoints.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/encoded-iris.csv` & `mezcla-1.3.9.9/mezcla/examples/encoded-iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/feature_importance.py` & `mezcla-1.3.9.9/mezcla/examples/feature_importance.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/fuzzy-testing-1-2-3.wav` & `mezcla-1.3.9.9/mezcla/examples/fuzzy-testing-1-2-3.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/hf_stable_diffusion.py` & `mezcla-1.3.9.9/mezcla/examples/hf_stable_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,16 +160,17 @@
         debug.trace_expr(5, word_list)
     debug.trace(5, "out hf_stable_diffusion.init")
 
 
 def show_gpu_usage(level=TL.DETAILED):
     """Show usage for GPU memory, etc.
     TODO: support other types besides NVidia"""
-    debug.trace(level, "GPU usage")
-    debug.trace(level, gh.run("nvidia-smi"))
+    if USE_HF_API:
+        debug.trace(level, "GPU usage")
+        debug.trace(level, gh.run("nvidia-smi"))
 
 #-------------------------------------------------------------------------------
 # Main Stable Diffusion support
 
 class StableDiffusion:
     """Class providing Stable Diffusion generative AI (e.g., text-to-image)"""
 
@@ -1070,15 +1071,15 @@
     # Parse command line argument, show usage if --help given
     # TODO? auto_help=False
     main_app = Main(description=__doc__,
                     ## OLD: skip_input=True,
                     boolean_options=[(BATCH_ARG, "Use batch mode--no UI"),
                                      (SERVER_ARG, "Run flask server"),
                                      (UI_ARG, "Show user interface"),
-                                     ## TODO?: (TXT2IMG_ARG, "Run text-to-image"),
+                                     (TXT2IMG_ARG, "Run text-to-image--the default"),
                                      (IMG2IMG_ARG, "Run image-to-image"),
                                      (IMG2TXT_ARG, "Run image-to-text: clip interrogator")],
                     text_options=[(PROMPT_ARG, "Positive prompt"),
                                   (NEGATIVE_ARG, "Negative prompt"),
                                   ## OLD: (IMAGE_ARG, "Filename for img2img input image")
                                   ],
                     int_options=[(GUIDANCE_ARG, GUIDANCE_HELP)],
@@ -1091,17 +1092,17 @@
     batch_mode = main_app.get_parsed_option(BATCH_ARG, BATCH_MODE_DEFAULT)
     server_mode = main_app.get_parsed_option(SERVER_ARG)
     ## OLD: ui_mode = main_app.get_parsed_option(UI_ARG, not (batch_mode or server_mode))
     ui_mode = main_app.get_parsed_option(UI_ARG)
     prompt = main_app.get_parsed_option(PROMPT_ARG, PROMPT)
     negative_prompt = main_app.get_parsed_option(NEGATIVE_ARG, NEGATIVE_PROMPT)
     guidance = main_app.get_parsed_option(GUIDANCE_ARG, GUIDANCE_SCALE)
-    ## TODO?: use_txt2img = main_app.get_parsed_option(TXT2IMG_ARG, USE_TXT2IMG)
     use_img2img = main_app.get_parsed_option(IMG2IMG_ARG, USE_IMG2IMG)
     use_img2txt = main_app.get_parsed_option(IMG2TXT_ARG, USE_IMG2TXT)
+    use_txt2img = main_app.get_parsed_option(TXT2IMG_ARG, not (use_img2img or use_img2txt))
     ## OLD: input_image_file = main_app.get_parsed_option(IMAGE_ARG)
     denoising_factor = main_app.get_parsed_option(DENOISING_ARG)
     ## TODO?: debug.assertion(use_txt2img ^ use_img2img)
     # TODO2: BASENAME and NUM_IMAGES (options)
     ## TODO: x_mode = main_app.get_parsed_option(X_ARG)
     debug.assertion(not (batch_mode and server_mode))
```

### Comparing `mezcla-1.3.9.8/mezcla/examples/hugging_face_speechrec.py` & `mezcla-1.3.9.9/mezcla/examples/hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/hugging_face_translation.py` & `mezcla-1.3.9.9/mezcla/examples/hugging_face_translation.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 ## TODO: import json
 
 # Intalled modules
 # Note: done dynamically below
 
 # Local modules
 from mezcla import debug
-from mezcla.main import Main
+from mezcla.main import Main, USE_PARAGRAPH_MODE
 # TODO2: add new mezcla.hugging_face module for common stuff
 import mezcla.examples.hugging_face_speechrec as hf_speechrec
 from mezcla import misc_utils
+from mezcla.my_regex import my_re
 from mezcla import system
 from mezcla import glue_helpers as gh
 
 # Constants and Environment options
 TL = debug.TL
 
 FROM = system.getenv_text("FROM", "es")
@@ -60,22 +61,31 @@
 TEXT_FILE = system.getenv_text("TEXT_FILE", "-",
                                "Text file to translate")
 USE_INTERFACE = system.getenv_bool("USE_INTERFACE", False,
                                    "Use web-based interface via gradio")
 
 #-------------------------------------------------------------------------------
 
+def show_gpu_usage(trace_level=None):
+    """Show nvidia usage if under GPU"""
+    if trace_level is None:
+        trace_level = 5
+    if (hf_speechrec.TORCH_DEVICE == "GPU"):
+        debug.code(trace_level, lambda: debug.trace(1, gh.run("nvidia-smi")))
+    return
+
+
 def main():
     """Entry point"""
     debug.trace(TL.USUAL, f"main(): script={system.real_path(__file__)}")
 
     # Show simple usage if --help given
     dummy_app = Main(description=__doc__.format(script=gh.basename(__file__)),
                      skip_input=False, manual_input=True,
-                     bool_options=[
+                     boolean_options=[
                          ## TODO3: (ELAPSED_ARG, "Show elapsed time")],
                          (UI_ARG, "Invoke user interface")],
                      text_options=[
                          (FROM_ARG, "Source language code"),
                          (TO_ARG, "Target language code"),
                          (TASK_ARG, "Translation task"),
                          (MODEL_ARG, "Model for translation"),
@@ -128,25 +138,27 @@
             ## TODO3: examples=[...]); See example in hf_stable_diffusion.py.
             )
         pipeline_if.launch()
 
     # Otherwise, do translation and output
     else:
         TRANSLATION_TEXT = "translation_text"
-        try:
-            translation = model(text, max_length=MAX_LENGTH)
-            debug.assertion(isinstance(translation, list)
-                            and (TRANSLATION_TEXT in translation[0]))
-            print(translation[0].get(TRANSLATION_TEXT) or "")
-        except:
-            system.print_exception_info("translation")
+        split_regex = r"\n\s*\n" if USE_PARAGRAPH_MODE else "\n"
+        for segment in my_re.split(split_regex, text):
+            try:
+                translation = model(segment, max_length=MAX_LENGTH)
+                debug.assertion(isinstance(translation, list)
+                                and (TRANSLATION_TEXT in translation[0]))
+                print(translation[0].get(TRANSLATION_TEXT) or "")
+            except:
+                system.print_exception_info("translation")
+            show_gpu_usage()
 
-    # Show nvidia usage if under GPU
-    if (hf_speechrec.TORCH_DEVICE == "GPU"):
-        debug.code(5, lambda: debug.trace(1, gh.run("nvidia-smi")))
+    # Wrap up
+    show_gpu_usage()
     return
 
 #-------------------------------------------------------------------------------
 
 if __name__ == '__main__':
     elapsed = misc_utils.time_function(main)
     if SHOW_ELAPSED:
```

### Comparing `mezcla-1.3.9.8/mezcla/examples/inspect_checkpoint.py` & `mezcla-1.3.9.9/mezcla/examples/inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/iris.csv` & `mezcla-1.3.9.9/mezcla/examples/iris.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/pima-indians-diabetes.csv` & `mezcla-1.3.9.9/mezcla/examples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/plot_forest_importances.py` & `mezcla-1.3.9.9/mezcla/examples/plot_forest_importances.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/resources/translate_es_25.txt` & `mezcla-1.3.9.9/mezcla/examples/resources/translate_es_25.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/resources/us1.wav` & `mezcla-1.3.9.9/mezcla/examples/resources/us1.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/resources/us10.wav` & `mezcla-1.3.9.9/mezcla/examples/resources/us10.wav`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/sd-spooky-pacman.png` & `mezcla-1.3.9.9/mezcla/examples/sd-spooky-pacman.png`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/sklearn_plot_precision_recall.py` & `mezcla-1.3.9.9/mezcla/examples/sklearn_plot_precision_recall.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/template.py` & `mezcla-1.3.9.9/mezcla/examples/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,16 +54,16 @@
                     skip_input=False)
     debug.assertion(main_app.parsed_args)
     ## TODO_OPT1 = main_app.get_parsed_option(TODO_OPT1)
 
     ## TODO:
     system.print_error("Error: Implement me!")
     ## ALT TODO:
-    ## for line in map_app.read_entire_input():
-    ##     print(modify_fn(line))
+    ## for line in main_app.read_entire_input().splitlines():
+    ##     print(TODO_fn(line))
     return
 
 #-------------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context(level=TL.QUITE_VERBOSE)
     main()
```

### Comparing `mezcla-1.3.9.8/mezcla/examples/tensorflow_matrix_multiply.py` & `mezcla-1.3.9.9/mezcla/examples/tensorflow_matrix_multiply.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/tests/test_hf_stable_diffusion.py` & `mezcla-1.3.9.9/mezcla/examples/tests/test_hf_stable_diffusion.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 #
 # Notes:
 # - This can be run as follows:
 #   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_hf_stable_diffusion.py
 #
 # TODO3: check image attributes (e.g., backgfround color) and work in image classification (e.g., box)
 #
+#--------------------------------------------------------------------------------
+# Note:
+# - This only runs if NVidia GPU support is installed OK, as determined via nvidia-smi output.
+#   $ nvidia-smi
+#   Fri Jan 26 12:51:57 2024       
+#   +---------------------------------------------------------------------------------------+
+#   | NVIDIA-SMI 535.98                 Driver Version: 535.98       CUDA Version: 12.2     |
+#   ...
+#   |   0  NVIDIA GeForce RTX 3080        Off | 00000000:01:00.0 Off |                  N/A |
+#   |  0%   42C    P8              28W / 320W |    677MiB / 10240MiB |      0%      Default |
+#   ...
+#
 
 """Tests for hf_stable_diffusion module"""
 
 # Standard packages
 ## OLD: import base64
 
 # Installed packages
@@ -32,31 +44,70 @@
 from mezcla.unittest_wrapper import TestWrapper, trap_exception
 from mezcla import debug
 from mezcla import system
 from mezcla import glue_helpers as gh
 from mezcla.misc_utils import RANDOM_SEED
 from mezcla.my_regex import my_re
 
+# HACK: Makes sure low-resource GPU configuration used for tests
+system.setenv("LOW_MEMORY", "1")
+system.setenv("STREAMLINED_CLIP", "1")
+
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:                  global module object
 #    TestTemplate.script_module:  path to file
 import mezcla.examples.hf_stable_diffusion as THE_MODULE
 hfsd = THE_MODULE
 
-# Constants
+# Constants, etc.
 TORCH_SEED = system.getenv_int("TORCH_SEED", RANDOM_SEED,
                                "Random seed for torch if non-zero")
 NUMPY_SEED = system.getenv_int("NUMPY_SEED", RANDOM_SEED,
                                "Random seed for numpy if non-zero")
+#................................................................................
+# Utility functions
+
+def get_gpu_stats():
+    """
+    Note: Currently uses NVIDIA System Management Interface (SMI) program"""
+    # TODO3: use torch.cuda.memory_summary
+    result = gh.run("nvidia-smi")
+    debug.trace(7, f"get_gpu_stats() => {result}")
+    return result
+
+
+def gpu_mem_usage():
+    """Return GPU memory usage in gigabytes"""
+    # TEMP: Uses nvidia-smi until torch bug fixed
+    # ex: |  0%   42C    P8              28W / 320W |    677MiB / 10240MiB |      0%      Default |
+    total_usage = 0.0
+    for line in get_gpu_stats().splitlines():
+        if my_re.search(r"(\d+)MiB */ *(\d+)MiB", line, flags=my_re.IGNORECASE):
+            device_usage, _device_total = my_re.groups()
+            total_usage += system.to_float(device_usage)
+    total_usage /= 1024
+    debug.trace(6, f"get_gpu_stats() => {total_usage}")
+    return total_usage
+
+#................................................................................
+# Globals
+
+## TODO3: rework NVidia test via torch CUDA support
+nvidia_ok = my_re.search("NVIDIA-SMI.*Driver Version",
+                         get_gpu_stats(), flags=my_re.IGNORECASE)
+sd_or_nvidia_issue = (not (diffusers and nvidia_ok))
+
+#................................................................................
 
 class TestIt(TestWrapper):
     """Class for testcase definition"""
     script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
     use_temp_base_dir = True            # treat TEMP_BASE as directory
     # note: temp_file defined by parent (along with script_module, temp_base, and test_num)
+    init_gpu_mem_usage = gpu_mem_usage()
 
     @classmethod
     def setUpClass(cls, filename=None, module=None):
         """One-time initialization (i.e., for entire class)"""
         debug.trace(5, f"TestIt.setUpClass(); cls={cls}")
         # note: should do parent processing first
         super().setUpClass(filename, module)
@@ -88,26 +139,29 @@
             # Save to disk if debugging
             if debug.debugging():
                 temp_image_file = f"{self.temp_file}{label_spec}-{i + 1}.png"
                 debug.trace_expr(4, temp_image_file)
                 hfsd.write_image_file(temp_image_file, spec)
         return images
 
+    
+    @pytest.mark.skipif(sd_or_nvidia_issue, reason="SD or NVidia not setup")
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_00_init_stable_diffusion(self):
         """Make sure ST module gets initialized OK"""
         debug.trace(4, f"test_00_init_stable_diffusion(); self={self}")
         ## HACK: This also serves to initialize the module for other tests (TODO2: fix init)
         THE_MODULE.init_stable_diffusion()
         self.do_assert(THE_MODULE.torch is not None)
         self.do_assert(THE_MODULE.sd_instance is not None)
         self.do_assert(isinstance(THE_MODULE.sd_instance, THE_MODULE.StableDiffusion))
+        self.do_assert(self.init_gpu_mem_usage > 0)
         return
     
-    @pytest.mark.skipif(not diffusers, reason="SD diffusers package missing")
+    @pytest.mark.skipif(sd_or_nvidia_issue, reason="SD or NVidia not setup")
     def test_01_simple_generation(self):
         """Makes sure simple image generation (txt2img) works as expected"""
         debug.trace(4, f"test_01_simple_generation(); self={self}")
 
         # Run script to generate orange ball and get image filename.
         # ex: "See sd-app-image-1.png for output image(s)."
         script_output = self.run_script(
@@ -129,28 +183,28 @@
     ## TODO?
     ## #...............................................................................
     ##
     ## class TestIt2:
     ##    """Another class for testcase definition
     ##    Note: Needed to avoid error with pytest due to inheritance with unittest.TestCase via TestWrapper"""
     
-    @pytest.mark.skipif(not diffusers, reason="SD diffusers package missing")
+    @pytest.mark.skipif(sd_or_nvidia_issue, reason="SD or NVidia not setup")
     def test_02_txt2img_pipeline(self):
         """Make sure valid SD pipeline created"""
         debug.trace(4, f"test_02_txt2img_pipeline(); self={self}")
         sd = THE_MODULE.StableDiffusion(use_hf_api=True)
         pipe = sd.init_pipeline()
         actual = my_re.split(r"\W+", str(pipe))
         expect = "CLIPImageProcessor CLIPTextModel StableDiffusionSafetyChecker text_encoder".split()
         debug.trace_expr(5, actual, expect, delim="\n")
         self.do_assert(len(system.intersection(actual, expect)) > 2)
         return
     
     @pytest.mark.xfail                   # TODO: remove xfail
-    @pytest.mark.skipif(not diffusers, reason="SD diffusers package missing")
+    @pytest.mark.skipif(sd_or_nvidia_issue, reason="SD or NVidia not setup")
     def test_03_txt2img_generation(self):
         """Make sure text-to-image reasonable"""
         debug.trace(4, f"test_03_txt2img_generation(); self={self}")
         sd = THE_MODULE.StableDiffusion(use_hf_api=True)
         ## TODO: NUM_IMAGES = 2
         NUM_IMAGES = 1
         # note: generate image with high adherence guidance for prompt
@@ -158,15 +212,15 @@
         images = self.check_images(image_specs, label="txt2img")
         self.do_assert(len(images) == NUM_IMAGES)
         description = sd.infer_img2txt(image_b64=image_specs[0])
         self.do_assert(my_re.search(r"canine|dog|puppy", description))
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
-    @pytest.mark.skipif(not diffusers, reason="SD diffusers package missing")
+    @pytest.mark.skipif(sd_or_nvidia_issue, reason="SD or NVidia not setup")
     @trap_exception
     def test_04_img2img_generation(self):
         """Make sure image-to-image reasonable"""
         debug.trace(4, f"test_04_img2img_generation(); self={self}")
         sd = THE_MODULE.StableDiffusion(use_hf_api=True)
         ## TODO: NUM_IMAGES = 2
         NUM_IMAGES = 1
@@ -182,28 +236,28 @@
         images = self.check_images(image_specs, label="img2img")
         self.do_assert(len(images) == NUM_IMAGES)
         description = sd.infer_img2txt(image_b64=image_specs[0])
         self.do_assert(not my_re.search(r"canine|dog|puppy", description))
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
-    @pytest.mark.skipif(not diffusers, reason="SD diffusers package missing")
+    @pytest.mark.skipif(sd_or_nvidia_issue, reason="SD or NVidia not setup")
     @trap_exception
     def test_05_img2txt_generation(self):
         """Make sure image-to-text reasonable"""
         debug.trace(4, f"test_05_img2txt_generation(); self={self}")
         # TODO2: use common setup method (e.g., via TestWrapper)
         sd = THE_MODULE.StableDiffusion(use_hf_api=True, low_memory=True)
         PACMAC_LIKE_IMAGE = gh.resolve_path("sd-spooky-pacman.png", heuristic=True)
         pacmac_like_base64 = THE_MODULE.encode_image_file(PACMAC_LIKE_IMAGE)
         description = sd.infer_img2txt(image_b64=pacmac_like_base64)
         debug.trace_expr(5, description)
         # TODO4: assert(english-like-text(description))
         self.do_assert(not my_re.search(r"canine|dog|puppy", description))
-        debug.trace(5, "post-test_05 GPU stats:\n" + gh.run("nvidia-smi"))
+        debug.trace(5, "post-test_05 GPU stats:\n" + get_gpu_stats())
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     @pytest.mark.skipif(not extcolors, reason="extcolors package missing")
     @trap_exception
     def test_06_prompted_color(self):
         """Make sure prompted color is used in txt2img"""
@@ -220,20 +274,33 @@
         # <(255, 153, 0), orange>  :   6.13% (16074)
         color_output = gh.run(f"extcolors '{image_path}' | rgb_color_name.py - 2> /dev/null")
         debug.trace_expr(4, color_output)
         self.do_assert("orange" in color_output)
         self.do_assert(len(images) == 1)
         return
 
+    @pytest.mark.xfail                   # TODO: remove xfail
+    @pytest.mark.skipif(not extcolors, reason="extcolors package missing")
+    def test_99_gpu_mem_usage(self):
+        """Ensure at least 2gb of GPU memory used
+        Note: This should be the last test run
+        """
+        usage_before = self.init_gpu_mem_usage
+        usage_after = gpu_mem_usage()
+        usage = (usage_after - usage_before)
+        debug.trace_expr(5, usage, usage_before, usage_after)
+        self.do_assert(usage >= 2)
+    
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
     try:
         pytest.main([__file__])
     except:
         system.print_exception_info("pytest.main")
     ## TEMP (Show GPU memory usage, etc.):
     ## NOTE: maldito pytest makes debugging a real pain!
-    gpu_stats = "post test-suite GPU stats: {{\n{out}\n}}".format(out=gh.indent_lines(gh.run("nvidia-smi")))
+    gpu_stats = "post test-suite GPU stats: {{\n{out}\n}}".format(
+        out=gh.indent_lines(get_gpu_stats()))
     print(gpu_stats)
     debug.trace(3, gpu_stats)
```

### Comparing `mezcla-1.3.9.8/mezcla/examples/tests/test_hugging_face_speechrec.py` & `mezcla-1.3.9.9/mezcla/examples/tests/test_hugging_face_speechrec.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/tests/test_hugging_face_translation.py` & `mezcla-1.3.9.9/mezcla/examples/tests/test_hugging_face_translation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/tracemalloc_display.py` & `mezcla-1.3.9.9/mezcla/examples/tracemalloc_display.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/examples/youtube_transcript.py` & `mezcla-1.3.9.9/mezcla/examples/youtube_transcript.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 import youtube_transcript_api as ytt_api
 from youtube_transcript_api import formatters
 
 # Local modules
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.main import Main
+from mezcla import misc_utils
 from mezcla.my_regex import my_re
 from mezcla import system
 
 # Constants
 TL = debug.TL
 
 #-------------------------------------------------------------------------------
@@ -61,21 +62,36 @@
     """Entry point"""
     debug.trace(TL.USUAL, f"main(): script={system.real_path(__file__)}")
 
     # Parse command line options, show usage if --help given
     main_app = Main(description=__doc__.format(script=gh.basename(__file__)),
                     skip_input=False, manual_input=False)
     debug.assertion(main_app.parsed_args)
-    video_id = my_re.sub(r"(https://)?www.youtube.com/watch\?v=", "", main_app.filename)
-    debug.trace_expr(5, video_id)
+    url = main_app.filename
+    video_id= url
+    YOUTUBE_PREFIX = "https://www.youtube.com/watch?v="
+    if url.startswith(YOUTUBE_PREFIX):
+        video_id = url[len(YOUTUBE_PREFIX):]
+    else:
+        url = YOUTUBE_PREFIX + url
+    ## TODO: video_id = my_re.sub(r"(https://)?www.youtube.com/watch\?v=", "", main_app.filename)
+    debug.trace_expr(5, url, video_id)
 
     # Download the transcript and print using YouTubeLike-format
-    # note: youtube_transcript_api 
-    transcript = ytt_api.YouTubeTranscriptApi.get_transcript(video_id)
-    print(YouTubeLikeFormatter().format_transcript(transcript))
+    # note: youtube_transcript_api
+    print(misc_utils.get_formatted_date())
+    print("")
+    print(url)
+    print("")
+    try:
+        transcript = ytt_api.YouTubeTranscriptApi.get_transcript(video_id)
+        print(YouTubeLikeFormatter().format_transcript(transcript))
+    except:
+        system.print_exception_info("transcript access")
+        print("n/a")
 
     return
 
 #-------------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context(level=TL.QUITE_VERBOSE)
```

### Comparing `mezcla-1.3.9.8/mezcla/extract_document_text.py` & `mezcla-1.3.9.9/mezcla/extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/file_utils.py` & `mezcla-1.3.9.9/mezcla/file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/filter_random.py` & `mezcla-1.3.9.9/mezcla/filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/format_profile.py` & `mezcla-1.3.9.9/mezcla/format_profile.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,31 +22,25 @@
 #
 # This method modifies the Stats object by sorting it according to the
 # supplied criteria. The argument is typically a string identifying
 # the basis of a sort (example: 'time' or 'name').
 #
 # Valid Arg    Meaning
 # 'calls'      call count
-# 'cumulative' cumulative time
 # 'cumtime'    cumulative time
-# 'file'       file name
 # 'filename'   file name
 # 'module'     file name
 # 'ncalls'     call count
 # 'pcalls'     primitive call count
 # 'line'       line number
 # 'name'       function name
 # 'nfl'        name/file/line
 # 'stdname'    standard name
-# 'time'       internal time
 # 'tottime'    internal time
 #
-# Note: following apply to version 2.7 or later
-# - cumtime, filename, ncalls, tottime
-#
 
 """Displays result of python profiling"""
 
 #------------------------------------------------------------------------
 # Library packages
 
 # Standard packages
@@ -56,33 +50,33 @@
 # Local packages
 from mezcla import debug
 ## OLD: from tpo_common import *
 from mezcla.system import getenv_text, print_stderr
 
 ## OLD: PROFILE_KEY = getenv_text("PROFILE_KEY", "cumulative")
 PROFILE_KEY = getenv_text("PROFILE_KEY", "cumulative",
-                          "Sort key (e.g., calls, cumulative, file, time)")
+                          "Sort key (e.g., cumtime, filename, ncalls, tottime)")
 
 #------------------------------------------------------------------------
 # Functions
 
 def usage():
     """Displays usage notes for script"""
     print_stderr("""
 
 Usage: {program} profile-log
 
 Notes:
 - use PROFILE_KEY to over default sorting (cumulative)
 - main keys: 
-       calls, cumulative, file, time
+       cumtime, filename, ncalls, tottime
 - other keys: 
        module, pcalls, line, name, nfl, stdname
-- 2.7+ keys: 
-       cumtime, filename, ncalls, tottime
+- alternative keys:
+       calls, cumulative, file, time
 - unfortunately, memory profiling is not supported
 - see http://docs.python.org/3/library/profile.html
 
 Example (assumes bash):
     $ python -m cProfile -o profile.data fubar.py
     $ PROFILE_KEY=calls {program} profile.data
```

### Comparing `mezcla-1.3.9.8/mezcla/gensim_test.py` & `mezcla-1.3.9.9/mezcla/gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/glue_helpers.py` & `mezcla-1.3.9.9/mezcla/glue_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #! /usr/bin/env python
 #
 # Utility functions for writing glue scripts, such as implementing functionality
 # available in Unix scripting (e.g., basename command).
 #
 # NOTE:
-# - *** This module is being phased out with important functionality being moved elsewhere.
 # - Some of the utilities are specific to Unix (e.g., full_mkdir and real_path). In
 #   contrast, system.py attempts to be more cross platform.
+# - ** It can be confusing debugging script that use run, because the trace level
+#  is raised by default. To disable this, set the SUB_DEBUG_LEVEL as follows:
+#     l=5; DEBUG_LEVEL=$l SUB_DEBUG_LEVEL=$l merge_files.py ...
+# - Also see ALLOW_SUBCOMMAND_TRACING usage below and in unittest_wrapper.py.
 #
 # TODO:
 # - Add more functions to facilitate command-line scripting (check bash scripts for commonly used features).
 # - Add functions to facilitate functional programming (e.g., to simply debugging traces).
 #
 
 """Helpers gluing scripts together
@@ -229,21 +232,27 @@
         debug.assertion(" " not in path)
         path = run(f"find {base_dir} -name '{path}'")
             
     debug_format("resolve_path({f}) => {p}", 4, f=filename, p=path)
     return path
 
 
-def form_path(*filenames):
+def form_path(*filenames, create=False):
     """Wrapper around os.path.join over FILENAMEs (with tracing)
     Note: includes sanity check about absolute filenames except for first
-    Warning: This will be deprecated: uses system.form_path instead.
+    If CREATE, then the directory for the path is created if needed
+    Warning: This might be deprecated: use system.form_path instead.
     """
     ## TODO3: return system.form_path(*filenames)
     debug.assertion(not any(f.startswith(system.path_separator()) for f in filenames[1:]))
+    if create:
+        path_dir = os.path.join(filenames[:-1])
+        if not system.file_exists(path_dir):
+            full_mkdir(path_dir)
+
     path = os.path.join(*filenames)
     debug_format("form_path{f} => {p}", 6, f=tuple(filenames), p=path)
     return path
 
 
 def is_directory(path):
     """Determins wther PATH represents a directory"""
```

### Comparing `mezcla-1.3.9.8/mezcla/html_utils.py` & `mezcla-1.3.9.9/mezcla/html_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -747,16 +747,16 @@
     return value_spec
 #
 # EX: format_url_param("r") => ""
 # EX: format_url_param("r", "R") => "R"
 
 
 def format_input_field(param_name : str, label: Optional[str] = None, skip_capitalize=None,
-                       default_value: Optional[str] = None, max_len : Optional[int] = None
-                       , size : Optional[int] = None, disabled : Optional[int] = None,
+                       default_value: Optional[str] = None, max_len : Optional[int] = None,
+                       size : Optional[int] = None, disabled : Optional[int] = None,
                        style: Optional[str] = None, misc_attr: Optional[str] = None,
                        tooltip: Optional[str] = None, text_area: Optional[str] = None,
                        num_rows : Optional[int] = None, on_change: Optional[str] = None):
     """Returns HTML specification for input field, optionally with LABEL, SKIP_CAPITALIZE, DEFAULT_VALUE, MAX_LEN, SIZE, DISABLED, CSS STYLE, MISC_ATTR (catch all), and NUM_ROWS.    
     Note:
     - param_name + "-id" is used for the field ID.
     - SIZE should be specified if not same as MAX_LEN.
@@ -786,31 +786,31 @@
     misc_spec += (f"onchange={on_change}" if on_change else "")
     tooltip_start_spec = tooltip_end_spec = ""
     if tooltip:
         tooltip_start_spec = f'<span class="tooltip-control"><span class="tooltip-field">{tooltip}</span>'
         tooltip_end_spec = "</span>"
     result = f'<label>{tooltip_start_spec}{label}{tooltip_end_spec}&nbsp;'
     if text_area:
-        max_len_spec = (f"maxlength={max_len}" if max_len else "")
+        max_len_spec = (f'maxlength="{max_len}"' if max_len else "")
         value_spec = format_url_param(param_name)
         result += f'<textarea id="{param_name}-id" name="{param_name}" rows={num_rows} {style_spec} {max_len_spec} {disabled_spec} {misc_spec}>{value_spec}</textarea>'
     else:
         ## OLD: max_len_spec = (f"maxlength={max_len} size={max_len}" if max_len else "")
         len_spec = ""
         if max_len:
-            len_spec += f" maxlength={max_len}"
+            len_spec += f' maxlength="{max_len}"'
         if size:
-            len_spec += f" size={size}"
+            len_spec += f' size="{size}"'
         result += f'<input id="{param_name}-id" value="{value_spec}" name="{param_name}" {style_spec} {len_spec} {disabled_spec} {misc_spec}>'
     result += "</label>"
         
     debug.trace(6, f"format_input_field({param_name}, ...) => {result}")
     return result
 #
-# EX: format_input_field("num-id", label="Num", max_len=3) => '<label>Num&nbsp;<input id="num-id-id" value="" name="num-id"  maxlength=3 size=3  ></label>'
+# EX: format_input_field("num-id", label="Num", max_len=3) => '<label>Num&nbsp;<input id="num-id-id" value="" name="num-id"  maxlength="3" size="3"  ></label>'
 
 #-------------------------------------------------------------------------------
 # TEMP: Code previously in other modules
 # TODO3: move above according to some logical grouping
 
 def escape_html_text(text : str):
     """Add entity encoding to TEXT to make suitable for HTML"""
```

### Comparing `mezcla-1.3.9.8/mezcla/ipython_utils.py` & `mezcla-1.3.9.9/mezcla/ipython_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/kenlm_example.py` & `mezcla-1.3.9.9/mezcla/kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/keras_param_search.py` & `mezcla-1.3.9.9/mezcla/keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/main.py` & `mezcla-1.3.9.9/mezcla/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,17 @@
 TEMP_FILE = gh.TEMP_FILE
 KEEP_TEMP_FILES = system.getenv_bool("KEEP_TEMP_FILES", debug.detailed_debugging(),
                                      "Retain temporary files")
 INPUT_ERROR_OPTION = "input_error"
 INPUT_ERROR = system.getenv_value(
     INPUT_ERROR_OPTION.upper(), None,
     description="Override for strict input processing error handling")
+DISABLE_RECURSIVE_DELETE = system.getenv_value(
+    "DISABLE_RECURSIVE_DELETE", None,
+    description="Disable use of potentially dangerous rm -r style recursive deletions")
 
 #-------------------------------------------------------------------------------
 
 class Main(object):
     """Class encompassing common script processing"""
     argument_parser = None
     force_unicode = False
@@ -290,15 +293,15 @@
         self.temp_file = (TEMP_FILE or default_temp_file)
 
         # Note: --help assumed for input-less scripts with command line options
         # to avoid inadvertent script processing.
         #
         if ((runtime_args is None) and (not skip_args)):
             # note: there is a quirk when using this with pytest
-            debug.assertion(sys.argv[1:] != "pytest")
+            debug.assertion(sys.argv[0] != "pytest")
             runtime_args = sys.argv[1:]
             debug.trace(4, f"Using sys.argv[1:] for runtime args: {runtime_args}")
             if self.auto_help and not runtime_args:
                 help_arg = (USAGE_ARG if self.brief_usage else HELP_ARG)
                 debug.trace(4, f"FYI: Adding {help_arg} to command line (as per auto_help)")
                 runtime_args = [help_arg]
         #
@@ -736,14 +739,16 @@
         self.init_input()
         try:
             # If not automatic input, process the main step of script
             if self.manual_input:
                 self.run_main_step()
             # Otherwise have client process input line by line
             else:
+                debug.assertion(not self.skip_input)
+
                 # TODO: Trace status only if script blocks waiting for user
                 if not QUIET_MODE:
                     debug.trace(2, "Processing input")
                 self.process_input()
         except BrokenPipeError:
             ## TODO: exit gracefully (e.g., after wrap_up)
             ## debug.trace_fmt(6, "Silly exception processing input: {exc}", 
@@ -946,15 +951,22 @@
         if not KEEP_TEMP_FILES:
             ## TODO2: 3=>6
             debug.trace_fmt(4, "Deleting any temporary files: {files}",
                             files=gh.run(f"echo {self.temp_base}* {self.temp_file}* | sort -u"))
                                 
             # Remove all temp_base* files (or the temp_base directory)
             if self.use_temp_base_dir:
-                gh.run("rm -rvf {dir}", dir=self.temp_base)
+                ## OLD: gh.run("rm -rf {dir}", dir=self.temp_base)
+                if DISABLE_RECURSIVE_DELETE:
+                    debug.trace(4, f"FYI: Only deleting top-level files in {self.temp_base} to avoid potentially dangerous rm -r")
+                    gh.run("rm -f {dir}/* {dir}/.*", dir=self.temp_base)
+                    gh.run("rm -f {dir}", dir=self.temp_base)
+                else:
+                    debug.trace(4, f"FYI: Using potentially dangerous rm -r over {self.temp_base}")
+                    gh.run("rm -rvf {dir}", dir=self.temp_base)
             else:
                 gh.run("rm -vf {file}*", file=self.temp_base)
             # Likewise remove all temp_file* files
             if (self.temp_file != self.temp_base):
                 gh.run("rm -vf {file}*", file=self.temp_file)
         return
 
@@ -966,13 +978,28 @@
 
 dummy_app = Main([])
 
 debug.trace_current_context(8, "main.py context")
 
 #------------------------------------------------------------------------
 
-if __name__ == "__main__":
-    system.print_stderr(f"Warning: {__file__} is not intended to be run standalone\n")
+def main():
+    """Entry point"""
+    class VacuousMain(Main):
+        """Sub-class that does nothing"""
+        # Note: complexity is for handle python running script from shell-scripts repo
+        #     run-python-sript"
+
+        def run_main_step(self):
+            print("No-op main step")
+            
     # note: Following used for argument parsing
-    main = Main(description=__doc__)
-    main.run()
+    ## OLD: main = Main(description=__doc__)
+    ## NOTE: That hangs with run-python-script main.py
+    main_app = VacuousMain(description=__doc__, skip_input=True, manual_input=True)
+    ## TODO3: main.run_main_step = lambda self: print("No-op main step")
+    main_app.run()
 
+
+if __name__ == "__main__":
+    system.print_stderr(f"Warning: {__file__} is not intended to be run standalone\n")
+    main()
```

### Comparing `mezcla-1.3.9.8/mezcla/merge_files.py` & `mezcla-1.3.9.9/mezcla/merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/merge_notes.py` & `mezcla-1.3.9.9/mezcla/merge_notes.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,17 +62,14 @@
 from mezcla import debug
 from mezcla.my_regex import my_re
 from mezcla import system
 
 SKIP_BOM = system.getenv_bool("SKIP_BOM", False,
                               "Don't output byte order mark U+FEFF")
 
-## TEMP: quiet picky pylint
-# pylint: disable=consider-using-f-string
-
 #...............................................................................
 
 def resolve_date(textual_date, default_date=None):
     """Converts from textual DATE into datetime object (using optional DEFAULT value)"""
     # TODO: """... Supports following date formats: [WWW] dd MMM YY[YY]"
     # ALSO: clarify that default date used after parsing errors
     #
@@ -110,15 +107,14 @@
     parser = argparse.ArgumentParser(description="Merges ascii notes files")
     parser.add_argument("--ignore-dividers", default=False, action='store_true', help="Ignore lines consisting soley of dashes")
     parser.add_argument("--output-dividers", default=False, action='store_true', help="Output divider lines (80 dashes) betweens sections for different days")
     parser.add_argument("--show-file-info", default=False, action='store_true', help="Include filename and line number of original file in output")
     parser.add_argument("filename", nargs='+', default='-', help="Input filename")
     args = vars(parser.parse_args())
     debug.trace(5, "args = %s" % args)
-    ## OLD: input_files = args['filename']
     full_input_files = args['filename']
     ignore_dividers = args['ignore_dividers']
     output_dividers = args['output_dividers']
     show_file_info = args['show_file_info']
 
     # Initial defaults
     # note: initializes current date to dummy from way back when
@@ -147,15 +143,14 @@
     if sys.version_info.major > 2:
         hook_utf8_replace = fileinput.hook_encoded('UTF-8', errors='replace')
     has_new_date = False
     for line in fileinput.input(input_files, openhook=hook_utf8_replace):
         line_num += 1
         # Note: strips leading and trailing spaces from line to facilitate regex
         # pattern matching, with raw line saved as original_line.
-        ## OLD: line = line.strip("\n")
         original_line = line.strip("\n")
         line = line.strip()
         debug.trace(6, "L%d: %s" % (line_num, line))
 
         # Reset default date if first line in file
         if fileinput.isfirstline():
             debug.trace_fmtd(4, "new file: {f}", f=fileinput.filename())
@@ -178,18 +173,16 @@
         new_date = last_date
         new_resolved_date = last_resolved_date
         # Ensure days of the week are abbreviated (with no more than 3 letters)
         line = re.sub(r"^(Sun|Mon|Tue|Wed|Thu|Fri|Sat)\w+day", r"\1", line, flags=re.IGNORECASE)
         line = re.sub(r"^(Tue)s (\d)", r"\1 \2", line, flags=re.IGNORECASE)
         line = re.sub(r"^(Thu)rs? (\d)", r"\1 \2", line, flags=re.IGNORECASE)
         # TODO: Ensure months are abbreviated
-        ## line = re.sub(r" (\d+) (Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\w* (\d+)", r" \1 \2 \3", line, flags=re.IGNORECASE)
-        ## OLD: if (re.search(r"^([a-z][a-z][a-z] )?\d+ [a-z][a-z][a-z] \d+$", line, flag=re.IGNORECASE)):
+        ## EX: line = re.sub(r" (\d+) (Jan|Feb|Mar|Apr|May|Jun|Jul|Aug|Sep|Oct|Nov|Dec)\w* (\d+)", r" \1 \2 \3", line, flags=re.IGNORECASE)
         if (my_re.search(r"^([a-z][a-z][a-z] )?\d+ [a-z][a-z][a-z] \d+$", line, re.IGNORECASE)):
-            ## OLD: new_date = line.strip()
             new_date = my_re.group(0)
             needs_source_info = True
             has_new_date = True
 
             # Resolve date format, adding to hash if not already there
             # TODO: if not resolvable, report file and line number
             if new_date not in resolved_date:
@@ -208,22 +201,21 @@
             debug.trace_fmtd(5, "New date at line {n}: raw={raw}; resolved={new}\n", 
                              n=line_num, raw=new_date, new=new_resolved_date)
         else:
             debug.trace_fmt(7, "Ignoring non-date in date check at line {n}", n=line_num)
                             
         # Add optional source indicator to current date
         if show_file_info and needs_source_info:
-            notes_hash[new_date] += "[src={f}:{n}]\n".format(f=fileinput.filename(), 
+            notes_hash[new_date] += "[src: {f}:{n}]\n".format(f=fileinput.filename(), 
                                                              n=fileinput.filelineno())
             needs_source_info = False
                 
         # Add line to notes for current date
         # TODO: use resolved date as key so different specifications for same date output together without new date spec
         debug.assertion((not has_new_date) or (new_date != dummy_date))
-        ## notes_hash[new_date] += line + "\n"
         notes_hash[new_date] += original_line + "\n"
         has_new_date = False
 
     # Print the note entries sorted by resolved date.
     # Note:
     # - The sorting is based on the datetime.datetime type. If an error
     #   occurs, the problem might be due to the resolve_date function
@@ -234,35 +226,29 @@
         r = resolved_date.get(k, resolved_dummy_date)
         debug.trace_fmtd(7, "get_resolved_date({k}) => {r}", k=k, r=r)
         return r
     #
     debug.trace_fmtd(7, "notes_hash keys: {{\n{k}\n}}", 
                      k="\t\n".join([str(v) for v in notes_hash.keys()]))
     #
-    # TODO: make byte order mark optional (used so special characters resolved automatically in Emacs)
     if not SKIP_BOM:
         try:
-            ## OLD:
             print("\uFEFF")
-            ## TEMP: print("\uFEFF".encode("UTF8"))
         except:
             system.print_exception_info("printing BOM")
     #
     for pos, date in enumerate(sorted(notes_hash.keys(), 
                                       key=get_resolved_date)):
         debug.trace_fmtd(6, "outputting notes for date {d} [resolved: {r}]", 
                          d=date, r=resolved_date.get(date))
         if output_dividers and (pos > 0):
             print("-" * 80)
-        debug.trace_fmtd(6, "[src={f}:{n}]", skip_newline=True,
+        debug.trace_fmtd(6, "[src {f}:{n}]", skip_newline=True,
                          f=fileinput.filename(), n=fileinput.filelineno())
-        ## OLD: print("%s\n\n" % notes_hash[date])
-        ## TEMP:
         try:
-            ## BAD: print("%s\n\n" % notes_hash[date].encode("UTF8", errors="ignore"))
             print("%s\n\n" % notes_hash[date])
         except:
             system.print_exception_info("printing entry")
 
     return
 
 #------------------------------------------------------------------------
```

### Comparing `mezcla-1.3.9.8/mezcla/mezcla` & `mezcla-1.3.9.9/mezcla/mezcla`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/misc_utils.py` & `mezcla-1.3.9.9/mezcla/misc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,28 +290,40 @@
     ## EX: is_close(1.001, 1.002, epsilon=.005)
     ## EX: (not is_close(1.001, 1.002, epsilon=.0005))
     result = math.isclose(value1, value2, abs_tol=epsilon)
     debug.trace(6, f"is_close({value1}, {value2}, [eps={epsilon}]) => {result}")
     return result
 
 
-def get_date_ddmmmyy(date=None):
-    """Return (today's) date in DDMMMYY format (e.g., 10oct22)"""
-    ## TODO EX: get_date_ddmmmyy(datetime.date(0)) => "01jan70"
+def get_formatted_date(date=None, fmt=None, sep=None):
+    """Return (today's) date in DD MMM YY format (e.g., 10 oct 22)
+    Note: uses optional SEP between components or FMT"""
+    ## EX: get_formatted_date(datetime.date(0)) => "01 jan 70"
+    ## TODO3: rename as get_formatted_date
     in_date = date
     if date is None:
         date = datetime.date.today()
+    if sep is None:
+        sep = " "
+    if fmt is None:
+        fmt = f"%d{sep}%b{sep}%y"
     try:
-        result = date.strftime("%d%b%y").lower()
+        result = date.strftime(fmt).lower()
     except:
         system.print_exception_info("get_today_ddmmmyy")
         result = "???"
-    debug.trace(6, f"get_date_ddmmmyy({in_date}) => {result}")
+    debug.trace(6, f"get_formatted_date({in_date}) => {result}")
     return result
 
+def get_date_ddmmmyy(date=None):
+    """Return (today's) date in DDMMMYY format (e.g., 10oct22)"""
+    ## EX: get_date_ddmmmyy(datetime.date(0)) => "01jan70"
+    result = get_formatted_date(date).replace(" ", "")
+    debug.trace(6, f"get_date_ddmmmyy({date}) => {result}")
+    return result
 
 def parse_timestamp(ts: str, truncate=None, utc=None) -> datetime.datetime:
     """Parse timestamp in ISO 8601 format (e.g., 2023-10-06T04:03:27.1271706Z)
     Note: The timestamp is truncated to micrososeconds unless TRUNCATE is false; and, it is optionally converted to UTC
     """
     # EX: parse_timestamp("2023-10-06T04:03:27.1271706Z") => datetime.datetime(2023, 10, 6, 4, 3, 27, 127170, tzinfo=datetime.timezone.utc)
     # Note: See https://stackoverflow.com/questions/6207365/working-with-high-precision-timestamps-in-python
```

### Comparing `mezcla-1.3.9.8/mezcla/my_regex.py` & `mezcla-1.3.9.9/mezcla/my_regex.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,27 +140,29 @@
                          r=regex, t=text, f=flags, s=self)
         ## OLD: debug.assertion(isinstance(text, six.string_types))
         debug.assertion(isinstance(text, (str, bytes)) and (isinstance(regex, type(text))))
         self.check_pattern(regex)
         self.match_result = re.search(regex, text, flags)
         if self.match_result:
             debug.trace_fmt(base_trace_level, "match: {m!r}; regex: {r!r}", m=self.grouping(), r=regex)
+            debug.trace_object(base_trace_level + 1, self.match_result)
         return self.match_result
 
     def match(self, regex, text, flags=0, base_trace_level=None):
         """Match REGEX to TEXT with optional FLAGS and BASE_TRACE_LEVEL (e.g., 6)"""
         ## TODO: rename as match_start for clarity; add match_all method (wrapper around fullmatch)
         if base_trace_level is None:
             base_trace_level = self.TRACE_LEVEL
         debug.trace_fmtd((1 + base_trace_level), "my_regex.match({r!r}, {t!r}, {f}): self={s}",
                          r=regex, t=text, f=flags, s=self)
         self.check_pattern(regex)
         self.match_result = re.match(regex, text, flags)
         if self.match_result:
             debug.trace_fmt(base_trace_level, "match: {m!r}; regex: {r!r}", m=self.grouping(), r=regex)
+            debug.trace_object(base_trace_level + 1, self.match_result)
         return self.match_result
 
     def get_match(self):
         """Return match result object for last search or match"""
         result = self.match_result
         debug.trace_fmtd(self.TRACE_LEVEL, "my_regex.get_match() => {r!r}: self={s}",
                          r=result, s=self)
```

### Comparing `mezcla-1.3.9.8/mezcla/ngram_tfidf.py` & `mezcla-1.3.9.9/mezcla/ngram_tfidf.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from mezcla.main import Main
 ## OLD: from mezcla import spacy_nlp
 from mezcla import system
 from mezcla.system import round_num as rnd
 from mezcla import tpo_common as tpo
 from mezcla import tfidf
 from mezcla.compute_tfidf import terms_overlap
-from mezcla.text_processing import stopwords as ENGLISH_STOPWORDS, create_text_proc
+from mezcla.text_processing import stopwords as ENGLISH_STOPWORDS, create_text_proc, split_word_tokens
 from mezcla.tfidf.corpus import Corpus as tfidf_corpus
 from mezcla.tfidf.preprocess import Preprocessor as tfidf_preprocessor
 from mezcla.tfidf import preprocess as tfidf_preprocess
 
 SKIP_TFIDF_PREPROCESSOR = system.getenv_bool(
     "SKIP_TFIDF_PREPROCESSOR", False,
     description="Skip tf/idf prepreprocessing",
@@ -92,14 +92,20 @@
     description="Boost factor for ngrams that are VP's")
 TFIDF_NUMERIC_BOOST = system.getenv_float(
     "TFIDF_NUMERIC_BOOST", 0,
     description="Boost factor for ngrams that have numeric tokens")
 TFIDF_TEXT_PROC = system.getenv_text(
     "TFIDF_TEXT_PROC", "spacy",
     description="name of text processor to use for chunking")
+TFIDF_BAD_BOOST = system.getenv_float(
+    "TFIDF_BAD_BOOST", 0,
+    description="Boost factor for ngrams that bad terms")
+TFIDF_GOOD_BOOST = system.getenv_float(
+    "TFIDF_GOOD_BOOST", 0,
+    description="Boost factor for ngrams that good terms")
 
 ## OLD:
 ## # Dynamic loading
 ## spacy_nlp = None
 ## if TFIDF_NP_BOOST:
 ##     from mezcla import spacy_nlp
 ##     debug.trace_expr(5, spacy_nlp)
@@ -111,47 +117,75 @@
     TFIDF_VERSION = float(major_minor)
 except:
     TFIDF_VERSION = 1.0
     system.print_stderr("Exception in main: " + str(sys.exc_info()))
 assert(TFIDF_VERSION > 1.0)
 
 
+def split_tokens(text, include_punct=None, include_stop=None):
+    """Split TEXT into word tokens (via NLTK), optionally with INCLUDE_PUNCT and INCLUDE_STOP"""
+    # EX: split_tokens("Jane's fast car") => ["Jane", "fast", "car"]
+    result = split_word_tokens(text, omit_punct=(not include_punct), omit_stop=(not include_stop))
+    debug.trace(6, f"split_tokens({text!r}, punct={include_punct}, stop={include_stop}) => {result!r}")
+    return result
+
+
 class ngram_tfidf_analysis(object):
     """Class for performing TF-IDF over ngrams and returning sorted list"""
 
-    def __init__(self, pp_lang=PREPROCESSOR_LANG, min_ngram_size=MIN_NGRAM_SIZE, max_ngram_size=MAX_NGRAM_SIZE, 
-                 *args, **kwargs):
-        """Class constructor: initialize corpus object (with PP_LANG, MIN_NGRAM_SIZE, and MAX_NGRAM_SIZE)"""
+    def __init__(self, pp_lang=PREPROCESSOR_LANG, min_ngram_size=MIN_NGRAM_SIZE, max_ngram_size=MAX_NGRAM_SIZE,
+                 good_terms=None, bad_terms=None, *args, **kwargs):
+        """Class constructor: initialize corpus object (with PP_LANG, MIN_NGRAM_SIZE, and MAX_NGRAM_SIZE)
+        Note: Optional BAD_TERMS used to boost or penalize certain ngrams (e.g., based on title)
+        """
         # EX: ((self := ngram_tfidf_analysis(pp_lang="")) and (not self.pp.stopwords))
         # TODO: add option for stemmer; add all_ngrams and min_ngram_size to constructor
         debug.trace_fmtd(4, "ngram_tfidf_analysis.__init__(lang={pl}, min={minsz}, max={maxsz})",
                          pl=pp_lang, minsz=min_ngram_size, maxsz=max_ngram_size)
         debug.trace_fmtd(5, "\targs={a} kwargs={k}", a=args, k=kwargs)
         if pp_lang is None:
             pp_lang = PREPROCESSOR_LANG
+        self.pp_lang = pp_lang
         self.min_ngram_size = min_ngram_size
         self.max_ngram_size = max_ngram_size
-        self.pp = tfidf_preprocessor(language=pp_lang,
+        self.pp = None
+        self.corpus = None
+        ## OLD: self.chunker = (None if (not TFIDF_NP_BOOST) else spacy_nlp.Chunker())
+        self.text_proc = None
+        if TFIDF_NP_BOOST or TFIDF_VP_BOOST:
+            self.text_proc = create_text_proc(TFIDF_TEXT_PROC)
+        ## TODO2: add international stopwords (e.g., English plus frequent ones from common languages)
+        self.stopwords = None
+        self.good_terms = (good_terms or [])
+        self.bad_terms = (bad_terms or [])
+        self.reset()
+        super().__init__(*args, **kwargs)
+
+    def reset(self):
+        """Re-initialize the instance"""
+        self.pp = tfidf_preprocessor(language=self.pp_lang,
                                      gramsize=self.max_ngram_size,
                                      min_ngram_size=self.min_ngram_size,
                                      all_ngrams=ALL_NGRAMS,
                                      stemmer=lambda x: x)
         self.corpus = tfidf_corpus(gramsize=self.max_ngram_size,
                                    min_ngram_size=self.min_ngram_size,
                                    all_ngrams=ALL_NGRAMS,
-                                   language=pp_lang,
+                                   language=self.pp_lang,
                                    preprocessor=self.pp)
-        ## OLD: self.chunker = (None if (not TFIDF_NP_BOOST) else spacy_nlp.Chunker())
-        self.text_proc = None
-        if TFIDF_NP_BOOST or TFIDF_VP_BOOST:
-            self.text_proc = create_text_proc(TFIDF_TEXT_PROC)
-        ## TODO2: add international stopwords (e.g., English plus frequent ones from common languages)
         self.stopwords = (self.pp.stopwords or ENGLISH_STOPWORDS)
-        super().__init__(*args, **kwargs)
 
+    def set_good_terms(self, text):
+        """Sets good terms to TEXT split into word tokens"""
+        self.good_terms = split_tokens(text)
+        
+    def set_bad_terms(self, text):
+        """Sets bad terms to TEXT split into word tokens"""
+        self.bad_terms = split_tokens(text)
+        
     def add_doc(self, text, doc_id=None):
         """Add document TEXT to collection with key DOC_ID, which defaults to order processed (1-based)"""
         if doc_id is None:
             doc_id = str(len(self.corpus) + 1)
         self.corpus[doc_id] = text
 
     def get_doc(self, doc_id):
@@ -166,15 +200,15 @@
         debug.trace(8, f"is_stopword({word!r}) => {result}")
         return result
 
     def capitalized_ngram(self, ngram):
         """Whethere NGRAM is capitalized, excepting internal stopwords"""
         ## EX: self.capitalized_ngram("House of Cards")
         ## EX: not self.capitalized_ngram("in New York")
-        tokens = ngram.split()
+        tokens = split_tokens(ngram, include_stop=True)
         result = (tokens and tokens[0].istitle()
                   and ((len(tokens) == 1) or tokens[-1].istitle()))
         if (result and (len(tokens) > 2)):
             for w in tokens[1: -1]:
                 if not (w.istitle() or self.is_stopword(w)):
                     debug.trace(5, f"ngram with lower inner non-stop word {w!r}: {tokens!r}")
                     result = False
@@ -232,16 +266,23 @@
                 # Apply boost if entire ngram is a noun phrase and likewise for verb phrase
                 if (TFIDF_NP_BOOST and self.text_proc.noun_phrases(ngram) == [ngram]):
                     score = old_score * TFIDF_NP_BOOST
                     debug.trace(5, f"boosted NP {ngram!r} from {rnd(old_score)} to {rnd(score)}")
                 if (TFIDF_VP_BOOST and self.text_proc.verb_phrases(ngram) == [ngram]):
                     score = old_score * TFIDF_VP_BOOST
                     debug.trace(5, f"boosted VP {ngram!r} from {rnd(old_score)} to {rnd(score)}")
-                if (TFIDF_NUMERIC_BOOST and any(tpo.is_numeric(token) for token in ngram.split())):
+                if (TFIDF_NUMERIC_BOOST and any(tpo.is_numeric(token) for token in split_tokens(ngram))):
                     score = old_score * TFIDF_NUMERIC_BOOST
+                    debug.trace(5, f"boosted numeric {ngram!r} from {rnd(old_score)} to {rnd(score)}")
+                if (TFIDF_GOOD_BOOST and system.intersection(split_tokens(ngram), self.good_terms)):
+                    score = old_score * TFIDF_GOOD_BOOST
+                    debug.trace(5, f"boosted good-term {ngram!r} from {rnd(old_score)} to {rnd(score)}")
+                if (TFIDF_BAD_BOOST and system.intersection(split_tokens(ngram), self.bad_terms)):
+                    score = old_score * TFIDF_BAD_BOOST
+                    debug.trace(5, f"boosted bad-term {ngram!r} from {rnd(old_score)} to {rnd(score)}")
                 # Update changed score
                 if old_score != score:
                     ## BAD: top_term_info[i][1] = score
                     top_term_info[i] = (ngram, score)
                     boosted = True
             # Re-rank if scores changed
             if boosted:
@@ -264,15 +305,15 @@
             debug.trace_fmtd(7, "spaced_ngrams={sn}", sn=spaced_ngrams)
         final_top_term_info = []
         for (i, (ngram, score)) in enumerate(top_term_info):
             
             if (not ngram.strip()):
                 debug.trace_fmt(6, "Omitting invalid ngram '{ng}'", ng=ngram)
                 continue
-            if ((not allow_numeric_ngrams) and any(tpo.is_numeric(token) for token in ngram.split())):
+            if ((not allow_numeric_ngrams) and any(tpo.is_numeric(token) for token in split_tokens(ngram))):
                 debug.trace_fmt(6, "Omitting ngram with numerics '{ng}'", ng=ngram)
                 continue
             
             # Check for subsumption (e.g., "new york" in "new york city") and overlap (e.g. "new york" and "york city")
             ## TODO: record ngram offsets to facilitate contiguity tests
             include = True
             if check_ngram_overlap:
@@ -342,15 +383,15 @@
     """Run test extracting ngrams from this source file"""
     debug.trace(4, "simple_main_test()")
     # Tabulate ngram occurrences
     ## BAD: ngram_analyzer = ngram_tfidf_analysis(min_ngram_size=2, max_ngram_size=3)
     ngram_analyzer = ngram_tfidf_analysis(min_ngram_size=MIN_NGRAM_SIZE, max_ngram_size=MAX_NGRAM_SIZE)
     all_text = system.read_entire_file(__file__)
     all_ngrams = ngram_analyzer.get_ngrams(all_text)
-    reversed_all_text = " ".join(list(reversed(all_text.split())))
+    reversed_all_text = " ".join(list(reversed(split_tokens(all_text, include_punct=True, include_stop=True))))
     ngram_analyzer.add_doc(all_text, doc_id="doc1")
     ngram_analyzer.add_doc(reversed_all_text, doc_id="rev-doc1")
     top_ngrams = ngram_analyzer.get_top_terms("rev-doc1", allow_ngram_subsumption=False, allow_ngram_overlap=False)
 
     # Check for common ngrams
     debug.assertion("simple test follows" in all_ngrams)
     debug.assertion("system getenv_boolean" in top_ngrams)
@@ -374,18 +415,22 @@
     init_ngram_spec = "\n\t".join(all_ngrams[:SAMPLE_SIZE])
     print(f"first 10 ngrams in {__file__}:\n\t{init_ngram_spec}")
     init_top_ngram_spec = "\n\t".join([f"{t}: {tpo.round_num(s, 3)}"
                                        for (t, s) in top_ngrams[:SAMPLE_SIZE]])
     print(f"top ngrams in {__file__}:\n\t{init_top_ngram_spec}")
 
 
-def output_tfidf_analysis(main_app):
+def output_tfidf_analysis(main_app, good_text=None, bad_text=None):
     """Output results for ngram TF/IDF analysis over input from MAIN_APP"""
     debug.trace(4, f"output_tfidf_analysis({main_app})")
-    ngram_analyzer = ngram_tfidf_analysis(min_ngram_size=MIN_NGRAM_SIZE, max_ngram_size=MAX_NGRAM_SIZE)
+    ## TODO3: let ngram_tfidf_analysis class do the splitting
+    good_terms = ([] if not good_text else split_tokens(good_text))
+    bad_terms = ([] if not bad_text else split_tokens(bad_text))
+    ngram_analyzer = ngram_tfidf_analysis(min_ngram_size=MIN_NGRAM_SIZE, max_ngram_size=MAX_NGRAM_SIZE,
+                                          good_terms=good_terms, bad_terms=bad_terms)
     all_text = main_app.read_entire_input()
     num_docs = 0
     for l, line in enumerate(all_text.splitlines()):
         ngram_analyzer.add_doc(line, doc_id=(l + 1))
         num_docs += 1
 
     # Output ngram sample
@@ -397,23 +442,29 @@
         print(f"{l}\t{top_ngram_spec}")
     
 def main():
     """Entry point for script"""
     debug.trace(4, "main()")
     SIMPLE_TEST_OPT = "simple-test"
     REGULAR_OPT = "regular"
+    GOOD_TERMS_OPT = "good-terms"
+    BAD_TERMS_OPT = "bad-terms"
     main_app = Main(description=__doc__.format(script=gh.basename(__file__),
                                                options=f"--{REGULAR_OPT}"),
-                    boolean_options=[(SIMPLE_TEST_OPT, "Run simple test (default)"),
-                                     (REGULAR_OPT, "Process regular input")],
+                    boolean_options=[(SIMPLE_TEST_OPT, "Run simple canned test--default"),
+                                     (REGULAR_OPT, "Process regular input--not canned test")],
+                    text_options=[(GOOD_TERMS_OPT, "Overlap terms for boosting ngrams scores"),
+                                  (BAD_TERMS_OPT, "Overlap terms for de-boosting ngrams scores")],
                     skip_input=False)
     regular = main_app.get_parsed_option(REGULAR_OPT)
     simple_test = main_app.get_parsed_option(SIMPLE_TEST_OPT, not regular)
+    good_terms_text = main_app.get_parsed_option(GOOD_TERMS_OPT)
+    bad_terms_text = main_app.get_parsed_option(BAD_TERMS_OPT)
     if (simple_test):
         simple_main_test()
     else:
-        output_tfidf_analysis(main_app)
+        output_tfidf_analysis(main_app, good_text=good_terms_text, bad_text=bad_terms_text)
    
 #-------------------------------------------------------------------------------
 
 if __name__ == '__main__':
     main()
```

### Comparing `mezcla-1.3.9.8/mezcla/os_utils.py` & `mezcla-1.3.9.9/mezcla/os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/pandas_sklearn.py` & `mezcla-1.3.9.9/mezcla/pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/plot_utils.py` & `mezcla-1.3.9.9/mezcla/plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/python_ast.py` & `mezcla-1.3.9.9/mezcla/python_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/randomize_lines.py` & `mezcla-1.3.9.9/mezcla/randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/rgb_color_name.py` & `mezcla-1.3.9.9/mezcla/rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/run_albert_classifier.py` & `mezcla-1.3.9.9/mezcla/run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/run_bert_classifier.py` & `mezcla-1.3.9.9/mezcla/run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/samples/pima-indians-diabetes.csv` & `mezcla-1.3.9.9/mezcla/samples/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/show_bert_representation.py` & `mezcla-1.3.9.9/mezcla/show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/simple_main_example.py` & `mezcla-1.3.9.9/mezcla/simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/spacy_nlp.py` & `mezcla-1.3.9.9/mezcla/spacy_nlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,24 +257,26 @@
             model = SPACY_MODEL
         self.model = model
         try:
             init()
             self.nlp = spacy.load(self.model)
         except:
             system.print_exception_info(f"load of model {model}")
-        debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
+        ## TODO3: debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
+        debug.trace_object(5, self, label="SpacyHelper instance")
 
 class Chunker(SpacyHelper):
     """Class for chunking text into noun phrases"""
 
     def __init__(self, model=None):
         """Initializer: ..."""
         debug.trace_fmtd(TL.VERBOSE, "Helper.__init__(): self={s}", s=self)
         super().__init__(model)
-        debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
+        ## TODO3: debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
+        debug.trace_object(5, self, label="Chunker instance")
 
     def noun_phrases(self, text):
         """Return list of noun chunks in text"""
         chunks = []
         try:
             doc = self.nlp(text)
             chunks = [ch.text for ch in doc.noun_chunks]
```

### Comparing `mezcla-1.3.9.8/mezcla/spell.py` & `mezcla-1.3.9.9/mezcla/spell.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/sys_version_info_hack.py` & `mezcla-1.3.9.9/mezcla/sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/system.py` & `mezcla-1.3.9.9/mezcla/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 #
 
 """System-related functions"""
 
 # Standard packages
 from collections import defaultdict, OrderedDict
 import datetime
-import importlib_metadata
+## OLD: import importlib_metadata
 import inspect
 import os
 import pickle
 import re
 import sys
 import time
 
@@ -801,14 +801,15 @@
 
 def split_path(path):
     """Split file PATH into directory and filename
     Note: wrapper around os.path.split with tracing and sanity checks
     """
     # EX: split_path("/etc/passwd") => ["etc", "passwd"]
     dir_name, filename = os.path.split(path)
+    debug.assertion((not dir_name.endswith(os.path.sep)) or (dir_name == os.path.sep))
     result = dir_name, filename
     debug.assertion(dir_name or filename)
     if dir_name and debug.active() and file_exists(path):
         debug.assertion(file_exists(dir_name))
     debug.trace(6, f"split_path({path}) => {result}")
     return result
 
@@ -1067,14 +1068,16 @@
     """Get version number for MODULE_NAME (string)"""
     # note: used in bash function (alias):
     #     python-module-version() = { python -c "print(get_module_version('$1))"; }'
 
     # Try to get the version number for the module
     version = "?.?.?"
     try:
+        # note: made conditional due to silly problem with shell-scripts repo workflow
+        import importlib_metadata       # pylint: disable=import-outside-toplevel
         version = importlib_metadata.version(module_name)
     except:
         print_exception_info("get_module_version for {module_name}")
     debug.trace(6, f"get_module_version({module_name}) => {version}")
     return version
```

### Comparing `mezcla-1.3.9.8/mezcla/temp/compound_CID_3672.xml` & `mezcla-1.3.9.9/mezcla/temp/compound_CID_3672.xml`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/temp/plot.py` & `mezcla-1.3.9.9/mezcla/temp/plot.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/temp/simple_batspp.py` & `mezcla-1.3.9.9/mezcla/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/template.py` & `mezcla-1.3.9.9/mezcla/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 # longer such as two or more tokens (e.g., "FUBAR" => "FUBAR_LEVEL").
 #
 TODO_FUBAR = system.getenv_bool("TODO_FUBAR", False,
                                 description="TODO:Fouled Up Beyond All Recognition processing")
 
 ## TODO: Use helper class for main logic
 ## class Helper:
+##     """TODO: class for doing ..."""
 ## 
 ##     def __init__(self, ...):
 ##         """Initializer: ..."""
 ##         debug.trace_fmtd(TL.VERBOSE, "Helper.__init__(): self={s}", s=self)
 ##         self.TODO = None
 ##         debug.trace_object(5, self, label=f"{self.__class__.__name__} instance")
 ## 
@@ -107,19 +108,19 @@
             print(f"arg1 line ({self.line_num}): {line}")
         else:
             debug.trace(3, f"Ignoring line ({self.line_num}): {line}")
         ## TODO: regex pattern matching
         ## elif my_re.search(self.text_arg, line):
         ##     print("arg2 line: %s" % line)
 
-    ## TODO: if no input proocessed, customize run_main_step instead
+    ## TODO: if no input prococessed, customize run_main_step instead
     ## and specify skip_input below
     ##
     ## def run_main_step(self):
-    ##     """Main processing step"""
+    ##     """Main processing step (n.b., assumes self.manual_input)"""
     ##     debug.trace_fmtd(5, "Script.run_main_step(): self={s}", s=self)
     ##
 
     ## TODO:
     ## def wrap_up(self):
     ##     """Do final processing"""
     ##     debug.trace(6, f"Script.wrap_up(); self={self}")
```

### Comparing `mezcla-1.3.9.8/mezcla/tests/LICENSE.txt` & `mezcla-1.3.9.9/mezcla/tests/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/adhoc-tests.batspp` & `mezcla-1.3.9.9/mezcla/tests/adhoc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/conftest.py` & `mezcla-1.3.9.9/mezcla/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt` & `mezcla-1.3.9.9/mezcla/tests/jupyter/jupyter-resource/sentence_es_30.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb` & `mezcla-1.3.9.9/mezcla/tests/jupyter/revised_checkout_mezcla_aviyan_dev.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/jupyter/test_audio_py.ipynb` & `mezcla-1.3.9.9/mezcla/tests/jupyter/test_audio_py.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/jupyter/test_audio_py_experimental.ipynb` & `mezcla-1.3.9.9/mezcla/tests/jupyter/test_audio_py_experimental.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb` & `mezcla-1.3.9.9/mezcla/tests/jupyter/test_hugging_face_speechrec.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/jupyter/test_hugging_face_translation.ipynb` & `mezcla-1.3.9.9/mezcla/tests/jupyter/test_hugging_face_translation.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/jupyter/test_template.ipynb` & `mezcla-1.3.9.9/mezcla/tests/jupyter/test_template.ipynb`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/misc-tests.batspp` & `mezcla-1.3.9.9/mezcla/tests/misc-tests.batspp`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/misc_doctests.py` & `mezcla-1.3.9.9/mezcla/tests/misc_doctests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/misc_tests.py` & `mezcla-1.3.9.9/mezcla/tests/misc_tests.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/argentinian-attraction-snippets.txt` & `mezcla-1.3.9.9/mezcla/tests/resources/argentinian-attraction-snippets.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/cars-csv-len-3.txt` & `mezcla-1.3.9.9/mezcla/tests/resources/cars-csv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/cars-tsv-len-3.txt` & `mezcla-1.3.9.9/mezcla/tests/resources/cars-tsv-len-3.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/cars.csv` & `mezcla-1.3.9.9/mezcla/tests/resources/cars.csv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/cars.tsv` & `mezcla-1.3.9.9/mezcla/tests/resources/cars.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/example_text.txt` & `mezcla-1.3.9.9/mezcla/tests/resources/example_text.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/example_text_tags.txt` & `mezcla-1.3.9.9/mezcla/tests/resources/example_text_tags.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/iris_output.txt` & `mezcla-1.3.9.9/mezcla/tests/resources/iris_output.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/random-10pct-tweet-emotions.tsv` & `mezcla-1.3.9.9/mezcla/tests/resources/random-10pct-tweet-emotions.tsv`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/simple-window-dimensions.html` & `mezcla-1.3.9.9/mezcla/tests/resources/simple-window-dimensions.html`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/spanish-accents.docx` & `mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.docx`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/spanish-accents.pdf` & `mezcla-1.3.9.9/mezcla/tests/resources/spanish-accents.pdf`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/resources/test.arpa` & `mezcla-1.3.9.9/mezcla/tests/resources/test.arpa`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/template.py` & `mezcla-1.3.9.9/mezcla/tests/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #! /usr/bin/env python
+# TODO: # -*- coding: utf-8 -*-
 #
 # TODO: Test(s) for ../<module>.py
 #
 # Notes:
 # - Fill out TODO's below. Use numbered tests to order (e.g., test_1_usage).
 # - * See test_python_ast.py for simple example of customization.
 # - TODO: If any of the setup/cleanup methods defined, make sure to invoke base
@@ -53,24 +54,23 @@
 
 class TestIt(TestWrapper):
     """Class for command-line based testcase definition"""
     script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
     #
     # TODO: use_temp_base_dir = True            # treat TEMP_BASE as directory
     # note: temp_file defined by parent (along with script_module, temp_base, and test_num)
-    # TODO: use TestIt2 if capsys needed
 
     ## TODO: optional setup methods
     ##
     ## @classmethod
-    ## def setUpClass(cls):
+    ## def setUpClass(cls, filename=None, module=None):
     ##     """One-time initialization (i.e., for entire class)"""
     ##     debug.trace(6, f"TestIt.setUpClass(); cls={cls}")
     ##     # note: should do parent processing first
-    ##     super().setUpClass()
+    ##     super().setUpClass(filename, module)
     ##     ...
     ##     debug.trace_object(5, cls, label=f"{cls.__class__.__name__} instance")
     ##     return
     ##
     ## def setUp(self):
     ##     """Per-test setup"""
     ##     debug.trace(6, f"TestIt.setUp(); self={self}")
@@ -78,33 +78,41 @@
     ##     super().setUp()
     ##     ...
     ##     # TODO: debug.trace_current_context(level=debug.QUITE_DETAILED)
     ##     return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     ## DEBUG: @trap_exception            # TODO: remove when debugged
-    def test_data_file(self):
+    def test_01_data_file(self):
         """Tests run_script w/ data file"""
-        debug.trace(4, f"TestIt.test_data_file(); self={self}")
+        debug.trace(4, f"TestIt.test_01_data_file(); self={self}")
         data = ["TODO1", "TODO2"]
         system.write_lines(self.temp_file, data)
         ## TODO: add use_stdin=True to following if no file argument
         output = self.run_script(options="", data_file=self.temp_file)
         self.do_assert(my_re.search(r"TODO-pattern", output.strip()))
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     ## DEBUG: @trap_exception            # TODO: remove when debugged
-    def test_something_else(self):
+    def test_02_something_else(self):
         """Test for something_else: TODO..."""
-        debug.trace(4, f"TestIt.test_something_else(); self={self}")
+        debug.trace(4, f"TestIt.test_02_something_else(); self={self}")
         self.do_assert(False)
         ## ex: self.do_assert(THE_MODULE.TODO_function() == TODO_value)
         return
 
+    @pytest.mark.xfail                   # TODO: remove xfail
+    def test_02_whatever(self):
+        """TODO: flesh out test for whatever (capsys-like)"""
+        debug.trace(4, f"TestIt2.test_02_whatever(); self={self}")
+        THE_MODULE.TODO_whatever()
+        captured = self.get_stderr()
+        self.do_assert("whatever" in captured, "TODO_whatever trace")
+        return
 
     ## TODO: optional cleanup methods
     ##
     ## def tearDown(self):
     ##     debug.trace(6, f"TestIt.tearDown(); self={self}")
     ##     super().tearDownClass()
     ##     ...
@@ -113,32 +121,12 @@
     ## @classmethod
     ## def tearDownClass(cls):
     ##     debug.trace(6, f"TestIt.tearDownClass(); cls={cls}")
     ##     super().tearDown()
     ##     ...
     ##     return
 
-class TestIt2:
-    """Class for API-based testcase definition
-    Note: Separate class avoids error with pytest due to inheritance with unittest.TestCase via TestWrapper (e.g., capsys support)"""
-
-    def do_assert(self, condition, message=None):
-        """Wrapper around assert"""
-        ## TODO2: put this in new AltTestWrapper
-        debug.trace(7, f"TestIt2.do_assert({condition}, msg={message})")
-        assert condition, message
-
-    @pytest.mark.xfail                   # TODO: remove xfail
-    def test_whatever(self, capsys):
-        """TODO: flesh out test for whatever"""
-        debug.trace(4, f"TestIt2.test_whatever(); self={self}")
-        THE_MODULE.TODO_whatever()
-        captured = capsys.readouterr()
-        self.do_assert("whatever" in captured.err, "TODO_whatever trace")
-        return
-
-
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.9.8/mezcla/tests/test___init__.py` & `mezcla-1.3.9.9/mezcla/tests/test___init__.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_audio.py` & `mezcla-1.3.9.9/mezcla/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_bert_multi_classification.py` & `mezcla-1.3.9.9/mezcla/tests/test_bert_multi_classification.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_bing_search.py` & `mezcla-1.3.9.9/mezcla/tests/test_bing_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_compute_tfidf.py` & `mezcla-1.3.9.9/mezcla/tests/test_compute_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_convert_emoticons.py` & `mezcla-1.3.9.9/mezcla/tests/test_convert_emoticons.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,35 +47,39 @@
 
 class TestIt(TestWrapper):
     """Class for testcase definition"""
     script_module = TestWrapper.get_testing_module_name(__file__, THE_MODULE)
     script_file = my_re.sub(rf"{D}tests{D}test_", f"{D}", __file__)
 
     @pytest.mark.xfail                   # TODO: remove xfail
+    ## TEST: @trap_exception
     def test_over_script(self):
         """Makes sure works as expected over script itself"""
         debug.trace(4, f"TestIt.test_over_script(); self={self}")
-        output = self.run_script(options="", data_file=self.script_file)
+        output = self.run_script(options="", data_file=__file__)
         # the example usage should have input emoticon changed to match output
         script_contents = system.read_file(self.script_file)
-        debug.trace_expr(6, script_contents)
+        debug.trace_expr(6, script_contents, max_len=8192)
         # ex (see above): "# Input:\n#   Nothing to do 😴\n# Output:\n#   Nothing to do [sleeping face]"
         self.do_assert(not my_re.search(r"(\[sleeping face\]).*\1", script_contents, flags=my_re.DOTALL))
         # ex (see above): "# Input:\n#   Nothing to do [sleeping face]\n#\n# Output:\n#   Nothing to do [sleeping face]"
         self.do_assert(my_re.search(r"(\[sleeping face\]).*\1", output, flags=my_re.DOTALL))
 
         # Make sure no emoticon byte sequences in UTF-8 sequences for output, although in script.
         # Note: Uses broader UTF8-based tests than Unicode character DB used in script.
         # Also, regex is done over byte sequences to account for misformed input.
         loose_emoticon_regex = br"[\xE0-\xFF][\x80-\xFF]{1,3}"
         # ex: "# EX: convert_emoticons("天気") => "天気"   # Japanese for weather"
         self.do_assert(my_re.search(loose_emoticon_regex, script_contents.encode()))
-        output_san_Japanese_example = my_re.sub(r"^.*Japanese.*$", "", output, flags=my_re.MULTILINE)
+        output_sans_cjk_examples = my_re.sub(r"^.*(Chinese|Japanese).*$", "", output,
+                                             flags=my_re.MULTILINE)
         # ex: [same as above because CJK preserved]
-        self.do_assert(not my_re.search(loose_emoticon_regex, output_san_Japanese_example.encode()))
+        bad_match = my_re.search(loose_emoticon_regex, output_sans_cjk_examples.encode())
+        debug.trace_expr(5, bad_match, output_sans_cjk_examples)
+        self.do_assert(not bad_match)
         return
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_over_script_sans_comments(self):
         """Makes sure works as expected over script itself"""
         debug.trace(4, f"TestIt.test_over_script_sans_comments(); self={self}")
 
@@ -87,19 +91,14 @@
         output = self.run_script(options="", data_file=self.temp_file)
 
         # There should be no extended ascii bytes
         self.do_assert(not my_re.search(b"[\x80-\xFF]", script_contents_sans_comments.encode()))
         self.do_assert(not my_re.search(b"[\x80-\xFF]", output.encode()))
         return
 
-    ## OLD:
-    ## class TestIt2:
-    ##     """Another class for testcase definition
-    ##     Note: Needed to avoid error with pytest due to inheritance with unittest.TestCase via TestWrapper    ## """
-    
     @trap_exception
     def test_misc(self):
         """Test direct calls for conversion"""
         debug.trace(4, f"TestIt2.test_whatever(); self={self}")
         convert_emoticons = THE_MODULE.convert_emoticons
         cool_smile = "\U0001F60E"        # 😎
         self.do_assert(convert_emoticons(cool_smile) == "[smiling face with sunglasses]")
```

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_cut.py` & `mezcla-1.3.9.9/mezcla/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_data_utils.py` & `mezcla-1.3.9.9/mezcla/tests/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_debug.py` & `mezcla-1.3.9.9/mezcla/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_extract_document_text.py` & `mezcla-1.3.9.9/mezcla/tests/test_extract_document_text.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_file_utils.py` & `mezcla-1.3.9.9/mezcla/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_filter_random.py` & `mezcla-1.3.9.9/mezcla/tests/test_filter_random.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_format_profile.py` & `mezcla-1.3.9.9/mezcla/tests/test_format_profile.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_gensim_test.py` & `mezcla-1.3.9.9/mezcla/tests/test_gensim_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_glue_helpers.py` & `mezcla-1.3.9.9/mezcla/tests/test_glue_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,34 +10,38 @@
 # - Add support for write_lines & read_lines.
 # - Add support for other commonly used functions.
 #
 
 """Tests for glue_helpers module"""
 
 # Standard packages
-from os import path
+import os
+## OLD: from os import path
 from io import StringIO
 import sys
 
 # Installed packages
 import pytest
 
 # Local packages
 from mezcla import debug
 from mezcla import glue_helpers as gh
-from mezcla import tpo_common as tpo # Deprecated, only used for mock
+from mezcla.my_regex import my_re
+from mezcla import tpo_common as tpo    # Deprecated, only used for mock
 ## OLD: from mezcla.unittest_wrapper import TestWrapper
 from mezcla import system
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 import mezcla.glue_helpers as THE_MODULE # pylint: disable=reimported
 
-class TestGlueHelpers:
+class TestGlueHelpers:      ## TODO: (TestWrapper)
     """Class for testcase definition"""
+    ## TEMP
+    temp_file = gh.get_temp_file()
 
     def test_get_temp_file(self):
         """Ensure get_temp_file works as expected"""
         debug.trace(4, "test_get_temp_file()")
         assert isinstance(THE_MODULE.get_temp_file(), str)
 
     def test_remove_extension(self):
@@ -46,14 +50,15 @@
         assert THE_MODULE.remove_extension("/tmp/solr-4888.log", ".log") == "/tmp/solr-4888"
         assert THE_MODULE.remove_extension("/tmp/fubar.py", ".py") == "/tmp/fubar"
         assert THE_MODULE.remove_extension("/tmp/fubar.py", "py") == "/tmp/fubar."
 
     def test_dir_path(self):
         """Ensure dir_path works as expected"""
         debug.trace(4, "test_dir_path()")
+        debug.assertion(os.name == "posix")
         assert THE_MODULE.dir_path("/tmp/solr-4888.log") == "/tmp"
 
     def test_file_exists(self):
         """Ensure file_exists works as expected"""
         debug.trace(4, "test_file_exists()")
         # Existent file
         test_filename = gh.get_temp_file()
@@ -76,18 +81,29 @@
 
         # Test empty file
         empty_file = gh.get_temp_file()
         with open(empty_file, 'wb') as _:
             pass # gh.write_file cant be used because appends a newline
         assert not THE_MODULE.non_empty_file(empty_file)
 
+    @pytest.mark.xfail
     def test_form_path(self):
         """Ensure form_path works as expected"""
         debug.trace(4, "test_form_path()")
-        assert THE_MODULE.form_path("/home/", "User/Desktop", "file.txt") == "/home/User/Desktop/file.txt"
+        debug.assertion(os.name == "posix")
+        assert(THE_MODULE.form_path("/", "home", "User", "Desktop", "file.txt")
+               == "/home/User/Desktop/file.txt")
+        ## TEMP:
+        self.temp_file += "-test_form_path"
+        # Make sure can create directory        
+        test_temp_dir = THE_MODULE.form_path(self.temp_file, "test_dir")
+        test_temp_file = THE_MODULE.form_path(test_temp_dir, "test_file",
+                                              create=True)
+        assert(system.file_exists(test_temp_dir))
+        assert(not system.file_exists(test_temp_file))
 
     @pytest.mark.xfail
     def test_create_directory(self):
         """Ensure create_directory works as expected"""
         debug.trace(4, "test_create_directory()")
         assert False
 
@@ -97,14 +113,16 @@
         debug.trace(4, "test_full_mkdir()")
         assert False
 
     @pytest.mark.xfail
     def test_real_path(self):
         """Ensure real_path works as expected"""
         debug.trace(4, "test_real_path()")
+        debug.assertion(my_re.search("ubuntu", gh.run("uname -a"),
+                                     flags=my_re.IGNORECASE))
         assert THE_MODULE.real_path("/etc/mtab").startswith("/proc")
 
     def test_indent(self):
         """Ensure indent works as expected"""
         debug.trace(4, "test_indent()")
         test_text = 'this is an example text to be indented'
         tab_indented_text = '\tthis is an example text to be indented'
@@ -199,26 +217,30 @@
         assert not THE_MODULE.basename("fubar.py", "") == "fubar"
         assert THE_MODULE.basename("/tmp/solr-4888.log", ".log") == "solr-4888"
 
     def test_resolve_path(self):
         """Tests for resolve_path(filename)"""
         script = "glue_helpers.py"
         test_script = "test_glue_helpers.py"
+        test_dir = gh.dir_path(__file__)
+        debug.assertion(test_script in __file__)
         # The main script should resolve to parent directory but this one to test dir
-        assert not THE_MODULE.resolve_path(script) == path.join(path.dirname(__file__), test_script)
-        assert THE_MODULE.resolve_path(test_script) == path.join(path.dirname(__file__), test_script)
+        assert not (THE_MODULE.resolve_path(script)
+                    == gh.form_path(test_dir, test_script))
+        assert (THE_MODULE.resolve_path(test_script)
+                == gh.form_path(test_dir, test_script))
 
     @pytest.mark.xfail
     def test_heuristic_resolve_path(self):
         """Tests for heuristic version of resolve_path(filename)"""
         requirements_filename = "requirements.txt"
         # The requirements normally isn't resolved
         assert(THE_MODULE.resolve_path(requirements_filename, heuristic=False)
                == requirements_filename)
-        test_dir = path.dirname(__file__)
+        test_dir = gh.dir_path(__file__)
         assert(gh.real_path(THE_MODULE.resolve_path(requirements_filename, heuristic=True))
                == gh.real_path(gh.form_path(test_dir, "..", "..", requirements_filename)))
 
     def test_extract_match_from_text(self):
         """Ensure extract_match_from_text works as expected"""
         debug.trace(4, "test_extract_match_from_text()")
         assert THE_MODULE.extract_match_from_text(r"Mr. (\S+)", "Mr. Smith\nMr. Jones\nMr.X") == "Smith"
```

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_html_utils.py` & `mezcla-1.3.9.9/mezcla/tests/test_html_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_ipython_utils.py` & `mezcla-1.3.9.9/mezcla/tests/test_ipython_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_kenlm_example.py` & `mezcla-1.3.9.9/mezcla/tests/test_kenlm_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_keras_param_search.py` & `mezcla-1.3.9.9/mezcla/tests/test_keras_param_search.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_main.py` & `mezcla-1.3.9.9/mezcla/tests/test_main.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         app = Test(text_options=[("name", "Full name", "John Doe")],
                    boolean_options=[("verbose", "testing verbose option", True)],
                    runtime_args=[],
                    )
         #
         self.do_assert(app.parsed_args.get("name") == "John Doe")
         self.do_assert(app.parsed_args.get("verbose"))
-        debug.trace(5, f"out test_script_options")
+        debug.trace(5, "out test_script_options")
 
     @pytest.mark.xfail                   # TODO: remove xfail
     @trap_exception
     def test_script_without_input(self):
         """Makes sure script class without input doesn't process input and that
         the main step gets invoked"""
         debug.trace(4, f"in test_script_without_input(); self={self}")
@@ -105,46 +105,59 @@
             def run_main_step(self):
                 """Dummy main step"""
                 tpo.debug_format("in Test.run_main_step()): self={s}", 5,
                                  s=self)
                 TestMain.main_step_invoked = True
 
         # Test scriptlet with test script as input w/ and w/o input enabled
-        debug.trace_expr(6, "app1")
+        debug.trace(6, "app1")
         TestMain.input_processed = None
-        app1 = Test(skip_input=False, runtime_args=[__file__])
+        ## TEST: MAIN_SCRIPT = "main.py"         # TOOD3: derive from __file__
+        MAIN_SCRIPT = __file__
+        app1 = Test(skip_input=False, manual_input=False, runtime_args=[__file__], program=MAIN_SCRIPT)          # avoids pytest if invoked via it
         try:
             app1.run()
         except:
             tpo.print_stderr("Exception during app1.run: {exc}",
                              exc=tpo.to_string(sys.exc_info()))
         self.do_assert(TestMain.input_processed)
         #
         TestMain.input_processed = None
-        debug.trace_expr(6, "app2")
-        app2 = Test(skip_input=True, runtime_args=[__file__])
+        debug.trace(6, "app2")
+        ## NOTE: This produces an extraneous error, but the test class still executes:
+        ##   test_main.py: error: unrecognized arguments: tests/test_main.py
+        ## BAD:
+        app2 = Test(skip_input=True, manual_input=True, runtime_args=[__file__], program=MAIN_SCRIPT)          # avoids pytest if invoked via it
+        ## TODO2: app3 = Test(skip_input=True, manual_input=True, runtime_args=["-", "<", __file__], program=MAIN_SCRIPT)        # avoids pytest if invoked via it
         try:
             app2.run()
         except:
             tpo.print_stderr("Exception during app2.run: {exc}",
                              exc=tpo.to_string(sys.exc_info()))
         self.do_assert(not TestMain.input_processed)
 
-        # Test scriptlet w/ input disabled and wihout arguments
+        # Test scriptlet w/ input disabled and without arguments
         # note: auto_help disabled so that no arguments needed
         TestMain.main_step_invoked = None
-        debug.trace_expr(6, "app3")
+        debug.trace(6, "app3")
         app3 = Test(skip_input=True, manual_input=True, auto_help=False, runtime_args=[])
         try:
             app3.run()
         except:
             tpo.print_stderr("Exception during app3.run: {exc}",
                              exc=tpo.to_string(sys.exc_info()))
+        self.do_assert(not TestMain.input_processed)
         self.do_assert(TestMain.main_step_invoked)
-        debug.trace(5, f"out test_script_without_input")
+        
+        ## TODO2: Test scriptlet w/ all input disabled
+        ## # note: auto_help disabled so that no arguments needed
+        ## debug.trace(6, "app4")
+        ## app4 = Test(skip_input=True, manual_input=True, auto_help=False, runtime_args=[])
+        ## ...
+        debug.trace(5, "out test_script_without_input")
 
     @pytest.mark.xfail                   # TODO: remove xfail
     @trap_exception
     def test_perl_arg(self):
         """Make sure perl-style arg can be parsed"""
         # TODO: create generic app-creation helper
         debug.trace(4, f"in test_perl_arg(); self={self}")
@@ -159,15 +172,15 @@
         #
         self.do_assert(app.parsed_args.get("verbose") == 0)
         #
         app = Test(boolean_options=[("verbose", "testing verbose option")],
                    runtime_args=[], perl_switch_parsing=False)
         # NOTE: this ensures that is None and not 0
         self.do_assert(app.parsed_args.get("verbose") is None)
-        debug.trace(5, f"out test_perl_arg")
+        debug.trace(5, "out test_perl_arg")
 
 
 class TestMain2:
     """Another class for testcase definition
     Note: Needed to avoid error with pytest due to inheritance with unittest.TestCase via TestWrapper (e.g., capsys)"""
 
     @pytest.mark.xfail                   # TODO: remove xfail
@@ -197,15 +210,15 @@
         monkeypatch.setattr('sys.stdin', io.StringIO(contents))
         main = THE_MODULE.Main(file_input_mode=True, skip_args=True, auto_help=False)
         main.run()
         captured = capsys.readouterr()
         ## TODO: assert(TestMain.process_line_count == 1)
         assert(num_lines == len(captured.out.split("\n")))
         debug.trace_expr(5, main, num_lines, pre_captured)
-        debug.trace(5, f"out test_input_modes")
+        debug.trace(5, "out test_input_modes")
 
     @pytest.mark.xfail                   # TODO: remove xfail
     def test_missing_newline(self, capsys, monkeypatch):
         """Make sure file with missing newline at end processed OK"""
         debug.trace(4, f"in test_missing_newline({capsys}); self={self}")
         contents = "1\n2\n3"
         num_lines = len(contents.split("\n"))
@@ -215,25 +228,25 @@
         main.run()
         captured = capsys.readouterr()
         # note: 1 extra line ('') and 1 extra character (final newline)
         assert((1 + num_lines) == len(captured.out.split("\n")))
         assert((1 + len(contents)) == len(captured.out))
         ## TODO: self.do_assert(TestMain.process_line_count == 3)
         debug.trace_expr(5, main, num_lines)
-        debug.trace(5, f"out test_missing_newline")
+        debug.trace(5, "out test_missing_newline")
 
     def test_has_parsed_option_hack(self):
         """Make sure (temporarily hacked) has_parsed_option differs from has_parsed_option_old"""
         debug.trace(4, f"in test_has_parsed_option_hack(); self={self}")
         ok_arg = "ok"
         missing_arg = "missing"
         main = THE_MODULE.Main(skip_args=True, auto_help=False)
         main.parsed_args = {ok_arg: True}
         assert(main.has_parsed_option_old(ok_arg) == main.has_parsed_option(ok_arg))
         assert(main.has_parsed_option_old(missing_arg) != main.has_parsed_option(missing_arg))
-        debug.trace(5, f"out test_has_parsed_option_hack")
+        debug.trace(5, "out test_has_parsed_option_hack")
 
 #------------------------------------------------------------------------
 
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_merge_files.py` & `mezcla-1.3.9.9/mezcla/tests/test_merge_files.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_merge_notes.py` & `mezcla-1.3.9.9/mezcla/tests/test_merge_notes.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_misc_utils.py` & `mezcla-1.3.9.9/mezcla/tests/test_misc_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,36 +8,41 @@
 # - This can be run as follows:
 #   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_misc_utils.py
 #
 
 """Tests for misc_utils module"""
 
 # Standard packages
+import math
+import datetime
+import time
 ## NOTE: this is empty for now
 
 # Installed packages
 import pytest
 
 # Local packages
 from mezcla import glue_helpers as gh
 from mezcla import debug
+from mezcla import system
+from mezcla.unittest_wrapper import TestWrapper
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 import mezcla.misc_utils as THE_MODULE
 
 # Make sure more_itertools available
-has_more_itertools = True
+HAS_MORE_ITERTOOLS = True
 try:
     import more_itertools
-except:
+except ImportError:
     system.print_exception_info("more_itertools import")
-    has_more_itertools = False
+    HAS_MORE_ITERTOOLS = False
 
-class TestMiscUtils:
+class TestMiscUtils(TestWrapper):
     """Class for test case definitions"""
 
     def test_transitive_closure(self):
         """Ensure transitive_closure works as expected"""
         debug.trace(4, "test_transitive_closure()")
 
         actual = THE_MODULE.transitive_closure([(1, 2), (2, 3), (3, 4)])
@@ -51,48 +56,48 @@
             'language\tPython\n' +
             'framework\tPytest\n'
         )
         dict_table = {
             'language': 'Python\n',
             'framework': 'Pytest\n',
         }
-        temp_file = gh.get_temp_file()
+        temp_file = self.get_temp_file()
         gh.write_file(temp_file, string_table)
         assert THE_MODULE.read_tabular_data(temp_file) == dict_table
 
     def test_extract_string_list(self):
         """Ensure extract_string_list works as expected"""
         debug.trace(4, "test_extract_string_list()")
         assert THE_MODULE.extract_string_list("1  2,3") == ['1', '2', '3']
 
     def test_is_prime(self):
         """Ensure is_prime works as expected"""
         debug.trace(4, "test_is_prime()")
 
-        FIRST_100_PRIMES = [
+        first_100_primes = [
             2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37,
             41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83,
             89, 97, 101, 103, 107, 109, 113, 127, 131,
             137, 139, 149, 151, 157, 163, 167, 173, 179,
             181, 191, 193, 197, 199, 211, 223, 227, 229,
             233, 239, 241, 251, 257, 263, 269, 271, 277,
             281, 283, 293, 307, 311, 313, 317, 331, 337,
             347, 349, 353, 359, 367, 373, 379, 383, 389,
             397, 401, 409, 419, 421, 431, 433, 439, 443,
             449, 457, 461, 463, 467, 479, 487, 491, 499,
             503, 509, 521, 523, 541,
         ]
 
-        assert all([THE_MODULE.is_prime(n) for n in FIRST_100_PRIMES])
-        assert all([(not THE_MODULE.is_prime(n)) for n in range(FIRST_100_PRIMES[-1])  if n not in FIRST_100_PRIMES])
+        assert all(THE_MODULE.is_prime(n) for n in first_100_primes)
+        assert all((not THE_MODULE.is_prime(n)) for n in range(first_100_primes[-1]) if n not in first_100_primes)
 
     def test_fibonacci(self):
         """Ensure fibonacci works as expected"""
         debug.trace(4, "test_fibonacci()")
-        assert THE_MODULE.fibonacci(-5) == []
+        assert not THE_MODULE.fibonacci(-5)
         assert THE_MODULE.fibonacci(1) == [0]
         assert THE_MODULE.fibonacci(10) == [0, 1, 1, 2, 3, 5, 8]
 
     def test_sort_weighted_hash(self):
         """Ensure sort_weighted_hash works as expected"""
         debug.trace(4, "test_sort_weighted_hash()")
         test_hash = {
@@ -121,70 +126,129 @@
         assert THE_MODULE.unzip(zip([], []), 2) == [[], []]
         assert THE_MODULE.unzip(zip(), 4) == [[], [], [], []]
         assert THE_MODULE.unzip(zip(), 4) != [[], []]
 
     def test_get_current_frame(self):
         """Ensure get_current_frame works as expected"""
         debug.trace(4, "test_get_current_frame()")
-        ## TODO: WORK-IN-PROGRESS
+        stack = str(THE_MODULE.get_current_frame())
+        test_name = system.get_current_function_name()
+        assert f'code {test_name}' in stack
+        assert __file__ in stack
 
     def test_eval_expression(self):
         """Ensure eval_expression works as expected"""
         debug.trace(4, "test_eval_expression()")
         assert THE_MODULE.eval_expression("len([123, 321]) == 2")
         assert not THE_MODULE.eval_expression("'helloworld' == 2")
 
-    def test_trace_named_object(self, capsys):
+    def test_trace_named_object(self):
         """Ensure trace_named_object works as expected"""
         debug.trace(4, "test_trace_named_object()")
         # With level -1 we ensure that the trace will be printed
         THE_MODULE.trace_named_object(-1, "sys.argv")
-        captured = capsys.readouterr()
-        assert "sys.argv" in captured.err
+        captured = self.get_stderr()
+        assert "sys.argv" in captured
 
-    def test_trace_named_objects(self, capsys):
+    def test_trace_named_objects(self):
         """Ensure trace_named_objects works as expected"""
         debug.trace(4, "test_trace_named_objects()")
         # With level -1 we ensure that the trace will be printed
         THE_MODULE.trace_named_objects(-1, "[len(sys.argv), sys.argv]")
-        captured = capsys.readouterr()
-        assert "len(sys.argv)" in captured.err
-        assert "sys.argv" in captured.err
+        captured = self.get_stderr()
+        assert "len(sys.argv)" in captured
+        assert "sys.argv" in captured
 
-    @pytest.mark.skipif(not has_more_itertools, reason="Unable to load more_itertools")
+    @pytest.mark.skipif(not HAS_MORE_ITERTOOLS, reason="Unable to load more_itertools")
     def test_exactly1(self):
         """Ensure exactly1 works as expected"""
         debug.trace(4, "test_exactly1()")
         assert THE_MODULE.exactly1([False, False, True])
         assert not THE_MODULE.exactly1([False, True, True])
         assert not THE_MODULE.exactly1([False, False, False])
         assert not THE_MODULE.exactly1([])
 
     def test_string_diff(self):
         """Ensure string_diff works as expected"""
         debug.trace(4, "test_string_diff()")
 
-        STRING_ONE = 'one\ntwo\nthree\nfour'
-        STRING_TWO = 'one\ntoo\ntree\nfour'
-        EXPECTED_DIFF = (
+        string_one = 'one\ntwo\nthree\nfour'
+        string_two = 'one\ntoo\ntree\nfour'
+        expected_diff = (
             '  one\n'
             '< two\n'
             '…  ^\n'
             '> too\n'
             '…  ^\n'
             '< three\n'
             '…  -\n'
             '> tree\n'
             '  four\n'
         )
 
-        assert THE_MODULE.string_diff(STRING_ONE, STRING_TWO) == EXPECTED_DIFF
+        assert THE_MODULE.string_diff(string_one, string_two) == expected_diff
+
 
     def test_elide_string_values(self):
         """Ensure elide_string_values works as expected"""
         debug.trace(4, "test_elide_string_values()")
-        ## TODO: WORK-IN-PROGRESS
+        hello = "hello"
+        assert 'hell...' == THE_MODULE.elide_string_values(hello, max_len=4)
 
+    def test_is_close(self):
+        """ensure is_close works as expected"""
+        debug.trace(4, "test_is_close()")
+        assert     THE_MODULE.is_close(1.0 + 0.999 , 2.0, 0.001)
+        assert not THE_MODULE.is_close(1.0 + 0.999 , 2.0, 0.0001)
+
+    def test_get_date_ddmmmyy(self):
+        """ensure get_date_ddmmmyy works as expected"""
+        debug.trace(4, "test_get_date_ddmmmyy()")
+        assert THE_MODULE.get_date_ddmmmyy(datetime.date(2004, 9, 16)) == '16sep04'
+
+    def test_parse_timestamp(self):
+        """ensure parse_timestamp works as expected"""
+        debug.trace(4, "test_parse_timestamp()")
+        ts = datetime.datetime(2004, 9, 16, 12, 30, 25, 123123)
+        ts_iso = '2004-09-16T12:30:25.1231234Z'
+        ts_iso_2 = '2004-09-16T12:30:25.123123Z'
+        parsed_ts = THE_MODULE.parse_timestamp(ts_iso, truncate=True)
+        parsed_ts_truncated = THE_MODULE.parse_timestamp(ts_iso_2, truncate=False)
+        assert parsed_ts == ts
+        assert parsed_ts_truncated == ts
+
+    def test_add_timestamp_diff(self):
+        """ensure add_timestamp_diff works as expected"""
+        debug.trace(4, "test_add_timestamp_diff()")
+        timestamp = "timestamp 2004-09-16T12:30:25.1231234Z"
+        file_in = f"{self.temp_file}.in"
+        file_out = f"{self.temp_file}.out"
+        system.write_file(file_in, timestamp)
+        THE_MODULE.add_timestamp_diff(file_in, file_out)
+        contents = system.read_file(file_out)
+        assert contents == f"{timestamp} [0]\n"
+
+    def test_random_int(self):
+        """ensure random_int works as expected"""
+        debug.trace(4, "test_random_int()")
+        assert 0 <= THE_MODULE.random_int(0,4) <= 4
+
+    def test_random_float(self):
+        """ensure random_float works as expected"""
+        debug.trace(4, "test_random_float()")
+        assert 0 <= THE_MODULE.random_float(0,4.3) < 4.3
+
+    def test_time_function(self):
+        """ensure time_function works as expected"""
+        debug.trace(4, "test_time_function()")
+        ms = THE_MODULE.time_function(time.sleep, 0.25)
+        assert math.floor(ms) == 250
+
+    def test_get_class_from_name(self):
+        """ensure get_class_from_name works as expected"""
+        debug.trace(4, "test_get_class_from_name()")
+        result_class = THE_MODULE.get_class_from_name('date', 'datetime')
+        assert result_class is datetime.date
 
 if __name__ == '__main__':
     debug.trace_current_context()
     pytest.main([__file__])
```

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_my_regex.py` & `mezcla-1.3.9.9/mezcla/tests/test_my_regex.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_ngram_tfidf.py` & `mezcla-1.3.9.9/mezcla/tests/test_ngram_tfidf.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_os_utils.py` & `mezcla-1.3.9.9/mezcla/tests/test_os_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_pandas_sklearn.py` & `mezcla-1.3.9.9/mezcla/tests/test_pandas_sklearn.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_plot_utils.py` & `mezcla-1.3.9.9/mezcla/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_python_ast.py` & `mezcla-1.3.9.9/mezcla/tests/test_python_ast.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_randomize_lines.py` & `mezcla-1.3.9.9/mezcla/tests/test_randomize_lines.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_rgb_color_name.py` & `mezcla-1.3.9.9/mezcla/tests/test_rgb_color_name.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_run_albert_classifier.py` & `mezcla-1.3.9.9/mezcla/tests/test_run_albert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_run_bert_classifier.py` & `mezcla-1.3.9.9/mezcla/tests/test_run_bert_classifier.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_show_bert_representation.py` & `mezcla-1.3.9.9/mezcla/tests/test_show_bert_representation.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_simple_main_example.py` & `mezcla-1.3.9.9/mezcla/tests/test_simple_main_example.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_spacy_nlp.py` & `mezcla-1.3.9.9/mezcla/tests/test_spacy_nlp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_spell.py` & `mezcla-1.3.9.9/mezcla/tests/test_spell.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_sys_version_info_hack.py` & `mezcla-1.3.9.9/mezcla/tests/test_sys_version_info_hack.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_system.py` & `mezcla-1.3.9.9/mezcla/tests/test_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,31 +13,33 @@
 
 # Standard packages
 import io
 from math import pi
 import time
 import sys
 import re
+import pickle
 
 # Installed packages
 import pytest
-import pickle
 
 # Local packages
 from mezcla.unittest_wrapper import TestWrapper
+from mezcla.unittest_wrapper import trap_exception
 from mezcla import glue_helpers as gh
 from mezcla.my_regex import my_re
 from mezcla import debug
 
 # Note: Two references are used for the module to be tested:
 #    THE_MODULE:	    global module object
 import mezcla.system as THE_MODULE
 
 class TestSystem(TestWrapper):
     """Class for test case definitions"""
+    script_module = None
 
     def test_maxint(self):
         """Ensure maxint works as expected"""
         debug.trace(4, "test_maxint()")
 
         assert THE_MODULE.maxint() is not None
         assert THE_MODULE.maxint() == sys.maxsize
@@ -170,15 +172,15 @@
     def test_get_exception(self):
         """Ensure get_exception works as expected"""
         debug.trace(4, "test_get_exception()")
         exception = None
         try:
             raise RuntimeError("testing")
         except RuntimeError:
-            exception = THE_MODULE.get_exception() 
+            exception = THE_MODULE.get_exception()
         assert str(exception[1]) == "testing"
 
     def test_print_error(self):
         """Ensure print_error works as expected"""
         debug.trace(4, "test_print_error()")
         THE_MODULE.print_error("this is an test error message")
         captured = self.get_stderr()
@@ -195,55 +197,58 @@
         """Ensure print_exception_info works as expected"""
         debug.trace(4, "test_print_exception_info()")
         THE_MODULE.print_exception_info("Foobar")
         captured = self.get_stderr()
         assert "Foobar" in captured
 
     @pytest.mark.xfail
+    @trap_exception                     # TODO: remove when debugged
     def test_exit(self):
         """Ensure exit works as expected"""
+        # Note: This modifies sys.exit so that system.exit doesn't really exit.
         debug.trace(4, "test_exit()")
-        def sys_exit_mock():
-            return 'exit'
-        ## BAD: self.set_attr(sys, "exit", sys_exit_mock)
+        #
+        EXIT = 'exit'
+        def sys_exit_mock(_status=None):
+            """Stub for sys.exit that just returns 'exit' text"""
+            debug.trace(4, "sys_exit_mock()")
+            return EXIT
+        #
         self.monkeypatch.setattr(sys, "exit", sys_exit_mock)
-        assert THE_MODULE.exit('test exit {method}', method='method') == 'exit'
+        MESSAGE = "test_exit method"
+        self.do_assert(THE_MODULE.exit(MESSAGE) == EXIT)
         # Exit is mocked, ignore code editor hidding
         captured = self.get_stderr()
-        assert "test exit method" in captured
+        self.do_assert(MESSAGE in captured)
 
     def test_setenv(self):
         """Ensure setenv works as expected"""
         debug.trace(4, "test_setenv()")
         THE_MODULE.setenv('NEW_TEST_ENV_VAR', 'the gravity is 10, pi is 3')
         assert THE_MODULE.getenv('NEW_TEST_ENV_VAR') == 'the gravity is 10, pi is 3'
 
     def test_print_full_stack(self):
         """Ensure print_full_stack works as expected"""
         debug.trace(4, "test_print_full_stack()")
-        def raiseException():
-            raise RuntimeError('test')
         try:
-            raiseException()
+            raise RuntimeError('test')
         except RuntimeError:
             THE_MODULE.print_full_stack(sys.stderr)
-        capturedError = self.get_stderr()
-        assert 'RuntimeError' in capturedError
+        captured_error = self.get_stderr()
+        assert 'RuntimeError' in captured_error
 
     def test_trace_stack(self):
         """Ensure trace_stack works as expected"""
         debug.trace(4, "test_trace_stack()")
-        def raiseException():
-            raise RuntimeError('test')
         try:
-            raiseException()
+            raise RuntimeError('test')
         except RuntimeError:
             THE_MODULE.trace_stack(1, sys.stderr)
-        capturedError = self.get_stderr()
-        assert 'RuntimeError' in capturedError
+        captured_error = self.get_stderr()
+        assert 'RuntimeError' in captured_error
 
     def test_get_current_function_name(self):
         """Ensure get_current_function_name works as expected"""
         debug.trace(4, "test_get_current_function_name()")
         assert THE_MODULE.get_current_function_name() == "test_get_current_function_name"
 
     def test_open_file(self):
@@ -263,32 +268,32 @@
             1: 'first',
             2: 'second',
         }
         test_filename = gh.get_temp_file()
 
         THE_MODULE.save_object(test_filename, test_dict)
 
-        test_file = open(test_filename, 'rb')
-        actual_object = pickle.load(test_file)
+        with open(test_filename, 'rb') as test_file:
+            actual_object = pickle.load(test_file)
         assert actual_object == test_dict
         test_file.close()
 
     def test_load_object(self):
         """Ensure load_object works as expected"""
         debug.trace(4, "test_load_object()")
 
         # Test valid file
         test_dict = {
             1: 'first',
             2: 'second',
         }
         test_filename = gh.get_temp_file()
-        test_file = open(test_filename, 'wb')
-        pickle.dump(test_dict, test_file)
-        test_file.close()
+        with open(test_filename, 'wb') as test_file :
+            pickle.dump(test_dict, test_file)
+            test_file.close()
         assert THE_MODULE.load_object(test_filename) == test_dict
 
         # Test invalid file
         THE_MODULE.load_object('bad_file_name')
         captured = self.get_stderr()
         assert "Error:" in captured
 
@@ -389,15 +394,15 @@
 
     def test_read_directory(self):
         """Ensure read_directory works as expected"""
         debug.trace(4, "test_read_directory()")
         split = gh.create_temp_file('').split('/')
         path = '/'.join(split[:-1])
         filename = split[-1]
-        assert filename in THE_MODULE.read_directory(path) 
+        assert filename in THE_MODULE.read_directory(path)
 
     def test_get_directory_filenames(self):
         """Ensure get_directory_filenames works as expected"""
         debug.trace(4, "test_get_directory_filenames()")
         assert "/etc/passwd" in THE_MODULE.get_directory_filenames("/etc")
         assert "/boot" not in THE_MODULE.get_directory_filenames("/", just_regular_files=True)
 
@@ -518,15 +523,14 @@
     def test_write_binary_file(self):
         """Ensure write_binary_file works as expected"""
         debug.trace(4, "test_write_binary_file()")
         filename = gh.get_temp_file()
         THE_MODULE.write_binary_file(filename, bytes("binary", "UTF-8"))
         assert THE_MODULE.read_binary_file(filename) == b'binary'
 
-        
     def test_write_lines(self):
         """Ensure write_lines works as expected"""
         debug.trace(4, "test_write_lines()")
 
         content = (
             'this is\n'
             'a multiline\n'
@@ -561,21 +565,21 @@
         # create two temp files at the same time
         filedir1 = gh.create_temp_file('test modified time')
         filedir2 = gh.create_temp_file('test modified time2')
         # get the modification time of the files
         timestamp1 = THE_MODULE.get_file_modification_time(filedir1)[:19]
         timestamp2 = THE_MODULE.get_file_modification_time(filedir2)[:19]
         # get and format local time
-        timestampNow = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
+        now = time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
 
-        # test timestamps are equal 
+        # test timestamps are equal
         assert timestamp1 == timestamp2
 
         # test timestamp is equal to actual time (ignoring miliseconds)
-        assert timestamp1 == timestampNow
+        assert timestamp1 == now
 
     def test_remove_extension(self):
         """Ensure remove_extension works as expected"""
         debug.trace(4, "test_remove_extension()")
         assert THE_MODULE.remove_extension("/tmp/document.pdf") == "/tmp/document"
         assert THE_MODULE.remove_extension("it.abc.def") == "it.abc"
         assert THE_MODULE.remove_extension("it.abc.def", "abc.def") == "it"
@@ -600,15 +604,15 @@
         gh.write_file(temp_file, 'content')
         assert THE_MODULE.get_file_size(temp_file) == 8
         assert THE_MODULE.get_file_size('non-existent-file.txt') == -1
 
     def test_form_path(self):
         """Ensure form_path works as expected"""
         debug.trace(4, "test_form_path()")
-        assert THE_MODULE.form_path('/usr', 'bin', 'cat') == '/usr/bin/cat'  
+        assert THE_MODULE.form_path('/usr', 'bin', 'cat') == '/usr/bin/cat'
 
     def test_is_directory(self):
         """Ensure is_directory works as expected"""
         debug.trace(4, "test_is_directory()")
         assert THE_MODULE.is_directory("/etc")
 
     def test_is_regular_file(self):
@@ -625,15 +629,16 @@
         path = '/tmp/mezcla_test'
         THE_MODULE.create_directory('/tmp/mezcla_test')
         assert THE_MODULE.is_directory(path)
 
     def test_get_current_directory(self):
         """Ensure get_current_directory works as expected"""
         debug.trace(4, "test_get_current_directory()")
-        assert '/home/' in THE_MODULE.get_current_directory()
+        ## BAD: assert '/home/' in THE_MODULE.get_current_directory()
+        assert 'mezcla' in THE_MODULE.get_current_directory()
 
     def test_set_current_directory(self):
         """Ensure set_current_directory works as expected"""
         debug.trace(4, "test_set_current_directory()")
         past_dir = THE_MODULE.get_current_directory()
         assert THE_MODULE.set_current_directory('/home') is None
         assert THE_MODULE.get_current_directory() == '/home'
@@ -654,15 +659,15 @@
 
     def test_from_utf8(self):
         """Ensure from_utf8 works as expected"""
         debug.trace(4, "test_from_utf8()")
         assert THE_MODULE.from_utf8("\xBF") == "\u00BF"
         # assert THE_MODULE.to_unicode("\xEF\xBB\xBF") == "\ufeff"
         # Lorenzo: can't convert "\ufeff" to BOM, but can convert "\xEF\xBB\xBF"
-    
+
     def test_to_unicode(self):
         """Ensure to_unicode works as expected"""
         debug.trace(4, "test_to_unicode()")
         assert THE_MODULE.to_unicode("\xEF\xBB\xBF") == "\xEF\xBB\xBF"
         ## TODO: add tests for sys.version_info.major < 3
         # assert THE_MODULE.to_unicode("\xEF\xBB\xBF") == "\ufeff"
 
@@ -714,15 +719,14 @@
         assert THE_MODULE.absolute_path("/etc/mtab").startswith("/etc")
 
     def test_real_path(self):
         """Ensure real_path works as expected"""
         debug.trace(4, "test_real_path()")
         assert THE_MODULE.real_path("/etc/mtab").startswith("/proc")
 
-    @pytest.mark.xfail
     def test_get_module_version(self):
         """Ensure get_module_version works as expected"""
         debug.trace(4, "test_get_module_version()")
         num_good = 0
         num_total = 0
         for line in gh.run("pip freeze").splitlines():
             if my_re.search(r"(\S+)==(\S+)", line):
@@ -730,15 +734,15 @@
                 module, version = my_re.groups()
                 if version == THE_MODULE.get_module_version(module):
                     num_good += 1
             else:
                 debug.trace(4, f"Ignoring pip freeze line: {line}")
         percent = (num_good / num_total * 100) if num_total else 0
         debug.trace_expr(5, num_good, num_total, percent)
-        assert (percent >= 90)
+        assert percent >= 90
 
     def test_intersection(self):
         """Ensure intersection works as expected"""
         debug.trace(4, "test_intersection()")
         assert THE_MODULE.intersection([1, 2], [5, 7, 8]) == []
         assert THE_MODULE.intersection([1, 2, 3, 4, 5], [2, 4]) == [2, 4]
         assert THE_MODULE.intersection([1, 2], [5, 7, 8], as_set=True) == set()
```

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_template.py` & `mezcla-1.3.9.9/mezcla/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_text_categorizer.py` & `mezcla-1.3.9.9/mezcla/tests/test_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_text_processing.py` & `mezcla-1.3.9.9/mezcla/tests/test_text_processing.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_text_utils.py` & `mezcla-1.3.9.9/mezcla/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_tpo_common.py` & `mezcla-1.3.9.9/mezcla/tests/test_tpo_common.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,31 +3,38 @@
 #
 # Test(s) for tpo_common.py
 #
 # Notes:
 # - This can be run as follows:
 #   $ PYTHONPATH=".:$PYTHONPATH" python ./mezcla/tests/test_tpo_common.py
 #
+# Warning:
+# - *** The tpo_common.py module is being phased out. Although there are
+#   a bunch of "work-in-progress" tests below, they are low priority because
+#   most are addressed by test_system.py or test_debug.py.
+#
 # TODO:
 # - Address commonly used debugging functions (e.g., debug_print) by redirecting output (via remapping sys.stderr to a file) and then checking file contents.
 # - add tests for normalize_unicode, ensure_unicode and other problematic functions
 #
 # Important:
 # - Most of the methods on tpo_common was moved to predecessors modules as system.py, debug.py etc.
 # - Using the predecessors module tests to these moved methods could be useful to avoid repeated tests but this could create conflicts with modified methods.
 #
 
 """Tests for tpo_common module"""
 
 # Standard modules
 import sys
+import re
 
 # Installed modules
 import pytest
 import pickle
+import trace
 
 # Local modules
 from mezcla import debug
 from mezcla import glue_helpers as gh
 from mezcla.unittest_wrapper import TestWrapper
 from mezcla.unittest_wrapper import trap_exception
 
@@ -56,15 +63,24 @@
         debug.trace(4, "test_debugging_level()")
         THE_MODULE.set_debug_level(5)
         assert THE_MODULE.debugging_level() == 5
 
     def test_debug_trace_without_newline(self):
         """Ensure debug_trace_without_newline works as expected"""
         debug.trace(4, "test_debug_trace_without_newline()")
-        ## TODO: WORK-IN-PROGRESS
+        tracer = trace.Trace(countfuncs=1)
+        tracer.runfunc(THE_MODULE.debug_trace_without_newline, ('test debug trace withouht newline'))
+        
+        # redirect write_results to temp file
+        temp = self.get_temp_file()
+        tracer.results().write_results(coverdir=temp)
+        
+        captured = self.get_stdout()
+        assert re.search(r'modulename: debug, funcname: trace', captured)
+
 
     def test_debug_trace(self):
         """Ensure debug_trace works as expected"""
         debug.trace(4, "test_debug_trace()")
         ## TODO: WORK-IN-PROGRESS
 
     def test_debug_print(self):
@@ -76,60 +92,121 @@
         """Ensure debug_format works as expected"""
         debug.trace(4, "test_debug_format()")
         ## TODO: WORK-IN-PROGRESS
 
     def test_debug_timestamp(self):
         """Ensure debug_timestamp works as expected"""
         debug.trace(4, "test_debug_timestamp()")
-        ## TODO: WORK-IN-PROGRESS
+        tracer = trace.Trace(countfuncs=1)
+        tracer.runfunc(THE_MODULE.debug_timestamp)
+        
+        # redirect write_results to temp file
+        temp = self.get_temp_file()
+        tracer.results().write_results(coverdir=temp)
+        
+        captured = self.get_stdout()
+        assert re.search(r'modulename: debug, funcname: timestamp', captured)
 
+    @trap_exception
     def test_debug_raise(self):
         """Ensure debug_raise works as expected"""
         debug.trace(4, "test_debug_raise()")
-        ## TODO: WORK-IN-PROGRESS
+        tracer = trace.Trace(countfuncs=1)
+        try:
+            raise RuntimeError
+        except RuntimeError:
+            with pytest.raises(RuntimeError):
+                tracer.runfunc(THE_MODULE.debug_raise)
+        
+        # redirect write_results to temp file
+        temp = self.get_temp_file()
+        tracer.results().write_results(coverdir=temp)
+        
+        captured = self.get_stdout()
+        assert re.search(r'modulename: debug, funcname: raise_exception', captured)
+
 
     def test_trace_array(self):
         """Ensure trace_array works as expected"""
         debug.trace(4, "test_trace_array()")
-        ## TODO: WORK-IN-PROGRESS
+        tracer = trace.Trace(countfuncs=1)
+        tracer.runfunc(THE_MODULE.trace_array, (['test', 'trace', 'array']))
+        
+        # redirect write_results to temp file
+        temp = self.get_temp_file()
+        tracer.results().write_results(coverdir=temp)
+        
+        captured = self.get_stdout()
+        assert re.search(r'modulename: debug, funcname: trace_values', captured)
 
     def test_trace_object(self):
         """Ensure trace_object works as expected"""
         debug.trace(4, "test_trace_object()")
-        ## TODO: WORK-IN-PROGRESS
+        tracer = trace.Trace(countfuncs=1)
+        tracer.runfunc(THE_MODULE.trace_object, ('test_trace_object'), show_methods_etc=True)
+        
+        # redirect write_results to temp file
+        temp = self.get_temp_file()
+        tracer.results().write_results(coverdir=temp)
+        
+        captured = self.get_stdout()
+        assert re.search(r'modulename: debug, funcname: trace_object', captured)
+        
 
     def test_trace_value(self):
         """Ensure trace_value works as expected"""
         debug.trace(4, "test_trace_value()")
         ## TODO: WORK-IN-PROGRESS
 
     def test_trace_current_context(self):
         """Ensure trace_current_context works as expected"""
         debug.trace(4, "test_trace_current_context()")
-        ## TODO: WORK-IN-PROGRESS
+        tracer = trace.Trace(countfuncs=1)
+        tracer.runfunc(THE_MODULE.trace_current_context, show_methods_etc=True)
+        
+        # redirect write_results to temp file
+        temp = self.get_temp_file()
+        tracer.results().write_results(coverdir=temp)
+        
+        captured = self.get_stdout()
+        assert re.search(r'modulename: debug, funcname: trace_current_context', captured)
 
     def test_during_debugging(self):
         """Ensure during_debugging works as expected"""
         debug.trace(4, "test_during_debugging()")
+
         ## TODO: WORK-IN-PROGRESS
 
     def test_debugging(self):
         """Ensure debugging works as expected"""
         debug.trace(4, "test_debugging()")
-        ## TODO: WORK-IN-PROGRESS
+        THE_MODULE.set_debug_level(4)
+        assert THE_MODULE.debugging(2)
+        assert THE_MODULE.debugging(4)
+        assert not THE_MODULE.debugging(6)
 
     def test_detailed_debugging(self):
         """Ensure detailed_debugging works as expected"""
         debug.trace(4, "test_detailed_debugging()")
-        ## TODO: WORK-IN-PROGRESS
+        THE_MODULE.set_debug_level(2)
+        assert not THE_MODULE.detailed_debugging()
+        THE_MODULE.set_debug_level(4)
+        assert THE_MODULE.detailed_debugging()
+        THE_MODULE.set_debug_level(6)
+        assert THE_MODULE.detailed_debugging()
 
     def test_verbose_debugging(self):
         """Ensure verbose_debugging works as expected"""
         debug.trace(4, "test_verbose_debugging()")
-        ## TODO: WORK-IN-PROGRESS
+        THE_MODULE.set_debug_level(2)
+        assert not THE_MODULE.verbose_debugging()
+        THE_MODULE.set_debug_level(5)
+        assert THE_MODULE.verbose_debugging()
+        THE_MODULE.set_debug_level(7)
+        assert THE_MODULE.verbose_debugging()
 
     def test_to_string(self):
         """Ensure to_string works as expected"""
         debug.trace(4, "test_to_string()")
         assert THE_MODULE.to_string(123) == "123"
         assert THE_MODULE.to_string("\u1234") == "\u1234"
         assert THE_MODULE.to_string(None) == "None"
@@ -290,29 +367,29 @@
     def test_load_object(self):
         """Ensure load_object works as expected"""
         debug.trace(4, "test_load_object()")
         test_dict = {
             1: 'first',
             2: 'second',
         }
-        test_filename = gh.get_temp_file()
+        test_filename = self.get_temp_file()
         test_file = open(test_filename, 'wb')
         pickle.dump(test_dict, test_file)
         test_file.close()
 
         assert THE_MODULE.load_object(test_filename) == test_dict
 
     def test_store_object(self):
         """Ensure store_object works as expected"""
         debug.trace(4, "test_store_object()")
         test_dict = {
             1: 'first',
             2: 'second',
         }
-        test_filename = gh.get_temp_file()
+        test_filename = self.get_temp_file()
 
         THE_MODULE.store_object(test_filename, test_dict)
 
         test_file = open(test_filename, 'rb')
         actual_object = pickle.load(test_file)
         assert actual_object == test_dict
         test_file.close()
@@ -323,15 +400,15 @@
 
         ## TODO: add tests related to redirect_stderr and restore_stderr
 
         test_dict = {
             1: 'first',
             2: 'second',
         }
-        test_filename = gh.get_temp_file()
+        test_filename = self.get_temp_file()
 
         THE_MODULE.store_object(test_filename, test_dict)
 
         test_file = open(test_filename, 'rb')
         actual_object = pickle.load(test_file)
         assert actual_object == test_dict
         test_file.close()
@@ -362,15 +439,15 @@
         )
         expected = {
             'emailentered - someemail@hotmail.com': True,
             'passwdentered - 12345': True,
             'isbusiness - true': True,
         }
 
-        temp_file = gh.get_temp_file()
+        temp_file = self.get_temp_file()
         gh.write_file(temp_file, content)
         assert THE_MODULE.create_boolean_lookup_table(temp_file) == expected
 
     def test_normalize_frequencies(self):
         """Ensure normalize_frequencies works as expected"""
         debug.trace(4, "test_normalize_frequencies()")
         ## TODO: WORK-IN-PROGRESS
@@ -503,85 +580,79 @@
         ## TODO: WORK-IN-PROGRESS
 
     def test_memodict(self):
         """Ensure memodict works as expected"""
         debug.trace(4, "test_memodict()")
         ## TODO: WORK-IN-PROGRESS
 
-
-class TestTpoCommon2:
-    """Another class for testcase definition
-    Note: works around silly issues with pytest and TestWrapper (e.g., capsys and monkeypatch)
-    """
-
     @pytest.mark.xfail                   # TODO: remove xfail
-    def test_exit(self, monkeypatch, capsys):
+    def test_exit(self):
         """Ensure exit works as expected"""
         debug.trace(4, "test_exit()")
         def sys_exit_mock():
             return 'exit'
-        monkeypatch.setattr(sys, "exit", sys_exit_mock)
+        self.monkeypatch.setattr(sys, "exit", sys_exit_mock)
         assert THE_MODULE.exit('test exit method') == 'exit'
         # Exit is mocked, ignore code editor hiding
         ## TODO: for some reason (probably the debug level) the message is not being printed
-        captured = capsys.readouterr()
+        captured = self.get_stdout_stderr()
         debug.trace_object(5, captured)
         ## TODO: assert "test exit method" in captured.err
-        debug.assertion("test exit method" in captured.err)
+        debug.assertion("test exit method" in captured[1])
 
-    def test_dummy_main(self, capsys):
+    def test_dummy_main(self):
         """Ensure dummy_main works as expected"""
         debug.trace(4, "test_dummy_main()")
         THE_MODULE.dummy_main()
-        captured = capsys.readouterr()
-        assert 'Environment options' in captured.out
+        captured = self.get_stdout()
+        assert 'Environment options' in captured
 
-    @pytest.mark.xfail                   # TODO: remove xfail
+    # @pytest.mark.xfail                   # TODO: remove xfail
     @trap_exception
-    def test_getenv(self, monkeypatch):
+    def test_getenv(self):
         """Ensure getenv works as expected"""
         debug.trace(4, "test_getenv()")
-        monkeypatch.setenv('TEST_ENV_VAR', 'some value', prepend=False)
+        self.monkeypatch.setenv('TEST_ENV_VAR', 'some value', prepend=False)
         assert THE_MODULE.getenv('TEST_ENV_VAR') == 'some value'
 
-    def test_getenv_value(self, monkeypatch):
+    def test_getenv_value(self):
         """Ensure getenv_value works as expected"""
         debug.trace(4, "test_getenv_value()")
-        monkeypatch.setenv('NEW_ENV_VAR', 'some value', prepend=False)
+        self.monkeypatch.setenv('NEW_ENV_VAR', 'some value', prepend=False)
         assert THE_MODULE.getenv_value('NEW_ENV_VAR', default='empty', description='another test env var') == 'some value'
         assert THE_MODULE.env_defaults['NEW_ENV_VAR'] == 'empty'
         assert THE_MODULE.env_options['NEW_ENV_VAR'] == 'another test env var'
 
-    def test_getenv_text(self, monkeypatch):
+    def test_getenv_text(self):
         """Ensure getenv_text works as expected"""
         debug.trace(4, "test_getenv_text()")
-        monkeypatch.setenv('TEST_ENV_VAR', 'some value', prepend=False)
+        self.monkeypatch.setenv('TEST_ENV_VAR', 'some value', prepend=False)
         assert THE_MODULE.getenv_text('TEST_ENV_VAR') == 'some value'
         assert THE_MODULE.getenv_text("REALLY FUBAR?", False) == 'False'
 
-    def test_getenv_number(self, monkeypatch):
+    def test_getenv_number(self):
         """Ensure getenv_number works as expected"""
         debug.trace(4, "test_getenv_number()")
-        monkeypatch.setenv('TEST_NUMBER', '9.81', prepend=False)
+        self.monkeypatch.setenv('TEST_NUMBER', '9.81', prepend=False)
         assert THE_MODULE.getenv_number('TEST_NUMBER', default=20) == 9.81
         assert THE_MODULE.getenv_number("REALLY FUBAR", 123) == 123.0
 
-    def test_getenv_int(self, monkeypatch):
+    def test_getenv_int(self):
         """Ensure getenv_int works as expected"""
         debug.trace(4, "test_getenv_int()")
-        monkeypatch.setenv('TEST_NUMBER', '34', prepend=False)
+        self.monkeypatch.setenv('TEST_NUMBER', '34', prepend=False)
         assert THE_MODULE.getenv_int('TEST_NUMBER', default=20) == 34
         assert THE_MODULE.getenv_int("REALLY FUBAR", 123) == 123
 
-    def test_getenv_bool(self, monkeypatch):
+    def test_getenv_bool(self):
         """Ensure getenv_bool works as expected"""
         debug.trace(4, "test_getenv_bool()")
-        monkeypatch.setenv('TEST_BOOL', 'FALSE', prepend=False)
+        self.monkeypatch.setenv('TEST_BOOL', 'FALSE', prepend=False)
         assert not THE_MODULE.getenv_bool('TEST_BOOL', None)
-        monkeypatch.setenv('TEST_BOOL', '  true   ', prepend=False)
+        self.monkeypatch.setenv('TEST_BOOL', '  true   ', prepend=False)
         assert THE_MODULE.getenv_bool('TEST_BOOL', None)
         assert not isinstance(THE_MODULE.getenv_boolean("REALLY FUBAR?", None), bool)
         assert isinstance(THE_MODULE.getenv_boolean("REALLY FUBAR?", False), bool)
 
 
 def set_test_env_var():
     """Set enviroment vars to run tests"""
```

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_train_language_model.py` & `mezcla-1.3.9.9/mezcla/tests/test_train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_train_text_categorizer.py` & `mezcla-1.3.9.9/mezcla/tests/test_train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_transpose_data.py` & `mezcla-1.3.9.9/mezcla/tests/test_transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/test_xml_utils.py` & `mezcla-1.3.9.9/mezcla/tests/test_xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/tfidf/test_corpus.py` & `mezcla-1.3.9.9/mezcla/tests/tfidf/test_corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/tfidf/test_dockeyword.py` & `mezcla-1.3.9.9/mezcla/tests/tfidf/test_dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/tfidf/test_document.py` & `mezcla-1.3.9.9/mezcla/tests/tfidf/test_document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tests/tfidf/test_preprocess.py` & `mezcla-1.3.9.9/mezcla/tests/tfidf/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/text_categorizer.py` & `mezcla-1.3.9.9/mezcla/text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/text_processing.py` & `mezcla-1.3.9.9/mezcla/text_processing.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,27 +170,32 @@
         # Note: uses a "positive lookbehind assertion" (i.e., (?<=...) to retain punctuation 
         sentences = re.split(r"(?<=[\.\!\?])\s\s+", text.strip())
     else:
         sentences = nltk.tokenize.sent_tokenize(text)
     return sentences
 
 
-def split_word_tokens(text, omit_punct=False):
-    """Splits TEXT into word tokens (i.e., words, punctuation, etc.) Note: run split_sentences first (e.g., to allow for proper handling of periods).
+def split_word_tokens(text, omit_punct=False, omit_stop=None):
+    """Splits TEXT into word tokens (i.e., words, punctuation, etc.), optionally with OMIT_PUNCT and OMIT_STOP.
+    Note: run split_sentences first (e.g., to allow for proper handling of periods).
     By default, this uses NLTK's PunktSentenceTokenizer."""
     # EX: split_word_tokens("How now, brown cow?") => ['How', 'now', ',', 'brown', 'cow', '?']
     debug.trace(7, "split_word_tokens(%s); type=%s" % (text, type(text)))
     if SKIP_NLTK:
         tokens = [t.strip() for t in re.split(r"(\W+)", text) if (len(t.strip()) > 0)]
     else:
         tokens = nltk.word_tokenize(text)
     if omit_punct:
         tokens = [t for t in tokens if not is_punct(t)]
+    if omit_stop:
+        tokens = [t for t in tokens if not is_stopword(t)]
     debug.trace(7, "tokens: %s" % [(t, type(t)) for t in tokens])
     return tokens
+#
+# split_word_tokens("How now, brown cow?", omit_punct=True, omit_stop=True) => ['now', 'brown', 'cow']
 
 
 def label_for_tag(POS, word=None):
     """Returns part-of-speech label for POS, optionally overriden based on WORD (e.g., original token if punctuation)"""
     label = POS
     if KEEP_PUNCT and word and re.match(r"\W", word[0]):
         label = word
```

### Comparing `mezcla-1.3.9.8/mezcla/text_utils.py` & `mezcla-1.3.9.9/mezcla/text_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,25 +140,25 @@
     Notes:
     - comparisons should be made against using functional constant, not number:
       EX: version_to_number("1.1.1") > version_to_number("1.1")
       EX: version_to_number("1.1.1") < 1.1
     - strings in the version are ignored
     - 0 is returned if version string is non-standard"""
     # EX: version_to_number("1.11.1") => 1.00110001
-    # EX: version_to_number("1") => 1
+    # EX: version_to_number("1") => 1.0
     # EX: version_to_number("") => 0
     # TODO: support string (e.g., 1.11.2a).
     version_number = 0
     version_text = version
     new_version_text = ""
     max_component_length = (1 + max_padding)
     debug.trace_fmt(5, "version_to_number({v})", v=version)
 
     # HACK: Remove newlines
-    # EX: "3.7.6 (default, Jan  8 2020, 19:59:22)<NL>[GCC 7.3.0]"
+    # example: "3.7.6 (default, Jan  8 2020, 19:59:22)<NL>[GCC 7.3.0]"
     if my_re.search(r"^([^\n]+)\n", version_text):
         debug.trace_fmt(5, "Removing pesky newline: '{vt}' => '{nvt}'", vt=version_text, nvt=my_re.group(1))
         version_text = my_re.group(1)
 
     # Remove all non-numeric components, after initial number-like value
     # ex: "3.7.6 (default, Jan  8 2020, 19:59:22" => "3.7.6"
     ## DEBUG: debug.trace_fmt(6, "stripped sys.version: {v}", v=re.sub(r"[^0-9\.]", "", sys.version))
@@ -218,15 +218,17 @@
     ## OLD: Note: the string values currently cannot be quoted (i.e., no embedded spaces)."""
     # EX: extract_string_list("1, 2,3 4") => ['1', '2', '3', '4']
     # EX: extract_string_list(" ") => []
     # EX: extract_string_list(",,") => []
     # EX: extract_string_list("'my dog'  likes  'my  hot  dog'") => ['my dog', 'likes', 'my  hot  dog']
 
     # Convert commas and whitespace to be blanks
+    # Also removes surrounding list brackets
     normalized_text = text.replace(",", " ").strip()
+    normalized_text = my_re.sub(r"^\[(.*)\]$", r"\1", normalized_text)
     normalized_text = re.sub(r"\s", " ", normalized_text)
     debug.trace_fmtd(6, "normalized_text1: {nt}", nt=normalized_text)
 
     # Change spaces within embedded quotes to be new-page (i.e., ^L)
     max_tries = 1 + text.count(" ")
     num_tries = 0
     quoted_space_regex = r"(['\"])([^ '\"]+) ([^'\"]+)\1"
@@ -261,15 +263,15 @@
 
 def extract_int_list(text, default_value=0):
     """Extract list of integral values from comma and/or whitespace delimited TEXT using DEFAULT_VALUE for non-integers (even if floating point)"""
     return [to_int(v, default_value) for v in extract_string_list(text)]
 
 
 def getenv_ints(var, default_values_spec):
-    """Get integer list using values specified for environment VAR (or DEFAULT_VALUES_SPEC)"""
+    """Get integer list using values specified for environment VAR (or DEFAULT_VALUES_SPEC text)"""
     # EX: getenv_ints("DUMMY VARIABLE", str(list(range(5)))) => [0, 1, 2, 3, 4]
     return extract_int_list(system.getenv_text(var, default_values_spec))
 
 
 def is_symbolic(token):
     """Indicates whether (string) token is symbolic (e.g., non-numeric like "ABC").
     Note: for convenience, tokens can be numeric types (e.g., 17), with False returned."""
```

### Comparing `mezcla-1.3.9.8/mezcla/tfidf/config.py` & `mezcla-1.3.9.9/mezcla/tfidf/config.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tfidf/corpus.py` & `mezcla-1.3.9.9/mezcla/tfidf/corpus.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tfidf/dockeyword.py` & `mezcla-1.3.9.9/mezcla/tfidf/dockeyword.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tfidf/document.py` & `mezcla-1.3.9.9/mezcla/tfidf/document.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tfidf/preprocess.py` & `mezcla-1.3.9.9/mezcla/tfidf/preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import nltk
 from nltk.stem import SnowballStemmer
 from sklearn.feature_extraction.text import CountVectorizer
 from stop_words import get_stop_words
 
 # Local modules
 from mezcla import debug
-from mezcla.my_regex import my_re
+from mezcla.my_regex import my_re, REGEX_TRACE_LEVEL
 from mezcla import system
 from mezcla.tfidf.config import BASE_DEBUG_LEVEL as BDL
 from mezcla.tfidf.dockeyword import DocKeyword
 
 unescape = html.unescape
 
 
@@ -73,20 +73,29 @@
     description="Language for text preprocessing")
 
 if SPLIT_WORDS:
     debug.trace(2, "FYI: Splitting by word token (not whitespace)\n")
     debug.assertion(not TFIDF_ALLOW_PUNCT)
 WORD_REGEX = r'\w+' if SPLIT_WORDS else r'\S+'
 
+
 def handle_unicode(text):
     """Needed for the description fields."""
+    # EX: handle_unicode("Predactica\u2122") => "Predactica \u2122"
     if re.search(r'\\+((u([0-9]|[a-z]|[A-Z]){4}))', text):
         text = text.encode('utf-8', 'ignore').decode('unicode-escape', 'ignore')
     text = re.sub(r'\\n', '\n', text)
     text = re.sub(r'\\t', '\t', text)
+    # Put space around non-ascii unicode characters
+    # note: excludes special punctuation like U+00A9 (©)
+    EXT_ASC_CH = "\u0000-\u007F\u00C0-\u0100"
+    if re.search(fr'[^{EXT_ASC_CH}]', text):
+        text = re.sub(fr'([{EXT_ASC_CH}]) ([^{EXT_ASC_CH}]) ([{EXT_ASC_CH}])',
+                      r'\1 \2 \3', f" {text} ", flags=re.VERBOSE)
+        text = text.strip(" ")
     return text
 
 
 def handle_html_unquote(text):
     """Detect if there are HTML encoded characters, then decode them."""
     if re.search(r'(&#?x?)([A-Z]|[a-z]|[0-9]){2,10};', text):
         text = unescape(text)
@@ -109,15 +118,16 @@
     will both convert to
         "She loved icecream; mint chip especially".
 
     However,
         "The 27-year-old could eat icecream any day"
     will not be changed.
     """
-    return re.sub(r'\s+-\s*|\s*-\s+', ';', text)
+    # EX: handle_text_break_dash("a - b") => "a; b"
+    return re.sub(r'\s+-\s*|\s*-\s+', '; ', text)
 
 
 def clean_text(raw_text):
     """Strip text of non useful characters.
     Note: This is no-op if SKIP_WORD_CLEANING (global).
     """
     # TODO: rework so SKIP_WORD_CLEANING applied elsewhere
@@ -130,14 +140,15 @@
         text = handle_unicode(text)
         text = handle_html_unquote(text)
         text = handle_mac_quotes(text)
         text = handle_text_break_dash(text)
         if not TFIDF_PRESERVE_CASE:
             text = text.lower()
 
+        ## TODO3: make &-stripping optional
         regex_subs = ['\t', '\n', '\r', r'\s+', '&']
         for regex_sub in regex_subs:
             text = re.sub(regex_sub, ' ', text)
     debug.trace(BDL + 2, f"clean_text({raw_text!r}) => {text!r}")
     return text
 
 
@@ -334,14 +345,20 @@
         ## TODO: yield_method = self.slow_yield_keywords if not USE_SKLEARN_COUNTER else self.yield_sklearn_keywords
         if USE_SKLEARN_COUNTER:
             result = self.quick_yield_keywords(raw_text, document=document)
         else:
             result = self.full_yield_keywords(raw_text, document=document)
         return result
 
+    def re_search(self, regex, text):
+        """Invoke my_re.search with higher tracing"""
+        debug.reference_var(self)
+        TRACE_LEVEL = (REGEX_TRACE_LEVEL + 1)
+        return my_re.search(regex, text, base_trace_level=TRACE_LEVEL)
+    
     def full_yield_keywords(self, raw_text, document=None):
         """Full-featured version of keyword generation, including support for offsets"""
         if sys.version_info[0] < 3:  # python2 support
             if isinstance(raw_text, str):
                 raw_text = raw_text.decode('utf-8', 'ignore')
         ## TPO: HACK: support min ngram size
         gramlist = None
@@ -381,21 +398,21 @@
                     data = words_no_stopwords[offset:]
                     text_in_chunks = [data[pos:pos + gramsize]
                                       for pos in range(0, len(data), gramsize)
                                       if len(data[pos:pos + gramsize]) == gramsize]
                     for word_list in text_in_chunks:
                         word_text = ' '.join([self.stem_term(w.text) for w in word_list])
                         ## OLD: if (SPLIT_WORDS or (not re.search(BAD_WORD_PUNCT_REGEX, word_text))):
-                        exclude = my_re.search(BAD_WORD_PUNCT_REGEX, word_text)
+                        exclude = self.re_search(BAD_WORD_PUNCT_REGEX, word_text)
                         if TFIDF_ALLOW_PUNCT and exclude:
                             # Include unless punctuation starts or ends the text or is after a space
                             # TODO2: add BAD_NGRAM_PUNCT_REGEX (e.g., "[;!?]")
-                            exclude = (my_re.search("^" + BAD_WORD_PUNCT_REGEX, word_text) or
-                                       my_re.search(BAD_WORD_PUNCT_REGEX + "$", word_text) or
-                                       my_re.search(" " + BAD_WORD_PUNCT_REGEX, word_text))
+                            exclude = (self.re_search("^" + BAD_WORD_PUNCT_REGEX, word_text) or
+                                       self.re_search(BAD_WORD_PUNCT_REGEX + "$", word_text) or
+                                       self.re_search(" " + BAD_WORD_PUNCT_REGEX, word_text))
                         if not exclude:
                             word_global_start = sentence.start + word_list[0].start
                             word_global_end = sentence.start + word_list[-1].end
                             yield DocKeyword(word_text, document=document, start=word_global_start, end=word_global_end)
                         else:
                             debug.trace(BDL + 3, f"Ignoring {gramsize}-gram {word_text!r}")
         return
```

### Comparing `mezcla-1.3.9.8/mezcla/tfidf/tests/misc_test.py` & `mezcla-1.3.9.9/mezcla/tfidf/tests/misc_test.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/tpo_common.py` & `mezcla-1.3.9.9/mezcla/tpo_common.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/train_language_model.py` & `mezcla-1.3.9.9/mezcla/train_language_model.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/train_text_categorizer.py` & `mezcla-1.3.9.9/mezcla/train_text_categorizer.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/transpose_data.py` & `mezcla-1.3.9.9/mezcla/transpose_data.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/mezcla/unittest_wrapper.py` & `mezcla-1.3.9.9/mezcla/unittest_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 # - Creates per-test temp file, based on same class-wide temp-base file.
 # - To treat temp-base as a subdirectory, set use_temp_base_dir to True in 
 #   class member initialiation section.
 # - Changes to temporary directory/file should be synchronized with ../main.py.
 # - Overriding the temporary directory can be handy during debugging; however,
 #   you might need to specify different ones if you invoke helper scripts. See
 #   tests/test_extract_company_info.py for an example.
+# - It can be confusing debugging tests that use run_script, because the trace level
+#   is raised by default. To disable this, set the SUB_DEBUG_LEVEL as follows:
+#      l=5; DEBUG_LEVEL=$l SUB_DEBUG_LEVEL=$l pytest -s tests/test_spell.py
+#   See glue_helper.py for implementation along with related ALLOW_SUBCOMMAND_TRACING.
 # TODO:
 # - * Clarify TEMP_BASE vs. TEMP_FILE usage.
 # - Clarify that this can co-exist with pytest-based tests (see tests/test_main.py).
 # TODO2:
 # - Clean up script_file usage (and unncessary settings in test scripts).
 #
 #-------------------------------------------------------------------------------
@@ -35,32 +39,34 @@
 #           self.assertTrue("really" in output)
 #
 #   if __name__ == '__main__':
 #      unittest.main()
 #-------------------------------------------------------------------------------
 # TODO:
 # - Add method to invoke unittest.main(), so clients don't need to import unittest.
-# - Clarify how ALLOW_SUBCOMMAND_TRACING affects tests that invoke external scripts.
 #
 
 """Unit test support class"""
 
 # Standard packages
 import inspect
 import os
+import sys
 import tempfile
 import unittest
 
 # Installed packages
 import pytest
 
 # Local packages
 import mezcla
 from mezcla import debug
 from mezcla import glue_helpers as gh
+from mezcla.main import DISABLE_RECURSIVE_DELETE
+from mezcla.misc_utils import string_diff
 from mezcla.my_regex import my_re
 from mezcla import system
 
 # Constants (e.g., environment options)
 
 TL = debug.TL
 KEEP_TEMP = system.getenv_bool("KEEP_TEMP", debug.detailed_debugging(),
@@ -76,14 +82,22 @@
 THIS_PACKAGE = getattr(mezcla.debug, "__package__", None)
 debug.assertion(THIS_PACKAGE == "mezcla")
 
 # Environment options
 VIA_UNITTEST = system.getenv_bool(
     "VIA_UNITTEST", False,
     description="Run tests via unittest instead of pytest")
+PROFILE_CODE = system.getenv_boolean(
+    "PROFILE_CODE", False,
+    description="Profile each test invocation")
+
+# Dynamic imports
+if PROFILE_CODE:
+    import cProfile
+    import pstats
 
 #-------------------------------------------------------------------------------
 
 def get_temp_dir(keep=None):
     """Get temporary directory, omitting later deletion if KEEP"""
     # NOTE: Unused function
     if keep is None:
@@ -161,16 +175,19 @@
                                    tempfile.NamedTemporaryFile().name)
     check_coverage = system.getenv_bool("CHECK_COVERAGE", False,
                                         "Check coverage during unit testing")
     ## TODO: temp_file = None
     ## TEMP: initialize to unique value independent of temp_base
     temp_file = None
     use_temp_base_dir = system.is_directory(temp_base)
-    test_num = 1
+    ## OLD: test_num = 1
+    test_num = 0
+    temp_file_count = 0
     class_setup = False
+    profiler = None
     
     ## TEST:
     ## NOTE: leads to pytest warning. See
     ##   https://stackoverflow.com/questions/62460557/cannot-collect-test-class-testmain-because-it-has-a-init-constructor-from
     ## def __init__(self, *args, **kwargs):
     ##     debug.trace_fmtd(6, "TestWrapper.__init__({a}): keywords={kw}; self={s}",
     ##                      a=",".join(args), kw=kwargs, s=self)
@@ -180,15 +197,15 @@
     ## __test__ = False                 # make sure not assumed test
         
     @classmethod
     def setUpClass(cls, filename=None, module=None):
         """Per-class initialization: make sure script_module set properly
         Note: Optional FILENAME is path for testing script and MODULE the imported object for tested script
         """
-        debug.trace(6, f"TestWrapper.setupClass({cls}, fn={filename}, mod={module})")
+        debug.trace(6, f"TestWrapper.setUpClass({cls}, fn={filename}, mod={module})")
         super().setUpClass()
         cls.class_setup = True
         debug.trace_object(7, cls, "TestWrapper class")
         debug.assertion(cls.script_module != TODO_MODULE)
         if (cls.script_module is not None):
             # Try to pull up usage via python -m mezcla.xyz --help
             help_usage = gh.run("python -m '{mod}' --help", mod=cls.script_module)
@@ -214,14 +231,18 @@
         if cls.check_coverage:
             # note: For proper invocation info, see https://coverage.readthedocs.io/en/latest
             test_module = "pytest ..." if not VIA_UNITTEST else "unittest discover"
             debug.trace(4, "FYI: coverage check only covers run_script usages; "
                         "invoke externally for more general support:\n"
                         f"    python -m coverage run -m {test_module}")
 
+        # Enable code profiling if desired
+        if PROFILE_CODE:
+            cls.profiler = cProfile.Profile()
+            
         # Optionally, setup up script_file and script_module
         if filename:
             cls.set_module_info(filename, module_object=module)
 
         return
 
     @staticmethod
@@ -269,93 +290,101 @@
         debug.assertion(result.endswith(".py"))
         debug.trace(7, f'get_module_file_path({test_filename}) => {result}')
         return result
 
     @classmethod
     def set_module_info(cls, test_filename, module_object=None):
         """Sets both script_module and script_path
-        Note: normally invoked in setupClass method
+        Note: normally invoked in setUpClass method
         Usage: cls.set_module_info(__file__, THE_MODULE)
         """
         debug.trace(7, f'set_module_info({test_filename}, {module_object})')
         cls.script_module = cls.get_testing_module_name(test_filename, module_object)
         cls.script_file = cls.get_module_file_path(test_filename)
         return 
     
     def setUp(self):
         """Per-test initializations
         Notes:
         - Disables tracing scripts invoked via run() unless ALLOW_SUBCOMMAND_TRACING
         - Initializes temp file name (With override from environment)."""
         # Note: By default, each test gets its own temp file.
-        debug.trace(6, "TestWrapper.setUp()")
+        debug.trace(5, "TestWrapper.setUp()")
         if not self.class_setup:
-            debug.trace(5, "Warning: invoking setupClass in setup")
-            TestWrapper.setupClass(self.__class__)
+            debug.trace(4, "Warning: invoking setUpClass in setUp")
+            TestWrapper.setUpClass(self.__class__)
         if not gh.ALLOW_SUBCOMMAND_TRACING:
             gh.disable_subcommand_tracing()
         # The temp file is an extension of temp-base file by default.
         # Optionally, if can be a file in temp-base subdrectory.
         if self.use_temp_base_dir:
             default_temp_file = gh.form_path(self.temp_base, "test-")
         else:
             default_temp_file = self.temp_base + "-test-"
-        default_temp_file += str(TestWrapper.test_num)
-        self.temp_file = system.getenv_text("TEMP_FILE", default_temp_file)
-        gh.delete_existing_file(self.temp_file)
         TestWrapper.test_num += 1
+        default_temp_file += str(TestWrapper.test_num)
 
+        # Get new temp file and delete existing file and variants based on temp_file_count,
+        # such as /tmp/test-2, /tmp/test-2-1, and /tmp/test-2-2 (but not /tmp/test-[13]*).
+        self.temp_file = system.getenv_text("TEMP_FILE", default_temp_file)
+        gh.delete_existing_file(f"{self.temp_file}")
+        for f in gh.get_matching_files(f"{self.temp_file}-[0-9]*"):
+            gh.delete_existing_file(f)
+
+        # Start the profiler
+        if PROFILE_CODE:
+            self.profiler.enable()
+        
         debug.trace_object(6, self, "TestWrapper instance")
         return
 
     def run_script(self, options=None, data_file=None, log_file=None, trace_level=4,
-                   out_file=None, env_options=None, uses_stdin=None, post_options=None, background=None):
+                   out_file=None, env_options=None, uses_stdin=None, post_options=None, background=None, skip_stdin=None):
         """Runs the script over the DATA_FILE (optional), passing (positional)
         OPTIONS and optional setting ENV_OPTIONS. If OUT_FILE and LOG_FILE are
         not specified, they  are derived from self.temp_file. The optional POST_OPTIONS
         go after the data file.
         Notes:
         - OPTIONS uses quotes around shell special characters used (e.g., '<', '>', '|')
         - issues warning if script invocation leads to error
-        - if USES_STDIN, requires explicit empty string for DATA_FILE to avoid use of - (n.b., as a precaution against hangups)"""
+        - if USES_STDIN, requires explicit empty string for DATA_FILE to avoid use of - (n.b., as a precaution against hangups)
+        - if SKIP_STDIN, then - omitted from command line"""
         debug.trace_fmtd(trace_level + 1,
                          "TestWrapper.run_script(opts={opts!r}, data={df}, log={lf}, lvl={lvl}, out={of}, env={env}, stdin={stdin}, post={post}, back={back})",
                          opts=options, df=data_file, lf=log_file, lvl=trace_level, of=out_file,
                          env=env_options, stdin=uses_stdin, post=post_options, back=background)
         if options is None:
             options = ""
         if env_options is None:
             env_options = ""
         if post_options is None:
             post_options = ""
+        if skip_stdin is None:
+            skip_stdin = False
 
         # Derive the full paths for data file and log, and then invoke script.
         # TODO: derive from temp base and data file name?;
         # TODO1: derive default for uses_stdin based on use of filename argment (e.g., from usage)
         uses_stdin_false = ((uses_stdin is not None) and not bool(uses_stdin))
-        data_path = ("" if uses_stdin_false else "-")
+        data_path = ("" if (skip_stdin or uses_stdin_false) else "-")
         if data_file is not None:
             data_path = (gh.resolve_path(data_file) if len(data_file) else data_file)
         if not log_file:
             log_file = self.temp_file + ".log"
         if not out_file:
             out_file = self.temp_file + ".out"
         # note: output is redirected to a file to preserve tabs
 
         # Set converage script path and command spec
         coverage_spec = ''
         script_module = self.script_module
         if self.check_coverage:
             debug.assertion(self.script_file)
-            ## BAD: self.script_module = self.script_file
             script_module = self.script_file
             coverage_spec = 'coverage run'
-        ## OLD:
-        ## else:
-        ##     debug.assertion(not self.script_module.endswith(".py"))
         debug.assertion(not script_module.endswith(".py"))
         amp_spec = "&" if background else ""
 
         # Run the command
         ## TODO3: allow for stdin_command (e.g., "echo hey" | ...)
         ## TODO2: add sanity check for special shell characters
         ##   shell_tokens = ['<', '>', '|']
@@ -364,67 +393,76 @@
                  env=env_options, cov_spec=coverage_spec, module=script_module,
                  opts=options, path=data_path, out=out_file, log=log_file, post=post_options, amp_spec=amp_spec)
         output = system.read_file(out_file)
         # note: trailing newline removed as with shell output
         if output.endswith("\n"):
             output = output[:-1]
         debug.trace_fmtd(trace_level, "output: {{\n{out}\n}}",
-                         out=gh.indent_lines(output), max_len=2048)
+                         out=gh.indent_lines(output), max_len=4096)
 
         # Make sure no python or bash errors. For example,
         #   "SyntaxError: invalid syntax" and "bash: python: command not found"
         log_contents = system.read_file(log_file)
         error_found = my_re.search(r"(\S+error:)|(no module)|(command not found)",
                                    log_contents.lower())
         debug.assertion(not error_found)
-        debug.trace_expr(trace_level + 1, log_contents, max_len=2048)
+        debug.trace_expr(trace_level + 1, log_contents, max_len=4096)
 
         # Do sanity check for python exceptions
         traceback_found = my_re.search("Traceback.*most recent call", log_contents)
         debug.assertion(not traceback_found)
 
         return output
 
+    def resolve_assertion(self, function_label, message):
+        """Returns statement text, filename, line number, and qualifier for FUNCTION_LABEL assertion failure"""
+        statement = filename = line_num = expr = qual = None
+        try:
+            # note: accounts for trap_exception and other decorators
+            for caller in inspect.stack():
+                debug.trace_expr(8, caller)
+                ## DEBUG: print(f"{caller=}")
+                (_frame, filename, line_num, _function, context, _index) = caller
+                statement = debug.read_line(filename, line_num).strip()
+                ## DEBUG: print(f"{statement=}")
+                if f".{function_label}(" in statement:
+                    break
+            # TODO3: use abstract syntax tree (AST) based extraction
+            # ex: self.do_assert(not my_re.search(r"cat|dog", description))  # no pets
+            # Isolate condition
+            cond = my_re.sub(fr"^\s*\S+\.{function_label}\((.*)\)", r"\1", statement)
+            # Get expression proper, removing optional comments and semicolon 
+            expr = my_re.sub(r";?\s*#.*$", "", cond)
+            # Strip optional message
+            qual = ""
+            if message is not None:
+                expr = my_re.sub(r", *([\'\"]).*\1\s*$", "", expr)   # string arg
+                expr = my_re.sub(r", *[a-z0-9_]+$", "", expr,        # variable arg
+                                 flags=my_re.IGNORECASE)
+                qual = f": {message}"
+            debug.trace_expr(7, filename, line_num, context, prefix="resolve_assertion: ")
+        except:
+            system.print_exception_info("resolve_assertion")
+        debug.assertion(statement)
+        result = (statement, filename, line_num, expr, qual)
+        debug.trace(7, f"resolve_assertion({function_label}) => {result}")
+        return result
+    
     def do_assert(self, condition, message=None):
         """Shows context for assertion failure with CONDITION and then issue assert
         If MESSAGE specified, included in assertion error
         Note:
         - Works around for maldito pytest, which makes it hard to do simple things like pinpointing errors.
         - Formatted similar to debug.assertion:
              Test assertion failed: <expr> (at <f><n>): <msg>
         """
         debug.trace(7, f"do_assert({condition}, msg={message})")
         if ((not condition) and debug.debugging(debug.TL.DEFAULT)):
-            statement = filename = line_num = None
-            try:
-                # note: accounts for trap_exception and other decorators
-                for caller in inspect.stack():
-                    debug.trace_expr(8, caller)
-                    (_frame, filename, line_num, _function, context, _index) = caller
-                    statement = debug.read_line(filename, line_num).strip()
-                    if "do_assert" in statement:
-                        break
-                debug.trace_expr(7, filename, line_num, context, prefix="do_assert: ")
-            except:
-                system.print_exception_info("do_assert")
-            debug.assertion(statement)
+            (statement, filename, line_num, expr, qual) = self.resolve_assertion("do_assert", message)
             if statement:
-                # TODO3: use abstract syntax tree (AST) based extraction
-                # ex: self.do_assert(not my_re.search(r"cat|dog", description))  # no pets
-                # Isolate condition
-                cond = my_re.sub(r"^\s*\S+\.do_assert\((.*)\)", r"\1", statement)
-                # Get expression proper, removing optional comments and semicolon 
-                expr = my_re.sub(r";?\s*#.*$", "", cond)
-                # Strip optional message
-                qual = ""
-                if message is not None:
-                    expr = my_re.sub(r", *([\'\"]).*\1\s*$", "", expr)   # string arg
-                    expr = my_re.sub(r", *[a-z0-9_]+$", "", expr,        # variable arg
-                                     flags=my_re.IGNORECASE)
-                    qual = f": {message}"
                 # Format assertion error with optional qualification (i.e., user message)
                 debug.trace(1, f"Test assertion failed: {expr} (at {filename}:{line_num}){qual}")
                 debug.trace(5, f"\t{statement}")
             else:
                 system.print_error("Warning: unexpected condition in do_assert")
         assert condition, message
     #
@@ -432,65 +470,125 @@
     ## assert = do_assert
     ##
     ## TEST:
     ## def assert(self, *args, **kwargs):
     ##     """Wrapper around do_assert (q.v.)"""
     ##     self.do_assert(*args, **kwargs)
 
+    def do_assert_equals(self, value1, value2, message=None):
+        """Make sure VALUE1 equals VALUE2, using optional MESSAGE"""
+        equals = value1 == value2
+        if ((not equals) and debug.debugging(debug.TL.DEFAULT)):
+            (statement, filename, line_num, expr, qual) = self.resolve_assertion("do_assert_equals", message)
+            if statement:
+                # Format assertion error with optional qualification (i.e., user message)
+                debug.trace(1, f"Test equality assertion failed: {expr} (at {filename}:{line_num}){qual}")
+                debug.trace(5, f"\t{statement}")
+                debug.trace(2, "diff:\n" + string_diff(value1, value2))
+            else:
+                system.print_error("Warning: unexpected condition in do_assert_equals")
+        assert equals, message
+    
     @pytest.fixture(autouse=True)
     def monkeypatch(self, monkeypatch):
         """Support for using pytest monkeypatch to modify objects (e.g., dictionaries or environment variables)"""
         # See https://docs.pytest.org/en/latest/how-to/monkeypatch.html
         self.monkeypatch = monkeypatch
 
     @pytest.fixture(autouse=True)
     def capsys(self, capsys):
         """Support for capturing stdout and stderr"""
         # See https://docs.pytest.org/en/latest/how-to/capture-stdout-stderr.html
         self.capsys = capsys
 
-    ## DUPLICATE
-    ## @pytest.fixture(autouse=True)
-    ## def monkeypatch(self, monkeypatch):
-    ##     """Support for modifying objects, dictionaries or environment variables"""
-    ##    self.monkeypatch = monkeypatch
-
     def get_stdout_stderr(self):
         """Get currently captured standard output and error
-        Note: Clears both stdout and stderr captured
+        Note: Clears both stdout and stderr captured afterwards. This might
+        be needed beforehand to clear capsys buffer.
         """
         stdout, stderr = self.capsys.readouterr()
-        debug.trace_expr(5, stdout, stderr, prefix="get_stdout_stderr:\n", delim="\n")
+        ## TODO4: resolve issue with resolve_assertion call-stack tracing being clippped
+        debug.trace_expr(5, stdout, stderr, prefix="get_stdout_stderr:\n", delim="\n", maxlen=8192)
         return stdout, stderr
         
     def get_stdout(self):
-        """Get currently captured standard output (see get_stdout_stderr)"""
+        """Get currently captured standard output (see get_stdout_stderr)
+        Warning: You might need to invoke beforehand to clear buffer.
+        """
         stdout, _stderr = self.get_stdout_stderr()
         return stdout
         
     def get_stderr(self):
-        """Get currently captured standard error (see get_stdout_stderr)"""
+        """Get currently captured standard error (see get_stdout_stderr)
+        Warning: You might need to invoke beforehand to clear buffer.
+        """
         _stdout, stderr = self.get_stdout_stderr()
         return stderr
 
+    def clear_stdout_stderr(self):
+        """Clears stdout and stderr by issuing dummy call"""
+        _result = self.get_stdout_stderr()
+        return
+    #
+    clear_stdout = clear_stdout_stderr
+    clear_stderr = clear_stdout_stderr
+    
+    def get_temp_file(self, delete=None):
+        """return name of temporary file based on self.temp_file, optionally with DELETE"""
+        # Note: delete defaults to False if detailed debugging
+        # TODO: allow for overriding other options to NamedTemporaryFile
+        if delete is None and debug.detailed_debugging():
+            delete = False
+        temp_file_name = f"{self.temp_file}-{self.temp_file_count}"
+        self.temp_file_count += 1
+        debug.assertion(not delete, "Support for delete not implemented")
+        debug.format_value(f"get_temp_file() => {temp_file_name}", 5)
+        return temp_file_name
+
+    def create_temp_file(self, contents,  binary=False):
+        """Create temporary file with CONTENTS and return full path"""
+        temp_filename = self.get_temp_file()
+        system.write_file(temp_filename, contents, binary=binary)
+        debug.trace(6, f"create_temp_file({contents!r}) => {temp_filename}")
+        return temp_filename
+
     def tearDown(self):
         """Per-test cleanup: deletes temp file unless detailed debugging"""
         debug.trace(6, "TestWrapper.tearDown()")
         if not KEEP_TEMP:
             gh.run("rm -vf {file}*", file=self.temp_file)
+            for i in range(self.temp_file_count):
+                gh.run(f"rm -vf {self.temp_file}-{i}")
+        self.temp_file_count = 0
+
+        # Show results of code profiling if enabled
+        if PROFILE_CODE:
+            self.profiler.disable()
+            ## TODO: debug.trace(1, f"Test {self.test_num} code profiling results")
+            print(f"Test {self.test_num} code profiling results")
+            ## OLD: self.profiler.print_stats(sort='cumulative')
+            ## NOTE: Based on cProfile's print_stats (in order to use stderr)
+            stats = pstats.Stats(self.profiler, stream=sys.stderr)
+            stats.strip_dirs().sort_stats('cumulative').print_stats()
         return
 
     @classmethod
     def tearDownClass(cls):
         """Per-class cleanup: stub for tracing purposes"""
-        debug.trace_fmtd(6, "TestWrapper.tearDownClass(); cls={c}", c=cls)
+        debug.trace_fmtd(5, "TestWrapper.tearDownClass(); cls={c}", c=cls)
         if not KEEP_TEMP:
             ## TODO: use shutil
             if cls.use_temp_base_dir:
-                gh.run("rm -rvf {dir}", dir=cls.temp_base)
+                if DISABLE_RECURSIVE_DELETE:
+                    debug.trace(4, f"FYI: Only deleting top-level files in {cls.temp_base} to avoid potentially dangerous rm -r")
+                    gh.run("rm -f {dir}/* {dir}/.*", dir=cls.temp_base)
+                    gh.run("rm -f {dir}", dir=cls.temp_base)
+                else:
+                    debug.trace(4, f"FYI: Using potentially dangerous rm -r over {cls.temp_base}")
+                    gh.run("rm -rvf {dir}", dir=cls.temp_base)
             else:
                 gh.run("rm -vf {base}*", base=cls.temp_base)
         super().tearDownClass()
         return
 
 ## TODO: TestWrapper.assert = TestWrapper.do_assert
```

### Comparing `mezcla-1.3.9.8/mezcla/xml_utils.py` & `mezcla-1.3.9.9/mezcla/xml_utils.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/pyproject.toml` & `mezcla-1.3.9.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## TODO: eliminate redundancy
 
 [tool.poetry]
 name = "mezcla"
-version = "1.3.9.8"
+version = "1.3.9.9"
 description = "Miscellaneous Python scripts developed over the course of several independent consulting projects. [Mezcla is Spanish for mixture.]"
 authors = ["Tom O'Hara <tomasohara@gmail.com>"]
 license = "LGPLv3"
 ## TODO:
 ## packages = ['mezcla', 'mezcla.tfidf']
 
 [tool.poetry.dependencies]
```

### Comparing `mezcla-1.3.9.8/required-packages.txt` & `mezcla-1.3.9.9/required-packages.txt`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/requirements.txt` & `mezcla-1.3.9.9/requirements.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # By default only the cases used in multuiple scripts are installed.
 #
 # Note:
 # - Usage examples:
 #   1. Usual
 #      pip install -r requirements.txt
 #   2. Optional (i.e., including most optional):
-#      pip install --verbose $(perl -pe 's/^#opt#\s*//;' ~/Mezcla/requirements.txt | grep -v '^#')
+#      pip install --verbose $(perl -pe 's/^#opt#\s*//;  s/\s*#.*//;' ~/Mezcla/requirements.txt | grep -v '^#')
 #   3. Full (i.e., including all optional):
-#      pip install --verbose $(perl -pe 's/^#(opt|full)#\s*//;' ~/Mezcla/requirements.txt | grep -v '^#')
+#      pip install --verbose $(perl -pe 's/^#(opt|full)#\s*//;  s/\s*#.*//;' ~/Mezcla/requirements.txt | grep -v '^#')
 #      # TODO2: --ignore-errors [maldito pip]
-#      perl -pe 's/^#full#\s*//;' ~/Mezcla/requirements.txt | grep -v '^#' | xargs -I '{}' pip install '{}'
+#      perl -pe 's/^#(opt|full)#\s*//;  s/\s*#.*//;' ~/Mezcla/requirements.txt | grep -v '^#' | xargs -I '{}' pip install '{}'
 # - use `pip freeze` to get current list of package specifications (n.b., >= better than == unless specific version needed)
 # - installing textract from PyPI fails https://github.com/deanmalmgren/textract/issues/461
 #
 # Installation:
 # - python -m nltk.downloader punkt averaged_perceptron_tagger stopwords
 #
 # TODO:
@@ -109,14 +109,15 @@
 ## OLD
 ## spacy==3.2.6
 ## en_core_web_md@https://github.com/explosion/spacy-models/releases/download/en_core_web_md-3.2.0/en_core_web_md-3.2.0.tar.gz
 ## typing_extensions==4.7.0
 typing_extensions>=4.7.0
 #
 #opt# textract
+#opt# youtube_transcript_api
 #opt# vaderSentiment
 #...............................................................................
 # "Fully optional" requirements
 # Note: these generally involve large or long installations.
 #
 #full# bert==2.2.0
 #full# albert==1.3.1
```

### Comparing `mezcla-1.3.9.8/setup.py` & `mezcla-1.3.9.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from distutils.core import setup
 
 setup(name='Mezcla',
       packages=['mezcla', 'mezcla.tfidf'],
       module="mezcla",
       ## TODO2: import mezcla; version=mezcla.VERSION
-      version="1.3.9.8",
+      version="1.3.9.9",
       ## BAD: description-file="README.txt",
       description_file="README.txt",
       ## BAD: dist-name="Mezcla",
       dist_name="Mezcla",
       author="Tom O'Hara",
       # TODO3: find out which email key is preferred
       email="tomasohara@gmail.com",
```

### Comparing `mezcla-1.3.9.8/temp/simple_batspp.py` & `mezcla-1.3.9.9/temp/simple_batspp.py`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/tools/local-workflows.sh` & `mezcla-1.3.9.9/tools/local-workflows.sh`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/tox.ini` & `mezcla-1.3.9.9/tox.ini`

 * *Files identical despite different names*

### Comparing `mezcla-1.3.9.8/PKG-INFO` & `mezcla-1.3.9.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: mezcla
-Version: 1.3.9.8
+Version: 1.3.9.9
 Summary: Mezcla is Spanish for mixture, and this repository contains a variety of Python scripts.
 Home-page: https://github.com/tomasohara/mezcla
 License: LGPLv3
 Author: Tomás O'Hara
 Author-email: tomasohara@gmail.com
 Description-Content-Type: text/plain
 
 ﻿Note: This is an upgrade of the misc-utility repository with Python 2 support being phased out.
 
 Miscellaneous Python scripts developed over the course of several independent consulting projects. This also includes some code samples I adapted from publicly available source. (The code is not proprietary in nature. For example, it was not "borrowed" from proprietary source files, nor based on proprietary processes.)
 
 Spoiler alter: this is not "Pythonic python": I'm more into R&D than production programming. Nonetheless, there's a some useful scripts here, so I made the repository available. It is public in the spirit of open source software. 
- 
+
+This is a companion script to shell-scripts from Github:
+     https://github.com/tomasohara/shell-scripts
+
 This repository is licensed under the GNU Lesser General Public Version 3 (LGPLv3). See LICENSE.txt.
 
 Tom O'Hara
 May 2021
```

