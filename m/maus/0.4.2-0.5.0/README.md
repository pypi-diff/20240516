# Comparing `tmp/maus-0.4.2.tar.gz` & `tmp/maus-0.5.0.tar.gz`

## Comparing `maus-0.4.2.tar` & `maus-0.5.0.tar`

### file list

```diff
@@ -1,81 +1,82 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 maus-0.4.2/.gitattributes
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 maus-0.4.2/.gitmodules
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 maus-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 maus-0.4.2/.readthedocs.yaml
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 maus-0.4.2/README.rst
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 maus-0.4.2/gon.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 maus-0.4.2/requirements.in
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 maus-0.4.2/requirements.txt
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 maus-0.4.2/tox.ini
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 maus-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 maus-0.4.2/.github/release-drafter.yml
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/integrationtests.yml
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/release.yml
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 maus-0.4.2/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-build_executable.in
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-build_executable.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-docs.in
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-docs.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-integration_tests.in
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-integration_tests.txt
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-json_schemas.in
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-test_packaging.in
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-test_packaging.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-unit_tests.in
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 maus-0.4.2/dev_requirements/requirements-unit_tests.txt
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 maus-0.4.2/docs/Makefile
--rw-r--r--   0        0        0     9803 2020-02-02 00:00:00.000000 maus-0.4.2/docs/conf.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 maus-0.4.2/docs/index.rst
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 maus-0.4.2/docs/make.bat
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.4.2/docs/_static/.gitkeep
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 maus-0.4.2/docs/_static/maus-favicon.png
--rw-r--r--   0        0        0    24553 2020-02-02 00:00:00.000000 maus-0.4.2/docs/_static/maus-logo.png
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 maus-0.4.2/docs/_static/maus-logo.svg
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 maus-0.4.2/docs/api/maus.models.rst
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 maus-0.4.2/docs/api/maus.reader.rst
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 maus-0.4.2/docs/api/maus.rst
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 maus-0.4.2/docs/api/modules.rst
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 maus-0.4.2/json_schemas/DeepAnwendungshandbuchSchema.json
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 maus-0.4.2/json_schemas/README.md
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 maus-0.4.2/json_schemas/generate_json_schemas.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 maus-0.4.2/src/_maus_version.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/__init__.py
--rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/cli.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/division_helper.py
--rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/edifact.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/maus_provider.py
--rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/mig_ahb_matching.py
--rw-r--r--   0        0        0    30507 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/navigation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/py.typed
--rw-r--r--   0        0        0     8967 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/transformation.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/models/__init__.py
--rw-r--r--   0        0        0    25192 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/models/anwendungshandbuch.py
--rw-r--r--   0        0        0    25221 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/models/edifact_components.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/models/message_implementation_guide.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/reader/__init__.py
--rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/reader/ahb_location_xml.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/reader/etree_element_helpers.py
--rw-r--r--   0        0        0    13735 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/reader/flat_ahb_reader.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/reader/mig_ahb_name_helpers.py
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/reader/mig_reader.py
--rw-r--r--   0        0        0    11113 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/reader/mig_xml_reader.py
--rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 maus-0.4.2/src/maus/reader/tree_to_sgh.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 maus-0.4.2/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 maus-0.4.2/LICENSE
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 maus-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 maus-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 maus-0.5.0/.gitattributes
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 maus-0.5.0/.gitmodules
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 maus-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 maus-0.5.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 maus-0.5.0/README.rst
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 maus-0.5.0/gon.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 maus-0.5.0/requirements.in
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 maus-0.5.0/requirements.txt
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 maus-0.5.0/tox.ini
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 maus-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 maus-0.5.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/integrationtests.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 maus-0.5.0/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-build_executable.in
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-build_executable.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-docs.in
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-docs.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-integration_tests.in
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-integration_tests.txt
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-json_schemas.in
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-json_schemas.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-test_packaging.in
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-test_packaging.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-unit_tests.in
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 maus-0.5.0/dev_requirements/requirements-unit_tests.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 maus-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0     9803 2020-02-02 00:00:00.000000 maus-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 maus-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 maus-0.5.0/docs/make.bat
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.5.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 maus-0.5.0/docs/_static/maus-favicon.png
+-rw-r--r--   0        0        0    24553 2020-02-02 00:00:00.000000 maus-0.5.0/docs/_static/maus-logo.png
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 maus-0.5.0/docs/_static/maus-logo.svg
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 maus-0.5.0/docs/api/maus.models.rst
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 maus-0.5.0/docs/api/maus.reader.rst
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 maus-0.5.0/docs/api/maus.rst
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 maus-0.5.0/docs/api/modules.rst
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 maus-0.5.0/json_schemas/DeepAnwendungshandbuchSchema.json
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 maus-0.5.0/json_schemas/README.md
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 maus-0.5.0/json_schemas/generate_json_schemas.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 maus-0.5.0/src/_maus_version.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/__init__.py
+-rw-r--r--   0        0        0     3874 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/cli.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/division_helper.py
+-rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/edifact.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/maus_provider.py
+-rw-r--r--   0        0        0    12090 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/mig_ahb_matching.py
+-rw-r--r--   0        0        0    30652 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/navigation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/py.typed
+-rw-r--r--   0        0        0     8992 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/transformation.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/models/__init__.py
+-rw-r--r--   0        0        0    25543 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/models/anwendungshandbuch.py
+-rw-r--r--   0        0        0    25583 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/models/edifact_components.py
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/models/message_implementation_guide.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/reader/__init__.py
+-rw-r--r--   0        0        0     4923 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/reader/ahb_location_xml.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/reader/etree_element_helpers.py
+-rw-r--r--   0        0        0    13735 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/reader/flat_ahb_reader.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/reader/mig_ahb_name_helpers.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/reader/mig_reader.py
+-rw-r--r--   0        0        0    11113 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/reader/mig_xml_reader.py
+-rw-r--r--   0        0        0     4020 2020-02-02 00:00:00.000000 maus-0.5.0/src/maus/reader/tree_to_sgh.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 maus-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 maus-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 maus-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 maus-0.5.0/PKG-INFO
```

