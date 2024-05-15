# Comparing `tmp/bo4e-202401.1.1rc4.tar.gz` & `tmp/bo4e-202401.1.2rc14.tar.gz`

## Comparing `bo4e-202401.1.1rc4.tar` & `bo4e-202401.1.2rc14.tar`

### file list

```diff
@@ -1,346 +1,347 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.pylintrc
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/CHANGELOG.rst
--rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/MANIFEST.in
--rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/README.rst
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/bo4e_schemas_create_release.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docker-compose.yml
--rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/generate_or_validate_json_schemas.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/requirements.in
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/requirements.txt
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tox.ini
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/dependabot.yml
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0        0        0     2696 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/docs_latest.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/formatting.yml
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/linting.yml
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/python-publish-scheduled.yml
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/test_docs.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.vscode/settings.json
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-json_schemas.in
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-json_schemas.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-packaging.in
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-packaging.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/Makefile
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/authors.rst
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/changelog.rst
--rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/conf.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/index.rst
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/license.rst
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/release_workflow.rst
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/requirements.in
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/requirements.txt
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/test_uml.py
--rw-r--r--   0        0        0    28472 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/uml.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/versioning.rst
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-python-favicon.png
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-python-favicon.svg
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-python-logo.png
--rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-python-logo.svg
--rw-r--r--   0        0        0   167661 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-release-workflow.excalidraw
--rw-r--r--   0        0        0   512116 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/_static/bo4e-release-workflow.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/__init__.py
--rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/__main__.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/change_schemas.py
--rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/diff.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/loader.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/docs/compatibility/matrix.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/_bo4e_python_version.py
--rw-r--r--   0        0        0    12614 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/py.typed
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/version.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/zusatzattribut.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/__init__.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/angebot.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/ausschreibung.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/buendelvertrag.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/energiemenge.py
--rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/fremdkosten.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/geraet.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/geschaeftsobjekt.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/geschaeftspartner.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/kosten.py
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/lastgang.py
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/marktlokation.py
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/marktteilnehmer.py
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/messlokation.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/person.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblatt.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblattdienstleistung.py
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblatthardware.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblattkonzessionsabgabe.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblattmessung.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/preisblattnetznutzung.py
--rw-r--r--   0        0        0     4822 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/rechnung.py
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/region.py
--rw-r--r--   0        0        0     2067 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/regionaltarif.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/standorteigenschaften.py
--rw-r--r--   0        0        0     2235 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/tarif.py
--rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/tarifinfo.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/tarifkosten.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/tarifpreisblatt.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/vertrag.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/zaehler.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/bo/zeitreihe.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/adresse.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/angebotsposition.py
--rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/angebotsteil.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/angebotsvariante.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/aufabschlag.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagproort.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagregional.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagstaffelproort.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/ausschreibungsdetail.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/ausschreibungslos.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/betrag.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/com.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/dienstleistung.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/energieherkunft.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/energiemix.py
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/fremdkostenblock.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/fremdkostenposition.py
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/geokoordinaten.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/katasteradresse.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/kontaktweg.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/konzessionsabgabe.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/kostenblock.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/kostenposition.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/kriteriumwert.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/marktgebietinfo.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/menge.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/messlokationszuordnung.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/positionsaufabschlag.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/preis.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/preisgarantie.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/preisposition.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/preisstaffel.py
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/rechnungsposition.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionalegueltigkeit.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionalepreisgarantie.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionalepreisstaffel.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionaleraufabschlag.py
--rw-r--r--   0        0        0     1673 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionaletarifpreisposition.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/regionskriterium.py
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/sigmoidparameter.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/standorteigenschaftengas.py
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/standorteigenschaftenstrom.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/steuerbetrag.py
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifberechnungsparameter.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifeinschraenkung.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifpreis.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifpreisposition.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifpreispositionproort.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/tarifpreisstaffelproort.py
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/unterschrift.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/verbrauch.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/vertragskonditionen.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/vertragsteil.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/verwendungszweckpromarktrolle.py
--rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zaehlwerk.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zaehlzeitregister.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zeitraum.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zeitreihenwert.py
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zeitspanne.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/com/zustaendigkeit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/__init__.py
--rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/abgabeart.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/angebotsstatus.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/anrede.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/arithmetische_operation.py
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/artikelid.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/aufabschlagstyp.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/aufabschlagsziel.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/ausschreibungsportal.py
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/ausschreibungsstatus.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/ausschreibungstyp.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/bdewartikelnummer.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/befestigungsart.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/bemessungsgroesse.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/bilanzierungsmethode.py
--rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/dienstleistungstyp.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/energierichtung.py
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/erzeugungsart.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/gasqualitaet.py
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/gebiettyp.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/geraeteklasse.py
--rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/geraetetyp.py
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/geschaeftspartnerrolle.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/gueltigkeitstyp.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kalkulationsmethode.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kontaktart.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kostenklasse.py
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kundengruppe.py
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kundengruppeka.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/kundentyp.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/landescode.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/leistungstyp.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/lokationstyp.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/marktrolle.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/medium.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/mengeneinheit.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/mengenoperator.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messart.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messgroesse.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messpreistyp.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messwerterfassung.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messwertstatus.py
--rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/messwertstatuszusatz.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/netzebene.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/netznutzungrechnungsart.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/netznutzungrechnungstyp.py
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/oekolabel.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/oekozertifikat.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/organisationstyp.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/preisgarantietyp.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/preismodell.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/preisstatus.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/preistyp.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/rechnungslegung.py
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/rechnungsstatus.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/rechnungstyp.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/regionskriteriumtyp.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/registeranzahl.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/rollencodetyp.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/sparte.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/steuerkennzeichen.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/strenum.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tarifkalkulationsmethode.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tarifmerkmal.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tarifregionskriterium.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tariftyp.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/tarifzeit.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/themengebiet.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/titel.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/typ.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/verbrauchsart.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/vertragsart.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/vertragsform.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/vertragsstatus.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/verwendungszweck.py
--rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/voraussetzungen.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/waehrungscode.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/waehrungseinheit.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/waermenutzung.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/wertermittlungsverfahren.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/zaehlerauspraegung.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/zaehlergroesse.py
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/zaehlertyp.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/enum/zaehlertypspezifikation.py
--rw-r--r--   0        0        0     3429 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/src/bo4e/utils/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/__init__.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/serialization_helper.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_adresse.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_angebot.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_angebotsposition.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_angebotsteil.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_angebotsvariante.py
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_aufabschlag.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_aufabschlagproort.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_aufabschlagregional.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_aufabschlagstaffelproort.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_ausschreibung.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_ausschreibungsdetail.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_ausschreibungslos.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_betrag.py
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_buendelvertrag.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_energieherkunft.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_energiemenge.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_energiemix.py
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_enums.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_fremdkosten.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_fremdkostenblock.py
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_fremdkostenposition.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_geokoordinaten.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_geraet.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_geschaeftsobjekt.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_geschaeftspartner.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_import_enum.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_katasteradresse.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kontakt.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kosten.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kostenblock.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kostenposition.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_kriteriumswert.py
--rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_lastgang.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_marktgebietinfo.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_marktlokation.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_marktteilnehmer.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_menge.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_messlokation.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_messlokationszuordnung.py
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_person.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_positionsaufabschlag.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preis.py
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt_dienstleistung.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt_hardware.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt_konzessionsabgabe.py
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblatt_messung.py
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisblattnetznutzung.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisgarantie.py
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisposition.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_preisstaffel.py
--rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_rechnung.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_rechnungsposition.py
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_region.py
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionalegueltigkeit.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionalepreisgarantie.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionalepreisstaffel.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionaleraufabschlag.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionaletarifpreisposition.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionaltarif.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_regionskriterium.py
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_sigmoidparameter.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_standorteigenschaften.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_standorteigenschaftengas.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_standorteigenschaftenstrom.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_steuerbetrag.py
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarif.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifberechnungsparameter.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifeinschraenkung.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifinfo.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifkosten.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreis.py
--rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreisblatt.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreisposition.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreispositionproort.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_tarifpreisstaffelproort.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_unterschrift.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_verbrauch.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_vertrag.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_vertragskonditionen.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_vertragsteil.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zaehler.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zeitraum.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zeitreihe.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zeitreihenwert.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zeitspanne.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_zusatz_attribut.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/utils.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/.gitignore
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/AUTHORS.rst
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/LICENSE.rst
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/pyproject.toml
--rw-r--r--   0        0        0     7050 2020-02-02 00:00:00.000000 bo4e-202401.1.1rc4/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    17211 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.pylintrc
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/CHANGELOG.rst
+-rw-r--r--   0        0        0     5590 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/MANIFEST.in
+-rw-r--r--   0        0        0     5748 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/README.rst
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/bo4e_schemas_create_release.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docker-compose.yml
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/generate_or_validate_json_schemas.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/requirements.in
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/requirements.txt
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tox.ini
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/dependabot.yml
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/docs_latest.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/formatting.yml
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/linting.yml
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/python-publish-scheduled.yml
+-rw-r--r--   0        0        0     7637 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/test_docs.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.vscode/settings.json
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-json_schemas.in
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-json_schemas.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-packaging.in
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-packaging.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0     7602 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/Makefile
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/authors.rst
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/changelog.rst
+-rw-r--r--   0        0        0    11523 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/conf.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/index.rst
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/license.rst
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/release_workflow.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/requirements.in
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/requirements.txt
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/test_uml.py
+-rw-r--r--   0        0        0    28472 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/uml.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/versioning.rst
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/_static/bo4e-python-favicon.png
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/_static/bo4e-python-favicon.svg
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/_static/bo4e-python-logo.png
+-rw-r--r--   0        0        0    26543 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/_static/bo4e-python-logo.svg
+-rw-r--r--   0        0        0   167661 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/_static/bo4e-release-workflow.excalidraw
+-rw-r--r--   0        0        0   512116 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/_static/bo4e-release-workflow.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/compatibility/__init__.py
+-rw-r--r--   0        0        0     9525 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/compatibility/__main__.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/compatibility/change_schemas.py
+-rw-r--r--   0        0        0    13297 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/compatibility/diff.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/compatibility/loader.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/compatibility/matrix.py
+-rw-r--r--   0        0        0    12151 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/docs/compatibility/versioning.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/_bo4e_python_version.py
+-rw-r--r--   0        0        0    13034 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/__init__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/py.typed
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/version.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/zusatzattribut.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/__init__.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/angebot.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/ausschreibung.py
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/buendelvertrag.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/energiemenge.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/fremdkosten.py
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/geraet.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/geschaeftsobjekt.py
+-rw-r--r--   0        0        0     3573 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/geschaeftspartner.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/kosten.py
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/lastgang.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/marktlokation.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/marktteilnehmer.py
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/messlokation.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/person.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/preisblatt.py
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/preisblattdienstleistung.py
+-rw-r--r--   0        0        0     1901 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/preisblatthardware.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/preisblattkonzessionsabgabe.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/preisblattmessung.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/preisblattnetznutzung.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/rechnung.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/region.py
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/regionaltarif.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/standorteigenschaften.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/tarif.py
+-rw-r--r--   0        0        0     2975 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/tarifinfo.py
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/tarifkosten.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/tarifpreisblatt.py
+-rw-r--r--   0        0        0     3237 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/vertrag.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/zaehler.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/bo/zeitreihe.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/__init__.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/adresse.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/angebotsposition.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/angebotsteil.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/angebotsvariante.py
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/aufabschlag.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/aufabschlagproort.py
+-rw-r--r--   0        0        0     3802 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/aufabschlagregional.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/aufabschlagstaffelproort.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/ausschreibungsdetail.py
+-rw-r--r--   0        0        0     3042 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/ausschreibungslos.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/betrag.py
+-rw-r--r--   0        0        0     2264 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/com.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/dienstleistung.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/energieherkunft.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/energiemix.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/fremdkostenblock.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/fremdkostenposition.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/geokoordinaten.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/katasteradresse.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/kontaktweg.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/konzessionsabgabe.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/kostenblock.py
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/kostenposition.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/kriteriumwert.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/marktgebietinfo.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/menge.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/messlokationszuordnung.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/positionsaufabschlag.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/preis.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/preisgarantie.py
+-rw-r--r--   0        0        0     3311 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/preisposition.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/preisstaffel.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/rechnungsposition.py
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/regionalegueltigkeit.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/regionalepreisgarantie.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/regionalepreisstaffel.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/regionaleraufabschlag.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/regionaletarifpreisposition.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/regionskriterium.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/sigmoidparameter.py
+-rw-r--r--   0        0        0     1029 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/standorteigenschaftengas.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/standorteigenschaftenstrom.py
+-rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/steuerbetrag.py
+-rw-r--r--   0        0        0     2740 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/tarifberechnungsparameter.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/tarifeinschraenkung.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/tarifpreis.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/tarifpreisposition.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/tarifpreispositionproort.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/tarifpreisstaffelproort.py
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/unterschrift.py
+-rw-r--r--   0        0        0     1786 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/verbrauch.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/vertragskonditionen.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/vertragsteil.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/verwendungszweckpromarktrolle.py
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/zaehlwerk.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/zaehlzeitregister.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/zeitraum.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/zeitreihenwert.py
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/zeitspanne.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/com/zustaendigkeit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/__init__.py
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/abgabeart.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/angebotsstatus.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/anrede.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/arithmetische_operation.py
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/artikelid.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/aufabschlagstyp.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/aufabschlagsziel.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/ausschreibungsportal.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/ausschreibungsstatus.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/ausschreibungstyp.py
+-rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/bdewartikelnummer.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/befestigungsart.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/bemessungsgroesse.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/bilanzierungsmethode.py
+-rw-r--r--   0        0        0     3853 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/dienstleistungstyp.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/energierichtung.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/erzeugungsart.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/gasqualitaet.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/gebiettyp.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/geraeteklasse.py
+-rw-r--r--   0        0        0     3540 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/geraetetyp.py
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/geschaeftspartnerrolle.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/gueltigkeitstyp.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/kalkulationsmethode.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/kontaktart.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/kostenklasse.py
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/kundengruppe.py
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/kundengruppeka.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/kundentyp.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/landescode.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/leistungstyp.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/lokationstyp.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/marktrolle.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/medium.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/mengeneinheit.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/mengenoperator.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/messart.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/messgroesse.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/messpreistyp.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/messwerterfassung.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/messwertstatus.py
+-rw-r--r--   0        0        0     4029 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/messwertstatuszusatz.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/netzebene.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/netznutzungrechnungsart.py
+-rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/netznutzungrechnungstyp.py
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/oekolabel.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/oekozertifikat.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/organisationstyp.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/preisgarantietyp.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/preismodell.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/preisstatus.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/preistyp.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/rechnungslegung.py
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/rechnungsstatus.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/rechnungstyp.py
+-rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/regionskriteriumtyp.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/registeranzahl.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/rollencodetyp.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/sparte.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/steuerkennzeichen.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/strenum.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/tarifkalkulationsmethode.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/tarifmerkmal.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/tarifregionskriterium.py
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/tariftyp.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/tarifzeit.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/themengebiet.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/titel.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/typ.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/verbrauchsart.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/vertragsart.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/vertragsform.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/vertragsstatus.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/verwendungszweck.py
+-rw-r--r--   0        0        0     4475 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/voraussetzungen.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/waehrungscode.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/waehrungseinheit.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/waermenutzung.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/wertermittlungsverfahren.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/zaehlerauspraegung.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/zaehlergroesse.py
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/zaehlertyp.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/enum/zaehlertypspezifikation.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/src/bo4e/utils/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/__init__.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/serialization_helper.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_adresse.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_angebot.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_angebotsposition.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_angebotsteil.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_angebotsvariante.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_aufabschlag.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_aufabschlagproort.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_aufabschlagregional.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_aufabschlagstaffelproort.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_ausschreibung.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_ausschreibungsdetail.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_ausschreibungslos.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_betrag.py
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_buendelvertrag.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_energieherkunft.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_energiemenge.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_energiemix.py
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_enums.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_fremdkosten.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_fremdkostenblock.py
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_fremdkostenposition.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_geokoordinaten.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_geraet.py
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_geschaeftsobjekt.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_geschaeftspartner.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_import_enum.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_katasteradresse.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_kontakt.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_kosten.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_kostenblock.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_kostenposition.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_kriteriumswert.py
+-rw-r--r--   0        0        0     1753 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_lastgang.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_marktgebietinfo.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_marktlokation.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_marktteilnehmer.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_menge.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_messlokation.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_messlokationszuordnung.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_person.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_positionsaufabschlag.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preis.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preisblatt.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preisblatt_dienstleistung.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preisblatt_hardware.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preisblatt_konzessionsabgabe.py
+-rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preisblatt_messung.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preisblattnetznutzung.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preisgarantie.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preisposition.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_preisstaffel.py
+-rw-r--r--   0        0        0     6039 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_rechnung.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_rechnungsposition.py
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_region.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_regionalegueltigkeit.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_regionalepreisgarantie.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_regionalepreisstaffel.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_regionaleraufabschlag.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_regionaletarifpreisposition.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_regionaltarif.py
+-rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_regionskriterium.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_sigmoidparameter.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_standorteigenschaften.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_standorteigenschaftengas.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_standorteigenschaftenstrom.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_steuerbetrag.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarif.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarifberechnungsparameter.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarifeinschraenkung.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarifinfo.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarifkosten.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarifpreis.py
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarifpreisblatt.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarifpreisposition.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarifpreispositionproort.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_tarifpreisstaffelproort.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_unterschrift.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_verbrauch.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_vertrag.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_vertragskonditionen.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_vertragsteil.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_zaehler.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_zeitraum.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_zeitreihe.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_zeitreihenwert.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_zeitspanne.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_zusatz_attribut.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/utils.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_data/test_data_adresse/test_data_adresse_missing_plz.json
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_data/test_data_adresse/test_data_adresse_only_required_fields.json
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/tests/test_data/test_data_adresse/test_data_adresse_with_all_possible_fields.json
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/.gitignore
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/AUTHORS.rst
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/LICENSE.rst
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/pyproject.toml
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 bo4e-202401.1.2rc14/PKG-INFO
```

### Comparing `bo4e-202401.1.1rc4/.pre-commit-config.yaml` & `bo4e-202401.1.2rc14/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/psf/black
-    rev: 23.9.1 # Replace by any tag/version: https://github.com/psf/black/tags
+    rev: 24.4.2 # Replace by any tag/version: https://github.com/psf/black/tags
     hooks:
       - id: black
         language_version: python3 # Should be a command that runs python3.6+
   - repo: https://github.com/pycqa/isort
     rev: 5.12.0
     hooks:
       - id: isort
```

### Comparing `bo4e-202401.1.1rc4/.pylintrc` & `bo4e-202401.1.2rc14/.pylintrc`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/CONTRIBUTING.md` & `bo4e-202401.1.2rc14/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/README.rst` & `bo4e-202401.1.2rc14/README.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/bo4e_schemas_create_release.py` & `bo4e-202401.1.2rc14/bo4e_schemas_create_release.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/generate_or_validate_json_schemas.py` & `bo4e-202401.1.2rc14/generate_or_validate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tox.ini` & `bo4e-202401.1.2rc14/tox.ini`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/dependabot.yml` & `bo4e-202401.1.2rc14/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md` & `bo4e-202401.1.2rc14/.github/ISSUE_TEMPLATE/funktionale-anforderung-an-den-bo4e-standard.md`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md` & `bo4e-202401.1.2rc14/.github/ISSUE_TEMPLATE/technisches-problem---python-specific-problem.md`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/workflows/codeql-analysis.yml` & `bo4e-202401.1.2rc14/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/workflows/coverage.yml` & `bo4e-202401.1.2rc14/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/workflows/dependabot_automerge.yml` & `bo4e-202401.1.2rc14/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/workflows/docs_latest.yml` & `bo4e-202401.1.2rc14/.github/workflows/docs_latest.yml`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,19 @@
           pip install tox
           pip install -r requirements.txt
         # Note: The sphinx action below can only install a single requirements file.
       - name: Build JSON Schemas
         run: tox -e generate_json_schemas
         env:
           TARGET_VERSION: ${{ env.REF_NAME }}
+      - name: Build BO4E package
+        # Note: This step necessary to correctly set the version in the JSON-Schema-links
+        run: |
+          pip install -e .
+          python -c "import bo4e; print(bo4e.__gh_version__)"
       - name: Run kroki with docker
         run: |
           docker compose up -d
       - name: Build the documentation
         uses: sphinx-notes/pages@v2
         # Note: This action has a newer version (v3 atm), but it doesn't has the feature to specify the target path.
         # We need that in order to be able to store (and deploy) multiple versions of the documentation.
```

### Comparing `bo4e-202401.1.1rc4/.github/workflows/linting.yml` & `bo4e-202401.1.2rc14/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/workflows/packaging_test.yml` & `bo4e-202401.1.2rc14/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/workflows/python-publish-scheduled.yml` & `bo4e-202401.1.2rc14/.github/workflows/python-publish-scheduled.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/workflows/python-publish.yml` & `bo4e-202401.1.2rc14/.github/workflows/python-publish.yml`

 * *Files 11% similar despite different names*

```diff
@@ -24,18 +24,43 @@
       - name: Install tox
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Run the Tests
         run: |
           tox -e tests
+  check_version_tag:
+    name: Check if the version tag is correct
+    runs-on: ubuntu-latest
+    steps:
+      - name: Check out Git repository
+        uses: actions/checkout@v4
+        with:
+          fetch-depth: 0
+      - name: Set up Python ${{ matrix.python-version }}
+        uses: actions/setup-python@v5
+        with:
+          python-version: "3.12"
+      - name: Install dependencies
+        run: |
+          python -m pip install --upgrade pip
+          pip install tox
+          pip install -r requirements.txt -r docs/requirements.txt
+      - name: Build JSON Schemas
+        run: tox -e generate_json_schemas
+        env:
+          TARGET_VERSION: ${{ github.ref_name }}
+      - name: Check version tag
+        run: |
+          python -m docs.compatibility.versioning --gh-version ${{ github.ref_name }} \
+          --gh-token ${{ secrets.GITHUB_TOKEN }} --major-bump-disallowed
   json_schemas:
     name: Generate JSON-Schemas
     runs-on: ubuntu-latest
-    needs: tests
+    needs: [tests, check_version_tag]
     steps:
       - name: Check out Git repository
         uses: actions/checkout@v4
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: "3.12"
@@ -74,15 +99,15 @@
           GITHUB_TOKEN: ${{ secrets.BO4E_PYTHON_GENERATE_SCHEMAS }} # this token expires on 2024-10-09
           VERSION: ${{ github.ref_name }}
   docs:
     name: 🚀📄 Build and deploy documentation to GitHub Pages
     # This setup is inspired by
     # https://github.com/KernelTuner/kernel_tuner/blob/master/.github/workflows/docs-on-release.yml
     runs-on: ubuntu-latest
-    needs: tests
+    needs: [tests, check_version_tag]
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0  # otherwise, you will fail to push refs to dest repo
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
@@ -93,14 +118,19 @@
           pip install tox
           pip install -r requirements.txt
         # Note: The sphinx action below can only install a single requirements file.
       - name: Build JSON Schemas
         run: tox -e generate_json_schemas
         env:
           TARGET_VERSION: ${{ github.ref_name }}
+      - name: Build BO4E package
+        # Note: This step necessary to correctly set the version in the JSON-Schema-links
+        run: |
+          pip install -e .
+          python -c "import bo4e; print(bo4e.__gh_version__)"
       - name: Run kroki with docker
         run: |
           docker compose up -d
       - name: Build the documentation
         uses: sphinx-notes/pages@v2
         # Note: This action has a newer version (v3 atm), but it doesn't has the feature to specify the target path.
         # We need that in order to be able to store (and deploy) multiple versions of the documentation.
```

### Comparing `bo4e-202401.1.1rc4/.github/workflows/test_docs.yml` & `bo4e-202401.1.2rc14/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.github/workflows/tests.yml` & `bo4e-202401.1.2rc14/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/dev_requirements/requirements-packaging.txt` & `bo4e-202401.1.2rc14/dev_requirements/requirements-packaging.txt`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/dev_requirements/requirements-type_check.txt` & `bo4e-202401.1.2rc14/dev_requirements/requirements-type_check.txt`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/Makefile` & `bo4e-202401.1.2rc14/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/changelog.rst` & `bo4e-202401.1.2rc14/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/conf.py` & `bo4e-202401.1.2rc14/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/index.rst` & `bo4e-202401.1.2rc14/docs/index.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/release_workflow.rst` & `bo4e-202401.1.2rc14/docs/release_workflow.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/requirements.txt` & `bo4e-202401.1.2rc14/docs/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile '.\docs\requirements.in'
 #
-alabaster==0.7.13
+alabaster==0.7.16
     # via sphinx
 annotated-types==0.5.0
     # via pydantic
 babel==2.12.1
     # via sphinx
 bo4e-schema-tool==0.0.7
     # via -r .\docs\requirements.in
@@ -17,15 +17,17 @@
 cffi==1.16.0
     # via
     #   cryptography
     #   pynacl
 charset-normalizer==2.1.0
     # via requests
 click==8.1.7
-    # via bo4e-schema-tool
+    # via
+    #   -r .\docs\requirements.in
+    #   bo4e-schema-tool
 colorama==0.4.6
     # via
     #   click
     #   sphinx
 cryptography==42.0.5
     # via pyjwt
 deprecated==1.2.14
@@ -36,15 +38,15 @@
     #   sphinx-rtd-theme
 idna==3.7
     # via requests
 imagesize==1.4.1
     # via sphinx
 iso3166==2.1.1
     # via -r .\docs\requirements.in
-jinja2==3.1.3
+jinja2==3.1.4
     # via sphinx
 markupsafe==2.1.3
     # via jinja2
 more-itertools==10.2.0
     # via bo4e-schema-tool
 networkx==3.3
     # via -r .\docs\requirements.in
@@ -72,25 +74,25 @@
     # via
     #   -r .\docs\requirements.in
     #   bo4e-schema-tool
     #   pygithub
     #   sphinx
 snowballstemmer==2.2.0
     # via sphinx
-sphinx==7.2.6
+sphinx==7.3.7
     # via
     #   -r .\docs\requirements.in
     #   sphinx-rtd-theme
     #   sphinxcontrib-applehelp
     #   sphinxcontrib-devhelp
     #   sphinxcontrib-htmlhelp
     #   sphinxcontrib-jquery
     #   sphinxcontrib-qthelp
     #   sphinxcontrib-serializinghtml
-sphinx-rtd-theme==1.3.0
+sphinx-rtd-theme==2.0.0
     # via -r .\docs\requirements.in
 sphinxcontrib-applehelp==1.0.7
     # via sphinx
 sphinxcontrib-devhelp==1.0.5
     # via sphinx
 sphinxcontrib-htmlhelp==2.0.4
     # via sphinx
@@ -98,20 +100,21 @@
     # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
 sphinxcontrib-qthelp==1.0.6
     # via sphinx
 sphinxcontrib-serializinghtml==1.1.9
     # via sphinx
-typeguard==4.1.5
+typeguard==4.2.1
     # via -r .\docs\requirements.in
 typing-extensions==4.11.0
     # via
     #   pydantic
     #   pydantic-core
     #   pygithub
+    #   typeguard
 urllib3==2.2.1
     # via
     #   pygithub
     #   requests
 wrapt==1.16.0
     # via deprecated
