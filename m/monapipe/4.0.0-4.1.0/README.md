# Comparing `tmp/monapipe-4.0.0.tar.gz` & `tmp/monapipe-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monapipe-4.0.0.tar", last modified: Wed Jan 17 10:56:25 2024, max compression
+gzip compressed data, was "monapipe-4.1.0.tar", last modified: Mon May 13 12:44:41 2024, max compression
```

## Comparing `monapipe-4.0.0.tar` & `monapipe-4.1.0.tar`

### file list

```diff
@@ -1,227 +1,234 @@
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.174272 monapipe-4.0.0/
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.843757 monapipe-4.0.0/LICENSES/
--rw-r--r--   0 florianbarth   (502) staff       (20)    18656 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/CC-BY 4.0.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)    20849 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/CC-BY-NC-SA 4.0.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)    22239 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/CC-BY-SA 3.0.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)    20137 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/CC-BY-SA 4.0.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)     7047 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/CC0-1.0.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)    18138 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/FDL-1.1.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)    35146 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/GPL-3.0.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)    42098 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)     1055 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/MIT.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)     1916 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/bsd-2-clause.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)      768 2023-11-30 17:01:54.000000 monapipe-4.0.0/LICENSES/open_multilingual_wordnet_license_statement.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)    47970 2024-01-17 10:56:25.173053 monapipe-4.0.0/PKG-INFO
--rw-r--r--   0 florianbarth   (502) staff       (20)     1528 2024-01-12 13:36:45.000000 monapipe-4.0.0/README.md
--rw-r--r--   0 florianbarth   (502) staff       (20)     1826 2024-01-17 10:55:46.000000 monapipe-4.0.0/pyproject.toml
--rw-r--r--   0 florianbarth   (502) staff       (20)       38 2024-01-17 10:56:25.174469 monapipe-4.0.0/setup.cfg
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.780056 monapipe-4.0.0/src/
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.872784 monapipe-4.0.0/src/monapipe/
--rw-r--r--   0 florianbarth   (502) staff       (20)      347 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2598 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/annotation.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      873 2024-01-12 13:36:36.000000 monapipe-4.0.0/src/monapipe/config.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.881861 monapipe-4.0.0/src/monapipe/lang/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/lang/__init__.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.897599 monapipe-4.0.0/src/monapipe/lang/de/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/lang/de/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      284 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/lang/de/auxiliary_verbs.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    13248 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/lang/de/inflection_table.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      189 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/lang/de/modal_verbs.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      165 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/lang/de/quotation_marks.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      218 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/lang/de/semi_modal_verbs.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      561 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/lang/de/speech_verbs.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     9024 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/linguistics.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      765 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/lookups.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     3138 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/model.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1810 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/neuralcoref.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     6376 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pickling.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.900489 monapipe-4.0.0/src/monapipe/pipeline/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/__init__.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.907724 monapipe-4.0.0/src/monapipe/pipeline/annotation_reader/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/annotation_reader/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      600 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/annotation_reader/annotation_reader.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    15821 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/annotation_reader/catma_annotation_reader.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.911599 monapipe-4.0.0/src/monapipe/pipeline/attribution_tagger/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/attribution_tagger/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      450 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/attribution_tagger/attribution_tagger.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     7986 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/attribution_tagger/neural_attribution_tagger.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.916744 monapipe-4.0.0/src/monapipe/pipeline/clausizer/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/clausizer/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1326 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/clausizer/clausizer.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     8328 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/clausizer/dependency_clausizer.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.921086 monapipe-4.0.0/src/monapipe/pipeline/coref/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/coref/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1056 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/coref/coref.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    25000 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/coref/rb_coref.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.923641 monapipe-4.0.0/src/monapipe/pipeline/emotion_tagger/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/emotion_tagger/__init__.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.926965 monapipe-4.0.0/src/monapipe/pipeline/event_tagger/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/event_tagger/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      420 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/event_tagger/event_tagger.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2816 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/event_tagger/neural_event_tagger.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.934101 monapipe-4.0.0/src/monapipe/pipeline/formatter/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/formatter/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     7262 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/formatter/conllu_formatter.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      931 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/formatter/formatter.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.938377 monapipe-4.0.0/src/monapipe/pipeline/gen_tagger/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/gen_tagger/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      514 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/gen_tagger/gen_tagger.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4240 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/gen_tagger/neural_gen_tagger.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4898 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/methods.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.940213 monapipe-4.0.0/src/monapipe/pipeline/ner/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/ner/__init__.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.943427 monapipe-4.0.0/src/monapipe/pipeline/normalizer/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/normalizer/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2160 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/normalizer/identity_normalizer.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      948 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/normalizer/normalizer.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.950664 monapipe-4.0.0/src/monapipe/pipeline/reflection_tagger/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/reflection_tagger/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2195 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/reflection_tagger/methods.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4218 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/reflection_tagger/neural_reflection_tagger.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      528 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/reflection_tagger/reflection_tagger.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.954818 monapipe-4.0.0/src/monapipe/pipeline/semantic_tagger/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/semantic_tagger/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    14223 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/semantic_tagger/germanet_semantic_tagger.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      567 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/semantic_tagger/semantic_tagger.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.960827 monapipe-4.0.0/src/monapipe/pipeline/slicer/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/slicer/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     3009 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/slicer/from_start_slicer.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1186 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/slicer/methods.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      577 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/slicer/slicer.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.964643 monapipe-4.0.0/src/monapipe/pipeline/speaker_extractor/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/speaker_extractor/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     7025 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/speaker_extractor/rb_speaker_extractor.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      552 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/speaker_extractor/speaker_extractor.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.973027 monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4321 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/flair_speech_tagger.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1864 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/methods.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2149 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/quotation_marks_speech_tagger.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      694 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/speech_tagger.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.977323 monapipe-4.0.0/src/monapipe/pipeline/temponym_tagger/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/temponym_tagger/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4918 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/temponym_tagger/heideltime_temponym_tagger.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      518 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/temponym_tagger/temponym_tagger.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.982028 monapipe-4.0.0/src/monapipe/pipeline/verb_analyzer/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/pipeline/verb_analyzer/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    26648 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/verb_analyzer/rb_verb_analyzer.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1348 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/pipeline/verb_analyzer/verb_analyzer.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     8828 2024-01-12 13:36:45.000000 monapipe-4.0.0/src/monapipe/resource_handler.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.984220 monapipe-4.0.0/src/monapipe/resources/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/__init__.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.985523 monapipe-4.0.0/src/monapipe/resources/attribution/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/attribution/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      501 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/resources/attribution/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.989724 monapipe-4.0.0/src/monapipe/resources/event_classification/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/__init__.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.006848 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1453 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/config.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    23254 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/datasets.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     9607 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/eval.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1409 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/evaluation_result.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1190 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/label_smoothing.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     7953 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/model.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.012457 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/parser/
--rw-r--r--   0 florianbarth   (502) staff       (20)      233 2023-11-30 17:29:04.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/parser/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2551 2023-11-30 17:29:04.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/parser/spacy_herma.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1259 2023-11-30 17:29:04.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/parser/spacy_parzu.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1727 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/preprocessing.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     5233 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/segmentations.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4614 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/util.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2296 2023-11-30 17:28:54.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/event_test.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1831 2024-01-11 17:13:47.000000 monapipe-4.0.0/src/monapipe/resources/event_classification/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.014660 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2798 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.799519 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.021157 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/
--rw-r--r--   0 florianbarth   (502) staff       (20)     2947 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_reflexive_training.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1785 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_training.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2668 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_xai.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.070584 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/
--rw-r--r--   0 florianbarth   (502) staff       (20)      122 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2863 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/custom_dataset.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2543 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/early_stopping.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    14733 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/experiment.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     3878 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/label_util.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4436 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/lamb.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     6800 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/model_util.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2342 2023-11-30 17:44:35.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/multi_label_classification_model.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2328 2023-11-30 17:44:35.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/saved_model_tester.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    11203 2023-11-30 17:44:35.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/trainer.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.077689 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/
--rw-r--r--   0 florianbarth   (502) staff       (20)     2621 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/cage_preprocessing.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     8940 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/conllu_parser.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.083805 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/
--rw-r--r--   0 florianbarth   (502) staff       (20)     5995 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/clause.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      235 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/document.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      347 2023-11-30 17:44:35.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/passage.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4418 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/monaco_preprocessing.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     7531 2023-11-30 17:44:35.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/sitent_preprocessing.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.091619 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/
--rw-r--r--   0 florianbarth   (502) staff       (20)     1471 2023-11-30 17:42:18.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/anchors_wrapper.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      923 2023-11-30 17:43:26.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/lime_clause.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2392 2023-11-30 17:44:35.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/prediction_pipeline.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     8186 2023-11-30 17:44:35.000000 monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/xai_graphic_generator.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.094653 monapipe-4.0.0/src/monapipe/resources/germanet/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/germanet/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      585 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/germanet/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.097567 monapipe-4.0.0/src/monapipe/resources/heideltime/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/heideltime/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2697 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/heideltime/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.101482 monapipe-4.0.0/src/monapipe/resources/open_multilingual_wordnet/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/open_multilingual_wordnet/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2122 2024-01-12 13:36:45.000000 monapipe-4.0.0/src/monapipe/resources/open_multilingual_wordnet/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.104070 monapipe-4.0.0/src/monapipe/resources/parsing/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/parsing/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      682 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/parsing/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.106849 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2798 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:24.804704 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.118530 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/
--rw-r--r--   0 florianbarth   (502) staff       (20)     2947 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_reflexive_training.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1785 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_training.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2668 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_xai.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.137614 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/
--rw-r--r--   0 florianbarth   (502) staff       (20)      122 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2863 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/custom_dataset.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2543 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/early_stopping.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    14733 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/experiment.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     3878 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/label_util.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4436 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/lamb.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     6800 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/model_util.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2342 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/multi_label_classification_model.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2328 2023-11-30 17:50:51.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/saved_model_tester.py
--rw-r--r--   0 florianbarth   (502) staff       (20)    11203 2023-11-30 17:50:51.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/trainer.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.144085 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/
--rw-r--r--   0 florianbarth   (502) staff       (20)     2621 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/cage_preprocessing.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     8940 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/conllu_parser.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.150955 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/
--rw-r--r--   0 florianbarth   (502) staff       (20)     5995 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/clause.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      235 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/document.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      347 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/passage.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     4418 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/monaco_preprocessing.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     7531 2023-11-30 17:50:51.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/sitent_preprocessing.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.158937 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/
--rw-r--r--   0 florianbarth   (502) staff       (20)     1471 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/anchors_wrapper.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      923 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/lime_clause.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     2392 2023-11-30 17:50:26.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/prediction_pipeline.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     8186 2023-11-30 17:50:51.000000 monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/xai_graphic_generator.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.161086 monapipe-4.0.0/src/monapipe/resources/spacy_model/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/spacy_model/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      606 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/spacy_model/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.164130 monapipe-4.0.0/src/monapipe/resources/speech_taggers/
--rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/speech_taggers/__init__.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1174 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/resources/speech_taggers/load.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.168910 monapipe-4.0.0/src/monapipe/scripts/
--rw-r--r--   0 florianbarth   (502) staff       (20)      693 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/scripts/delete_resource_files.py
--rw-r--r--   0 florianbarth   (502) staff       (20)      694 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/scripts/load_resource_files.py
--rw-r--r--   0 florianbarth   (502) staff       (20)     1972 2023-11-30 17:01:54.000000 monapipe-4.0.0/src/monapipe/silence.py
-drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-01-17 10:56:25.170944 monapipe-4.0.0/src/monapipe.egg-info/
--rw-r--r--   0 florianbarth   (502) staff       (20)    47970 2024-01-17 10:56:24.000000 monapipe-4.0.0/src/monapipe.egg-info/PKG-INFO
--rw-r--r--   0 florianbarth   (502) staff       (20)    10505 2024-01-17 10:56:24.000000 monapipe-4.0.0/src/monapipe.egg-info/SOURCES.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)        1 2024-01-17 10:56:24.000000 monapipe-4.0.0/src/monapipe.egg-info/dependency_links.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)      235 2024-01-17 10:56:24.000000 monapipe-4.0.0/src/monapipe.egg-info/requires.txt
--rw-r--r--   0 florianbarth   (502) staff       (20)        9 2024-01-17 10:56:24.000000 monapipe-4.0.0/src/monapipe.egg-info/top_level.txt
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.276322 monapipe-4.1.0/
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:40.996351 monapipe-4.1.0/LICENSES/
+-rw-r--r--   0 florianbarth   (502) staff       (20)    18656 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/CC-BY 4.0.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)    20849 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/CC-BY-NC-SA 4.0.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)    22239 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/CC-BY-SA 3.0.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)    20137 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/CC-BY-SA 4.0.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)     7047 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)    18138 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/FDL-1.1.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)    35146 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/GPL-3.0.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)    42098 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1055 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1916 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/bsd-2-clause.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)      768 2023-11-30 17:01:54.000000 monapipe-4.1.0/LICENSES/open_multilingual_wordnet_license_statement.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)    48058 2024-05-13 12:44:41.268515 monapipe-4.1.0/PKG-INFO
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1516 2024-05-13 12:43:53.000000 monapipe-4.1.0/README.md
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2935 2024-05-13 12:43:53.000000 monapipe-4.1.0/pyproject.toml
+-rw-r--r--   0 florianbarth   (502) staff       (20)       38 2024-05-13 12:44:41.277024 monapipe-4.1.0/setup.cfg
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:40.954091 monapipe-4.1.0/src/
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.012327 monapipe-4.1.0/src/monapipe/
+-rw-r--r--   0 florianbarth   (502) staff       (20)      370 2024-05-13 12:43:53.000000 monapipe-4.1.0/src/monapipe/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2598 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/annotation.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1154 2024-05-13 12:43:53.000000 monapipe-4.1.0/src/monapipe/config.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.021411 monapipe-4.1.0/src/monapipe/lang/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/lang/__init__.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.031363 monapipe-4.1.0/src/monapipe/lang/de/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/lang/de/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      284 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/lang/de/auxiliary_verbs.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    13248 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/lang/de/inflection_table.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      189 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/lang/de/modal_verbs.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      165 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/lang/de/quotation_marks.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      218 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/lang/de/semi_modal_verbs.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      561 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/lang/de/speech_verbs.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     9024 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/linguistics.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      765 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/lookups.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     3138 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/model.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1810 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/neuralcoref.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     6376 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pickling.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.033496 monapipe-4.1.0/src/monapipe/pipeline/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/__init__.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.037115 monapipe-4.1.0/src/monapipe/pipeline/annotation_reader/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/annotation_reader/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      600 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/annotation_reader/annotation_reader.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    15821 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/annotation_reader/catma_annotation_reader.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.040482 monapipe-4.1.0/src/monapipe/pipeline/attribution_tagger/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/attribution_tagger/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      450 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/attribution_tagger/attribution_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     7986 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/attribution_tagger/neural_attribution_tagger.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.044098 monapipe-4.1.0/src/monapipe/pipeline/clausizer/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/clausizer/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1326 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/clausizer/clausizer.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     8328 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/clausizer/dependency_clausizer.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.048076 monapipe-4.1.0/src/monapipe/pipeline/coref/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/coref/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1056 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/coref/coref.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    25000 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/coref/rb_coref.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.050059 monapipe-4.1.0/src/monapipe/pipeline/emotion_tagger/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/emotion_tagger/__init__.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.053189 monapipe-4.1.0/src/monapipe/pipeline/event_tagger/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/event_tagger/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      420 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/event_tagger/event_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2816 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/event_tagger/neural_event_tagger.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.056656 monapipe-4.1.0/src/monapipe/pipeline/formatter/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/formatter/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     7262 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/formatter/conllu_formatter.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      931 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/formatter/formatter.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.060929 monapipe-4.1.0/src/monapipe/pipeline/gen_tagger/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/gen_tagger/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     5162 2024-05-13 12:43:53.000000 monapipe-4.1.0/src/monapipe/pipeline/gen_tagger/flair_gen_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      514 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/gen_tagger/gen_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4240 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/gen_tagger/neural_gen_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4898 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/methods.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.065401 monapipe-4.1.0/src/monapipe/pipeline/ner/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/ner/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     5564 2024-05-13 12:43:53.000000 monapipe-4.1.0/src/monapipe/pipeline/ner/bert_character_ner.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     3030 2024-05-13 12:43:53.000000 monapipe-4.1.0/src/monapipe/pipeline/ner/methods.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      293 2024-05-13 12:43:53.000000 monapipe-4.1.0/src/monapipe/pipeline/ner/ner.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.068575 monapipe-4.1.0/src/monapipe/pipeline/normalizer/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/normalizer/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2160 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/normalizer/identity_normalizer.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      948 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/normalizer/normalizer.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.074324 monapipe-4.1.0/src/monapipe/pipeline/reflection_tagger/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/reflection_tagger/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2195 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/reflection_tagger/methods.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4218 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/reflection_tagger/neural_reflection_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      528 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/reflection_tagger/reflection_tagger.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.078075 monapipe-4.1.0/src/monapipe/pipeline/semantic_tagger/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/semantic_tagger/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    14223 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/semantic_tagger/germanet_semantic_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      567 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/semantic_tagger/semantic_tagger.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.082841 monapipe-4.1.0/src/monapipe/pipeline/slicer/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/slicer/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     3009 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/slicer/from_start_slicer.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1186 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/slicer/methods.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      577 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/slicer/slicer.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.086652 monapipe-4.1.0/src/monapipe/pipeline/speaker_extractor/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/speaker_extractor/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     7025 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/speaker_extractor/rb_speaker_extractor.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      552 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/speaker_extractor/speaker_extractor.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.093335 monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4321 2024-05-07 07:09:34.000000 monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/flair_speech_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1864 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/methods.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2149 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/quotation_marks_speech_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      694 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/speech_tagger.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.098770 monapipe-4.1.0/src/monapipe/pipeline/temponym_tagger/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/temponym_tagger/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4918 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/temponym_tagger/heideltime_temponym_tagger.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      518 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/temponym_tagger/temponym_tagger.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.108108 monapipe-4.1.0/src/monapipe/pipeline/verb_analyzer/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/pipeline/verb_analyzer/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    26648 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/verb_analyzer/rb_verb_analyzer.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1348 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/pipeline/verb_analyzer/verb_analyzer.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     8828 2024-01-12 13:36:45.000000 monapipe-4.1.0/src/monapipe/resource_handler.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.109616 monapipe-4.1.0/src/monapipe/resources/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/__init__.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.111423 monapipe-4.1.0/src/monapipe/resources/attribution/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/attribution/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      501 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/resources/attribution/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.115607 monapipe-4.1.0/src/monapipe/resources/event_classification/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/__init__.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.132213 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1453 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/config.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    23254 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/datasets.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     9607 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/eval.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1409 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/evaluation_result.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1190 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/label_smoothing.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     7953 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/model.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.138327 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/parser/
+-rw-r--r--   0 florianbarth   (502) staff       (20)      233 2023-11-30 17:29:04.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/parser/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2551 2023-11-30 17:29:04.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/parser/spacy_herma.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1259 2023-11-30 17:29:04.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/parser/spacy_parzu.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1727 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/preprocessing.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     5233 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/segmentations.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4614 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/util.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2296 2023-11-30 17:28:54.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/event_test.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1831 2024-01-11 17:13:47.000000 monapipe-4.1.0/src/monapipe/resources/event_classification/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.140310 monapipe-4.1.0/src/monapipe/resources/flair_gen_tagger_cv/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:43:53.000000 monapipe-4.1.0/src/monapipe/resources/flair_gen_tagger_cv/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      735 2024-05-13 12:43:53.000000 monapipe-4.1.0/src/monapipe/resources/flair_gen_tagger_cv/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.142166 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2798 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:40.973701 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.147257 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2947 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_reflexive_training.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1785 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_training.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2668 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_xai.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.166119 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/
+-rw-r--r--   0 florianbarth   (502) staff       (20)      122 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2863 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/custom_dataset.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2543 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/early_stopping.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    14733 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/experiment.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     3878 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/label_util.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4436 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/lamb.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     6800 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/model_util.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2342 2023-11-30 17:44:35.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/multi_label_classification_model.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2328 2023-11-30 17:44:35.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/saved_model_tester.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    11203 2023-11-30 17:44:35.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/trainer.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.173278 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2621 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/cage_preprocessing.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     8940 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/conllu_parser.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.177444 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/
+-rw-r--r--   0 florianbarth   (502) staff       (20)     5995 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/clause.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      235 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/document.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      347 2023-11-30 17:44:35.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/passage.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4418 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/monaco_preprocessing.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     7531 2023-11-30 17:44:35.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/sitent_preprocessing.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.183211 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1471 2023-11-30 17:42:18.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/anchors_wrapper.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      923 2023-11-30 17:43:26.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/lime_clause.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2392 2023-11-30 17:44:35.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/prediction_pipeline.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     8186 2023-11-30 17:44:35.000000 monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/xai_graphic_generator.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.185332 monapipe-4.1.0/src/monapipe/resources/germanet/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/germanet/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      585 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/germanet/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.187712 monapipe-4.1.0/src/monapipe/resources/heideltime/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/heideltime/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2697 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/heideltime/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.190682 monapipe-4.1.0/src/monapipe/resources/open_multilingual_wordnet/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/open_multilingual_wordnet/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2122 2024-01-12 13:36:45.000000 monapipe-4.1.0/src/monapipe/resources/open_multilingual_wordnet/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.193122 monapipe-4.1.0/src/monapipe/resources/parsing/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/parsing/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      682 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/parsing/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.195882 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2798 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:40.978376 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.200815 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2947 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_reflexive_training.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1785 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_training.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2668 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_xai.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.219367 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/
+-rw-r--r--   0 florianbarth   (502) staff       (20)      122 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2863 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/custom_dataset.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2543 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/early_stopping.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    14733 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/experiment.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     3878 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/label_util.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4436 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/lamb.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     6800 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/model_util.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2342 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/multi_label_classification_model.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2328 2023-11-30 17:50:51.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/saved_model_tester.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)    11203 2023-11-30 17:50:51.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/trainer.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.225900 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2621 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/cage_preprocessing.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     8940 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/conllu_parser.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.229558 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/
+-rw-r--r--   0 florianbarth   (502) staff       (20)     5995 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/clause.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      235 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/document.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      347 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/passage.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     4418 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/monaco_preprocessing.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     7531 2023-11-30 17:50:51.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/sitent_preprocessing.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.234634 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1471 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/anchors_wrapper.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      923 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/lime_clause.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     2392 2023-11-30 17:50:26.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/prediction_pipeline.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     8186 2023-11-30 17:50:51.000000 monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/xai_graphic_generator.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.237217 monapipe-4.1.0/src/monapipe/resources/spacy_model/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/spacy_model/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      606 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/spacy_model/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.246513 monapipe-4.1.0/src/monapipe/resources/speech_taggers/
+-rw-r--r--   0 florianbarth   (502) staff       (20)        0 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/resources/speech_taggers/__init__.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1174 2024-05-07 07:09:34.000000 monapipe-4.1.0/src/monapipe/resources/speech_taggers/load.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.256675 monapipe-4.1.0/src/monapipe/scripts/
+-rw-r--r--   0 florianbarth   (502) staff       (20)      693 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/scripts/delete_resource_files.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)      694 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/scripts/load_resource_files.py
+-rw-r--r--   0 florianbarth   (502) staff       (20)     1972 2023-11-30 17:01:54.000000 monapipe-4.1.0/src/monapipe/silence.py
+drwxr-xr-x   0 florianbarth   (502) staff       (20)        0 2024-05-13 12:44:41.260500 monapipe-4.1.0/src/monapipe.egg-info/
+-rw-r--r--   0 florianbarth   (502) staff       (20)    48058 2024-05-13 12:44:40.000000 monapipe-4.1.0/src/monapipe.egg-info/PKG-INFO
+-rw-r--r--   0 florianbarth   (502) staff       (20)    10782 2024-05-13 12:44:40.000000 monapipe-4.1.0/src/monapipe.egg-info/SOURCES.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)        1 2024-05-13 12:44:40.000000 monapipe-4.1.0/src/monapipe.egg-info/dependency_links.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)      290 2024-05-13 12:44:40.000000 monapipe-4.1.0/src/monapipe.egg-info/requires.txt
+-rw-r--r--   0 florianbarth   (502) staff       (20)        9 2024-05-13 12:44:40.000000 monapipe-4.1.0/src/monapipe.egg-info/top_level.txt
```

### Comparing `monapipe-4.0.0/LICENSES/CC-BY 4.0.txt` & `monapipe-4.1.0/LICENSES/CC-BY 4.0.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/CC-BY-NC-SA 4.0.txt` & `monapipe-4.1.0/LICENSES/CC-BY-NC-SA 4.0.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/CC-BY-SA 3.0.txt` & `monapipe-4.1.0/LICENSES/CC-BY-SA 3.0.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/CC-BY-SA 4.0.txt` & `monapipe-4.1.0/LICENSES/CC-BY-SA 4.0.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/CC0-1.0.txt` & `monapipe-4.1.0/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/FDL-1.1.txt` & `monapipe-4.1.0/LICENSES/FDL-1.1.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/GPL-3.0.txt` & `monapipe-4.1.0/LICENSES/GPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/LGPL-3.0-or-later.txt` & `monapipe-4.1.0/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/MIT.txt` & `monapipe-4.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/bsd-2-clause.txt` & `monapipe-4.1.0/LICENSES/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/LICENSES/open_multilingual_wordnet_license_statement.txt` & `monapipe-4.1.0/LICENSES/open_multilingual_wordnet_license_statement.txt`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/PKG-INFO` & `monapipe-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monapipe
-Version: 4.0.0
+Version: 4.1.0
 Summary: MONAPipe provides natural-language-processing tools for German, implemented in Python/spaCy.
 Author: Tillmann Dönicke, Florian Barth, Hanna Varachkina
 Maintainer-email: Florian Barth <florian.barth@uni-goettingen.de>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -327,41 +327,44 @@
 License-File: LICENSES/CC0-1.0.txt
 License-File: LICENSES/FDL-1.1.txt
 License-File: LICENSES/GPL-3.0.txt
 License-File: LICENSES/LGPL-3.0-or-later.txt
 License-File: LICENSES/MIT.txt
 License-File: LICENSES/bsd-2-clause.txt
 License-File: LICENSES/open_multilingual_wordnet_license_statement.txt
-Requires-Dist: pip>=23.2.1
-Requires-Dist: setuptools>=61.0
+Requires-Dist: pip>=23.2.2
+Requires-Dist: setuptools>=69.0.3
+Requires-Dist: wheel>=0.42.0
 Requires-Dist: dill
 Requires-Dist: flair<=0.12.2
 Requires-Dist: germanetpy
 Requires-Dist: ipykernel
 Requires-Dist: minetext
 Requires-Dist: mlflow
 Requires-Dist: nltk
 Requires-Dist: omegaconf
 Requires-Dist: pytorch_transformers
 Requires-Dist: seaborn
-Requires-Dist: spacy
+Requires-Dist: scipy<1.13.0
+Requires-Dist: spacy>=3.0
 Requires-Dist: spacy-dbpedia-spotlight
 Requires-Dist: spacy_download
 Requires-Dist: spacyopentapioca
-Requires-Dist: tensorflow
+Requires-Dist: spacyfishing
+Requires-Dist: tensorflow<=2.13.1
 Requires-Dist: torch<2.0
 Requires-Dist: tgclients
 Requires-Dist: transformers
 
 <!--readme-about-start-->
 # MONAPipe
 
 MONAPipe stands for "Modes of Narration and Attribution Pipeline". It provides natural-language-processing tools for German, implemented in Python/spaCy. In addition to spaCy's default components, MONAPipe adds specific custom components and models for Digital Humanities and Computational Literary Studies.
 
-MONAPipe was originally created in the project group [MONA](https://www.uni-goettingen.de/de/mona/626918.html) and is now further developed within the [Text+](https://www.text-plus.org/en/home/) infrastructure.
+MONAPipe was originally created in the project group [MONA](https://www.uni-goettingen.de/de/mona/626918.html) and is now further developed within the [Text+](https://text-plus.org/) infrastructure.
 <!--readme-about-end-->
 
 
 ## Installation and Usage
 
 <!--readme-installation-start-->
 Currently, MONAPipe supports Python 3.8, 3.9, and 3.10. Support for Python 3.11 is on the way.
```