### Comparing `maus-0.4.2/.pre-commit-config.yaml` & `maus-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.readthedocs.yaml` & `maus-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/README.rst` & `maus-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/tox.ini` & `maus-0.5.0/tox.ini`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/dependabot.yml` & `maus-0.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/workflows/codeql-analysis.yml` & `maus-0.5.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/workflows/coverage.yml` & `maus-0.5.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/workflows/dependabot_automerge.yml` & `maus-0.5.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/workflows/docs.yml` & `maus-0.5.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/workflows/formatting.yml` & `maus-0.5.0/.github/workflows/formatting.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/workflows/integrationtests.yml` & `maus-0.5.0/.github/workflows/integrationtests.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/workflows/packaging_test.yml` & `maus-0.5.0/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/workflows/pythonlint.yml` & `maus-0.5.0/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.github/workflows/release.yml` & `maus-0.5.0/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           architecture: x64
           python-version: ${{ matrix.python-version }}
-      - uses: apple-actions/import-codesign-certs@v2
+      - uses: apple-actions/import-codesign-certs@v3
         with:
           p12-file-base64: ${{ secrets.DEVELOPER_CERT_BASE64 }}
           p12-password: ${{ secrets.DEVELOPER_CERT_PW }}
         if: matrix.os == 'macos-latest'
       - name: Set up gon
         run: |
           brew tap mitchellh/gon
@@ -108,20 +108,20 @@
       - name: Repackage stapled app
         run: |
           rm -rf dist/maus_cli_macos.zip
           ditto -c -k --keepParent "dist/maus_cli_macos.app" dist/maus_cli_macos.zip
         if: matrix.os == 'macos-latest'
       - name: Generate release notes
         id: create_release_notes
-        uses: release-drafter/release-drafter@v5
+        uses: release-drafter/release-drafter@v6
         with:
           config-name: release-drafter.yml
           version: ${{ github.ref }}
           publish: true
           token: ${{ secrets.GITHUB_TOKEN }}
 
       - name: Create Release and Upload Executable
-        uses: softprops/action-gh-release@v1
+        uses: softprops/action-gh-release@v2
         with:
           body: ${{ steps.create_release_notes.outputs.body }}
           files: |
             ./dist/maus_cli_${{ runner.os == 'Windows' && 'win' || runner.os == 'macOS' && 'macos' || 'linux' }}${{ runner.os == 'Windows' && '.exe' || runner.os == 'macOS' && '' || '' }}
```

### Comparing `maus-0.4.2/.github/workflows/unittests.yml` & `maus-0.5.0/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/dev_requirements/requirements-docs.txt` & `maus-0.5.0/dev_requirements/requirements-docs.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,60 @@
+# SHA1:c8e7f810d1ef3d2747c05687c62856943f9e1faa
 #
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
+# This file is autogenerated by pip-compile-multi
+# To update, run:
 #
-#    pip-compile requirements-docs.in
+#    pip-compile-multi
 #
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
-babel==2.12.1
+babel==2.15.0
     # via sphinx
