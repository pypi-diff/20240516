# Comparing `tmp/beaker_bunsen-0.0.2.tar.gz` & `tmp/beaker_bunsen-0.0.3.tar.gz`

## Comparing `beaker_bunsen-0.0.2.tar` & `beaker_bunsen-0.0.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/DEFINITIONS.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/.github/workflows/build-publish.yaml
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/.github/workflows/test.yaml
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/__init__.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/bunsen_agent.py
--rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/bunsen_context.py
--rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/corpus.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/builder/__init__.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/builder/hooks.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/__init__.py
--rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/chromadb_store.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/types.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/vector_store.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/__init__.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/base.py
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/code.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/document.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/documentation.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/examples.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/__init__.py
--rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/base.py
--rw-r--r--   0        0        0     5352 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/code_library_loader.py
--rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/local_file_loader.py
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/schemes.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/util/helpers.py
--rw-r--r--   0        0        0    10848 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/util/splitters.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_base_embedder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_build.py
--rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_chromadb.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_code_loaders.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_corpus.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_documentation_embedder.py
--rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_example_embedder.py
--rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_local_file_loader.py
--rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_schemes.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_utils.py
--rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/test_zipped_chromadb.py
--rw-r--r--   0        0        0  1828380 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/store.zip
--rw-r--r--   0        0        0  5947974 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/corpus.zip
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/config.yaml
--rw-r--r--   0        0        0  5692346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/store.zip
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.__version__
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.adapters
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.api
--rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.auth
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.certs
--rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.compat
--rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.cookies
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.exceptions
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.help
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.hooks
--rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.models
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.packages
--rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.sessions
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.status_codes
--rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.structures
--rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.utils
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documentation/ruff_readme.md
--rw-r--r--   0        0        0   137697 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/Lunar_Sample_Laboratory_Facility.html
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/yorkshire.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/yorkshire.txt.metadata
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/.metadata
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/ham_and_lentil_soup
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/irish_potato_caserole
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/tajine_maadnous
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/winter_risotto
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/documents/recipes/winter_risotto.metadata
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/examples/example_1.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/examples/example_2.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/examples/example_3.md
--rw-r--r--   0        0        0   307464 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/images/kitten-sad.jpg
--rw-r--r--   0        0        0   417493 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/images/kitten_hacker.jpg
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/images/puppy_hacker.jpg
--rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/images/puppy_sad.png
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/pyproject.toml
--rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/documentation/mathjax_readme.md
--rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/documentation/ruff_readme.md
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/examples/example_1.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/examples/example_2.md
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/examples/example_3.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/src/test_project/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/src/test_project/agent.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/tests/data/subproject/src/test_project/context.py
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/README.md
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6076 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/DEFINITIONS.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/.github/workflows/build-publish.yaml
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/__init__.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/bunsen_agent.py
+-rw-r--r--   0        0        0     8638 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/bunsen_context.py
+-rw-r--r--   0        0        0     9901 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/corpus.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/builder/__init__.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/builder/hooks.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/__init__.py
+-rw-r--r--   0        0        0    14512 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/chromadb_store.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/types.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/vector_store.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/embedders/__init__.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/embedders/base.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/embedders/code.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/embedders/document.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/embedders/documentation.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/embedders/examples.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/loaders/__init__.py
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/loaders/base.py
+-rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/loaders/code_library_loader.py
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/loaders/local_file_loader.py
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/loaders/schemes.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/util/helpers.py
+-rw-r--r--   0        0        0    11738 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/util/splitters.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_base_embedder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_build.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_chromadb.py
+-rw-r--r--   0        0        0     4593 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_code_loaders.py
+-rw-r--r--   0        0        0     5302 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_corpus.py
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_documentation_embedder.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_example_embedder.py
+-rw-r--r--   0        0        0     6588 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_local_file_loader.py
+-rw-r--r--   0        0        0     3937 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_schemes.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_utils.py
+-rw-r--r--   0        0        0     9969 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/test_zipped_chromadb.py
+-rw-r--r--   0        0        0  1828380 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/store.zip
+-rw-r--r--   0        0        0  5947974 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/corpus.zip
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/config.yaml
+-rw-r--r--   0        0        0  5692346 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/store.zip
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.__version__
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils
+-rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.adapters
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.api
+-rw-r--r--   0        0        0    10187 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.auth
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.certs
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.compat
+-rw-r--r--   0        0        0    18560 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.cookies
+-rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.exceptions
+-rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.help
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.hooks
+-rw-r--r--   0        0        0    35223 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.models
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.packages
+-rw-r--r--   0        0        0    30373 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.sessions
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.status_codes
+-rw-r--r--   0        0        0     2912 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.structures
+-rw-r--r--   0        0        0    33448 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.utils
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documentation/ruff_readme.md
+-rw-r--r--   0        0        0   137697 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documents/Lunar_Sample_Laboratory_Facility.html
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documents/yorkshire.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documents/yorkshire.txt.metadata
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documents/recipes/.metadata
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documents/recipes/ham_and_lentil_soup
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documents/recipes/irish_potato_caserole
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documents/recipes/tajine_maadnous
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documents/recipes/winter_risotto
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/documents/recipes/winter_risotto.metadata
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/examples/example_1.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/examples/example_2.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/examples/example_3.md
+-rw-r--r--   0        0        0   307464 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/images/kitten-sad.jpg
+-rw-r--r--   0        0        0   417493 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/images/kitten_hacker.jpg
+-rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/images/puppy_hacker.jpg
+-rw-r--r--   0        0        0    64027 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/images/puppy_sad.png
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/subproject/pyproject.toml
+-rw-r--r--   0        0        0     9885 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/subproject/documentation/mathjax_readme.md
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/subproject/documentation/ruff_readme.md
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/subproject/examples/example_1.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/subproject/examples/example_2.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/subproject/examples/example_3.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/subproject/src/test_project/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/subproject/src/test_project/agent.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/tests/data/subproject/src/test_project/context.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/README.md
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 beaker_bunsen-0.0.3/PKG-INFO
```

### Comparing `beaker_bunsen-0.0.2/DEFINITIONS.md` & `beaker_bunsen-0.0.3/DEFINITIONS.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/.github/workflows/build-publish.yaml` & `beaker_bunsen-0.0.3/.github/workflows/build-publish.yaml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/.github/workflows/test.yaml` & `beaker_bunsen-0.0.3/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/bunsen_agent.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/bunsen_agent.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/bunsen_context.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/bunsen_context.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/corpus.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/corpus.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/builder/hooks.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/builder/hooks.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/chromadb_store.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/chromadb_store.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/types.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/types.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/vector_store.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/vector_store.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/base.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/embedders/base.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/document.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/embedders/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         chunk_size: int = 2000,
         chunk_overlap: int = 100,
         splitter: TextSplitter =  None,
     ) -> None:
         self.splitter = splitter
         super().__init__(store, loader, embedding_function, chunk_size, chunk_overlap)
 