### Comparing `monapipe-4.0.0/README.md` & `monapipe-4.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!--readme-about-start-->
 # MONAPipe
 
 MONAPipe stands for "Modes of Narration and Attribution Pipeline". It provides natural-language-processing tools for German, implemented in Python/spaCy. In addition to spaCy's default components, MONAPipe adds specific custom components and models for Digital Humanities and Computational Literary Studies.
 
-MONAPipe was originally created in the project group [MONA](https://www.uni-goettingen.de/de/mona/626918.html) and is now further developed within the [Text+](https://www.text-plus.org/en/home/) infrastructure.
+MONAPipe was originally created in the project group [MONA](https://www.uni-goettingen.de/de/mona/626918.html) and is now further developed within the [Text+](https://text-plus.org/) infrastructure.
 <!--readme-about-end-->
 
 
 ## Installation and Usage
 
 <!--readme-installation-start-->
 Currently, MONAPipe supports Python 3.8, 3.9, and 3.10. Support for Python 3.11 is on the way.
```

### Comparing `monapipe-4.0.0/pyproject.toml` & `monapipe-4.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "monapipe"
-version = "4.0.0"
+version = "4.1.0"
 authors = [
     { name = "Tillmann Dönicke, Florian Barth, Hanna Varachkina"}
 ]
 maintainers = [
     { name = "Florian Barth", email = "florian.barth@uni-goettingen.de"}
 ]
 description = "MONAPipe provides natural-language-processing tools for German, implemented in Python/spaCy."
@@ -25,36 +25,64 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "pip>=23.2.1",
-    "setuptools>=61.0",
+    "pip>=23.2.2",
+    "setuptools>=69.0.3",
+    "wheel>=0.42.0",
     "dill",
     "flair<=0.12.2", # 13.0 produces https://gitlab.gwdg.de/text-plus-collections/mona-pipe/-/jobs/1214318
     "germanetpy",
     "ipykernel",
     "minetext",
     "mlflow",
     "nltk",
     "omegaconf",
     "pytorch_transformers",
     "seaborn",
-    "spacy",
+    "scipy<1.13.0", # 1.13.0 produces https://gitlab.gwdg.de/text-plus-collections/mona-pipe/-/jobs/1377017 for Python 3.9/3.10
+    "spacy>=3.0",
     "spacy-dbpedia-spotlight",
     "spacy_download",
     "spacyopentapioca",
-    "tensorflow",
+    "spacyfishing",
+    "tensorflow<=2.13.1", # 2.16.1 installs incompatible keras version that produces https://gitlab.gwdg.de/text-plus-collections/mona-pipe/-/jobs/1377080 in attribution tagger for Python 3.9/3.10
     "torch<2.0", # <2.0 to work with flair
     "tgclients",
     "transformers",
 ]
 
+[tool.semantic_release]
+commit_parser = "angular"
+version_variables = ["src/monapipe/__init__.py:__version__"]
+version_toml = [
+    "pyproject.toml:project.version",
+]
+
+[tool.semantic_release.branches.main]
+match = "main"
+
+[tool.semantic_release.changelog]
+exclude_commit_patterns = ["build", "chore", "ci", "docs", "perf", "style", "refactor", "test", "Conflicts", "Merge branch*", "Revert*"]
+
+[tool.semantic_release.commit_author]
+env = "GIT_COMMIT_AUTHOR"
+default = "semantic-release <semantic-release>"
+
+[tool.semantic_release.commit_parser_options]
+allowed_tags = ["build", "chore", "ci", "docs", "feat", "fix", "perf", "style", "refactor", "test"]
+minor_tags = ["feat"]
+patch_tags = ["fix", "perf"]
+
+[tool.semantic_release.remote]
+type = "gitlab"
+
 [tool.setuptools]
 license-files = ["LICENSES/*.txt"]
 package-dir = {"" = "src"}
 
 [project.urls]
 "Documentation" = "https://text-plus-collections.pages.gwdg.de/mona-pipe"
 "Source" = "https://gitlab.gwdg.de/text-plus-collections/mona-pipe"
```

### Comparing `monapipe-4.0.0/src/monapipe/annotation.py` & `monapipe-4.1.0/src/monapipe/annotation.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/config.py` & `monapipe-4.1.0/src/monapipe/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,20 +6,28 @@
 
 from torch import cuda
 
 DATAVERSE = {
     "api_token": "",
     "doi_attribution": "doi:10.25625/2D9CAV&version=1.0",
     "doi_event_classification": "doi:10.25625/0GUOMC&version=1.1",
+    "doi_flair_gen_tagger_cv": "doi:10.25625/V7HTB8&version=2.1",
     "doi_generalizing_passages_identification_bert": "doi:10.25625/2PHXNC&version=1.1",
     "doi_heideltime": "doi:10.25625/SIPQEF&version=1.0",
     "doi_open_multilingual_wordnet": "doi:10.25625/LE57DV&version=1.0",
     "doi_parsing": "doi:10.25625/S2LPJP&version=1.1",
     "doi_reflective_passages_identification_bert": "doi:10.25625/0HXWYG&version=1.1",
 }
 
+HUGGINGFACE_HUB = {
+    "fiction-gbert-char-ner": {
+        "pretrained_model_name_or_path": "LennartKeller/fiction-gbert-large-droc-np-ner",
+        "revision": "a75cf9fe8be4e45856049c289a0317c82f68c50a",
+    }
+}
+
 LOCAL_PATHS = {"germanet": os.path.join(os.path.dirname(__file__), "..", "..", "..", "germanet")}
 
 SETTINGS = {
     "spacy_max_length": 12000000,
     "torch_device": ("cuda" if cuda.is_available() else "cpu"),
 }
```

### Comparing `monapipe-4.0.0/src/monapipe/lang/de/inflection_table.py` & `monapipe-4.1.0/src/monapipe/lang/de/inflection_table.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/lang/de/speech_verbs.py` & `monapipe-4.1.0/src/monapipe/lang/de/speech_verbs.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/linguistics.py` & `monapipe-4.1.0/src/monapipe/linguistics.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/lookups.py` & `monapipe-4.1.0/src/monapipe/lookups.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/model.py` & `monapipe-4.1.0/src/monapipe/model.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/neuralcoref.py` & `monapipe-4.1.0/src/monapipe/neuralcoref.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pickling.py` & `monapipe-4.1.0/src/monapipe/pickling.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/annotation_reader/annotation_reader.py` & `monapipe-4.1.0/src/monapipe/pipeline/annotation_reader/annotation_reader.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/annotation_reader/catma_annotation_reader.py` & `monapipe-4.1.0/src/monapipe/pipeline/annotation_reader/catma_annotation_reader.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/attribution_tagger/neural_attribution_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/attribution_tagger/neural_attribution_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/clausizer/clausizer.py` & `monapipe-4.1.0/src/monapipe/pipeline/clausizer/clausizer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/clausizer/dependency_clausizer.py` & `monapipe-4.1.0/src/monapipe/pipeline/clausizer/dependency_clausizer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/coref/coref.py` & `monapipe-4.1.0/src/monapipe/pipeline/coref/coref.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/coref/rb_coref.py` & `monapipe-4.1.0/src/monapipe/pipeline/coref/rb_coref.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/event_tagger/neural_event_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/event_tagger/neural_event_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/formatter/conllu_formatter.py` & `monapipe-4.1.0/src/monapipe/pipeline/formatter/conllu_formatter.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/formatter/formatter.py` & `monapipe-4.1.0/src/monapipe/pipeline/formatter/formatter.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/gen_tagger/gen_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/gen_tagger/gen_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/gen_tagger/neural_gen_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/gen_tagger/neural_gen_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/methods.py` & `monapipe-4.1.0/src/monapipe/pipeline/methods.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/normalizer/identity_normalizer.py` & `monapipe-4.1.0/src/monapipe/pipeline/normalizer/identity_normalizer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/normalizer/normalizer.py` & `monapipe-4.1.0/src/monapipe/pipeline/normalizer/normalizer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/reflection_tagger/methods.py` & `monapipe-4.1.0/src/monapipe/pipeline/reflection_tagger/methods.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/reflection_tagger/neural_reflection_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/reflection_tagger/neural_reflection_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/reflection_tagger/reflection_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/reflection_tagger/reflection_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/semantic_tagger/germanet_semantic_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/semantic_tagger/germanet_semantic_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/semantic_tagger/semantic_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/semantic_tagger/semantic_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/slicer/from_start_slicer.py` & `monapipe-4.1.0/src/monapipe/pipeline/slicer/from_start_slicer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/slicer/methods.py` & `monapipe-4.1.0/src/monapipe/pipeline/slicer/methods.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/slicer/slicer.py` & `monapipe-4.1.0/src/monapipe/pipeline/slicer/slicer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/speaker_extractor/rb_speaker_extractor.py` & `monapipe-4.1.0/src/monapipe/pipeline/speaker_extractor/rb_speaker_extractor.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/speaker_extractor/speaker_extractor.py` & `monapipe-4.1.0/src/monapipe/pipeline/speaker_extractor/speaker_extractor.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/flair_speech_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/flair_speech_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/methods.py` & `monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/methods.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/quotation_marks_speech_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/quotation_marks_speech_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/speech_tagger/speech_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/speech_tagger/speech_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/temponym_tagger/heideltime_temponym_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/temponym_tagger/heideltime_temponym_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/temponym_tagger/temponym_tagger.py` & `monapipe-4.1.0/src/monapipe/pipeline/temponym_tagger/temponym_tagger.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/verb_analyzer/rb_verb_analyzer.py` & `monapipe-4.1.0/src/monapipe/pipeline/verb_analyzer/rb_verb_analyzer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/pipeline/verb_analyzer/verb_analyzer.py` & `monapipe-4.1.0/src/monapipe/pipeline/verb_analyzer/verb_analyzer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resource_handler.py` & `monapipe-4.1.0/src/monapipe/resource_handler.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/config.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/config.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/datasets.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/datasets.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/eval.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/eval.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/evaluation_result.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/label_smoothing.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/model.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/model.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/parser/spacy_herma.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/parser/spacy_herma.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/parser/spacy_parzu.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/parser/spacy_parzu.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/preprocessing.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/preprocessing.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/segmentations.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/segmentations.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_classify/util.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_classify/util.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/event_test.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/event_test.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/event_classification/load.py` & `monapipe-4.1.0/src/monapipe/resources/event_classification/load.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/load.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/load.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_reflexive_training.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_reflexive_training.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_training.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_training.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_xai.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_xai.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/custom_dataset.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/early_stopping.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/early_stopping.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/experiment.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/label_util.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/label_util.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/lamb.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/lamb.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/model_util.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/model_util.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/multi_label_classification_model.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/multi_label_classification_model.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/saved_model_tester.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/saved_model_tester.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/trainer.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/ml/trainer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/cage_preprocessing.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/cage_preprocessing.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/conllu_parser.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/conllu_parser.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/clause.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/models/clause.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/monaco_preprocessing.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/monaco_preprocessing.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/sitent_preprocessing.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/preprocessing/sitent_preprocessing.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/anchors_wrapper.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/anchors_wrapper.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/lime_clause.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/lime_clause.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/prediction_pipeline.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/xai_graphic_generator.py` & `monapipe-4.1.0/src/monapipe/resources/generalizing_passages_identification_bert/src/xai/xai_graphic_generator.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/germanet/load.py` & `monapipe-4.1.0/src/monapipe/resources/germanet/load.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/heideltime/load.py` & `monapipe-4.1.0/src/monapipe/resources/heideltime/load.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/open_multilingual_wordnet/load.py` & `monapipe-4.1.0/src/monapipe/resources/open_multilingual_wordnet/load.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/parsing/load.py` & `monapipe-4.1.0/src/monapipe/resources/parsing/load.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/load.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/load.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_reflexive_training.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_reflexive_training.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_training.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_training.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_xai.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/examples/example_xai.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/custom_dataset.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/early_stopping.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/early_stopping.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/experiment.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/label_util.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/label_util.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/lamb.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/lamb.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/model_util.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/model_util.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/multi_label_classification_model.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/multi_label_classification_model.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/saved_model_tester.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/saved_model_tester.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/trainer.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/ml/trainer.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/cage_preprocessing.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/cage_preprocessing.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/conllu_parser.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/conllu_parser.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/clause.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/models/clause.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/monaco_preprocessing.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/monaco_preprocessing.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/sitent_preprocessing.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/preprocessing/sitent_preprocessing.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/anchors_wrapper.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/anchors_wrapper.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/lime_clause.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/lime_clause.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/prediction_pipeline.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/prediction_pipeline.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/xai_graphic_generator.py` & `monapipe-4.1.0/src/monapipe/resources/reflective_passages_identification_bert/src/xai/xai_graphic_generator.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/spacy_model/load.py` & `monapipe-4.1.0/src/monapipe/resources/spacy_model/load.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/resources/speech_taggers/load.py` & `monapipe-4.1.0/src/monapipe/resources/speech_taggers/load.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/scripts/delete_resource_files.py` & `monapipe-4.1.0/src/monapipe/scripts/delete_resource_files.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/scripts/load_resource_files.py` & `monapipe-4.1.0/src/monapipe/scripts/load_resource_files.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe/silence.py` & `monapipe-4.1.0/src/monapipe/silence.py`

 * *Files identical despite different names*

### Comparing `monapipe-4.0.0/src/monapipe.egg-info/PKG-INFO` & `monapipe-4.1.0/src/monapipe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monapipe
-Version: 4.0.0
+Version: 4.1.0
 Summary: MONAPipe provides natural-language-processing tools for German, implemented in Python/spaCy.
 Author: Tillmann Dönicke, Florian Barth, Hanna Varachkina
 Maintainer-email: Florian Barth <florian.barth@uni-goettingen.de>
 License: GNU LESSER GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -327,41 +327,44 @@
 License-File: LICENSES/CC0-1.0.txt
 License-File: LICENSES/FDL-1.1.txt
 License-File: LICENSES/GPL-3.0.txt
 License-File: LICENSES/LGPL-3.0-or-later.txt
 License-File: LICENSES/MIT.txt
 License-File: LICENSES/bsd-2-clause.txt
 License-File: LICENSES/open_multilingual_wordnet_license_statement.txt
-Requires-Dist: pip>=23.2.1
-Requires-Dist: setuptools>=61.0
+Requires-Dist: pip>=23.2.2
+Requires-Dist: setuptools>=69.0.3
+Requires-Dist: wheel>=0.42.0
 Requires-Dist: dill
 Requires-Dist: flair<=0.12.2
 Requires-Dist: germanetpy
 Requires-Dist: ipykernel
 Requires-Dist: minetext
 Requires-Dist: mlflow
 Requires-Dist: nltk
 Requires-Dist: omegaconf
 Requires-Dist: pytorch_transformers
 Requires-Dist: seaborn
-Requires-Dist: spacy
+Requires-Dist: scipy<1.13.0
+Requires-Dist: spacy>=3.0
 Requires-Dist: spacy-dbpedia-spotlight
 Requires-Dist: spacy_download
 Requires-Dist: spacyopentapioca
-Requires-Dist: tensorflow
+Requires-Dist: spacyfishing
+Requires-Dist: tensorflow<=2.13.1
 Requires-Dist: torch<2.0
 Requires-Dist: tgclients
 Requires-Dist: transformers
 
 <!--readme-about-start-->
 # MONAPipe
 
 MONAPipe stands for "Modes of Narration and Attribution Pipeline". It provides natural-language-processing tools for German, implemented in Python/spaCy. In addition to spaCy's default components, MONAPipe adds specific custom components and models for Digital Humanities and Computational Literary Studies.
 
-MONAPipe was originally created in the project group [MONA](https://www.uni-goettingen.de/de/mona/626918.html) and is now further developed within the [Text+](https://www.text-plus.org/en/home/) infrastructure.
+MONAPipe was originally created in the project group [MONA](https://www.uni-goettingen.de/de/mona/626918.html) and is now further developed within the [Text+](https://text-plus.org/) infrastructure.
 <!--readme-about-end-->
 
 
 ## Installation and Usage
 
 <!--readme-installation-start-->
 Currently, MONAPipe supports Python 3.8, 3.9, and 3.10. Support for Python 3.11 is on the way.
```

### Comparing `monapipe-4.0.0/src/monapipe.egg-info/SOURCES.txt` & `monapipe-4.1.0/src/monapipe.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -52,17 +52,21 @@
 src/monapipe/pipeline/event_tagger/__init__.py
 src/monapipe/pipeline/event_tagger/event_tagger.py
 src/monapipe/pipeline/event_tagger/neural_event_tagger.py
 src/monapipe/pipeline/formatter/__init__.py
 src/monapipe/pipeline/formatter/conllu_formatter.py
 src/monapipe/pipeline/formatter/formatter.py
 src/monapipe/pipeline/gen_tagger/__init__.py
+src/monapipe/pipeline/gen_tagger/flair_gen_tagger.py
 src/monapipe/pipeline/gen_tagger/gen_tagger.py
 src/monapipe/pipeline/gen_tagger/neural_gen_tagger.py
 src/monapipe/pipeline/ner/__init__.py
+src/monapipe/pipeline/ner/bert_character_ner.py
+src/monapipe/pipeline/ner/methods.py
+src/monapipe/pipeline/ner/ner.py
 src/monapipe/pipeline/normalizer/__init__.py
 src/monapipe/pipeline/normalizer/identity_normalizer.py
 src/monapipe/pipeline/normalizer/normalizer.py
 src/monapipe/pipeline/reflection_tagger/__init__.py
 src/monapipe/pipeline/reflection_tagger/methods.py
 src/monapipe/pipeline/reflection_tagger/neural_reflection_tagger.py
 src/monapipe/pipeline/reflection_tagger/reflection_tagger.py
@@ -102,14 +106,16 @@
 src/monapipe/resources/event_classification/event_classify/model.py
 src/monapipe/resources/event_classification/event_classify/preprocessing.py
 src/monapipe/resources/event_classification/event_classify/segmentations.py
 src/monapipe/resources/event_classification/event_classify/util.py
 src/monapipe/resources/event_classification/event_classify/parser/__init__.py
 src/monapipe/resources/event_classification/event_classify/parser/spacy_herma.py
 src/monapipe/resources/event_classification/event_classify/parser/spacy_parzu.py
+src/monapipe/resources/flair_gen_tagger_cv/__init__.py
+src/monapipe/resources/flair_gen_tagger_cv/load.py
 src/monapipe/resources/generalizing_passages_identification_bert/__init__.py
 src/monapipe/resources/generalizing_passages_identification_bert/load.py
 src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_reflexive_training.py
 src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_training.py
 src/monapipe/resources/generalizing_passages_identification_bert/src/examples/example_xai.py
 src/monapipe/resources/generalizing_passages_identification_bert/src/ml/__init__.py
 src/monapipe/resources/generalizing_passages_identification_bert/src/ml/custom_dataset.py
```