-certifi==2023.7.22
+certifi==2024.2.2
     # via requests
-charset-normalizer==3.1.0
+charset-normalizer==3.3.2
     # via requests
-docutils==0.18.1
+colorama==0.4.6
+    # via sphinx
+docutils==0.20.1
     # via
     #   sphinx
     #   sphinx-rtd-theme
-idna==3.4
+idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
-jinja2==3.1.3
+jinja2==3.1.4
     # via sphinx
-markupsafe==2.1.2
+markupsafe==2.1.5
     # via jinja2
-packaging==23.0
+packaging==24.0
     # via sphinx
-pygments==2.15.0
+pygments==2.18.0
     # via sphinx
 requests==2.31.0
     # via sphinx
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==7.2.6
+sphinx==7.3.7
     # via
-    #   -r dev_requirements/requirements-docs.in
+    #   -r dev_requirements\requirements-docs.in
     #   sphinx-rtd-theme
     #   sphinxcontrib-jquery
-    #   sphinxcontrib-serializinghtml
 sphinx-rtd-theme==2.0.0
-    # via -r dev_requirements/requirements-docs.in
-sphinxcontrib-applehelp==1.0.4
+    # via -r dev_requirements\requirements-docs.in
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.1
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
 sphinxcontrib-jquery==4.1
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.9
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-urllib3==1.26.18
+urllib3==2.2.1
     # via requests
```

### Comparing `maus-0.4.2/dev_requirements/requirements-test_packaging.txt` & `maus-0.5.0/dev_requirements/requirements-test_packaging.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,75 @@
+# SHA1:93e4fbf2b6cce1574fe3d5315360512fa9927699
 #
-# This file is autogenerated by pip-compile with Python 3.11
-# by the following command:
+# This file is autogenerated by pip-compile-multi
+# To update, run:
 #
-#    pip-compile '.\dev_requirements\requirements-test_packaging.in'
+#    pip-compile-multi
 #
-bleach==6.0.0
-    # via readme-renderer
-build==1.0.3
-    # via -r dev_requirements/requirements-test_packaging.in
-certifi==2023.7.22
+backports-tarfile==1.1.1
+    # via jaraco-context
+build==1.2.1
+    # via -r dev_requirements\requirements-test_packaging.in
+certifi==2024.2.2
     # via requests
-cffi==1.15.1
-    # via cryptography
-charset-normalizer==3.1.0
+charset-normalizer==3.3.2
     # via requests
-cryptography==41.0.6
-    # via secretstorage
-docutils==0.19
+colorama==0.4.6
+    # via build
+docutils==0.21.2
     # via readme-renderer
-idna==3.4
+idna==3.7
     # via requests
-importlib-metadata==6.1.0
+importlib-metadata==7.1.0
     # via
     #   keyring
     #   twine
-jaraco-classes==3.2.3
+jaraco-classes==3.4.0
     # via keyring
-jeepney==0.8.0
-    # via
-    #   keyring
-    #   secretstorage
-keyring==23.13.1
+jaraco-context==5.3.0
+    # via keyring
+jaraco-functools==4.0.1
+    # via keyring
+keyring==25.2.1
     # via twine
-markdown-it-py==2.2.0
+markdown-it-py==3.0.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
 more-itertools==10.2.0
-    # via jaraco-classes
-packaging==23.0
+    # via
+    #   jaraco-classes
+    #   jaraco-functools
+nh3==0.2.17
+    # via readme-renderer
+packaging==24.0
     # via build
-pkginfo==1.9.6
+pkginfo==1.10.0
     # via twine
-pycparser==2.21
-    # via cffi
-pygments==2.15.0
+pygments==2.18.0
     # via
     #   readme-renderer
     #   rich
-pyproject-hooks==1.0.0
+pyproject-hooks==1.1.0
     # via build
-readme-renderer==37.3
+pywin32-ctypes==0.2.2
+    # via keyring
+readme-renderer==43.0
     # via twine
 requests==2.31.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.3
+rich==13.7.1
     # via twine
-secretstorage==3.3.3
-    # via keyring
-six==1.16.0
-    # via bleach
-twine==4.0.2
-    # via -r dev_requirements/requirements-test_packaging.in
-urllib3==1.26.18
+twine==5.0.0
+    # via -r dev_requirements\requirements-test_packaging.in
+urllib3==2.2.1
     # via
     #   requests
     #   twine
-webencodings==0.5.1
-    # via bleach
-zipp==3.15.0
+zipp==3.18.2
     # via importlib-metadata