```

### Comparing `bo4e-202401.1.1rc4/docs/uml.py` & `bo4e-202401.1.2rc14/docs/uml.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/versioning.rst` & `bo4e-202401.1.2rc14/docs/versioning.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/_static/bo4e-python-favicon.png` & `bo4e-202401.1.2rc14/docs/_static/bo4e-python-favicon.png`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/_static/bo4e-python-favicon.svg` & `bo4e-202401.1.2rc14/docs/_static/bo4e-python-favicon.svg`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/_static/bo4e-python-logo.png` & `bo4e-202401.1.2rc14/docs/_static/bo4e-python-logo.png`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/_static/bo4e-python-logo.svg` & `bo4e-202401.1.2rc14/docs/_static/bo4e-python-logo.svg`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/_static/bo4e-release-workflow.excalidraw` & `bo4e-202401.1.2rc14/docs/_static/bo4e-release-workflow.excalidraw`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/_static/bo4e-release-workflow.png` & `bo4e-202401.1.2rc14/docs/_static/bo4e-release-workflow.png`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/compatibility/__main__.py` & `bo4e-202401.1.2rc14/docs/compatibility/__main__.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/compatibility/change_schemas.py` & `bo4e-202401.1.2rc14/docs/compatibility/change_schemas.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/compatibility/diff.py` & `bo4e-202401.1.2rc14/docs/compatibility/diff.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/compatibility/loader.py` & `bo4e-202401.1.2rc14/docs/compatibility/loader.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/docs/compatibility/matrix.py` & `bo4e-202401.1.2rc14/docs/compatibility/matrix.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/__init__.py` & `bo4e-202401.1.2rc14/src/bo4e/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     "Marktrolle",
     "Medium",
     "Mengeneinheit",
     "Mengenoperator",
     "Messart",
     "Messgroesse",
     "Messpreistyp",
+    "Messwerterfassung",
     "Messwertstatus",
     "Messwertstatuszusatz",
     "Netzebene",
     "NetznutzungRechnungsart",
     "NetznutzungRechnungstyp",
     "Oekolabel",
     "Oekozertifikat",
@@ -183,14 +184,16 @@
     "Zaehlertyp",
     "ZaehlertypSpezifikation",
     "ZusatzAttribut",
     "__version__",
     "__gh_version__",
 ]
 
+from pydantic import BaseModel as _PydanticBaseModel
+
 # Import BOs
 from .bo.angebot import Angebot
 from .bo.ausschreibung import Ausschreibung
 from .bo.buendelvertrag import Buendelvertrag
 from .bo.energiemenge import Energiemenge
 from .bo.fremdkosten import Fremdkosten
 from .bo.geraet import Geraet
@@ -318,14 +321,15 @@
 from .enum.marktrolle import Marktrolle
 from .enum.medium import Medium
 from .enum.mengeneinheit import Mengeneinheit
 from .enum.mengenoperator import Mengenoperator
 from .enum.messart import Messart
 from .enum.messgroesse import Messgroesse
 from .enum.messpreistyp import Messpreistyp
+from .enum.messwerterfassung import Messwerterfassung
 from .enum.messwertstatus import Messwertstatus
 from .enum.messwertstatuszusatz import Messwertstatuszusatz
 from .enum.netzebene import Netzebene
 from .enum.netznutzungrechnungsart import NetznutzungRechnungsart
 from .enum.netznutzungrechnungstyp import NetznutzungRechnungstyp
 from .enum.oekolabel import Oekolabel
 from .enum.oekozertifikat import Oekozertifikat
@@ -363,7 +367,14 @@
 from .enum.wertermittlungsverfahren import Wertermittlungsverfahren
 from .enum.zaehlerauspraegung import Zaehlerauspraegung
 from .enum.zaehlergroesse import Zaehlergroesse
 from .enum.zaehlertyp import Zaehlertyp
 from .enum.zaehlertypspezifikation import ZaehlertypSpezifikation
 from .version import __gh_version__, __version__
 from .zusatzattribut import ZusatzAttribut
+
+# Resolve all ForwardReferences. This design prevents circular import errors.
+for cls_name in __all__:
+    cls = globals().get(cls_name, None)
+    if cls is None or not isinstance(cls, type) or not issubclass(cls, _PydanticBaseModel):
+        continue
+    cls.model_rebuild(force=True)
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/version.py` & `bo4e-202401.1.2rc14/src/bo4e/version.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/zusatzattribut.py` & `bo4e-202401.1.2rc14/src/bo4e/zusatzattribut.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/angebot.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/angebot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 Contains Angebot class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.angebotsvariante import Angebotsvariante
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .geschaeftspartner import Geschaeftspartner
-from .person import Person
+
+if TYPE_CHECKING:
+    from ..com.angebotsvariante import Angebotsvariante
+    from ..enum.sparte import Sparte
+    from .geschaeftspartner import Geschaeftspartner
+    from .person import Person
 
 
 @postprocess_docstring
 class Angebot(Geschaeftsobjekt):
     """
     Mit diesem BO kann ein Versorgungsangebot zur Strom- oder Gasversorgung oder die Teilnahme an einer Ausschreibung
     übertragen werden. Es können verschiedene Varianten enthalten sein (z.B. ein- und mehrjährige Laufzeit).
@@ -32,32 +34,32 @@
 
     .. HINT::
         `Angebot JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Angebot.json>`_
 
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.ANGEBOT
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.ANGEBOT
     #: Eindeutige Nummer des Angebotes
     angebotsnummer: Optional[str] = None
     #: Erstellungsdatum des Angebots
     angebotsdatum: Optional[pydantic.AwareDatetime] = None
     #: Sparte, für die das Angebot abgegeben wird (Strom/Gas)
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
     #: Ersteller des Angebots
-    angebotsgeber: Optional[Geschaeftspartner] = None
+    angebotsgeber: Optional["Geschaeftspartner"] = None
     #: Empfänger des Angebots
-    angebotsnehmer: Optional[Geschaeftspartner] = None
+    angebotsnehmer: Optional["Geschaeftspartner"] = None
 
-    varianten: Optional[list[Angebotsvariante]] = None
+    varianten: Optional[list["Angebotsvariante"]] = None
     """ Eine oder mehrere Varianten des Angebots mit den Angebotsteilen;
     Ein Angebot besteht mindestens aus einer Variante."""
 
     anfragereferenz: Optional[str] = None
     """	Referenz auf eine Anfrage oder Ausschreibung;
     Kann dem Empfänger des Angebotes bei Zuordnung des Angebotes zur Anfrage bzw. Ausschreibung helfen."""
     #: Bis zu diesem Zeitpunkt (Tag/Uhrzeit) inklusive gilt das Angebot
     bindefrist: Optional[pydantic.AwareDatetime] = None
     #: Person, die als Angebotsnehmer das Angebot angenommen hat
-    unterzeichner_angebotsnehmer: Optional[Person] = None
+    unterzeichner_angebotsnehmer: Optional["Person"] = None
     #: Person, die als Angebotsgeber das Angebots ausgestellt hat
-    unterzeichner_angebotsgeber: Optional[Person] = None
+    unterzeichner_angebotsgeber: Optional["Person"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/ausschreibung.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/ausschreibung.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 Contains Ausschreibung class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.ausschreibungslos import Ausschreibungslos
-from ..com.zeitraum import Zeitraum
-from ..enum.ausschreibungsportal import Ausschreibungsportal
-from ..enum.ausschreibungsstatus import Ausschreibungsstatus
-from ..enum.ausschreibungstyp import Ausschreibungstyp
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .geschaeftspartner import Geschaeftspartner
+
+if TYPE_CHECKING:
+    from ..com.ausschreibungslos import Ausschreibungslos
+    from ..com.zeitraum import Zeitraum
+    from ..enum.ausschreibungsportal import Ausschreibungsportal
+    from ..enum.ausschreibungsstatus import Ausschreibungsstatus
+    from ..enum.ausschreibungstyp import Ausschreibungstyp
+    from .geschaeftspartner import Geschaeftspartner
 
 
 @postprocess_docstring
 class Ausschreibung(Geschaeftsobjekt):
     """
     Das BO Ausschreibung dient zur detaillierten Darstellung von ausgeschriebenen Energiemengen in der Energiewirtschaft
 
@@ -30,40 +32,40 @@
         <object data="../_static/images/bo4e/bo/Ausschreibung.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Ausschreibung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Ausschreibung.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.AUSSCHREIBUNG
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.AUSSCHREIBUNG
     #: Vom Herausgeber der Ausschreibung vergebene eindeutige Nummer
     ausschreibungsnummer: Optional[str] = None
     #: Aufzählung für die Typisierung von Ausschreibungen
-    ausschreibungstyp: Optional[Ausschreibungstyp] = None
+    ausschreibungstyp: Optional["Ausschreibungstyp"] = None
     #: Bezeichnungen für die Ausschreibungsphasen
-    ausschreibungsstatus: Optional[Ausschreibungsstatus] = None
+    ausschreibungsstatus: Optional["Ausschreibungsstatus"] = None
     #: Kennzeichen, ob die Ausschreibung kostenpflichtig ist
     ist_kostenpflichtig: Optional[bool] = None
     #: Gibt den Veröffentlichungszeitpunkt der Ausschreibung an
     veroeffentlichungszeitpunkt: Optional[pydantic.AwareDatetime] = None
-    ausschreibender: Optional[Geschaeftspartner] = None
+    ausschreibender: Optional["Geschaeftspartner"] = None
     """
     Mit diesem Objekt können Geschäftspartner übertragen werden.
     Sowohl Unternehmen, als auch Privatpersonen können Geschäftspartner sein
     """
-    abgabefrist: Optional[Zeitraum] = None
+    abgabefrist: Optional["Zeitraum"] = None
     """
     Diese Komponente wird zur Abbildung von Zeiträumen in Form von Dauern oder der Angabe von Start und Ende verwendet.
     Es muss daher entweder eine Dauer oder ein Zeitraum in Form von Start und Ende angegeben sein
     """
-    bindefrist: Optional[Zeitraum] = None
+    bindefrist: Optional["Zeitraum"] = None
     """
     Diese Komponente wird zur Abbildung von Zeiträumen in Form von Dauern oder der Angabe von Start und Ende verwendet.
     Es muss daher entweder eine Dauer oder ein Zeitraum in Form von Start und Ende angegeben sein
     """
     #: Die einzelnen Lose, aus denen sich die Ausschreibung zusammensetzt
-    lose: Optional[list[Ausschreibungslos]] = None
+    lose: Optional[list["Ausschreibungslos"]] = None
 
     #: Aufzählung der unterstützten Ausschreibungsportale
-    ausschreibungportal: Optional[Ausschreibungsportal] = None
+    ausschreibungportal: Optional["Ausschreibungsportal"] = None
     #: Internetseite, auf der die Ausschreibung veröffentlicht wurde (falls vorhanden)
     webseite: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/buendelvertrag.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/buendelvertrag.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 """
 Contains Buendelvertrag class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.unterschrift import Unterschrift
-from ..com.vertragskonditionen import Vertragskonditionen
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
-from ..enum.vertragsart import Vertragsart
-from ..enum.vertragsstatus import Vertragsstatus
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .geschaeftspartner import Geschaeftspartner
-from .vertrag import Vertrag
+
+if TYPE_CHECKING:
+    from ..com.unterschrift import Unterschrift
+    from ..com.vertragskonditionen import Vertragskonditionen
+    from ..enum.sparte import Sparte
+    from ..enum.vertragsart import Vertragsart
+    from ..enum.vertragsstatus import Vertragsstatus
+    from .geschaeftspartner import Geschaeftspartner
+    from .vertrag import Vertrag
 
 
 @postprocess_docstring
 class Buendelvertrag(Geschaeftsobjekt):
     """
     Abbildung eines Bündelvertrags.
     Es handelt sich hierbei um eine Liste von Einzelverträgen, die in einem Vertragsobjekt gebündelt sind.
@@ -32,39 +34,39 @@
         <object data="../_static/images/bo4e/bo/Buendelvertrag.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Buendelvertrag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Buendelvertrag.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.BUENDELVERTRAG
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.BUENDELVERTRAG
 
     # pylint: disable=duplicate-code
     #: Eine im Verwendungskontext eindeutige Nummer für den Vertrag
     vertragsnummer: Optional[str] = None
     #: Hier ist festgelegt, um welche Art von Vertrag es sich handelt. Z.B. Netznutzungvertrag
-    vertragsart: Optional[Vertragsart] = None
+    vertragsart: Optional["Vertragsart"] = None
     #: Gibt den Status des Vertrages an
-    vertragsstatus: Optional[Vertragsstatus] = None
+    vertragsstatus: Optional["Vertragsstatus"] = None
     #: Unterscheidungsmöglichkeiten für die Sparte
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
     #: Gibt an, wann der Vertrag beginnt (inklusiv)
     vertragsbeginn: Optional[pydantic.AwareDatetime] = None
     #: Gibt an, wann der Vertrag (voraussichtlich) endet oder beendet wurde (exklusiv)
     vertragsende: Optional[pydantic.AwareDatetime] = None
     #: Der "erstgenannte" Vertragspartner. In der Regel der Aussteller des Vertrags.
     #: Beispiel: "Vertrag zwischen Vertagspartner 1 ..."
-    vertragspartner1: Optional[Geschaeftspartner] = None
+    vertragspartner1: Optional["Geschaeftspartner"] = None
     #: Der "zweitgenannte" Vertragspartner. In der Regel der Empfänger des Vertrags.
     #: Beispiel "Vertrag zwischen Vertagspartner 1 und Vertragspartner 2"
-    vertragspartner2: Optional[Geschaeftspartner] = None
+    vertragspartner2: Optional["Geschaeftspartner"] = None
 
     #: Die Liste mit den Einzelverträgen zu den Abnahmestellen
-    einzelvertraege: Optional[list[Vertrag]] = None
+    einzelvertraege: Optional[list["Vertrag"]] = None
     #: Festlegungen zu Laufzeiten und Kündigungsfristen
-    vertragskonditionen: Optional[list[Vertragskonditionen]] = None
+    vertragskonditionen: Optional[list["Vertragskonditionen"]] = None
     #: Unterzeichner des Vertragspartners1
-    unterzeichnervp1: Optional[list[Unterschrift]] = None
+    unterzeichnervp1: Optional[list["Unterschrift"]] = None
     #: Unterzeichner des Vertragspartners2
-    unterzeichnervp2: Optional[list[Unterschrift]] = None
+    unterzeichnervp2: Optional[list["Unterschrift"]] = None
     #: Beschreibung zum Vertrag
     beschreibung: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/energiemenge.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/energiemenge.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Contains Energiemenge class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..com.verbrauch import Verbrauch
-from ..enum.lokationstyp import Lokationstyp
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
 
+if TYPE_CHECKING:
+    from ..com.verbrauch import Verbrauch
+    from ..enum.lokationstyp import Lokationstyp
+
+
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class Energiemenge(Geschaeftsobjekt):
     """
@@ -27,17 +30,17 @@
         <object data="../_static/images/bo4e/bo/Energiemenge.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Energiemenge JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Energiemenge.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.ENERGIEMENGE
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.ENERGIEMENGE
     #: Eindeutige Nummer der Marktlokation bzw. der Messlokation, zu der die Energiemenge gehört
     lokations_id: Optional[str] = None
     # todo: add validator such that only mess- or marktlokations IDs are accepted + cross check with lokationstyp
     #: Gibt an, ob es sich um eine Markt- oder Messlokation handelt
-    lokationstyp: Optional[Lokationstyp] = None
+    lokationstyp: Optional["Lokationstyp"] = None
 
     #: Gibt den Verbrauch in einer Zeiteinheit an
-    energieverbrauch: Optional[list[Verbrauch]] = None
+    energieverbrauch: Optional[list["Verbrauch"]] = None
     # there are no optional attributes
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/fremdkosten.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/kosten.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 """
-Contains Fremdkosten class and corresponding marshmallow schema for de-/serialization
+Contains Kosten class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..com.betrag import Betrag
-from ..com.fremdkostenblock import Fremdkostenblock
-from ..com.zeitraum import Zeitraum
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
 
-# pylint: disable=too-few-public-methods
+if TYPE_CHECKING:
+    from ..com.betrag import Betrag
+    from ..com.kostenblock import Kostenblock
+    from ..com.zeitraum import Zeitraum
+    from ..enum.kostenklasse import Kostenklasse
+
+
+# pylint: disable=too-many-instance-attributes, too-few-public-methods
+# pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
-class Fremdkosten(Geschaeftsobjekt):
+class Kosten(Geschaeftsobjekt):
     """
-    Mit diesem BO werden die Fremdkosten, beispielsweise für eine Angebotserstellung oder eine Rechnungsprüfung,
-    übertragen.
-    Die Fremdkosten enthalten dabei alle Kostenblöcke, die von anderen Marktteilnehmern oder Instanzen erhoben werden.
+    Dieses BO wird zur Übertagung von hierarchischen Kostenstrukturen verwendet.
+    Die Kosten werden dabei in Kostenblöcke und diese wiederum in Kostenpositionen strukturiert.
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/bo/Fremdkosten.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/bo/Kosten.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `Fremdkosten JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Fremdkosten.json>`_
+        `Kosten JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Kosten.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.FREMDKOSTEN
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.KOSTEN
+    #: Klasse der Kosten, beispielsweise Fremdkosten
+    kostenklasse: Optional["Kostenklasse"] = None
     #: Für diesen Zeitraum wurden die Kosten ermittelt
-    gueltigkeit: Optional[Zeitraum] = None
-    #: Die Gesamtsumme über alle Kostenblöcke und -positionen
-    summe_kosten: Optional[Betrag] = None
+    gueltigkeit: Optional["Zeitraum"] = None
     #: In Kostenblöcken werden Kostenpositionen zusammengefasst. Beispiele: Netzkosten, Umlagen, Steuern etc
-    kostenbloecke: Optional[list[Fremdkostenblock]] = None
+    kostenbloecke: Optional[list["Kostenblock"]] = None
+
+    #: Die Gesamtsumme über alle Kostenblöcke und -positionen
+    summe_kosten: Optional[list["Betrag"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/geraet.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/geraet.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Contains Geraet class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..enum.geraeteklasse import Geraeteklasse
-from ..enum.geraetetyp import Geraetetyp
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
 
+if TYPE_CHECKING:
+    from ..enum.geraeteklasse import Geraeteklasse
+    from ..enum.geraetetyp import Geraetetyp
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Geraet(Geschaeftsobjekt):
     """
     Mit diesem BO werden alle Geräte modelliert, die keine Zähler sind.
@@ -26,17 +29,17 @@
         <object data="../_static/images/bo4e/bo/Geraet.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Geraet JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Geraet.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.GERAET
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.GERAET
 
     #: Die auf dem Gerät aufgedruckte Nummer, die vom MSB vergeben wird.
     geraetenummer: Optional[str] = None
     #: Bezeichnung des Geräts
     bezeichnung: Optional[str] = None
     #: Die übergreifende Klasse eines Geräts, beispielsweise Wandler
-    geraeteklasse: Optional[Geraeteklasse] = None
+    geraeteklasse: Optional["Geraeteklasse"] = None
     #: Der speziellere Typ eines Gerätes, beispielsweise Stromwandler
