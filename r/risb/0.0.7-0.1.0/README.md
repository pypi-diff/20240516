# Comparing `tmp/risb-0.0.7.tar.gz` & `tmp/risb-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue May 14 01:44:14 2024, max compression
+gzip compressed data, last modified: Thu May 16 06:52:43 2024, max compression
```

## Comparing `risb-0.0.7.tar` & `risb-0.1.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0      202 2024-05-14 01:44:14.000000 risb-0.0.7/.dockerignore
--rw-r--r--   0        0        0      124 2024-05-14 01:44:14.000000 risb-0.0.7/.git_archival.txt
--rw-r--r--   0        0        0       98 2024-05-14 01:44:14.000000 risb-0.0.7/.gitattributes
--rw-r--r--   0        0        0     3481 2024-05-14 01:44:14.000000 risb-0.0.7/CITATION
--rw-r--r--   0        0        0      822 2024-05-14 01:44:14.000000 risb-0.0.7/COPYRIGHT
--rw-r--r--   0        0        0     1168 2024-05-14 01:44:14.000000 risb-0.0.7/TODO.md
--rw-r--r--   0        0        0       37 2024-05-14 01:44:14.000000 risb-0.0.7/.github/CODEOWNERS
--rw-r--r--   0        0        0      223 2024-05-14 01:44:14.000000 risb-0.0.7/.github/dependabot.yml
--rw-r--r--   0        0        0     3302 2024-05-14 01:44:14.000000 risb-0.0.7/.github/actions/setup-triqs/action.yml
--rw-r--r--   0        0        0     2752 2024-05-14 01:44:14.000000 risb-0.0.7/.github/workflows/cd.yml
--rw-r--r--   0        0        0     1776 2024-05-14 01:44:14.000000 risb-0.0.7/.github/workflows/ci.yml
--rw-r--r--   0        0        0      382 2024-05-14 01:44:14.000000 risb-0.0.7/docker/Dockerfile
--rw-r--r--   0        0        0     3434 2024-05-14 01:44:14.000000 risb-0.0.7/docker/Dockerfile.dev
--rw-r--r--   0        0        0      608 2024-05-14 01:44:14.000000 risb-0.0.7/docker/Dockerfile.docs
--rw-r--r--   0        0        0      567 2024-05-14 01:44:14.000000 risb-0.0.7/docker/conda.sh
--rw-r--r--   0        0        0      332 2024-05-14 01:44:14.000000 risb-0.0.7/docker/docker-compose-dev.yml
--rw-r--r--   0        0        0      334 2024-05-14 01:44:14.000000 risb-0.0.7/docker/docker-compose-docs.yml
--rw-r--r--   0        0        0      266 2024-05-14 01:44:14.000000 risb-0.0.7/docker/docker-compose.yml
--rw-r--r--   0        0        0       10 2024-05-14 01:44:14.000000 risb-0.0.7/docs/.gitignore
--rw-r--r--   0        0        0     3376 2024-05-14 01:44:14.000000 risb-0.0.7/docs/about.md
--rw-r--r--   0        0        0     2359 2024-05-14 01:44:14.000000 risb-0.0.7/docs/conf.py
--rw-r--r--   0        0        0      422 2024-05-14 01:44:14.000000 risb-0.0.7/docs/index.md
--rw-r--r--   0        0        0      111 2024-05-14 01:44:14.000000 risb-0.0.7/docs/install.md
--rw-r--r--   0        0        0     5636 2024-05-14 01:44:14.000000 risb-0.0.7/docs/explanations/embedding.md
--rw-r--r--   0        0        0      114 2024-05-14 01:44:14.000000 risb-0.0.7/docs/explanations/index.md
--rw-r--r--   0        0        0     2090 2024-05-14 01:44:14.000000 risb-0.0.7/docs/explanations/kweight.md
--rw-r--r--   0        0        0     3176 2024-05-14 01:44:14.000000 risb-0.0.7/docs/explanations/projectors.md
--rw-r--r--   0        0        0     2426 2024-05-14 01:44:14.000000 risb-0.0.7/docs/how-to/diis.md
--rw-r--r--   0        0        0     5629 2024-05-14 01:44:14.000000 risb-0.0.7/docs/how-to/embedding.md
--rw-r--r--   0        0        0      119 2024-05-14 01:44:14.000000 risb-0.0.7/docs/how-to/index.md
--rw-r--r--   0        0        0     2520 2024-05-14 01:44:14.000000 risb-0.0.7/docs/how-to/kweight.md
--rw-r--r--   0        0        0     7176 2024-05-14 01:44:14.000000 risb-0.0.7/docs/how-to/lattice_solver.md
--rw-r--r--   0        0        0     4622 2024-05-14 01:44:14.000000 risb-0.0.7/docs/how-to/projectors.md
--rw-r--r--   0        0        0     9168 2024-05-14 01:44:14.000000 risb-0.0.7/docs/how-to/quadratic_terms.md
--rw-r--r--   0        0        0    13537 2024-05-14 01:44:14.000000 risb-0.0.7/docs/tutorials/hubbard.md
--rw-r--r--   0        0        0       77 2024-05-14 01:44:14.000000 risb-0.0.7/docs/tutorials/index.md
--rw-r--r--   0        0        0     1977 2024-05-14 01:44:14.000000 risb-0.0.7/docs/tutorials/kagome.md
--rw-r--r--   0        0        0    19265 2024-05-14 01:44:14.000000 risb-0.0.7/docs/tutorials/self-consistent.md
--rw-r--r--   0        0        0     3407 2024-05-14 01:44:14.000000 risb-0.0.7/examples/bilayer_hubbard.py
--rw-r--r--   0        0        0     7530 2024-05-14 01:44:14.000000 risb-0.0.7/examples/decorated_honeycomb.py
--rw-r--r--   0        0        0     4422 2024-05-14 01:44:14.000000 risb-0.0.7/examples/hubbard.py
--rw-r--r--   0        0        0     4881 2024-05-14 01:44:14.000000 risb-0.0.7/examples/kagome_hubbard.py
--rw-r--r--   0        0        0      206 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/__init__.py
--rw-r--r--   0        0        0    17127 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/helpers.py
--rw-r--r--   0        0        0     8233 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/helpers_triqs.py
--rw-r--r--   0        0        0    27703 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/solve_lattice.py
--rw-r--r--   0        0        0      411 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/version.py
--rw-r--r--   0        0        0       84 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/embedding/__init__.py
--rw-r--r--   0        0        0     2561 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/embedding/dummy.py
--rw-r--r--   0        0        0    12048 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/embedding/embedding_atom_diag.py
--rw-r--r--   0        0        0       36 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/kweight/__init__.py
--rw-r--r--   0        0        0     1656 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/kweight/from_triqs_hartree.py
--rw-r--r--   0        0        0     4931 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/kweight/kweight.py
--rw-r--r--   0        0        0      234 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/optimize/__init__.py
--rw-r--r--   0        0        0     2969 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/optimize/diis.py
--rw-r--r--   0        0        0      640 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/optimize/linear_mixing.py
--rw-r--r--   0        0        0     6064 2024-05-14 01:44:14.000000 risb-0.0.7/src/risb/optimize/solver_newton.py
--rw-r--r--   0        0        0     1506 2024-05-14 01:44:14.000000 risb-0.0.7/tests/common.py
--rw-r--r--   0        0        0    13056 2024-05-14 01:44:14.000000 risb-0.0.7/tests/data_helpers.h5
--rw-r--r--   0        0        0     7541 2024-05-14 01:44:14.000000 risb-0.0.7/tests/test_atomdiag.py
--rw-r--r--   0        0        0     3482 2024-05-14 01:44:14.000000 risb-0.0.7/tests/test_helpers.py
--rw-r--r--   0        0        0     6360 2024-05-14 01:44:14.000000 risb-0.0.7/tests/test_latticesolver.py
--rw-r--r--   0        0        0      230 2024-05-14 01:44:14.000000 risb-0.0.7/.gitignore
--rw-r--r--   0        0        0    35149 2024-05-14 01:44:14.000000 risb-0.0.7/LICENSE
--rw-r--r--   0        0        0     3984 2024-05-14 01:44:14.000000 risb-0.0.7/README.md
--rw-r--r--   0        0        0     1775 2024-05-14 01:44:14.000000 risb-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    45795 2024-05-14 01:44:14.000000 risb-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      202 2024-05-16 06:52:43.000000 risb-0.1.0/.dockerignore
+-rw-r--r--   0        0        0      124 2024-05-16 06:52:43.000000 risb-0.1.0/.git_archival.txt
+-rw-r--r--   0        0        0       98 2024-05-16 06:52:43.000000 risb-0.1.0/.gitattributes
+-rw-r--r--   0        0        0     3481 2024-05-16 06:52:43.000000 risb-0.1.0/CITATION
+-rw-r--r--   0        0        0      822 2024-05-16 06:52:43.000000 risb-0.1.0/COPYRIGHT
+-rw-r--r--   0        0        0     1308 2024-05-16 06:52:43.000000 risb-0.1.0/TODO.md
+-rw-r--r--   0        0        0       37 2024-05-16 06:52:43.000000 risb-0.1.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      223 2024-05-16 06:52:43.000000 risb-0.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     3302 2024-05-16 06:52:43.000000 risb-0.1.0/.github/actions/setup-triqs/action.yml
+-rw-r--r--   0        0        0     2752 2024-05-16 06:52:43.000000 risb-0.1.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1776 2024-05-16 06:52:43.000000 risb-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      382 2024-05-16 06:52:43.000000 risb-0.1.0/docker/Dockerfile
+-rw-r--r--   0        0        0     3434 2024-05-16 06:52:43.000000 risb-0.1.0/docker/Dockerfile.dev
+-rw-r--r--   0        0        0      608 2024-05-16 06:52:43.000000 risb-0.1.0/docker/Dockerfile.docs
+-rw-r--r--   0        0        0      567 2024-05-16 06:52:43.000000 risb-0.1.0/docker/conda.sh
+-rw-r--r--   0        0        0      332 2024-05-16 06:52:43.000000 risb-0.1.0/docker/docker-compose-dev.yml
+-rw-r--r--   0        0        0      334 2024-05-16 06:52:43.000000 risb-0.1.0/docker/docker-compose-docs.yml
+-rw-r--r--   0        0        0      266 2024-05-16 06:52:43.000000 risb-0.1.0/docker/docker-compose.yml
+-rw-r--r--   0        0        0       10 2024-05-16 06:52:43.000000 risb-0.1.0/docs/.gitignore
+-rw-r--r--   0        0        0     3376 2024-05-16 06:52:43.000000 risb-0.1.0/docs/about.md
+-rw-r--r--   0        0        0     2359 2024-05-16 06:52:43.000000 risb-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0      422 2024-05-16 06:52:43.000000 risb-0.1.0/docs/index.md
+-rw-r--r--   0        0        0      111 2024-05-16 06:52:43.000000 risb-0.1.0/docs/install.md
+-rw-r--r--   0        0        0     5636 2024-05-16 06:52:43.000000 risb-0.1.0/docs/explanations/embedding.md
+-rw-r--r--   0        0        0      114 2024-05-16 06:52:43.000000 risb-0.1.0/docs/explanations/index.md
+-rw-r--r--   0        0        0     2090 2024-05-16 06:52:43.000000 risb-0.1.0/docs/explanations/kweight.md
+-rw-r--r--   0        0        0     3176 2024-05-16 06:52:43.000000 risb-0.1.0/docs/explanations/projectors.md
+-rw-r--r--   0        0        0     2426 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/diis.md
+-rw-r--r--   0        0        0     5629 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/embedding.md
+-rw-r--r--   0        0        0      119 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/index.md
+-rw-r--r--   0        0        0     2520 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/kweight.md
+-rw-r--r--   0        0        0     7176 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/lattice_solver.md
+-rw-r--r--   0        0        0     4622 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/projectors.md
+-rw-r--r--   0        0        0     9168 2024-05-16 06:52:43.000000 risb-0.1.0/docs/how-to/quadratic_terms.md
+-rw-r--r--   0        0        0    13537 2024-05-16 06:52:43.000000 risb-0.1.0/docs/tutorials/hubbard.md
+-rw-r--r--   0        0        0       77 2024-05-16 06:52:43.000000 risb-0.1.0/docs/tutorials/index.md
+-rw-r--r--   0        0        0     1977 2024-05-16 06:52:43.000000 risb-0.1.0/docs/tutorials/kagome.md
+-rw-r--r--   0        0        0    19265 2024-05-16 06:52:43.000000 risb-0.1.0/docs/tutorials/self-consistent.md
+-rw-r--r--   0        0        0     4863 2024-05-16 06:52:43.000000 risb-0.1.0/examples/bilayer_hubbard.py
+-rw-r--r--   0        0        0     7530 2024-05-16 06:52:43.000000 risb-0.1.0/examples/decorated_honeycomb.py
+-rw-r--r--   0        0        0     4620 2024-05-16 06:52:43.000000 risb-0.1.0/examples/hubbard.py
+-rw-r--r--   0        0        0     4881 2024-05-16 06:52:43.000000 risb-0.1.0/examples/kagome_hubbard.py
+-rw-r--r--   0        0        0      206 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/__init__.py
+-rw-r--r--   0        0        0    17127 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/helpers.py
+-rw-r--r--   0        0        0    17730 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/helpers_triqs.py
+-rw-r--r--   0        0        0    27703 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/solve_lattice.py
+-rw-r--r--   0        0        0      411 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/version.py
+-rw-r--r--   0        0        0       84 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/embedding/__init__.py
+-rw-r--r--   0        0        0     2561 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/embedding/dummy.py
+-rw-r--r--   0        0        0    12048 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/embedding/embedding_atom_diag.py
+-rw-r--r--   0        0        0       36 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/kweight/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/kweight/from_triqs_hartree.py
+-rw-r--r--   0        0        0     4931 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/kweight/kweight.py
+-rw-r--r--   0        0        0      234 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/optimize/__init__.py
+-rw-r--r--   0        0        0     2969 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/optimize/diis.py
+-rw-r--r--   0        0        0      640 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/optimize/linear_mixing.py
+-rw-r--r--   0        0        0     6064 2024-05-16 06:52:43.000000 risb-0.1.0/src/risb/optimize/solver_newton.py
+-rw-r--r--   0        0        0     1506 2024-05-16 06:52:43.000000 risb-0.1.0/tests/common.py
+-rw-r--r--   0        0        0    13056 2024-05-16 06:52:43.000000 risb-0.1.0/tests/data_helpers.h5
+-rw-r--r--   0        0        0     7541 2024-05-16 06:52:43.000000 risb-0.1.0/tests/test_atomdiag.py
+-rw-r--r--   0        0        0     3482 2024-05-16 06:52:43.000000 risb-0.1.0/tests/test_helpers.py
+-rw-r--r--   0        0        0     6360 2024-05-16 06:52:43.000000 risb-0.1.0/tests/test_latticesolver.py
+-rw-r--r--   0        0        0      230 2024-05-16 06:52:43.000000 risb-0.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2024-05-16 06:52:43.000000 risb-0.1.0/LICENSE
+-rw-r--r--   0        0        0     3984 2024-05-16 06:52:43.000000 risb-0.1.0/README.md
+-rw-r--r--   0        0        0     1775 2024-05-16 06:52:43.000000 risb-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    45795 2024-05-16 06:52:43.000000 risb-0.1.0/PKG-INFO
```

### Comparing `risb-0.0.7/CITATION` & `risb-0.1.0/CITATION`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/COPYRIGHT` & `risb-0.1.0/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/.github/actions/setup-triqs/action.yml` & `risb-0.1.0/.github/actions/setup-triqs/action.yml`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/.github/workflows/cd.yml` & `risb-0.1.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/.github/workflows/ci.yml` & `risb-0.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docker/Dockerfile.dev` & `risb-0.1.0/docker/Dockerfile.dev`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docker/Dockerfile.docs` & `risb-0.1.0/docker/Dockerfile.docs`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docker/conda.sh` & `risb-0.1.0/docker/conda.sh`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/about.md` & `risb-0.1.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/conf.py` & `risb-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/explanations/embedding.md` & `risb-0.1.0/docs/explanations/embedding.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/explanations/kweight.md` & `risb-0.1.0/docs/explanations/kweight.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/explanations/projectors.md` & `risb-0.1.0/docs/explanations/projectors.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/how-to/diis.md` & `risb-0.1.0/docs/how-to/diis.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/how-to/embedding.md` & `risb-0.1.0/docs/how-to/embedding.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/how-to/kweight.md` & `risb-0.1.0/docs/how-to/kweight.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/how-to/lattice_solver.md` & `risb-0.1.0/docs/how-to/lattice_solver.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/how-to/projectors.md` & `risb-0.1.0/docs/how-to/projectors.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/how-to/quadratic_terms.md` & `risb-0.1.0/docs/how-to/quadratic_terms.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/tutorials/hubbard.md` & `risb-0.1.0/docs/tutorials/hubbard.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/tutorials/kagome.md` & `risb-0.1.0/docs/tutorials/kagome.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/docs/tutorials/self-consistent.md` & `risb-0.1.0/docs/tutorials/self-consistent.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/examples/decorated_honeycomb.py` & `risb-0.1.0/examples/decorated_honeycomb.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/examples/hubbard.py` & `risb-0.1.0/examples/hubbard.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 
 from triqs.lattice.tight_binding import TBLattice, BravaisLattice, BrillouinZone, MeshBrZone
 from triqs.operators import Operator, n
 from triqs.operators.util.op_struct import set_operator_structure
 from triqs.operators.util.observables import S2_op, N_op
-from triqs.gf import BlockGf, MeshImFreq, MeshProduct
+from triqs.gf import MeshImFreq, MeshProduct
 
 from risb import LatticeSolver
 from risb.kweight import SmearingKWeight
 from risb.embedding import EmbeddingAtomDiag
-from risb.helpers_triqs import get_sigma_w, get_g_qp_k_w, get_g_k_w, get_g_w_loc
+from risb.helpers_triqs import get_g0_k_w, get_sigma_w, get_g_qp_k_w, get_g_k_w, get_g_w_loc
 
 import matplotlib.pyplot as plt
 
 def hubbard(U, n_orb):
     h_int = Operator()
     for o in range(n_orb):
         h_int += U * n("up",o) * n("dn",o)
@@ -85,40 +85,43 @@
     total_spin.append( embedding.overlap(total_spin_Op) )
     Z.append(S.Z[0]['up'][0,0])
     
     if np.abs(U - 3.5) < 1e-10:
         # Some different ways to construct some Green's functions
         mu = kweight.mu
 
-        # Non-interacting lattice Green's function
+        # The k-space and frequency mesh of the problem
         iw_mesh = MeshImFreq(beta=beta, S='Fermion', n_max=64)
         k_iw_mesh = MeshProduct(mk, iw_mesh)
-        G0_k_iw = BlockGf(mesh=k_iw_mesh, gf_struct=gf_struct)
-        for bl, gf in G0_k_iw:
-            e_k = tbl.fourier(mk)
-            for k, iw in gf.mesh:
-                gf[k,iw] = 1 / (iw - e_k[k] + mu)
 
-        # Quasiparticle lattice Green's function, local self-energy, lattice Green's function
-        G_qp_k_iw = get_g_qp_k_w(gf_struct=gf_struct, mesh=k_iw_mesh, h0_kin_k=S.h0_kin_k, Lambda=S.Lambda[0], R=S.R[0], mu=mu)
-        Sigma_iw = get_sigma_w(mesh=iw_mesh, gf_struct=gf_struct, Lambda=S.Lambda[0], R=S.R[0], mu=mu)
+        mu = kweight.mu
+
+        # Gf constructed from local self-energy
+        G0_k_iw = get_g0_k_w(gf_struct=gf_struct, mesh=k_iw_mesh, h0_k=h0_k, mu=mu)
+        Sigma_iw = get_sigma_w(mesh=iw_mesh, gf_struct=gf_struct, Lambda=S.Lambda[0], R=S.R[0], h0_loc=S.h0_loc_matrix[0], mu=mu)
         G_k_iw = get_g_k_w(g0_k_w=G0_k_iw, sigma_w=Sigma_iw)
+                
+        # Gf constructed from quasiparticle Gf
+        G_qp_k_iw = get_g_qp_k_w(gf_struct=gf_struct, mesh=k_iw_mesh, h0_kin_k=S.h0_kin_k, Lambda=S.Lambda[0], R=S.R[0], mu=mu)
         G_k_iw2 = get_g_k_w(g_qp_k_w=G_qp_k_iw, R=S.R[0])
-
-        # Local Green's functions integrated over k
-        G0_iw_loc = get_g_w_loc(G0_k_iw)
+        
+        # Local Gf integrated over k
+        G0_iw_loc = get_g_w_loc(G0_k_iw) # this is using the correlated chemical potential, so will not have right filling
         G_qp_iw_loc = get_g_w_loc(G_qp_k_iw)
         G_iw_loc = get_g_w_loc(G_k_iw)
         G_iw_loc2 = get_g_w_loc(G_k_iw2)
         
         # Filling of physical electron scales with Z
-        print("G0:", G0_iw_loc.total_density().real)
-        print("G_qp:", G_qp_iw_loc.total_density().real)
-        print("G:", G_iw_loc.total_density().real)
-        print("G2:", G_iw_loc2.total_density().real)
-        print("Z:", S.Z[0]['up'][0,0])
-        print()
+        print(f"Filling G0: {G0_iw_loc.total_density().real:.4f}")
+        print(f"Filling G_qp: {G_qp_iw_loc.total_density().real:.4f}")
+        print(f"Filling G: {G_iw_loc.total_density().real:.4f}")
+        print(f"Filling G2: {G_iw_loc2.total_density().real:.4f}")
+        print(f"Filling Z:: {S.Z[0]['up'][0,0]:.4f}")
         
 fig, axis = plt.subplots(1,2)
 axis[0].plot(U_arr, Z, '-ok')
-axis[0].plot(U_arr, -0.5 + 0.5 * np.sqrt( 1 + 4*np.array(total_spin) ), '-ok')
+axis[0].set_xlabel(r'$U$')
+axis[0].set_ylabel(r'$Z$')
+axis[1].plot(U_arr, -0.5 + 0.5 * np.sqrt( 1 + 4*np.array(total_spin) ), '-ok')
+axis[1].set_xlabel(r'$U$')
+axis[1].set_ylabel(r'$\mathcal{S}$')
 plt.show()
```