```

### Comparing `maus-0.4.2/docs/Makefile` & `maus-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/docs/conf.py` & `maus-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/docs/make.bat` & `maus-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/docs/_static/maus-favicon.png` & `maus-0.5.0/docs/_static/maus-favicon.png`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/docs/_static/maus-logo.png` & `maus-0.5.0/docs/_static/maus-logo.png`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/docs/_static/maus-logo.svg` & `maus-0.5.0/docs/_static/maus-logo.svg`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/docs/api/maus.models.rst` & `maus-0.5.0/docs/api/maus.models.rst`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/docs/api/maus.reader.rst` & `maus-0.5.0/docs/api/maus.reader.rst`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/docs/api/maus.rst` & `maus-0.5.0/docs/api/maus.rst`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/json_schemas/DeepAnwendungshandbuchSchema.json` & `maus-0.5.0/json_schemas/DeepAnwendungshandbuchSchema.json`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/json_schemas/README.md` & `maus-0.5.0/json_schemas/README.md`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/json_schemas/generate_json_schemas.py` & `maus-0.5.0/json_schemas/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/cli.py` & `maus-0.5.0/src/maus/cli.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/division_helper.py` & `maus-0.5.0/src/maus/division_helper.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/edifact.py` & `maus-0.5.0/src/maus/edifact.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/maus_provider.py` & `maus-0.5.0/src/maus/maus_provider.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/mig_ahb_matching.py` & `maus-0.5.0/src/maus/mig_ahb_matching.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/navigation.py` & `maus-0.5.0/src/maus/navigation.py`

 * *Files 0% similar despite different names*

```diff
@@ -642,16 +642,20 @@
                 )
             )
             continue
         if change == _DifferentialAhbLineHierarchyChange.LEAVE_TO_PARENT_AND_DIVE_INTO_SUB_GROUP:
             # [SG2 (NAD+MS), SG3]->[SG2 (NAD+MR)] # one group up (leave SG3, then remove old SG2)
             # [SG4, SG8, SG10]-> [SG4,SG12] # two groups up! (leave SG10, leave SG8, then enter sg12)
             common_ancestor = _find_common_ancestor_from_sgh(
-                last(last(result)[1].layers).segment_group_key, this_ahb_line.segment_group_key, segment_group_hierarchy
+                # pylint:disable=unsubscriptable-object
+                last(last(result)[1].layers).segment_group_key,
+                this_ahb_line.segment_group_key,
+                segment_group_hierarchy,
             )
