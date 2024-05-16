# Comparing `tmp/stepup_reprep-1.1.1.tar.gz` & `tmp/stepup_reprep-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepup_reprep-1.1.1.tar", last modified: Tue May  7 17:50:13 2024, max compression
+gzip compressed data, was "stepup_reprep-1.1.2.tar", last modified: Thu May 16 11:29:58 2024, max compression
```

## Comparing `stepup_reprep-1.1.1.tar` & `stepup_reprep-1.1.2.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.145305 stepup_reprep-1.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.153305 stepup_reprep-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.github/workflows/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.153305 stepup_reprep-1.1.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.153305 stepup_reprep-1.1.1/docs/advanced_topics/
--rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/good_practices.md
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/manifest_files.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.157306 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/figure.png
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/hexagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/pentagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/square.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/triangle.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs.md
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/clean_stdout.sed
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/development.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.157306 stepup_reprep-1.1.1/docs/from_scratch/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_scratch/introduction.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.157306 stepup_reprep-1.1.1/docs/from_template/
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_template/before_you_begin.md
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_template/create_or_clone_a_project.md
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_template/introduction.md
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/from_template/working_on_a_project.md
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.157306 stepup_reprep-1.1.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/reference/stepup.reprep.api.md
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/docs/reference/stepup.reprep.tile_pdf.md
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.149305 stepup_reprep-1.1.1/stepup/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.161306 stepup_reprep-1.1.1/stepup/reprep/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/add_notes_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    25407 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/bibtex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/check_hrefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/check_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/convert_inkscape.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/convert_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/latex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/latex_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/latex_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/latex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/make_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/normalize_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/nup_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/raster_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/tile_pdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/stepup/reprep/zip_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/stepup_reprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-07 17:50:13.000000 stepup_reprep-1.1.1/stepup_reprep.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.161306 stepup_reprep-1.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.149305 stepup_reprep-1.1.1/tests/cases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.161306 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/notes.pdf
--rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/add_notes_pdf/src.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.165305 stepup_reprep-1.1.1/tests/cases/cat_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/doc1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/doc2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      955 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/cat_pdf/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.165305 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_html/test.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.165305 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      596 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_md/test.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.169306 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/check_hrefs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      728 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/main.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.169306 stepup_reprep-1.1.1/tests/cases/convert_inkscape/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/glasses.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1179 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape/smile.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.173306 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_050.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_055.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_060.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_065.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_070.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_075.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_080.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_085.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_090.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_095.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_100.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_105.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_110.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_115.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_120.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_125.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_130.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_135.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_140.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_145.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1892 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.173306 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      988 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice/slide.odp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.173306 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)     1886 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/something.odt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.173306 stepup_reprep-1.1.1/tests/cases/convert_markdown/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/demo.md
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      976 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_markdown/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.177306 stepup_reprep-1.1.1/tests/cases/convert_mutool/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/example.pdf
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_mutool/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.177306 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/doc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      963 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/convert_weasyprint/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.177306 stepup_reprep-1.1.1/tests/cases/latex_diff/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      904 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/new.tex
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/old.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_diff/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.181306 stepup_reprep-1.1.1/tests/cases/latex_flat/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/article_structured.tex
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_article.tex
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_graph_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_graph_02.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_stdout_01.txt
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/expected_stdout_02.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1117 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/part1.tex
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/part2.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/plan_01.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/plan_02.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.181306 stepup_reprep-1.1.1/tests/cases/latex_flat/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat/sub/original.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.181306 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/expected_article.tex
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      724 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.181306 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/sub/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/sub/article_structured.tex
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/sub/part1.tex
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/sub/part2.tex
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/lualatex_simple/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1103 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/lualatex_simple/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/make_manifest_in/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/hello.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      685 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      187 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/sub/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/sub/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/sub/hello.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.185306 stepup_reprep-1.1.1/tests/cases/make_manifest_list/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      634 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/make_manifest_list/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.189306 stepup_reprep-1.1.1/tests/cases/nup_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/nup_pdf/src.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.189306 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1071 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/paper.bbl
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.189306 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/bibsane.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1350 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/pdflatex_input/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/pdflatex_input/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/raster_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1004 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/raster_pdf/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/render_basic/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      696 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/template.md
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_basic/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/render_relpath/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      931 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.193306 stepup_reprep-1.1.1/tests/cases/render_relpath/static/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/static/main.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/static/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/static/preamble.inc.tex
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/static/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/render_relpath/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.197306 stepup_reprep-1.1.1/tests/cases/tile_pdf/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    15801 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/expected_stdout.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/hexagon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/horizontal.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1373 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/pentagon.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/square.svg
--rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/triangle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/vera.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/tile_pdf/vertical.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.197306 stepup_reprep-1.1.1/tests/cases/xelatex_input/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1217 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/main.sh
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/paper.tex
--rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/xelatex_input/smile.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 17:50:13.201306 stepup_reprep-1.1.1/tests/cases/zip_manifest/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/expected_graph.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/expected_stdout.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      994 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/main.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/cases/zip_manifest/static.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/reprep_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_bibtex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_latex_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_latex_flat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_latex_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-07 17:50:09.000000 stepup_reprep-1.1.1/tests/test_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.563519 stepup_reprep-1.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.571519 stepup_reprep-1.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.github/workflows/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3167 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.571519 stepup_reprep-1.1.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/advanced_topics/
+-rw-r--r--   0 runner    (1001) docker     (127)     6818 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/good_practices.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/manifest_files.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    22692 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/figure.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/hexagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      114 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      278 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/square.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      413 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/clean_stdout.sed
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/development.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/from_scratch/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_scratch/introduction.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/from_template/
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_template/before_you_begin.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_template/create_or_clone_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_template/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/from_template/working_on_a_project.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.575519 stepup_reprep-1.1.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/reference/stepup.reprep.api.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/docs/reference/stepup.reprep.tile_pdf.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.567519 stepup_reprep-1.1.2/stepup/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.579519 stepup_reprep-1.1.2/stepup/reprep/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/add_notes_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25407 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/check_hrefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/check_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/convert_inkscape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/convert_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/latex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/make_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/normalize_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/nup_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/raster_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/tile_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/stepup/reprep/zip_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/stepup_reprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12175 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 11:29:58.000000 stepup_reprep-1.1.2/stepup_reprep.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.583519 stepup_reprep-1.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.571519 stepup_reprep-1.1.2/tests/cases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.583519 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/notes.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      182 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/add_notes_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.583519 stepup_reprep-1.1.2/tests/cases/cat_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/doc1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/doc2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/cat_pdf/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.587519 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      178 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_html/test.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.587519 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      749 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_md/test.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.587519 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/check_hrefs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      881 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      202 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.591519 stepup_reprep-1.1.2/tests/cases/convert_inkscape/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3106 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/glasses.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1332 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      244 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape/smile.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.595519 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_050.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_055.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_060.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_065.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_070.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_075.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_080.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_085.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_090.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_095.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_100.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_105.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_110.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_115.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_120.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_125.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_130.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6355 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_135.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_140.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_145.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2045 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      163 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.595519 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1141 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      153 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice/slide.odp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.595519 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2039 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10286 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/something.odt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.599519 stepup_reprep-1.1.2/tests/cases/convert_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/demo.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1129 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      151 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_markdown/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.599519 stepup_reprep-1.1.2/tests/cases/convert_mutool/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/example.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1110 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_mutool/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.599519 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1116 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/convert_weasyprint/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.603519 stepup_reprep-1.1.2/tests/cases/latex_diff/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1057 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/new.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/old.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      173 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_diff/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.603519 stepup_reprep-1.1.2/tests/cases/latex_flat/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_graph_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_graph_02.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_stdout_01.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/expected_stdout_02.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1423 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/part2.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/plan_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      249 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/plan_02.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.603519 stepup_reprep-1.1.2/tests/cases/latex_flat/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat/sub/original.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.603519 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/expected_article.tex
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      877 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      238 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.607519 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/sub/article_structured.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/sub/part1.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/sub/part2.tex
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.607519 stepup_reprep-1.1.2/tests/cases/lualatex_simple/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1256 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      134 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/lualatex_simple/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.607519 stepup_reprep-1.1.2/tests/cases/make_manifest_in/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/hello.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      787 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.611519 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      838 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      187 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.611519 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/sub/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/sub/hello.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.611519 stepup_reprep-1.1.2/tests/cases/make_manifest_list/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      787 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      166 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/make_manifest_list/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.611519 stepup_reprep-1.1.2/tests/cases/nup_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1078 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9122 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/nup_pdf/src.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.615519 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/paper.bbl
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      172 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.615519 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/bibsane.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1503 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.615519 stepup_reprep-1.1.2/tests/cases/pdflatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1269 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      224 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/pdflatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.619520 stepup_reprep-1.1.2/tests/cases/raster_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1157 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      181 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/raster_pdf/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.619520 stepup_reprep-1.1.2/tests/cases/render_basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      849 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      188 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_basic/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.619520 stepup_reprep-1.1.2/tests/cases/render_relpath/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     9195 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1084 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      270 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.619520 stepup_reprep-1.1.2/tests/cases/render_relpath/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/static/main.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      213 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/static/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/static/preamble.inc.tex
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/static/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/render_relpath/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.623520 stepup_reprep-1.1.2/tests/cases/tile_pdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15675 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/expected_stdout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/hexagon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/horizontal.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1526 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/pentagon.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      227 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/square.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      674 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/triangle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/vera.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/tile_pdf/vertical.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.623520 stepup_reprep-1.1.2/tests/cases/xelatex_input/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     6384 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1370 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/main.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/paper.tex
+-rwxr-xr-x   0 runner    (1001) docker     (127)      348 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/xelatex_input/smile.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:29:58.627519 stepup_reprep-1.1.2/tests/cases/zip_manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/expected_graph.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/expected_stdout.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1147 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/main.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      290 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/cases/zip_manifest/static.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/reprep_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_bibtex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_latex_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_latex_flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_latex_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-16 11:29:54.000000 stepup_reprep-1.1.2/tests/test_zip.py
```

### Comparing `stepup_reprep-1.1.1/.github/workflows/release.yaml` & `stepup_reprep-1.1.2/.github/workflows/release.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 name: release
 
 on: push
 