### Comparing `risb-0.0.7/examples/kagome_hubbard.py` & `risb-0.1.0/examples/kagome_hubbard.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/src/risb/helpers.py` & `risb-0.1.0/src/risb/helpers.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/src/risb/solve_lattice.py` & `risb-0.1.0/src/risb/solve_lattice.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/src/risb/embedding/dummy.py` & `risb-0.1.0/src/risb/embedding/dummy.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/src/risb/embedding/embedding_atom_diag.py` & `risb-0.1.0/src/risb/embedding/embedding_atom_diag.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/src/risb/kweight/from_triqs_hartree.py` & `risb-0.1.0/src/risb/kweight/from_triqs_hartree.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/src/risb/kweight/kweight.py` & `risb-0.1.0/src/risb/kweight/kweight.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/src/risb/optimize/diis.py` & `risb-0.1.0/src/risb/optimize/diis.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/src/risb/optimize/linear_mixing.py` & `risb-0.1.0/src/risb/optimize/linear_mixing.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/src/risb/optimize/solver_newton.py` & `risb-0.1.0/src/risb/optimize/solver_newton.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/tests/common.py` & `risb-0.1.0/tests/common.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/tests/data_helpers.h5` & `risb-0.1.0/tests/data_helpers.h5`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/tests/test_atomdiag.py` & `risb-0.1.0/tests/test_atomdiag.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/tests/test_helpers.py` & `risb-0.1.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/tests/test_latticesolver.py` & `risb-0.1.0/tests/test_latticesolver.py`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/LICENSE` & `risb-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/README.md` & `risb-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/pyproject.toml` & `risb-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `risb-0.0.7/PKG-INFO` & `risb-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: risb
-Version: 0.0.7
+Version: 0.1.0
 Summary: Rotationally invariant slave boson mean-field theory.
 Project-URL: Homepage, https://github.com/thenoursehorse/risb
 Project-URL: Documentation, https://thenoursehorse.github.io/risb
 Author: H. L. Nourse
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

