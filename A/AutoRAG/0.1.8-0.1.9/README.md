# Comparing `tmp/autorag-0.1.8.tar.gz` & `tmp/autorag-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autorag-0.1.8.tar", last modified: Mon Apr 29 14:33:49 2024, max compression
+gzip compressed data, was "autorag-0.1.9.tar", last modified: Wed May  1 06:27:49 2024, max compression
```

## Comparing `autorag-0.1.8.tar` & `autorag-0.1.9.tar`

### file list

```diff
@@ -1,515 +1,518 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.267387 autorag-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.175387 autorag-0.1.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-29 14:33:32.000000 autorag-0.1.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.175387 autorag-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-29 14:33:32.000000 autorag-0.1.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 14:33:32.000000 autorag-0.1.8/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-29 14:33:32.000000 autorag-0.1.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-29 14:33:32.000000 autorag-0.1.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.263387 autorag-0.1.8/AutoRAG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-29 14:33:49.000000 autorag-0.1.8/AutoRAG.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-29 14:33:32.000000 autorag-0.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-29 14:33:32.000000 autorag-0.1.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 14:33:32.000000 autorag-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-04-29 14:33:49.263387 autorag-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-04-29 14:33:32.000000 autorag-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.175387 autorag-0.1.8/autorag/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/data/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/corpus/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/corpus/llama_index.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/data/qacreation/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/llama_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/llama_index_default_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/ragas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/qacreation/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/data/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/data/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/evaluate/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.179386 autorag-0.1.8/autorag/evaluate/metric/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/retrieval_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/metric/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/retrieval_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17379 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/node_line.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/llama_index_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/generator/vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/nodes/passageaugmenter/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/prev_next_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passageaugmenter/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.183386 autorag-0.1.8/autorag/nodes/passagecompressor/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/pass_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagecompressor/tree_summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.187387 autorag-0.1.8/autorag/nodes/passagefilter/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/pass_passage_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/recency.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagefilter/threshold_cutoff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.187387 autorag-0.1.8/autorag/nodes/passagereranker/
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/cohere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/colbert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/flag_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/flag_embedding_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/jina.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/koreranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/monot5.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/pass_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/rankgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/sentence_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.187387 autorag-0.1.8/autorag/nodes/passagereranker/tart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/tart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/tart/tart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/time_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/passagereranker/upr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.191387 autorag-0.1.8/autorag/nodes/promptmaker/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/long_context_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/promptmaker/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.191387 autorag-0.1.8/autorag/nodes/queryexpansion/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/hyde.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/pass_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/query_decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/queryexpansion/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.191387 autorag-0.1.8/autorag/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/hybrid_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/hybrid_dbsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/hybrid_rrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/hybrid_rsf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/nodes/retrieval/vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.191387 autorag-0.1.8/autorag/schema/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/schema/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/schema/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/support.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.195387 autorag-0.1.8/autorag/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-29 14:33:32.000000 autorag-0.1.8/autorag/web.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-29 14:33:32.000000 autorag-0.1.8/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.195387 autorag-0.1.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.195387 autorag-0.1.8/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.199386 autorag-0.1.8/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    57124 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/data_creation.png
--rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/data_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_line_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    42589 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_line_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)    92939 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_lines.png
--rw-r--r--   0 runner    (1001) docker     (127)    95669 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/node_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/project_folder_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    19853 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/project_folders.png
--rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/resources_folder.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.203387 autorag-0.1.8/docs/source/_static/roadmap/
--rw-r--r--   0 runner    (1001) docker     (127)   159068 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/RAG_paradigms.png
--rw-r--r--   0 runner    (1001) docker     (127)    38568 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/advanced_RAG.png
--rw-r--r--   0 runner    (1001) docker     (127)    62853 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/cycle.png
--rw-r--r--   0 runner    (1001) docker     (127)    75826 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/merger.png
--rw-r--r--   0 runner    (1001) docker     (127)    82200 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/node_line_modular.png
--rw-r--r--   0 runner    (1001) docker     (127)    69999 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/roadmap/policy.png
--rw-r--r--   0 runner    (1001) docker     (127)   567356 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/samsung_sundae.jpeg
--rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/trial_folder.png
--rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/trial_json.png
--rw-r--r--   0 runner    (1001) docker     (127)   177107 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/trial_summary.png
--rw-r--r--   0 runner    (1001) docker     (127)   269046 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/_static/web_interface.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/api_spec/
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.data.corpus.rst
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.data.qacreation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.data.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.evaluate.metric.rst
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.evaluate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.generator.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagecompressor.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagefilter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagereranker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.promptmaker.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.queryexpansion.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.retrieval.rst
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.nodes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.rst
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/autorag.utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/api_spec/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/data_creation/
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/data_creation/data_format.md
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/data_creation/ragas.md
--rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/data_creation/tutorial.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/deploy/api_endpoint.md
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/deploy/web.md
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/install.md
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/local_model.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/generator/generator.md
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/generator/llama_index_llm.md
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/generator/vllm.md
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/nodes/passage_augmenter/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_augmenter/passage_augmenter.md
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.207387 autorag-0.1.8/docs/source/nodes/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_compressor/passage_compressor.md
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_compressor/refine.md
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_compressor/tree_summarize.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.211387 autorag-0.1.8/docs/source/nodes/passage_filter/
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_filter/passage_filter.md
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_filter/recency_filter.md
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.211387 autorag-0.1.8/docs/source/nodes/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/cohere.md
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/colbert.md
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/jina_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/koreranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/monot5.md
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/passage_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/rankgpt.md
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/tart.md
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/time_reranker.md
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/passage_reranker/upr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.211387 autorag-0.1.8/docs/source/nodes/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/prompt_maker/fstring.md
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/prompt_maker/long_context_reorder.md
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/prompt_maker/prompt_maker.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.211387 autorag-0.1.8/docs/source/nodes/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/query_expansion/hyde.md
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/query_expansion/query_decompose.md
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/query_expansion/query_expansion.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/docs/source/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/bm25.md
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/hybrid_cc.md
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/hybrid_dbsf.md
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/hybrid_rrf.md
--rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/hybrid_rsf.md
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/retrieval.md
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/nodes/retrieval/vectordb.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/docs/source/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/optimization/custom_config.md
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/optimization/folder_structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/optimization/optimization.md
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/optimization/sample_full_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/docs/source/roadmap/
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/roadmap/modular_rag.md
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/structure.md
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/troubleshooting.md
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-29 14:33:32.000000 autorag-0.1.8/docs/source/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-29 14:33:32.000000 autorag-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-29 14:33:32.000000 autorag-0.1.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/sample_config/
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/compact_local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/compact_openai.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/config_korean.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/extracted_sample.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/simple_local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_config/simple_openai.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/sample_dataset/
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_dataset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.215386 autorag-0.1.8/sample_dataset/eli5/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_dataset/eli5/load_eli5_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/sample_dataset/msmarco/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_dataset/msmarco/load_msmarco_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/sample_dataset/triviaqa/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-29 14:33:32.000000 autorag-0.1.8/sample_dataset/triviaqa/load_triviaqa_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 14:33:49.267387 autorag-0.1.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/autorag/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.163386 autorag-0.1.8/tests/autorag/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/autorag/data/corpus/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/corpus/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/corpus/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/corpus/test_llama_index_corpus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/autorag/data/qacreation/
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/qacreation/test_base_qacreation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/qacreation/test_llama_index_qacreation.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/qacreation/test_ragas_qa_creation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/data/qacreation/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.219387 autorag-0.1.8/tests/autorag/evaluate/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.223387 autorag-0.1.8/tests/autorag/evaluate/metric/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/metric/test_generation_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/metric/test_retrieval_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/test_evaluate_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/test_generation_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/evaluate/test_retrieval_evaluate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.167386 autorag-0.1.8/tests/autorag/nodes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.223387 autorag-0.1.8/tests/autorag/nodes/generator/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/generator/test_generator_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/generator/test_llama_index_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/generator/test_run_generator_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/generator/test_vllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.223387 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.223387 autorag-0.1.8/tests/autorag/nodes/passagecompressor/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_refine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.227387 autorag-0.1.8/tests/autorag/nodes/passagefilter/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_recency_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.227387 autorag-0.1.8/tests/autorag/nodes/passagereranker/
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_flag_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_jina_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_koreranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_monot5.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_pass_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_rankgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_tart.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_time_reranker.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/passagereranker/test_upr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.227387 autorag-0.1.8/tests/autorag/nodes/promptmaker/
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/promptmaker/test_fstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.231387 autorag-0.1.8/tests/autorag/nodes/queryexpansion/
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_hyde.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_decompose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.231387 autorag-0.1.8/tests/autorag/nodes/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_bm25.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_retrieval_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/nodes/retrieval/test_vectordb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.231387 autorag-0.1.8/tests/autorag/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/schema/test_module_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/schema/test_node_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_support.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/test_web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.231387 autorag-0.1.8/tests/autorag/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/utils/test_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/autorag/utils/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/corpus_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.167386 autorag-0.1.8/tests/resources/data_creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/data_creation/raw_dir/
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/data_creation/raw_dir/sample1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/data_creation/raw_dir/sample2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/data_creation/raw_dir/sample3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/full.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/qa_gen_prompts/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_gen_prompts/prompt1.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_gen_prompts/prompt2.txt
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_gen_prompts/prompt3.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/qa_test_data_sample.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/result_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/result_project/0/
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.235387 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/
--rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    26448 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    41557 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.239387 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/0/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/1/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.171387 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.243387 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.171387 autorag-0.1.8/tests/resources/result_project/2/post_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.247387 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
--rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
--rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
--rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/3/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/3/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/best.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/data/
--rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/data/corpus.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/data/qa.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   109454 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/bm25.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.251387 autorag-0.1.8/tests/resources/result_project/resources/chroma/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.263387 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
--rw-r--r--   0 runner    (1001) docker     (127)  6284000 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
--rw-r--r--   0 runner    (1001) docker     (127)   352256 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/resources/chroma/chroma.sqlite3
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/result_project/trial.json
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/sample_contents_nqa.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.171387 autorag-0.1.8/tests/resources/sample_project/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.263387 autorag-0.1.8/tests/resources/sample_project/data/
--rw-r--r--   0 runner    (1001) docker     (127)   115302 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/sample_project/data/corpus.parquet
--rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/sample_project/data/qa.parquet
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 14:33:49.263387 autorag-0.1.8/tests/resources/sample_project/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   109454 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/sample_project/resources/bm25.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/simple.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-04-29 14:33:32.000000 autorag-0.1.8/tests/resources/test_bm25_retrieval.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.746204 autorag-0.1.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-01 06:27:38.000000 autorag-0.1.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.746204 autorag-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-01 06:27:38.000000 autorag-0.1.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-01 06:27:38.000000 autorag-0.1.9/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-01 06:27:38.000000 autorag-0.1.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-01 06:27:38.000000 autorag-0.1.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/AutoRAG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19965 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-01 06:27:49.000000 autorag-0.1.9/AutoRAG.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-05-01 06:27:38.000000 autorag-0.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-01 06:27:38.000000 autorag-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 06:27:38.000000 autorag-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24187 2024-05-01 06:27:49.838204 autorag-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9161 2024-05-01 06:27:38.000000 autorag-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.750204 autorag-0.1.9/autorag/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.750204 autorag-0.1.9/autorag/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.750204 autorag-0.1.9/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/corpus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/corpus/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/corpus/llama_index.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.750204 autorag-0.1.9/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/llama_index_default_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/ragas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/qacreation/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/data/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/data/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8871 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/evaluate/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/metric/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/retrieval_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17379 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/node_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.754204 autorag-0.1.9/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/openai_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/generator/vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.758204 autorag-0.1.9/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4771 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passageaugmenter/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.758204 autorag-0.1.9/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagecompressor/tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.758204 autorag-0.1.9/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3922 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/recency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagefilter/threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.762204 autorag-0.1.9/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/colbert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/jina.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/sentence_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.762204 autorag-0.1.9/autorag/nodes/passagereranker/tart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/tart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/tart/modeling_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/tart/tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/passagereranker/upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.762204 autorag-0.1.9/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/promptmaker/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.762204 autorag-0.1.9/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7932 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/queryexpansion/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.766204 autorag-0.1.9/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/nodes/retrieval/vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.766204 autorag-0.1.9/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/schema/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/schema/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/support.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.766204 autorag-0.1.9/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4020 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12777 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-01 06:27:38.000000 autorag-0.1.9/autorag/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 06:27:38.000000 autorag-0.1.9/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.766204 autorag-0.1.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.770204 autorag-0.1.9/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.774204 autorag-0.1.9/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    57124 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/data_creation.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30770 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/data_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31538 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18941 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_line_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42589 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_line_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    92939 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_lines.png
+-rw-r--r--   0 runner    (1001) docker     (127)    95669 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/node_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36728 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/project_folder_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19853 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/project_folders.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22432 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/resources_folder.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.774204 autorag-0.1.9/docs/source/_static/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)   159068 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/RAG_paradigms.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38568 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/advanced_RAG.png
+-rw-r--r--   0 runner    (1001) docker     (127)    62853 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/cycle.png
+-rw-r--r--   0 runner    (1001) docker     (127)    75826 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/merger.png
+-rw-r--r--   0 runner    (1001) docker     (127)    82200 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/node_line_modular.png
+-rw-r--r--   0 runner    (1001) docker     (127)    69999 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/roadmap/policy.png
+-rw-r--r--   0 runner    (1001) docker     (127)   567356 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/samsung_sundae.jpeg
+-rw-r--r--   0 runner    (1001) docker     (127)    37348 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/trial_folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25499 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/trial_json.png
+-rw-r--r--   0 runner    (1001) docker     (127)   177107 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/trial_summary.png
+-rw-r--r--   0 runner    (1001) docker     (127)   269046 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/_static/web_interface.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.778204 autorag-0.1.9/docs/source/api_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.data.corpus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.data.qacreation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.data.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.evaluate.metric.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.evaluate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.generator.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passageaugmenter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagecompressor.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagefilter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagereranker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.promptmaker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.queryexpansion.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.retrieval.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.nodes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/autorag.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/api_spec/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.778204 autorag-0.1.9/docs/source/data_creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/data_creation/data_format.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/data_creation/ragas.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5543 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/data_creation/tutorial.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/deploy/api_endpoint.md
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/deploy/web.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/local_model.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/generator/generator.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/generator/llama_index_llm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/generator/openai_llm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/generator/vllm.md
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/passage_augmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_augmenter/passage_augmenter.md
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_augmenter/prev_next_augmenter.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     3046 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_compressor/passage_compressor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_compressor/refine.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_compressor/tree_summarize.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.782204 autorag-0.1.9/docs/source/nodes/passage_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_filter/passage_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_filter/recency_filter.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/nodes/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/cohere.md
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/colbert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/flag_embedding_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/jina_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/koreranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/monot5.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/passage_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/rankgpt.md
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/tart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/time_reranker.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/passage_reranker/upr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/nodes/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/prompt_maker/fstring.md
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/prompt_maker/long_context_reorder.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/prompt_maker/prompt_maker.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/nodes/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/query_expansion/hyde.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/query_expansion/query_decompose.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/query_expansion/query_expansion.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/bm25.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/hybrid_cc.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/hybrid_dbsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/hybrid_rrf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2304 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/hybrid_rsf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/retrieval.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/nodes/retrieval/vectordb.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/optimization/custom_config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/optimization/folder_structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/optimization/optimization.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/optimization/sample_full_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.786204 autorag-0.1.9/docs/source/roadmap/
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/roadmap/modular_rag.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/structure.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/troubleshooting.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-05-01 06:27:38.000000 autorag-0.1.9/docs/source/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-05-01 06:27:38.000000 autorag-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-01 06:27:38.000000 autorag-0.1.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/compact_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/compact_openai.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/config_korean.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/extracted_sample.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/simple_local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_config/simple_openai.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_dataset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_dataset/eli5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_dataset/eli5/load_eli5_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_dataset/msmarco/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_dataset/msmarco/load_msmarco_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/sample_dataset/triviaqa/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-01 06:27:38.000000 autorag-0.1.9/sample_dataset/triviaqa/load_triviaqa_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 06:27:49.838204 autorag-0.1.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/tests/autorag/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.738204 autorag-0.1.9/tests/autorag/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.790204 autorag-0.1.9/tests/autorag/data/corpus/
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/corpus/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/corpus/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/corpus/test_llama_index_corpus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/data/qacreation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/qacreation/test_base_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/qacreation/test_llama_index_qacreation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/qacreation/test_ragas_qa_creation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/data/qacreation/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/evaluate/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/evaluate/metric/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/metric/test_generation_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/metric/test_retrieval_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/test_evaluate_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/test_generation_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/test_retrieval_contents_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/evaluate/test_retrieval_evaluate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.742204 autorag-0.1.9/tests/autorag/nodes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/nodes/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_generator_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_llama_index_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_run_generator_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/generator/test_vllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.794204 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.798204 autorag-0.1.9/tests/autorag/nodes/passagecompressor/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_pass_compressor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_refine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_tree_summarize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.798204 autorag-0.1.9/tests/autorag/nodes/passagefilter/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_passage_filter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_passage_filter_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_recency_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/nodes/passagereranker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_cohere_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_colbert_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_flag_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_jina_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_koreranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_monot5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_pass_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_rankgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_tart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_time_reranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/passagereranker/test_upr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/nodes/promptmaker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/promptmaker/test_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/promptmaker/test_long_context_reorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8310 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/nodes/queryexpansion/
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_hyde.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6880 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/nodes/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_bm25.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_rrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_rsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_retrieval_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_run_retrieval_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/nodes/retrieval/test_vectordb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.802204 autorag-0.1.9/tests/autorag/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/schema/test_module_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/schema/test_node_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/autorag/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/utils/test_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/autorag/utils/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/corpus_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.742204 autorag-0.1.9/tests/resources/data_creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/data_creation/raw_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/data_creation/raw_dir/sample1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/data_creation/raw_dir/sample2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/data_creation/raw_dir/sample3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/full.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/qa_gen_prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_gen_prompts/prompt1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_gen_prompts/prompt2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_gen_prompts/prompt3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5910 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/qa_test_data_sample.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/result_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.806204 autorag-0.1.9/tests/resources/result_project/0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)    23516 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    26448 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    33716 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14618 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    54234 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    41557 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.810204 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/0/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.814204 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.742204 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.746204 autorag-0.1.9/tests/resources/result_project/2/post_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.818204 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    28924 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    14607 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/
+-rw-r--r--   0 runner    (1001) docker     (127)     9073 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    31124 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/
+-rw-r--r--   0 runner    (1001) docker     (127)    67610 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    67719 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    84239 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.822204 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)   103655 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)    86579 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)   117633 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/summary.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.826204 autorag-0.1.9/tests/resources/result_project/3/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/3/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/best.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.826204 autorag-0.1.9/tests/resources/result_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   111931 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.826204 autorag-0.1.9/tests/resources/result_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   109454 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/bm25.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.826204 autorag-0.1.9/tests/resources/result_project/resources/chroma/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/
+-rw-r--r--   0 runner    (1001) docker     (127)  6284000 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/header.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/link_lists.bin
+-rw-r--r--   0 runner    (1001) docker     (127)   352256 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/resources/chroma/chroma.sqlite3
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/result_project/trial.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/sample_contents_nqa.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.746204 autorag-0.1.9/tests/resources/sample_project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/tests/resources/sample_project/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   115302 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/sample_project/data/corpus.parquet
+-rw-r--r--   0 runner    (1001) docker     (127)     9928 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/sample_project/data/qa.parquet
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 06:27:49.838204 autorag-0.1.9/tests/resources/sample_project/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   109454 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/sample_project/resources/bm25.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/simple.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-05-01 06:27:38.000000 autorag-0.1.9/tests/resources/test_bm25_retrieval.pkl
```

### Comparing `autorag-0.1.8/.github/workflows/publish.yml` & `autorag-0.1.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/.github/workflows/sphinx.yml` & `autorag-0.1.9/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/.github/workflows/test.yml` & `autorag-0.1.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/.gitignore` & `autorag-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/AutoRAG.egg-info/PKG-INFO` & `autorag-0.1.9/AutoRAG.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.8
+Version: 0.1.9
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `autorag-0.1.8/AutoRAG.egg-info/SOURCES.txt` & `autorag-0.1.9/AutoRAG.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 autorag/evaluate/metric/g_eval_prompts/con_detailed.txt
 autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt
 autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt
 autorag/nodes/__init__.py
 autorag/nodes/generator/__init__.py
 autorag/nodes/generator/base.py
 autorag/nodes/generator/llama_index_llm.py
+autorag/nodes/generator/openai_llm.py
 autorag/nodes/generator/run.py
 autorag/nodes/generator/vllm.py
 autorag/nodes/passageaugmenter/__init__.py
 autorag/nodes/passageaugmenter/base.py
 autorag/nodes/passageaugmenter/pass_passage_augmenter.py
 autorag/nodes/passageaugmenter/prev_next_augmenter.py
 autorag/nodes/passageaugmenter/run.py
@@ -175,14 +176,15 @@
 docs/source/data_creation/ragas.md
 docs/source/data_creation/tutorial.md
 docs/source/deploy/api_endpoint.md
 docs/source/deploy/web.md
 docs/source/nodes/index.md
 docs/source/nodes/generator/generator.md
 docs/source/nodes/generator/llama_index_llm.md
+docs/source/nodes/generator/openai_llm.md
 docs/source/nodes/generator/vllm.md
 docs/source/nodes/passage_augmenter/passage_augmenter.md
 docs/source/nodes/passage_augmenter/prev_next_augmenter.md
 docs/source/nodes/passage_compressor/passage_compressor.md
 docs/source/nodes/passage_compressor/refine.md
 docs/source/nodes/passage_compressor/tree_summarize.md
 docs/source/nodes/passage_filter/passage_filter.md
@@ -252,14 +254,15 @@
 tests/autorag/evaluate/test_retrieval_contents_evaluate.py
 tests/autorag/evaluate/test_retrieval_evaluate.py
 tests/autorag/evaluate/metric/test_generation_metric.py
 tests/autorag/evaluate/metric/test_retrieval_contents_metric.py
 tests/autorag/evaluate/metric/test_retrieval_metric.py
 tests/autorag/nodes/generator/test_generator_base.py
 tests/autorag/nodes/generator/test_llama_index_llm.py
+tests/autorag/nodes/generator/test_openai.py
 tests/autorag/nodes/generator/test_run_generator_node.py
 tests/autorag/nodes/generator/test_vllm.py
 tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py
 tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py
 tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py
 tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py
 tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py
```