+            # pylint:disable=unsubscriptable-object
             distance_to_common_ancestor = calculate_distance(last(result)[1], common_ancestor)
             for _ in range(0, distance_to_common_ancestor.layers_up):
                 # actually: this should be a separate case in the differential change enum
                 layers.pop()
                 if last(layers).segment_group_key == this_ahb_line.segment_group_key:  # this removes the old SG2
                     layers.pop()
             layers.append(  # this adds the next SG2
```

### Comparing `maus-0.4.2/src/maus/transformation.py` & `maus-0.5.0/src/maus/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
         modified_application_value = application_accessor.get_value(modified_application_data, non_edi_path)
         return {modified_edi_value: modified_application_value}
 
     value_pool_mapping_tasks: List[Awaitable[Dict[str, Optional[str]]]] = [
         _get_value_pool_mapping(value_pool_entry) for value_pool_entry in data_element.value_pool
     ]
     for result in await asyncio.gather(*value_pool_mapping_tasks):
-        edi_to_non_edi_value_mapping.update(result)
+        edi_to_non_edi_value_mapping.update(result)  # type:ignore[arg-type]
     return edi_to_non_edi_value_mapping
 
 
 async def transform_all_value_pools(
     application_data_model: ApplicationData,
     deep_ahb: DeepAnwendungshandbuch,
     converter: ApplicationEdifactConverter,
```

### Comparing `maus-0.4.2/src/maus/models/__init__.py` & `maus-0.5.0/src/maus/models/__init__.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/models/anwendungshandbuch.py` & `maus-0.5.0/src/maus/models/anwendungshandbuch.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,14 +50,22 @@
     """the segment, e.g. 'IDE'"""
 
     data_element: Optional[str] = attrs.field(
         validator=attrs.validators.optional(validator=attrs.validators.instance_of(str))
     )
     """ the data element ID, e.g. '3224' """
 
+    segment_id: Optional[str] = attrs.field(
+        validator=attrs.validators.optional(validator=attrs.validators.instance_of(str)), default=None
+    )
+    """
+    the 5 digit segment id, e.g. '00003' for Nachrichten Kopfsegment
+    This is available since FV2410.
+    """
+
     value_pool_entry: Optional[str] = attrs.field(
         validator=attrs.validators.optional(attrs.validators.instance_of(str))
     )
     """ one of (possible multiple) allowed values, e.g. 'E01' or '293' """
 
     name: Optional[str] = attrs.field(validator=attrs.validators.optional(validator=attrs.validators.instance_of(str)))
     """the name, e.g. 'Meldepunkt'. It can be both the description of a field but also its meaning"""
@@ -124,14 +132,15 @@
     """
     A schema to (de-)serialize :class:`.AhbLine`
     """
 
     guid = fields.UUID(required=False, load_default=None)
     segment_group_key = fields.String(required=False, load_default=None)
     segment_code = fields.String(required=False, load_default=None)
+    segment_id = fields.String(required=False, load_default=None)
     data_element = fields.String(required=False, load_default=None)
     value_pool_entry = fields.String(required=False, load_default=None)
     name = fields.String(required=False, load_default=None)
     ahb_expression = fields.String(required=False, load_default=None)
     section_name = fields.String(required=False, load_default=None)
     index = fields.Int(required=False, load_default=None, dump_default=None)
```

### Comparing `maus-0.4.2/src/maus/models/edifact_components.py` & `maus-0.5.0/src/maus/models/edifact_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -407,14 +407,21 @@
         validator=attrs.validators.optional(attrs.validators.instance_of(str)), default=None
     )
     """
     For the MIG matching it might be necessary to know the section in which the data element occured in the AHB.
     This might be necessary to e.g. distinguish gas and electricity fields which look the same otherwise.
     See e.g. UTILMD 'Geplante Turnusablesung des MSB (Strom)' vs. 'Geplante Turnusablesung des NB (Gas)'
     """
+    segment_id: Optional[str] = attrs.field(
+        validator=attrs.validators.optional(attrs.validators.matches_re(r"^\d{5}$")), default=None
+    )
+    """
+    The 5 digit segment id, e.g. '00522' for UTILMD Strom SG12, NAD "Korrespondenzanschrift des
+    Kunden des Lieferanten"
+    """
 
     def get_all_value_pools(self) -> List[DataElementValuePool]:
         """
         find all value pools in this segment
         :return: a list of all value pools
         """
         return [de for de in self.data_elements if isinstance(de, DataElementValuePool)]
@@ -423,14 +430,15 @@
 class SegmentSchema(SegmentLevelSchema):
     """
     A Schema to serialize Segments
     """
 
     data_elements = fields.List(fields.Nested(_FreeTextOrValuePoolSchema))
     section_name = fields.String(required=False)
+    segment_id = fields.String(required=False, allow_none=True)
 
     # pylint:disable=unused-argument
     @post_load
     def deserialize(self, data, **kwargs) -> Segment:
         """
         Converts the barely typed data dictionary into an actual :class:`.Segment`
         """
```

### Comparing `maus-0.4.2/src/maus/models/message_implementation_guide.py` & `maus-0.5.0/src/maus/models/message_implementation_guide.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/reader/ahb_location_xml.py` & `maus-0.5.0/src/maus/reader/ahb_location_xml.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/reader/etree_element_helpers.py` & `maus-0.5.0/src/maus/reader/etree_element_helpers.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/reader/flat_ahb_reader.py` & `maus-0.5.0/src/maus/reader/flat_ahb_reader.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/reader/mig_ahb_name_helpers.py` & `maus-0.5.0/src/maus/reader/mig_ahb_name_helpers.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/reader/mig_reader.py` & `maus-0.5.0/src/maus/reader/mig_reader.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/reader/mig_xml_reader.py` & `maus-0.5.0/src/maus/reader/mig_xml_reader.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/src/maus/reader/tree_to_sgh.py` & `maus-0.5.0/src/maus/reader/tree_to_sgh.py`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/.gitignore` & `maus-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/LICENSE` & `maus-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/pyproject.toml` & `maus-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maus-0.4.2/PKG-INFO` & `maus-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: maus
-Version: 0.4.2
+Version: 0.5.0
 Summary: Python Library that consolidates Anwendungshandbücher (AHB) and Message Implementation Guides (MIG)
 Project-URL: Changelog, https://github.com/Hochfrequenz/mig_ahb_utility_stack/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/mig_ahb_utility_stack
 Project-URL: Documentation, https://maus.readthedocs.io/en/latest/
 Author-email: Hochfrequenz Unternehmensberatung GmbH <info@hochfrequenz.de>
 License: MIT
 License-File: LICENSE
```