+env:
+  # This is not critical
+  # It is used only for showing URLs in GitHub Actions web interface.
+  PYPI_NAME: stepup-reprep
+
 jobs:
   build:
     name: Build distribution
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v4
@@ -18,34 +23,34 @@
     - name: Install pypa/build
       run: >-
         python -m pip install build
     - name: Build package
       run: >-
         python -m build
     - name: Store the distribution packages
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
 
   publish-to-pypi:
     name: Publish Python distribution to PyPI
     if: startsWith(github.ref, 'refs/tags/')  # only publish to PyPI on tag pushes
     needs:
     - build
     runs-on: ubuntu-latest
     environment:
       name: pypi
-      url: https://pypi.org/p/stepup-reprep
+      url: https://pypi.org/p/${{ env.PYPI_NAME }}
     permissions:
       id-token: write
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
 
   github-release:
@@ -58,20 +63,20 @@
 
     permissions:
       contents: write
       id-token: write
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Sign the dists with Sigstore
-      uses: sigstore/gh-action-sigstore-python@v1.2.3
+      uses: sigstore/gh-action-sigstore-python@v2
       with:
         inputs: >-
           ./dist/*.tar.gz
           ./dist/*.whl
     - name: Create GitHub Release
       env:
         GITHUB_TOKEN: ${{ github.token }}
@@ -96,22 +101,22 @@
     if: ${{ github.ref == 'refs/heads/main' &&  github.repository_owner == 'reproducible-reporting'}}
     needs:
     - build
     runs-on: ubuntu-latest
 
     environment:
       name: testpypi
-      url: https://test.pypi.org/p/stepup-reprep
+      url: https://test.pypi.org/p/${{ env.PYPI_NAME }}
 
     permissions:
       id-token: write
 
     steps:
     - name: Download all the dists
-      uses: actions/download-artifact@v3
+      uses: actions/download-artifact@v4
       with:
         name: python-package-distributions
         path: dist/
     - name: Publish distribution to TestPyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         repository-url: https://test.pypi.org/legacy/
```

### Comparing `stepup_reprep-1.1.1/.pre-commit-config.yaml` & `stepup_reprep-1.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/LICENSE` & `stepup_reprep-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/PKG-INFO` & `stepup_reprep-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.1.1
+Version: 1.1.2
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
 Requires-Dist: markdown_katex
 Requires-Dist: numpy
 Requires-Dist: path
 Requires-Dist: pymupdf
 Requires-Dist: pyyaml
 Requires-Dist: scipy
 Requires-Dist: setuptools
-Requires-Dist: stepup>=1.2.0
+Requires-Dist: stepup>=1.2.2
 Requires-Dist: weasyprint
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `stepup_reprep-1.1.1/README.md` & `stepup_reprep-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/advanced_topics/good_practices.md` & `stepup_reprep-1.1.2/docs/advanced_topics/good_practices.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/advanced_topics/manifest_files.md` & `stepup_reprep-1.1.2/docs/advanced_topics/manifest_files.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/figure.png` & `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/figure.png`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/hexagon.svg` & `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/pentagon.svg` & `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/square.svg` & `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/stdout.txt` & `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs/triangle.svg` & `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/advanced_topics/tiling_pdfs.md` & `stepup_reprep-1.1.2/docs/advanced_topics/tiling_pdfs.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/changelog.md` & `stepup_reprep-1.1.2/docs/changelog.md`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [1.1.2] - 2024-05-16
+
+### Fixed
+
+- Nicer fix for concurrent Inkscape SVG to PDF or PNG conversion
+  (with `SELF_CALL=x`).
+  See: https://gitlab.com/inkscape/inkscape/-/issues/4716
+- Make unit tests work with stepup-core 1.2.2.
+
+
 ## [1.1.1] - 2024-05-07
 
 ### Fixed
 
 - Inkscape SVG to PDF or PNG conversion now works also in parallel,
   thanks to the workaround posted here:
   https://gitlab.com/inkscape/inkscape/-/issues/4716
```

### Comparing `stepup_reprep-1.1.1/docs/development.md` & `stepup_reprep-1.1.2/docs/development.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,12 +33,13 @@
 (Keep this running.)
 Then open the live preview in your browser: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
 and edit Markdown files in your IDE.
 
 Please, use [Semantic Line Breaks](https://sembr.org/)
 because it results in cleaner file diffs when editing documentation.
 
-## How to Make A Release
+
+## How to Make a Release
 
 - Mark the release in `changelog.md`.
 - Make a new commit and tag it with `vX.Y.Z`.
 - Trigger the PyPI GitHub Action: `git push origin main --tags`.
```

### Comparing `stepup_reprep-1.1.1/docs/from_template/before_you_begin.md` & `stepup_reprep-1.1.2/docs/from_template/before_you_begin.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/from_template/create_or_clone_a_project.md` & `stepup_reprep-1.1.2/docs/from_template/create_or_clone_a_project.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/from_template/introduction.md` & `stepup_reprep-1.1.2/docs/from_template/introduction.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/from_template/working_on_a_project.md` & `stepup_reprep-1.1.2/docs/from_template/working_on_a_project.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/index.md` & `stepup_reprep-1.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/installation.md` & `stepup_reprep-1.1.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/docs/license.md` & `stepup_reprep-1.1.2/docs/license.md`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/mkdocs.yml` & `stepup_reprep-1.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/pyproject.toml` & `stepup_reprep-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "markdown_katex",
     "numpy",
     "path",
     "pymupdf",
     "pyyaml",
     "scipy",
     "setuptools",
-    "stepup>=1.2.0",
+    "stepup>=1.2.2",
     "weasyprint",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `stepup_reprep-1.1.1/stepup/reprep/__init__.py` & `stepup_reprep-1.1.2/stepup/reprep/__init__.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/add_notes_pdf.py` & `stepup_reprep-1.1.2/stepup/reprep/add_notes_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/api.py` & `stepup_reprep-1.1.2/stepup/reprep/api.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/bibtex_log.py` & `stepup_reprep-1.1.2/stepup/reprep/bibtex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/check_hrefs.py` & `stepup_reprep-1.1.2/stepup/reprep/check_hrefs.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/check_manifest.py` & `stepup_reprep-1.1.2/stepup/reprep/check_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/convert_inkscape.py` & `stepup_reprep-1.1.2/stepup/reprep/convert_inkscape.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 def convert_svg_pdf(
     path_svg: str, path_out: Path, inkscape: str, inkscape_args: str, optional: bool
 ):
     inp_paths = search_svg_deps(path_svg)
     ffmt = path_out.suffix[1:]
     step(
-        f"unshare --user {inkscape} {path_svg} {inkscape_args} "
+        f"SELF_CALL=x {inkscape} {path_svg} {inkscape_args} "
         f"--export-filename={path_out} --export-type={ffmt}",
         inp=[path_svg, *inp_paths],
         out=path_out,
         optional=optional,
     )
```

### Comparing `stepup_reprep-1.1.1/stepup/reprep/convert_markdown.py` & `stepup_reprep-1.1.2/stepup/reprep/convert_markdown.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/latex.py` & `stepup_reprep-1.1.2/stepup/reprep/latex.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/latex_deps.py` & `stepup_reprep-1.1.2/stepup/reprep/latex_deps.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/latex_flat.py` & `stepup_reprep-1.1.2/stepup/reprep/latex_flat.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/latex_log.py` & `stepup_reprep-1.1.2/stepup/reprep/latex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/make_manifest.py` & `stepup_reprep-1.1.2/stepup/reprep/make_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/normalize_pdf.py` & `stepup_reprep-1.1.2/stepup/reprep/normalize_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/nup_pdf.py` & `stepup_reprep-1.1.2/stepup/reprep/nup_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/pytest.py` & `stepup_reprep-1.1.2/stepup/reprep/pytest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/raster_pdf.py` & `stepup_reprep-1.1.2/stepup/reprep/raster_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/render.py` & `stepup_reprep-1.1.2/stepup/reprep/render.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/tile_pdf.py` & `stepup_reprep-1.1.2/stepup/reprep/tile_pdf.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup/reprep/zip_manifest.py` & `stepup_reprep-1.1.2/stepup/reprep/zip_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/stepup_reprep.egg-info/PKG-INFO` & `stepup_reprep-1.1.2/stepup_reprep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stepup-reprep
-Version: 1.1.1
+Version: 1.1.2
 Summary: StepUp RepRep is the StepUp extension for Reproducible Reporting
 Author-email: Toon Verstraelen <toon.verstraelen@ugent.be>
 Project-URL: Documentation, https://reproducible-reporting.github.io/stepup-reprep/
 Project-URL: Issues, https://github.com/reproducible-reporting/stepup-reprep/issues
 Project-URL: Source, https://github.com/reproducible-reporting/stepup-reprep/
 Project-URL: Changelog, https://reproducible-reporting.github.io/stepup-reprep/changelog/
 Classifier: Environment :: Console
@@ -25,15 +25,15 @@
 Requires-Dist: markdown_katex
 Requires-Dist: numpy
 Requires-Dist: path
 Requires-Dist: pymupdf
 Requires-Dist: pyyaml
 Requires-Dist: scipy
 Requires-Dist: setuptools
-Requires-Dist: stepup>=1.2.0
+Requires-Dist: stepup>=1.2.2
 Requires-Dist: weasyprint
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
```

### Comparing `stepup_reprep-1.1.1/stepup_reprep.egg-info/SOURCES.txt` & `stepup_reprep-1.1.2/stepup_reprep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/main.sh` & `stepup_reprep-1.1.2/tests/cases/nup_pdf/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
@@ -22,16 +27,15 @@
 watch_delete("dst.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["dst.pdf", "dst1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f src.pdf ]] || exit -1
-[[ -f notes.pdf ]] || exit -1
 [[ -f dst.pdf ]] || exit -1
 [[ -f dst1.pdf ]] || exit -1
 [[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/notes.pdf` & `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/notes.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/add_notes_pdf/src.pdf` & `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/cat_pdf/doc1.pdf` & `stepup_reprep-1.1.2/tests/cases/cat_pdf/doc1.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/cat_pdf/doc2.pdf` & `stepup_reprep-1.1.2/tests/cases/cat_pdf/doc2.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/cat_pdf/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/cat_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/cat_pdf/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/cat_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/cat_pdf/main.sh` & `stepup_reprep-1.1.2/tests/cases/cat_pdf/main.sh`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
@@ -22,15 +27,15 @@
 watch_delete("cat.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["cat.pdf", "cat1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f doc1.pdf ]] || exit -1
 [[ -f doc2.pdf ]] || exit -1
 [[ -f cat.pdf ]] || exit -1
 [[ -f cat1.pdf ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_html/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_html/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_html/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_html/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_html/main.sh` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_html/main.sh`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,27 @@
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f README.md ]] || exit -1
 [[ ! -f BROKEN.md ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_html/test.html` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_html/test.html`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_md/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_md/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_md/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_md/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_md/main.sh` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_md/main.sh`

 * *Files 20% similar despite different names*

```diff
@@ -3,22 +3,27 @@
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f README.md ]] || exit -1
 [[ ! -f BROKEN.md ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/main.sh` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f main.pdf ]] || exit -1
 [[ -f main.log ]] || exit -1
 [[ -f main.aux ]] || exit -1
 [[ -f README.md ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/check_hrefs_pdf/main.tex` & `stepup_reprep-1.1.2/tests/cases/check_hrefs_pdf/main.tex`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape/expected_graph.txt`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,18 @@
           created by   root:
             supplies   file:final.pdf
             supplies   file:glasses.png
             supplies   file:glasses.svg
             supplies   file:plan.py
             supplies   file:smile.svg
             supplies   step:./plan.py
+            supplies   step:SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+            supplies   step:SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
             supplies   step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
-            supplies   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-            supplies   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
           created by   root:
             consumes   file:./
@@ -39,76 +39,76 @@
              creates   step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
 
 file:glasses.svg
                 path = glasses.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
             supplies   step:python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
-            supplies   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
 
 file:smile.svg
                 path = smile.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
-            supplies   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PNG_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:glasses.svg
-             creates   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+             creates   step:SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
 
 step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape smile.svg final.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:smile.svg
-             creates   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+             creates   step:SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
 
-step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+step:SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
              workdir = ./
-             command = unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+             command = SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
                state = SUCCEEDED
            mandatory = IMPLIED
           created by   step:python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
             consumes   file:./
             consumes   file:glasses.svg
              creates   file:glasses.png
             supplies   file:glasses.png
 
 file:glasses.png
                 path = glasses.png
                state = BUILT
-          created by   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+          created by   step:SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
             consumes   file:./
-            consumes   step:unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-            supplies   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+            consumes   step:SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+            supplies   step:SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
 
-step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+step:SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
              workdir = ./
-             command = unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+             command = SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
                state = SUCCEEDED
           created by   step:python -m stepup.reprep.convert_inkscape smile.svg final.pdf
             consumes   file:./
             consumes   file:glasses.png
             consumes   file:smile.svg
              creates   file:final.pdf
             supplies   file:final.pdf
 
 file:final.pdf
                 path = final.pdf
                state = BUILT
-          created by   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+          created by   step:SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+            consumes   step:SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
```

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape/expected_stdout.txt`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,24 @@
      PHASE │ run
      START │ ./plan.py
    SUCCESS │ ./plan.py
      START │ python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
    SUCCESS │ python -m stepup.reprep.convert_inkscape glasses.svg glasses.png --optional
      START │ python -m stepup.reprep.convert_inkscape smile.svg final.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape smile.svg final.pdf
-     START │ unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-   SUCCESS │ unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-     START │ unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
-   SUCCESS │ unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+     START │ SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+   SUCCESS │ SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+     START │ SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+   SUCCESS │ SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ final.pdf
    DELETED │ glasses.png
      PHASE │ run
-     START │ unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-   SUCCESS │ unshare --user inkscape glasses.svg  --export-filename=glasses.png --export-type=png
-     START │ unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
-   SUCCESS │ unshare --user inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+     START │ SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+   SUCCESS │ SELF_CALL=x inkscape glasses.svg  --export-filename=glasses.png --export-type=png
+     START │ SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
+   SUCCESS │ SELF_CALL=x inkscape smile.svg  --export-filename=final.pdf --export-type=pdf
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
   DIRECTOR │ Stopping workers.
   DIRECTOR │ See you!
```

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape/glasses.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape/glasses.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape/main.sh` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/main.sh`

 * *Files 23% similar despite different names*

```diff
@@ -2,40 +2,53 @@
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
+export PUBLIC="public/"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-mv final.pdf final1.pdf
-mv glasses.png glasses1.png
+mv figure.pdf figure1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_delete("final.pdf")
-watch_delete("glasses.png")
+watch_delete("figure.pdf")
 run()
 join()
-write_manifest("reproducibility_png_manifest.txt", ["glasses.png", "glasses1.png"])
-write_manifest("reproducibility_pdf_manifest.txt", ["final.pdf", "final1.pdf"])
+write_manifest("reproducibility_manifest.txt", ["figure.pdf", "figure1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f smile.svg ]] || exit -1
-[[ -f final.pdf ]] || exit -1
-[[ -f final1.pdf ]] || exit -1
-[[ -f reproducibility_pdf_manifest.txt ]] || exit -1
-[[ -f reproducibility_png_manifest.txt ]] || exit -1
+[[ -f triangle.svg ]] || exit -1
+[[ -f square.svg ]] || exit -1
+[[ -f pentagon.svg ]] || exit -1
+[[ -f hexagon.svg ]] || exit -1
+[[ -f vertical.svg ]] || exit -1
+[[ -f horizontal.svg ]] || exit -1
+[[ -f triangle.pdf ]] || exit -1
+[[ -f square.pdf ]] || exit -1
+[[ -f pentagon.pdf ]] || exit -1
+[[ -f hexagon.pdf ]] || exit -1
+[[ -f vertical.pdf ]] || exit -1
+[[ -f horizontal.pdf ]] || exit -1
+[[ -f figure.pdf ]] || exit -1
+[[ -f figure1.pdf ]] || exit -1
+[[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape/smile.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape/smile.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_050.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_050.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_055.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_055.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_060.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_060.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_065.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_065.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_070.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_070.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_075.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_075.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_080.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_080.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_085.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_085.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_090.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_090.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_095.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_095.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_100.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_100.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_105.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_105.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_110.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_110.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_115.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_115.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_120.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_120.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_125.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_125.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_130.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_130.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_135.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_135.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_140.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_140.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/dots_145.svg` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/dots_145.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_inkscape_concurrency/main.sh` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape_concurrency/main.sh`

 * *Files 13% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
 stepup -w 20 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f dots_050.svg ]] || exit -1
 [[ -f dots_055.svg ]] || exit -1
 [[ -f dots_060.svg ]] || exit -1
 [[ -f dots_065.svg ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_libreoffice/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/convert_libreoffice/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_libreoffice/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/convert_libreoffice/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_libreoffice/main.sh` & `stepup_reprep-1.1.2/tests/cases/latex_diff/main.sh`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-mv slide.pdf slide1.pdf
+mv diff.tex diff1.tex
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_delete("slide.pdf")
+watch_delete("diff.tex")
 run()
 join()
-write_manifest("reproducibility_manifest_skip.txt", ["slide.pdf", "slide1.pdf"])
+write_manifest("reproducibility_manifest.txt", ["diff.tex", "diff1.tex"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f slide.odp ]] || exit -1
-[[ -f slide.pdf ]] || exit -1
-[[ -f slide1.pdf ]] || exit -1
-[[ -f reproducibility_manifest_skip.txt ]] || exit -1
+[[ -f diff.tex ]] || exit -1
+[[ -f diff1.tex ]] || exit -1
+[[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_libreoffice/slide.odp` & `stepup_reprep-1.1.2/tests/cases/convert_libreoffice/slide.odp`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/main.sh` & `stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
 stepup -w 20 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f something.odt ]] || exit -1
 [[ -f copy_00.odt ]] || exit -1
 [[ -f copy_01.odt ]] || exit -1
 [[ -f copy_02.odt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_libreoffice_concurrency/something.odt` & `stepup_reprep-1.1.2/tests/cases/convert_libreoffice_concurrency/something.odt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_markdown/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/convert_markdown/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_markdown/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/convert_markdown/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_markdown/main.sh` & `stepup_reprep-1.1.2/tests/cases/convert_markdown/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
@@ -23,15 +28,15 @@
 watch_delete("demo.html")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["demo.html", "demo1.html"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f demo.md ]] || exit -1
 [[ -f demo.html ]] || exit -1
 [[ -f demo1.html ]] || exit -1
 [[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_mutool/example.pdf` & `stepup_reprep-1.1.2/tests/cases/convert_mutool/example.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_mutool/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/convert_mutool/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_mutool/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/convert_mutool/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_mutool/main.sh` & `stepup_reprep-1.1.2/tests/cases/convert_mutool/main.sh`

 * *Files 27% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
@@ -22,15 +27,15 @@
 watch_delete("example.png")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["example.png", "example1.png"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f example.pdf ]] || exit -1
 [[ -f example.png ]] || exit -1
 [[ -f example1.png ]] || exit -1
 [[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_weasyprint/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/convert_weasyprint/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_weasyprint/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/convert_weasyprint/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/convert_weasyprint/main.sh` & `stepup_reprep-1.1.2/tests/cases/convert_weasyprint/main.sh`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
@@ -23,15 +28,15 @@
 watch_delete("doc.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["doc.pdf", "doc1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f doc.html ]] || exit -1
 [[ -f doc.pdf ]] || exit -1
 [[ -f doc1.pdf ]] || exit -1
 [[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/latex_diff/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/latex_diff/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/latex_diff/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/latex_diff/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/latex_diff/main.sh` & `stepup_reprep-1.1.2/tests/cases/convert_libreoffice/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
+export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-mv diff.tex diff1.tex
+mv slide.pdf slide1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_delete("diff.tex")
+watch_delete("slide.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["diff.tex", "diff1.tex"])
+write_manifest("reproducibility_manifest_skip.txt", ["slide.pdf", "slide1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f diff.tex ]] || exit -1
-[[ -f diff1.tex ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f slide.odp ]] || exit -1
+[[ -f slide.pdf ]] || exit -1
+[[ -f slide1.pdf ]] || exit -1
+[[ -f reproducibility_manifest_skip.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/latex_flat/expected_graph_01.txt` & `stepup_reprep-1.1.2/tests/cases/latex_flat/expected_graph_01.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/latex_flat/expected_graph_02.txt` & `stepup_reprep-1.1.2/tests/cases/latex_flat/expected_graph_02.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/latex_flat/expected_stdout_01.txt` & `stepup_reprep-1.1.2/tests/cases/latex_flat/expected_stdout_01.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/latex_flat/main.sh` & `stepup_reprep-1.1.2/tests/cases/latex_flat/main.sh`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 cp plan_01.py plan.py
 stepup -w 1 plan.py & # > current_stdout_01.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 print("HERE")
 wait()
 graph("current_graph_01")
 join()
@@ -19,27 +24,32 @@
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f article_structured.tex ]] || exit -1
 [[ ! -f article.tex ]] || exit -1
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Add the missing file and run again
 cp plan_02.py plan.py
 cp sub/original.tex sub/other.tex
 stepup -w 1 plan.py & # > current_stdout_02.txt &
+
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph_02")
 join()
 EOD
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f article_structured.tex ]] || exit -1
 [[ -f article.tex ]] || exit -1
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
```

### Comparing `stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/latex_flat_subdir/main.sh` & `stepup_reprep-1.1.2/tests/cases/latex_flat_subdir/main.sh`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
@@ -20,8 +25,8 @@
 [[ -f sub/article_structured.tex ]] || exit -1
 [[ -f sub/part1.tex ]] || exit -1
 [[ -f sub/part2.tex ]] || exit -1
 [[ -f sub/article.tex ]] || exit -1
 cp sub/article.tex current_article.tex
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
```

### Comparing `stepup_reprep-1.1.1/tests/cases/lualatex_simple/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/lualatex_simple/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/lualatex_simple/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/lualatex_simple/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/lualatex_simple/main.sh` & `stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/main.sh`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
-export REPREP_LATEX="lualatex"
+export SOURCE_DATE_EPOCH"315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
@@ -25,15 +29,15 @@
 watch_delete("paper.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f paper.pdf ]] || exit -1
 [[ -f paper.log ]] || exit -1
 [[ -f paper.aux ]] || exit -1
 [[ -f paper1.pdf ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/make_manifest_in/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/make_manifest_in/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/make_manifest_in/main.sh` & `stepup_reprep-1.1.2/tests/cases/make_manifest_in/main.sh`

 * *Files 19% similar despite different names*

```diff
@@ -3,23 +3,28 @@
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f README.md ]] || exit -1
 [[ -f MANIFEST.txt ]] || exit -1
 mv MANIFEST.txt current_manifest.txt
```

### Comparing `stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/make_manifest_in_sub/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/make_manifest_in_sub/main.sh` & `stepup_reprep-1.1.2/tests/cases/make_manifest_list/main.sh`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f sub/hello.txt ]] || exit -1
-[[ -f sub/MANIFEST.txt ]] || exit -1
-reprep-check-manifest sub/MANIFEST.txt
-mv sub/MANIFEST.txt current_manifest.txt
+[[ -f README.md ]] || exit -1
+[[ -f MANIFEST.txt ]] || exit -1
+mv MANIFEST.txt current_manifest.txt
```

### Comparing `stepup_reprep-1.1.1/tests/cases/make_manifest_list/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/make_manifest_list/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/nup_pdf/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/nup_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/nup_pdf/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/nup_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/nup_pdf/main.sh` & `stepup_reprep-1.1.2/tests/cases/add_notes_pdf/main.sh`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,19 @@
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
@@ -22,15 +27,16 @@
 watch_delete("dst.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["dst.pdf", "dst1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f src.pdf ]] || exit -1
+[[ -f notes.pdf ]] || exit -1
 [[ -f dst.pdf ]] || exit -1
 [[ -f dst1.pdf ]] || exit -1
 [[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/nup_pdf/src.pdf` & `stepup_reprep-1.1.2/tests/cases/nup_pdf/src.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/pdflatex_bbl/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_bbl/main.sh` & `stepup_reprep-1.1.2/tests/cases/lualatex_simple/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH"315532800"
+export SOURCE_DATE_EPOCH="315532800"
+export REPREP_LATEX="lualatex"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
@@ -24,15 +30,15 @@
 watch_delete("paper.pdf")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f paper.pdf ]] || exit -1
 [[ -f paper.log ]] || exit -1
 [[ -f paper.aux ]] || exit -1
 [[ -f paper1.pdf ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/pdflatex_bibtex/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_bibtex/main.sh` & `stepup_reprep-1.1.2/tests/cases/zip_manifest/main.sh`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
-export LATEX_MAIN="paper"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux paper.log
-mv paper.pdf paper1.pdf
-mv paper.bbl paper1.bbl
+rm built.txt
+mv upload.zip upload1.zip
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_delete("paper.pdf")
-watch_delete("paper.bbl")
+watch_delete("upload.zip")
 run()
 join()
-write_manifest("reproducibility_pdf_manifest.txt", ["paper.pdf", "paper1.pdf"])
-write_manifest("reproducibility_bbl_manifest.txt", ["paper.bbl", "paper1.bbl"])
+write_manifest("reproducibility_manifest.txt", ["upload.zip", "upload1.zip"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f paper.pdf ]] || exit -1
-[[ -f paper.log ]] || exit -1
-[[ -f paper.aux ]] || exit -1
-[[ -f paper.bbl ]] || exit -1
-[[ -f paper1.pdf ]] || exit -1
-[[ -f paper1.bbl ]] || exit -1
-[[ -f reproducibility_pdf_manifest.txt ]] || exit -1
-[[ -f reproducibility_bbl_manifest.txt ]] || exit -1
-reprep-check-manifest paper.MANIFEST.txt
+[[ -f built.txt ]] || exit -1
+[[ -f MANIFEST.txt ]] || exit -1
+[[ -f upload.zip ]] || exit -1
+[[ -f upload1.zip ]] || exit -1
+[[ -f reproducibility_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_input/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/pdflatex_input/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_input/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/pdflatex_input/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_input/main.sh` & `stepup_reprep-1.1.2/tests/cases/raster_pdf/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
-export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux paper.log generated.tex
-mv paper.pdf paper1.pdf
+mv rastered/smile.pdf rastered/smile1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_delete("paper.pdf")
-watch_delete("generated.tex")
+watch_delete("rastered/smile.pdf")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
+write_manifest("reproducibility_manifest.txt", ["rastered/smile.pdf", "rastered/smile1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f paper.pdf ]] || exit -1
-[[ -f paper.log ]] || exit -1
-[[ -f paper.aux ]] || exit -1
-[[ -f paper1.pdf ]] || exit -1
+[[ -f smile.pdf ]] || exit -1
+[[ -f rastered/smile.pdf ]] || exit -1
+[[ -f rastered/smile1.pdf ]] || exit -1
 [[ -f reproducibility_manifest.txt ]] || exit -1
-reprep-check-manifest paper.MANIFEST.txt
```

### Comparing `stepup_reprep-1.1.1/tests/cases/pdflatex_input/smile.pdf` & `stepup_reprep-1.1.2/tests/cases/pdflatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/raster_pdf/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/raster_pdf/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/raster_pdf/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/raster_pdf/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/raster_pdf/smile.pdf` & `stepup_reprep-1.1.2/tests/cases/raster_pdf/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/render_basic/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/render_basic/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/render_basic/main.sh` & `stepup_reprep-1.1.2/tests/cases/render_basic/main.sh`

 * *Files 12% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export ENV_VAR_TEST_STEPUP_RENDER="cool"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 join()
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f template.md ]] || exit -1
 [[ -f variables.py ]] || exit -1
 [[ -f rendered.md ]] || exit -1
 grep RepRep rendered.md
```

### Comparing `stepup_reprep-1.1.1/tests/cases/render_relpath/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/render_relpath/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/render_relpath/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/render_relpath/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/expected_graph.txt`

 * *Files 7% similar despite different names*

```diff
@@ -30,26 +30,26 @@
             supplies   file:triangle.svg
             supplies   file:vera.ttf
             supplies   file:vertical.pdf
             supplies   file:vertical.svg
             supplies   step:./plan.py
             supplies   step:./tile.py plan
             supplies   step:./tile.py run
+            supplies   step:SELF_CALL=x inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+            supplies   step:SELF_CALL=x inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+            supplies   step:SELF_CALL=x inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+            supplies   step:SELF_CALL=x inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+            supplies   step:SELF_CALL=x inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+            supplies   step:SELF_CALL=x inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape square.svg square.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
             supplies   step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
-            supplies   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
-            supplies   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
-            supplies   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
-            supplies   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
-            supplies   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
-            supplies   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
 
 step:./plan.py
              workdir = ./
              command = ./plan.py
                state = SUCCEEDED
                  ngm = ['*.svg'] {}
           created by   root:
@@ -72,122 +72,122 @@
              creates   step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
 
 file:hexagon.svg
                 path = hexagon.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:SELF_CALL=x inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
-            supplies   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
 
 file:horizontal.svg
                 path = horizontal.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:SELF_CALL=x inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
-            supplies   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
 
 file:pentagon.svg
                 path = pentagon.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:SELF_CALL=x inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
-            supplies   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
 
 file:square.svg
                 path = square.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:SELF_CALL=x inkscape square.svg  --export-filename=square.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape square.svg square.pdf
-            supplies   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
 
 file:triangle.svg
                 path = triangle.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:SELF_CALL=x inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
-            supplies   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
 
 file:vertical.svg
                 path = vertical.svg
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
+            supplies   step:SELF_CALL=x inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             supplies   step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
-            supplies   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:hexagon.svg
-             creates   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+             creates   step:SELF_CALL=x inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:horizontal.svg
-             creates   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+             creates   step:SELF_CALL=x inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:pentagon.svg
-             creates   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+             creates   step:SELF_CALL=x inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape square.svg square.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape square.svg square.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:square.svg
-             creates   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+             creates   step:SELF_CALL=x inkscape square.svg  --export-filename=square.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:triangle.svg
-             creates   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+             creates   step:SELF_CALL=x inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
 
 step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
              workdir = ./
              command = python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
                state = SUCCEEDED
    env_var (amended) = REPREP_INKSCAPE
                      = REPREP_INKSCAPE_PDF_ARGS
           created by   step:./plan.py
             consumes   file:./
             consumes   file:vertical.svg
-             creates   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+             creates   step:SELF_CALL=x inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
 
 file:tile.py
                 path = tile.py
                state = STATIC
           created by   step:./plan.py
             consumes   file:./
             supplies   step:./tile.py plan
@@ -205,120 +205,120 @@
              command = ./tile.py plan
                state = SUCCEEDED
           created by   step:./plan.py
             consumes   file:./
             consumes   file:tile.py
              creates   step:./tile.py run
 
-step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+step:SELF_CALL=x inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
              workdir = ./
-             command = unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+             command = SELF_CALL=x inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
                state = SUCCEEDED
           created by   step:python -m stepup.reprep.convert_inkscape hexagon.svg hexagon.pdf
             consumes   file:./
             consumes   file:hexagon.svg
              creates   file:hexagon.pdf
             supplies   file:hexagon.pdf
 
 file:hexagon.pdf
                 path = hexagon.pdf
                state = BUILT
-          created by   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+          created by   step:SELF_CALL=x inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+            consumes   step:SELF_CALL=x inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+step:SELF_CALL=x inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
              workdir = ./
-             command = unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+             command = SELF_CALL=x inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
                state = SUCCEEDED
           created by   step:python -m stepup.reprep.convert_inkscape horizontal.svg horizontal.pdf
             consumes   file:./
             consumes   file:horizontal.svg
              creates   file:horizontal.pdf
             supplies   file:horizontal.pdf
 
 file:horizontal.pdf
                 path = horizontal.pdf
                state = BUILT
-          created by   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+          created by   step:SELF_CALL=x inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+            consumes   step:SELF_CALL=x inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+step:SELF_CALL=x inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
              workdir = ./
-             command = unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+             command = SELF_CALL=x inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
                state = SUCCEEDED
           created by   step:python -m stepup.reprep.convert_inkscape pentagon.svg pentagon.pdf
             consumes   file:./
             consumes   file:pentagon.svg
              creates   file:pentagon.pdf
             supplies   file:pentagon.pdf
 
 file:pentagon.pdf
                 path = pentagon.pdf
                state = BUILT
-          created by   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+          created by   step:SELF_CALL=x inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+            consumes   step:SELF_CALL=x inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+step:SELF_CALL=x inkscape square.svg  --export-filename=square.pdf --export-type=pdf
              workdir = ./
-             command = unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+             command = SELF_CALL=x inkscape square.svg  --export-filename=square.pdf --export-type=pdf
                state = SUCCEEDED
           created by   step:python -m stepup.reprep.convert_inkscape square.svg square.pdf
             consumes   file:./
             consumes   file:square.svg
              creates   file:square.pdf
             supplies   file:square.pdf
 
 file:square.pdf
                 path = square.pdf
                state = BUILT
-          created by   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+          created by   step:SELF_CALL=x inkscape square.svg  --export-filename=square.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+            consumes   step:SELF_CALL=x inkscape square.svg  --export-filename=square.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+step:SELF_CALL=x inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
              workdir = ./
-             command = unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+             command = SELF_CALL=x inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
                state = SUCCEEDED
           created by   step:python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
             consumes   file:./
             consumes   file:triangle.svg
              creates   file:triangle.pdf
             supplies   file:triangle.pdf
 
 file:triangle.pdf
                 path = triangle.pdf
                state = BUILT
-          created by   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+          created by   step:SELF_CALL=x inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+            consumes   step:SELF_CALL=x inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
             supplies   step:./tile.py run
 
-step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+step:SELF_CALL=x inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
              workdir = ./
-             command = unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+             command = SELF_CALL=x inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
                state = SUCCEEDED
           created by   step:python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
             consumes   file:./
             consumes   file:vertical.svg
              creates   file:vertical.pdf
             supplies   file:vertical.pdf
 
 file:vertical.pdf
                 path = vertical.pdf
                state = BUILT
-          created by   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+          created by   step:SELF_CALL=x inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             consumes   file:./
-            consumes   step:unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+            consumes   step:SELF_CALL=x inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
             supplies   step:./tile.py run
 
 step:./tile.py run
              workdir = ./
              command = ./tile.py run
                state = SUCCEEDED
           created by   step:./tile.py plan
```

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/expected_stdout.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,26 +12,26 @@
    SUCCESS │ python -m stepup.reprep.convert_inkscape square.svg square.pdf
      START │ python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape triangle.svg triangle.pdf
      START │ python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
    SUCCESS │ python -m stepup.reprep.convert_inkscape vertical.svg vertical.pdf
      START │ ./tile.py plan
    SUCCESS │ ./tile.py plan
-     START │ unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
-   SUCCESS │ unshare --user inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
-     START │ unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
-   SUCCESS │ unshare --user inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
-     START │ unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
-   SUCCESS │ unshare --user inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
-     START │ unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
-   SUCCESS │ unshare --user inkscape square.svg  --export-filename=square.pdf --export-type=pdf
-     START │ unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
-   SUCCESS │ unshare --user inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
-     START │ unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
-   SUCCESS │ unshare --user inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+     START │ SELF_CALL=x inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+   SUCCESS │ SELF_CALL=x inkscape hexagon.svg  --export-filename=hexagon.pdf --export-type=pdf
+     START │ SELF_CALL=x inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+   SUCCESS │ SELF_CALL=x inkscape horizontal.svg  --export-filename=horizontal.pdf --export-type=pdf
+     START │ SELF_CALL=x inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+   SUCCESS │ SELF_CALL=x inkscape pentagon.svg  --export-filename=pentagon.pdf --export-type=pdf
+     START │ SELF_CALL=x inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+   SUCCESS │ SELF_CALL=x inkscape square.svg  --export-filename=square.pdf --export-type=pdf
+     START │ SELF_CALL=x inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+   SUCCESS │ SELF_CALL=x inkscape triangle.svg  --export-filename=triangle.pdf --export-type=pdf
+     START │ SELF_CALL=x inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
+   SUCCESS │ SELF_CALL=x inkscape vertical.svg  --export-filename=vertical.pdf --export-type=pdf
      START │ ./tile.py run
    SUCCESS │ ./tile.py run
   WORKFLOW │ Dumped to .stepup/workflow.mpk.xz
      PHASE │ watch
    DELETED │ figure.pdf
      PHASE │ run
      START │ ./tile.py run
```

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/hexagon.svg` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/hexagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/horizontal.svg` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/horizontal.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/pentagon.svg` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/pentagon.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/square.svg` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/square.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/tile.py` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/tile.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/triangle.svg` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/triangle.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/vera.ttf` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/vera.ttf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/tile_pdf/vertical.svg` & `stepup_reprep-1.1.2/tests/cases/tile_pdf/vertical.svg`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/xelatex_input/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/xelatex_input/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/xelatex_input/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/xelatex_input/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/xelatex_input/main.sh` & `stepup_reprep-1.1.2/tests/cases/pdflatex_input/main.sh`

 * *Files 18% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
 export SOURCE_DATE_EPOCH="315532800"
-export REPREP_LATEX="xelatex"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-rm paper.aux
-rm paper.log
-rm subdir/generated.tex
-rm subdir/code.txt
+rm paper.aux paper.log generated.tex
 mv paper.pdf paper1.pdf
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
 watch_delete("paper.pdf")
-watch_delete("subdir/generated.tex")
-watch_delete("subdir/code.txt")
+watch_delete("generated.tex")
 run()
 join()
 write_manifest("reproducibility_manifest.txt", ["paper.pdf", "paper1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
 [[ -f paper.pdf ]] || exit -1
 [[ -f paper.log ]] || exit -1
 [[ -f paper.aux ]] || exit -1
 [[ -f paper1.pdf ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/cases/xelatex_input/smile.pdf` & `stepup_reprep-1.1.2/tests/cases/xelatex_input/smile.pdf`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/zip_manifest/expected_graph.txt` & `stepup_reprep-1.1.2/tests/cases/zip_manifest/expected_graph.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/zip_manifest/expected_stdout.txt` & `stepup_reprep-1.1.2/tests/cases/zip_manifest/expected_stdout.txt`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/cases/zip_manifest/main.sh` & `stepup_reprep-1.1.2/tests/cases/convert_inkscape/main.sh`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 #!/usr/bin/env -S bash -x
 # Exit on first error and cleanup.
 set -e
 trap 'kill $(pgrep -g $$ | grep -v $$) > /dev/null 2> /dev/null || :' EXIT
 xargs rm -rvf < .gitignore
 
 # Run the example
+export SOURCE_DATE_EPOCH="315532800"
 stepup -w 1 plan.py & # > current_stdout.txt &
 
+# Wait for the director and get its socket.
+export STEPUP_DIRECTOR_SOCKET=$(
+  python -c "import stepup.core.director; print(stepup.core.director.get_socket())"
+)
+
 # Get the graph after completion of the pending steps.
 python3 - << EOD
 from stepup.core.interact import *
 wait()
 graph("current_graph")
 EOD
 
 # Reproducibility test
-rm built.txt
-mv upload.zip upload1.zip
+mv final.pdf final1.pdf
+mv glasses.png glasses1.png
 python3 - << EOD
 from stepup.core.interact import *
 from stepup.reprep.make_manifest import write_manifest
-watch_delete("upload.zip")
+watch_delete("final.pdf")
+watch_delete("glasses.png")
 run()
 join()
-write_manifest("reproducibility_manifest.txt", ["upload.zip", "upload1.zip"])
+write_manifest("reproducibility_png_manifest.txt", ["glasses.png", "glasses1.png"])
+write_manifest("reproducibility_pdf_manifest.txt", ["final.pdf", "final1.pdf"])
 EOD
 
 # Wait for background processes, if any.
-wait $(jobs -p)
+wait
 
 # Check files that are expected to be present and/or missing.
 [[ -f plan.py ]] || exit -1
-[[ -f built.txt ]] || exit -1
-[[ -f MANIFEST.txt ]] || exit -1
-[[ -f upload.zip ]] || exit -1
-[[ -f upload1.zip ]] || exit -1
-[[ -f reproducibility_manifest.txt ]] || exit -1
+[[ -f smile.svg ]] || exit -1
+[[ -f final.pdf ]] || exit -1
+[[ -f final1.pdf ]] || exit -1
+[[ -f reproducibility_pdf_manifest.txt ]] || exit -1
+[[ -f reproducibility_png_manifest.txt ]] || exit -1
```

### Comparing `stepup_reprep-1.1.1/tests/conftest.py` & `stepup_reprep-1.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/reprep_common.py` & `stepup_reprep-1.1.2/tests/reprep_common.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/test_bibtex_log.py` & `stepup_reprep-1.1.2/tests/test_bibtex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/test_cases.py` & `stepup_reprep-1.1.2/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/test_latex_deps.py` & `stepup_reprep-1.1.2/tests/test_latex_deps.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/test_latex_flat.py` & `stepup_reprep-1.1.2/tests/test_latex_flat.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/test_latex_log.py` & `stepup_reprep-1.1.2/tests/test_latex_log.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/test_manifest.py` & `stepup_reprep-1.1.2/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `stepup_reprep-1.1.1/tests/test_zip.py` & `stepup_reprep-1.1.2/tests/test_zip.py`

 * *Files identical despite different names*