-    def get_splitter(self):
+    def get_splitter(self, resource: Resource):
         if self.splitter:
             return self.splitter
         splitter = self.splitter_class(
             chunk_size=self.chunk_size,
             chunk_overlap=self.chunk_overlap
         )
         return splitter
@@ -52,15 +52,15 @@
         if content is None:
             raise ValueError(f"Can't retrieve content for resource {resource}")
 
         if isinstance(content, (str, bytes)) and len(content) == 0:
             # Empty file, no chunks to yield
             return
 
-        splitter = self.get_splitter()
+        splitter = self.get_splitter(resource)
         for i, content_chunk in enumerate(
                 splitter.split_text(content),
                 start=1
         ):
             record = Record(
                 id=f"{resource.id}:{i}",
                 uri=resource.uri,
```

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/embedders/examples.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/embedders/examples.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/base.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/loaders/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,17 @@
     def parse_locations(
         self,
         locations: list[str],
     ) -> tuple[list[str], list[str]]:
         exclusions = []
         for location in locations[:]:
             if str(location).startswith("!"):
-                exclusion_value = str(locations.pop(location))
-                exclusions.append(exclusion_value.removeprefix('!'))
+                locations.remove(location)
+                exclusion_value = str(location).removeprefix('!')
+                exclusions.append(exclusion_value)
         return locations, exclusions
 
 
     def should_exclude(
         self,
         location: str,
         exclusions: list[str] | DefaultType = Default
```

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/code_library_loader.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/loaders/code_library_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
             if getattr(module_spec, "submodule_search_locations", []):
                 subpkg_info: pkgutil.ModuleInfo = pkgutil.iter_modules(path=module_spec.submodule_search_locations)
                 subpkg_specs = (info.module_finder.find_spec(f"{module_spec.name}.{info.name}") for info in subpkg_info)
                 if self.exclusions:
                     subpkg_specs = (
                         spec for spec in subpkg_specs
-                        if not self.should_exclude(spec)
+                        if not self.should_exclude(spec.name)
                     )
                 modules_to_collect.extend(
                     subpkg_specs
                 )
 
             if hasattr(module_spec, "loader"):
                 source = module_spec.loader.get_source(module_spec.name)
```

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/local_file_loader.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/loaders/local_file_loader.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/loaders/schemes.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/loaders/schemes.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/util/helpers.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/util/helpers.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/src/beaker_bunsen/vectordb/util/splitters.py` & `beaker_bunsen-0.0.3/src/beaker_bunsen/vectordb/util/splitters.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,14 +178,69 @@
 class RecursiveCharacterTextSplitter(TextSplitter):
     """Splitting text by recursively look at characters.
 
     Recursively tries to split by different characters to find one
     that works.
     """
 
+    LANGUAGES_BY_EXTENSION = {
+        "rst": "restructured",
+        "py": "python",
+        "md": "markdown",
+        "jl": "julia",
+        "r": "r",
+    }
+
+    SEPARATORS_BY_LANGUAGE = {
+        "restructured": [
+                # Split along section titles
+                "\n=+\n",
+                "\n-+\n",
+                "\n\\*+\n",
+                # Split along directive markers
+                "\n\n.. *\n\n",
+                # Split by the normal type of lines
+                "\n\n",
+                "\n",
+                " ",
+                "",
+            ],
+        'python': [
+                # First, try to split along class definitions
+                "\nclass ",
+                "\ndef ",
+                "\n\tdef ",
+                "\n    def ",
+                # Now split by the normal type of lines
+                "\n\n",
+                "\n",
+                " ",
+                "",
+            ],
+        "markdown": [
+                # First, try to split along Markdown headings (starting with level 2)
+                "\n#{1,6} ",
+                # Note the alternative syntax for headings (below) is not handled here
+                # Heading level 2
+                # ---------------
+                # End of code block
+                "```\n",
+                # Horizontal lines
+                "\n\\*\\*\\*+\n",
+                "\n---+\n",
+                "\n___+\n",
+                # Note that this splitter doesn't handle horizontal lines defined
+                # by *three or more* of ***, ---, or ___, but this is not handled
+                "\n\n",
+                "\n",
+                " ",
+                "",
+            ]
+    }
+
     def __init__(
         self,
         separators: Optional[List[str]] = None,
         keep_separator: bool = True,
         is_separator_regex: bool = False,
         **kwargs: Any,
     ) -> None:
@@ -237,59 +292,28 @@
     def split_text(self, text: str) -> List[str]:
         return self._split_text(text, self._separators)
 
     @classmethod
     def from_language(
         cls, language: str, **kwargs: Any
     ):
-        separators = cls.get_separators_for_language(language)
+        if language in cls.SEPARATORS_BY_LANGUAGE:
+            separators = cls.SEPARATORS_BY_LANGUAGE[language]
+        elif language in cls.LANGUAGES_BY_EXTENSION:
+            separators = cls.SEPARATORS_BY_LANGUAGE(cls.LANGUAGES_BY_EXTENSION[language])
+        else:
+            raise ValueError(f"Could not map language '{language}' to a known type for splitting/chunking.")
         return cls(separators=separators, is_separator_regex=True, **kwargs)
 
-    @staticmethod
-    def get_separators_for_language(extension: str) -> List[str]:
-        if extension == ".rst":
-            return [
-                # Split along section titles
-                "\n=+\n",
-                "\n-+\n",
-                "\n\\*+\n",
-                # Split along directive markers
-                "\n\n.. *\n\n",
-                # Split by the normal type of lines
-                "\n\n",
-                "\n",
-                " ",
-                "",
-            ]
-        elif extension == '.py':
-            return [
-                # First, try to split along class definitions
-                "\nclass ",
-                "\ndef ",
-                "\n\tdef ",
-                "\n    def ",
-                # Now split by the normal type of lines
-                "\n\n",
-                "\n",
-                " ",
-                "",
-            ]
-        elif extension == ".md":
-            return [
-                # First, try to split along Markdown headings (starting with level 2)
-                "\n#{1,6} ",
-                # Note the alternative syntax for headings (below) is not handled here
-                # Heading level 2
-                # ---------------
-                # End of code block
-                "```\n",
-                # Horizontal lines
-                "\n\\*\\*\\*+\n",
-                "\n---+\n",
-                "\n___+\n",
-                # Note that this splitter doesn't handle horizontal lines defined
-                # by *three or more* of ***, ---, or ___, but this is not handled
-                "\n\n",
-                "\n",
-                " ",
-                "",
-            ]
+    @classmethod
+    def from_extension(
+        cls, extension: str, **kwargs: Any
+    ):
+        if extension.startswith("."):
+            extension = extension.removeprefix(".")
+
+        language = cls.LANGUAGES_BY_EXTENSION.get(extension, None)
+        if language not in cls.SEPARATORS_BY_LANGUAGE:
+            raise ValueError(f"Could not map extension '{extension}' to a known type for splitting/chunking.")
+
+        separators = cls.SEPARATORS_BY_LANGUAGE[language]
+        return cls(separators=separators, is_separator_regex=True, **kwargs)
```

### Comparing `beaker_bunsen-0.0.2/tests/test_base_embedder.py` & `beaker_bunsen-0.0.3/tests/test_base_embedder.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/test_chromadb.py` & `beaker_bunsen-0.0.3/tests/test_chromadb.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/test_corpus.py` & `beaker_bunsen-0.0.3/tests/test_corpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 import pytest
 import zipfile
 from pathlib import Path
 
 from beaker_bunsen.vectordb.types import Resource
 from beaker_bunsen.vectordb.chromadb_store import BaseChromaDBStore, ZippedChromaDBStore