### Comparing `autorag-0.1.8/AutoRAG.egg-info/requires.txt` & `autorag-0.1.9/AutoRAG.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/CODE_OF_CONDUCT.md` & `autorag-0.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/CONTRIBUTING.md` & `autorag-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/LICENSE` & `autorag-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/PKG-INFO` & `autorag-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoRAG
-Version: 0.1.8
+Version: 0.1.9
 Summary: Automatically Evaluate RAG pipelines with your own data. Find optimal structure for new RAG product.
 Author-email: Marker-Inc <vkehfdl1@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `autorag-0.1.8/README.md` & `autorag-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/__init__.py` & `autorag-0.1.9/autorag/__init__.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/cli.py` & `autorag-0.1.9/autorag/cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/data/corpus/langchain.py` & `autorag-0.1.9/autorag/data/corpus/langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/data/corpus/llama_index.py` & `autorag-0.1.9/autorag/data/corpus/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/data/qacreation/base.py` & `autorag-0.1.9/autorag/data/qacreation/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/data/qacreation/llama_index.py` & `autorag-0.1.9/autorag/data/qacreation/llama_index.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/data/qacreation/llama_index_default_prompt.txt` & `autorag-0.1.9/autorag/data/qacreation/llama_index_default_prompt.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/data/qacreation/ragas.py` & `autorag-0.1.9/autorag/data/qacreation/ragas.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/data/qacreation/simple.py` & `autorag-0.1.9/autorag/data/qacreation/simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/data/utils/util.py` & `autorag-0.1.9/autorag/data/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/deploy.py` & `autorag-0.1.9/autorag/deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/evaluate/generation.py` & `autorag-0.1.9/autorag/evaluate/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt` & `autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/coh_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt` & `autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/con_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt` & `autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/flu_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt` & `autorag-0.1.9/autorag/evaluate/metric/g_eval_prompts/rel_detailed.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/evaluate/metric/generation.py` & `autorag-0.1.9/autorag/evaluate/metric/generation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/evaluate/metric/retrieval.py` & `autorag-0.1.9/autorag/evaluate/retrieval.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,52 +1,55 @@
 import functools
-from typing import List
+import warnings
+from typing import List, Callable, Any, Tuple
 
+import pandas as pd
 
-def retrieval_metric(func):
-    @functools.wraps(func)
-    def wrapper(retrieval_gt: List[List[List[str]]], pred_ids: List[List[str]]) -> List[float]:
-        results = []
-        for gt, pred in zip(retrieval_gt, pred_ids):
-            if gt == [[]] or any(bool(g_) is False for g in gt for g_ in g):
-                results.append(None)
-            else:
-                results.append(func(gt, pred))
-        return results
-
-    return wrapper
-
-
-@retrieval_metric
-def retrieval_f1(gt: List[List[str]], pred: List[str]):
-    """
-    Compute f1 score for retrieval.
-
-    :param gt: 2-d list of ground truth ids.
-        It contains and/or connections between ids.
-    :param pred: Prediction ids.
-    :return: The f1 score.
-    """
-    recall_score = retrieval_recall.__wrapped__(gt, pred)
-    precision_score = retrieval_precision.__wrapped__(gt, pred)
-    if recall_score + precision_score == 0:
-        return 0
-    else:
-        return 2 * (recall_score * precision_score) / (recall_score + precision_score)
-
-
-@retrieval_metric
-def retrieval_recall(gt: List[List[str]], pred: List[str]):
-    gt_sets = [frozenset(g) for g in gt]
-    pred_set = set(pred)
-    hits = sum(any(pred_id in gt_set for pred_id in pred_set) for gt_set in gt_sets)
-    recall = hits / len(gt) if len(gt) > 0 else 0.0
-    return recall
-
-
-@retrieval_metric
-def retrieval_precision(gt: List[List[str]], pred: List[str]):
-    gt_sets = [frozenset(g) for g in gt]
-    pred_set = set(pred)
-    hits = sum(any(pred_id in gt_set for gt_set in gt_sets) for pred_id in pred_set)
-    precision = hits / len(pred) if len(pred) > 0 else 0.0
-    return precision
+from autorag.evaluate.metric import (retrieval_recall, retrieval_precision, retrieval_f1, retrieval_ndcg, retrieval_mrr,
+                                     retrieval_map)
+
+
+def evaluate_retrieval(retrieval_gt: List[List[List[str]]], metrics: List[str]):
+    def decorator_evaluate_retrieval(
+            func: Callable[[Any], Tuple[List[List[str]], List[List[str]], List[List[float]]]]):
+        """
+        Decorator for evaluating retrieval results.
+        You can use this decorator to any method that returns (contents, scores, ids),
+        which is the output of conventional retrieval modules.
+
+        :param func: Must return (contents, scores, ids)
+        :return: wrapper function that returns pd.DataFrame, which is the evaluation result.
+        """
+
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs) -> pd.DataFrame:
+            contents, pred_ids, scores = func(*args, **kwargs)
+            metric_funcs = {
+                retrieval_recall.__name__: retrieval_recall,
+                retrieval_precision.__name__: retrieval_precision,
+                retrieval_f1.__name__: retrieval_f1,
+                retrieval_ndcg.__name__: retrieval_ndcg,
+                retrieval_mrr.__name__: retrieval_mrr,
+                retrieval_map.__name__: retrieval_map,
+            }
+
+            metric_scores = {}
+            for metric in metrics:
+                if metric not in metric_funcs:
+                    warnings.warn(f"metric {metric} is not in supported metrics: {metric_funcs.keys()}"
+                                  f"{metric} will be ignored.")
+                else:
+                    metric_func = metric_funcs[metric]
+                    metric_scores[metric] = metric_func(retrieval_gt=retrieval_gt, pred_ids=pred_ids)
+
+            metric_result_df = pd.DataFrame(metric_scores)
+            execution_result_df = pd.DataFrame({
+                'retrieved_contents': contents,
+                'retrieved_ids': pred_ids,
+                'retrieve_scores': scores,
+            })
+            result_df = pd.concat([execution_result_df, metric_result_df], axis=1)
+            return result_df
+
+        return wrapper
+
+    return decorator_evaluate_retrieval
```