-    geraetetyp: Optional[Geraetetyp] = None
+    geraetetyp: Optional["Geraetetyp"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/geschaeftsobjekt.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/geschaeftsobjekt.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,22 @@
 
     .. HINT::
         `Geschaeftsobjekt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Geschaeftsobjekt.json>`_
 
     """
 
     # required attributes
-    version: Annotated[
-        Optional[str], Field(alias="_version")
-    ] = __version__  #: Version der BO-Struktur aka "fachliche Versionierung"
+    version: Annotated[Optional[str], Field(alias="_version")] = (
+        __version__  #: Version der BO-Struktur aka "fachliche Versionierung"
+    )
     # src/_bo4e_python_version.py
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.GESCHAEFTSOBJEKT  #: Der Typ des Geschäftsobjektes
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.GESCHAEFTSOBJEKT  #: Der Typ des Geschäftsobjektes
     # bo_typ is used as discriminator f.e. for databases or deserialization
 
-    zusatz_attribute: Optional[list[ZusatzAttribut]] = None
+    zusatz_attribute: Optional[list["ZusatzAttribut"]] = None
     # zusatz_attribute is a list of ZusatzAttribut objects which are used to store additional information
 
     # Python internal: The field is not named '_id' because leading underscores are not allowed in pydantic field names.
     # NameError: Fields must not use names with leading underscores; e.g., use 'id' instead of '_id'.
     id: Annotated[Optional[str], Field(alias="_id")] = None
     """
     Eine generische ID, die für eigene Zwecke genutzt werden kann.
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/geschaeftspartner.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/geschaeftspartner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,84 @@
 """
 Contains Geschaeftspartner class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods, disable=duplicate-code
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..com.adresse import Adresse
-from ..com.kontaktweg import Kontaktweg
-from ..enum.anrede import Anrede
-from ..enum.geschaeftspartnerrolle import Geschaeftspartnerrolle
-from ..enum.organisationstyp import Organisationstyp
-from ..enum.titel import Titel
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .person import Person
+
+if TYPE_CHECKING:
+    from ..com.adresse import Adresse
+    from ..com.kontaktweg import Kontaktweg
+    from ..enum.anrede import Anrede
+    from ..enum.geschaeftspartnerrolle import Geschaeftspartnerrolle
+    from ..enum.organisationstyp import Organisationstyp
+    from ..enum.titel import Titel
+    from .person import Person
 
 
 @postprocess_docstring
 class Geschaeftspartner(Geschaeftsobjekt):
     """
     Mit diesem Objekt können Geschäftspartner übertragen werden.
     Sowohl Unternehmen, als auch Privatpersonen können Geschäftspartner sein.
-    Hinweis: Marktteilnehmer haben ein eigenes BO, welches sich von diesem BO ableitet.
+    Hinweis: "Marktteilnehmer" haben ein eigenes BO, welches sich von diesem BO ableitet.
     Hier sollte daher keine Zuordnung zu Marktrollen erfolgen.
 
     .. raw:: html
 
         <object data="../_static/images/bo4e/bo/Geschaeftspartner.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Geschaeftspartner JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Geschaeftspartner.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.GESCHAEFTSPARTNER
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.GESCHAEFTSPARTNER
     #: Mögliche Anrede der Person
-    anrede: Optional[Anrede] = None
+    anrede: Optional["Anrede"] = None
     individuelle_anrede: Optional[str] = None
     """
     Im Falle einer nicht standardisierten Anrede kann hier eine frei definierbare Anrede vorgegeben werden.
     Beispiel: "Vereinsgemeinschaft", "Pfarrer", "Hochwürdigster Herr Abt".
     """
     #: Möglicher Titel der Person
-    titel: Optional[Titel] = None
+    titel: Optional["Titel"] = None
     #: Vorname der Person
     vorname: Optional[str] = None
     #: Nachname (Familienname) der Person
     nachname: Optional[str] = None
 
-    ansprechpartner: Optional[list[Person]] = None
-    organisationstyp: Optional[Organisationstyp] = None
+    ansprechpartner: Optional[list["Person"]] = None
+    organisationstyp: Optional["Organisationstyp"] = None
     """
     Kennzeichnung ob es sich um ein Gewerbe/Unternehmen, eine Privatperson oder eine andere Art von Organisation handelt.
     """
     organisationsname: Optional[str] = None
     """
     Name der Firma, wenn Gewerbe oder andere Organisation.
     """
     #: Kontaktwege des Geschäftspartners
-    kontaktwege: Optional[list[Kontaktweg]] = None
+    kontaktwege: Optional[list["Kontaktweg"]] = None
     #: Rollen, die die Geschäftspartner inne haben (z.B. Interessent, Kunde)
-    geschaeftspartnerrollen: Optional[list[Geschaeftspartnerrolle]] = None
+    geschaeftspartnerrollen: Optional[list["Geschaeftspartnerrolle"]] = None
     #: Handelsregisternummer des Geschäftspartners
     handelsregisternummer: Optional[str] = None
     #: Amtsgericht bzw Handelsregistergericht, das die Handelsregisternummer herausgegeben hat
     amtsgericht: Optional[str] = None
     #: Die Steuer-ID des Geschäftspartners; Beispiel: "DE 813281825"
     umsatzsteuer_id: Optional[str] = None
     #: Die Gläubiger-ID welche im Zahlungsverkehr verwendet wird; Z.B. "DE 47116789"
     glaeubiger_id: Optional[str] = None
     #: Internetseite des Marktpartners
     website: Optional[str] = None
     #: Adresse des Geschäftspartners
-    adresse: Optional[Adresse] = None
+    adresse: Optional["Adresse"] = None
     #: Todo: Add optional connection to marktteilnehmer as discussed in workshop
     #: not clear what is the best solution here - circular import marktteilnehmer?
     #: discussed in workshop on Feb 6 2024: yes we need the bidirectional option, let's figure out a solution somehow.
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/kosten.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/fremdkosten.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 """
-Contains Kosten class and corresponding marshmallow schema for de-/serialization
+Contains Fremdkosten class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..com.betrag import Betrag
-from ..com.kostenblock import Kostenblock
-from ..com.zeitraum import Zeitraum
-from ..enum.kostenklasse import Kostenklasse
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
 
-# pylint: disable=too-many-instance-attributes, too-few-public-methods
-# pylint: disable=no-name-in-module
+if TYPE_CHECKING:
+    from ..com.betrag import Betrag
+    from ..com.fremdkostenblock import Fremdkostenblock
+    from ..com.zeitraum import Zeitraum
+
+
+# pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
-class Kosten(Geschaeftsobjekt):
+class Fremdkosten(Geschaeftsobjekt):
     """
-    Dieses BO wird zur Übertagung von hierarchischen Kostenstrukturen verwendet.
-    Die Kosten werden dabei in Kostenblöcke und diese wiederum in Kostenpositionen strukturiert.
+    Mit diesem BO werden die Fremdkosten, beispielsweise für eine Angebotserstellung oder eine Rechnungsprüfung,
+    übertragen.
+    Die Fremdkosten enthalten dabei alle Kostenblöcke, die von anderen Marktteilnehmern oder Instanzen erhoben werden.
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/bo/Kosten.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/bo/Fremdkosten.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `Kosten JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Kosten.json>`_
+        `Fremdkosten JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Fremdkosten.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.KOSTEN
-    #: Klasse der Kosten, beispielsweise Fremdkosten
-    kostenklasse: Optional[Kostenklasse] = None
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.FREMDKOSTEN
     #: Für diesen Zeitraum wurden die Kosten ermittelt
-    gueltigkeit: Optional[Zeitraum] = None
-    #: In Kostenblöcken werden Kostenpositionen zusammengefasst. Beispiele: Netzkosten, Umlagen, Steuern etc
-    kostenbloecke: Optional[list[Kostenblock]] = None
-
+    gueltigkeit: Optional["Zeitraum"] = None
     #: Die Gesamtsumme über alle Kostenblöcke und -positionen
-    summe_kosten: Optional[list[Betrag]] = None
+    summe_kosten: Optional["Betrag"] = None
+    #: In Kostenblöcken werden Kostenpositionen zusammengefasst. Beispiele: Netzkosten, Umlagen, Steuern etc
+    kostenbloecke: Optional[list["Fremdkostenblock"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/lastgang.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/lastgang.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 """
 Contains Lastgang class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 from pydantic import Field, constr
 
-from ..bo.marktlokation import Marktlokation
-from ..bo.messlokation import Messlokation
-from ..com.menge import Menge
-from ..com.zeitreihenwert import Zeitreihenwert
-from ..enum.mengeneinheit import Mengeneinheit
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
 
+if TYPE_CHECKING:
+    from ..bo.marktlokation import Marktlokation
+    from ..bo.messlokation import Messlokation
+    from ..com.menge import Menge
+    from ..com.zeitreihenwert import Zeitreihenwert
+    from ..enum.mengeneinheit import Mengeneinheit
+    from ..enum.sparte import Sparte
+
+
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 
 
 @postprocess_docstring
 class Lastgang(Geschaeftsobjekt):
     """
     Modell zur Abbildung eines Lastganges;
@@ -33,23 +36,23 @@
         <object data="../_static/images/bo4e/bo/Lastgang.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Lastgang JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Lastgang.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.LASTGANG
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.LASTGANG
     #: Angabe, ob es sich um einen Gas- oder Stromlastgang handelt
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
     #: Definition der gemessenen Größe anhand ihrer Einheit
-    messgroesse: Optional[Mengeneinheit] = None
+    messgroesse: Optional["Mengeneinheit"] = None
     #:Marktlokation, zu der der Lastgang gehört
-    marktlokation: Optional[Marktlokation] = None
+    marktlokation: Optional["Marktlokation"] = None
     #:Marktlokation, zu der der Lastgang gehört
-    messlokation: Optional[Messlokation] = None
+    messlokation: Optional["Messlokation"] = None
     #: Die im Lastgang enthaltenen Messwerte
-    werte: Optional[list[Zeitreihenwert]] = None
+    werte: Optional[list["Zeitreihenwert"]] = None
     #: Versionsnummer des Lastgangs
     version: Optional[str] = None
     #: Die OBIS-Kennzahl für den Wert, die festlegt, welche Größe mit dem Stand gemeldet wird, z.B. '1-0:1.8.1'
     obis_kennzahl: Optional[constr(strict=True)] = None  # type: ignore[valid-type]
-    zeit_intervall_laenge: Optional[Menge]
+    zeit_intervall_laenge: Optional["Menge"]
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/marktlokation.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/marktlokation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 """
 Contains Marktlokation class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..com.adresse import Adresse
-from ..com.geokoordinaten import Geokoordinaten
-from ..com.katasteradresse import Katasteradresse
-from ..com.messlokationszuordnung import Messlokationszuordnung
-from ..com.verbrauch import Verbrauch
-from ..com.zaehlwerk import Zaehlwerk
-from ..enum.bilanzierungsmethode import Bilanzierungsmethode
-from ..enum.energierichtung import Energierichtung
-from ..enum.gasqualitaet import Gasqualitaet
-from ..enum.gebiettyp import Gebiettyp
-from ..enum.kundentyp import Kundentyp
-from ..enum.netzebene import Netzebene
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
-from ..enum.verbrauchsart import Verbrauchsart
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .geschaeftspartner import Geschaeftspartner
+
+if TYPE_CHECKING:
+    from ..com.adresse import Adresse
+    from ..com.geokoordinaten import Geokoordinaten
+    from ..com.katasteradresse import Katasteradresse
+    from ..com.messlokationszuordnung import Messlokationszuordnung
+    from ..com.verbrauch import Verbrauch
+    from ..com.zaehlwerk import Zaehlwerk
+    from ..enum.bilanzierungsmethode import Bilanzierungsmethode
+    from ..enum.energierichtung import Energierichtung
+    from ..enum.gasqualitaet import Gasqualitaet
+    from ..enum.gebiettyp import Gebiettyp
+    from ..enum.kundentyp import Kundentyp
+    from ..enum.netzebene import Netzebene
+    from ..enum.sparte import Sparte
+    from ..enum.verbrauchsart import Verbrauchsart
+    from .geschaeftspartner import Geschaeftspartner
 
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class Marktlokation(Geschaeftsobjekt):
     """
@@ -40,49 +42,49 @@
         <object data="../_static/images/bo4e/bo/Marktlokation.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Marktlokation JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Marktlokation.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.MARKTLOKATION
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.MARKTLOKATION
     #: Identifikationsnummer einer Marktlokation, an der Energie entweder verbraucht, oder erzeugt wird.
     marktlokations_id: Optional[str] = None
     #: Sparte der Marktlokation, z.B. Gas oder Strom
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
     #: Kennzeichnung, ob Energie eingespeist oder entnommen (ausgespeist) wird
-    energierichtung: Optional[Energierichtung] = None
+    energierichtung: Optional["Energierichtung"] = None
     #: Die Bilanzierungsmethode, RLM oder SLP
-    bilanzierungsmethode: Optional[Bilanzierungsmethode] = None
-    netzebene: Optional[Netzebene] = None
+    bilanzierungsmethode: Optional["Bilanzierungsmethode"] = None
+    netzebene: Optional["Netzebene"] = None
     """
     Netzebene, in der der Bezug der Energie erfolgt.
     Bei Strom Spannungsebene der Lieferung, bei Gas Druckstufe.
     Beispiel Strom: Niederspannung Beispiel Gas: Niederdruck.
     """
 
     #: Verbrauchsart der Marktlokation.
-    verbrauchsart: Optional[Verbrauchsart] = None
+    verbrauchsart: Optional["Verbrauchsart"] = None
     #: Gibt an, ob es sich um eine unterbrechbare Belieferung handelt
     ist_unterbrechbar: Optional[bool] = None
     #: Codenummer des Netzbetreibers, an dessen Netz diese Marktlokation angeschlossen ist.
     netzbetreibercodenr: Optional[str] = None
     #: Typ des Netzgebietes, z.B. Verteilnetz
-    gebietstyp: Optional[Gebiettyp] = None
+    gebietstyp: Optional["Gebiettyp"] = None
     #: Die ID des Gebietes in der ene't-Datenbank
     netzgebietsnr: Optional[str] = None  # todo: rename to "id" (see 2021-12-15 update)
     #: Bilanzierungsgebiet, dem das Netzgebiet zugeordnet ist - im Falle eines Strom Netzes
     bilanzierungsgebiet: Optional[str] = None
     #: Codenummer des Grundversorgers, der für diese Marktlokation zuständig ist
     grundversorgercodenr: Optional[str] = None
     #: Die Gasqualität in diesem Netzgebiet. H-Gas oder L-Gas. Im Falle eines Gas-Netzes
-    gasqualitaet: Optional[Gasqualitaet] = None
+    gasqualitaet: Optional["Gasqualitaet"] = None
     #: Geschäftspartner, dem diese Marktlokation gehört
-    endkunde: Optional[Geschaeftspartner] = None
-    zugehoerige_messlokation: Optional[Messlokationszuordnung] = None  # todo: rename to plural
+    endkunde: Optional["Geschaeftspartner"] = None
+    zugehoerige_messlokation: Optional["Messlokationszuordnung"] = None  # todo: rename to plural
     """
     Aufzählung der Messlokationen, die zu dieser Marktlokation gehören.
     Es können 3 verschiedene Konstrukte auftreten:
 
     Beziehung 1 : 0 : Hier handelt es sich um Pauschalanlagen ohne Messung. D.h. die Verbrauchsdaten sind direkt über
     die Marktlokation abgreifbar.
     Beziehung 1 : 1 : Das ist die Standard-Beziehung für die meisten Fälle. In diesem Fall gibt es zu einer
@@ -99,29 +101,29 @@
     In den Zuordnungen sind ist die arithmetische Operation mit der der Verbrauch einer Messlokation zum Verbrauch einer
     Marktlokation beitrögt mit aufgeführt.
     Der Standard ist hier die Addition.
     """
 
     # only one of the following three optional attributes can be set
     #: Die Adresse, an der die Energie-Lieferung oder -Einspeisung erfolgt
-    lokationsadresse: Optional[Adresse] = None
-    geoadresse: Optional[Geokoordinaten] = None
+    lokationsadresse: Optional["Adresse"] = None
+    geoadresse: Optional["Geokoordinaten"] = None
     """
     Alternativ zu einer postalischen Adresse kann hier ein Ort mittels Geokoordinaten angegeben werden
     (z.B. zur Identifikation von Sendemasten).
     """
-    katasterinformation: Optional[Katasteradresse] = None
+    katasterinformation: Optional["Katasteradresse"] = None
     """
     Alternativ zu einer postalischen Adresse und Geokoordinaten kann hier eine Ortsangabe mittels Gemarkung und
     Flurstück erfolgen.
     """
 
-    kundengruppen: Optional[list[Kundentyp]] = None
+    kundengruppen: Optional[list["Kundentyp"]] = None
     #: Kundengruppen der Marktlokation
 
-    regelzone: Optional[
-        str
-    ] = None  #: für Strom. Code vom EIC, https://www.entsoe.eu/data/energy-identification-codes-eic/eic-approved-codes/
+    regelzone: Optional[str] = (
+        None  #: für Strom. Code vom EIC, https://www.entsoe.eu/data/energy-identification-codes-eic/eic-approved-codes/
+    )
     marktgebiet: Optional[str] = None  #: für Gas. Code vom EIC, https://www.entsog.eu/data/data-portal/codes-list
-    zaehlwerke: Optional[list[Zaehlwerk]] = None
-    verbrauchsmengen: Optional[list[Verbrauch]] = None
-    zaehlwerke_der_beteiligten_marktrolle: Optional[list[Zaehlwerk]] = None
+    zaehlwerke: Optional[list["Zaehlwerk"]] = None
+    verbrauchsmengen: Optional[list["Verbrauch"]] = None
+    zaehlwerke_der_beteiligten_marktrolle: Optional[list["Zaehlwerk"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/marktteilnehmer.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/marktteilnehmer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 Contains Marktteilnehmer class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..enum.marktrolle import Marktrolle
-from ..enum.rollencodetyp import Rollencodetyp
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .geschaeftspartner import Geschaeftspartner
+
+if TYPE_CHECKING:
+    from ..enum.marktrolle import Marktrolle
+    from ..enum.rollencodetyp import Rollencodetyp
+    from ..enum.sparte import Sparte
+    from .geschaeftspartner import Geschaeftspartner
 
 
 @postprocess_docstring
 class Marktteilnehmer(Geschaeftsobjekt):
     """
     Objekt zur Aufnahme der Information zu einem Marktteilnehmer
 
@@ -28,20 +30,20 @@
         <object data="../_static/images/bo4e/bo/Marktteilnehmer.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Marktteilnehmer JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Marktteilnehmer.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.MARKTTEILNEHMER
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.MARKTTEILNEHMER
     #: Gibt im Klartext die Bezeichnung der Marktrolle an
-    marktrolle: Optional[Marktrolle] = None
+    marktrolle: Optional["Marktrolle"] = None
     #: Gibt die Codenummer der Marktrolle an
     rollencodenummer: Optional[str] = None
     #: Gibt den Typ des Codes an
-    rollencodetyp: Optional[Rollencodetyp] = None
+    rollencodetyp: Optional["Rollencodetyp"] = None
     #: Sparte des Marktteilnehmers, z.B. Gas oder Strom
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
     #: Die 1:1-Kommunikationsadresse des Marktteilnehmers. Diese wird in der Marktkommunikation verwendet. Konkret kann dies eine eMail-Adresse oder ein AS4-Endpunkt sein.
     makoadresse: Optional[list[str]] = None
     #: Der zu diesem Marktteilnehmer gehörende Geschäftspartner
-    geschaeftspartner: Optional[Geschaeftspartner] = None
+    geschaeftspartner: Optional["Geschaeftspartner"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/messlokation.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/messlokation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 Contains Messlokation class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..bo.geraet import Geraet
-from ..com.adresse import Adresse
-from ..com.dienstleistung import Dienstleistung
-from ..com.geokoordinaten import Geokoordinaten
-from ..com.katasteradresse import Katasteradresse
-from ..enum.netzebene import Netzebene
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .zaehler import Zaehler
+
+if TYPE_CHECKING:
+    from ..bo.geraet import Geraet
+    from ..com.adresse import Adresse
+    from ..com.dienstleistung import Dienstleistung
+    from ..com.geokoordinaten import Geokoordinaten
+    from ..com.katasteradresse import Katasteradresse
+    from ..enum.netzebene import Netzebene
+    from ..enum.sparte import Sparte
+    from .zaehler import Zaehler
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 
 
 @postprocess_docstring
 class Messlokation(Geschaeftsobjekt):
     """
@@ -32,52 +34,52 @@
         <object data="../_static/images/bo4e/bo/Messlokation.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Messlokation JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Messlokation.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.MESSLOKATION
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.MESSLOKATION
     #: Die Messlokations-Identifikation; Das ist die frühere Zählpunktbezeichnung
     messlokations_id: Optional[str] = None
     #: Sparte der Messlokation, z.B. Gas oder Strom
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
 
     #: Spannungsebene der Messung
-    netzebene_messung: Optional[Netzebene] = None
+    netzebene_messung: Optional["Netzebene"] = None
     #: Die Nummer des Messgebietes in der ene't-Datenbank
     messgebietnr: Optional[str] = None
     #: Liste der Geräte, die zu dieser Messstelle gehört
-    geraete: Optional[list[Geraet]] = None
+    geraete: Optional[list["Geraet"]] = None
     #: Liste der Messdienstleistungen, die zu dieser Messstelle gehört
-    messdienstleistung: Optional[list[Dienstleistung]] = None  # todo: rename to plural
+    messdienstleistung: Optional[list["Dienstleistung"]] = None  # todo: rename to plural
     #: Zähler, die zu dieser Messlokation gehören
-    messlokationszaehler: Optional[list[Zaehler]] = None
+    messlokationszaehler: Optional[list["Zaehler"]] = None
 
     # only one of the following two optional codenr attributes can be set
     grundzustaendiger_msb_codenr: Optional[str] = None
     """
     Codenummer des grundzuständigen Messstellenbetreibers, der für diese Messlokation zuständig ist.
     (Dieser ist immer dann Messstellenbetreiber, wenn kein anderer MSB die Einrichtungen an der Messlokation betreibt.)
     """
     grundzustaendiger_msbim_codenr: Optional[str] = None
     """
     Codenummer des grundzuständigen Messstellenbetreibers für intelligente Messsysteme, der für diese Messlokation
     zuständig ist.
     (Dieser ist immer dann Messstellenbetreiber, wenn kein anderer MSB die Einrichtungen an der Messlokation betreibt.)
     """
     # only one of the following three optional address attributes can be set
-    messadresse: Optional[Adresse] = None
+    messadresse: Optional["Adresse"] = None
     """
     Die Adresse, an der die Messeinrichtungen zu finden sind.
     (Nur angeben, wenn diese von der Adresse der Marktlokation abweicht.)
     """
-    geoadresse: Optional[Geokoordinaten] = None
+    geoadresse: Optional["Geokoordinaten"] = None
     """
     Alternativ zu einer postalischen Adresse kann hier ein Ort mittels Geokoordinaten angegeben werden
     (z.B. zur Identifikation von Sendemasten).
     """
-    katasterinformation: Optional[Katasteradresse] = None
+    katasterinformation: Optional["Katasteradresse"] = None
     """
     Alternativ zu einer postalischen Adresse und Geokoordinaten kann hier eine Ortsangabe mittels Gemarkung und
     Flurstück erfolgen.
     """
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/person.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/person.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 """
 Contains Person class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.adresse import Adresse
-from ..com.kontaktweg import Kontaktweg
-from ..com.zustaendigkeit import Zustaendigkeit
-from ..enum.anrede import Anrede
-from ..enum.titel import Titel
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
 
+if TYPE_CHECKING:
+    from ..com.adresse import Adresse
+    from ..com.kontaktweg import Kontaktweg
+    from ..com.zustaendigkeit import Zustaendigkeit
+    from ..enum.anrede import Anrede
+    from ..enum.titel import Titel
+
+
 # pylint: disable=too-many-instance-attributes, too-few-public-methods, disable=duplicate-code
 
 
 @postprocess_docstring
 class Person(Geschaeftsobjekt):
     """
     Object containing information about a Person
@@ -30,31 +33,31 @@
         <object data="../_static/images/bo4e/bo/Person.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Person JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Person.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.PERSON
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.PERSON
     #: Mögliche Anrede der Person
-    anrede: Optional[Anrede] = None
+    anrede: Optional["Anrede"] = None
     individuelle_anrede: Optional[str] = None
     """
     Im Falle einer nicht standardisierten Anrede kann hier eine frei definierbare Anrede vorgegeben werden.
     Beispiel: "Vereinsgemeinschaft", "Pfarrer", "Hochwürdigster Herr Abt".
     """
     #: Möglicher Titel der Person
-    titel: Optional[Titel] = None
+    titel: Optional["Titel"] = None
     #: Vorname der Person
     vorname: Optional[str] = None
     #: Nachname (Familienname) der Person
     nachname: Optional[str] = None
     #: Kontaktwege der Person
-    kontaktwege: Optional[list[Kontaktweg]] = None
+    kontaktwege: Optional[list["Kontaktweg"]] = None
     #: Geburtsdatum der Person
     geburtsdatum: Optional[pydantic.AwareDatetime] = None
     #: Weitere Informationen zur Person
     kommentar: Optional[str] = None
     #: Liste der Abteilungen und Zuständigkeiten der Person
-    zustaendigkeiten: Optional[list[Zustaendigkeit]] = None
+    zustaendigkeiten: Optional[list["Zustaendigkeit"]] = None
     #: Adresse der Person, falls diese von der Adresse des Geschäftspartners abweicht
-    adresse: Optional[Adresse] = None
+    adresse: Optional["Adresse"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/preisblatt.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/preisblatt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Contains Preisblatt class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..com.preisposition import Preisposition
-from ..com.zeitraum import Zeitraum
-from ..enum.preisstatus import Preisstatus
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .marktteilnehmer import Marktteilnehmer
+
+if TYPE_CHECKING:
+    from ..com.preisposition import Preisposition
+    from ..com.zeitraum import Zeitraum
+    from ..enum.preisstatus import Preisstatus
+    from ..enum.sparte import Sparte
+    from .marktteilnehmer import Marktteilnehmer
 
 
 @postprocess_docstring
 class Preisblatt(Geschaeftsobjekt):
     """
     Das allgemeine Modell zur Abbildung von Preisen;
     Davon abgeleitet können, über die Zuordnung identifizierender Merkmale, spezielle Preisblatt-Varianten modelliert
@@ -34,20 +36,20 @@
         <object data="../_static/images/bo4e/bo/Preisblatt.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Preisblatt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Preisblatt.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.PREISBLATT
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.PREISBLATT
     #: Eine Bezeichnung für das Preisblatt
     bezeichnung: Optional[str] = None
     #: Preisblatt gilt für angegebene Sparte
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
     #: Merkmal, das anzeigt, ob es sich um vorläufige oder endgültige Preise handelt
-    preisstatus: Optional[Preisstatus] = None
+    preisstatus: Optional["Preisstatus"] = None
     #: Der Zeitraum für den der Preis festgelegt ist
-    gueltigkeit: Optional[Zeitraum] = None
+    gueltigkeit: Optional["Zeitraum"] = None
     #: Die einzelnen Positionen, die mit dem Preisblatt abgerechnet werden können. Z.B. Arbeitspreis, Grundpreis etc
-    preispositionen: Optional[list[Preisposition]] = None
+    preispositionen: Optional[list["Preisposition"]] = None
     #: Der Netzbetreiber, der die Preise veröffentlicht hat
-    herausgeber: Optional[Marktteilnehmer] = None
+    herausgeber: Optional["Marktteilnehmer"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/preisblattdienstleistung.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/preisblattdienstleistung.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Contains PreisblattDienstleistung class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..bo.geraet import Geraet
-from ..enum.bilanzierungsmethode import Bilanzierungsmethode
-from ..enum.dienstleistungstyp import Dienstleistungstyp
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .preisblatt import Preisblatt
 
+if TYPE_CHECKING:
+    from ..bo.geraet import Geraet
+    from ..enum.bilanzierungsmethode import Bilanzierungsmethode
+    from ..enum.dienstleistungstyp import Dienstleistungstyp
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class PreisblattDienstleistung(Preisblatt):
     """
     Variante des Preisblattmodells zur Abbildung der Preise für wahlfreie Dienstleistungen
@@ -26,19 +29,19 @@
         <object data="../_static/images/bo4e/bo/PreisblattDienstleistung.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `PreisblattDienstleistung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/PreisblattDienstleistung.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.PREISBLATTDIENSTLEISTUNG
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.PREISBLATTDIENSTLEISTUNG
     # required attributes (additional to those of Preisblatt)
     #: Die Preise gelten für Marktlokationen der angebebenen Bilanzierungsmethode
-    bilanzierungsmethode: Optional[Bilanzierungsmethode] = None
+    bilanzierungsmethode: Optional["Bilanzierungsmethode"] = None
     #: Dienstleistung, für die der Preis abgebildet wird, z.B. Sperrung/Entsperrung
-    basisdienstleistung: Optional[Dienstleistungstyp] = None
+    basisdienstleistung: Optional["Dienstleistungstyp"] = None
 
     #: Hier kann der Preis auf bestimmte Geräte eingegrenzt werden. Z.B. auf die Zählergröße
-    geraetedetails: Optional[Geraet] = None
+    geraetedetails: Optional["Geraet"] = None
 
     #: Weitere Dienstleistungen, die im Preis enthalten sind
-    inklusive_dienstleistungen: Optional[list[Dienstleistungstyp]] = None
+    inklusive_dienstleistungen: Optional[list["Dienstleistungstyp"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/preisblatthardware.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/preisblattmessung.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,52 @@
 """
-Contains PreisblattHardware class and corresponding marshmallow schema for de-/serialization
+Contains PreisblattMessung class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..bo.geraet import Geraet
-from ..enum.bilanzierungsmethode import Bilanzierungsmethode
-from ..enum.dienstleistungstyp import Dienstleistungstyp
-from ..enum.netzebene import Netzebene
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .preisblatt import Preisblatt
 
+if TYPE_CHECKING:
+    from ..bo.geraet import Geraet
+    from ..bo.zaehler import Zaehler
+    from ..enum.bilanzierungsmethode import Bilanzierungsmethode
+    from ..enum.dienstleistungstyp import Dienstleistungstyp
+    from ..enum.netzebene import Netzebene
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
-class PreisblattHardware(Preisblatt):
+class PreisblattMessung(Preisblatt):
     """
-    Variante des Preisblattmodells zur Abbildung der Preise für zusätzliche Hardware
+    Variante des Preisblattmodells zur Abbildung der Preise des Messstellenbetriebs und damit verbundener Leistungen
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/bo/PreisblattHardware.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/bo/PreisblattMessung.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `PreisblattHardware JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/PreisblattHardware.json>`_
+        `PreisblattMessung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/PreisblattMessung.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.PREISBLATTHARDWARE
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.PREISBLATTMESSUNG
     # required attributes (additional to those of Preisblatt)
     #: Die Preise gelten für Marktlokationen der angebebenen Bilanzierungsmethode
-    bilanzierungsmethode: Optional[Bilanzierungsmethode] = None
+    bilanzierungsmethode: Optional["Bilanzierungsmethode"] = None
     #: Die Preise gelten für Messlokationen in der angebebenen Netzebene
-    messebene: Optional[Netzebene] = None
+    messebene: Optional["Netzebene"] = None
 
-    #: Der Preis betriftt das hier angegebene Gerät, z.B. ein Tarifschaltgerät
-    basisgeraet: Optional[Geraet] = None
+    #: Der Preis betrifft den hier angegebenen Zähler, z.B. einen Drehstromzähler
+    zaehler: Optional["Zaehler"] = None
 
     #: Im Preis sind die hier angegebenen Dienstleistungen enthalten, z.B. Jährliche Ablesung
-    inklusive_dienstleistungen: Optional[list[Dienstleistungstyp]] = None
+    inklusive_dienstleistungen: Optional[list["Dienstleistungstyp"]] = None
 
     #: Im Preis sind die hier angegebenen Geräte mit enthalten, z.B. ein Wandler
-    inklusive_geraete: Optional[list[Geraet]] = None
+    inklusive_geraete: Optional[list["Geraet"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/preisblattkonzessionsabgabe.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/preisblattkonzessionsabgabe.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 Contains PreisblattKonzessionsabgabe class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..enum.kundengruppeka import KundengruppeKA
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .preisblatt import Preisblatt
 
+if TYPE_CHECKING:
+    from ..enum.kundengruppeka import KundengruppeKA
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class PreisblattKonzessionsabgabe(Preisblatt):
     """
     Die Variante des Preisblattmodells zur Abbildung von allgemeinen Abgaben
@@ -24,13 +27,13 @@
         <object data="../_static/images/bo4e/bo/PreisblattKonzessionsabgabe.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `PreisblattKonzessionsabgabe JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/PreisblattKonzessionsabgabe.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.PREISBLATTKONZESSIONSABGABE
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.PREISBLATTKONZESSIONSABGABE
     # required attributes (additional to those of Preisblatt)
     #: Kundegruppe anhand derer die Höhe der Konzessionabgabe festgelegt ist
-    kundengruppe_k_a: Optional[KundengruppeKA] = None
+    kundengruppe_k_a: Optional["KundengruppeKA"] = None
 
     # there are no optional attributes (additionally to those of Preisblatt)
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/preisblattmessung.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/preisblatthardware.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,51 @@
 """
-Contains PreisblattMessung class and corresponding marshmallow schema for de-/serialization
+Contains PreisblattHardware class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..bo.geraet import Geraet
-from ..bo.zaehler import Zaehler
-from ..enum.bilanzierungsmethode import Bilanzierungsmethode
-from ..enum.dienstleistungstyp import Dienstleistungstyp
-from ..enum.netzebene import Netzebene
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .preisblatt import Preisblatt
 
+if TYPE_CHECKING:
+    from ..bo.geraet import Geraet
+    from ..enum.bilanzierungsmethode import Bilanzierungsmethode
+    from ..enum.dienstleistungstyp import Dienstleistungstyp
+    from ..enum.netzebene import Netzebene
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
-class PreisblattMessung(Preisblatt):
+class PreisblattHardware(Preisblatt):
     """
-    Variante des Preisblattmodells zur Abbildung der Preise des Messstellenbetriebs und damit verbundener Leistungen
+    Variante des Preisblattmodells zur Abbildung der Preise für zusätzliche Hardware
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/bo/PreisblattMessung.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/bo/PreisblattHardware.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `PreisblattMessung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/PreisblattMessung.json>`_
+        `PreisblattHardware JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/PreisblattHardware.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.PREISBLATTMESSUNG
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.PREISBLATTHARDWARE
     # required attributes (additional to those of Preisblatt)
     #: Die Preise gelten für Marktlokationen der angebebenen Bilanzierungsmethode
-    bilanzierungsmethode: Optional[Bilanzierungsmethode] = None
+    bilanzierungsmethode: Optional["Bilanzierungsmethode"] = None
     #: Die Preise gelten für Messlokationen in der angebebenen Netzebene
-    messebene: Optional[Netzebene] = None
+    messebene: Optional["Netzebene"] = None
 
-    #: Der Preis betrifft den hier angegebenen Zähler, z.B. einen Drehstromzähler
-    zaehler: Optional[Zaehler] = None
+    #: Der Preis betriftt das hier angegebene Gerät, z.B. ein Tarifschaltgerät
+    basisgeraet: Optional["Geraet"] = None
 
     #: Im Preis sind die hier angegebenen Dienstleistungen enthalten, z.B. Jährliche Ablesung
-    inklusive_dienstleistungen: Optional[list[Dienstleistungstyp]] = None
+    inklusive_dienstleistungen: Optional[list["Dienstleistungstyp"]] = None
 
     #: Im Preis sind die hier angegebenen Geräte mit enthalten, z.B. ein Wandler
-    inklusive_geraete: Optional[list[Geraet]] = None
+    inklusive_geraete: Optional[list["Geraet"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/preisblattnetznutzung.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/preisblattnetznutzung.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Contains PreisblattNetnutzung class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..enum.bilanzierungsmethode import Bilanzierungsmethode
-from ..enum.kundengruppe import Kundengruppe
-from ..enum.netzebene import Netzebene
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .preisblatt import Preisblatt
 
+if TYPE_CHECKING:
+    from ..enum.bilanzierungsmethode import Bilanzierungsmethode
+    from ..enum.kundengruppe import Kundengruppe
+    from ..enum.netzebene import Netzebene
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class PreisblattNetznutzung(Preisblatt):
     """
     Die Variante des Preisblattmodells zur Abbildung der Netznutzungspreise
@@ -26,16 +29,16 @@
         <object data="../_static/images/bo4e/bo/PreisblattNetznutzung.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `PreisblattNetznutzung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/PreisblattNetznutzung.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.PREISBLATTNETZNUTZUNG
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.PREISBLATTNETZNUTZUNG
     # required attributes (additional to those of Preisblatt)
     #: Die Preise gelten für Marktlokationen der angebebenen Bilanzierungsmethode
-    bilanzierungsmethode: Optional[Bilanzierungsmethode] = None
+    bilanzierungsmethode: Optional["Bilanzierungsmethode"] = None
     #: Die Preise gelten für Marktlokationen in der angebebenen Netzebene
-    netzebene: Optional[Netzebene] = None
-    kundengruppe: Optional[Kundengruppe] = None
+    netzebene: Optional["Netzebene"] = None
+    kundengruppe: Optional["Kundengruppe"] = None
 
     # there are no optional attributes (additionally to those of Preisblatt)
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/rechnung.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/rechnung.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """
 Contains Rechnung class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.betrag import Betrag
-from ..com.rechnungsposition import Rechnungsposition
-from ..com.steuerbetrag import Steuerbetrag
-from ..com.zeitraum import Zeitraum
-from ..enum.netznutzungrechnungsart import NetznutzungRechnungsart
-from ..enum.netznutzungrechnungstyp import NetznutzungRechnungstyp
-from ..enum.rechnungsstatus import Rechnungsstatus
-from ..enum.rechnungstyp import Rechnungstyp
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .geschaeftspartner import Geschaeftspartner
-from .marktlokation import Marktlokation
-from .messlokation import Messlokation
+
+if TYPE_CHECKING:
+    from ..com.betrag import Betrag
+    from ..com.rechnungsposition import Rechnungsposition
+    from ..com.steuerbetrag import Steuerbetrag
+    from ..com.zeitraum import Zeitraum
+    from ..enum.netznutzungrechnungsart import NetznutzungRechnungsart
+    from ..enum.netznutzungrechnungstyp import NetznutzungRechnungstyp
+    from ..enum.rechnungsstatus import Rechnungsstatus
+    from ..enum.rechnungstyp import Rechnungstyp
+    from ..enum.sparte import Sparte
+    from .geschaeftspartner import Geschaeftspartner
+    from .marktlokation import Marktlokation
+    from .messlokation import Messlokation
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 
 
 @postprocess_docstring
 class Rechnung(Geschaeftsobjekt):
     """
@@ -37,66 +39,66 @@
         <object data="../_static/images/bo4e/bo/Rechnung.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Rechnung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Rechnung.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.RECHNUNG
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.RECHNUNG
     ist_storno: Optional[bool] = None
     """
     Kennzeichnung, ob es sich um eine Stornorechnung handelt;
     im Falle "true" findet sich im Attribut "originalrechnungsnummer" die Nummer der Originalrechnung.
     """
     #: Eine im Verwendungskontext eindeutige Nummer für die Rechnung
     rechnungsnummer: Optional[str] = None
     #: Ausstellungsdatum der Rechnung
     rechnungsdatum: Optional[pydantic.AwareDatetime] = None
     #: Zu diesem Datum ist die Zahlung fällig
     faelligkeitsdatum: Optional[pydantic.AwareDatetime] = None
     #: Ein kontextbezogender Rechnungstyp, z.B. Netznutzungsrechnung
-    rechnungstyp: Optional[Rechnungstyp] = None
+    rechnungstyp: Optional["Rechnungstyp"] = None
     #: Der Zeitraum der zugrunde liegenden Lieferung zur Rechnung
-    rechnungsperiode: Optional[Zeitraum] = None
+    rechnungsperiode: Optional["Zeitraum"] = None
     #: Der Aussteller der Rechnung, die Rollencodenummer kennt man über den im Geschäftspartner verlinkten Marktteilnehmer
-    rechnungsersteller: Optional[Geschaeftspartner] = None
+    rechnungsersteller: Optional["Geschaeftspartner"] = None
     #: Der Aussteller der Rechnung, die Rollencodenummer kennt man über den im Geschäftspartner verlinkten Marktteilnehmer
-    rechnungsempfaenger: Optional[Geschaeftspartner] = None
+    rechnungsempfaenger: Optional["Geschaeftspartner"] = None
     #: Die Summe der Nettobeträge der Rechnungsteile
-    gesamtnetto: Optional[Betrag] = None
+    gesamtnetto: Optional["Betrag"] = None
     #: Die Summe der Steuerbeträge der Rechnungsteile
-    gesamtsteuer: Optional[Betrag] = None
+    gesamtsteuer: Optional["Betrag"] = None
     #: Die Summe aus Netto- und Steuerbetrag
-    gesamtbrutto: Optional[Betrag] = None
+    gesamtbrutto: Optional["Betrag"] = None
     #: Der zu zahlende Betrag, der sich aus (gesamtbrutto - vorausbezahlt - rabattBrutto) ergibt
-    zu_zahlen: Optional[Betrag] = None
+    zu_zahlen: Optional["Betrag"] = None
     #: Die Rechnungspositionen
-    rechnungspositionen: Optional[list[Rechnungsposition]] = None
+    rechnungspositionen: Optional[list["Rechnungsposition"]] = None
     #: Bezeichnung für die vorliegende Rechnung
     rechnungstitel: Optional[str] = None
     #: Status der Rechnung zur Kennzeichnung des Bearbeitungsstandes
-    rechnungsstatus: Optional[Rechnungsstatus] = None
+    rechnungsstatus: Optional["Rechnungsstatus"] = None
     #: Im Falle einer Stornorechnung (storno = true) steht hier die Rechnungsnummer der stornierten Rechnung
     original_rechnungsnummer: Optional[str] = None
     #: Die Summe evtl. vorausgezahlter Beträge, z.B. Abschläge. Angabe als Bruttowert
-    vorausgezahlt: Optional[Betrag] = None
+    vorausgezahlt: Optional["Betrag"] = None
     #: Gesamtrabatt auf den Bruttobetrag
-    rabatt_brutto: Optional[Betrag] = None
-    steuerbetraege: Optional[list[Steuerbetrag]] = None
+    rabatt_brutto: Optional["Betrag"] = None
+    steuerbetraege: Optional[list["Steuerbetrag"]] = None
     """
     Eine Liste mit Steuerbeträgen pro Steuerkennzeichen/Steuersatz;
     die Summe dieser Beträge ergibt den Wert für gesamtsteuer.
     """
     #: Sparte (Strom, Gas ...) für die die Rechnung ausgestellt ist
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
     #: Aus der INVOIC entnommen, befüllt wenn es sich um eine Netznutzungsrechnung handelt
-    netznutzungrechnungsart: Optional[NetznutzungRechnungsart] = None
+    netznutzungrechnungsart: Optional["NetznutzungRechnungsart"] = None
     #: Aus der INVOIC entnommen, befüllt wenn es sich um eine Netznutzungsrechnung handelt
-    netznutzungrechnungstyp: Optional[NetznutzungRechnungstyp] = None
+    netznutzungrechnungstyp: Optional["NetznutzungRechnungstyp"] = None
     #: Kennzeichen, ob es sich um ein Original (true) oder eine Kopie handelt (false)
     ist_original: Optional[bool] = None
     #: Kennzeichen, ob es sich um eine simulierte Rechnung, z.B. zur Rechnungsprüfung handelt
     ist_simuliert: Optional[bool] = None
     #: Marktlokation, auf die sich die Rechnung bezieht
-    marktlokation: Optional[Marktlokation] = None
+    marktlokation: Optional["Marktlokation"] = None
     #: Messlokation, auf die sich die Rechnung bezieht
-    messlokation: Optional[Messlokation] = None
+    messlokation: Optional["Messlokation"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/region.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/region.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 Contains Region class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..com.regionskriterium import Regionskriterium
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
 
+if TYPE_CHECKING:
+    from ..com.regionskriterium import Regionskriterium
+
+
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class Region(Geschaeftsobjekt):
     """
@@ -25,16 +28,16 @@
         <object data="../_static/images/bo4e/bo/Region.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Region JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Region.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.REGION
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.REGION
     #: Bezeichnung der Region
     bezeichnung: Optional[str] = None
 
     #: Positivliste der Kriterien zur Definition der Region
-    positiv_liste: Optional[list[Regionskriterium]] = None
+    positiv_liste: Optional[list["Regionskriterium"]] = None
 
     #: Negativliste der Kriterien zur Definition der Region
-    negativ_liste: Optional[list[Regionskriterium]] = None
+    negativ_liste: Optional[list["Regionskriterium"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/regionaltarif.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/regionaltarif.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 """
 Contains Regionaltarif class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.regionalepreisgarantie import RegionalePreisgarantie
-from ..com.regionaleraufabschlag import RegionalerAufAbschlag
-from ..com.regionaletarifpreisposition import RegionaleTarifpreisposition
-from ..com.tarifberechnungsparameter import Tarifberechnungsparameter
-from ..com.tarifeinschraenkung import Tarifeinschraenkung
 from ..enum.typ import Typ
 from .tarifinfo import Tarifinfo
 
+if TYPE_CHECKING:
+    from ..com.regionalepreisgarantie import RegionalePreisgarantie
+    from ..com.regionaleraufabschlag import RegionalerAufAbschlag
+    from ..com.regionaletarifpreisposition import RegionaleTarifpreisposition
+    from ..com.tarifberechnungsparameter import Tarifberechnungsparameter
+    from ..com.tarifeinschraenkung import Tarifeinschraenkung
+
+
 # pylint: disable=too-few-public-methods, empty-docstring
 # pylint: disable=no-name-in-module
 
 
 class Regionaltarif(Tarifinfo):
     #: Abbildung eines Tarifs mit regionaler Zuordnung von Preisen und Auf- und Abschlägen.
     """
@@ -28,21 +31,21 @@
         <object data="../_static/images/bo4e/bo/Regionaltarif.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Regionaltarif JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Regionaltarif.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.REGIONALTARIF
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.REGIONALTARIF
     #: Gibt an, wann der Preis zuletzt angepasst wurde
     preisstand: Optional[pydantic.AwareDatetime] = None
     #: Für die Berechnung der Kosten sind die hier abgebildeten Parameter heranzuziehen
-    berechnungsparameter: Optional[Tarifberechnungsparameter] = None
+    berechnungsparameter: Optional["Tarifberechnungsparameter"] = None
     #: Die festgelegten Preise mit regionaler Eingrenzung, z.B. für Arbeitspreis, Grundpreis etc.
-    tarifpreise: Optional[list[RegionaleTarifpreisposition]] = None
+    tarifpreise: Optional[list["RegionaleTarifpreisposition"]] = None
 
     #: Auf- und Abschläge auf die Preise oder Kosten mit regionaler Eingrenzung
-    tarif_auf_abschlaege: Optional[list[RegionalerAufAbschlag]] = None
+    tarif_auf_abschlaege: Optional[list["RegionalerAufAbschlag"]] = None
     #: Festlegung von Garantien für bestimmte Preisanteile
-    preisgarantien: Optional[list[RegionalePreisgarantie]] = None
+    preisgarantien: Optional[list["RegionalePreisgarantie"]] = None
     #: Die Bedingungen und Einschränkungen unter denen ein Tarif angewendet werden kann
-    tarifeinschraenkung: Optional[Tarifeinschraenkung] = None
+    tarifeinschraenkung: Optional["Tarifeinschraenkung"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/standorteigenschaften.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/standorteigenschaften.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Contains Standorteigenschaften class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..com.standorteigenschaftengas import StandorteigenschaftenGas
-from ..com.standorteigenschaftenstrom import StandorteigenschaftenStrom
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
 
+if TYPE_CHECKING:
+    from ..com.standorteigenschaftengas import StandorteigenschaftenGas
+    from ..com.standorteigenschaftenstrom import StandorteigenschaftenStrom
+
 
 @postprocess_docstring
 class Standorteigenschaften(Geschaeftsobjekt):
     """
     Modelliert die regionalen und spartenspezifischen Eigenschaften einer gegebenen Adresse.
 
     .. raw:: html
@@ -26,13 +28,13 @@
         <object data="../_static/images/bo4e/bo/Standorteigenschaften.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Standorteigenschaften JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Standorteigenschaften.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.STANDORTEIGENSCHAFTEN
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.STANDORTEIGENSCHAFTEN
     #: Eigenschaften zur Sparte Strom
-    eigenschaften_strom: Optional[list[StandorteigenschaftenStrom]] = None
+    eigenschaften_strom: Optional[list["StandorteigenschaftenStrom"]] = None
 
     #: Eigenschaften zur Sparte Gas
-    eigenschaften_gas: Optional[StandorteigenschaftenGas] = None
+    eigenschaften_gas: Optional["StandorteigenschaftenGas"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/tarif.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/tarif.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 Contains Tarif class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.aufabschlagregional import AufAbschlagRegional
-from ..com.preisgarantie import Preisgarantie
-from ..com.tarifberechnungsparameter import Tarifberechnungsparameter
-from ..com.tarifeinschraenkung import Tarifeinschraenkung
-from ..com.tarifpreispositionproort import TarifpreispositionProOrt
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .tarifinfo import Tarifinfo
 
+if TYPE_CHECKING:
+    from ..com.aufabschlagregional import AufAbschlagRegional
+    from ..com.preisgarantie import Preisgarantie
+    from ..com.tarifberechnungsparameter import Tarifberechnungsparameter
+    from ..com.tarifeinschraenkung import Tarifeinschraenkung
+    from ..com.tarifpreispositionproort import TarifpreispositionProOrt
+
+
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class Tarif(Tarifinfo):
     """
@@ -30,25 +33,25 @@
         <object data="../_static/images/bo4e/bo/Tarif.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Tarif JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Tarif.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.TARIF
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.TARIF
     #: Gibt an, wann der Preis zuletzt angepasst wurde
     preisstand: Optional[pydantic.AwareDatetime] = None
     #: Für die Berechnung der Kosten sind die hier abgebildeten Parameter heranzuziehen
-    berechnungsparameter: Optional[Tarifberechnungsparameter] = None
+    berechnungsparameter: Optional["Tarifberechnungsparameter"] = None
     #: Die festgelegten Preise mit regionaler Eingrenzung z.B. für Arbeitspreis, Grundpreis etc.
-    tarifpreise: Optional[list[TarifpreispositionProOrt]] = None
+    tarifpreise: Optional[list["TarifpreispositionProOrt"]] = None
 
     #: Auf- und Abschläge auf die Preise oder Kosten mit regionaler Eingrenzung
-    tarif_auf_abschlaege: Optional[list[AufAbschlagRegional]] = None
+    tarif_auf_abschlaege: Optional[list["AufAbschlagRegional"]] = None
     # todo: fix inconsistency: RegionalerAufAbschlag vs. AufAbschlagRegional
     # https://github.com/Hochfrequenz/BO4E-python/issues/345
 
     #: Preisgarantie für diesen Tarif
-    preisgarantie: Optional[Preisgarantie] = None
+    preisgarantie: Optional["Preisgarantie"] = None
     # todo: fix inconsistency with regionaltarif https://github.com/Hochfrequenz/BO4E-python/issues/346
     #: Die Bedingungen und Einschränkungen unter denen ein Tarif angewendet werden kann
-    tarifeinschraenkung: Optional[Tarifeinschraenkung] = None
+    tarifeinschraenkung: Optional["Tarifeinschraenkung"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/tarifinfo.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/tarifinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """
 Contains Tarifinfo class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.energiemix import Energiemix
-from ..com.vertragskonditionen import Vertragskonditionen
-from ..com.zeitraum import Zeitraum
-from ..enum.kundentyp import Kundentyp
-from ..enum.registeranzahl import Registeranzahl
-from ..enum.sparte import Sparte
-from ..enum.tarifmerkmal import Tarifmerkmal
-from ..enum.tariftyp import Tariftyp
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .marktteilnehmer import Marktteilnehmer
+
+if TYPE_CHECKING:
+    from ..com.energiemix import Energiemix
+    from ..com.vertragskonditionen import Vertragskonditionen
+    from ..com.zeitraum import Zeitraum
+    from ..enum.kundentyp import Kundentyp
+    from ..enum.registeranzahl import Registeranzahl
+    from ..enum.sparte import Sparte
+    from ..enum.tarifmerkmal import Tarifmerkmal
+    from ..enum.tariftyp import Tariftyp
+    from .marktteilnehmer import Marktteilnehmer
 
 
 @postprocess_docstring
 class Tarifinfo(Geschaeftsobjekt):
     """
     Das BO Tarifinfo liefert die Merkmale, die einen Endkundentarif identifizierbar machen.
     Dieses BO dient als Basis für weitere BOs mit erweiterten Anwendungsmöglichkeiten.
@@ -35,41 +37,41 @@
         <object data="../_static/images/bo4e/bo/Tarifinfo.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Tarifinfo JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Tarifinfo.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.TARIFINFO
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.TARIFINFO
     #: Name des Tarifs
     bezeichnung: Optional[str] = None
     #: Der Name des Marktpartners, der den Tarif anbietet
     anbietername: Optional[str] = None
     #: Strom oder Gas, etc.
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
     #: Kundentypen für den der Tarif gilt, z.B. Privatkunden
-    kundentypen: Optional[list[Kundentyp]] = None
+    kundentypen: Optional[list["Kundentyp"]] = None
     #: Die Art des Tarifes, z.B. Eintarif oder Mehrtarif
-    registeranzahl: Optional[Registeranzahl] = None
+    registeranzahl: Optional["Registeranzahl"] = None
     #: Hinweis auf den Tariftyp, z.B. Grundversorgung oder Sondertarif
-    tariftyp: Optional[Tariftyp] = None
+    tariftyp: Optional["Tariftyp"] = None
     #: Weitere Merkmale des Tarifs, z.B. Festpreis oder Vorkasse
-    tarifmerkmale: Optional[list[Tarifmerkmal]] = None
+    tarifmerkmale: Optional[list["Tarifmerkmal"]] = None
     #: Der Marktteilnehmer (Lieferant), der diesen Tarif anbietet
-    anbieter: Optional[Marktteilnehmer] = None
+    anbieter: Optional["Marktteilnehmer"] = None
 
     #: Internetseite auf dem der Tarif zu finden ist
     website: Optional[str] = None
     #: Freitext
     bemerkung: Optional[str] = None
 
     #: Angabe, in welchem Zeitraum der Tarif gültig ist
-    zeitliche_gueltigkeit: Optional[Zeitraum] = None
+    zeitliche_gueltigkeit: Optional["Zeitraum"] = None
     #: Der Energiemix, der für diesen Tarif gilt
-    energiemix: Optional[Energiemix] = None
+    energiemix: Optional["Energiemix"] = None
     #: Mindestlaufzeiten und Kündigungsfristen zusammengefasst
-    vertragskonditionen: Optional[Vertragskonditionen] = None
+    vertragskonditionen: Optional["Vertragskonditionen"] = None
     anwendung_von: Optional[pydantic.AwareDatetime] = None
     """
     Angabe des inklusiven Zeitpunkts, ab dem der Tarif bzw. der Preis angewendet und abgerechnet wird,
     z.B. "2021-07-20T18:31:48Z"
     """
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/tarifkosten.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/tarifkosten.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 Contains Tarifkosten class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
-from .kosten import Kosten
 from .tarifinfo import Tarifinfo
 
+if TYPE_CHECKING:
+
+    from .kosten import Kosten
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Tarifkosten(Tarifinfo):
     """
     Objekt zur Kommunikation von Kosten, die im Rahmen der Tarifanwendung entstehen
@@ -25,15 +28,15 @@
         <object data="../_static/images/bo4e/bo/Tarifkosten.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Tarifkosten JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Tarifkosten.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.TARIFKOSTEN
-    kosten: Optional[Kosten] = None
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.TARIFKOSTEN
+    kosten: Optional["Kosten"] = None
     """
     Referenz (Link) zu einem Kostenobjekt, in dem die Kosten für die Anwendung
     des Tarifs auf eine Abnahmesituation berechnet wurden
     """
 
     # there are no optional attributes
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/tarifpreisblatt.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/tarifpreisblatt.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 Contains Tarifpreisblatt class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.aufabschlag import AufAbschlag
-from ..com.preisgarantie import Preisgarantie
-from ..com.tarifberechnungsparameter import Tarifberechnungsparameter
-from ..com.tarifeinschraenkung import Tarifeinschraenkung
-from ..com.tarifpreisposition import Tarifpreisposition
 from ..enum.typ import Typ
 from ..utils import postprocess_docstring
 from .tarifinfo import Tarifinfo
 
+if TYPE_CHECKING:
+    from ..com.aufabschlag import AufAbschlag
+    from ..com.preisgarantie import Preisgarantie
+    from ..com.tarifberechnungsparameter import Tarifberechnungsparameter
+    from ..com.tarifeinschraenkung import Tarifeinschraenkung
+    from ..com.tarifpreisposition import Tarifpreisposition
+
+
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class Tarifpreisblatt(Tarifinfo):
     """
@@ -30,22 +33,22 @@
         <object data="../_static/images/bo4e/bo/Tarifpreisblatt.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Tarifpreisblatt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Tarifpreisblatt.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.TARIFPREISBLATT
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.TARIFPREISBLATT
     # required attributes (additional to those of Tarifinfo)
     #: Gibt an, wann der Preis zuletzt angepasst wurde
     preisstand: Optional[pydantic.AwareDatetime] = None
     #: Die festgelegten Preise, z.B. für Arbeitspreis, Grundpreis etc.
-    tarifpreise: Optional[list[Tarifpreisposition]] = None
+    tarifpreise: Optional[list["Tarifpreisposition"]] = None
     #: Für die Berechnung der Kosten sind die hier abgebildeten Parameter heranzuziehen
-    berechnungsparameter: Optional[Tarifberechnungsparameter] = None
+    berechnungsparameter: Optional["Tarifberechnungsparameter"] = None
 
     #: Die Bedingungen und Einschränkungen unter denen ein Tarif angewendet werden kann
-    tarifeinschraenkung: Optional[Tarifeinschraenkung] = None
+    tarifeinschraenkung: Optional["Tarifeinschraenkung"] = None
     #: Festlegung von Garantien für bestimmte Preisanteile
-    preisgarantie: Optional[Preisgarantie] = None
+    preisgarantie: Optional["Preisgarantie"] = None
     #: Auf- und Abschläge auf die Preise oder Kosten
-    tarif_auf_abschlaege: Optional[list[AufAbschlag]] = None
+    tarif_auf_abschlaege: Optional[list["AufAbschlag"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/vertrag.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/vertrag.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 Contains Vertrag class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..com.unterschrift import Unterschrift
-from ..com.vertragskonditionen import Vertragskonditionen
-from ..com.vertragsteil import Vertragsteil
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
-from ..enum.vertragsart import Vertragsart
-from ..enum.vertragsstatus import Vertragsstatus
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .geschaeftspartner import Geschaeftspartner
+
+if TYPE_CHECKING:
+    from ..com.unterschrift import Unterschrift
+    from ..com.vertragskonditionen import Vertragskonditionen
+    from ..com.vertragsteil import Vertragsteil
+    from ..enum.sparte import Sparte
+    from ..enum.vertragsart import Vertragsart
+    from ..enum.vertragsstatus import Vertragsstatus
+    from .geschaeftspartner import Geschaeftspartner
 
 # pylint: disable=unused-argument
 # pylint: disable=no-name-in-module
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 
 
@@ -36,48 +38,48 @@
         <object data="../_static/images/bo4e/bo/Vertrag.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Vertrag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Vertrag.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.VERTRAG
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.VERTRAG
     # pylint: disable=duplicate-code
     #: Eine im Verwendungskontext eindeutige Nummer für den Vertrag
     vertragsnummer: Optional[str] = None
     #: Hier ist festgelegt, um welche Art von Vertrag es sich handelt.
-    vertragsart: Optional[Vertragsart] = None
+    vertragsart: Optional["Vertragsart"] = None
     #: Gibt den Status des Vertrags an
-    vertragsstatus: Optional[Vertragsstatus] = None
+    vertragsstatus: Optional["Vertragsstatus"] = None
     #: Unterscheidungsmöglichkeiten für die Sparte
-    sparte: Optional[Sparte] = None
+    sparte: Optional["Sparte"] = None
     #: Gibt an, wann der Vertrag beginnt (inklusiv)
     vertragsbeginn: Optional[pydantic.AwareDatetime] = None
     #: Gibt an, wann der Vertrag (voraussichtlich) endet oder beendet wurde (exklusiv)
     vertragsende: Optional[pydantic.AwareDatetime] = None
     # todo: add von/bis validator
-    vertragspartner1: Optional[Geschaeftspartner] = None
+    vertragspartner1: Optional["Geschaeftspartner"] = None
     """
     Der "erstgenannte" Vertragspartner.
     In der Regel der Aussteller des Vertrags.
     Beispiel: "Vertrag zwischen Vertragspartner 1 ..."
     """
-    vertragspartner2: Optional[Geschaeftspartner] = None
+    vertragspartner2: Optional["Geschaeftspartner"] = None
     """
     Der "zweitgenannte" Vertragspartner.
     In der Regel der Empfänger des Vertrags.
     Beispiel "Vertrag zwischen Vertragspartner 1 und Vertragspartner 2".
     """
-    vertragsteile: Optional[list[Vertragsteil]] = None
+    vertragsteile: Optional[list["Vertragsteil"]] = None
     """
     Der Vertragsteil wird dazu verwendet, eine vertragliche Leistung in Bezug zu einer Lokation
     (Markt- oder Messlokation) festzulegen.
     """
 
     #: Beschreibung zum Vertrag
     beschreibung: Optional[str] = None
     #: Festlegungen zu Laufzeiten und Kündigungsfristen
-    vertragskonditionen: Optional[Vertragskonditionen] = None
+    vertragskonditionen: Optional["Vertragskonditionen"] = None
     #: Unterzeichner des Vertragspartners 1
-    unterzeichnervp1: Optional[list[Unterschrift]] = None
+    unterzeichnervp1: Optional[list["Unterschrift"]] = None
     #: Unterzeichner des Vertragspartners 2
-    unterzeichnervp2: Optional[list[Unterschrift]] = None
+    unterzeichnervp2: Optional[list["Unterschrift"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/zaehler.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/zaehler.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,33 +3,35 @@
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
 
 # pylint: disable=unused-argument
 # pylint: disable=no-name-in-module
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 import pydantic
 from pydantic import Field
 
-from ..bo.geraet import Geraet
-from ..com.zaehlwerk import Zaehlwerk
-from ..enum.befestigungsart import Befestigungsart
-from ..enum.messwerterfassung import Messwerterfassung
-from ..enum.registeranzahl import Registeranzahl
-from ..enum.sparte import Sparte
 from ..enum.typ import Typ
-from ..enum.zaehlerauspraegung import Zaehlerauspraegung
-from ..enum.zaehlergroesse import Zaehlergroesse
-from ..enum.zaehlertyp import Zaehlertyp
-from ..enum.zaehlertypspezifikation import ZaehlertypSpezifikation
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
-from .geschaeftspartner import Geschaeftspartner
+
+if TYPE_CHECKING:
+    from ..bo.geraet import Geraet
+    from ..com.zaehlwerk import Zaehlwerk
+    from ..enum.befestigungsart import Befestigungsart
+    from ..enum.messwerterfassung import Messwerterfassung
+    from ..enum.registeranzahl import Registeranzahl
+    from ..enum.sparte import Sparte
+    from ..enum.zaehlerauspraegung import Zaehlerauspraegung
+    from ..enum.zaehlergroesse import Zaehlergroesse
+    from ..enum.zaehlertyp import Zaehlertyp
+    from ..enum.zaehlertypspezifikation import ZaehlertypSpezifikation
+    from .geschaeftspartner import Geschaeftspartner
 
 # pylint: disable=too-many-instance-attributes, too-few-public-methods
 
 
 @postprocess_docstring
 class Zaehler(Geschaeftsobjekt):
     """
@@ -40,26 +42,28 @@
         <object data="../_static/images/bo4e/bo/Zaehler.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Zaehler JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Zaehler.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.ZAEHLER
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.ZAEHLER
     zaehlernummer: Optional[str] = None  #: Nummerierung des Zählers,vergeben durch den Messstellenbetreiber
-    sparte: Optional[Sparte] = None  #: Strom oder Gas
-    zaehlerauspraegung: Optional[Zaehlerauspraegung] = None  #: Spezifikation die Richtung des Zählers betreffend
-    zaehlertyp: Optional[Zaehlertyp] = None  #: Typisierung des Zählers
-    zaehlwerke: Optional[list[Zaehlwerk]] = None
-    registeranzahl: Optional[Registeranzahl] = None  #: Spezifikation bezüglich unterstützter Tarif
+    sparte: Optional["Sparte"] = None  #: Strom oder Gas
+    zaehlerauspraegung: Optional["Zaehlerauspraegung"] = None  #: Spezifikation die Richtung des Zählers betreffend
+    zaehlertyp: Optional["Zaehlertyp"] = None  #: Typisierung des Zählers
+    zaehlwerke: Optional[list["Zaehlwerk"]] = None
+    registeranzahl: Optional["Registeranzahl"] = None  #: Spezifikation bezüglich unterstützter Tarif
     zaehlerkonstante: Optional[Decimal] = None  #: Zählerkonstante auf dem Zähler
     eichung_bis: Optional[pydantic.AwareDatetime] = None  #: Bis zu diesem Datum (exklusiv) ist der Zähler geeicht.
-    letzte_eichung: Optional[
-        pydantic.AwareDatetime
-    ] = None  #: Zu diesem Datum fand die letzte Eichprüfung des Zählers statt.
-    zaehlerhersteller: Optional[Geschaeftspartner] = None  #: Der Hersteller des Zählers
+    letzte_eichung: Optional[pydantic.AwareDatetime] = (
+        None  #: Zu diesem Datum fand die letzte Eichprüfung des Zählers statt.
+    )
+    zaehlerhersteller: Optional["Geschaeftspartner"] = None  #: Der Hersteller des Zählers
     ist_fernschaltbar: Optional[bool] = None  #: Fernschaltung
-    messwerterfassung: Optional[Messwerterfassung] = None  #: Messwerterfassung des Zählers
-    zaehlertypSpezifikation: Optional[ZaehlertypSpezifikation] = None  #: Besondere Spezifikation des Zählers
-    befestigungsart: Optional[Befestigungsart] = None  #: Befestigungsart
-    zaehlergroesse: Optional[Zaehlergroesse] = None  #: Größe des Zählers
-    geraete: Optional[list[Geraet]] = None  #: Liste der Geräte, die zu diesem Zähler gehören, bspw. Smartmeter-Gateway
+    messwerterfassung: Optional["Messwerterfassung"] = None  #: Messwerterfassung des Zählers
+    zaehlertypSpezifikation: Optional["ZaehlertypSpezifikation"] = None  #: Besondere Spezifikation des Zählers
+    befestigungsart: Optional["Befestigungsart"] = None  #: Befestigungsart
+    zaehlergroesse: Optional["Zaehlergroesse"] = None  #: Größe des Zählers
+    geraete: Optional[list["Geraet"]] = (
+        None  #: Liste der Geräte, die zu diesem Zähler gehören, bspw. Smartmeter-Gateway
+    )
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/bo/zeitreihe.py` & `bo4e-202401.1.2rc14/src/bo4e/bo/zeitreihe.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
 Contains Zeitreihe class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
-from typing import Annotated, Optional
+from typing import TYPE_CHECKING, Annotated, Optional
 
 from pydantic import Field
 
-from ..com.zeitreihenwert import Zeitreihenwert
-from ..enum.medium import Medium
-from ..enum.mengeneinheit import Mengeneinheit
-from ..enum.messart import Messart
-from ..enum.messgroesse import Messgroesse
 from ..enum.typ import Typ
-from ..enum.wertermittlungsverfahren import Wertermittlungsverfahren
 from ..utils import postprocess_docstring
 from .geschaeftsobjekt import Geschaeftsobjekt
 
+if TYPE_CHECKING:
+    from ..com.zeitreihenwert import Zeitreihenwert
+    from ..enum.medium import Medium
+    from ..enum.mengeneinheit import Mengeneinheit
+    from ..enum.messart import Messart
+    from ..enum.messgroesse import Messgroesse
+    from ..enum.wertermittlungsverfahren import Wertermittlungsverfahren
+
 
 @postprocess_docstring
 class Zeitreihe(Geschaeftsobjekt):
     """
     Abbildung einer allgemeinen Zeitreihe mit einem Wertvektor.
     Die Werte können mit wahlfreier zeitlicher Distanz im Vektor abgelegt sein.
 
@@ -30,27 +32,27 @@
         <object data="../_static/images/bo4e/bo/Zeitreihe.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Zeitreihe JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/bo/Zeitreihe.json>`_
 
     """
 
-    typ: Annotated[Optional[Typ], Field(alias="_typ")] = Typ.ZEITREIHE
+    typ: Annotated[Optional["Typ"], Field(alias="_typ")] = Typ.ZEITREIHE
     #: Bezeichnung für die Zeitreihe
     bezeichnung: Optional[str] = None
     #: Beschreibt, was gemessen wurde (z.B. Strom, Spannung, Wirkleistung, Scheinleistung)
-    messgroesse: Optional[Messgroesse] = None
+    messgroesse: Optional["Messgroesse"] = None
     #: Beschreibt die Art der Messung (z.B. aktueller Wert, mittlerer Wert, maximaler Wert)
-    messart: Optional[Messart] = None
+    messart: Optional["Messart"] = None
     #: Medium, das gemessen wurde (z.B. Wasser, Dampf, Strom, Gas)
-    medium: Optional[Medium] = None
+    medium: Optional["Medium"] = None
     #: Alle Werte in der Tabelle haben die Einheit, die hier angegeben ist
-    einheit: Optional[Mengeneinheit] = None
+    einheit: Optional["Mengeneinheit"] = None
     #: Hier liegen jeweils die Werte
-    werte: Optional[list[Zeitreihenwert]] = None
+    werte: Optional[list["Zeitreihenwert"]] = None
 
     #: Beschreibt die Verwendung der Zeitreihe
     beschreibung: Optional[str] = None
     #: Version der Zeitreihe
     version: Optional[str] = None
     #: Kennzeichnung, wie die Werte entstanden sind, z.B. durch Messung
-    wertherkunft: Optional[Wertermittlungsverfahren] = None
+    wertherkunft: Optional["Wertermittlungsverfahren"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/adresse.py` & `bo4e-202401.1.2rc14/src/bo4e/com/adresse.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,8 +40,8 @@
     #: Im Falle einer Postfachadresse das Postfach; Damit werden Straße und Hausnummer nicht berücksichtigt
     postfach: Optional[str] = None
     #: Zusatzhinweis zum Auffinden der Adresse, z.B. "3. Stock linke Wohnung"
     adresszusatz: Optional[str] = None
     #: Im Falle einer c/o-Adresse steht in diesem Attribut die Anrede. Z.B. "c/o Veronica Hauptmieterin"
     co_ergaenzung: Optional[str] = None
     #: Offizieller ISO-Landescode
-    landescode: Optional[Landescode] = Landescode.DE  # type:ignore
+    landescode: Optional["Landescode"] = Landescode.DE  # type:ignore
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/angebotsposition.py` & `bo4e-202401.1.2rc14/src/bo4e/com/angebotsposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Contains Angebotsposition class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from ..utils import postprocess_docstring
-from .betrag import Betrag
 from .com import COM
-from .menge import Menge
-from .preis import Preis
+
+if TYPE_CHECKING:
+
+    from .betrag import Betrag
+    from .menge import Menge
+    from .preis import Preis
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Angebotsposition(COM):
     """
@@ -31,16 +34,16 @@
         `Angebotsposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Angebotsposition.json>`_
 
     """
 
     #: Bezeichnung der jeweiligen Position des Angebotsteils
     positionsbezeichnung: Optional[str] = None
     #: Preis pro Einheit/Stückpreis des angebotenen Artikels.
-    positionspreis: Optional[Preis] = None
+    positionspreis: Optional["Preis"] = None
 
     #: Menge des angebotenen Artikels (z.B. Wirkarbeit in kWh), in dieser Angebotsposition
-    positionsmenge: Optional[Menge] = None
+    positionsmenge: Optional["Menge"] = None
     #: Kosten (positionspreis * positionsmenge) für diese Angebotsposition
-    positionskosten: Optional[Betrag] = None
+    positionskosten: Optional["Betrag"] = None
 
     # for a preis = menge*times validation we first need to resolve
     # https://github.com/Hochfrequenz/BO4E-python/issues/126
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/angebotsteil.py` & `bo4e-202401.1.2rc14/src/bo4e/com/angebotsteil.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Contains Angebotsteil class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..bo.marktlokation import Marktlokation
 from ..utils import postprocess_docstring
-from .angebotsposition import Angebotsposition
-from .betrag import Betrag
 from .com import COM
-from .menge import Menge
-from .zeitraum import Zeitraum
+
+if TYPE_CHECKING:
+    from ..bo.marktlokation import Marktlokation
+    from .angebotsposition import Angebotsposition
+    from .betrag import Betrag
+    from .menge import Menge
+    from .zeitraum import Zeitraum
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class Angebotsteil(COM):
@@ -32,22 +34,22 @@
 
     .. HINT::
         `Angebotsteil JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Angebotsteil.json>`_
 
     """
 
     #: Einzelne Positionen, die zu diesem Angebotsteil gehören
-    positionen: Optional[list[Angebotsposition]] = None
+    positionen: Optional[list["Angebotsposition"]] = None
 
     #: Identifizierung eines Subkapitels einer Anfrage, beispielsweise das Los einer Ausschreibung
     anfrage_subreferenz: Optional[str] = None
-    lieferstellenangebotsteil: Optional[list[Marktlokation]] = None
+    lieferstellenangebotsteil: Optional[list["Marktlokation"]] = None
     """
     Marktlokationen, für die dieses Angebotsteil gilt, falls vorhanden.
     Durch die Marktlokation ist auch die Lieferadresse festgelegt
     """
     #: Summe der Verbräuche aller in diesem Angebotsteil eingeschlossenen Lieferstellen
-    gesamtmengeangebotsteil: Optional[Menge] = None
+    gesamtmengeangebotsteil: Optional["Menge"] = None
     #: Summe der Jahresenergiekosten aller in diesem Angebotsteil enthaltenen Lieferstellen
-    gesamtkostenangebotsteil: Optional[Betrag] = None
+    gesamtkostenangebotsteil: Optional["Betrag"] = None
     #: Hier kann der Belieferungszeitraum angegeben werden, für den dieser Angebotsteil gilt
-    lieferzeitraum: Optional[Zeitraum] = None
+    lieferzeitraum: Optional["Zeitraum"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/angebotsvariante.py` & `bo4e-202401.1.2rc14/src/bo4e/com/angebotsvariante.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 Contains Angebotsvariante and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 import pydantic
 
-from ..enum.angebotsstatus import Angebotsstatus
 from ..utils import postprocess_docstring
-from .angebotsteil import Angebotsteil
-from .betrag import Betrag
 from .com import COM
-from .menge import Menge
+
+if TYPE_CHECKING:
+    from ..enum.angebotsstatus import Angebotsstatus
+    from .angebotsteil import Angebotsteil
+    from .betrag import Betrag
+    from .menge import Menge
 
 
 @postprocess_docstring
 class Angebotsvariante(COM):
     """
     Führt die verschiedenen Ausprägungen der Angebotsberechnung auf
 
@@ -27,27 +29,27 @@
 
     .. HINT::
         `Angebotsvariante JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Angebotsvariante.json>`_
 
     """
 
     #: Gibt den Status eines Angebotes an.
-    angebotsstatus: Optional[Angebotsstatus] = None
+    angebotsstatus: Optional["Angebotsstatus"] = None
 
     #: Datum der Erstellung der Angebotsvariante
     erstellungsdatum: Optional[pydantic.AwareDatetime] = None
 
     #: Bis zu diesem Zeitpunkt gilt die Angebotsvariante
     bindefrist: Optional[pydantic.AwareDatetime] = None
 
-    teile: Optional[list[Angebotsteil]] = None
+    teile: Optional[list["Angebotsteil"]] = None
     """
     Angebotsteile werden im einfachsten Fall für eine Marktlokation oder Lieferstellenadresse erzeugt.
     Hier werden die Mengen und Gesamtkosten aller Angebotspositionen zusammengefasst.
     Eine Variante besteht mindestens aus einem Angebotsteil.
     """
 
     #: Aufsummierte Wirkarbeitsmenge aller Angebotsteile
-    gesamtmenge: Optional[Menge] = None
+    gesamtmenge: Optional["Menge"] = None
     # todo: write a validator for this: https://github.com/Hochfrequenz/BO4E-python/issues/320
     #: Aufsummierte Kosten aller Angebotsteile
-    gesamtkosten: Optional[Betrag] = None
+    gesamtkosten: Optional["Betrag"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/aufabschlag.py` & `bo4e-202401.1.2rc14/src/bo4e/com/aufabschlag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Contains AufAbschlag class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.aufabschlagstyp import AufAbschlagstyp
-from ..enum.aufabschlagsziel import AufAbschlagsziel
-from ..enum.waehrungseinheit import Waehrungseinheit
 from ..utils import postprocess_docstring
 from .com import COM
-from .preisstaffel import Preisstaffel
-from .zeitraum import Zeitraum
+
+if TYPE_CHECKING:
+    from ..enum.aufabschlagstyp import AufAbschlagstyp
+    from ..enum.aufabschlagsziel import AufAbschlagsziel
+    from ..enum.waehrungseinheit import Waehrungseinheit
+    from .preisstaffel import Preisstaffel
+    from .zeitraum import Zeitraum
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 
 
 @postprocess_docstring
 class AufAbschlag(COM):
     """
@@ -30,22 +32,22 @@
         `AufAbschlag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/AufAbschlag.json>`_
 
     """
 
     #: Bezeichnung des Auf-/Abschlags
     bezeichnung: Optional[str] = None
     #: Werte für die gestaffelten Auf/Abschläge.
-    staffeln: Optional[list[Preisstaffel]] = None
+    staffeln: Optional[list["Preisstaffel"]] = None
 
     #: Beschreibung zum Auf-/Abschlag
     beschreibung: Optional[str] = None
     #: Typ des Aufabschlages (z.B. absolut oder prozentual).
-    auf_abschlagstyp: Optional[AufAbschlagstyp] = None
+    auf_abschlagstyp: Optional["AufAbschlagstyp"] = None
     #: Diesem Preis oder den Kosten ist der Auf/Abschlag zugeordnet. Z.B. Arbeitspreis, Gesamtpreis etc..
-    auf_abschlagsziel: Optional[AufAbschlagsziel] = None
-    einheit: Optional[Waehrungseinheit] = None
+    auf_abschlagsziel: Optional["AufAbschlagsziel"] = None
+    einheit: Optional["Waehrungseinheit"] = None
     """ Gibt an in welcher Währungseinheit der Auf/Abschlag berechnet wird. Euro oder Ct..
     (Nur im Falle absoluter Aufschlagstypen). """
     #: Internetseite, auf der die Informationen zum Auf-/Abschlag veröffentlicht sind.
     website: Optional[str] = None
     #: Internetseite, auf der die Informationen zum Auf-/Abschlag veröffentlicht sind.
-    gueltigkeitszeitraum: Optional[Zeitraum] = None
+    gueltigkeitszeitraum: Optional["Zeitraum"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagproort.py` & `bo4e-202401.1.2rc14/src/bo4e/com/aufabschlagproort.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
 Contains AufAbschlagProOrt class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from ..utils import postprocess_docstring
-from .aufabschlagstaffelproort import AufAbschlagstaffelProOrt
 from .com import COM
 
+if TYPE_CHECKING:
+
+    from .aufabschlagstaffelproort import AufAbschlagstaffelProOrt
+
+
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class AufAbschlagProOrt(COM):
     """
@@ -31,8 +35,8 @@
     #: Die Postleitzahl des Ortes für den der Aufschlag gilt.
     postleitzahl: Optional[str] = None
     #: Der Ort für den der Aufschlag gilt.
     ort: Optional[str] = None
     #: Die ene't-Netznummer des Netzes in dem der Aufschlag gilt.
     netznr: Optional[str] = None
     #: Werte für die gestaffelten Auf/Abschläge mit regionaler Eingrenzung.
-    staffeln: Optional[list[AufAbschlagstaffelProOrt]] = None
+    staffeln: Optional[list["AufAbschlagstaffelProOrt"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagregional.py` & `bo4e-202401.1.2rc14/src/bo4e/com/aufabschlagregional.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Contains AufAbschlagRegional and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.aufabschlagstyp import AufAbschlagstyp
-from ..enum.aufabschlagsziel import AufAbschlagsziel
-from ..enum.waehrungseinheit import Waehrungseinheit
+from ..utils import postprocess_docstring
 
 # pylint: disable=R0801
-from ..utils import postprocess_docstring
-from .aufabschlagproort import AufAbschlagProOrt
 from .com import COM
-from .energiemix import Energiemix
-from .preisgarantie import Preisgarantie
-from .tarifeinschraenkung import Tarifeinschraenkung
-from .vertragskonditionen import Vertragskonditionen
-from .zeitraum import Zeitraum
+
+if TYPE_CHECKING:
+    from ..enum.aufabschlagstyp import AufAbschlagstyp
+    from ..enum.aufabschlagsziel import AufAbschlagsziel
+    from ..enum.waehrungseinheit import Waehrungseinheit
+    from .aufabschlagproort import AufAbschlagProOrt
+    from .energiemix import Energiemix
+    from .preisgarantie import Preisgarantie
+    from .tarifeinschraenkung import Tarifeinschraenkung
+    from .vertragskonditionen import Vertragskonditionen
+    from .zeitraum import Zeitraum
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class AufAbschlagRegional(COM):
@@ -39,39 +41,39 @@
 
     """
 
     # required attributess
     #: Bezeichnung des Auf-/Abschlags
     bezeichnung: Optional[str] = None
     #: Werte für die gestaffelten Auf/Abschläge mit regionaler Eingrenzung
-    betraege: Optional[list[AufAbschlagProOrt]] = None
+    betraege: Optional[list["AufAbschlagProOrt"]] = None
 
     #: Beschreibung zum Auf-/Abschlag
     beschreibung: Optional[str] = None
     #:Typ des Aufabschlages (z.B. absolut oder prozentual)
-    auf_abschlagstyp: Optional[AufAbschlagstyp] = None
+    auf_abschlagstyp: Optional["AufAbschlagstyp"] = None
     #: Diesem Preis oder den Kosten ist der Auf/Abschlag zugeordnet. Z.B. Arbeitspreis, Gesamtpreis etc.
-    auf_abschlagsziel: Optional[AufAbschlagsziel] = None
+    auf_abschlagsziel: Optional["AufAbschlagsziel"] = None
     #: Gibt an in welcher Währungseinheit der Auf/Abschlag berechnet wird. Euro oder Ct.
-    einheit: Optional[Waehrungseinheit] = None
+    einheit: Optional["Waehrungseinheit"] = None
     #: Internetseite, auf der die Informationen zum Auf-/Abschlag veröffentlicht sind
     website: Optional[str] = None
     #: Zusatzprodukte, die nur in Kombination mit diesem AufAbschlag erhältlich sind
     zusatzprodukte: Optional[list[str]] = None
     #: Voraussetzungen, die erfüllt sein müssen, damit dieser AufAbschlag zur Anwendung kommen kann
     voraussetzungen: Optional[list[str]] = None
     #: Durch die Anwendung des Auf/Abschlags kann eine Änderung des Tarifnamens auftreten.
     tarifnamensaenderungen: Optional[str] = None
     #: Zeitraum, in dem der Abschlag zur Anwendung kommen kann
-    gueltigkeitszeitraum: Optional[Zeitraum] = None
-    energiemixaenderung: Optional[Energiemix] = None
+    gueltigkeitszeitraum: Optional["Zeitraum"] = None
+    energiemixaenderung: Optional["Energiemix"] = None
     """ Der Energiemix kann sich durch einen AufAbschlag ändern (z.B. zwei Cent Aufschlag für Ökostrom:
     Sollte dies der Fall sein, wird hier die neue Zusammensetzung des Energiemix angegeben."""
-    vertagskonditionsaenderung: Optional[Vertragskonditionen] = None
+    vertagskonditionsaenderung: Optional["Vertragskonditionen"] = None
     """ Änderungen in den Vertragskonditionen. Falls in dieser Komponenten angegeben,
     werden die Tarifparameter hiermit überschrieben."""
-    garantieaenderung: Optional[Preisgarantie] = None
+    garantieaenderung: Optional["Preisgarantie"] = None
     """ Änderungen in den Garantievereinbarungen. Falls in dieser Komponenten angegeben,
     werden die Tarifparameter hiermit überschrieben."""
-    einschraenkungsaenderung: Optional[Tarifeinschraenkung] = None
+    einschraenkungsaenderung: Optional["Tarifeinschraenkung"] = None
     """ Änderungen in den Einschränkungen zum Tarif. Falls in dieser Komponenten angegeben,
     werden die Tarifparameter hiermit überschrieben."""
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/aufabschlagstaffelproort.py` & `bo4e-202401.1.2rc14/src/bo4e/com/aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/ausschreibungsdetail.py` & `bo4e-202401.1.2rc14/src/bo4e/com/ausschreibungsdetail.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Contains class Ausschreibungsdetail and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.zaehlertyp import Zaehlertyp
 from ..utils import postprocess_docstring
-from .adresse import Adresse
 from .com import COM
-from .menge import Menge
-from .zeitraum import Zeitraum
+
+if TYPE_CHECKING:
+    from ..enum.zaehlertyp import Zaehlertyp
+    from .adresse import Adresse
+    from .menge import Menge
+    from .zeitraum import Zeitraum
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 
 
 @postprocess_docstring
 class Ausschreibungsdetail(COM):
     """
@@ -32,36 +34,36 @@
     #: Identifikation einer ausgeschriebenen Marktlokation
     marktlokations_id: Optional[str] = None
     #: In der angegebenen Netzebene wird die Marktlokation versorgt, z.B. MSP für Mittelspannung
     netzebene_lieferung: Optional[str] = None
     #: In der angegebenen Netzebene wird die Lokation gemessen, z.B. NSP für Niederspannung
     netzebene_messung: Optional[str] = None
     #: Die Adresse an der die Marktlokation sich befindet
-    marktlokationsadresse: Optional[Adresse] = None
+    marktlokationsadresse: Optional["Adresse"] = None
     #: Angefragter Zeitraum für die ausgeschriebene Belieferung
-    lieferzeitraum: Optional[Zeitraum] = None
+    lieferzeitraum: Optional["Zeitraum"] = None
 
     #: Bezeichnung des zuständigen Netzbetreibers, z.B. 'Stromnetz Hamburg GmbH'
     netzbetreiber: Optional[str] = None
     #: Bezeichnung des Kunden, der die Marktlokation nutzt
     kunde: Optional[str] = None
     #: Die Bezeichnung des Zählers an der Marktlokation
     zaehlernummer: Optional[str] = None
     #: Bezeichnung für die Lokation, z.B. 'Zentraler Einkauf, Hamburg'
     marktlokationsbezeichnung: Optional[str] = None
 
     #: Spezifikation, um welche Zählertechnik es sich im vorliegenden Fall handelt, z.B. Leistungsmessung
-    zaehlertechnik: Optional[Zaehlertyp] = None
+    zaehlertechnik: Optional["Zaehlertyp"] = None
     ist_lastgang_vorhanden: Optional[bool] = None
     """
     Zeigt an, ob es zu der Marktlokation einen Lastgang gibt.
     Falls ja, kann dieser abgerufen werden und daraus die Verbrauchswerte ermittelt werden
     """
 
     #: Prognosewert für die Jahresarbeit der ausgeschriebenen Lokation
-    prognose_jahresarbeit: Optional[Menge] = None
+    prognose_jahresarbeit: Optional["Menge"] = None
     #: Ein Prognosewert für die Arbeit innerhalb des angefragten Lieferzeitraums der ausgeschriebenen Lokation
-    prognose_arbeit_lieferzeitraum: Optional[Menge] = None
+    prognose_arbeit_lieferzeitraum: Optional["Menge"] = None
     #: Prognosewert für die abgenommene maximale Leistung der ausgeschriebenen Lokation
-    prognose_leistung: Optional[Menge] = None
+    prognose_leistung: Optional["Menge"] = None
     #: Die (evtl. abweichende) Rechnungsadresse
-    rechnungsadresse: Optional[Adresse] = None
+    rechnungsadresse: Optional["Adresse"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/ausschreibungslos.py` & `bo4e-202401.1.2rc14/src/bo4e/com/ausschreibungslos.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Contains Ausschreibungslos class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.preismodell import Preismodell
-from ..enum.rechnungslegung import Rechnungslegung
-from ..enum.sparte import Sparte
-from ..enum.vertragsform import Vertragsform
 from ..utils import postprocess_docstring
-from .ausschreibungsdetail import Ausschreibungsdetail
 from .com import COM
-from .menge import Menge
-from .zeitraum import Zeitraum
+
+if TYPE_CHECKING:
+    from ..enum.preismodell import Preismodell
+    from ..enum.rechnungslegung import Rechnungslegung
+    from ..enum.sparte import Sparte
+    from ..enum.vertragsform import Vertragsform
+    from .ausschreibungsdetail import Ausschreibungsdetail
+    from .menge import Menge
+    from .zeitraum import Zeitraum
 
 
 @postprocess_docstring
 class Ausschreibungslos(COM):
     """
     Eine Komponente zur Abbildung einzelner Lose einer Ausschreibung
 
@@ -32,45 +34,45 @@
     """
 
     #: Laufende Nummer des Loses
     losnummer: Optional[str] = None
     #: Bezeichnung der Ausschreibung
     bezeichnung: Optional[str] = None
     #: Bezeichnung der Preismodelle in Ausschreibungen für die Energielieferung
-    preismodell: Optional[Preismodell] = None
+    preismodell: Optional["Preismodell"] = None
 
     #: Unterscheidungsmöglichkeiten für die Sparte
-    energieart: Optional[Sparte] = None
+    energieart: Optional["Sparte"] = None
     #: Aufzählung der Möglichkeiten zur Rechnungslegung in Ausschreibungen
-    wunsch_rechnungslegung: Optional[Rechnungslegung] = None
+    wunsch_rechnungslegung: Optional["Rechnungslegung"] = None
     #: Aufzählung der Möglichkeiten zu Vertragsformen in Ausschreibungen
-    wunsch_vertragsform: Optional[Vertragsform] = None
+    wunsch_vertragsform: Optional["Vertragsform"] = None
     #: Name des Lizenzpartners
     betreut_durch: Optional[str] = None
     #: Anzahl der Lieferstellen in dieser Ausschreibung
     anzahl_lieferstellen: Optional[int] = None
 
     #: Die ausgeschriebenen Lieferstellen
-    lieferstellen: Optional[list[Ausschreibungsdetail]] = None
+    lieferstellen: Optional[list["Ausschreibungsdetail"]] = None
 
     #: Zeitraum, für den die in diesem Los enthaltenen Lieferstellen beliefert werden sollen
-    lieferzeitraum: Optional[Zeitraum] = None
+    lieferzeitraum: Optional["Zeitraum"] = None
 
     #: Bemerkung des Kunden zum Los
     bemerkung: Optional[str] = None
     #: Gibt den Gesamtjahresverbrauch (z.B. in kWh) aller in diesem Los enthaltenen Lieferstellen an
-    gesamt_menge: Optional[Menge] = None
+    gesamt_menge: Optional["Menge"] = None
     #: Mindesmenge Toleranzband (kWh, %)
-    wunsch_mindestmenge: Optional[Menge] = None
+    wunsch_mindestmenge: Optional["Menge"] = None
     #: Maximalmenge Toleranzband (kWh, %)
-    wunsch_maximalmenge: Optional[Menge] = None
+    wunsch_maximalmenge: Optional["Menge"] = None
 
-    wiederholungsintervall: Optional[Zeitraum] = None
+    wiederholungsintervall: Optional["Zeitraum"] = None
     """
     In welchem Intervall die Angebotsabgabe wiederholt werden darf.
     Angabe nur gesetzt für die 2. Phase bei öffentlich-rechtlichen Ausschreibungen
     """
 
     #: Kundenwunsch zur Kündigungsfrist in der Ausschreibung
-    wunsch_kuendingungsfrist: Optional[Zeitraum] = None
+    wunsch_kuendingungsfrist: Optional["Zeitraum"] = None
     #: Kundenwunsch zum Zahlungsziel in der Ausschreibung
-    wunsch_zahlungsziel: Optional[Zeitraum] = None
+    wunsch_zahlungsziel: Optional["Zeitraum"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/betrag.py` & `bo4e-202401.1.2rc14/src/bo4e/com/betrag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Contains Betrag class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.waehrungscode import Waehrungscode
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.waehrungscode import Waehrungscode
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Betrag(COM):
     """
     Die Komponente wird dazu verwendet, Summenbeträge (beispielsweise in Angeboten und Rechnungen) als Geldbeträge
@@ -25,8 +28,8 @@
 
     .. HINT::
         `Betrag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Betrag.json>`_
 
     """
 
     wert: Optional[Decimal] = None  #: Gibt den Betrag des Preises an.
-    waehrung: Optional[Waehrungscode] = None  #: Die entsprechende Waehrung
+    waehrung: Optional["Waehrungscode"] = None  #: Die entsprechende Waehrung
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/com.py` & `bo4e-202401.1.2rc14/src/bo4e/com/com.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,27 @@
         <object data="../_static/images/bo4e/com/COM.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `COM JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/COM.json>`_
 
     """
 
-    version: Annotated[
-        Optional[str], Field(alias="_version")
-    ] = __version__  #: Version der BO-Struktur aka "fachliche Versionierung"
+    version: Annotated[Optional[str], Field(alias="_version")] = (
+        __version__  #: Version der BO-Struktur aka "fachliche Versionierung"
+    )
 
     # Python internal: The field is not named '_id' because leading underscores are not allowed in pydantic field names.
     # NameError: Fields must not use names with leading underscores; e.g., use 'id' instead of '_id'.
     id: Annotated[Optional[str], Field(alias="_id")] = None
     """
     Eine generische ID, die für eigene Zwecke genutzt werden kann.
     Z.B. könnten hier UUIDs aus einer Datenbank stehen oder URLs zu einem Backend-System.
     """
 
-    zusatz_attribute: Optional[list[ZusatzAttribut]] = None
+    zusatz_attribute: Optional[list["ZusatzAttribut"]] = None
 
     # pylint: disable=duplicate-code
     model_config = ConfigDict(
         alias_generator=camelize,
         populate_by_name=True,
         extra="allow",
         # json_encoders is deprecated, but there is no easy-to-use alternative. The best way would be to create
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/dienstleistung.py` & `bo4e-202401.1.2rc14/src/bo4e/com/dienstleistung.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Contains Dienstleistung class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.dienstleistungstyp import Dienstleistungstyp
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.dienstleistungstyp import Dienstleistungstyp
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Dienstleistung(COM):
     """
     Abbildung einer abrechenbaren Dienstleistung.
@@ -23,10 +26,10 @@
 
     .. HINT::
         `Dienstleistung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Dienstleistung.json>`_
 
     """
 
     #: Kennzeichnung der Dienstleistung
-    dienstleistungstyp: Optional[Dienstleistungstyp] = None
+    dienstleistungstyp: Optional["Dienstleistungstyp"] = None
     #: Bezeichnung der Dienstleistung
     bezeichnung: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/energieherkunft.py` & `bo4e-202401.1.2rc14/src/bo4e/com/energieherkunft.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Contains Energieherkunft class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.erzeugungsart import Erzeugungsart
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.erzeugungsart import Erzeugungsart
+
+
 # pylint: disable=no-name-in-module
 
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
@@ -27,10 +30,10 @@
 
     .. HINT::
         `Energieherkunft JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Energieherkunft.json>`_
 
     """
 
     #: Art der Erzeugung der Energie.
-    erzeugungsart: Optional[Erzeugungsart] = None
+    erzeugungsart: Optional["Erzeugungsart"] = None
     #: Prozentualer Anteil der jeweiligen Erzeugungsart.
     anteil_prozent: Optional[Decimal] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/energiemix.py` & `bo4e-202401.1.2rc14/src/bo4e/com/energiemix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Contains Energiemix class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.oekolabel import Oekolabel
-from ..enum.oekozertifikat import Oekozertifikat
-from ..enum.sparte import Sparte
 from ..utils import postprocess_docstring
 from .com import COM
-from .energieherkunft import Energieherkunft
+
+if TYPE_CHECKING:
+    from ..enum.oekolabel import Oekolabel
+    from ..enum.oekozertifikat import Oekozertifikat
+    from ..enum.sparte import Sparte
+    from .energieherkunft import Energieherkunft
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class Energiemix(COM):
@@ -30,29 +32,29 @@
         `Energiemix JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Energiemix.json>`_
 
     """
 
     #: Eindeutige Nummer zur Identifizierung des Energiemixes
     energiemixnummer: Optional[int] = None
     #: Strom oder Gas etc.
-    energieart: Optional[Sparte] = None
+    energieart: Optional["Sparte"] = None
     #: Bezeichnung des Energiemix
     bezeichnung: Optional[str] = None
     #: Jahr, für das der Energiemix gilt
     gueltigkeitsjahr: Optional[int] = None
     #: Anteile der jeweiligen Erzeugungsart
-    anteil: Optional[list[Energieherkunft]] = None
+    anteil: Optional[list["Energieherkunft"]] = None
 
     #: Bemerkung zum Energiemix
     bemerkung: Optional[str] = None
     #: Höhe des erzeugten CO2-Ausstosses in g/kWh
     co2_emission: Optional[Decimal] = None
     #: Höhe des erzeugten Atommülls in g/kWh
     atommuell: Optional[Decimal] = None
     #: Zertifikate für den Energiemix
-    oekozertifikate: Optional[list[Oekozertifikat]] = None
+    oekozertifikate: Optional[list["Oekozertifikat"]] = None
     #: Ökolabel für den Energiemix
-    oekolabel: Optional[list[Oekolabel]] = None
+    oekolabel: Optional[list["Oekolabel"]] = None
     #: Kennzeichen, ob der Versorger zu den Öko Top Ten gehört
     ist_in_oeko_top_ten: Optional[bool] = None
     #: Internetseite, auf der die Strommixdaten veröffentlicht sind
     website: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/fremdkostenblock.py` & `bo4e-202401.1.2rc14/src/bo4e/com/kostenblock.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 """
-Contains Fremdkostenblock class
-and corresponding marshmallow schema for de-/serialization
+Contains Kostenblock and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from ..utils import postprocess_docstring
-from .betrag import Betrag
 from .com import COM
-from .fremdkostenposition import Fremdkostenposition
+
+if TYPE_CHECKING:
+
+    from .betrag import Betrag
+    from .kostenposition import Kostenposition
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
-class Fremdkostenblock(COM):
+class Kostenblock(COM):
     """
-    Komponente zur Abbildung eines Kostenblocks in den Fremdkosten
+    Mit dieser Komponente werden mehrere Kostenpositionen zusammengefasst.
 
     .. raw:: html
 
-        <object data="../_static/images/bo4e/com/Fremdkostenblock.svg" type="image/svg+xml"></object>
+        <object data="../_static/images/bo4e/com/Kostenblock.svg" type="image/svg+xml"></object>
 
     .. HINT::
-        `Fremdkostenblock JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Fremdkostenblock.json>`_
+        `Kostenblock JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Kostenblock.json>`_
 
     """
 
     #: Bezeichnung für einen Kostenblock. Z.B. Netzkosten, Messkosten, Umlagen, etc.
     kostenblockbezeichnung: Optional[str] = None
 
-    kostenpositionen: Optional[list[Fremdkostenposition]] = None
+    #: Die Summe aller Kostenpositionen dieses Blocks
+    summe_kostenblock: Optional["Betrag"] = None
+
+    kostenpositionen: Optional[list["Kostenposition"]] = None
     """
     Hier sind die Details zu einer Kostenposition aufgeführt. Z.B.:
-    Alliander Netz Heinsberg GmbH, 2018-02-01, 2019-01-01, Arbeitspreis HT, 3.660 kWh,
-    5,8200 ct/kWh, 213,01 €
+    Alliander Netz Heinsberg GmbH, 01.02.2018, 31.12.2018, Arbeitspreis HT, 3.660 kWh, 5,8200 ct/kWh, 213,01 €
     """
-
-    #: Die Summe aller Kostenpositionen dieses Blocks
-    summe_kostenblock: Optional[Betrag] = None
-    # todo: write validator fo this sum, see https://github.com/Hochfrequenz/BO4E-python/issues/324
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/fremdkostenposition.py` & `bo4e-202401.1.2rc14/src/bo4e/com/fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/geokoordinaten.py` & `bo4e-202401.1.2rc14/src/bo4e/com/geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/katasteradresse.py` & `bo4e-202401.1.2rc14/src/bo4e/com/katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/kontaktweg.py` & `bo4e-202401.1.2rc14/src/bo4e/com/kontaktweg.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Contains Kontaktweg class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.kontaktart import Kontaktart
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.kontaktart import Kontaktart
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Kontaktweg(COM):
     """
     Die Komponente wird dazu verwendet, die Kontaktwege innerhalb des BOs Person darzustellen
@@ -23,14 +26,14 @@
 
     .. HINT::
         `Kontakt JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Kontakt.json>`_
 
     """
 
     #: Gibt die Kontaktart des Kontaktes an.
-    kontaktart: Optional[Kontaktart] = None
+    kontaktart: Optional["Kontaktart"] = None
     #: Spezifikation, beispielsweise "Durchwahl", "Sammelnummer" etc.
     beschreibung: Optional[str] = None
     #: Die Nummer oder E-Mail-Adresse.
     kontaktwert: Optional[str] = None
     #: Gibt an, ob es sich um den bevorzugten Kontaktweg handelt.
     ist_bevorzugter_kontaktweg: Optional[bool] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/konzessionsabgabe.py` & `bo4e-202401.1.2rc14/src/bo4e/com/konzessionsabgabe.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Contains Konzessionsabgabe and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..com.com import COM
-from ..enum.abgabeart import AbgabeArt
 from ..utils import postprocess_docstring
+from .com import COM
+
+if TYPE_CHECKING:
+    from ..enum.abgabeart import AbgabeArt
+
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 
 
 @postprocess_docstring
 class Konzessionsabgabe(COM):
     """
@@ -23,14 +26,14 @@
 
     .. HINT::
         `Konzessionsabgabe JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Konzessionsabgabe.json>`_
 
     """
 
     #: Art der Abgabe
-    satz: Optional[AbgabeArt] = None
+    satz: Optional["AbgabeArt"] = None
 
     #: Konzessionsabgabe in E/kWh
     kosten: Optional[Decimal] = None
 
     #: Gebührenkategorie der Konzessionsabgabe
     kategorie: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/kostenposition.py` & `bo4e-202401.1.2rc14/src/bo4e/com/kostenposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 Contains Kostenposition and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 import pydantic
 
 from ..utils import postprocess_docstring
-from .betrag import Betrag
 from .com import COM
-from .menge import Menge
-from .preis import Preis
+
+if TYPE_CHECKING:
+
+    from .betrag import Betrag
+    from .menge import Menge
+    from .preis import Preis
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 
 
 @postprocess_docstring
 class Kostenposition(COM):
     """
@@ -28,34 +31,34 @@
         `Kostenposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Kostenposition.json>`_
 
     """
 
     #: Ein Titel für die Zeile. Hier kann z.B. der Netzbetreiber eingetragen werden, wenn es sich um Netzkosten handelt.
     positionstitel: Optional[str] = None
 
-    betrag_kostenposition: Optional[Betrag] = None
+    betrag_kostenposition: Optional["Betrag"] = None
     """Der errechnete Gesamtbetrag der Position als Ergebnis der Berechnung <Menge * Einzelpreis> oder
     <Einzelpreis / (Anzahl Tage Jahr) * zeitmenge>"""
     # todo: validate above calculation, see https://github.com/Hochfrequenz/BO4E-python/issues/282
 
     #: Bezeichnung für den Artikel für den die Kosten ermittelt wurden. Beispiel: Arbeitspreis HT
     artikelbezeichnung: Optional[str] = None
 
     #: Der Preis für eine Einheit. Beispiele: 5,8200 ct/kWh oder 55 €/Jahr.
-    einzelpreis: Optional[Preis] = None
+    einzelpreis: Optional["Preis"] = None
 
     #: inklusiver von-Zeitpunkt der Kostenzeitscheibe
     von: Optional[pydantic.AwareDatetime] = None
     #: exklusiver bis-Zeitpunkt der Kostenzeitscheibe
     bis: Optional[pydantic.AwareDatetime] = None
 
     #: Die Menge, die in die Kostenberechnung eingeflossen ist. Beispiel: 3.660 kWh
-    menge: Optional[Menge] = None
+    menge: Optional["Menge"] = None
 
-    zeitmenge: Optional[Menge] = None
+    zeitmenge: Optional["Menge"] = None
     """
     Wenn es einen zeitbasierten Preis gibt (z.B. €/Jahr), dann ist hier die Menge angegeben mit der die Kosten berechnet
     wurden. Z.B. 138 Tage.
     """
 
     #: Detaillierung des Artikels (optional). Beispiel: 'Drehstromzähler'
     artikeldetail: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/kriteriumwert.py` & `bo4e-202401.1.2rc14/src/bo4e/com/kriteriumwert.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """
 Contains KriteriumWert class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
-
 # pylint: disable=too-few-public-methods
-from ..enum.tarifregionskriterium import Tarifregionskriterium
+from typing import TYPE_CHECKING, Optional
+
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.tarifregionskriterium import Tarifregionskriterium
+
 
 @postprocess_docstring
 class KriteriumWert(COM):
     """
     Mit dieser Komponente können Kriterien und deren Werte definiert werden
 
     .. raw:: html
@@ -22,10 +24,10 @@
 
     .. HINT::
         `KriteriumWert JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/KriteriumWert.json>`_
 
     """
 
     #: Hier steht, für welches Kriterium der Wert gilt. Z.B. Postleitzahlen
-    kriterium: Optional[Tarifregionskriterium] = None
+    kriterium: Optional["Tarifregionskriterium"] = None
     #: Ein Wert, passend zum Kriterium. Z.B. eine Postleitzahl.
     wert: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/marktgebietinfo.py` & `bo4e-202401.1.2rc14/src/bo4e/com/marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/menge.py` & `bo4e-202401.1.2rc14/src/bo4e/com/menge.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Contains Menge class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.mengeneinheit import Mengeneinheit
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.mengeneinheit import Mengeneinheit
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Menge(COM):
     """
     Abbildung einer Menge mit Wert und Einheit.
@@ -26,8 +29,8 @@
         `Menge JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Menge.json>`_
 
     """
 
     #: Gibt den absoluten Wert der Menge an
     wert: Optional[Decimal] = None
     #: Gibt die Einheit zum jeweiligen Wert an
-    einheit: Optional[Mengeneinheit] = None
+    einheit: Optional["Mengeneinheit"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/messlokationszuordnung.py` & `bo4e-202401.1.2rc14/src/bo4e/com/messlokationszuordnung.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 Contains Messlokationszuordnung class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 import pydantic
 
-from ..enum.arithmetische_operation import ArithmetischeOperation
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.arithmetische_operation import ArithmetischeOperation
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Messlokationszuordnung(COM):
     """
     Mit dieser Komponente werden Messlokationen zu Marktlokationen zugeordnet.
@@ -30,15 +33,15 @@
 
     """
 
     messlokations_id: Optional[str] = None
     """
     ID der zugeordneten Messlokation
     """
-    arithmetik: Optional[ArithmetischeOperation] = None
+    arithmetik: Optional["ArithmetischeOperation"] = None
 
     gueltig_seit: Optional[pydantic.AwareDatetime] = None
     """
     inklusives Beginndatum
     """
     gueltig_bis: Optional[pydantic.AwareDatetime] = None
     """
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/positionsaufabschlag.py` & `bo4e-202401.1.2rc14/src/bo4e/com/positionsaufabschlag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 Contains PositionsAufAbschlag and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
 
 # pylint: disable=too-few-public-methods
-from ..enum.aufabschlagstyp import AufAbschlagstyp
-from ..enum.waehrungseinheit import Waehrungseinheit
+from typing import TYPE_CHECKING, Optional
+
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.aufabschlagstyp import AufAbschlagstyp
+    from ..enum.waehrungseinheit import Waehrungseinheit
+
 
 @postprocess_docstring
 class PositionsAufAbschlag(COM):
     """
     Differenzierung der zu betrachtenden Produkte anhand der preiserhöhenden (Aufschlag)
     bzw. preisvermindernden (Abschlag) Zusatzvereinbarungen,
     die individuell zu einem neuen oder bestehenden Liefervertrag abgeschlossen werden können.
@@ -30,12 +33,12 @@
     """
 
     #: Bezeichnung des Auf-/Abschlags
     bezeichnung: Optional[str] = None
     #: Beschreibung zum Auf-/Abschlag
     beschreibung: Optional[str] = None
     #: Typ des AufAbschlages
-    auf_abschlagstyp: Optional[AufAbschlagstyp] = None
+    auf_abschlagstyp: Optional["AufAbschlagstyp"] = None
     #: Höhe des Auf-/Abschlages
     auf_abschlagswert: Optional[Decimal] = None
     #: Einheit, in der der Auf-/Abschlag angegeben ist (z.B. ct/kWh).
-    auf_abschlagswaehrung: Optional[Waehrungseinheit] = None
+    auf_abschlagswaehrung: Optional["Waehrungseinheit"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/preisgarantie.py` & `bo4e-202401.1.2rc14/src/bo4e/com/preisgarantie.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Contains Preisgarantie class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.preisgarantietyp import Preisgarantietyp
 from ..utils import postprocess_docstring
 from .com import COM
-from .zeitraum import Zeitraum
+
+if TYPE_CHECKING:
+    from ..enum.preisgarantietyp import Preisgarantietyp
+    from .zeitraum import Zeitraum
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Preisgarantie(COM):
     """
@@ -24,15 +26,15 @@
 
     .. HINT::
         `Preisgarantie JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Preisgarantie.json>`_
 
     """
 
     #: Festlegung, auf welche Preisbestandteile die Garantie gewährt wird.
-    preisgarantietyp: Optional[Preisgarantietyp] = None
-    zeitliche_gueltigkeit: Optional[Zeitraum] = None
+    preisgarantietyp: Optional["Preisgarantietyp"] = None
+    zeitliche_gueltigkeit: Optional["Zeitraum"] = None
     """ Zeitraum, bis zu dem die Preisgarantie gilt, z.B. bis zu einem absolutem / fixem Datum
     oder als Laufzeit in Monaten. """
 
     # optionale attributes
     #: Freitext zur Beschreibung der Preisgarantie.
     beschreibung: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/preisposition.py` & `bo4e-202401.1.2rc14/src/bo4e/com/preisposition.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """
 Contains Preisposition class and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
 
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.bdewartikelnummer import BDEWArtikelnummer
-from ..enum.bemessungsgroesse import Bemessungsgroesse
-from ..enum.kalkulationsmethode import Kalkulationsmethode
-from ..enum.leistungstyp import Leistungstyp
-from ..enum.mengeneinheit import Mengeneinheit
-from ..enum.tarifzeit import Tarifzeit
-from ..enum.waehrungseinheit import Waehrungseinheit
 from ..utils import postprocess_docstring
 from .com import COM
-from .preisstaffel import Preisstaffel
+
+if TYPE_CHECKING:
+    from ..enum.bdewartikelnummer import BDEWArtikelnummer
+    from ..enum.bemessungsgroesse import Bemessungsgroesse
+    from ..enum.kalkulationsmethode import Kalkulationsmethode
+    from ..enum.leistungstyp import Leistungstyp
+    from ..enum.mengeneinheit import Mengeneinheit
+    from ..enum.tarifzeit import Tarifzeit
+    from ..enum.waehrungseinheit import Waehrungseinheit
+    from .preisstaffel import Preisstaffel
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 
 
 @postprocess_docstring
 class Preisposition(COM):
     """
@@ -32,40 +34,40 @@
 
     .. HINT::
         `Preisposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Preisposition.json>`_
 
     """
 
     #: Das Modell, das der Preisbildung zugrunde liegt
-    berechnungsmethode: Optional[Kalkulationsmethode] = None
+    berechnungsmethode: Optional["Kalkulationsmethode"] = None
     #: Standardisierte Bezeichnung für die abgerechnete Leistungserbringung
-    leistungstyp: Optional[Leistungstyp] = None  #
+    leistungstyp: Optional["Leistungstyp"] = None  #
     #: Bezeichnung für die in der Position abgebildete Leistungserbringung
     leistungsbezeichnung: Optional[str] = None
     #: Festlegung, mit welcher Preiseinheit abgerechnet wird, z.B. Ct. oder €
-    preiseinheit: Optional[Waehrungseinheit] = None
+    preiseinheit: Optional["Waehrungseinheit"] = None
     #: Hier wird festgelegt, auf welche Bezugsgrösse sich der Preis bezieht, z.B. kWh oder Stück
-    bezugsgroesse: Optional[Mengeneinheit] = None
+    bezugsgroesse: Optional["Mengeneinheit"] = None
     #: Preisstaffeln, die zu dieser Preisposition gehören
-    preisstaffeln: Optional[list[Preisstaffel]] = None
+    preisstaffeln: Optional[list["Preisstaffel"]] = None
 
-    zeitbasis: Optional[Mengeneinheit] = None
+    zeitbasis: Optional["Mengeneinheit"] = None
     """
     Die Zeit(dauer) auf die sich der Preis bezieht.
     Z.B. ein Jahr für einen Leistungspreis der in €/kW/Jahr ausgegeben wird
     """
     #: Festlegung, für welche Tarifzeit der Preis hier festgelegt ist
-    tarifzeit: Optional[Tarifzeit] = None
-    bdew_artikelnummer: Optional[BDEWArtikelnummer] = None
+    tarifzeit: Optional["Tarifzeit"] = None
+    bdew_artikelnummer: Optional["BDEWArtikelnummer"] = None
     """
     Eine vom BDEW standardisierte Bezeichnug für die abgerechnete Leistungserbringung;
     Diese Artikelnummer wird auch im Rechnungsteil der INVOIC verwendet.
     """
     #: Mit der Menge der hier angegebenen Größe wird die Staffelung/Zonung durchgeführt. Z.B. Vollbenutzungsstunden
-    zonungsgroesse: Optional[Bemessungsgroesse] = None
+    zonungsgroesse: Optional["Bemessungsgroesse"] = None
     #: Der Anteil der Menge der Blindarbeit in Prozent von der Wirkarbeit, für die keine Abrechnung erfolgt
     freimenge_blindarbeit: Optional[Decimal] = None
     freimenge_leistungsfaktor: Optional[Decimal] = None
     """
     Der cos phi (Verhältnis Wirkleistung/Scheinleistung) aus dem die Freimenge für die Blindarbeit berechnet wird als
     tan phi (Verhältnis Blindleistung/Wirkleistung)
     """
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/preisstaffel.py` & `bo4e-202401.1.2rc14/src/bo4e/com/preisstaffel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Contains Preisstaffel and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from ..utils import postprocess_docstring
 from .com import COM
-from .sigmoidparameter import Sigmoidparameter
+
+if TYPE_CHECKING:
+
+    from .sigmoidparameter import Sigmoidparameter
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Preisstaffel(COM):
     """
@@ -30,8 +33,8 @@
     einheitspreis: Optional[Decimal] = None
     #: Inklusiver unterer Wert, ab dem die Staffel gilt
     staffelgrenze_von: Optional[Decimal] = None
     #: Exklusiver oberer Wert, bis zu dem die Staffel gilt
     staffelgrenze_bis: Optional[Decimal] = None
 
     #: Parameter zur Berechnung des Preises anhand der Jahresmenge und weiterer netzbezogener Parameter
-    sigmoidparameter: Optional[Sigmoidparameter] = None
+    sigmoidparameter: Optional["Sigmoidparameter"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/rechnungsposition.py` & `bo4e-202401.1.2rc14/src/bo4e/com/rechnungsposition.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """
 Contains Rechnungsposition class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 import pydantic
 
-from ..enum.bdewartikelnummer import BDEWArtikelnummer
-from ..enum.mengeneinheit import Mengeneinheit
 from ..utils import postprocess_docstring
-from .betrag import Betrag
 from .com import COM
-from .menge import Menge
-from .preis import Preis
-from .steuerbetrag import Steuerbetrag
+
+if TYPE_CHECKING:
+    from ..enum.bdewartikelnummer import BDEWArtikelnummer
+    from ..enum.mengeneinheit import Mengeneinheit
+    from .betrag import Betrag
+    from .menge import Menge
+    from .preis import Preis
+    from .steuerbetrag import Steuerbetrag
 
 
 @postprocess_docstring
 class Rechnungsposition(COM):
     """
     Über Rechnungspositionen werden Rechnungen strukturiert.
     In einem Rechnungsteil wird jeweils eine in sich geschlossene Leistung abgerechnet.
@@ -31,52 +33,52 @@
         `Rechnungsposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Rechnungsposition.json>`_
 
     """
 
     #: Fortlaufende Nummer für die Rechnungsposition
     positionsnummer: Optional[int] = None
 
-    lieferung_von: Optional[
-        pydantic.AwareDatetime
-    ] = None  #: Start der Lieferung für die abgerechnete Leistung (inklusiv)
-    lieferung_bis: Optional[
-        pydantic.AwareDatetime
-    ] = None  #: Ende der Lieferung für die abgerechnete Leistung (exklusiv)
+    lieferung_von: Optional[pydantic.AwareDatetime] = (
+        None  #: Start der Lieferung für die abgerechnete Leistung (inklusiv)
+    )
+    lieferung_bis: Optional[pydantic.AwareDatetime] = (
+        None  #: Ende der Lieferung für die abgerechnete Leistung (exklusiv)
+    )
 
     #: Bezeichung für die abgerechnete Position
     positionstext: Optional[str] = None
 
     #: Die abgerechnete Menge mit Einheit
-    positions_menge: Optional[Menge] = None
+    positions_menge: Optional["Menge"] = None
     #: Der Preis für eine Einheit der energetischen Menge
-    einzelpreis: Optional[Preis] = None
+    einzelpreis: Optional["Preis"] = None
 
-    teilsumme_netto: Optional[Betrag] = None
+    teilsumme_netto: Optional["Betrag"] = None
     """
     Das Ergebnis der Multiplikation aus einzelpreis * positionsMenge * (Faktor aus zeitbezogeneMenge).
     Z.B. 12,60€ * 120 kW * 3/12 (für 3 Monate).
     """
     # the cross check in general doesn't work because Betrag and Preis use different enums to describe the currency
     # see https://github.com/Hochfrequenz/BO4E-python/issues/126
 
     #: Auf die Position entfallende Steuer, bestehend aus Steuersatz und Betrag
-    teilsumme_steuer: Optional[Steuerbetrag] = None
+    teilsumme_steuer: Optional["Steuerbetrag"] = None
 
     #: Falls sich der Preis auf eine Zeit bezieht, steht hier die Einheit
-    zeiteinheit: Optional[Mengeneinheit] = None
+    zeiteinheit: Optional["Mengeneinheit"] = None
 
     #: Kennzeichnung der Rechnungsposition mit der Standard-Artikelnummer des BDEW
-    artikelnummer: Optional[BDEWArtikelnummer] = None
+    artikelnummer: Optional["BDEWArtikelnummer"] = None
     #: Marktlokation, die zu dieser Position gehört
     lokations_id: Optional[str] = None
 
-    zeitbezogene_menge: Optional[Menge] = None
+    zeitbezogene_menge: Optional["Menge"] = None
     """
     Eine auf die Zeiteinheit bezogene Untermenge.
     Z.B. bei einem Jahrespreis, 3 Monate oder 146 Tage.
     Basierend darauf wird der Preis aufgeteilt.
     """
     #: Nettobetrag für den Rabatt dieser Position
-    teilrabatt_netto: Optional[Betrag] = None
+    teilrabatt_netto: Optional["Betrag"] = None
 
     #: Standardisierte vom BDEW herausgegebene Liste, welche im Strommarkt die BDEW-Artikelnummer ablöst
     artikel_id: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/regionalegueltigkeit.py` & `bo4e-202401.1.2rc14/src/bo4e/com/regionalegueltigkeit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Contains RegionaleGueltigkeit class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.gueltigkeitstyp import Gueltigkeitstyp
 from ..utils import postprocess_docstring
 from .com import COM
-from .kriteriumwert import KriteriumWert
+
+if TYPE_CHECKING:
+    from ..enum.gueltigkeitstyp import Gueltigkeitstyp
+    from .kriteriumwert import KriteriumWert
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class RegionaleGueltigkeit(COM):
@@ -24,13 +26,13 @@
         <object data="../_static/images/bo4e/com/RegionaleGueltigkeit.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `RegionaleGueltigkeit JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/RegionaleGueltigkeit.json>`_
 
     """
 
-    gueltigkeitstyp: Optional[
-        Gueltigkeitstyp
-    ] = None  #: Unterscheidung ob Positivliste oder Negativliste übertragen wird
-    kriteriums_werte: Optional[
-        list[KriteriumWert]
-    ] = None  #: Hier stehen die Kriterien, die die regionale Gültigkeit festlegen
+    gueltigkeitstyp: Optional["Gueltigkeitstyp"] = (
+        None  #: Unterscheidung ob Positivliste oder Negativliste übertragen wird
+    )
+    kriteriums_werte: Optional[list["KriteriumWert"]] = (
+        None  #: Hier stehen die Kriterien, die die regionale Gültigkeit festlegen
+    )
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/regionalepreisgarantie.py` & `bo4e-202401.1.2rc14/src/bo4e/com/regionalepreisgarantie.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Contains RegionalePreisgarantie class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from ..utils import postprocess_docstring
 from .preisgarantie import Preisgarantie
-from .regionalegueltigkeit import RegionaleGueltigkeit
+
+if TYPE_CHECKING:
+    from .regionalegueltigkeit import RegionaleGueltigkeit
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class RegionalePreisgarantie(Preisgarantie):
     """
@@ -23,8 +25,8 @@
 
     .. HINT::
         `RegionalePreisgarantie JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/RegionalePreisgarantie.json>`_
 
     """
 
     #: Regionale Eingrenzung der Preisgarantie.
-    regionale_gueltigkeit: Optional[RegionaleGueltigkeit] = None
+    regionale_gueltigkeit: Optional["RegionaleGueltigkeit"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/regionalepreisstaffel.py` & `bo4e-202401.1.2rc14/src/bo4e/com/regionalepreisstaffel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """
 Contains RegionalePreisstaffel class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from ..utils import postprocess_docstring
 from .preisstaffel import Preisstaffel
-from .regionalegueltigkeit import RegionaleGueltigkeit
+
+if TYPE_CHECKING:
+    from .regionalegueltigkeit import RegionaleGueltigkeit
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class RegionalePreisstaffel(Preisstaffel):
     """
@@ -22,8 +24,8 @@
 
     .. HINT::
         `RegionalePreisstaffel JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/RegionalePreisstaffel.json>`_
 
     """
 
     #: Regionale Eingrenzung der Preisstaffel
-    regionale_gueltigkeit: Optional[RegionaleGueltigkeit] = None
+    regionale_gueltigkeit: Optional["RegionaleGueltigkeit"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/regionaleraufabschlag.py` & `bo4e-202401.1.2rc14/src/bo4e/com/regionaleraufabschlag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """
 Contains RegionalerAufAbschlag class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
-
-from ..enum.aufabschlagstyp import AufAbschlagstyp
-from ..enum.aufabschlagsziel import AufAbschlagsziel
-from ..enum.waehrungseinheit import Waehrungseinheit
+from typing import TYPE_CHECKING, Optional
 
 # pylint: disable=R0801
 from ..utils import postprocess_docstring
 from .com import COM
-from .energiemix import Energiemix
-from .preisgarantie import Preisgarantie
-from .regionalepreisstaffel import RegionalePreisstaffel
-from .tarifeinschraenkung import Tarifeinschraenkung
-from .vertragskonditionen import Vertragskonditionen
-from .zeitraum import Zeitraum
+
+if TYPE_CHECKING:
+    from ..enum.aufabschlagstyp import AufAbschlagstyp
+    from ..enum.aufabschlagsziel import AufAbschlagsziel
+    from ..enum.waehrungseinheit import Waehrungseinheit
+    from .energiemix import Energiemix
+    from .preisgarantie import Preisgarantie
+    from .regionalepreisstaffel import RegionalePreisstaffel
+    from .tarifeinschraenkung import Tarifeinschraenkung
+    from .vertragskonditionen import Vertragskonditionen
+    from .zeitraum import Zeitraum
 
 # pylint: disable=too-few-public-methods, too-many-instance-attributes
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class RegionalerAufAbschlag(COM):
@@ -39,59 +40,59 @@
 
     """
 
     #: Bezeichnung des Auf-/Abschlags
     bezeichnung: Optional[str] = None
 
     #: Werte für die gestaffelten Auf/Abschläge mit regionaler Eingrenzung
-    staffeln: Optional[list[RegionalePreisstaffel]] = None
+    staffeln: Optional[list["RegionalePreisstaffel"]] = None
 
     #: Beschreibung des Auf-/Abschlags
     beschreibung: Optional[str] = None
 
     #: Typ des Aufabschlages (z.B. absolut oder prozentual)
-    auf_abschlagstyp: Optional[AufAbschlagstyp] = None
+    auf_abschlagstyp: Optional["AufAbschlagstyp"] = None
 
     #: Diesem Preis oder den Kosten ist der Auf/Abschlag zugeordnet. Z.B. Arbeitspreis, Gesamtpreis etc.
-    auf_abschlagsziel: Optional[AufAbschlagsziel] = None
+    auf_abschlagsziel: Optional["AufAbschlagsziel"] = None
 
     #: Gibt an in welcher Währungseinheit der Auf/Abschlag berechnet wird (nur im Falle absoluter Aufschlagstypen).
-    einheit: Optional[Waehrungseinheit] = None
+    einheit: Optional["Waehrungseinheit"] = None
 
     #: Internetseite, auf der die Informationen zum Auf-/Abschlag veröffentlicht sind
     website: Optional[str] = None
 
     #: Zusatzprodukte, die nur in Kombination mit diesem AufAbschlag erhältlich sind
     zusatzprodukte: Optional[list[str]] = None
 
     #: Voraussetzungen, die erfüllt sein müssen, damit dieser AufAbschlag zur Anwendung kommen kann
     voraussetzungen: Optional[list[str]] = None
 
     #: Durch die Anwendung des Auf/Abschlags kann eine Änderung des Tarifnamens auftreten
     tarifnamensaenderungen: Optional[str] = None
 
     #: Zeitraum, in dem der Abschlag zur Anwendung kommen kann
-    gueltigkeitszeitraum: Optional[Zeitraum] = None
+    gueltigkeitszeitraum: Optional["Zeitraum"] = None
 
-    energiemixaenderung: Optional[Energiemix] = None
+    energiemixaenderung: Optional["Energiemix"] = None
     """
     Der Energiemix kann sich durch einen AufAbschlag ändern (z.B. zwei Cent Aufschlag für Ökostrom).
     Sollte dies der Fall sein, wird hier die neue Zusammensetzung des Energiemix angegeben.
     """
 
-    vertagskonditionsaenderung: Optional[Vertragskonditionen] = None
+    vertagskonditionsaenderung: Optional["Vertragskonditionen"] = None
     """
     Änderungen in den Vertragskonditionen;
     Falls in dieser Komponenten angegeben, werden die Tarifparameter hiermit überschrieben.
     """
 
-    garantieaenderung: Optional[Preisgarantie] = None
+    garantieaenderung: Optional["Preisgarantie"] = None
     """
     Änderungen in den Garantievereinbarungen;
     Falls in dieser Komponenten angegeben, werden die Tarifparameter hiermit überschrieben.
     """
 
-    einschraenkungsaenderung: Optional[Tarifeinschraenkung] = None
+    einschraenkungsaenderung: Optional["Tarifeinschraenkung"] = None
     """
     Änderungen in den Einschränkungen zum Tarif;
     Falls in dieser Komponenten angegeben, werden die Tarifparameter hiermit überschrieben.
     """
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/regionaletarifpreisposition.py` & `bo4e-202401.1.2rc14/src/bo4e/com/regionaletarifpreisposition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Contains RegionaleTarifpreisposition class and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.mengeneinheit import Mengeneinheit
-from ..enum.preistyp import Preistyp
-from ..enum.waehrungseinheit import Waehrungseinheit
 from ..utils import postprocess_docstring
 from .com import COM
-from .regionalepreisstaffel import RegionalePreisstaffel
+
+if TYPE_CHECKING:
+    from ..enum.mengeneinheit import Mengeneinheit
+    from ..enum.preistyp import Preistyp
+    from ..enum.waehrungseinheit import Waehrungseinheit
+    from .regionalepreisstaffel import RegionalePreisstaffel
 
 
 @postprocess_docstring
 class RegionaleTarifpreisposition(COM):
     """
     Mit dieser Komponente können Tarifpreise verschiedener Typen im Zusammenhang mit regionalen Gültigkeiten abgebildet
     werden.
@@ -26,17 +28,17 @@
 
     .. HINT::
         `RegionaleTarifpreisposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/RegionaleTarifpreisposition.json>`_
 
     """
 
     #: Angabe des Preistypes (z.B. Grundpreis)
-    preistyp: Optional[Preistyp] = None
+    preistyp: Optional["Preistyp"] = None
     #: Einheit des Preises (z.B. EURO)
-    einheit: Optional[Waehrungseinheit] = None
+    einheit: Optional["Waehrungseinheit"] = None
     #: Größe, auf die sich die Einheit bezieht, beispielsweise kWh, Jahr
-    bezugseinheit: Optional[Mengeneinheit] = None
+    bezugseinheit: Optional["Mengeneinheit"] = None
     #: Hier sind die Staffeln mit ihren Preisangaben und regionalen Gültigkeiten definiert
-    preisstaffeln: Optional[list[RegionalePreisstaffel]] = None
+    preisstaffeln: Optional[list["RegionalePreisstaffel"]] = None
 
     #: Gibt an, nach welcher Menge die vorgenannte Einschränkung erfolgt (z.B. Jahresstromverbrauch in kWh)
-    mengeneinheitstaffel: Optional[Mengeneinheit] = None
+    mengeneinheitstaffel: Optional["Mengeneinheit"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/regionskriterium.py` & `bo4e-202401.1.2rc14/src/bo4e/com/regionskriterium.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Contains Regionskriterium class and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.gueltigkeitstyp import Gueltigkeitstyp
-from ..enum.regionskriteriumtyp import Regionskriteriumtyp
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.gueltigkeitstyp import Gueltigkeitstyp
+    from ..enum.regionskriteriumtyp import Regionskriteriumtyp
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Regionskriterium(COM):
     """
     Komponente zur Abbildung eines Regionskriteriums
@@ -22,18 +25,18 @@
         <object data="../_static/images/bo4e/com/Regionskriterium.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Regionskriterium JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Regionskriterium.json>`_
 
     """
 
-    gueltigkeitstyp: Optional[
-        Gueltigkeitstyp
-    ] = None  #: Hier wird festgelegt, ob es sich um ein einschließendes oder ausschließendes Kriterium handelt.
-    regionskriteriumtyp: Optional[
-        Regionskriteriumtyp
-    ] = None  #: Hier wird das Kriterium selbst angegeben, z.B. Bundesland.
+    gueltigkeitstyp: Optional["Gueltigkeitstyp"] = (
+        None  #: Hier wird festgelegt, ob es sich um ein einschließendes oder ausschließendes Kriterium handelt.
+    )
+    regionskriteriumtyp: Optional["Regionskriteriumtyp"] = (
+        None  #: Hier wird das Kriterium selbst angegeben, z.B. Bundesland.
+    )
     wert: Optional[str] = None
     """
     Der Wert, den das Kriterium annehmen kann, z.B. NRW.
     Im Falle des Regionskriteriumstyp BUNDESWEIT spielt dieser Wert keine Rolle.
     """
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/sigmoidparameter.py` & `bo4e-202401.1.2rc14/src/bo4e/com/sigmoidparameter.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,17 +26,7 @@
 
     """
 
     A: Optional[Decimal] = None  #: Briefmarke Ortsverteilnetz (EUR/kWh)
     B: Optional[Decimal] = None  #: Wendepunkt für die bepreiste Menge (kW)
     C: Optional[Decimal] = None  #: Exponent (einheitenlos)
     D: Optional[Decimal] = None  #: Briefmarke Transportnetz (EUR/kWh)
-
-    def calculate(self, leistung: Decimal) -> Decimal:
-        """
-        calculates LP
-        :param leistung: Leistung in Kilowatt
-        :return: den Sigmoidparameter LP in EUR/kWh
-        """
-        if self.A is None or self.B is None or self.C is None or self.D is None:
-            raise ValueError("Sigmoidparameter is not fully defined")
-        return self.A / (1 + (leistung / self.B) ** self.C) + self.D
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/standorteigenschaftengas.py` & `bo4e-202401.1.2rc14/src/bo4e/com/standorteigenschaftengas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Contains StandorteigenschaftenGas class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from ..utils import postprocess_docstring
 from .com import COM
-from .marktgebietinfo import MarktgebietInfo
+
+if TYPE_CHECKING:
+
+    from .marktgebietinfo import MarktgebietInfo
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class StandorteigenschaftenGas(COM):
@@ -24,8 +27,8 @@
 
     .. HINT::
         `StandorteigenschaftenGas JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/StandorteigenschaftenGas.json>`_
 
     """
 
     netzkontonummern: Optional[list[str]] = None  #: Netzkontonummern der Gasnetze
-    marktgebiete: Optional[list[MarktgebietInfo]] = None  #: Die Informationen zu Marktgebieten in dem Netz.
+    marktgebiete: Optional[list["MarktgebietInfo"]] = None  #: Die Informationen zu Marktgebieten in dem Netz.
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/standorteigenschaftenstrom.py` & `bo4e-202401.1.2rc14/src/bo4e/com/standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/steuerbetrag.py` & `bo4e-202401.1.2rc14/src/bo4e/com/steuerbetrag.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """
 Contains Steuerbetrag class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.steuerkennzeichen import Steuerkennzeichen
-from ..enum.waehrungscode import Waehrungscode
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.steuerkennzeichen import Steuerkennzeichen
+    from ..enum.waehrungscode import Waehrungscode
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Steuerbetrag(COM):
     """
     Abbildung eines Steuerbetrages.
@@ -25,14 +28,14 @@
 
     .. HINT::
         `Steuerbetrag JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Steuerbetrag.json>`_
 
     """
 
     #: Kennzeichnung des Steuersatzes, bzw. Verfahrens.
-    steuerkennzeichen: Optional[Steuerkennzeichen] = None
+    steuerkennzeichen: Optional["Steuerkennzeichen"] = None
     #: Nettobetrag für den die Steuer berechnet wurde. Z.B. 100
     basiswert: Optional[Decimal] = None
     #: Aus dem Basiswert berechnete Steuer. Z.B. 19 (bei UST_19)
     steuerwert: Optional[Decimal] = None
     #: Währung. Z.B. Euro.
-    waehrung: Optional[Waehrungscode] = None
+    waehrung: Optional["Waehrungscode"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/tarifberechnungsparameter.py` & `bo4e-202401.1.2rc14/src/bo4e/com/tarifberechnungsparameter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """
 Contains Tarifberechnungsparameter class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.messpreistyp import Messpreistyp
-from ..enum.tarifkalkulationsmethode import Tarifkalkulationsmethode
 from ..utils import postprocess_docstring
 from .com import COM
-from .preis import Preis
-from .tarifpreis import Tarifpreis
+
+if TYPE_CHECKING:
+    from ..enum.messpreistyp import Messpreistyp
+    from ..enum.tarifkalkulationsmethode import Tarifkalkulationsmethode
+    from .preis import Preis
+    from .tarifpreis import Tarifpreis
 
 # yes. there is no description in the official docs.
 # https://github.com/Hochfrequenz/BO4E-python/issues/328
 
 # pylint: disable=too-few-public-methods, empty-docstring, too-many-instance-attributes
 
 
@@ -31,36 +33,36 @@
         `Tarifberechnungsparameter JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Tarifberechnungsparameter.json>`_
 
     """
 
     # there are no required attributes
 
     #: Gibt an, wie die Einzelpreise des Tarifes zu verarbeiten sind
-    berechnungsmethode: Optional[Tarifkalkulationsmethode] = None
+    berechnungsmethode: Optional["Tarifkalkulationsmethode"] = None
     #: True, falls der Messpreis im Grundpreis (GP) enthalten ist
     ist_messpreis_in_grundpreis_enthalten: Optional[bool] = None
 
     ist_messpreis_zu_beruecksichtigen: Optional[bool] = None
     """
     True, falls bei der Bildung des Durchschnittspreises für die Höchst- und Mindestpreisbetrachtung der Messpreis mit
     berücksichtigt wird
     """
 
     #: Typ des Messpreises
-    messpreistyp: Optional[Messpreistyp] = None
+    messpreistyp: Optional["Messpreistyp"] = None
 
     #: Im Preis bereits eingeschlossene Leistung (für Gas)
     kw_inklusive: Optional[Decimal] = None
     # todo: type decimal is most likely wrong: https://github.com/Hochfrequenz/BO4E-python/issues/327
 
     #: Intervall, indem die über "kwInklusive" hinaus abgenommene Leistung kostenpflichtig wird (z.B. je 5 kW 20 EURO)
     kw_weitere_mengen: Optional[Decimal] = None
     # todo: type decimal is most likely wrong: https://github.com/Hochfrequenz/BO4E-python/issues/327
 
     #: Höchstpreis für den Durchschnitts-Arbeitspreis NT
-    hoechstpreis_n_t: Optional[Preis] = None
+    hoechstpreis_n_t: Optional["Preis"] = None
     #: Höchstpreis für den Durchschnitts-Arbeitspreis HT
-    hoechstpreis_h_t: Optional[Preis] = None
+    hoechstpreis_h_t: Optional["Preis"] = None
     #: Mindestpreis für den Durchschnitts-Arbeitspreis
-    mindestpreis: Optional[Preis] = None
+    mindestpreis: Optional["Preis"] = None
     #: Liste mit zusätzlichen Preisen, beispielsweise Messpreise und/oder Leistungspreise
-    zusatzpreise: Optional[list[Tarifpreis]] = None
+    zusatzpreise: Optional[list["Tarifpreis"]] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/tarifeinschraenkung.py` & `bo4e-202401.1.2rc14/src/bo4e/com/tarifeinschraenkung.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Contains Tarifeinschraenkung and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..bo.geraet import Geraet
-from ..enum.voraussetzungen import Voraussetzungen
 from ..utils import postprocess_docstring
 from .com import COM
-from .menge import Menge
+
+if TYPE_CHECKING:
+    from ..bo.geraet import Geraet
+    from ..enum.voraussetzungen import Voraussetzungen
+    from .menge import Menge
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Tarifeinschraenkung(COM):
     """
@@ -26,14 +28,14 @@
         `Tarifeinschraenkung JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Tarifeinschraenkung.json>`_
 
     """
 
     #: Weitere Produkte, die gemeinsam mit diesem Tarif bestellt werden können
     zusatzprodukte: Optional[list[str]] = None
     #: Voraussetzungen, die erfüllt sein müssen, damit dieser Tarif zur Anwendung kommen kann
-    voraussetzungen: Optional[list[Voraussetzungen]] = None
-    einschraenkungzaehler: Optional[list[Geraet]] = None
+    voraussetzungen: Optional[list["Voraussetzungen"]] = None
+    einschraenkungzaehler: Optional[list["Geraet"]] = None
     """ Liste der Zähler/Geräte, die erforderlich sind, damit dieser Tarif zur Anwendung gelangen kann.
     (Falls keine Zähler angegeben sind, ist der Tarif nicht an das Vorhandensein bestimmter Zähler gebunden.) """
-    einschraenkungleistung: Optional[list[Menge]] = None
+    einschraenkungleistung: Optional[list["Menge"]] = None
     """ Die vereinbarte Leistung, die (näherungsweise) abgenommen wird.
     Insbesondere Gastarife können daran gebunden sein, dass die Leistung einer vereinbarten Höhe entspricht. """
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/tarifpreis.py` & `bo4e-202401.1.2rc14/src/bo4e/com/tarifpreis.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Contains Tarifpreis class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.preistyp import Preistyp
 from ..utils import postprocess_docstring
 from .preis import Preis
 
+if TYPE_CHECKING:
+    from ..enum.preistyp import Preistyp
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Tarifpreis(Preis):
     """
     Abbildung eines Tarifpreises mit Preistyp und Beschreibung abgeleitet von COM Preis.
@@ -23,11 +26,11 @@
 
     .. HINT::
         `Tarifpreis JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Tarifpreis.json>`_
 
     """
 
     #:  Angabe des Preistypes (z.B. Grundpreis)
-    preistyp: Optional[Preistyp] = None
+    preistyp: Optional["Preistyp"] = None
 
     #:  Beschreibung des Preises. Hier können z.B. Preisdetails angegeben sein, beispielsweise "Drehstromzähler".
     beschreibung: Optional[str] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/tarifpreisposition.py` & `bo4e-202401.1.2rc14/src/bo4e/com/tarifpreisposition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 Contains Tarifpreisposition class
 and corresponding marshmallow schema for de-/serialization
 """
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.mengeneinheit import Mengeneinheit
-from ..enum.preistyp import Preistyp
-from ..enum.waehrungseinheit import Waehrungseinheit
 from ..utils import postprocess_docstring
 from .com import COM
-from .preisstaffel import Preisstaffel
+
+if TYPE_CHECKING:
+    from ..enum.mengeneinheit import Mengeneinheit
+    from ..enum.preistyp import Preistyp
+    from ..enum.waehrungseinheit import Waehrungseinheit
+    from .preisstaffel import Preisstaffel
 
 
 @postprocess_docstring
 class Tarifpreisposition(COM):
     """
     Mit dieser Komponente können Tarifpreise verschiedener Typen abgebildet werden.
 
@@ -26,17 +28,17 @@
 
     .. HINT::
         `Tarifpreisposition JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Tarifpreisposition.json>`_
 
     """
 
     #: Angabe des Preistypes (z.B. Grundpreis)
-    preistyp: Optional[Preistyp] = None
+    preistyp: Optional["Preistyp"] = None
     #: Einheit des Preises (z.B. EURO)
-    einheit: Optional[Waehrungseinheit] = None
+    einheit: Optional["Waehrungseinheit"] = None
     #: Größe, auf die sich die Einheit bezieht, beispielsweise kWh, Jahr
-    bezugseinheit: Optional[Mengeneinheit] = None
+    bezugseinheit: Optional["Mengeneinheit"] = None
     #: Hier sind die Staffeln mit ihren Preisenangaben definiert
-    preisstaffeln: Optional[list[Preisstaffel]] = None
+    preisstaffeln: Optional[list["Preisstaffel"]] = None
 
     #: Gibt an, nach welcher Menge die vorgenannte Einschränkung erfolgt (z.B. Jahresstromverbrauch in kWh)
-    mengeneinheitstaffel: Optional[Mengeneinheit] = None
+    mengeneinheitstaffel: Optional["Mengeneinheit"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/tarifpreispositionproort.py` & `bo4e-202401.1.2rc14/src/bo4e/com/tarifpreispositionproort.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """
 Contains TarifpreispositionProOrt class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from ..utils import postprocess_docstring
 from .com import COM
-from .tarifpreisstaffelproort import TarifpreisstaffelProOrt
+
+if TYPE_CHECKING:
+
+    from .tarifpreisstaffelproort import TarifpreisstaffelProOrt
 
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class TarifpreispositionProOrt(COM):
@@ -30,9 +33,9 @@
     #: Postleitzahl des Ortes für den der Preis gilt
     postleitzahl: Optional[str] = None
     #: Ort für den der Preis gilt
     ort: Optional[str] = None
     #: ene't-Netznummer des Netzes in dem der Preis gilt
     netznr: Optional[str] = None
     # Hier sind die Staffeln mit ihren Preisenangaben definiert
-    preisstaffeln: Optional[list[TarifpreisstaffelProOrt]] = None
+    preisstaffeln: Optional[list["TarifpreisstaffelProOrt"]] = None
     # there are no optional attributes
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/tarifpreisstaffelproort.py` & `bo4e-202401.1.2rc14/src/bo4e/com/tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/unterschrift.py` & `bo4e-202401.1.2rc14/src/bo4e/com/unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/verbrauch.py` & `bo4e-202401.1.2rc14/src/bo4e/com/verbrauch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """
 Contains Verbrauch and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 import pydantic
 
-from ..enum.mengeneinheit import Mengeneinheit
-from ..enum.messwertstatus import Messwertstatus
-from ..enum.wertermittlungsverfahren import Wertermittlungsverfahren
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.mengeneinheit import Mengeneinheit
+    from ..enum.messwertstatus import Messwertstatus
+    from ..enum.wertermittlungsverfahren import Wertermittlungsverfahren
+
+
 # pylint: disable=too-few-public-methods
 # pylint: disable=no-name-in-module
 
 
 @postprocess_docstring
 class Verbrauch(COM):
     """
@@ -28,21 +31,21 @@
 
     .. HINT::
         `Verbrauch JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Verbrauch.json>`_
 
     """
 
     #: Gibt an, ob es sich um eine PROGNOSE oder eine MESSUNG handelt
-    wertermittlungsverfahren: Optional[Wertermittlungsverfahren] = None
+    wertermittlungsverfahren: Optional["Wertermittlungsverfahren"] = None
     #: Die OBIS-Kennzahl für den Wert, die festlegt, welche Größe mit dem Stand gemeldet wird, z.B. '1-0:
     obis_kennzahl: Optional[str] = None
     #: Gibt den absoluten Wert der Menge an
     wert: Optional[Decimal] = None
     #: Gibt die Einheit zum jeweiligen Wert an
-    einheit: Optional[Mengeneinheit] = None
+    einheit: Optional["Mengeneinheit"] = None
 
     #: Inklusiver Beginn des Zeitraumes, für den der Verbrauch angegeben wird
     startdatum: Optional[pydantic.AwareDatetime] = None
     #: Exklusives Ende des Zeitraumes, für den der Verbrauch angegeben wird
     enddatum: Optional[pydantic.AwareDatetime] = None
     #: Messwertstatus includes the plausibility of the value
-    messwertstatus: Optional[Messwertstatus] = None
+    messwertstatus: Optional["Messwertstatus"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/vertragskonditionen.py` & `bo4e-202401.1.2rc14/src/bo4e/com/vertragskonditionen.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Contains Vertragskonditionen class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 from ..utils import postprocess_docstring
 from .com import COM
-from .zeitraum import Zeitraum
+
+if TYPE_CHECKING:
+
+    from .zeitraum import Zeitraum
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Vertragskonditionen(COM):
     """
@@ -28,14 +31,14 @@
     """
 
     #: Freitext zur Beschreibung der Konditionen, z.B. "Standardkonditionen Gas"
     beschreibung: Optional[str] = None
     #: Anzahl der vereinbarten Abschläge pro Jahr, z.B. 12
     anzahl_abschlaege: Optional[Decimal] = None
     #: Über diesen Zeitraum läuft der Vertrag
-    vertragslaufzeit: Optional[Zeitraum] = None
+    vertragslaufzeit: Optional["Zeitraum"] = None
     #: Innerhalb dieser Frist kann der Vertrag gekündigt werden
-    kuendigungsfrist: Optional[Zeitraum] = None
+    kuendigungsfrist: Optional["Zeitraum"] = None
     #: Falls der Vertrag nicht gekündigt wird, verlängert er sich automatisch um die hier angegebene Zeit
-    vertragsverlaengerung: Optional[Zeitraum] = None
+    vertragsverlaengerung: Optional["Zeitraum"] = None
     #: In diesen Zyklen werden Abschläge gestellt. Alternativ kann auch die Anzahl in den Konditionen angeben werden.
-    abschlagszyklus: Optional[Zeitraum] = None
+    abschlagszyklus: Optional["Zeitraum"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/vertragsteil.py` & `bo4e-202401.1.2rc14/src/bo4e/com/vertragsteil.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 Contains Vertragsteil class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 import pydantic
 
 from ..utils import postprocess_docstring
 from .com import COM
-from .menge import Menge
+
+if TYPE_CHECKING:
+
+    from .menge import Menge
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Vertragsteil(COM):
     """
@@ -39,19 +42,19 @@
     """
 
     lokation: Optional[str] = None
     """
     Der Identifier für diejenigen Markt- oder Messlokation, die zu diesem Vertragsteil gehören.
     Verträge für mehrere Lokationen werden mit mehreren Vertragsteilen abgebildet
     """
-    vertraglich_fixierte_menge: Optional[Menge] = None
+    vertraglich_fixierte_menge: Optional["Menge"] = None
     """
     Für die Lokation festgeschriebene Abnahmemenge
     """
-    minimale_abnahmemenge: Optional[Menge] = None
+    minimale_abnahmemenge: Optional["Menge"] = None
     """
     Für die Lokation festgelegte Mindestabnahmemenge (inklusiv)
     """
-    maximale_abnahmemenge: Optional[Menge] = None
+    maximale_abnahmemenge: Optional["Menge"] = None
     """
     Für die Lokation festgelegte maximale Abnahmemenge (exklusiv)
     """
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/verwendungszweckpromarktrolle.py` & `bo4e-202401.1.2rc14/src/bo4e/com/verwendungszweckpromarktrolle.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Contains Verwendungszweck class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..com.com import COM
-from ..enum.marktrolle import Marktrolle
-from ..enum.verwendungszweck import Verwendungszweck
 from ..utils import postprocess_docstring
+from .com import COM
+
+if TYPE_CHECKING:
+    from ..enum.marktrolle import Marktrolle
+    from ..enum.verwendungszweck import Verwendungszweck
+
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class VerwendungszweckProMarktrolle(COM):
     """
@@ -23,15 +26,15 @@
         <object data="../_static/images/bo4e/com/Verwendungszweck.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Verwendungszweck JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Verwendungszweck.json>`_
 
     """
 
-    marktrolle: Optional[Marktrolle] = None
+    marktrolle: Optional["Marktrolle"] = None
     """
     Marktrolle, für die die Daten relevant sind
     """
-    Zwecke: Optional[list[Verwendungszweck]] = None
+    Zwecke: Optional[list["Verwendungszweck"]] = None
     """
     Verwendungszwecke
     """
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/zaehlwerk.py` & `bo4e-202401.1.2rc14/src/bo4e/com/zaehlwerk.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 Contains Zaehlwerk class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..com.konzessionsabgabe import Konzessionsabgabe
-from ..com.verwendungszweckpromarktrolle import VerwendungszweckProMarktrolle
-from ..com.zaehlzeitregister import Zaehlzeitregister
-from ..enum.energierichtung import Energierichtung
-from ..enum.mengeneinheit import Mengeneinheit
-from ..enum.verbrauchsart import Verbrauchsart
-from ..enum.waermenutzung import Waermenutzung
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..com.konzessionsabgabe import Konzessionsabgabe
+    from ..com.verwendungszweckpromarktrolle import VerwendungszweckProMarktrolle
+    from ..com.zaehlzeitregister import Zaehlzeitregister
+    from ..enum.energierichtung import Energierichtung
+    from ..enum.mengeneinheit import Mengeneinheit
+    from ..enum.verbrauchsart import Verbrauchsart
+    from ..enum.waermenutzung import Waermenutzung
+
+
 # pylint: disable=no-name-in-module
 # pylint: disable=no-name-in-module
 
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
@@ -35,33 +38,33 @@
         `Zaehlwerk JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Zaehlwerk.json>`_
 
     """
 
     zaehlwerk_id: Optional[str] = None  # Identifikation des Zählwerks (Registers) innerhalb des Zählers.
     # Oftmals eine laufende Nummer hinter der Zählernummer. Z.B. 47110815_1
     bezeichnung: Optional[str] = None  # Zusätzliche Bezeichnung, z.B. Zählwerk_Wirkarbeit.
-    richtung: Optional[Energierichtung] = None  # Die Energierichtung, Einspeisung oder Ausspeisung.
-    obis_kennzahl: Optional[
-        str
-    ] = None  # Die OBIS-Kennzahl für das Zählwerk, die festlegt, welche auf die gemessene Größe mit dem Stand gemeldet wird.
+    richtung: Optional["Energierichtung"] = None  # Die Energierichtung, Einspeisung oder Ausspeisung.
+    obis_kennzahl: Optional[str] = (
+        None  # Die OBIS-Kennzahl für das Zählwerk, die festlegt, welche auf die gemessene Größe mit dem Stand gemeldet wird.
+    )
     # Nur Zählwerkstände mit dieser OBIS-Kennzahl werden an diesem Zählwerk registriert.
-    wandlerfaktor: Optional[
-        Decimal
-    ] = None  # Mit diesem Faktor wird eine Zählerstandsdifferenz multipliziert, um zum eigentlichen Verbrauch im Zeitraum
+    wandlerfaktor: Optional[Decimal] = (
+        None  # Mit diesem Faktor wird eine Zählerstandsdifferenz multipliziert, um zum eigentlichen Verbrauch im Zeitraum
+    )
     # zu kommen.
-    einheit: Optional[Mengeneinheit] = None  # Die Einheit der gemessenen Größe, z.B. kWh
+    einheit: Optional["Mengeneinheit"] = None  # Die Einheit der gemessenen Größe, z.B. kWh
     ist_schwachlastfaehig: Optional[bool] = None  #: Schwachlastfaehigkeit
-    verwendungszwecke: Optional[
-        list[VerwendungszweckProMarktrolle]
-    ] = None  #: Verwendungungszweck der Werte Marktlokation
-    verbrauchsart: Optional[Verbrauchsart] = None  #: Stromverbrauchsart/Verbrauchsart Marktlokation
+    verwendungszwecke: Optional[list["VerwendungszweckProMarktrolle"]] = (
+        None  #: Verwendungungszweck der Werte Marktlokation
+    )
+    verbrauchsart: Optional["Verbrauchsart"] = None  #: Stromverbrauchsart/Verbrauchsart Marktlokation
     ist_unterbrechbar: Optional[bool] = None  #: Unterbrechbarkeit Marktlokation
-    waermenutzung: Optional[Waermenutzung] = None  #: Wärmenutzung Marktlokation
-    konzessionsabgabe: Optional[Konzessionsabgabe] = None  #: Konzessionsabgabe
+    waermenutzung: Optional["Waermenutzung"] = None  #: Wärmenutzung Marktlokation
+    konzessionsabgabe: Optional["Konzessionsabgabe"] = None  #: Konzessionsabgabe
     ist_steuerbefreit: Optional[bool] = None  #: Steuerbefreiung
     vorkommastelle: Optional[int] = None  #: Anzahl der Vorkommastellen
     nachkommastelle: Optional[int] = None  #: Anzahl der Nachkommastellen
     ist_abrechnungsrelevant: Optional[bool] = None  #: Abrechnungsrelevant
     anzahlAblesungen: Optional[int] = None  #: Anzahl Ablesungen pro Jahr
-    zaehlzeitregister: Optional[
-        Zaehlzeitregister
-    ] = None  #: Erweiterte Definition der Zählzeit in Bezug auf ein Register
+    zaehlzeitregister: Optional["Zaehlzeitregister"] = (
+        None  #: Erweiterte Definition der Zählzeit in Bezug auf ein Register
+    )
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/zaehlzeitregister.py` & `bo4e-202401.1.2rc14/src/bo4e/com/zaehlzeitregister.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Contains Zaehlzeitregister class and corresponding marshmallow schema for de-/serialization
 """
 
 from typing import Optional
 
-from ..com.com import COM
 from ..utils import postprocess_docstring
+from .com import COM
 
 # pylint: disable=no-name-in-module
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Zaehlzeitregister(COM):
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/zeitraum.py` & `bo4e-202401.1.2rc14/src/bo4e/com/zeitraum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 Contains Zeitraum class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
 import pydantic
 
-from ..enum.mengeneinheit import Mengeneinheit
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.mengeneinheit import Mengeneinheit
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Zeitraum(COM):
     """
     Diese Komponente wird zur Abbildung von Zeiträumen in Form von Dauern oder der Angabe von Start und Ende verwendet.
@@ -29,13 +32,13 @@
         <object data="../_static/images/bo4e/com/Zeitraum.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Zeitraum JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Zeitraum.json>`_
 
     """
 
-    einheit: Optional[Mengeneinheit] = None
+    einheit: Optional["Mengeneinheit"] = None
     dauer: Optional[Decimal] = None
     startdatum: Optional[pydantic.AwareDatetime] = None
     enddatum: Optional[pydantic.AwareDatetime] = None
     startzeitpunkt: Optional[pydantic.AwareDatetime] = None
     endzeitpunkt: Optional[pydantic.AwareDatetime] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/zeitreihenwert.py` & `bo4e-202401.1.2rc14/src/bo4e/com/zeitreihenwert.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """
 Contains Zeitreihenwert class
 and corresponding marshmallow schema for de-/serialization
 """
 
 from decimal import Decimal
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..com.zeitspanne import Zeitspanne
-from ..enum.messwertstatus import Messwertstatus
-from ..enum.messwertstatuszusatz import Messwertstatuszusatz
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..com.zeitspanne import Zeitspanne
+    from ..enum.messwertstatus import Messwertstatus
+    from ..enum.messwertstatuszusatz import Messwertstatuszusatz
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Zeitreihenwert(COM):
     """
     Abbildung eines Zeitreihenwertes bestehend aus Zeitraum, Wert und Statusinformationen.
@@ -25,16 +28,16 @@
         <object data="../_static/images/bo4e/com/Zeitreihenwert.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Zeitreihenwert JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Zeitreihenwert.json>`_
 
     """
 
-    zeitspanne: Optional[Zeitspanne] = None  #: Zeitespanne für das Messintervall
+    zeitspanne: Optional["Zeitspanne"] = None  #: Zeitespanne für das Messintervall
 
     wert: Optional[Decimal] = None  #: Der in der Zeitspanne gültige Wert.
 
     #: Der Status gibt an, wie der Wert zu interpretieren ist, z.B. in Berechnungen.
-    status: Optional[Messwertstatus] = None
+    status: Optional["Messwertstatus"] = None
 
     #: Eine Zusatzinformation zum Status, beispielsweise ein Grund für einen fehlenden Wert.
-    statuszusatz: Optional[Messwertstatuszusatz] = None
+    statuszusatz: Optional["Messwertstatuszusatz"] = None
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/zeitspanne.py` & `bo4e-202401.1.2rc14/src/bo4e/com/zeitspanne.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/com/zustaendigkeit.py` & `bo4e-202401.1.2rc14/src/bo4e/com/zustaendigkeit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 Contains Zustaendigkeit class
 and corresponding marshmallow schema for de-/serialization
 """
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
 
-from ..enum.themengebiet import Themengebiet
 from ..utils import postprocess_docstring
 from .com import COM
 
+if TYPE_CHECKING:
+    from ..enum.themengebiet import Themengebiet
+
+
 # pylint: disable=too-few-public-methods
 
 
 @postprocess_docstring
 class Zustaendigkeit(COM):
     """
     Enthält die zeitliche Zuordnung eines Ansprechpartners zu Abteilungen und Zuständigkeiten.
@@ -22,14 +25,14 @@
         <object data="../_static/images/bo4e/com/Zustaendigkeit.svg" type="image/svg+xml"></object>
 
     .. HINT::
         `Zustaendigkeit JSON Schema <https://json-schema.app/view/%23?url=https://raw.githubusercontent.com/BO4E/BO4E-Schemas/{__gh_version__}/src/bo4e_schemas/com/Zustaendigkeit.json>`_
 
     """
 
-    themengebiet: Optional[Themengebiet] = None
+    themengebiet: Optional["Themengebiet"] = None
     """
     Hier kann eine thematische Zuordnung des Ansprechpartners bzw. der Person angegeben werden
     """
 
     position: Optional[str] = None  #: Berufliche Rolle des Ansprechpartners/ der Person
     abteilung: Optional[str] = None  #: Abteilung, in der der Ansprechpartner/ die Person tätig ist
```

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/abgabeart.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/abgabeart.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/angebotsstatus.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/angebotsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/artikelid.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/artikelid.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/aufabschlagsziel.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/aufabschlagsziel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/ausschreibungsportal.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/ausschreibungsportal.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/bdewartikelnummer.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/bdewartikelnummer.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/bemessungsgroesse.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/bemessungsgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/bilanzierungsmethode.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/bilanzierungsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/dienstleistungstyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/dienstleistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/erzeugungsart.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/erzeugungsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/gebiettyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/gebiettyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/geraeteklasse.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/geraeteklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/geraetetyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/geraetetyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/gueltigkeitstyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/gueltigkeitstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/kalkulationsmethode.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/kalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/kostenklasse.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/kostenklasse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/kundengruppe.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/kundengruppe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/kundengruppeka.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/kundengruppeka.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/kundentyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/kundentyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/leistungstyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/leistungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/marktrolle.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/marktrolle.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/mengeneinheit.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/mengeneinheit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/messgroesse.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/messgroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/messpreistyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/messpreistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/messwertstatus.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/messwertstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/messwertstatuszusatz.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/messwertstatuszusatz.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/netzebene.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/netzebene.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/netznutzungrechnungstyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/netznutzungrechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/oekolabel.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/oekolabel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/oekozertifikat.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/oekozertifikat.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/preisgarantietyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/preisgarantietyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/preistyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/preistyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/rechnungslegung.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/rechnungslegung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/rechnungsstatus.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/rechnungsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/rechnungstyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/rechnungstyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/regionskriteriumtyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/regionskriteriumtyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/steuerkennzeichen.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/steuerkennzeichen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/tarifkalkulationsmethode.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/tarifkalkulationsmethode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/tarifmerkmal.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/tarifmerkmal.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/themengebiet.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/themengebiet.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/typ.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/typ.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/vertragsart.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/vertragsart.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/vertragsstatus.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/vertragsstatus.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/verwendungszweck.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/verwendungszweck.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/voraussetzungen.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/voraussetzungen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/waehrungscode.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/waehrungscode.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/zaehlergroesse.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/zaehlergroesse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/enum/zaehlertyp.py` & `bo4e-202401.1.2rc14/src/bo4e/enum/zaehlertyp.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/src/bo4e/utils/__init__.py` & `bo4e-202401.1.2rc14/src/bo4e/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,17 @@
                 break
         if description is not None:
             field_info.description = description
             continue
 
         print(f"Could not find a comment for field {field_name} in class {cls}")
 
-    cls.model_rebuild(force=True)
+    # cls.model_rebuild(force=True)
+    # Unnecessary here since the models will be rebuilt in __init__.py.
+    # Keeping this here as comment though.
     return cls
 
 
 def postprocess_docstring(cls: type[T]) -> type[T]:
     """
     Postprocess the docstring to inject the __gh_version__ for proper linking of the JSON-schemas.
     Note that doc-strings in Python have to be string literals, so we cannot use f-strings.
```

### Comparing `bo4e-202401.1.1rc4/tests/serialization_helper.py` & `bo4e-202401.1.2rc14/tests/serialization_helper.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_adresse.py` & `bo4e-202401.1.2rc14/tests/test_adresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_angebot.py` & `bo4e-202401.1.2rc14/tests/test_angebot.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_angebotsposition.py` & `bo4e-202401.1.2rc14/tests/test_angebotsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_angebotsteil.py` & `bo4e-202401.1.2rc14/tests/test_angebotsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_angebotsvariante.py` & `bo4e-202401.1.2rc14/tests/test_angebotsvariante.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_aufabschlag.py` & `bo4e-202401.1.2rc14/tests/test_aufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_aufabschlagproort.py` & `bo4e-202401.1.2rc14/tests/test_aufabschlagproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_aufabschlagregional.py` & `bo4e-202401.1.2rc14/tests/test_aufabschlagregional.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_aufabschlagstaffelproort.py` & `bo4e-202401.1.2rc14/tests/test_aufabschlagstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_ausschreibung.py` & `bo4e-202401.1.2rc14/tests/test_ausschreibung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_ausschreibungsdetail.py` & `bo4e-202401.1.2rc14/tests/test_ausschreibungsdetail.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_ausschreibungslos.py` & `bo4e-202401.1.2rc14/tests/test_ausschreibungslos.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_betrag.py` & `bo4e-202401.1.2rc14/tests/test_betrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_buendelvertrag.py` & `bo4e-202401.1.2rc14/tests/test_buendelvertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_energieherkunft.py` & `bo4e-202401.1.2rc14/tests/test_energieherkunft.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_energiemenge.py` & `bo4e-202401.1.2rc14/tests/test_energiemenge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_energiemix.py` & `bo4e-202401.1.2rc14/tests/test_energiemix.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_enums.py` & `bo4e-202401.1.2rc14/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_fremdkosten.py` & `bo4e-202401.1.2rc14/tests/test_fremdkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_fremdkostenblock.py` & `bo4e-202401.1.2rc14/tests/test_fremdkostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_fremdkostenposition.py` & `bo4e-202401.1.2rc14/tests/test_fremdkostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_geokoordinaten.py` & `bo4e-202401.1.2rc14/tests/test_geokoordinaten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_geraet.py` & `bo4e-202401.1.2rc14/tests/test_geraet.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_geschaeftsobjekt.py` & `bo4e-202401.1.2rc14/tests/test_geschaeftsobjekt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_geschaeftspartner.py` & `bo4e-202401.1.2rc14/tests/test_geschaeftspartner.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_katasteradresse.py` & `bo4e-202401.1.2rc14/tests/test_katasteradresse.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_kontakt.py` & `bo4e-202401.1.2rc14/tests/test_kontakt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_kosten.py` & `bo4e-202401.1.2rc14/tests/test_kosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_kostenblock.py` & `bo4e-202401.1.2rc14/tests/test_kostenblock.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_kostenposition.py` & `bo4e-202401.1.2rc14/tests/test_kostenposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_kriteriumswert.py` & `bo4e-202401.1.2rc14/tests/test_kriteriumswert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_lastgang.py` & `bo4e-202401.1.2rc14/tests/test_lastgang.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_marktgebietinfo.py` & `bo4e-202401.1.2rc14/tests/test_marktgebietinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_marktlokation.py` & `bo4e-202401.1.2rc14/tests/test_marktlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_marktteilnehmer.py` & `bo4e-202401.1.2rc14/tests/test_marktteilnehmer.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_menge.py` & `bo4e-202401.1.2rc14/tests/test_menge.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_messlokation.py` & `bo4e-202401.1.2rc14/tests/test_messlokation.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_messlokationszuordnung.py` & `bo4e-202401.1.2rc14/tests/test_messlokationszuordnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_person.py` & `bo4e-202401.1.2rc14/tests/test_person.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_positionsaufabschlag.py` & `bo4e-202401.1.2rc14/tests/test_positionsaufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preis.py` & `bo4e-202401.1.2rc14/tests/test_preis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preisblatt.py` & `bo4e-202401.1.2rc14/tests/test_preisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preisblatt_dienstleistung.py` & `bo4e-202401.1.2rc14/tests/test_preisblatt_dienstleistung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preisblatt_hardware.py` & `bo4e-202401.1.2rc14/tests/test_preisblatt_hardware.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preisblatt_konzessionsabgabe.py` & `bo4e-202401.1.2rc14/tests/test_preisblatt_konzessionsabgabe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preisblatt_messung.py` & `bo4e-202401.1.2rc14/tests/test_preisblatt_messung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preisblattnetznutzung.py` & `bo4e-202401.1.2rc14/tests/test_preisblattnetznutzung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preisgarantie.py` & `bo4e-202401.1.2rc14/tests/test_preisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preisposition.py` & `bo4e-202401.1.2rc14/tests/test_preisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_preisstaffel.py` & `bo4e-202401.1.2rc14/tests/test_preisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_rechnung.py` & `bo4e-202401.1.2rc14/tests/test_rechnung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_rechnungsposition.py` & `bo4e-202401.1.2rc14/tests/test_rechnungsposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_region.py` & `bo4e-202401.1.2rc14/tests/test_region.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_regionalegueltigkeit.py` & `bo4e-202401.1.2rc14/tests/test_regionalegueltigkeit.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_regionalepreisgarantie.py` & `bo4e-202401.1.2rc14/tests/test_regionalepreisgarantie.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_regionalepreisstaffel.py` & `bo4e-202401.1.2rc14/tests/test_regionalepreisstaffel.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_regionaleraufabschlag.py` & `bo4e-202401.1.2rc14/tests/test_regionaleraufabschlag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_regionaletarifpreisposition.py` & `bo4e-202401.1.2rc14/tests/test_regionaletarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_regionaltarif.py` & `bo4e-202401.1.2rc14/tests/test_regionaltarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_regionskriterium.py` & `bo4e-202401.1.2rc14/tests/test_regionskriterium.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_standorteigenschaften.py` & `bo4e-202401.1.2rc14/tests/test_standorteigenschaften.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_standorteigenschaftengas.py` & `bo4e-202401.1.2rc14/tests/test_standorteigenschaftengas.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_standorteigenschaftenstrom.py` & `bo4e-202401.1.2rc14/tests/test_standorteigenschaftenstrom.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_steuerbetrag.py` & `bo4e-202401.1.2rc14/tests/test_steuerbetrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarif.py` & `bo4e-202401.1.2rc14/tests/test_tarif.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarifberechnungsparameter.py` & `bo4e-202401.1.2rc14/tests/test_tarifberechnungsparameter.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarifeinschraenkung.py` & `bo4e-202401.1.2rc14/tests/test_tarifeinschraenkung.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarifinfo.py` & `bo4e-202401.1.2rc14/tests/test_tarifinfo.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarifkosten.py` & `bo4e-202401.1.2rc14/tests/test_tarifkosten.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarifpreis.py` & `bo4e-202401.1.2rc14/tests/test_tarifpreis.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarifpreisblatt.py` & `bo4e-202401.1.2rc14/tests/test_tarifpreisblatt.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarifpreisposition.py` & `bo4e-202401.1.2rc14/tests/test_tarifpreisposition.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarifpreispositionproort.py` & `bo4e-202401.1.2rc14/tests/test_tarifpreispositionproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_tarifpreisstaffelproort.py` & `bo4e-202401.1.2rc14/tests/test_tarifpreisstaffelproort.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_unterschrift.py` & `bo4e-202401.1.2rc14/tests/test_unterschrift.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_verbrauch.py` & `bo4e-202401.1.2rc14/tests/test_verbrauch.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_vertrag.py` & `bo4e-202401.1.2rc14/tests/test_vertrag.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_vertragskonditionen.py` & `bo4e-202401.1.2rc14/tests/test_vertragskonditionen.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_vertragsteil.py` & `bo4e-202401.1.2rc14/tests/test_vertragsteil.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_zaehler.py` & `bo4e-202401.1.2rc14/tests/test_zaehler.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_zeitraum.py` & `bo4e-202401.1.2rc14/tests/test_zeitraum.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_zeitreihe.py` & `bo4e-202401.1.2rc14/tests/test_zeitreihe.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_zeitreihenwert.py` & `bo4e-202401.1.2rc14/tests/test_zeitreihenwert.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_zeitspanne.py` & `bo4e-202401.1.2rc14/tests/test_zeitspanne.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/test_zusatz_attribut.py` & `bo4e-202401.1.2rc14/tests/test_zusatz_attribut.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/tests/utils.py` & `bo4e-202401.1.2rc14/tests/utils.py`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/.gitignore` & `bo4e-202401.1.2rc14/.gitignore`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/LICENSE.rst` & `bo4e-202401.1.2rc14/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `bo4e-202401.1.1rc4/pyproject.toml` & `bo4e-202401.1.2rc14/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -84,7 +84,13 @@
 # for strict mypy: (this is the tricky one :-))
 disallow_untyped_defs = true
 [tool.pydantic-mypy]
 init_forbid_extra = true
 init_typed = true
 warn_required_dynamic_aliases = true
 warn_untyped_fields = true
+
+[tool.coverage.report]
+exclude_also = [
+    # This covers both typing.TYPE_CHECKING and plain TYPE_CHECKING, with any amount of whitespace
+    "if\\s+(typing\\.)?TYPE_CHECKING:"
+]
```

### Comparing `bo4e-202401.1.1rc4/PKG-INFO` & `bo4e-202401.1.2rc14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bo4e
-Version: 202401.1.1rc4
+Version: 202401.1.2rc14
 Summary: Python Library that implements the BO4E Standard.
 Project-URL: Changelog, https://github.com/bo4e/bo4e-python/releases
 Project-URL: Homepage, https://github.com/bo4e/bo4e-python
 Project-URL: Documentation, https://bo4e-python.readthedocs.io/en/latest/
 Author-email: Kevin Krechan <kevin.krechan@hochfrequenz.de>, Leon Haffmans <leon.haffmans@hochfrequenz.de>, Annika Schlögl <annika.schloegl@hochfrequenz.de>, Franziska Vesely <franziska.vesely@hochfrequenz.de>, Konstantin Klein <konstantin.klein@hochfrequenz.de>
 License: MIT
 License-File: AUTHORS.rst
```