-from beaker_bunsen.vectordb.embedders import BaseEmbedder, DocumentationEmbedder, ExampleEmbedder
+from beaker_bunsen.vectordb.embedders import BaseEmbedder, DocumentationEmbedder, ExampleEmbedder, CodeEmbedder
 from beaker_bunsen.vectordb.loaders import LocalFileLoader, PythonLibraryLoader
 from beaker_bunsen.vectordb.loaders.schemes import read_from_uri
 from beaker_bunsen.corpus import Corpus
 
 def get_all_records_by_partition(store: BaseChromaDBStore):
     return sorted(
         ((partition, sorted(store.get_all(partition=partition), key=lambda p:p.id))
@@ -43,15 +43,15 @@
 
     # example_embedder = DocumentationEmbedder
     example_loader = LocalFileLoader(locations=[test_data_path / "documentation"])
     corpus.ingest(embedder_cls=DocumentationEmbedder, loader=example_loader, partition="documentation")
     corpus_records_2 = get_all_records_by_partition(corpus.store)
 
     requests_loader = PythonLibraryLoader(locations=["requests"])
-    corpus.ingest(embedder_cls=DocumentationEmbedder, loader=requests_loader, partition="code")
+    corpus.ingest(embedder_cls=CodeEmbedder, loader=requests_loader, partition="code")
 
     corpus_records_3 = get_all_records_by_partition(corpus.store)
 
     assert len(corpus_records_1) == 0
     assert len(corpus_records_2) > len(corpus_records_1)
     assert len(corpus_records_3) > len(corpus_records_2)
 
@@ -65,15 +65,15 @@
     corpus = Corpus(store=store)
 
     # example_embedder = DocumentationEmbedder
     example_loader = LocalFileLoader(locations=[test_data_path / "documentation"])
     corpus.ingest(embedder_cls=DocumentationEmbedder, loader=example_loader, partition="documentation")
 
     requests_loader = PythonLibraryLoader(locations=["requests"])
-    corpus.ingest(embedder_cls=DocumentationEmbedder, loader=requests_loader, partition="code")
+    corpus.ingest(embedder_cls=CodeEmbedder, loader=requests_loader, partition="code")
 
     corpus.save_to_dir(save_dir=save_location)
 
     corpus_files = list((
         str(Path(dir_path).relative_to(save_location) /  file)
         for dir_path, _, files in os.walk(save_location)
         for file in files
```

### Comparing `beaker_bunsen-0.0.2/tests/test_documentation_embedder.py` & `beaker_bunsen-0.0.3/tests/test_documentation_embedder.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/test_example_embedder.py` & `beaker_bunsen-0.0.3/tests/test_example_embedder.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/test_local_file_loader.py` & `beaker_bunsen-0.0.3/tests/test_local_file_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -116,7 +116,28 @@
 
     excluded_files = files_from_os_walk - found_files
 
     assert len(found_files) < len(files_from_os_walk)
     assert any([exclusion in filename for filename in files_from_os_walk])
     assert all([exclusion in filename for filename in excluded_files])
     assert all([exclusion not in filename for filename in found_files])
+
+def test_exclusions_discover():
+    exclusion = "ato"
+    abs_file_path = Path(__file__).parent / "data" / "documents"
+    local_file_loader = LocalFileLoader()
+    found_locations = set([record.uri for record in local_file_loader.discover(
+        locations=[abs_file_path, f"!{exclusion}"],
+    )])
+    # Strip off any `{prefix}:` from the locations
+    found_files = set([location.split(":", maxsplit=1)[1] for location in found_locations])
+
+    files_from_os_walk = set()
+    for path, _, files in os.walk(abs_file_path, ):
+        files_from_os_walk.update([os.path.join(path, f) for f in files if not f.endswith('.metadata')])
+
+    excluded_files = files_from_os_walk - found_files
+
+    assert len(found_files) < len(files_from_os_walk)
+    assert any([exclusion in filename for filename in files_from_os_walk])
+    assert all([exclusion in filename for filename in excluded_files])
+    assert all([exclusion not in filename for filename in found_files])
```

### Comparing `beaker_bunsen-0.0.2/tests/test_schemes.py` & `beaker_bunsen-0.0.3/tests/test_schemes.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/test_utils.py` & `beaker_bunsen-0.0.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/test_zipped_chromadb.py` & `beaker_bunsen-0.0.3/tests/test_zipped_chromadb.py`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/store.zip` & `beaker_bunsen-0.0.3/tests/data/store.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/corpus.zip` & `beaker_bunsen-0.0.3/tests/data/corpuses/corpus.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/store.zip` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/store.zip`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests._internal_utils`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.adapters` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.adapters`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.api` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.api`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.auth` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.auth`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.compat` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.compat`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.cookies` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.cookies`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.exceptions` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.exceptions`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.help` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.help`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.hooks` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.hooks`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.models` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.models`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.packages` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.packages`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.sessions` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.sessions`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.status_codes` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.status_codes`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.structures` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.structures`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/code/requests.utils` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/code/requests.utils`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md` & `beaker_bunsen-0.0.3/tests/data/corpuses/test-corpus/resources/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.3/tests/data/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/documentation/ruff_readme.md` & `beaker_bunsen-0.0.3/tests/data/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/documents/Lunar_Sample_Laboratory_Facility.html` & `beaker_bunsen-0.0.3/tests/data/documents/Lunar_Sample_Laboratory_Facility.html`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/documents/yorkshire.txt` & `beaker_bunsen-0.0.3/tests/data/documents/yorkshire.txt`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/documents/recipes/irish_potato_caserole` & `beaker_bunsen-0.0.3/tests/data/documents/recipes/irish_potato_caserole`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/documents/recipes/tajine_maadnous` & `beaker_bunsen-0.0.3/tests/data/documents/recipes/tajine_maadnous`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/documents/recipes/winter_risotto` & `beaker_bunsen-0.0.3/tests/data/documents/recipes/winter_risotto`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/images/kitten-sad.jpg` & `beaker_bunsen-0.0.3/tests/data/images/kitten-sad.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/images/kitten_hacker.jpg` & `beaker_bunsen-0.0.3/tests/data/images/kitten_hacker.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/images/puppy_hacker.jpg` & `beaker_bunsen-0.0.3/tests/data/images/puppy_hacker.jpg`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/images/puppy_sad.png` & `beaker_bunsen-0.0.3/tests/data/images/puppy_sad.png`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/subproject/pyproject.toml` & `beaker_bunsen-0.0.3/tests/data/subproject/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/subproject/documentation/mathjax_readme.md` & `beaker_bunsen-0.0.3/tests/data/subproject/documentation/mathjax_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/tests/data/subproject/documentation/ruff_readme.md` & `beaker_bunsen-0.0.3/tests/data/subproject/documentation/ruff_readme.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/.gitignore` & `beaker_bunsen-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/LICENSE.txt` & `beaker_bunsen-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/README.md` & `beaker_bunsen-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/pyproject.toml` & `beaker_bunsen-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beaker_bunsen-0.0.2/PKG-INFO` & `beaker_bunsen-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: beaker-bunsen
-Version: 0.0.2
+Version: 0.0.3
 Summary: Quickly generate new Beaker contexts for new domains and libraries.
 Project-URL: Documentation, https://github.com/unknown/beaker-bunsen#readme
 Project-URL: Issues, https://github.com/unknown/beaker-bunsen/issues
 Project-URL: Source, https://github.com/unknown/beaker-bunsen
 Author-email: Matthew Printz <matt@jataware.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