### Comparing `autorag-0.1.8/autorag/evaluate/metric/retrieval_contents.py` & `autorag-0.1.9/autorag/evaluate/metric/retrieval_contents.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/evaluate/retrieval.py` & `autorag-0.1.9/autorag/evaluate/retrieval_contents.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 import functools
-import warnings
 from typing import List, Callable, Any, Tuple
 
 import pandas as pd
 
-from autorag.evaluate.metric import retrieval_recall, retrieval_precision, retrieval_f1
+from autorag.evaluate.metric import retrieval_token_f1, retrieval_token_precision, retrieval_token_recall
 
 
-def evaluate_retrieval(retrieval_gt: List[List[List[str]]], metrics: List[str]):
-    def decorator_evaluate_retrieval(
+def evaluate_retrieval_contents(retrieval_gt: List[List[str]], metrics: List[str]):
+    def decorator_evaluate_retireval_contents(
             func: Callable[[Any], Tuple[List[List[str]], List[List[str]], List[List[float]]]]):
         """
-        Decorator for evaluating retrieval results.
+        Decorator for evaluating retrieval contents.
         You can use this decorator to any method that returns (contents, scores, ids),
         which is the output of conventional retrieval modules.
 
         :param func: Must return (contents, scores, ids)
-        :return: wrapper function that returns pd.DataFrame, which is the evaluation result.
+        :return: pd.DataFrame, which is the evaluation result and function result.
         """
 
         @functools.wraps(func)
         def wrapper(*args, **kwargs) -> pd.DataFrame:
             contents, pred_ids, scores = func(*args, **kwargs)
             metric_funcs = {
-                retrieval_recall.__name__: retrieval_recall,
-                retrieval_precision.__name__: retrieval_precision,
-                retrieval_f1.__name__: retrieval_f1,
+                retrieval_token_recall.__name__: retrieval_token_recall,
+                retrieval_token_precision.__name__: retrieval_token_precision,
+                retrieval_token_f1.__name__: retrieval_token_f1,
             }
 
-            metric_scores = {}
+            metrics_scores = {}
             for metric in metrics:
                 if metric not in metric_funcs:
-                    warnings.warn(f"metric {metric} is not in supported metrics: {metric_funcs.keys()}"
-                                  f"{metric} will be ignored.")
+                    raise ValueError(f"metric {metric} is not in supported metrics: {metric_funcs.keys()}")
                 else:
                     metric_func = metric_funcs[metric]
-                    metric_scores[metric] = metric_func(retrieval_gt=retrieval_gt, pred_ids=pred_ids)
+                    metric_scores = metric_func(gt_contents=retrieval_gt, pred_contents=contents)
+                    metrics_scores[metric] = metric_scores
 
-            metric_result_df = pd.DataFrame(metric_scores)
+            metric_result_df = pd.DataFrame(metrics_scores)
             execution_result_df = pd.DataFrame({
                 'retrieved_contents': contents,
                 'retrieved_ids': pred_ids,
                 'retrieve_scores': scores,
             })
             result_df = pd.concat([execution_result_df, metric_result_df], axis=1)
             return result_df
 
         return wrapper
 
-    return decorator_evaluate_retrieval
+    return decorator_evaluate_retireval_contents
```

### Comparing `autorag-0.1.8/autorag/evaluate/util.py` & `autorag-0.1.9/autorag/evaluate/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/evaluator.py` & `autorag-0.1.9/autorag/evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/node_line.py` & `autorag-0.1.9/autorag/node_line.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/generator/base.py` & `autorag-0.1.9/autorag/nodes/generator/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,14 +39,11 @@
                 raise ValueError(f"{llm} is not a valid llm name. Please check the llm name."
                                  "You can check valid llm names from autorag.generator_models.")
             batch = kwargs.pop('batch', 16)
             llm_instance = generator_models[llm](**kwargs)
             result = func(prompts=prompts, llm=llm_instance, batch=batch)
             del llm_instance
             return result
-        elif func.__name__ == 'vllm':
-            return func(prompts=prompts, llm=llm, **kwargs)
         else:
-            raise ValueError(f"{func.__name__} is not a valid generator node name. "
-                             "Please check the generator node name.")
+            return func(prompts=prompts, llm=llm, **kwargs)
 
     return wrapper
```

### Comparing `autorag-0.1.8/autorag/nodes/generator/llama_index_llm.py` & `autorag-0.1.9/autorag/nodes/generator/llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/generator/run.py` & `autorag-0.1.9/autorag/nodes/generator/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/generator/vllm.py` & `autorag-0.1.9/autorag/nodes/generator/vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passageaugmenter/base.py` & `autorag-0.1.9/autorag/nodes/passageaugmenter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passageaugmenter/prev_next_augmenter.py` & `autorag-0.1.9/autorag/nodes/passageaugmenter/prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passageaugmenter/run.py` & `autorag-0.1.9/autorag/nodes/passageaugmenter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagecompressor/base.py` & `autorag-0.1.9/autorag/nodes/passagecompressor/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagecompressor/refine.py` & `autorag-0.1.9/autorag/nodes/passagecompressor/refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagecompressor/run.py` & `autorag-0.1.9/autorag/nodes/passagecompressor/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagecompressor/tree_summarize.py` & `autorag-0.1.9/autorag/nodes/passagecompressor/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagefilter/base.py` & `autorag-0.1.9/autorag/nodes/passagefilter/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagefilter/percentile_cutoff.py` & `autorag-0.1.9/autorag/nodes/passagefilter/percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagefilter/recency.py` & `autorag-0.1.9/autorag/nodes/passagefilter/recency.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagefilter/run.py` & `autorag-0.1.9/autorag/nodes/passagefilter/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagefilter/threshold_cutoff.py` & `autorag-0.1.9/autorag/nodes/passagefilter/threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/base.py` & `autorag-0.1.9/autorag/nodes/passagereranker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/cohere.py` & `autorag-0.1.9/autorag/nodes/passagereranker/cohere.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/colbert.py` & `autorag-0.1.9/autorag/nodes/passagereranker/colbert.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/flag_embedding.py` & `autorag-0.1.9/autorag/nodes/passagereranker/flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/flag_embedding_llm.py` & `autorag-0.1.9/autorag/nodes/passagereranker/flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/jina.py` & `autorag-0.1.9/autorag/nodes/passagereranker/jina.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/koreranker.py` & `autorag-0.1.9/autorag/nodes/passagereranker/tart/tart.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,79 @@
-import asyncio
+from itertools import chain
 from typing import List, Tuple
 
-import numpy as np
+import pandas as pd
 import torch
-from transformers import AutoModelForSequenceClassification, AutoTokenizer
+import torch.nn.functional as F
+from tqdm import tqdm
 
 from autorag.nodes.passagereranker.base import passage_reranker_node
+from autorag.nodes.passagereranker.tart.modeling_enc_t5 import EncT5ForSequenceClassification
+from autorag.nodes.passagereranker.tart.tokenization_enc_t5 import EncT5Tokenizer
+from autorag.utils.util import make_batch, sort_by_scores, flatten_apply, select_top_k
 
 
 @passage_reranker_node
-def koreranker(queries: List[str], contents_list: List[List[str]],
-               scores_list: List[List[float]], ids_list: List[List[str]],
-               top_k: int) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
+def tart(queries: List[str], contents_list: List[List[str]],
+         scores_list: List[List[float]], ids_list: List[List[str]],
+         top_k: int, instruction: str = "Find passage to answer given question",
+         batch: int = 64) -> Tuple[List[List[str]], List[List[str]], List[List[float]]]:
     """
-    Rerank a list of contents based on their relevance to a query using ko-reranker.
-    ko-reranker is a reranker based on korean (https://huggingface.co/Dongjin-kr/ko-reranker).
+    Rerank a list of contents based on their relevance to a query using Tart.
+    TART is a reranker based on TART (https://github.com/facebookresearch/tart).
+    You can rerank the passages with the instruction using TARTReranker.
+    The default model is facebook/tart-full-flan-t5-xl.
 
     :param queries: The list of queries to use for reranking
     :param contents_list: The list of lists of contents to rerank
     :param scores_list: The list of lists of scores retrieved from the initial ranking
     :param ids_list: The list of lists of ids retrieved from the initial ranking
     :param top_k: The number of passages to be retrieved
+    :param instruction: The instruction for reranking.
+        Note: default instruction is "Find passage to answer given question"
+            The default instruction from the TART paper is being used.
+            If you want to use a different instruction, you can change the instruction through this parameter
+    :param batch: The number of queries to be processed in a batch
     :return: tuple of lists containing the reranked contents, ids, and scores
     """
-    model_path = "Dongjin-kr/ko-reranker"
-    tokenizer = AutoTokenizer.from_pretrained(model_path)
-    model = AutoModelForSequenceClassification.from_pretrained(model_path)
-    model.eval()
-
-    # Determine the device to run the model on (GPU if available, otherwise CPU)
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    model.to(device)
-    # Run async ko_rerank_pure function
-    tasks = [koreranker_pure(query, contents, scores, ids, top_k, model, tokenizer, device)
-             for query, contents, scores, ids in zip(queries, contents_list, scores_list, ids_list)]
-    loop = asyncio.get_event_loop()
-    results = loop.run_until_complete(asyncio.gather(*tasks))
-    content_result = list(map(lambda x: x[0], results))
-    id_result = list(map(lambda x: x[1], results))
-    score_result = list(map(lambda x: x[2], results))
+    model_name = "facebook/tart-full-flan-t5-xl"
+    model = EncT5ForSequenceClassification.from_pretrained(model_name)
+    tokenizer = EncT5Tokenizer.from_pretrained(model_name)
+    device = "cuda" if torch.cuda.is_available() else "cpu"
+    model = model.to(device)
+
+    nested_list = [[['{} [SEP] {}'.format(instruction, query)] for _ in contents] for query, contents in
+                   zip(queries, contents_list)]
+
+    rerank_scores = flatten_apply(tart_run_model, nested_list, model=model, batch_size=batch,
+                                  tokenizer=tokenizer, device=device, contents_list=contents_list)
+
+    df = pd.DataFrame({
+        'contents': contents_list,
+        'ids': ids_list,
+        'scores': rerank_scores,
+    })
+    df[['contents', 'ids', 'scores']] = df.apply(sort_by_scores, axis=1, result_type='expand')
+    results = select_top_k(df, ['contents', 'ids', 'scores'], top_k)
 
     del model
     del tokenizer
     if torch.cuda.is_available():
         torch.cuda.empty_cache()
 
-    return content_result, id_result, score_result
+    return results['contents'].tolist(), results['ids'].tolist(), results['scores'].tolist()
 
 
-async def koreranker_pure(query: str, contents: List[str],
-                          scores: List[float], ids: List[str],
-                          top_k: int, model, tokenizer, device) \
-        -> Tuple[List[str], List[str], List[float]]:
-    """
-    Rerank a list of contents based on their relevance to a query using ko-reranker.
-
-    :param query: The query to use for reranking
-    :param contents: The list of contents to rerank
-    :param scores: The list of scores retrieved from the initial ranking
-    :param ids: The list of ids retrieved from the initial ranking
-    :param top_k: The number of passages to be retrieved
-    :param model: The ko-reranker model to use for reranking
-    :param tokenizer: The tokenizer to use for the model
-    :param device: The device to run the model on (GPU if available, otherwise CPU)
-    :return: tuple of lists containing the reranked contents, ids, and scores
-    """
-    input_pairs = [[query, content] for content in contents]
-    inputs = tokenizer(input_pairs, padding=True, truncation=True, return_tensors='pt', max_length=512)
-    inputs = inputs.to(device)
-
-    with torch.no_grad():
-        scores = model(**inputs, return_dict=True).logits.view(-1, ).float()
-        scores_np = scores.cpu().numpy()
-        scores = exp_normalize(scores_np)
-
-    # Convert scores type to float
-    scores = scores.astype(float)
-
-    # Create a list of tuples pairing each content with its relevance score
-    content_ids_scores = list(zip(contents, ids, scores))
-
-    # Sort the list of pairs based on the relevance score in descending order
-    sorted_content_ids_scores = sorted(content_ids_scores, key=lambda x: x[2], reverse=True)
-
-    # crop with top_k
-    if len(contents) < top_k:
-        top_k = len(contents)
-    sorted_content_ids_scores = sorted_content_ids_scores[:top_k]
-
-    content_result, id_result, score_result = zip(*sorted_content_ids_scores)
-
-    return list(content_result), list(id_result), list(score_result)
-
-
-def exp_normalize(x):
-    b = x.max()
-    y = np.exp(x - b)
-    return y / y.sum()
+def tart_run_model(input_texts, contents_list, model, batch_size: int, tokenizer, device):
+    flattened_texts = list(chain.from_iterable(input_texts))
+    flattened_contents = list(chain.from_iterable(contents_list))
+    batch_input_texts = make_batch(flattened_texts, batch_size)
+    batch_contents_list = make_batch(flattened_contents, batch_size)
+    results = []
+    for batch_texts, batch_contents in tqdm(zip(batch_input_texts, batch_contents_list)):
+        feature = tokenizer(batch_texts, batch_contents, padding=True, truncation=True,
+                            return_tensors="pt").to(device)
+        with torch.no_grad():
+            pred_scores = model(**feature).logits
+            normalized_scores = [float(score[1]) for score in F.softmax(pred_scores, dim=1)]
+        results.extend(normalized_scores)
+    return results
```

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/monot5.py` & `autorag-0.1.9/autorag/nodes/passagereranker/monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/pass_reranker.py` & `autorag-0.1.9/autorag/nodes/passagereranker/pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/rankgpt.py` & `autorag-0.1.9/autorag/nodes/passagereranker/rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/run.py` & `autorag-0.1.9/autorag/nodes/passagereranker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/sentence_transformer.py` & `autorag-0.1.9/autorag/nodes/passagereranker/sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/tart/modeling_enc_t5.py` & `autorag-0.1.9/autorag/nodes/passagereranker/tart/modeling_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py` & `autorag-0.1.9/autorag/nodes/passagereranker/tart/tokenization_enc_t5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/time_reranker.py` & `autorag-0.1.9/autorag/nodes/passagereranker/time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/passagereranker/upr.py` & `autorag-0.1.9/autorag/nodes/passagereranker/upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/promptmaker/base.py` & `autorag-0.1.9/autorag/nodes/promptmaker/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/promptmaker/fstring.py` & `autorag-0.1.9/autorag/nodes/promptmaker/fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/promptmaker/long_context_reorder.py` & `autorag-0.1.9/autorag/nodes/promptmaker/long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/promptmaker/run.py` & `autorag-0.1.9/autorag/nodes/promptmaker/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/queryexpansion/base.py` & `autorag-0.1.9/autorag/nodes/queryexpansion/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/queryexpansion/hyde.py` & `autorag-0.1.9/autorag/nodes/queryexpansion/hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/queryexpansion/query_decompose.py` & `autorag-0.1.9/autorag/nodes/queryexpansion/query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/queryexpansion/run.py` & `autorag-0.1.9/autorag/nodes/queryexpansion/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/retrieval/base.py` & `autorag-0.1.9/autorag/nodes/retrieval/base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/retrieval/bm25.py` & `autorag-0.1.9/autorag/nodes/retrieval/bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/retrieval/hybrid_cc.py` & `autorag-0.1.9/autorag/nodes/retrieval/hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/retrieval/hybrid_dbsf.py` & `autorag-0.1.9/autorag/nodes/retrieval/hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/retrieval/hybrid_rrf.py` & `autorag-0.1.9/autorag/nodes/retrieval/hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/retrieval/hybrid_rsf.py` & `autorag-0.1.9/autorag/nodes/retrieval/hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/retrieval/run.py` & `autorag-0.1.9/autorag/nodes/retrieval/run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/nodes/retrieval/vectordb.py` & `autorag-0.1.9/autorag/nodes/retrieval/vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/schema/module.py` & `autorag-0.1.9/autorag/schema/module.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/schema/node.py` & `autorag-0.1.9/autorag/schema/node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/strategy.py` & `autorag-0.1.9/autorag/strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/support.py` & `autorag-0.1.9/autorag/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
         'refine': ('autorag.nodes.passagecompressor', 'refine'),
         # prompt_maker
         'fstring': ('autorag.nodes.promptmaker', 'fstring'),
         'long_context_reorder': ('autorag.nodes.promptmaker', 'long_context_reorder'),
         # generator
         'llama_index_llm': ('autorag.nodes.generator', 'llama_index_llm'),
         'vllm': ('autorag.nodes.generator', 'vllm'),
+        'openai_llm': ('autorag.nodes.generator', 'openai_llm'),
     }
     return dynamically_find_function(module_name, support_modules)
 
 
 def get_support_nodes(node_name: str) -> Callable:
     support_nodes = {
         'query_expansion': ('autorag.nodes.queryexpansion.run', 'run_query_expansion_node'),
```

### Comparing `autorag-0.1.8/autorag/utils/preprocess.py` & `autorag-0.1.9/autorag/utils/preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/utils/util.py` & `autorag-0.1.9/autorag/utils/util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/autorag/web.py` & `autorag-0.1.9/autorag/web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/Makefile` & `autorag-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/make.bat` & `autorag-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/data_creation.png` & `autorag-0.1.9/docs/source/_static/data_creation.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/data_folder.png` & `autorag-0.1.9/docs/source/_static/data_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/node_folder.png` & `autorag-0.1.9/docs/source/_static/node_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/node_line_folder.png` & `autorag-0.1.9/docs/source/_static/node_line_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/node_line_summary.png` & `autorag-0.1.9/docs/source/_static/node_line_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/node_lines.png` & `autorag-0.1.9/docs/source/_static/node_lines.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/node_summary.png` & `autorag-0.1.9/docs/source/_static/node_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/project_folder_example.png` & `autorag-0.1.9/docs/source/_static/project_folder_example.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/project_folders.png` & `autorag-0.1.9/docs/source/_static/project_folders.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/resources_folder.png` & `autorag-0.1.9/docs/source/_static/resources_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/roadmap/RAG_paradigms.png` & `autorag-0.1.9/docs/source/_static/roadmap/RAG_paradigms.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/roadmap/advanced_RAG.png` & `autorag-0.1.9/docs/source/_static/roadmap/advanced_RAG.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/roadmap/cycle.png` & `autorag-0.1.9/docs/source/_static/roadmap/cycle.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/roadmap/merger.png` & `autorag-0.1.9/docs/source/_static/roadmap/merger.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/roadmap/node_line_modular.png` & `autorag-0.1.9/docs/source/_static/roadmap/node_line_modular.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/roadmap/policy.png` & `autorag-0.1.9/docs/source/_static/roadmap/policy.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/samsung_sundae.jpeg` & `autorag-0.1.9/docs/source/_static/samsung_sundae.jpeg`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/trial_folder.png` & `autorag-0.1.9/docs/source/_static/trial_folder.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/trial_json.png` & `autorag-0.1.9/docs/source/_static/trial_json.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/trial_summary.png` & `autorag-0.1.9/docs/source/_static/trial_summary.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/_static/web_interface.png` & `autorag-0.1.9/docs/source/_static/web_interface.png`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.data.corpus.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.data.corpus.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.data.qacreation.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.data.qacreation.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.evaluate.metric.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.evaluate.metric.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.evaluate.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.evaluate.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.nodes.generator.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.nodes.generator.rst`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,22 @@
 ------------------------------------------------
 
 .. automodule:: autorag.nodes.generator.llama_index_llm
    :members:
    :undoc-members:
    :show-inheritance:
 
+autorag.nodes.generator.openai\_llm module
+------------------------------------------
+
+.. automodule:: autorag.nodes.generator.openai_llm
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 autorag.nodes.generator.run module
 ----------------------------------
 
 .. automodule:: autorag.nodes.generator.run
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passageaugmenter.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.nodes.passageaugmenter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagecompressor.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagecompressor.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagefilter.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagefilter.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagereranker.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagereranker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.nodes.passagereranker.tart.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.nodes.promptmaker.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.nodes.promptmaker.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.nodes.queryexpansion.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.nodes.queryexpansion.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.nodes.retrieval.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.nodes.retrieval.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/api_spec/autorag.rst` & `autorag-0.1.9/docs/source/api_spec/autorag.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/conf.py` & `autorag-0.1.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/data_creation/data_format.md` & `autorag-0.1.9/docs/source/data_creation/data_format.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/data_creation/ragas.md` & `autorag-0.1.9/docs/source/data_creation/ragas.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/data_creation/tutorial.md` & `autorag-0.1.9/docs/source/data_creation/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/deploy/api_endpoint.md` & `autorag-0.1.9/docs/source/deploy/api_endpoint.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/deploy/web.md` & `autorag-0.1.9/docs/source/deploy/web.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/index.rst` & `autorag-0.1.9/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/install.md` & `autorag-0.1.9/docs/source/install.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/local_model.md` & `autorag-0.1.9/docs/source/local_model.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/generator/generator.md` & `autorag-0.1.9/docs/source/nodes/generator/generator.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,8 +71,9 @@
 
 ```{toctree}
 ---
 maxdepth: 1
 ---
 llama_index_llm.md
 vllm.md
+openai_llm.md
 ```
```

### Comparing `autorag-0.1.8/docs/source/nodes/generator/llama_index_llm.md` & `autorag-0.1.9/docs/source/nodes/generator/llama_index_llm.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/generator/vllm.md` & `autorag-0.1.9/docs/source/nodes/generator/vllm.md`

 * *Files 8% similar despite different names*

```diff
@@ -23,12 +23,12 @@
   from [LLM initialization](https://github.com/vllm-project/vllm/blob/main/vllm/entrypoints/llm.py#L14)
   and [Sampling Params](https://github.com/vllm-project/vllm/blob/main/vllm/sampling_params.py#L25).
 
 ## **Example config.yaml**
 
 ```yaml
 modules:
-  - module_type: llama_index_llm
+  - module_type: vllm
     llm: mistralai/Mistral-7B-Instruct-v0.2
     temperature: [ 0.1, 1.0 ]
     max_tokens: 512
 ```
```

### Comparing `autorag-0.1.8/docs/source/nodes/passage_augmenter/passage_augmenter.md` & `autorag-0.1.9/docs/source/nodes/passage_augmenter/passage_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_augmenter/prev_next_augmenter.md` & `autorag-0.1.9/docs/source/nodes/passage_augmenter/prev_next_augmenter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_compressor/passage_compressor.md` & `autorag-0.1.9/docs/source/nodes/passage_compressor/passage_compressor.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_compressor/refine.md` & `autorag-0.1.9/docs/source/nodes/passage_compressor/refine.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_compressor/tree_summarize.md` & `autorag-0.1.9/docs/source/nodes/passage_compressor/tree_summarize.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_filter/passage_filter.md` & `autorag-0.1.9/docs/source/nodes/passage_filter/passage_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_filter/recency_filter.md` & `autorag-0.1.9/docs/source/nodes/passage_filter/recency_filter.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md` & `autorag-0.1.9/docs/source/nodes/passage_filter/similarity_percentile_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md` & `autorag-0.1.9/docs/source/nodes/passage_filter/similarity_threshold_cutoff.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/cohere.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/cohere.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/colbert.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/colbert.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/flag_embedding_llm_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/flag_embedding_reranker.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/flag_embedding_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/jina_reranker.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/jina_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/monot5.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/monot5.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/passage_reranker.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/passage_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/rankgpt.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/rankgpt.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/sentence_transformer_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/tart.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/tart.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/time_reranker.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/time_reranker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/passage_reranker/upr.md` & `autorag-0.1.9/docs/source/nodes/passage_reranker/upr.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/prompt_maker/fstring.md` & `autorag-0.1.9/docs/source/nodes/prompt_maker/fstring.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/prompt_maker/long_context_reorder.md` & `autorag-0.1.9/docs/source/nodes/prompt_maker/long_context_reorder.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/prompt_maker/prompt_maker.md` & `autorag-0.1.9/docs/source/nodes/prompt_maker/prompt_maker.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/query_expansion/hyde.md` & `autorag-0.1.9/docs/source/nodes/query_expansion/hyde.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/query_expansion/query_decompose.md` & `autorag-0.1.9/docs/source/nodes/query_expansion/query_decompose.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/query_expansion/query_expansion.md` & `autorag-0.1.9/docs/source/nodes/query_expansion/query_expansion.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/retrieval/bm25.md` & `autorag-0.1.9/docs/source/nodes/retrieval/bm25.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/retrieval/hybrid_cc.md` & `autorag-0.1.9/docs/source/nodes/retrieval/hybrid_cc.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/retrieval/hybrid_dbsf.md` & `autorag-0.1.9/docs/source/nodes/retrieval/hybrid_dbsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/retrieval/hybrid_rrf.md` & `autorag-0.1.9/docs/source/nodes/retrieval/hybrid_rrf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/retrieval/hybrid_rsf.md` & `autorag-0.1.9/docs/source/nodes/retrieval/hybrid_rsf.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/retrieval/retrieval.md` & `autorag-0.1.9/docs/source/nodes/retrieval/retrieval.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/nodes/retrieval/vectordb.md` & `autorag-0.1.9/docs/source/nodes/retrieval/vectordb.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/optimization/custom_config.md` & `autorag-0.1.9/docs/source/optimization/custom_config.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/optimization/folder_structure.md` & `autorag-0.1.9/docs/source/optimization/folder_structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/optimization/optimization.md` & `autorag-0.1.9/docs/source/optimization/optimization.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/optimization/sample_full_config.yaml` & `autorag-0.1.9/docs/source/optimization/sample_full_config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/roadmap/modular_rag.md` & `autorag-0.1.9/docs/source/roadmap/modular_rag.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/structure.md` & `autorag-0.1.9/docs/source/structure.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/troubleshooting.md` & `autorag-0.1.9/docs/source/troubleshooting.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/docs/source/tutorial.md` & `autorag-0.1.9/docs/source/tutorial.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/pyproject.toml` & `autorag-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/requirements.txt` & `autorag-0.1.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_config/compact_local.yaml` & `autorag-0.1.9/sample_config/compact_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_config/compact_openai.yaml` & `autorag-0.1.9/sample_config/compact_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_config/config_korean.yaml` & `autorag-0.1.9/sample_config/config_korean.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_config/extracted_sample.yaml` & `autorag-0.1.9/sample_config/extracted_sample.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_config/full.yaml` & `autorag-0.1.9/sample_config/full.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -134,7 +134,10 @@
           - metric_name: g_eval
         speed_threshold: 10
       modules:
         - module_type: llama_index_llm
           llm: [openai]
           model: [gpt-3.5-turbo-16k, gpt-3.5-turbo-1106]
           temperature: [0.5, 1.0, 1.5]
+        - module_type: openai_llm
+          llm: gpt-3.5-turbo
+          temperature: 0.8
```

### Comparing `autorag-0.1.8/sample_config/simple_local.yaml` & `autorag-0.1.9/sample_config/simple_local.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_config/simple_openai.yaml` & `autorag-0.1.9/sample_config/simple_openai.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_dataset/README.md` & `autorag-0.1.9/sample_dataset/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_dataset/eli5/load_eli5_dataset.py` & `autorag-0.1.9/sample_dataset/eli5/load_eli5_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_dataset/msmarco/load_msmarco_dataset.py` & `autorag-0.1.9/sample_dataset/msmarco/load_msmarco_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/sample_dataset/triviaqa/load_triviaqa_dataset.py` & `autorag-0.1.9/sample_dataset/triviaqa/load_triviaqa_dataset.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/data/corpus/test_base.py` & `autorag-0.1.9/tests/autorag/data/corpus/test_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/data/corpus/test_langchain.py` & `autorag-0.1.9/tests/autorag/data/corpus/test_langchain.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/data/corpus/test_llama_index_corpus.py` & `autorag-0.1.9/tests/autorag/data/corpus/test_llama_index_corpus.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/data/qacreation/test_base_qacreation.py` & `autorag-0.1.9/tests/autorag/data/qacreation/test_base_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/data/qacreation/test_llama_index_qacreation.py` & `autorag-0.1.9/tests/autorag/data/qacreation/test_llama_index_qacreation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/data/qacreation/test_ragas_qa_creation.py` & `autorag-0.1.9/tests/autorag/data/qacreation/test_ragas_qa_creation.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/data/qacreation/test_simple.py` & `autorag-0.1.9/tests/autorag/data/qacreation/test_simple.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/evaluate/metric/test_generation_metric.py` & `autorag-0.1.9/tests/autorag/evaluate/metric/test_generation_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py` & `autorag-0.1.9/tests/autorag/evaluate/metric/test_retrieval_contents_metric.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/evaluate/test_evaluate_util.py` & `autorag-0.1.9/tests/autorag/evaluate/test_evaluate_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/evaluate/test_generation_evaluate.py` & `autorag-0.1.9/tests/autorag/evaluate/test_generation_evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from unittest.mock import patch
 
+import openai
 import pandas as pd
 import pytest
 from openai.resources.chat import Completions
 from openai.types.chat import ChatCompletion, ChatCompletionMessage, ChatCompletionTokenLogprob
 from openai.types.chat.chat_completion import Choice, ChoiceLogprobs
 from openai.types.chat.chat_completion_token_logprob import TopLogprob
 from transformers import AutoTokenizer
@@ -40,15 +41,15 @@
 
 @evaluate_generation(generation_gt=generation_gts, metrics=[{'metric_name': 'bleu'}, {'metric_name': 'sem_score',
                                                                                       'embedding_model': 'openai'}])
 def pseudo_generation_dict_metrics():
     return pseudo_generations
 
 
-def mock_g_eval_openai_create(*args, **kwargs):
+async def mock_g_eval_openai_create(*args, **kwargs):
     sample_choice = Choice(finish_reason="stop", index=0,
                            message=ChatCompletionMessage(
                                content="2",
                                role="assistant",
                            ),
                            logprobs=ChoiceLogprobs(
                                content=[
@@ -65,15 +66,15 @@
         n = kwargs['n']
     return ChatCompletion(id='_id',
                           choices=[sample_choice] * n,
                           created=1713363661, model=kwargs['model'],
                           object="chat.completion")
 
 
-@patch.object(Completions, 'create', mock_g_eval_openai_create)
+@patch.object(openai.resources.chat.completions.AsyncCompletions, 'create', mock_g_eval_openai_create)
 def test_evaluate_generation():
     result_df = pseudo_generation()
     assert isinstance(result_df, pd.DataFrame)
     assert len(result_df) == 3
     assert len(result_df.columns) == 6
     assert set(result_df.columns) == {'generated_texts', 'bleu', 'meteor', 'rouge', 'sem_score', 'g_eval'}
```

### Comparing `autorag-0.1.8/tests/autorag/evaluate/test_retrieval_contents_evaluate.py` & `autorag-0.1.9/tests/autorag/evaluate/test_retrieval_contents_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/evaluate/test_retrieval_evaluate.py` & `autorag-0.1.9/tests/autorag/evaluate/test_retrieval_evaluate.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/generator/test_generator_base.py` & `autorag-0.1.9/tests/autorag/nodes/generator/test_generator_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/generator/test_llama_index_llm.py` & `autorag-0.1.9/tests/autorag/nodes/generator/test_llama_index_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/generator/test_run_generator_node.py` & `autorag-0.1.9/tests/autorag/nodes/generator/test_run_generator_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/generator/test_vllm.py` & `autorag-0.1.9/tests/autorag/nodes/generator/test_vllm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py` & `autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_base_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py` & `autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_pass_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py` & `autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_prev_next_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py` & `autorag-0.1.9/tests/autorag/nodes/passageaugmenter/test_run_passage_augmenter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py` & `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_base_passage_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_pass_compressor.py` & `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_pass_compressor.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_refine.py` & `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_refine.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py` & `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_run_passage_compressor_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagecompressor/test_tree_summarize.py` & `autorag-0.1.9/tests/autorag/nodes/passagecompressor/test_tree_summarize.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py` & `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_pass_passage_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_passage_filter_base.py` & `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_passage_filter_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_passage_filter_run.py` & `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_passage_filter_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py` & `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_percentile_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_recency_filter.py` & `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_recency_filter.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py` & `autorag-0.1.9/tests/autorag/nodes/passagefilter/test_threshold_cutoff.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_cohere_reranker.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_cohere_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_colbert_reranker.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_colbert_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_flag_embedding.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_flag_embedding.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_flag_embedding_llm.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_jina_reranker.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_jina_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_koreranker.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_koreranker.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,11 +13,21 @@
     original_koreranker = koreranker.__wrapped__
     contents_result, id_result, score_result \
         = original_koreranker(ko_queries_example, ko_contents_example, scores_example, ids_example, top_k)
     base_reranker_test(contents_result, id_result, score_result, top_k, use_ko=True)
 
 
 @pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
+def test_koreranker_batch_one():
+    top_k = 1
+    batch = 1
+    original_koreranker = koreranker.__wrapped__
+    contents_result, id_result, score_result \
+        = original_koreranker(ko_queries_example, ko_contents_example, scores_example, ids_example, top_k, batch)
+    base_reranker_test(contents_result, id_result, score_result, top_k, use_ko=True)
+
+
+@pytest.mark.skipif(is_github_action(), reason="Skipping this test on GitHub Actions")
 def test_koreranker_node():
     top_k = 1
     result_df = koreranker(project_dir=project_dir, previous_result=ko_previous_result, top_k=top_k)
     base_reranker_node_test(result_df, top_k, use_ko=True)
```

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_monot5.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_monot5.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_pass_reranker.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_pass_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_passage_reranker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_passage_reranker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_rankgpt.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_rankgpt.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_sentence_transformer.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_sentence_transformer.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_tart.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_tart.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_time_reranker.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_time_reranker.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/passagereranker/test_upr.py` & `autorag-0.1.9/tests/autorag/nodes/passagereranker/test_upr.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/promptmaker/test_fstring.py` & `autorag-0.1.9/tests/autorag/nodes/promptmaker/test_fstring.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/promptmaker/test_long_context_reorder.py` & `autorag-0.1.9/tests/autorag/nodes/promptmaker/test_long_context_reorder.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py` & `autorag-0.1.9/tests/autorag/nodes/promptmaker/test_prompt_maker_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py` & `autorag-0.1.9/tests/autorag/nodes/promptmaker/test_prompt_maker_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_hyde.py` & `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_hyde.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py` & `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_pass_query_expansion.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_decompose.py` & `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_decompose.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py` & `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_expansion_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py` & `autorag-0.1.9/tests/autorag/nodes/queryexpansion/test_query_expansion_run.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/retrieval/test_bm25.py` & `autorag-0.1.9/tests/autorag/nodes/retrieval/test_bm25.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_base.py` & `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_cc.py` & `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_cc.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py` & `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_dbsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_rrf.py` & `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_rrf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/retrieval/test_hybrid_rsf.py` & `autorag-0.1.9/tests/autorag/nodes/retrieval/test_hybrid_rsf.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/retrieval/test_retrieval_base.py` & `autorag-0.1.9/tests/autorag/nodes/retrieval/test_retrieval_base.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/retrieval/test_run_retrieval_node.py` & `autorag-0.1.9/tests/autorag/nodes/retrieval/test_run_retrieval_node.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/nodes/retrieval/test_vectordb.py` & `autorag-0.1.9/tests/autorag/nodes/retrieval/test_vectordb.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/schema/test_module_schema.py` & `autorag-0.1.9/tests/autorag/schema/test_module_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/schema/test_node_schema.py` & `autorag-0.1.9/tests/autorag/schema/test_node_schema.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/test_cli.py` & `autorag-0.1.9/tests/autorag/test_cli.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/test_deploy.py` & `autorag-0.1.9/tests/autorag/test_deploy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/test_evaluator.py` & `autorag-0.1.9/tests/autorag/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/test_strategy.py` & `autorag-0.1.9/tests/autorag/test_strategy.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/test_web.py` & `autorag-0.1.9/tests/autorag/test_web.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/utils/test_preprocess.py` & `autorag-0.1.9/tests/autorag/utils/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/autorag/utils/test_util.py` & `autorag-0.1.9/tests/autorag/utils/test_util.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/delete_tests.py` & `autorag-0.1.9/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/README.md` & `autorag-0.1.9/tests/resources/README.md`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/corpus_data_sample.parquet` & `autorag-0.1.9/tests/resources/corpus_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/data_creation/raw_dir/sample1.txt` & `autorag-0.1.9/tests/resources/data_creation/raw_dir/sample1.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/data_creation/raw_dir/sample2.txt` & `autorag-0.1.9/tests/resources/data_creation/raw_dir/sample2.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/data_creation/raw_dir/sample3.txt` & `autorag-0.1.9/tests/resources/data_creation/raw_dir/sample3.txt`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/full.yaml` & `autorag-0.1.9/tests/resources/full.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/qa_data_sample.parquet` & `autorag-0.1.9/tests/resources/qa_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/qa_test_data_sample.parquet` & `autorag-0.1.9/tests/resources/qa_test_data_sample.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/config.yaml` & `autorag-0.1.9/tests/resources/result_project/0/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/3.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/4.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/best_5.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/generator/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv` & `autorag-0.1.9/tests/resources/result_project/0/post_retrieve_node_line/prompt_maker/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/0/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/0/summary.csv` & `autorag-0.1.9/tests/resources/result_project/0/summary.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/config.yaml` & `autorag-0.1.9/tests/resources/result_project/1/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/1/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/1/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/config.yaml` & `autorag-0.1.9/tests/resources/result_project/2/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet` & `autorag-0.1.9/tests/resources/result_project/2/post_retrieve_node_line/prompt_maker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet` & `autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet` & `autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet` & `autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/2.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/2/pre_retrieve_node_line/query_expansion/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet` & `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_compressor/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet` & `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet` & `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/passage_reranker/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet` & `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet` & `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/1.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet` & `autorag-0.1.9/tests/resources/result_project/2/retrieve_node_line/retrieval/best_0.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/3/config.yaml` & `autorag-0.1.9/tests/resources/result_project/3/config.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/best.yaml` & `autorag-0.1.9/tests/resources/result_project/best.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/data/corpus.parquet` & `autorag-0.1.9/tests/resources/result_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/data/qa.parquet` & `autorag-0.1.9/tests/resources/result_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/resources/bm25.pkl` & `autorag-0.1.9/tests/resources/result_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin` & `autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/data_level0.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin` & `autorag-0.1.9/tests/resources/result_project/resources/chroma/6595d304-5270-4d9f-a267-c191366804ce/length.bin`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/result_project/resources/chroma/chroma.sqlite3` & `autorag-0.1.9/tests/resources/result_project/resources/chroma/chroma.sqlite3`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/sample_contents_nqa.csv` & `autorag-0.1.9/tests/resources/sample_contents_nqa.csv`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/sample_project/data/corpus.parquet` & `autorag-0.1.9/tests/resources/sample_project/data/corpus.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/sample_project/data/qa.parquet` & `autorag-0.1.9/tests/resources/sample_project/data/qa.parquet`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/sample_project/resources/bm25.pkl` & `autorag-0.1.9/tests/resources/sample_project/resources/bm25.pkl`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/simple.yaml` & `autorag-0.1.9/tests/resources/simple.yaml`

 * *Files identical despite different names*

### Comparing `autorag-0.1.8/tests/resources/test_bm25_retrieval.pkl` & `autorag-0.1.9/tests/resources/test_bm25_retrieval.pkl`

 * *Files identical despite different names*

