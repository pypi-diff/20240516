# Comparing `tmp/h5rdmtoolbox-1.3.0a1.tar.gz` & `tmp/h5rdmtoolbox-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5rdmtoolbox-1.3.0a1.tar", last modified: Thu May  2 12:07:38 2024, max compression
+gzip compressed data, was "h5rdmtoolbox-1.3.1.tar", last modified: Thu May 16 14:09:54 2024, max compression
```

## Comparing `h5rdmtoolbox-1.3.0a1.tar` & `h5rdmtoolbox-1.3.1.tar`

### file list

```diff
@@ -1,165 +1,165 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.722196 h5rdmtoolbox-1.3.0a1/
--rw-rw-rw-   0        0        0     1090 2024-04-22 14:41:40.000000 h5rdmtoolbox-1.3.0a1/LICENSE
--rw-rw-rw-   0        0        0    14625 2024-05-02 12:07:38.721208 h5rdmtoolbox-1.3.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     9172 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.300527 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/
--rw-rw-rw-   0        0        0     9533 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/__init__.py
--rw-rw-rw-   0        0        0     3913 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_cfg.py
--rw-rw-rw-   0        0        0    26542 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_repr.py
--rw-rw-rw-   0        0        0     5257 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_user.py
--rw-rw-rw-   0        0        0      232 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_version.py
--rw-rw-rw-   0        0        0     1621 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/cli.py
--rw-rw-rw-   0        0        0       94 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/consts.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.345535 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/
--rw-rw-rw-   0        0        0     1402 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/__init__.py
--rw-rw-rw-   0        0        0       56 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/cfg.py
--rw-rw-rw-   0        0        0      775 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/consts.py
--rw-rw-rw-   0        0        0    31958 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/core.py
--rw-rw-rw-   0        0        0      988 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/definition.py
--rw-rw-rw-   0        0        0     1026 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/errors.py
--rw-rw-rw-   0        0        0    17349 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/generate.py
--rw-rw-rw-   0        0        0     2724 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/hdf_ontology.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.352535 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/
--rw-rw-rw-   0        0        0      150 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/__init__.py
--rw-rw-rw-   0        0        0     1308 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/h5namespace.py
--rw-rw-rw-   0        0        0     1445 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/h5ontocls.py
--rw-rw-rw-   0        0        0      417 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/references.py
--rw-rw-rw-   0        0        0    17167 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_attributes.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.405058 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/
--rw-rw-rw-   0        0        0     2125 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/__init__.py
--rw-rw-rw-   0        0        0     4726 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/accessor.py
--rw-rw-rw-   0        0        0    13103 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/affixes.py
--rw-rw-rw-   0        0        0       51 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/cache.py
--rw-rw-rw-   0        0        0      469 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/consts.py
--rw-rw-rw-   0        0        0     6662 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/h5interface.py
--rw-rw-rw-   0        0        0     4808 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/name.py
--rw-rw-rw-   0        0        0    35542 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/table.py
--rw-rw-rw-   0        0        0    10035 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/transformation.py
--rw-rw-rw-   0        0        0     2354 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/utils.py
--rw-rw-rw-   0        0        0     8680 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/toolbox_validators.py
--rw-rw-rw-   0        0        0     7428 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/utils.py
--rw-rw-rw-   0        0        0      146 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/warnings.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.471603 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/
--rw-rw-rw-   0        0        0     1084 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/def_icon.png
--rw-rw-rw-   0        0        0     1070 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/fluid-v1.yml
--rw-rw-rw-   0        0        0      717 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/h5tbx.yaml
--rw-rw-rw-   0        0        0     2587 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/id_icon.png
--rw-rw-rw-   0        0        0     3340 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/iri_icon.png
--rw-rw-rw-   0        0        0     1064 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/piv-v1.yml
--rw-rw-rw-   0        0        0     3651 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/style.css
--rw-rw-rw-   0        0        0     2532 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/tutorial_convention.yaml
--rw-rw-rw-   0        0        0     2558 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/tutorial_standard_name_table.yaml
--rw-rw-rw-   0        0        0     3287 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/type_icon.png
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.499606 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/
--rw-rw-rw-   0        0        0     3170 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.513607 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/
--rw-rw-rw-   0        0        0      107 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/__init__.py
--rw-rw-rw-   0        0        0     4727 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/filedb.py
--rw-rw-rw-   0        0        0    21521 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/objdb.py
--rw-rw-rw-   0        0        0     2697 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/query.py
--rw-rw-rw-   0        0        0     1933 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/utils.py
--rw-rw-rw-   0        0        0     2156 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/interface.py
--rw-rw-rw-   0        0        0    14802 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/mongo.py
--rw-rw-rw-   0        0        0        0 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/dev.py
--rw-rw-rw-   0        0        0      123 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.525612 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/
--rw-rw-rw-   0        0        0        0 2023-03-27 13:37:37.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/__init__.py
--rw-rw-rw-   0        0        0     2507 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/magnitude.py
--rw-rw-rw-   0        0        0     4045 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/normalize.py
--rw-rw-rw-   0        0        0     1903 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/units.py
--rw-rw-rw-   0        0        0     4872 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/vector.py
--rw-rw-rw-   0        0        0     8675 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/identifiers.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.530609 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/layout/
--rw-rw-rw-   0        0        0       50 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/layout/__init__.py
--rw-rw-rw-   0        0        0    24988 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/layout/core.py
--rw-rw-rw-   0        0        0     6546 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/plotting.py
--rw-rw-rw-   0        0        0      290 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/protected_attributes.py
--rw-rw-rw-   0        0        0     5282 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/protocols.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.533609 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/
--rw-rw-rw-   0        0        0      337 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/__init__.py
--rw-rw-rw-   0        0        0     2039 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/interface.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.545621 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/
--rw-rw-rw-   0        0        0      222 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/__init__.py
--rw-rw-rw-   0        0        0    16277 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/core.py
--rw-rw-rw-   0        0        0     7647 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/metadata.py
--rw-rw-rw-   0        0        0     3533 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/tokens.py
--rw-rw-rw-   0        0        0      610 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/utils.py
--rw-rw-rw-   0        0        0    15780 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/tutorial.py
--rw-rw-rw-   0        0        0    21187 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/utils.py
--rw-rw-rw-   0        0        0      101 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/warnings.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.572663 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/
--rw-rw-rw-   0        0        0       99 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/__init__.py
--rw-rw-rw-   0        0        0     3106 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/accessor.py
--rw-rw-rw-   0        0        0    96947 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/core.py
--rw-rw-rw-   0        0        0     4027 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/ds_decoder.py
--rw-rw-rw-   0        0        0    18622 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5attr.py
--rw-rw-rw-   0        0        0      465 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5ext.py
--rw-rw-rw-   0        0        0      899 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5utils.py
--rw-rw-rw-   0        0        0     4047 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5yaml.py
--rw-rw-rw-   0        0        0    42227 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/jsonld.py
--rw-rw-rw-   0        0        0     6241 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/lazy.py
--rw-rw-rw-   0        0        0    17291 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/rdf.py
--rw-rw-rw-   0        0        0     4582 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/xr2hdf.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.710194 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/
--rw-rw-rw-   0        0        0    14625 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4872 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      976 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-02 12:07:38.000000 h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-03-08 18:17:38.000000 h5rdmtoolbox-1.3.0a1/pyproject.toml
--rw-rw-rw-   0        0        0     2271 2024-05-02 12:07:38.724196 h5rdmtoolbox-1.3.0a1/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-09-27 08:03:12.000000 h5rdmtoolbox-1.3.0a1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.595663 h5rdmtoolbox-1.3.0a1/tests/
--rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.0a1/tests/__init__.py
--rw-rw-rw-   0        0        0     1013 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/clean_zenodo_sandbox.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.616660 h5rdmtoolbox-1.3.0a1/tests/conventions/
--rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.624662 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/
--rw-rw-rw-   0        0        0        0 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.660187 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/
--rw-rw-rw-   0        0        0        0 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/__init__.py
--rw-rw-rw-   0        0        0     6464 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_interface.py
--rw-rw-rw-   0        0        0     6827 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_provenance.py
--rw-rw-rw-   0        0        0    13348 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_snt.py
--rw-rw-rw-   0        0        0    13236 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_transformations_and_affixes.py
--rw-rw-rw-   0        0        0     2503 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/test_standard_attributes.py
--rw-rw-rw-   0        0        0    13045 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/test_standard_names.py
--rw-rw-rw-   0        0        0    30934 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_conventions.py
--rw-rw-rw-   0        0        0     2051 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_engmeta.py
--rw-rw-rw-   0        0        0     8450 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_ontology.py
--rw-rw-rw-   0        0        0      548 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_references.py
--rw-rw-rw-   0        0        0     5094 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_toolbox_validators.py
--rw-rw-rw-   0        0        0     5060 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/conventions/test_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.670187 h5rdmtoolbox-1.3.0a1/tests/database/
--rw-rw-rw-   0        0        0        0 2023-12-12 15:09:30.000000 h5rdmtoolbox-1.3.0a1/tests/database/__init__.py
--rw-rw-rw-   0        0        0     1252 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/database/test_find_rdf.py
--rw-rw-rw-   0        0        0    25285 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/database/test_hdfDB.py
--rw-rw-rw-   0        0        0     9625 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/database/test_mongo.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.677187 h5rdmtoolbox-1.3.0a1/tests/layouts/
--rw-rw-rw-   0        0        0        0 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/layouts/__init__.py
--rw-rw-rw-   0        0        0    12712 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/layouts/test_core.py
--rw-rw-rw-   0        0        0     2282 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/layouts/test_docs.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.681208 h5rdmtoolbox-1.3.0a1/tests/repository/
--rw-rw-rw-   0        0        0        0 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/repository/__init__.py
--rw-rw-rw-   0        0        0    18963 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/repository/test_zenodo.py
--rw-rw-rw-   0        0        0     2679 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/tests/test_config.py
--rw-rw-rw-   0        0        0     6015 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_extensions.py
--rw-rw-rw-   0        0        0     4243 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_identifiers.py
--rw-rw-rw-   0        0        0     6930 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/test_plotting.py
--rw-rw-rw-   0        0        0     5035 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_repr.py
--rw-rw-rw-   0        0        0     4079 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_user.py
--rw-rw-rw-   0        0        0     4604 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/test_utils.py
--rw-rw-rw-   0        0        0      798 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.0a1/tests/test_version.py
--rw-rw-rw-   0        0        0     1169 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.0a1/tests/test_xarray_export.py
-drwxrwxrwx   0        0        0        0 2024-05-02 12:07:38.707191 h5rdmtoolbox-1.3.0a1/tests/wrapper/
--rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/__init__.py
--rw-rw-rw-   0        0        0    43471 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_core.py
--rw-rw-rw-   0        0        0     2020 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_dump.py
--rw-rw-rw-   0        0        0    16978 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_file.py
--rw-rw-rw-   0        0        0      829 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_h5ext.py
--rw-rw-rw-   0        0        0    20791 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_jsonld.py
--rw-rw-rw-   0        0        0     1930 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_lazy.py
--rw-rw-rw-   0        0        0     1629 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_namespaces.py
--rw-rw-rw-   0        0        0    18383 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_rdf.py
--rw-rw-rw-   0        0        0     1360 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.3.0a1/tests/wrapper/test_xr2df.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:54.315092 h5rdmtoolbox-1.3.1/
+-rw-rw-rw-   0        0        0     1090 2024-04-22 14:41:40.000000 h5rdmtoolbox-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0    14960 2024-05-16 14:09:54.314099 h5rdmtoolbox-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9509 2024-05-06 09:42:07.000000 h5rdmtoolbox-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:50.518032 h5rdmtoolbox-1.3.1/h5rdmtoolbox/
+-rw-rw-rw-   0        0        0     9533 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/__init__.py
+-rw-rw-rw-   0        0        0     3913 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/_cfg.py
+-rw-rw-rw-   0        0        0    26542 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/_repr.py
+-rw-rw-rw-   0        0        0     5257 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/_user.py
+-rw-rw-rw-   0        0        0      232 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/_version.py
+-rw-rw-rw-   0        0        0     1621 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/cli.py
+-rw-rw-rw-   0        0        0       94 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/consts.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:51.029975 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/
+-rw-rw-rw-   0        0        0     1402 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/__init__.py
+-rw-rw-rw-   0        0        0       56 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/cfg.py
+-rw-rw-rw-   0        0        0      775 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/consts.py
+-rw-rw-rw-   0        0        0    31958 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/core.py
+-rw-rw-rw-   0        0        0      988 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/definition.py
+-rw-rw-rw-   0        0        0     1026 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/errors.py
+-rw-rw-rw-   0        0        0    17349 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/generate.py
+-rw-rw-rw-   0        0        0     2724 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/hdf_ontology.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:51.149728 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/ontology/
+-rw-rw-rw-   0        0        0      150 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/ontology/__init__.py
+-rw-rw-rw-   0        0        0     1308 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/ontology/h5namespace.py
+-rw-rw-rw-   0        0        0     1445 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/ontology/h5ontocls.py
+-rw-rw-rw-   0        0        0      417 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/references.py
+-rw-rw-rw-   0        0        0    17167 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_attributes.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:51.522753 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/
+-rw-rw-rw-   0        0        0     2125 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/__init__.py
+-rw-rw-rw-   0        0        0     4726 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/accessor.py
+-rw-rw-rw-   0        0        0    13103 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/affixes.py
+-rw-rw-rw-   0        0        0       51 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/cache.py
+-rw-rw-rw-   0        0        0      469 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/consts.py
+-rw-rw-rw-   0        0        0     6660 2024-05-03 12:35:23.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/h5interface.py
+-rw-rw-rw-   0        0        0     4808 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/name.py
+-rw-rw-rw-   0        0        0    35542 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/table.py
+-rw-rw-rw-   0        0        0    10035 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/transformation.py
+-rw-rw-rw-   0        0        0     2354 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/utils.py
+-rw-rw-rw-   0        0        0     8695 2024-05-07 06:38:07.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/toolbox_validators.py
+-rw-rw-rw-   0        0        0     7428 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/utils.py
+-rw-rw-rw-   0        0        0      146 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/warnings.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:51.761536 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/
+-rw-rw-rw-   0        0        0     1084 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/def_icon.png
+-rw-rw-rw-   0        0        0     1070 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/fluid-v1.yml
+-rw-rw-rw-   0        0        0      717 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/h5tbx.yaml
+-rw-rw-rw-   0        0        0     2587 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/id_icon.png
+-rw-rw-rw-   0        0        0     3340 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/iri_icon.png
+-rw-rw-rw-   0        0        0     1064 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/piv-v1.yml
+-rw-rw-rw-   0        0        0     3651 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/style.css
+-rw-rw-rw-   0        0        0     2532 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/tutorial_convention.yaml
+-rw-rw-rw-   0        0        0     2558 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/tutorial_standard_name_table.yaml
+-rw-rw-rw-   0        0        0     3287 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/type_icon.png
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:51.866491 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/
+-rw-rw-rw-   0        0        0     3170 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:52.023052 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/
+-rw-rw-rw-   0        0        0      107 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/__init__.py
+-rw-rw-rw-   0        0        0     4727 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/filedb.py
+-rw-rw-rw-   0        0        0    21521 2024-05-15 08:07:59.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/objdb.py
+-rw-rw-rw-   0        0        0     2851 2024-05-16 14:08:31.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/query.py
+-rw-rw-rw-   0        0        0     1933 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/utils.py
+-rw-rw-rw-   0        0        0     2156 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/interface.py
+-rw-rw-rw-   0        0        0    14802 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/mongo.py
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/dev.py
+-rw-rw-rw-   0        0        0      123 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:52.183054 h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/
+-rw-rw-rw-   0        0        0        0 2023-03-27 13:37:37.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/__init__.py
+-rw-rw-rw-   0        0        0     2507 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/magnitude.py
+-rw-rw-rw-   0        0        0     4043 2024-05-03 12:35:23.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/normalize.py
+-rw-rw-rw-   0        0        0     1903 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/units.py
+-rw-rw-rw-   0        0        0     5269 2024-05-03 12:35:23.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/vector.py
+-rw-rw-rw-   0        0        0     8675 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/identifiers.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:52.239926 h5rdmtoolbox-1.3.1/h5rdmtoolbox/layout/
+-rw-rw-rw-   0        0        0       50 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/layout/__init__.py
+-rw-rw-rw-   0        0        0    25624 2024-05-16 14:08:31.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/layout/core.py
+-rw-rw-rw-   0        0        0     6546 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/plotting.py
+-rw-rw-rw-   0        0        0      290 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/protected_attributes.py
+-rw-rw-rw-   0        0        0     5449 2024-05-16 14:08:31.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/protocols.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:52.306618 h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/
+-rw-rw-rw-   0        0        0      337 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/__init__.py
+-rw-rw-rw-   0        0        0     2039 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/interface.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:52.473842 h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/
+-rw-rw-rw-   0        0        0      222 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/__init__.py
+-rw-rw-rw-   0        0        0    16277 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/core.py
+-rw-rw-rw-   0        0        0     7647 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/metadata.py
+-rw-rw-rw-   0        0        0     3533 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/tokens.py
+-rw-rw-rw-   0        0        0      610 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/utils.py
+-rw-rw-rw-   0        0        0    15780 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/tutorial.py
+-rw-rw-rw-   0        0        0    21187 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/utils.py
+-rw-rw-rw-   0        0        0      101 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/warnings.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:52.877817 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/
+-rw-rw-rw-   0        0        0       99 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/__init__.py
+-rw-rw-rw-   0        0        0     3106 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/accessor.py
+-rw-rw-rw-   0        0        0   101086 2024-05-16 14:08:31.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/core.py
+-rw-rw-rw-   0        0        0     4027 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/ds_decoder.py
+-rw-rw-rw-   0        0        0    18233 2024-05-07 06:38:07.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/h5attr.py
+-rw-rw-rw-   0        0        0      465 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/h5ext.py
+-rw-rw-rw-   0        0        0      899 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/h5utils.py
+-rw-rw-rw-   0        0        0     3908 2024-05-16 14:08:31.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/h5yaml.py
+-rw-rw-rw-   0        0        0    42312 2024-05-03 12:35:23.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/jsonld.py
+-rw-rw-rw-   0        0        0     6518 2024-05-06 09:42:07.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/lazy.py
+-rw-rw-rw-   0        0        0    17384 2024-05-03 12:35:23.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/rdf.py
+-rw-rw-rw-   0        0        0     4753 2024-05-03 12:35:23.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/xr2hdf.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:54.301391 h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/
+-rw-rw-rw-   0        0        0    14960 2024-05-16 14:09:49.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4872 2024-05-16 14:09:49.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:09:49.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-16 14:09:49.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      976 2024-05-16 14:09:49.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-16 14:09:49.000000 h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-03-08 18:17:38.000000 h5rdmtoolbox-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0     2269 2024-05-16 14:09:54.347214 h5rdmtoolbox-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-09-27 08:03:12.000000 h5rdmtoolbox-1.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:53.237511 h5rdmtoolbox-1.3.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.1/tests/__init__.py
+-rw-rw-rw-   0        0        0     1013 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/clean_zenodo_sandbox.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:53.510424 h5rdmtoolbox-1.3.1/tests/conventions/
+-rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.1/tests/conventions/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:53.605111 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/
+-rw-rw-rw-   0        0        0        0 2023-09-02 07:03:47.000000 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:53.777782 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/
+-rw-rw-rw-   0        0        0        0 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/__init__.py
+-rw-rw-rw-   0        0        0     6464 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/test_interface.py
+-rw-rw-rw-   0        0        0     6827 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/test_provenance.py
+-rw-rw-rw-   0        0        0    13348 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/test_snt.py
+-rw-rw-rw-   0        0        0    13236 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/test_transformations_and_affixes.py
+-rw-rw-rw-   0        0        0     2503 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/test_standard_attributes.py
+-rw-rw-rw-   0        0        0    13045 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/test_standard_names.py
+-rw-rw-rw-   0        0        0    30934 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/conventions/test_conventions.py
+-rw-rw-rw-   0        0        0     2051 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/conventions/test_engmeta.py
+-rw-rw-rw-   0        0        0     8450 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/conventions/test_ontology.py
+-rw-rw-rw-   0        0        0      548 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/tests/conventions/test_references.py
+-rw-rw-rw-   0        0        0     5094 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/conventions/test_toolbox_validators.py
+-rw-rw-rw-   0        0        0     5060 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/tests/conventions/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:53.887607 h5rdmtoolbox-1.3.1/tests/database/
+-rw-rw-rw-   0        0        0        0 2023-12-12 15:09:30.000000 h5rdmtoolbox-1.3.1/tests/database/__init__.py
+-rw-rw-rw-   0        0        0     1252 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/database/test_find_rdf.py
+-rw-rw-rw-   0        0        0    28194 2024-05-16 14:08:31.000000 h5rdmtoolbox-1.3.1/tests/database/test_hdfDB.py
+-rw-rw-rw-   0        0        0     9625 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/database/test_mongo.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:53.962067 h5rdmtoolbox-1.3.1/tests/layouts/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/tests/layouts/__init__.py
+-rw-rw-rw-   0        0        0    15529 2024-05-16 14:08:31.000000 h5rdmtoolbox-1.3.1/tests/layouts/test_core.py
+-rw-rw-rw-   0        0        0     2282 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/layouts/test_docs.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:54.001045 h5rdmtoolbox-1.3.1/tests/repository/
+-rw-rw-rw-   0        0        0        0 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/tests/repository/__init__.py
+-rw-rw-rw-   0        0        0    18963 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/repository/test_zenodo.py
+-rw-rw-rw-   0        0        0     2679 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.1/tests/test_config.py
+-rw-rw-rw-   0        0        0     6487 2024-05-03 12:35:23.000000 h5rdmtoolbox-1.3.1/tests/test_extensions.py
+-rw-rw-rw-   0        0        0     4243 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/test_identifiers.py
+-rw-rw-rw-   0        0        0     6930 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/tests/test_plotting.py
+-rw-rw-rw-   0        0        0     5035 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/test_repr.py
+-rw-rw-rw-   0        0        0     4079 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/test_user.py
+-rw-rw-rw-   0        0        0     4604 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/test_utils.py
+-rw-rw-rw-   0        0        0      798 2024-04-29 16:01:13.000000 h5rdmtoolbox-1.3.1/tests/test_version.py
+-rw-rw-rw-   0        0        0     1169 2024-04-22 14:41:41.000000 h5rdmtoolbox-1.3.1/tests/test_xarray_export.py
+drwxrwxrwx   0        0        0        0 2024-05-16 14:09:54.298396 h5rdmtoolbox-1.3.1/tests/wrapper/
+-rw-rw-rw-   0        0        0        0 2023-03-09 20:20:48.000000 h5rdmtoolbox-1.3.1/tests/wrapper/__init__.py
+-rw-rw-rw-   0        0        0    46136 2024-05-07 06:38:07.000000 h5rdmtoolbox-1.3.1/tests/wrapper/test_core.py
+-rw-rw-rw-   0        0        0     2020 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/wrapper/test_dump.py
+-rw-rw-rw-   0        0        0    16978 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/wrapper/test_file.py
+-rw-rw-rw-   0        0        0      829 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.3.1/tests/wrapper/test_h5ext.py
+-rw-rw-rw-   0        0        0    21003 2024-05-03 12:35:23.000000 h5rdmtoolbox-1.3.1/tests/wrapper/test_jsonld.py
+-rw-rw-rw-   0        0        0     2395 2024-05-06 09:42:07.000000 h5rdmtoolbox-1.3.1/tests/wrapper/test_lazy.py
+-rw-rw-rw-   0        0        0     1629 2024-05-01 19:48:03.000000 h5rdmtoolbox-1.3.1/tests/wrapper/test_namespaces.py
+-rw-rw-rw-   0        0        0    19077 2024-05-07 06:38:07.000000 h5rdmtoolbox-1.3.1/tests/wrapper/test_rdf.py
+-rw-rw-rw-   0        0        0     1360 2023-12-13 11:01:54.000000 h5rdmtoolbox-1.3.1/tests/wrapper/test_xr2df.py
```

### Comparing `h5rdmtoolbox-1.3.0a1/LICENSE` & `h5rdmtoolbox-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/PKG-INFO` & `h5rdmtoolbox-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5rdmtoolbox
-Version: 1.3.0a1
+Version: 1.3.1
 Summary: Supporting a FAIR Research Data lifecycle using Python and HDF5.
 Home-page: https://h5rdmtoolbox.readthedocs.io/en/latest/
 Author: Matthias Probst
 Author-email: matthias.probst@kit.edu
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -148,57 +148,60 @@
 
 ## Highlights
 
 - Combining HDF5 and [xarray](https://docs.xarray.dev/en/stable/) to allow easy access to metadata and data during
   analysis and processing (
   see [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/quickoverview.html#datasets-xarray-interface)).
 - Assigning [metadata with "globally unique and persistent identifiers"]() as required
-  by [F1 of the FAIR principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/)
-  . This "remove[s] ambiguity in the meaning of your published data...".
+  by [F1 of the FAIR principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/).
+  This can be achieved by using [RDF triples](https://www.w3.org/RDF/), which removes "ambiguity in the meaning of your
+  published data".
 - Define standard attributes through
   [conventions](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/convention/index.html) and enforce users to use
-  them
+  certain attributes in their HDF5 files, such as units and a description, for example.
 - Upload HDF5 files directly
   to [repositories](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/repository/index.html)
   like [Zenodo](https://zenodo.org/)
   or [use them with noSQL databases](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/database/index.html) like
   [mongoDB](https://www.mongodb.com/).
 
 ## Who is the package for?
 
 For everybody, who is...
 
-- ... looking for a management approach for his or her data
-- ... community has not yet established a stable convention
-- ... working with small and big data, that fits into HDF5 files
-- ... looking for an easy way to work with HDF5, especially through Jupyter Notebooks
-- ... looking to integrate HDF5 with repositories and databases
-- ... looking for a way to do all the above whiles not needing to learn a new syntax
-- ... new to HDF5 and wants to learn about it, especially with respect to the FAIR principles and data management
+- ... looking for a management approach for his or her data.
+- ... community has not yet established a stable convention.
+- ... working with small and big data, that fits into HDF5 files.
+- ... looking for an easy way to work with HDF5, especially through Jupyter Notebooks.
+- ... trying to integrate HDF5 with repositories and databases.
+- ... wishing to enrich data semantically with the RDF standard.
+- ... looking for a way to do all the above whiles not needing to learn a new syntax.
+- ... new to HDF5 and wants to learn about it, especially with respect to the FAIR principles and data management.
 
 ## Who is it not for?
 
 For everybody, who ...
 
 - ... is looking for a management approach which at the same time allows high-performance and/or parallel work with HDF5
-- ... has established conventions and managements approaches in his or her community
+- ... has already well-established conventions and managements approaches in his or her community
 
 ## Package Architecture/structure
 
 The toolbox implements five modules, which are shown below. The numbers reference to their main usage in the stages in
 the data lifecycle above. Except the wrapper module, which uses the convention module, all other modules are independent
 of each other.
 
 <a href="https://h5rdmtoolbox.readthedocs.io/en/latest/"><img src="docs/_static/h5tbx_modules.svg" alt="H5TBX modules" style="widht:600px;"></a>
 
 Current implementation highlights in the modules:
 
 - The **wrapper** module adds functionality on top of the `h5py` package. It allows to include so-called standard names,
-  which are defined in conventions. And it implements an interface with the package `xarray`, which allows to carry
-  metadata from HDF5 to the user.
+  which are defined in conventions. And it implements interfaces, such as to the package `xarray`, which allows to carry
+  metadata from HDF5 to the user. Other high-level interfaces like `.rdf` allows assigning semantic information to the
+  HDF5 file.
 - For the **database** module, `hdfDB` and `mongoDB` are implemented. The `hdfDB` module allows to use HDF5 files as a
   database. The `mongoDB` module allows to use mongoDB as a database by mapping the metadata of HDF5 files to the
   database.
 - For the **repository** module, a Zenodo interface is implemented. Zenodo is a repository, which allows to upload and
   download data with a persistent identifier.
 - For the **convention** module,
   the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
@@ -262,22 +265,22 @@
 - `h5py=3.7.0`: HDF5 file interface
 - `xarray>=2022.3.0`: Working with scientific arrays in combination with attributes. Allows carrying metadata from HDF5
   to user
 - `pint>=0.19.2`: Allows working with units
 - `pint_xarray>=0.2.1`: Working with units for usage with xarray
 - `python-forge==18.6.0`: Used to update function signatures when using
   the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
-- `pydantic`: Used to validate [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
+- `pydantic`: Used to
+  validate [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
 - `pyyaml>6.0.0`: Reading and writing of yaml files, e.g. metadata definitions (conventions). Note, lower versions
   collide with python 3.11
 - `requests`: Used to download files from the internet or validate URLs, e.g. metadata definitions (conventions)
 - `rdflib`: Used to enable working with RDF
 - `ontolutils`: Required to work with RDF and derive semantic description of HDF5 file content
 
-
 #### Optional dependencies
 
 To run unit tests or to enable certain features, additional dependencies must be installed.
 
 Install optional dependencies by specifying them in square brackets after the package name, e.g.:
 
     pip install h5RDMtoolbox[mongodb]
@@ -293,15 +296,14 @@
 [snt]
 
 - `xmltodict`: Reading of xml files
 - `tabulate>=0.8.10`: Pretty printing of tables
 - `python-gitlab`: Access to gitlab repositories
 - `pypandoc>=2.3`: Conversion of markdown files to html
 
-
 ## Citing the package
 
 If you intend to use the package in your work, you may cite the paper in the
 journal [inggrid](https://preprints.inggrid.org/repository/view/23/)
 
 Here's the bibtext to it:
```

### Comparing `h5rdmtoolbox-1.3.0a1/README.md` & `h5rdmtoolbox-1.3.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,57 +16,60 @@
 
 ## Highlights
 
 - Combining HDF5 and [xarray](https://docs.xarray.dev/en/stable/) to allow easy access to metadata and data during
   analysis and processing (
   see [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/quickoverview.html#datasets-xarray-interface)).
 - Assigning [metadata with "globally unique and persistent identifiers"]() as required
-  by [F1 of the FAIR principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/)
-  . This "remove[s] ambiguity in the meaning of your published data...".
+  by [F1 of the FAIR principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/).
+  This can be achieved by using [RDF triples](https://www.w3.org/RDF/), which removes "ambiguity in the meaning of your
+  published data".
 - Define standard attributes through
   [conventions](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/convention/index.html) and enforce users to use
-  them
+  certain attributes in their HDF5 files, such as units and a description, for example.
 - Upload HDF5 files directly
   to [repositories](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/repository/index.html)
   like [Zenodo](https://zenodo.org/)
   or [use them with noSQL databases](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/database/index.html) like
   [mongoDB](https://www.mongodb.com/).
 
 ## Who is the package for?
 
 For everybody, who is...
 
-- ... looking for a management approach for his or her data
-- ... community has not yet established a stable convention
-- ... working with small and big data, that fits into HDF5 files
-- ... looking for an easy way to work with HDF5, especially through Jupyter Notebooks
-- ... looking to integrate HDF5 with repositories and databases
-- ... looking for a way to do all the above whiles not needing to learn a new syntax
-- ... new to HDF5 and wants to learn about it, especially with respect to the FAIR principles and data management
+- ... looking for a management approach for his or her data.
+- ... community has not yet established a stable convention.
+- ... working with small and big data, that fits into HDF5 files.
+- ... looking for an easy way to work with HDF5, especially through Jupyter Notebooks.
+- ... trying to integrate HDF5 with repositories and databases.
+- ... wishing to enrich data semantically with the RDF standard.
+- ... looking for a way to do all the above whiles not needing to learn a new syntax.
+- ... new to HDF5 and wants to learn about it, especially with respect to the FAIR principles and data management.
 
 ## Who is it not for?
 
 For everybody, who ...
 
 - ... is looking for a management approach which at the same time allows high-performance and/or parallel work with HDF5
-- ... has established conventions and managements approaches in his or her community
+- ... has already well-established conventions and managements approaches in his or her community
 
 ## Package Architecture/structure
 
 The toolbox implements five modules, which are shown below. The numbers reference to their main usage in the stages in
 the data lifecycle above. Except the wrapper module, which uses the convention module, all other modules are independent
 of each other.
 
 <a href="https://h5rdmtoolbox.readthedocs.io/en/latest/"><img src="docs/_static/h5tbx_modules.svg" alt="H5TBX modules" style="widht:600px;"></a>
 
 Current implementation highlights in the modules:
 
 - The **wrapper** module adds functionality on top of the `h5py` package. It allows to include so-called standard names,
-  which are defined in conventions. And it implements an interface with the package `xarray`, which allows to carry
-  metadata from HDF5 to the user.
+  which are defined in conventions. And it implements interfaces, such as to the package `xarray`, which allows to carry
+  metadata from HDF5 to the user. Other high-level interfaces like `.rdf` allows assigning semantic information to the
+  HDF5 file.
 - For the **database** module, `hdfDB` and `mongoDB` are implemented. The `hdfDB` module allows to use HDF5 files as a
   database. The `mongoDB` module allows to use mongoDB as a database by mapping the metadata of HDF5 files to the
   database.
 - For the **repository** module, a Zenodo interface is implemented. Zenodo is a repository, which allows to upload and
   download data with a persistent identifier.
 - For the **convention** module,
   the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
@@ -130,22 +133,22 @@
 - `h5py=3.7.0`: HDF5 file interface
 - `xarray>=2022.3.0`: Working with scientific arrays in combination with attributes. Allows carrying metadata from HDF5
   to user
 - `pint>=0.19.2`: Allows working with units
 - `pint_xarray>=0.2.1`: Working with units for usage with xarray
 - `python-forge==18.6.0`: Used to update function signatures when using
   the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
-- `pydantic`: Used to validate [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
+- `pydantic`: Used to
+  validate [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
 - `pyyaml>6.0.0`: Reading and writing of yaml files, e.g. metadata definitions (conventions). Note, lower versions
   collide with python 3.11
 - `requests`: Used to download files from the internet or validate URLs, e.g. metadata definitions (conventions)
 - `rdflib`: Used to enable working with RDF
 - `ontolutils`: Required to work with RDF and derive semantic description of HDF5 file content
 
-
 #### Optional dependencies
 
 To run unit tests or to enable certain features, additional dependencies must be installed.
 
 Install optional dependencies by specifying them in square brackets after the package name, e.g.:
 
     pip install h5RDMtoolbox[mongodb]
@@ -161,15 +164,14 @@
 [snt]
 
 - `xmltodict`: Reading of xml files
 - `tabulate>=0.8.10`: Pretty printing of tables
 - `python-gitlab`: Access to gitlab repositories
 - `pypandoc>=2.3`: Conversion of markdown files to html
 
-
 ## Citing the package
 
 If you intend to use the package in your work, you may cite the paper in the
 journal [inggrid](https://preprints.inggrid.org/repository/view/23/)
 
 Here's the bibtext to it:
```

#### html2text {}

```diff
@@ -15,51 +15,54 @@
 detailed information of try the [quickstart using colab](#quickstart). ##
 Highlights - Combining HDF5 and [xarray](https://docs.xarray.dev/en/stable/) to
 allow easy access to metadata and data during analysis and processing ( see
 [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/
 quickoverview.html#datasets-xarray-interface)). - Assigning [metadata with
 "globally unique and persistent identifiers"]() as required by [F1 of the FAIR
 principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-
-globally-unique-persistent-identifiers/) . This "remove[s] ambiguity in the
-meaning of your published data...". - Define standard attributes through
-[conventions](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/
-convention/index.html) and enforce users to use them - Upload HDF5 files
-directly to [repositories](https://h5rdmtoolbox.readthedocs.io/en/latest/
-userguide/repository/index.html) like [Zenodo](https://zenodo.org/) or [use
-them with noSQL databases](https://h5rdmtoolbox.readthedocs.io/en/latest/
-userguide/database/index.html) like [mongoDB](https://www.mongodb.com/). ## Who
-is the package for? For everybody, who is... - ... looking for a management
-approach for his or her data - ... community has not yet established a stable
-convention - ... working with small and big data, that fits into HDF5 files -
-... looking for an easy way to work with HDF5, especially through Jupyter
-Notebooks - ... looking to integrate HDF5 with repositories and databases - ...
-looking for a way to do all the above whiles not needing to learn a new syntax
-- ... new to HDF5 and wants to learn about it, especially with respect to the
-FAIR principles and data management ## Who is it not for? For everybody, who
-... - ... is looking for a management approach which at the same time allows
-high-performance and/or parallel work with HDF5 - ... has established
-conventions and managements approaches in his or her community ## Package
-Architecture/structure The toolbox implements five modules, which are shown
-below. The numbers reference to their main usage in the stages in the data
-lifecycle above. Except the wrapper module, which uses the convention module,
-all other modules are independent of each other. _[_H_5_T_B_X_ _m_o_d_u_l_e_s_]Current
-implementation highlights in the modules: - The **wrapper** module adds
-functionality on top of the `h5py` package. It allows to include so-called
-standard names, which are defined in conventions. And it implements an
-interface with the package `xarray`, which allows to carry metadata from HDF5
-to the user. - For the **database** module, `hdfDB` and `mongoDB` are
-implemented. The `hdfDB` module allows to use HDF5 files as a database. The
-`mongoDB` module allows to use mongoDB as a database by mapping the metadata of
-HDF5 files to the database. - For the **repository** module, a Zenodo interface
-is implemented. Zenodo is a repository, which allows to upload and download
-data with a persistent identifier. - For the **convention** module, the
-[standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/
-conventions/standard_attributes_and_conventions.html) are implemented. - The
-**layout** module allows to define expectations on the internal layout (object
-names, location, attributes, properties) of HDF5 files. ## Quickstart A
+globally-unique-persistent-identifiers/). This can be achieved by using [RDF
+triples](https://www.w3.org/RDF/), which removes "ambiguity in the meaning of
+your published data". - Define standard attributes through [conventions](https:
+//h5rdmtoolbox.readthedocs.io/en/latest/userguide/convention/index.html) and
+enforce users to use certain attributes in their HDF5 files, such as units and
+a description, for example. - Upload HDF5 files directly to [repositories]
+(https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/repository/index.html)
+like [Zenodo](https://zenodo.org/) or [use them with noSQL databases](https://
+h5rdmtoolbox.readthedocs.io/en/latest/userguide/database/index.html) like
+[mongoDB](https://www.mongodb.com/). ## Who is the package for? For everybody,
+who is... - ... looking for a management approach for his or her data. - ...
+community has not yet established a stable convention. - ... working with small
+and big data, that fits into HDF5 files. - ... looking for an easy way to work
+with HDF5, especially through Jupyter Notebooks. - ... trying to integrate HDF5
+with repositories and databases. - ... wishing to enrich data semantically with
+the RDF standard. - ... looking for a way to do all the above whiles not
+needing to learn a new syntax. - ... new to HDF5 and wants to learn about it,
+especially with respect to the FAIR principles and data management. ## Who is
+it not for? For everybody, who ... - ... is looking for a management approach
+which at the same time allows high-performance and/or parallel work with HDF5 -
+... has already well-established conventions and managements approaches in his
+or her community ## Package Architecture/structure The toolbox implements five
+modules, which are shown below. The numbers reference to their main usage in
+the stages in the data lifecycle above. Except the wrapper module, which uses
+the convention module, all other modules are independent of each other. _[_H_5_T_B_X
+_m_o_d_u_l_e_s_]Current implementation highlights in the modules: - The **wrapper**
+module adds functionality on top of the `h5py` package. It allows to include
+so-called standard names, which are defined in conventions. And it implements
+interfaces, such as to the package `xarray`, which allows to carry metadata
+from HDF5 to the user. Other high-level interfaces like `.rdf` allows assigning
+semantic information to the HDF5 file. - For the **database** module, `hdfDB`
+and `mongoDB` are implemented. The `hdfDB` module allows to use HDF5 files as a
+database. The `mongoDB` module allows to use mongoDB as a database by mapping
+the metadata of HDF5 files to the database. - For the **repository** module, a
+Zenodo interface is implemented. Zenodo is a repository, which allows to upload
+and download data with a persistent identifier. - For the **convention**
+module, the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/
+latest/conventions/standard_attributes_and_conventions.html) are implemented. -
+The **layout** module allows to define expectations on the internal layout
+(object names, location, attributes, properties) of HDF5 files. ## Quickstart A
 quickstart notebook can be tested by clicking on the following badge: [![Open
 Quickstart Notebook](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/github/matthiasprobst/h5RDMtoolbox/blob/
 colab/docs/colab/quickstart.ipynb) ## Documentation Please find a comprehensive
 documentation with many examples [here](https://h5rdmtoolbox.readthedocs.io/en/
 latest/) or by click on the image, which shows the research data lifecycle in
 the center and the respective toolbox features on the outside: A paper is
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/__init__.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_cfg.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/_cfg.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_repr.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/_repr.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/_user.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/_user.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/cli.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/cli.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/__init__.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/__init__.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/consts.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/consts.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/core.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/core.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/definition.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/definition.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/errors.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/errors.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/generate.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/generate.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/hdf_ontology.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/hdf_ontology.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/h5namespace.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/ontology/h5namespace.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/ontology/h5ontocls.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/ontology/h5ontocls.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_attributes.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_attributes.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/__init__.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/__init__.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/accessor.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/accessor.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/affixes.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/affixes.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/h5interface.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/h5interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
     def get_xrdataset(self, create_coords_if_missing: bool = False) -> xr.Dataset:
         """Return a dataset with the components of the tensor as variables"""
         ds = xr.Dataset({n: self[c][()] for n, c in zip(self.component_names, self.components)})
         if not create_coords_if_missing:
             return ds
 
-        if all(len(c.coords()) == 0 for c in self.components.values()):
+        if all(len(c.coords) == 0 for c in self.components.values()):
             for i in range(len(self.components)):
                 ds = ds.assign_coords({f'dim_{i}': range(self.components[self.component_names[i]].shape[i])})
         return ds
 
 
 class HDF5StandardNameInterface:
     """High level interface to HDF5 files following convention which use
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/name.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/name.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/table.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/table.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/transformation.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/transformation.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/standard_names/utils.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/standard_names/utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/toolbox_validators.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/toolbox_validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """general validation functions of the toolbox usable by convention. If users wish to user
 their own validators, they need to define them separately. The respective python script then
 must be provided during initialization of a Convention"""
+import re
+from typing import Union, Dict
 
 import pint
-import re
 import typing_extensions
 from pydantic.functional_validators import WrapValidator
-from typing import Union, Dict
 from typing_extensions import Annotated
 
 from h5rdmtoolbox import get_ureg, errors
 from h5rdmtoolbox import identifiers
 
 
 def __verify_version(version, handler, info) -> str:
@@ -66,15 +66,15 @@
         if units is None:
             raise KeyError('No units defined for this variable!')
 
         # check if scale is provided:
         data_scale = parent.attrs.get('DATA_SCALE', None)
         if data_scale is not None:
             # scale_ds = parent.rootparent[data_scale]
-            ds_scale_units = data_scale.attrs.raw.get('units', '')
+            ds_scale_units = parent.rootparent[data_scale].attrs.get('units', '')
             ureg = get_ureg()
             units = str(ureg.Unit(ds_scale_units) * units)
 
         sn = snt[value]
         if sn.is_vector():
             raise errors.StandardAttributeError(f'Standard name {value} is a vector and cannot be used as '
                                                 'attribute. Use a transformation e.g. with a component or magnitude '
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/convention/utils.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/convention/utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/def_icon.png` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/def_icon.png`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/fluid-v1.yml` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/fluid-v1.yml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/h5tbx.yaml` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/h5tbx.yaml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/id_icon.png` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/id_icon.png`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/iri_icon.png` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/iri_icon.png`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/piv-v1.yml` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/piv-v1.yml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/style.css` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/style.css`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/tutorial_convention.yaml` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/tutorial_convention.yaml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/tutorial_standard_name_table.yaml` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/tutorial_standard_name_table.yaml`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/data/type_icon.png` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/data/type_icon.png`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/__init__.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/__init__.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/filedb.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/filedb.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/objdb.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/objdb.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/query.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """query module"""
 import logging
+import numpy as np
 import re
 import warnings
 
-import numpy as np
-
 logger = logging.getLogger('h5rdmtoolbox')
 
 
 def _eq(a, b):
     """Check if a == b"""
     if a is None or b is None:
         return False
@@ -40,14 +39,21 @@
     """Check if a < b"""
     logger.debug(f'checking if a < b ({a} < {b})')
     if a is None or b is None:
         return False
     return a < b
 
 
+def _in(a, b) -> bool:
+    """Check if a is in b"""
+    if a is None or b is None:
+        return False
+    return a in b
+
+
 def _lte(a, b):
     """Check if a <= b"""
     if a is None or b is None:
         return False
     return a <= b
 
 
@@ -93,14 +99,15 @@
 
 operator = {'$regex': _regex,
             '$basename': _basename,
             '$eq': _eq,
             '$gt': _gt,
             '$gte': _gte,
             '$lt': _lt,
+            '$in': _in,
             '$lte': _lte,
             '$exists': _exists,
             '$userdefined': _userdefined}
 value_operator = {'$eq': _arreq, '$gt': _gt, '$gte': _gte, '$lt': _lt, '$lte': _lte}
 
 
 def _pass(obj, comparison_value):
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/hdfdb/utils.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/hdfdb/utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/interface.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/interface.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/database/mongo.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/database/mongo.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/magnitude.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/magnitude.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/normalize.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/normalize.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class NormalizationInterface:
 
     def __init__(self,
                  dataset: H5TbxDataset,
                  norm_data: Dict[str, Union[float, str]],
                  name: bool = False):
         self.dataset = dataset
-        self._coord_names = list(dataset.coords())
+        self._coord_names = list(dataset.coords)
         self.norm_data: Dict = norm_data
         self.cnorm_data: Dict = {}
         self.cnorm_name: Dict = {}
         self.name = name
 
     def __getattr__(self, item: str):
         if item in self._coord_names:
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/units.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/units.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/extensions/vector.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/extensions/vector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 # noinspection PyUnresolvedReferences
+from typing import Dict, Optional
+
 import h5py
 import xarray as xr
-from typing import Dict, Optional
 
 from h5rdmtoolbox.protocols import H5TbxDataset
 from h5rdmtoolbox.wrapper.accessor import Accessor, register_accessor
 
 
 class VectorInterface:
     def __init__(self,
                  datasets: Dict[str, H5TbxDataset],
                  name: Optional[str] = None,
-                 combine_attrs: str = "override"):
+                 **xr_merge_kwargs):
         self.datasets = datasets
         self.name = name
-        self.combine_attrs = combine_attrs
+        self.xr_merge_kwargs = xr_merge_kwargs
 
     def __getitem__(self, item) -> xr.Dataset:
         return xr.merge(
             [da.__getitem__(item).rename(k) for k, da in self.datasets.items()],
-            combine_attrs=self.combine_attrs)
+            **self.xr_merge_kwargs)
+
+    def isel(self, **indexers) -> xr.Dataset:
+        return xr.merge(
+            [da.isel(**indexers).rename(k) for k, da in self.datasets.items()],
+            **self.xr_merge_kwargs)
+
+    def sel(self, method: str = None, **kwargs) -> xr.Dataset:
+        return xr.merge(
+            [da.sel(method=method, **kwargs).rename(k) for k, da in self.datasets.items()],
+            **self.xr_merge_kwargs)
 
 
 @register_accessor("Vector", "Group")
 @register_accessor("Vector", "File")
 class Vector(Accessor):
     def __call__(self,
                  *args,
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/identifiers.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/identifiers.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/layout/core.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/layout/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,18 +105,20 @@
         hdf5 root group.
     """
 
     def __init__(self,
                  func: QueryCallable,
                  kwargs: Dict,
                  n: Union[int, None, Dict],
+                 rebase: bool = False,
                  description: Optional[str] = None,
                  parent: Optional["LayoutSpecification"] = None):
         self.func = func
         self.kwargs = kwargs
+        self.rebase = rebase
 
         self.n, self.number_of_result_comparison = self._parse_n_def(n)
 
         self.id = uuid.uuid4()
         self.specifications: List[LayoutSpecification] = []
         self.alt_specifications: List[LayoutSpecification] = []
         self.parent: Optional["LayoutSpecification"] = parent
@@ -215,18 +217,21 @@
     def __repr__(self):
         _kwargs = _replace_callables_with_names(self.kwargs)
         if self.description:
             return f'{self.__class__.__name__}(description="{self.description}", kwargs={_kwargs})'
         return f'{self.__class__.__name__}(kwargs={_kwargs})'
 
     def __call__(self, target: Union[h5py.Group, h5py.Dataset]):
-        if isinstance(target, h5tbx.database.lazy.LHDFObject):
+        if isinstance(target, h5tbx.wrapper.lazy.LHDFObject):
             with target as _target:
                 return self.__call__(_target)
 
+        if self.rebase and isinstance(target, (h5tbx.Dataset, h5tbx.Group)):
+            target = target.rootparent
+
         self._n_calls += 1
         scr = SpecificationResult(target)
 
         if self.n is None:
             # per definition successful since n is None
             scr.validation_flag = VALIDATION_FLAGS.SUCCESSFUL.value + VALIDATION_FLAGS.OPTIONAL.value
 
@@ -326,14 +331,15 @@
                              f'matching the number of results: {self.n} != {n_res}')
         self.results.append(scr)
 
     def add(self,
             func: QueryCallable,
             *,
             n: Optional[Union[int, None, Dict]] = None,
+            rebase: bool = False,
             description: Optional[str] = None,
             **kwargs):
         """
         Add a specification by providing a callable query obj. Optionally, the
         number of exact matches can be provided as well as the a description string.
         The kwargs are passed to the callable
 
@@ -359,14 +365,15 @@
         >>> spec1 = lay.__set_meta_field__(hdfdb.FileDB.find, flt={'$name': '/u'}, n=1)
         >>> spec2 = lay.__set_meta_field__(...) # add another spec to layout
         >>> spec_sub1 = spec1.__set_meta_field__(...)  # add spec to `spec1` if it succeeds and apply to all results of `spec1`
         """
         new_spec = LayoutSpecification(func=func,
                                        kwargs=kwargs,
                                        n=n,
+                                       rebase=rebase,
                                        description=description,
                                        parent=self)
         for spec in self.specifications:
             if spec == new_spec:
                 warnings.warn(f'Specification "{new_spec}" already exists. Skipping.',
                               UserWarning)
                 return spec
@@ -452,17 +459,18 @@
             failed.append(self)
         if self.specifications:
             failed.extend(spec.get_failed() for spec in self.specifications)
             # flatten list:
             return [item for sublist in failed for item in sublist]
         return failed
 
-    def get_summary(self, exclude_keys: Optional[List] = None) -> List[Dict]:
+    def get_summary(self, exclude_keys: Optional[Union[str, List[str]]] = None) -> List[Dict]:
         """return a summary as dictionary"""
-
+        if isinstance(exclude_keys, str):
+            exclude_keys = [exclude_keys, ]
         data = []
         for res in self.results:
             data.append({'id': self.id,
                          'called': len(self.results) > 0,
                          # 'n_calls/n_res/n_fails': f'{self.n_calls}/{n_res}/{self.n_fails}' if self.called else '-(-)',
                          'flag': res.validation_flag,
                          'flag description': _get_flag_explanations(res.validation_flag),
@@ -472,14 +480,17 @@
                          # '_n_fails': self._n_fails,
                          'func': f'{self.func.__module__}.{self.func.__name__}',
                          'kwargs': self.kwargs,
                          })
 
         if exclude_keys is None:
             exclude_keys = []
+        elif isinstance(exclude_keys, str):
+            exclude_keys = [exclude_keys, ]
+
         for key in exclude_keys:
             # pop keys from dict:
             for i, d in enumerate(data):
                 data[i].pop(key)
 
         for spec in self.specifications:
             data.extend(spec.get_summary(exclude_keys))
@@ -504,27 +515,27 @@
         # flatten list:
         return [item for sublist in valid_specs for item in sublist]
 
     def is_valid(self) -> bool:
         """Return True if the layout is valid, which is the case if no specs failed"""
         return len(self.get_failed()) == 0
 
-    def get_summary(self, exclude_keys: Optional[List] = None,
+    def get_summary(self, exclude_keys: Optional[Union[str, List[str]]] = None,
                     failed_only: bool = False) -> List[Dict]:
         """return a list of dictionaries containing information about a specification call"""
         data = []
         for spec in self.specifications:
             s = spec.get_summary(exclude_keys=exclude_keys)
             if failed_only:
                 data.extend([d for d in s if d['flag'] & 2 == 2])
             else:
                 data.extend(s)
         return data
 
-    def print_summary(self, exclude_keys: Optional[List[str]] = None,
+    def print_summary(self, exclude_keys: Optional[Union[str, List[str]]] = None,
                       failed_only: bool = False):
         """Prints a summary of the specification. Requires the tabulate package."""
         try:
             from tabulate import tabulate
         except ImportError:
             raise ImportError('Please install tabulate to use this method')
         print('\nSummary of layout validation')
@@ -561,19 +572,20 @@
     >>>     hdfdb.FileDB.find,  # query function
     >>>     flt={'$name': '/u'},
     >>>     objfilter='dataset'
     >>> )
     >>> lay.validate('path/to/file.h5')
     """
 
-    def __init__(self):
+    def __init__(self, description: str = ''):
+        self.description = description  # description of the layout class
         self.specifications: List[LayoutSpecification] = []
 
     def __repr__(self):
-        return f'{self.__class__.__name__}'
+        return f'{self.__class__.__name__} (description="{self.description}")'
 
     def __eq__(self, other):
         if not isinstance(other, Layout):
             return False
         return self.specifications == other.specifications
 
     def validate(self, filename_or_root_group: Union[str, pathlib.Path, h5py.Group]) -> LayoutResult:
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/plotting.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/plotting.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/protocols.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/protocols.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,18 @@
 
 class LazyDataset(LazyObject):
     """Lazy Dataset Protocol class"""
 
     def __init__(self, obj: h5py.Dataset):
         ...
 
+    def __getitem__(self, item):
+        """Return the item by the item name or index"""
+        ...
+
     def coords(self):
         """Return the coordinates associated to the Dataset"""
         ...
 
     def isel(self, **indexers: Dict):
         """Return the Dataset indexed by the indexers"""
         ...
@@ -102,14 +106,15 @@
     def __getitem__(self, item: str) -> LazyObject:
         """Return the dataset or group by the item name"""
         ...
 
 
 class H5TbxAttributeManager(Protocol):
     """Protocol for the AttributeManager class."""
+    _parent: Union[h5py.Group, h5py.Dataset]
 
     @property
     def raw(self) -> h5py.AttributeManager:
         ...
 
     def pop(self, key: str, default=None):
         ...
@@ -176,14 +181,15 @@
         of the HDF5 object path."""
 
 
 class H5TbxDataset(H5TbxHLObject):
     """Protocol for the h5tbx.Dataset class."""
     name: str
 
+    @property
     def coords(self):
         ...
 
     @property
     def hdf_filename(self) -> pathlib.Path:
         """Return the filename as a pathlib.Path object."""
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/interface.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/interface.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/core.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/core.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/metadata.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/metadata.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/tokens.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/tokens.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/repository/zenodo/utils.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/repository/zenodo/utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/tutorial.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/tutorial.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/utils.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/accessor.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/accessor.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/core.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 """Core wrapper module containing basic wrapper implementation of File, Dataset and Group
 """
 
-import h5py
 import json
 import logging
-import numpy as np
 import os
 import pathlib
-# noinspection PyUnresolvedReferences
-import pint
 import shutil
 import warnings
-import xarray as xr
 from collections.abc import Iterable
 from datetime import datetime, timezone
-from h5py._hl.base import phil, with_phil
-from h5py._objects import ObjectID
 from pathlib import Path
 from typing import List, Dict, Union, Tuple, Optional
 
+import h5py
+import numpy as np
+# noinspection PyUnresolvedReferences
+import pint
+import xarray as xr
+from h5py._hl.base import phil, with_phil
+from h5py._objects import ObjectID
+
 # noinspection PyUnresolvedReferences
 from . import xr2hdf, rdf
 from .ds_decoder import dataset_value_decoder
 from .h5attr import H5_DIM_ATTRS, pop_hdf_attributes, WrapperAttributeManager
 from .h5utils import _is_not_valid_natural_name, get_rootparent
 from .. import _repr, get_config, convention, utils, consts, protected_attributes
 from .. import get_ureg
@@ -880,15 +881,15 @@
                                 ignore_attribute_error=ignore_attribute_error)
 
     def create_dataset_from_csv(self, csv_filename: Union[str, pathlib.Path], *args, **kwargs):
         """Create datasets from a single csv file. Docstring: See File.create_datasets_from_csv()"""
         return self.create_datasets_from_csv(csv_filenames=[csv_filename, ], *args, **kwargs)
 
     def create_datasets_from_csv(self,
-                                 csv_filenames: Union[str, pathlib.Path, List[str], List[pathlib.Path]],
+                                 csv_filenames: Union[str, pathlib.Path, List[Union[str, pathlib.Path]]],
                                  dimension: Union[int, str] = 0,
                                  shape=None,
                                  overwrite=False,
                                  combine_opt='stack',
                                  axis=0,
                                  chunks=None,
                                  attrs: Dict = None,
@@ -995,14 +996,20 @@
                         f'Could not read {variable_name} from csv file due to: {e}')
 
             # attach scale if dimension is set
             if dimension:
                 for ds, variable_name in zip(datasets, column_names):
                     if variable_name != dimension:
                         ds.dims[0].attach_scale(self[dimension])
+            for ds in datasets:
+                ds.attrs['source_filename'] = csv_filenames
+                if isinstance(csv_filenames, (list, tuple)):
+                    ds.attrs['source_filename_hash_md5'] = [utils.get_checksum(f) for f in csv_filenames]
+                else:
+                    ds.attrs['source_filename_hash_md5'] = utils.get_checksum(csv_filenames)
             return datasets
 
         data = {}
         for name, value in dfs[0].items():
             if shape is None:
                 data[name] = [value.values, ]
             else:
@@ -1011,21 +1018,24 @@
             for name, value in df.items():
                 if shape is None:
                     data[name].append(value.values)
                 else:
                     data[name].append(value.values.reshape(shape))
 
         for name, value in data.items():
-            self.create_dataset(name=str(name),
-                                data=np.stack(value, axis=axis),
-                                attrs=attrs.get(name, None),
-                                overwrite=overwrite,
-                                compression=compression,
-                                compression_opts=compression_opts,
-                                chunks=chunks)
+            ds = self.create_dataset(name=str(name),
+                                     data=np.stack(value, axis=axis),
+                                     attrs=attrs.get(name, None),
+                                     overwrite=overwrite,
+                                     compression=compression,
+                                     compression_opts=compression_opts,
+                                     chunks=chunks)
+
+            ds.attrs['source_filename'] = csv_filenames
+            ds.attrs['source_filename_has_md5'] = [utils.get_checksum(f) for f in csv_filenames]
 
     def create_dataset_from_image(self,
                                   img_data: Union[Iterable, np.ndarray, List[np.ndarray]],
                                   name,
                                   chunks=None,
                                   dtype=None,
                                   axis=0,
@@ -1173,18 +1183,20 @@
             raise ValueError(f'External link {name} was not created. A Dataset with this name'
                              ' already exists and overwrite is set to False! '
                              'You can pass overwrite=True in order to overwrite the '
                              'existing dataset')
         self[name] = h5py.ExternalLink(filename, path)
         return self[name]
 
-    def create_from_yaml(self, yaml_filename: Path):
+    def create_from_yaml(self, yaml_filename: Path, num_dtype:Optional[str]=None):
         """creates groups, datasets and attributes defined in a yaml file.
         Creation is performed relative to the current group level.
 
+        If a num_dtype is provided, all numerical datasets are created with this dtype.
+
         An example YAML file content could look like this:
 
         >>> title: 'Title of the file'
         >>> contact: '0000-1234-1234-1234'
         >>> grp:
         >>>   attrs:
         >>>     comment: test
@@ -1204,15 +1216,15 @@
 
         Examples
         --------
         >>> with h5tbx.File('test.h5', 'w') as h5:
         >>>     h5.create_from_yaml('test.yaml')
         """
         from . import h5yaml
-        h5yaml.H5Yaml(yaml_filename).write(self)
+        h5yaml.H5Yaml(yaml_filename).write(self, num_dtype=num_dtype)
 
     def create_from_dict(self, dictionary: Dict):
         """Create groups and datasets based on a dictionary"""
         from . import h5yaml
         h5yaml.H5Dict(dictionary).write(self)
 
     def create_from_jsonld(self, data: str, context: Optional[Dict] = None):
@@ -1563,25 +1575,60 @@
         if 'DATA_OFFSET' in self.attrs:
             _src = self.attrs['DATA_OFFSET']
             if isinstance(_src, str):
                 return self.rootparent[_src]
             return self.rootparent[self.attrs['DATA_OFFSET'].name]
         return None
 
+    @property
     def coords(self) -> Dict:
         """Return a dictionary of the dimension scales of the dataset.
         Corresponds to the xarray coordinates."""
         coords = {}
         for dim in self.dims:
             if len(dim) > 0:
                 for i, d in enumerate(dim):
                     coords[dim[i].name.rsplit('/')[-1]] = dim[i]
         return coords
         # return {d[0].name.rsplit('/')[-1]: d[0] for d in self.dims if len(d) > 0}
 
+    def assign_coord(self, coord):
+        if isinstance(coord, str):
+            if coord not in self.rootparent:
+                raise ValueError(f'Coordinate {coord} not found in the file!')
+            coord = self.rootparent[coord]
+        curr_coords = self.attrs.get(protected_attributes.COORDINATES, [])
+        curr_coords.append(coord.name)
+        self.attrs[protected_attributes.COORDINATES] = curr_coords
+
+        # if coords is not None:
+        #     if not isinstance(coords, list):
+        #         coords = [coords]
+        #     for c in coords:
+        #         if not isinstance(c, h5py.Dataset):
+        #             raise ValueError('Only h5py.Dataset objects can be assigned as coordinates!')
+        #         coords_kwargs.update({c.name: c})
+        #
+        # for k, v in coords_kwargs.items():
+        #
+        #     if not isinstance(v, h5py.Dataset):
+        #         if not isinstance(v, xr.DataArray):
+        #             raise TypeError(f'Only h5py.Dataset or xarray.DataArray objects can be assigned as coordinates, '
+        #                             f'but got {type(v)}')
+        #         raise TypeError('Only h5py.Dataset objects can be assigned as coordinates!')
+        #
+        #     if v.ndim not in (0, self.ndim):
+        #         raise ValueError(f'Coordinate {k} must have the same dimension as the dataset or be a scalar!')
+        #     elif isinstance(v, xr.DataArray):
+        #         self.parent.create_dataset_from_xarray_dataset(v)
+        #
+        # curr_coords = self.attrs.get(protected_attributes.COORDINATES, {})
+        # curr_coords.update(coords_kwargs)
+        # self.attrs[protected_attributes.COORDINATES] = curr_coords
+
     def isel(self, **indexers) -> xr.DataArray:
         """Index selection by providing the coordinate name.
 
         Parameters
         ----------
         indexers: Dict
             Dictionary with coordinate name as key and slice or index as value
@@ -1594,38 +1641,52 @@
         Exampels
         --------
         >>> with h5tbx.File(filename) as h5:
         >>>     h5.vel.isel(time=0, z=3)
         """
         if len(indexers) == 0:
             return self[()]
-        ds_coords = self.coords()
+        ds_coords = self.coords
         if ds_coords:
             for cname in indexers.keys():
                 if cname not in ds_coords:
                     raise KeyError(f'Coordinate {cname} not in {list(ds_coords.keys())}')
 
             sl = {cname: slice(None) for cname, _ in zip(ds_coords.keys(), range(self.ndim))}
+            sl_key_list = list(sl.keys())
             for (cname, item), _ in zip(indexers.items(), range(self.ndim)):
-                sl[cname] = item
+                # if the indexer name is in the same dimension as one of the already registered
+                # coordinates in "sl", then replace
+                _replaced = False
+                for idim, d in enumerate(self.dims):
+                    for i in range(len(d)):
+                        if d[i].name.rsplit('/')[-1] == cname:
+                            sl[sl_key_list[idim]] = item
+                            _replaced = True
+                            break
+                if not _replaced:
+                    sl[cname] = item
+            # for k in sl.copy().keys():
+            #     if k not in indexers:
+            #         sl.pop(k)
         else:
             # no indexers available. User must provide dim_<i> then!
             if not all([cname.startswith('dim_') for cname in indexers.keys()]):
                 raise KeyError(f'No coordinates available. Provide dim_<i> as key!')
             dim_dict = {f'dim_{i}': slice(None) for i in range(len(self.shape))}
             # indices = [int(cname.split('_')[1]) for cname in indexers.keys()]
             sl = {cname: slice(None) for cname, _ in zip(dim_dict.keys(), range(self.ndim))}
             for (cname, item), _ in zip(indexers.items(), range(self.ndim)):
                 sl[cname] = item
 
         def _make_ascending(_data):
             if isinstance(_data, (np.ndarray, list)):
-                warnings.warn(
-                    'Only ascending order is supported for np.ndarray and list. Reducing the data to unique values'
-                )
+                # warnings.warn(
+                #     'Only ascending order is supported for np.ndarray and list. Reducing the data to unique values'
+                # )
                 unique_data = np.unique(_data)
                 _diff = np.diff(unique_data)
                 if np.all(_diff == 1):
                     # more efficient to use slice
                     return slice(unique_data[0], unique_data[-1] + 1, 1)
                 if np.all(_diff == 2):
                     # more efficient to use slice
@@ -1634,15 +1695,15 @@
             return _data
 
         return self[tuple([_make_ascending(v) for v in sl.values()])]
 
     def sel(self, method=None, **coords):
         """Select data based on coordinates and specific value(s). This is useful if the index
         is not known. Only works for a single dimension and for method 'exact'."""
-        av_coord_datasets = self.coords()
+        av_coord_datasets = self.coords
         isel = {}
         for coord_name, coord_values in coords.items():
             if coord_name not in av_coord_datasets:
                 raise KeyError(f'Coordinate {coord_name} not in {list(av_coord_datasets.keys())}')
             sel_coord_data = av_coord_datasets[coord_name][()]
             if method is None or method == 'exact':
                 idx = np.where(sel_coord_data == coord_values)[0]
@@ -1840,14 +1901,35 @@
                     _arr = _flat_arr.reshape(orig_shape)
                 return xr.DataArray(_arr, attrs=attrs)
             else:
                 if isinstance(_arr, np.ndarray):
                     return _arr
             return _arr
 
+        coords = {}
+        coordinates: Optional[Union[str, List[str]]] = ds_attrs.get(protected_attributes.COORDINATES, None)
+        if coordinates is not None:
+            if isinstance(coordinates, str):
+                coordinates = [coordinates, ]
+            else:
+                coordinates = list(coordinates)
+
+            for c in coordinates:
+                if c[0] == '/':
+                    _data = self.rootparent[c]
+                else:
+                    _data = self.parent[c]
+                _name = Path(c).stem
+                coords.update({_name: xr.DataArray(name=_name, dims=(),
+                                                   data=_data,
+                                                   attrs=pop_hdf_attributes(self.parent[c].attrs))})
+            da = xr.DataArray(name=Path(self.name).stem, data=arr, attrs=attrs)
+            for k, v in coords.items():
+                da = da.assign_coords({k: v})
+            return da
         return xr.DataArray(name=Path(self.name).stem, data=arr, attrs=attrs)
 
     def __repr__(self) -> str:
         r = super().__repr__()
         if not self:
             return r[:-1] + f' (convention "{convention.get_current_convention().name}")>'
         else:
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/ds_decoder.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/ds_decoder.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5attr.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/h5attr.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,16 +51,14 @@
 
     def __init__(self,
                  value, *,
                  definition: Optional[str] = None,
                  rdf_predicate=None,
                  rdf_object=None):
         self.value = value
-        if not isinstance(value, str):
-            raise TypeError(f'Attribute value must be a string but got {type(value)}')
         self.definition = definition  # skos:definition
         self.rdf_predicate = self._validate_rdf(rdf_predicate)
         self.rdf_object = self._validate_rdf(rdf_object)
 
     @staticmethod
     def _validate_rdf(value):
         if value is None:
@@ -84,25 +82,14 @@
         out += ')'
         return out
 
     def __str__(self) -> str:
         return self.__repr__()
 
 
-# def Attribute(value, definition: Optional[str] = None,
-#               rdf_predicate=None, rdf_object=None) -> AttributeValue:
-#     """attribute interface function"""
-#     return AttributeValue(
-#         value,
-#         definition,
-#         rdf_predicate,
-#         rdf_object
-#     )
-
-
 def pop_hdf_attributes(attrs: Dict) -> Dict:
     """Remove HDF attributes like NAME, CLASS, .... from the input dictionary
 
     Parameters
     ----------
     attrs: Dict
         Input dictionary
@@ -154,37 +141,37 @@
                 return ret
             if ret[0] == '{':
                 dictionary = json.loads(ret)
                 for k, v in dictionary.items():
                     if isinstance(v, str):
                         if not v:
                             dictionary[k] = ''
-                        else:
-                            if v[0] == '/':
-                                if isinstance(_id, h5py.h5g.GroupID):
-                                    rootgrp = get_rootparent(h5py.Group(_id))
-                                    dictionary[k] = rootgrp.get(v)
-                                elif isinstance(_id, h5py.h5d.DatasetID):
-                                    rootgrp = get_rootparent(h5py.Dataset(_id).parent)
-                                    dictionary[k] = rootgrp.get(v)
+                        # else:
+                        #     if v[0] == '/':
+                        #         if isinstance(_id, h5py.h5g.GroupID):
+                        #             rootgrp = get_rootparent(h5py.Group(_id))
+                        #             dictionary[k] = rootgrp.get(v)
+                        #         elif isinstance(_id, h5py.h5d.DatasetID):
+                        #             rootgrp = get_rootparent(h5py.Dataset(_id).parent)
+                        #             dictionary[k] = rootgrp.get(v)
                 return dictionary
-            if ret[0] == '/':
-                # it may be group or dataset path or actually just a filepath stored by the user
-                if isinstance(_id, h5py.h5g.GroupID):
-                    # call like this, otherwise recursive call!
-                    from .core import Group
-                    rootgrp = get_rootparent(Group(_id))
-                    if rootgrp.get(ret) is None:
-                        # not a dataset or group, maybe just a filename that has been stored
-                        return ret
-                    return rootgrp.get(ret)
-                else:
-                    from .core import Dataset
-                    rootgrp = get_rootparent(Dataset(_id).parent)
-                    return rootgrp.get(ret)
+            # if ret[0] == '/':
+            #     # it may be group or dataset path or actually just a filepath stored by the user
+            #     if isinstance(_id, h5py.h5g.GroupID):
+            #         # call like this, otherwise recursive call!
+            #         from .core import Group
+            #         rootgrp = get_rootparent(Group(_id))
+            #         if rootgrp.get(ret) is None:
+            #             # not a dataset or group, maybe just a filename that has been stored
+            #             return ret
+            #         return rootgrp.get(ret)
+            #     else:
+            #         from .core import Dataset
+            #         rootgrp = get_rootparent(Dataset(_id).parent)
+            #         return rootgrp.get(ret)
             if ret[0] == '(':
                 if ret[-1] == ')':
                     # might be a tuple object
                     return ast.literal_eval(ret)
                 return ret
             if ret[0] == '[':
                 if ret[-1] == ']':
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5utils.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/h5utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/h5yaml.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/h5yaml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,55 +1,47 @@
 import h5py
 import pathlib
 import yaml
-from typing import Dict
-from typing import Protocol
+from typing import Dict, Optional, Protocol
 
 
 class _H5DictDataInterface(Protocol):
 
     @property
     def data(self) -> Dict:
         """Return data"""
         ...
 
-    def write(self, h5: h5py.Group):
+    def write(self, h5: h5py.Group, num_dtype:Optional[str]=None):
         data = self.data
         for k, v in data.items():
             if not isinstance(v, dict):
                 # is an attribute of the grou
                 h5.attrs[k] = v
             else:
                 # can be dataset or group
-                if H5Yaml.is_dataset(v):
+                if self.is_dataset(v):
                     v.pop('type', None)
                     if 'name' not in v:
                         v['name'] = k
                     # units = v.pop('units', None)
                     # standard_name = v.pop('standard_name', None)
                     # TODO remove the following hotfix
                     name = v.pop('name')
                     data = v.pop('data')
+                    dtype = v.pop('dtype', None)
                     try:
-                        h5.create_dataset(name, data=data, **v)
+                        if dtype is None and num_dtype and not isinstance(data, str):
+                            dtype = num_dtype
+
+                        h5.create_dataset(name, data=data, dtype=dtype, **v)
                     except (TypeError,) as e:
                         raise RuntimeError('Could not create dataset. Please check the yaml file. The orig. '
                                            f'error is "{e}"')
-                    # if isinstance(data, str):
-                    #     ds = h5.create_string_dataset(name, data=data,
-                    #                                   **v)
-                    # else:
-                    #     ds = h5.create_dataset(name=name, data=data)
-                    # for ak, av in v.items():
-                    #     ds.attrs[ak] = av
-                    # if units:
-                    #     ds.attrs['units'] = units
-                    # if standard_name:
-                    #     ds.attrs['standard_name'] = standard_name
-                elif H5Yaml.is_group(v):
+                elif self.is_group(v):
                     v.pop('type', None)
 
                     group_data = v.copy()
 
                     datasets = {_k: group_data.pop(_k) for _k, _v in v.items() if H5Yaml.is_dataset(_v)}
 
                     group_data['overwrite'] = group_data.get('overwrite', None)
@@ -57,15 +49,18 @@
 
                     if 'name' not in group_data:
                         group_data['name'] = k
 
                     g = h5.create_group(**group_data)
 
                     for ds_name, ds_params in datasets.items():
-                        g.create_dataset(name=ds_name, **ds_params)
+                        dtype = ds_params.pop('dtype', None)
+                        if dtype is None and num_dtype and not isinstance(ds_params['data'], str):
+                            dtype = num_dtype
+                        g.create_dataset(name=ds_name, dtype=dtype, **ds_params)
 
     @staticmethod
     def is_dataset(item) -> bool:
         if 'type' in item:
             return item['type'].lower() == 'dataset'
         if 'shape' in item:
             return True
@@ -78,15 +73,15 @@
         if 'type' in item:
             return item['type'].lower() == 'group'
         if isinstance(item, dict):
             for n, v in item.items():
                 if isinstance(v, dict):
                     return True
                 break
-            return not H5Yaml.is_dataset(item)
+            return not self.is_dataset(item)
         return False
 
 
 class H5Dict(_H5DictDataInterface):
 
     def __init__(self, data):
         self._data = data
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/jsonld.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/jsonld.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import pathlib
 import rdflib
 import warnings
 from itertools import count
 from ontolutils.classes.utils import split_URIRef
 from rdflib import Graph, URIRef, BNode, XSD, RDF, SKOS
 from rdflib.plugins.shared.jsonld.context import Context
-from typing import Dict, List
-from typing import Optional, Union, Iterable, Tuple, Any
+from typing import Dict, List, Optional, Union, Iterable, Tuple, Any
 
 from h5rdmtoolbox.convention import hdf_ontology
 from .core import Dataset, File
 from ..convention.ontology import HDF5
+from .rdf import RDF_TYPE_ATTR_NAME
 
 _bnode_counter = count()
 logger = logging.getLogger('h5rdmtoolbox')
 
 CONTEXT_PREFIXES = {
     'schema': 'https://schema.org/',
     'prov': 'http://www.w3.org/ns/prov#',
@@ -589,14 +589,17 @@
             if parent_node is not None:
                 _add_node(g, (parent_node, HDF5.member, obj_node))
 
         if isinstance(obj, h5py.Group):
             if structural:
                 _add_node(g, (obj_node, RDF.type, HDF5.Group))
                 _add_node(g, (obj_node, HDF5.name, rdflib.Literal(obj.name)))
+            h5_rdf_type = obj.attrs.get(RDF_TYPE_ATTR_NAME, None)
+            if h5_rdf_type:
+                _add_node(g, (obj_node, RDF.type, rdflib.URIRef(h5_rdf_type)))
             group_type = obj.rdf.type
             if isinstance(group_type, list):
                 for gs in group_type:
                     nsp, key = split_URIRef(gs)
                     ns_prefix, ns_iri = _get_iri_from_prefix(nsp, _context.get('@import', {}).values())
                     if ns_iri is not None:
                         _context.update({ns_prefix: ns_iri})
@@ -618,14 +621,18 @@
                 if obj.dtype.kind == 'S':
                     _add_node(g, (obj_node, HDF5.datatype, rdflib.Literal('H5T_STRING')))
                 elif obj.dtype.kind in ('i', 'u'):
                     _add_node(g, (obj_node, HDF5.datatype, rdflib.Literal('H5T_INTEGER')))
                 else:
                     _add_node(g, (obj_node, HDF5.datatype, rdflib.Literal('H5T_FLOAT')))
 
+            h5_rdf_type = obj.attrs.get(RDF_TYPE_ATTR_NAME, None)
+            if h5_rdf_type:
+                _add_node(g, (obj_node, RDF.type, rdflib.URIRef(h5_rdf_type)))
+
             obj_type = obj.rdf.subject
             if obj_type is not None:
                 _add_node(g, (obj_node, RDF.type, rdflib.URIRef(obj_type)))
 
         for ak, av in obj.attrs.items():
             logger.debug(f'Processing attribute "{ak}" with value "{av}"')
             if ak.isupper() or ak.startswith('@'):
@@ -634,24 +641,20 @@
 
             # create a new node for the attribute
             attr_node = rdflib.BNode(value=f'N{next(_bnode_counter)}') if use_simple_bnode_value else rdflib.BNode()
             logger.debug(f'Create new node for attribute "{ak}": {attr_node}')
 
             if structural:  # add hdf type and name nodes
                 _add_node(g, (attr_node, RDF.type, HDF5.Attribute))
-                # attr_def: str = obj.attrsdef.get(ak, None)
-                attr_def: str = obj.rdf[ak].definition# .get(ak, None)
+                attr_def: str = obj.rdf[ak].definition
                 if attr_def:
                     _add_node(g, (attr_node, HDF5.name, rdflib.Literal(ak)))
                     _add_node(g, (attr_node, SKOS.definition, rdflib.Literal(attr_def)))
                     if 'skos' not in ctx:
                         ctx['skos'] = 'http://www.w3.org/2004/02/skos/core#'
-                    # def_node = rdflib.BNode()
-                    # _add_node(g, (def_node, SCHEMA.comment, rdflib.Literal(attr_def)))
-                    # _add_node(g, (attr_node, HDF5.name, def_node))
                 else:
                     _add_node(g, (attr_node, HDF5.name, rdflib.Literal(ak)))
 
             list_node = None
             attr_literal = None
             # determine the attribute type and select respective RDF literal type
             if isinstance(av, str):
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/lazy.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/lazy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """lazy objects. user can work with datasets and groups without having to open the file him/her-self"""
 import pathlib
 from typing import Union, List, Dict, Optional
 
 import h5py
 
+from h5rdmtoolbox.protected_attributes import COORDINATES
 from h5rdmtoolbox.protocols import LazyObject
 
 
 class LHDFObject:
     """Lazy HDF object. This object is a proxy for an HDF object (dataset or group) that returns data
     on-demand. This means, that the file is opened when the object is accessed and closed when the object
     is no longer needed. This is useful for working with large files, where the user does not want to
@@ -109,30 +110,36 @@
         self.compression_opts = obj.compression_opts
         self.shuffle = obj.shuffle
         self.fletcher32 = obj.fletcher32
         self.maxshape = obj.maxshape
         self.fillvalue = obj.fillvalue
         self.scaleoffset = obj.scaleoffset
         self.external = obj.external
-
+        _coords = obj.attrs.get(COORDINATES, None)
+        if _coords is None:
+            self._coords = []
+        else:
+            self._coords = list(_coords)
+        for dim in obj.dims:
+            for i in range(len(dim)):
+                self._coords.append(lazy(dim[i]))
         self._file = None
 
     def __repr__(self):
         attrs_str = ', '.join({f'{k}={v}' for k, v in self.attrs.items() if not k.isupper()})
         return f'<LDataset "{self.name}" in "{self.filename}" attrs=({attrs_str})>'
 
     def __getitem__(self, item):
         from .. import File
         with File(self.filename, mode='r') as h5:
             return h5[self.name][item]
 
+    @property
     def coords(self):
-        from .. import File
-        with File(self.filename) as h5:
-            return h5[self.name].coords()
+        return self._coords
 
     def isel(self, **indexers):
         from .. import File
         with File(self.filename) as h5:
             return h5[self.name].isel(**indexers)
 
     def sel(self, **coords):
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/rdf.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/rdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """RDF (Resource Description Framework) module for use with HDF5 files"""
 import abc
 import h5py
 import pydantic
 from pydantic import HttpUrl
 from typing import Dict, Union, Optional, List
 
+from . import lazy
+from ..protocols import H5TbxAttributeManager
+
 RDF_OBJECT_ATTR_NAME = 'RDF_OBJECT'
 RDF_PREDICATE_ATTR_NAME = 'RDF_PREDICATE'
 RDF_SUBJECT_ATTR_NAME = '@ID'  # equivalent to @ID in JSON-LD, thus can only be one value!!!
 RDF_TYPE_ATTR_NAME = '@TYPE'  # equivalent to @type in JSON-LD, thus can be multiple values.
 
 DEFINITION_ATTR_NAME = 'ATTR_DEFINITION'
 
@@ -239,15 +242,15 @@
     def __setiri__(self, key, value):
         set_object(self._attr, key, value)
 
 
 class RDFManager:
     """IRI attribute manager"""
 
-    def __init__(self, attr: h5py.AttributeManager = None):
+    def __init__(self, attr: H5TbxAttributeManager = None):
         self._attr = attr
 
     def __str__(self) -> str:
         return f'{self.__class__.__name__} ({self.parent.name})'
 
     def __repr__(self) -> str:
         return self.__str__()
@@ -342,15 +345,15 @@
         for flag, item in zip([rdf_subject, res_types, rdf_predicate, rdf_object], res):
             if flag:
                 item_set = set(item)
                 if not common_objects:
                     common_objects = item_set
                 else:
                     common_objects = common_objects.intersection(item_set)
-        return list(common_objects)
+        return [lazy.lazy(c) for c in list(common_objects)]
 
     @property
     def type(self) -> Union[str, List[str], None]:
         """Returns the RDF subject (@type in JSON-LD syntax) of the group or dataset.
         Note, that it can be None, if no type is set and a list if multiple types are set.
         Else it will return a string.
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox/wrapper/xr2hdf.py` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox/wrapper/xr2hdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
                                      'different values. \nCannot create the dataset '
                                      f'"{name}". Either delete the existing coordinate dataset '
                                      'or write the dataset to a different group.')
 
         attach_scales = []
         coordinates_0dim = []
 
+
         for coord in self._obj.coords:
             if coord not in group:
                 _data = self._obj.coords[coord].values
                 coord_attrs = self._obj.coords[coord].attrs
                 if _data.ndim == 0:
                     _ = kwargs.pop('compression_opts', None)
                     _ = kwargs.pop('compression', None)
@@ -67,23 +68,25 @@
                                                attrs=coord_attrs, **kwargs)
                 else:
                     cds = group.create_dataset(coord,
                                                data=self._obj.coords[coord].values,
                                                attrs=coord_attrs, **kwargs)
                 for k, v in self._obj.coords[coord].attrs.items():
                     cds.attrs[k] = v
-                cds.make_scale()
-
-            if 'REFERENCE_LIST' not in group[coord].attrs:
-                group[coord].make_scale()
+                if self._obj.shape != cds.shape and cds.ndim == 0:
+                    coordinates_0dim.append(coord)
+                else:
+                    cds.make_scale()
+                    if 'REFERENCE_LIST' not in group[coord].attrs:
+                        group[coord].make_scale()
 
-            if self._obj.coords[coord].ndim == 0:
-                coordinates_0dim.append(coord)  # will be written to attribute "COORDINATES"
-            else:
-                attach_scales.append(coord)
+            # if self._obj.coords[coord].ndim == 0:
+            #     coordinates_0dim.append(coord)  # will be written to attribute "COORDINATES"
+            # else:
+            #     attach_scales.append(coord)
 
         dset = group.create_dataset(name, data=self._obj.data, attrs=ds_attrs, **kwargs)
         # for k, v in ds_attrs.items():
         #     try:
         #         if isinstance(v, str):
         #             dset.attrs[k] = str(v)
         #         else:
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/PKG-INFO` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5rdmtoolbox
-Version: 1.3.0a1
+Version: 1.3.1
 Summary: Supporting a FAIR Research Data lifecycle using Python and HDF5.
 Home-page: https://h5rdmtoolbox.readthedocs.io/en/latest/
 Author: Matthias Probst
 Author-email: matthias.probst@kit.edu
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -148,57 +148,60 @@
 
 ## Highlights
 
 - Combining HDF5 and [xarray](https://docs.xarray.dev/en/stable/) to allow easy access to metadata and data during
   analysis and processing (
   see [here](https://h5rdmtoolbox.readthedocs.io/en/latest/gettingstarted/quickoverview.html#datasets-xarray-interface)).
 - Assigning [metadata with "globally unique and persistent identifiers"]() as required
-  by [F1 of the FAIR principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/)
-  . This "remove[s] ambiguity in the meaning of your published data...".
+  by [F1 of the FAIR principles](https://www.go-fair.org/fair-principles/f1-meta-data-assigned-globally-unique-persistent-identifiers/).
+  This can be achieved by using [RDF triples](https://www.w3.org/RDF/), which removes "ambiguity in the meaning of your
+  published data".
 - Define standard attributes through
   [conventions](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/convention/index.html) and enforce users to use
-  them
+  certain attributes in their HDF5 files, such as units and a description, for example.
 - Upload HDF5 files directly
   to [repositories](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/repository/index.html)
   like [Zenodo](https://zenodo.org/)
   or [use them with noSQL databases](https://h5rdmtoolbox.readthedocs.io/en/latest/userguide/database/index.html) like
   [mongoDB](https://www.mongodb.com/).
 
 ## Who is the package for?
 
 For everybody, who is...
 
-- ... looking for a management approach for his or her data
-- ... community has not yet established a stable convention
-- ... working with small and big data, that fits into HDF5 files
-- ... looking for an easy way to work with HDF5, especially through Jupyter Notebooks
-- ... looking to integrate HDF5 with repositories and databases
-- ... looking for a way to do all the above whiles not needing to learn a new syntax
-- ... new to HDF5 and wants to learn about it, especially with respect to the FAIR principles and data management
+- ... looking for a management approach for his or her data.
+- ... community has not yet established a stable convention.
+- ... working with small and big data, that fits into HDF5 files.
+- ... looking for an easy way to work with HDF5, especially through Jupyter Notebooks.
+- ... trying to integrate HDF5 with repositories and databases.
+- ... wishing to enrich data semantically with the RDF standard.
+- ... looking for a way to do all the above whiles not needing to learn a new syntax.
+- ... new to HDF5 and wants to learn about it, especially with respect to the FAIR principles and data management.
 
 ## Who is it not for?
 
 For everybody, who ...
 
 - ... is looking for a management approach which at the same time allows high-performance and/or parallel work with HDF5
-- ... has established conventions and managements approaches in his or her community
+- ... has already well-established conventions and managements approaches in his or her community
 
 ## Package Architecture/structure
 
 The toolbox implements five modules, which are shown below. The numbers reference to their main usage in the stages in
 the data lifecycle above. Except the wrapper module, which uses the convention module, all other modules are independent
 of each other.
 
 <a href="https://h5rdmtoolbox.readthedocs.io/en/latest/"><img src="docs/_static/h5tbx_modules.svg" alt="H5TBX modules" style="widht:600px;"></a>
 
 Current implementation highlights in the modules:
 
 - The **wrapper** module adds functionality on top of the `h5py` package. It allows to include so-called standard names,
-  which are defined in conventions. And it implements an interface with the package `xarray`, which allows to carry
-  metadata from HDF5 to the user.
+  which are defined in conventions. And it implements interfaces, such as to the package `xarray`, which allows to carry
+  metadata from HDF5 to the user. Other high-level interfaces like `.rdf` allows assigning semantic information to the
+  HDF5 file.
 - For the **database** module, `hdfDB` and `mongoDB` are implemented. The `hdfDB` module allows to use HDF5 files as a
   database. The `mongoDB` module allows to use mongoDB as a database by mapping the metadata of HDF5 files to the
   database.
 - For the **repository** module, a Zenodo interface is implemented. Zenodo is a repository, which allows to upload and
   download data with a persistent identifier.
 - For the **convention** module,
   the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
@@ -262,22 +265,22 @@
 - `h5py=3.7.0`: HDF5 file interface
 - `xarray>=2022.3.0`: Working with scientific arrays in combination with attributes. Allows carrying metadata from HDF5
   to user
 - `pint>=0.19.2`: Allows working with units
 - `pint_xarray>=0.2.1`: Working with units for usage with xarray
 - `python-forge==18.6.0`: Used to update function signatures when using
   the [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
-- `pydantic`: Used to validate [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
+- `pydantic`: Used to
+  validate [standard attributes](https://h5rdmtoolbox.readthedocs.io/en/latest/conventions/standard_attributes_and_conventions.html)
 - `pyyaml>6.0.0`: Reading and writing of yaml files, e.g. metadata definitions (conventions). Note, lower versions
   collide with python 3.11
 - `requests`: Used to download files from the internet or validate URLs, e.g. metadata definitions (conventions)
 - `rdflib`: Used to enable working with RDF
 - `ontolutils`: Required to work with RDF and derive semantic description of HDF5 file content
 
-
 #### Optional dependencies
 
 To run unit tests or to enable certain features, additional dependencies must be installed.
 
 Install optional dependencies by specifying them in square brackets after the package name, e.g.:
 
     pip install h5RDMtoolbox[mongodb]
@@ -293,15 +296,14 @@
 [snt]
 
 - `xmltodict`: Reading of xml files
 - `tabulate>=0.8.10`: Pretty printing of tables
 - `python-gitlab`: Access to gitlab repositories
 - `pypandoc>=2.3`: Conversion of markdown files to html
 
-
 ## Citing the package
 
 If you intend to use the package in your work, you may cite the paper in the
 journal [inggrid](https://preprints.inggrid.org/repository/view/23/)
 
 Here's the bibtext to it:
```

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/SOURCES.txt` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/h5rdmtoolbox.egg-info/requires.txt` & `h5rdmtoolbox-1.3.1/h5rdmtoolbox.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/setup.cfg` & `h5rdmtoolbox-1.3.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,142 +1,142 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2068 3572 646d 746f 6f6c 626f 780d   = h5rdmtoolbox.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e33 2e30  .version = 1.3.0
-00000030: 6131 0d0a 6175 7468 6f72 203d 204d 6174  a1..author = Mat
-00000040: 7468 6961 7320 5072 6f62 7374 0d0a 6175  thias Probst..au
-00000050: 7468 6f72 5f65 6d61 696c 203d 206d 6174  thor_email = mat
-00000060: 7468 6961 732e 7072 6f62 7374 406b 6974  thias.probst@kit
-00000070: 2e65 6475 0d0a 6465 7363 7269 7074 696f  .edu..descriptio
-00000080: 6e20 3d20 5375 7070 6f72 7469 6e67 2061  n = Supporting a
-00000090: 2046 4149 5220 5265 7365 6172 6368 2044   FAIR Research D
-000000a0: 6174 6120 6c69 6665 6379 636c 6520 7573  ata lifecycle us
-000000b0: 696e 6720 5079 7468 6f6e 2061 6e64 2048  ing Python and H
-000000c0: 4446 352e 0d0a 6c6f 6e67 5f64 6573 6372  DF5...long_descr
-000000d0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
-000000e0: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
-000000f0: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
-00000100: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
-00000110: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
-00000120: 7474 7073 3a2f 2f68 3572 646d 746f 6f6c  ttps://h5rdmtool
-00000130: 626f 782e 7265 6164 7468 6564 6f63 732e  box.readthedocs.
-00000140: 696f 2f65 6e2f 6c61 7465 7374 2f0d 0a63  io/en/latest/..c
-00000150: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
-00000160: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-00000170: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-00000180: 3a20 332e 380d 0a09 5072 6f67 7261 6d6d  : 3.8...Programm
-00000190: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000001a0: 5079 7468 6f6e 203a 3a20 332e 390d 0a09  Python :: 3.9...
-000001b0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001c0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001d0: 3a20 332e 3130 0d0a 0950 726f 6772 616d  : 3.10...Program
-000001e0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001f0: 2050 7974 686f 6e20 3a3a 2033 2e31 310d   Python :: 3.11.
-00000200: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000210: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000220: 203a 3a20 332e 3132 0d0a 094c 6963 656e   :: 3.12...Licen
-00000230: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000240: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-00000250: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
-00000260: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000270: 656e 6465 6e74 0d0a 0944 6576 656c 6f70  endent...Develop
-00000280: 6d65 6e74 2053 7461 7475 7320 3a3a 2034  ment Status :: 4
-00000290: 202d 2042 6574 610d 0a09 546f 7069 6320   - Beta...Topic 
-000002a0: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
-000002b0: 6769 6e65 6572 696e 670d 0a0d 0a5b 6f70  gineering....[op
-000002c0: 7469 6f6e 735d 0d0a 7061 636b 6167 6573  tions]..packages
-000002d0: 203d 2066 696e 643a 0d0a 7079 7468 6f6e   = find:..python
-000002e0: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-000002f0: 382c 203c 332e 3133 0d0a 696e 636c 7564  8, <3.13..includ
-00000300: 655f 7061 636b 6167 655f 6461 7461 203d  e_package_data =
-00000310: 2054 7275 650d 0a69 6e73 7461 6c6c 5f72   True..install_r
-00000320: 6571 7569 7265 7320 3d20 0d0a 0961 7070  equires = ...app
-00000330: 6469 7273 203e 3d20 312e 342e 340d 0a09  dirs >= 1.4.4...
-00000340: 696d 706f 7274 6c69 625f 7265 736f 7572  importlib_resour
-00000350: 6365 730d 0a09 6e75 6d70 7920 3e3d 2031  ces...numpy >= 1
-00000360: 2e32 300d 0a09 6835 7079 203e 2033 2e37  .20...h5py > 3.7
-00000370: 2e30 0d0a 096d 6174 706c 6f74 6c69 6220  .0...matplotlib 
-00000380: 3e3d 2033 2e35 2e32 0d0a 0949 5079 7468  >= 3.5.2...IPyth
-00000390: 6f6e 203e 3d20 372e 3334 2e30 2020 2320  on >= 7.34.0  # 
-000003a0: 636f 6c61 6220 7761 6e74 7320 372e 3334  colab wants 7.34
-000003b0: 2e30 0d0a 0970 7979 616d 6c20 3e20 362e  .0...pyyaml > 6.
-000003c0: 3020 2023 2035 2e34 2064 6f65 7320 6e6f  0  # 5.4 does no
-000003d0: 7420 776f 726b 2077 6974 6820 7079 7468  t work with pyth
-000003e0: 6f6e 2033 2e31 3121 0d0a 0978 6172 7261  on 3.11!...xarra
-000003f0: 7920 3e3d 2032 3032 322e 332e 300d 0a09  y >= 2022.3.0...
-00000400: 7069 6e74 203d 3d20 302e 3231 2e31 2020  pint == 0.21.1  
-00000410: 2320 7069 6e74 203e 3d20 302e 3139 2e32  # pint >= 0.19.2
-00000420: 3c30 2e32 322e 3020 4e6f 7465 3a20 302e  <0.22.0 Note: 0.
-00000430: 3232 2e30 2073 686f 7773 2062 6164 2073  22.0 shows bad s
-00000440: 7472 2d6f 7574 7075 7420 666f 7220 7175  tr-output for qu
-00000450: 616e 7469 7469 6573 2077 6974 6820 666f  antities with fo
-00000460: 726d 6174 204c 787e 0d0a 0970 696e 745f  rmat Lx~...pint_
-00000470: 7861 7272 6179 2023 203e 3d20 302e 322e  xarray # >= 0.2.
-00000480: 310d 0a09 7265 6765 7820 2320 3e3d 2032  1...regex # >= 2
-00000490: 3032 330d 0a09 7061 636b 6167 696e 670d  023...packaging.
-000004a0: 0a09 6f6e 746f 6c75 7469 6c73 3e3d 302e  ..ontolutils>=0.
-000004b0: 322e 3230 0d0a 0970 7974 686f 6e2d 666f  2.20...python-fo
-000004c0: 7267 6520 2320 3d3d 2031 382e 362e 300d  rge # == 18.6.0.
-000004d0: 0a09 7265 7175 6573 7473 0d0a 0970 7964  ..requests...pyd
-000004e0: 616e 7469 6320 3e3d 2032 2e33 2e30 0d0a  antic >= 2.3.0..
-000004f0: 0972 6466 6c69 620d 0a0d 0a5b 6f70 7469  .rdflib....[opti
-00000500: 6f6e 732e 6578 7472 6173 5f72 6571 7569  ons.extras_requi
-00000510: 7265 5d0d 0a64 6174 6162 6173 6520 3d20  re]..database = 
-00000520: 0d0a 0970 796d 6f6e 676f 2023 203e 3d20  ...pymongo # >= 
-00000530: 342e 322e 300d 0a6c 6179 6f75 745f 7661  4.2.0..layout_va
-00000540: 6c69 6461 7469 6f6e 203d 200d 0a09 7461  lidation = ...ta
-00000550: 6275 6c61 7465 0d0a 6373 7620 3d20 0d0a  bulate..csv = ..
-00000560: 0970 616e 6461 7320 2320 3e3d 2031 2e34  .pandas # >= 1.4
-00000570: 2e33 0d0a 736e 7420 3d20 0d0a 0978 6d6c  .3..snt = ...xml
-00000580: 746f 6469 6374 0d0a 0974 6162 756c 6174  todict...tabulat
-00000590: 6520 2320 3e3d 2030 2e38 2e31 300d 0a09  e # >= 0.8.10...
-000005a0: 7079 7468 6f6e 2d67 6974 6c61 620d 0a09  python-gitlab...
-000005b0: 7079 7061 6e64 6f63 2023 203e 3d20 312e  pypandoc # >= 1.
-000005c0: 3131 0d0a 6775 6920 3d20 0d0a 0950 7951  11..gui = ...PyQ
-000005d0: 7435 0d0a 7465 7374 203d 200d 0a09 7079  t5..test = ...py
-000005e0: 7465 7374 203e 3d20 372e 312e 320d 0a09  test >= 7.1.2...
-000005f0: 7079 7465 7374 2d63 6f76 0d0a 0970 796c  pytest-cov...pyl
-00000600: 696e 740d 0a09 786d 6c74 6f64 6963 740d  int...xmltodict.
-00000610: 0a09 7363 6970 7920 2023 2070 726f 7669  ..scipy  # provi
-00000620: 6465 7320 6e65 7463 6466 340d 0a09 2528  des netcdf4...%(
-00000630: 6373 7629 730d 0a09 2528 736e 7429 730d  csv)s...%(snt)s.
-00000640: 0a09 2528 6461 7461 6261 7365 2973 0d0a  ..%(database)s..
-00000650: 646f 6373 203d 200d 0a09 2528 6373 7629  docs = ...%(csv)
-00000660: 730d 0a09 2528 736e 7429 730d 0a09 2528  s...%(snt)s...%(
-00000670: 6461 7461 6261 7365 2973 0d0a 0925 2874  database)s...%(t
-00000680: 6573 7429 730d 0a09 6a75 7079 7465 726c  est)s...jupyterl
-00000690: 6162 0d0a 0953 7068 696e 7820 3e3d 2033  ab...Sphinx >= 3
-000006a0: 2c3c 350d 0a09 7370 6869 6e78 5f62 6f6f  ,<5...sphinx_boo
-000006b0: 6b5f 7468 656d 6520 3d3d 2030 2e33 2e33  k_theme == 0.3.3
-000006c0: 0d0a 0973 7068 696e 782d 636f 7079 6275  ...sphinx-copybu
-000006d0: 7474 6f6e 0d0a 0973 6369 6b69 742d 696d  tton...scikit-im
-000006e0: 6167 650d 0a09 7363 696b 6974 2d6c 6561  age...scikit-lea
-000006f0: 726e 0d0a 0973 7068 696e 782d 6465 7369  rn...sphinx-desi
-00000700: 676e 0d0a 0973 696d 706c 656a 736f 6e0d  gn...simplejson.
-00000710: 0a09 6d79 7374 2d6e 620d 0a09 7370 6869  ..myst-nb...sphi
-00000720: 6e78 636f 6e74 7269 622d 6269 6274 6578  nxcontrib-bibtex
-00000730: 0d0a 096b 676c 6162 0d0a 636f 6d70 6c65  ...kglab..comple
-00000740: 7465 203d 200d 0a09 2528 6775 6929 730d  te = ...%(gui)s.
-00000750: 0a09 2528 7465 7374 2973 0d0a 0925 2864  ..%(test)s...%(d
-00000760: 6f63 7329 730d 0a0d 0a5b 6f70 7469 6f6e  ocs)s....[option
-00000770: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
-00000780: 0a68 3572 646d 746f 6f6c 626f 7820 3d20  .h5rdmtoolbox = 
-00000790: 0d0a 0964 6174 612f 2a2e 7961 6d6c 0d0a  ...data/*.yaml..
-000007a0: 0964 6174 612f 2a2e 796d 6c0d 0a09 6461  .data/*.yml...da
-000007b0: 7461 2f2a 2e70 6e67 0d0a 0964 6174 612f  ta/*.png...data/
-000007c0: 5462 784c 6179 6f75 742e 6864 660d 0a09  TbxLayout.hdf...
-000007d0: 6461 7461 2f45 6d70 7479 4c61 796f 7574  data/EmptyLayout
-000007e0: 2e68 6466 0d0a 0964 6174 612f 7374 796c  .hdf...data/styl
-000007f0: 652e 6373 730d 0a09 7465 7374 732f 6461  e.css...tests/da
-00000800: 7461 2f2a 0d0a 0963 6f6e 7665 6e74 696f  ta/*...conventio
-00000810: 6e73 2f68 746d 6c2f 7465 6d70 6c61 7465  ns/html/template
-00000820: 2e68 746d 6c0d 0a0d 0a5b 746f 6f6c 3a70  .html....[tool:p
-00000830: 7974 6573 745d 0d0a 7079 7468 6f6e 5f66  ytest]..python_f
-00000840: 696c 6573 203d 2074 6573 745f 2a2e 7079  iles = test_*.py
-00000850: 0d0a 7465 7374 7061 7468 7320 3d20 7465  ..testpaths = te
-00000860: 7374 730d 0a0d 0a5b 6f70 7469 6f6e 732e  sts....[options.
-00000870: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
-00000880: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
-00000890: 200d 0a09 6835 7462 7820 3d20 6835 7264   ...h5tbx = h5rd
-000008a0: 6d74 6f6f 6c62 6f78 2e63 6c69 3a6d 6169  mtoolbox.cli:mai
-000008b0: 6e0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  n....[egg_info].
-000008c0: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-000008d0: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e33 2e31  .version = 1.3.1
+00000030: 0d0a 6175 7468 6f72 203d 204d 6174 7468  ..author = Matth
+00000040: 6961 7320 5072 6f62 7374 0d0a 6175 7468  ias Probst..auth
+00000050: 6f72 5f65 6d61 696c 203d 206d 6174 7468  or_email = matth
+00000060: 6961 732e 7072 6f62 7374 406b 6974 2e65  ias.probst@kit.e
+00000070: 6475 0d0a 6465 7363 7269 7074 696f 6e20  du..description 
+00000080: 3d20 5375 7070 6f72 7469 6e67 2061 2046  = Supporting a F
+00000090: 4149 5220 5265 7365 6172 6368 2044 6174  AIR Research Dat
+000000a0: 6120 6c69 6665 6379 636c 6520 7573 696e  a lifecycle usin
+000000b0: 6720 5079 7468 6f6e 2061 6e64 2048 4446  g Python and HDF
+000000c0: 352e 0d0a 6c6f 6e67 5f64 6573 6372 6970  5...long_descrip
+000000d0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
+000000e0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
+000000f0: 6372 6970 7469 6f6e 5f63 6f6e 7465 6e74  cription_content
+00000100: 5f74 7970 6520 3d20 7465 7874 2f6d 6172  _type = text/mar
+00000110: 6b64 6f77 6e0d 0a75 726c 203d 2068 7474  kdown..url = htt
+00000120: 7073 3a2f 2f68 3572 646d 746f 6f6c 626f  ps://h5rdmtoolbo
+00000130: 782e 7265 6164 7468 6564 6f63 732e 696f  x.readthedocs.io
+00000140: 2f65 6e2f 6c61 7465 7374 2f0d 0a63 6c61  /en/latest/..cla
+00000150: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
+00000160: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000170: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000180: 332e 380d 0a09 5072 6f67 7261 6d6d 696e  3.8...Programmin
+00000190: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+000001a0: 7468 6f6e 203a 3a20 332e 390d 0a09 5072  thon :: 3.9...Pr
+000001b0: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+000001c0: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+000001d0: 332e 3130 0d0a 0950 726f 6772 616d 6d69  3.10...Programmi
+000001e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+000001f0: 7974 686f 6e20 3a3a 2033 2e31 310d 0a09  ython :: 3.11...
+00000200: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000210: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000220: 3a20 332e 3132 0d0a 094c 6963 656e 7365  : 3.12...License
+00000230: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00000240: 203a 3a20 4d49 5420 4c69 6365 6e73 650d   :: MIT License.
+00000250: 0a09 4f70 6572 6174 696e 6720 5379 7374  ..Operating Syst
+00000260: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000270: 6465 6e74 0d0a 0944 6576 656c 6f70 6d65  dent...Developme
+00000280: 6e74 2053 7461 7475 7320 3a3a 2034 202d  nt Status :: 4 -
+00000290: 2042 6574 610d 0a09 546f 7069 6320 3a3a   Beta...Topic ::
+000002a0: 2053 6369 656e 7469 6669 632f 456e 6769   Scientific/Engi
+000002b0: 6e65 6572 696e 670d 0a0d 0a5b 6f70 7469  neering....[opti
+000002c0: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
+000002d0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
+000002e0: 6571 7569 7265 7320 3d20 3e3d 332e 382c  equires = >=3.8,
+000002f0: 203c 332e 3133 0d0a 696e 636c 7564 655f   <3.13..include_
+00000300: 7061 636b 6167 655f 6461 7461 203d 2054  package_data = T
+00000310: 7275 650d 0a69 6e73 7461 6c6c 5f72 6571  rue..install_req
+00000320: 7569 7265 7320 3d20 0d0a 0961 7070 6469  uires = ...appdi
+00000330: 7273 203e 3d20 312e 342e 340d 0a09 696d  rs >= 1.4.4...im
+00000340: 706f 7274 6c69 625f 7265 736f 7572 6365  portlib_resource
+00000350: 730d 0a09 6e75 6d70 7920 3e3d 2031 2e32  s...numpy >= 1.2
+00000360: 300d 0a09 6835 7079 203e 2033 2e37 2e30  0...h5py > 3.7.0
+00000370: 0d0a 096d 6174 706c 6f74 6c69 6220 3e3d  ...matplotlib >=
+00000380: 2033 2e35 2e32 0d0a 0949 5079 7468 6f6e   3.5.2...IPython
+00000390: 203e 3d20 372e 3334 2e30 2020 2320 636f   >= 7.34.0  # co
+000003a0: 6c61 6220 7761 6e74 7320 372e 3334 2e30  lab wants 7.34.0
+000003b0: 0d0a 0970 7979 616d 6c20 3e20 362e 3020  ...pyyaml > 6.0 
+000003c0: 2023 2035 2e34 2064 6f65 7320 6e6f 7420   # 5.4 does not 
+000003d0: 776f 726b 2077 6974 6820 7079 7468 6f6e  work with python
+000003e0: 2033 2e31 3121 0d0a 0978 6172 7261 7920   3.11!...xarray 
+000003f0: 3e3d 2032 3032 322e 332e 300d 0a09 7069  >= 2022.3.0...pi
+00000400: 6e74 203d 3d20 302e 3231 2e31 2020 2320  nt == 0.21.1  # 
+00000410: 7069 6e74 203e 3d20 302e 3139 2e32 3c30  pint >= 0.19.2<0
+00000420: 2e32 322e 3020 4e6f 7465 3a20 302e 3232  .22.0 Note: 0.22
+00000430: 2e30 2073 686f 7773 2062 6164 2073 7472  .0 shows bad str
+00000440: 2d6f 7574 7075 7420 666f 7220 7175 616e  -output for quan
+00000450: 7469 7469 6573 2077 6974 6820 666f 726d  tities with form
+00000460: 6174 204c 787e 0d0a 0970 696e 745f 7861  at Lx~...pint_xa
+00000470: 7272 6179 2023 203e 3d20 302e 322e 310d  rray # >= 0.2.1.
+00000480: 0a09 7265 6765 7820 2320 3e3d 2032 3032  ..regex # >= 202
+00000490: 330d 0a09 7061 636b 6167 696e 670d 0a09  3...packaging...
+000004a0: 6f6e 746f 6c75 7469 6c73 3e3d 302e 322e  ontolutils>=0.2.
+000004b0: 3230 0d0a 0970 7974 686f 6e2d 666f 7267  20...python-forg
+000004c0: 6520 2320 3d3d 2031 382e 362e 300d 0a09  e # == 18.6.0...
+000004d0: 7265 7175 6573 7473 0d0a 0970 7964 616e  requests...pydan
+000004e0: 7469 6320 3e3d 2032 2e33 2e30 0d0a 0972  tic >= 2.3.0...r
+000004f0: 6466 6c69 620d 0a0d 0a5b 6f70 7469 6f6e  dflib....[option
+00000500: 732e 6578 7472 6173 5f72 6571 7569 7265  s.extras_require
+00000510: 5d0d 0a64 6174 6162 6173 6520 3d20 0d0a  ]..database = ..
+00000520: 0970 796d 6f6e 676f 2023 203e 3d20 342e  .pymongo # >= 4.
+00000530: 322e 300d 0a6c 6179 6f75 745f 7661 6c69  2.0..layout_vali
+00000540: 6461 7469 6f6e 203d 200d 0a09 7461 6275  dation = ...tabu
+00000550: 6c61 7465 0d0a 6373 7620 3d20 0d0a 0970  late..csv = ...p
+00000560: 616e 6461 7320 2320 3e3d 2031 2e34 2e33  andas # >= 1.4.3
+00000570: 0d0a 736e 7420 3d20 0d0a 0978 6d6c 746f  ..snt = ...xmlto
+00000580: 6469 6374 0d0a 0974 6162 756c 6174 6520  dict...tabulate 
+00000590: 2320 3e3d 2030 2e38 2e31 300d 0a09 7079  # >= 0.8.10...py
+000005a0: 7468 6f6e 2d67 6974 6c61 620d 0a09 7079  thon-gitlab...py
+000005b0: 7061 6e64 6f63 2023 203e 3d20 312e 3131  pandoc # >= 1.11
+000005c0: 0d0a 6775 6920 3d20 0d0a 0950 7951 7435  ..gui = ...PyQt5
+000005d0: 0d0a 7465 7374 203d 200d 0a09 7079 7465  ..test = ...pyte
+000005e0: 7374 203e 3d20 372e 312e 320d 0a09 7079  st >= 7.1.2...py
+000005f0: 7465 7374 2d63 6f76 0d0a 0970 796c 696e  test-cov...pylin
+00000600: 740d 0a09 786d 6c74 6f64 6963 740d 0a09  t...xmltodict...
+00000610: 7363 6970 7920 2023 2070 726f 7669 6465  scipy  # provide
+00000620: 7320 6e65 7463 6466 340d 0a09 2528 6373  s netcdf4...%(cs
+00000630: 7629 730d 0a09 2528 736e 7429 730d 0a09  v)s...%(snt)s...
+00000640: 2528 6461 7461 6261 7365 2973 0d0a 646f  %(database)s..do
+00000650: 6373 203d 200d 0a09 2528 6373 7629 730d  cs = ...%(csv)s.
+00000660: 0a09 2528 736e 7429 730d 0a09 2528 6461  ..%(snt)s...%(da
+00000670: 7461 6261 7365 2973 0d0a 0925 2874 6573  tabase)s...%(tes
+00000680: 7429 730d 0a09 6a75 7079 7465 726c 6162  t)s...jupyterlab
+00000690: 0d0a 0953 7068 696e 7820 3e3d 2033 2c3c  ...Sphinx >= 3,<
+000006a0: 350d 0a09 7370 6869 6e78 5f62 6f6f 6b5f  5...sphinx_book_
+000006b0: 7468 656d 6520 3d3d 2030 2e33 2e33 0d0a  theme == 0.3.3..
+000006c0: 0973 7068 696e 782d 636f 7079 6275 7474  .sphinx-copybutt
+000006d0: 6f6e 0d0a 0973 6369 6b69 742d 696d 6167  on...scikit-imag
+000006e0: 650d 0a09 7363 696b 6974 2d6c 6561 726e  e...scikit-learn
+000006f0: 0d0a 0973 7068 696e 782d 6465 7369 676e  ...sphinx-design
+00000700: 0d0a 0973 696d 706c 656a 736f 6e0d 0a09  ...simplejson...
+00000710: 6d79 7374 2d6e 620d 0a09 7370 6869 6e78  myst-nb...sphinx
+00000720: 636f 6e74 7269 622d 6269 6274 6578 0d0a  contrib-bibtex..
+00000730: 096b 676c 6162 0d0a 636f 6d70 6c65 7465  .kglab..complete
+00000740: 203d 200d 0a09 2528 6775 6929 730d 0a09   = ...%(gui)s...
+00000750: 2528 7465 7374 2973 0d0a 0925 2864 6f63  %(test)s...%(doc
+00000760: 7329 730d 0a0d 0a5b 6f70 7469 6f6e 732e  s)s....[options.
+00000770: 7061 636b 6167 655f 6461 7461 5d0d 0a68  package_data]..h
+00000780: 3572 646d 746f 6f6c 626f 7820 3d20 0d0a  5rdmtoolbox = ..
+00000790: 0964 6174 612f 2a2e 7961 6d6c 0d0a 0964  .data/*.yaml...d
+000007a0: 6174 612f 2a2e 796d 6c0d 0a09 6461 7461  ata/*.yml...data
+000007b0: 2f2a 2e70 6e67 0d0a 0964 6174 612f 5462  /*.png...data/Tb
+000007c0: 784c 6179 6f75 742e 6864 660d 0a09 6461  xLayout.hdf...da
+000007d0: 7461 2f45 6d70 7479 4c61 796f 7574 2e68  ta/EmptyLayout.h
+000007e0: 6466 0d0a 0964 6174 612f 7374 796c 652e  df...data/style.
+000007f0: 6373 730d 0a09 7465 7374 732f 6461 7461  css...tests/data
+00000800: 2f2a 0d0a 0963 6f6e 7665 6e74 696f 6e73  /*...conventions
+00000810: 2f68 746d 6c2f 7465 6d70 6c61 7465 2e68  /html/template.h
+00000820: 746d 6c0d 0a0d 0a5b 746f 6f6c 3a70 7974  tml....[tool:pyt
+00000830: 6573 745d 0d0a 7079 7468 6f6e 5f66 696c  est]..python_fil
+00000840: 6573 203d 2074 6573 745f 2a2e 7079 0d0a  es = test_*.py..
+00000850: 7465 7374 7061 7468 7320 3d20 7465 7374  testpaths = test
+00000860: 730d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  s....[options.en
+00000870: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
+00000880: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
+00000890: 0a09 6835 7462 7820 3d20 6835 7264 6d74  ..h5tbx = h5rdmt
+000008a0: 6f6f 6c62 6f78 2e63 6c69 3a6d 6169 6e0d  oolbox.cli:main.
+000008b0: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+000008c0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000008d0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `h5rdmtoolbox-1.3.0a1/tests/clean_zenodo_sandbox.py` & `h5rdmtoolbox-1.3.1/tests/clean_zenodo_sandbox.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_interface.py` & `h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/test_interface.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_provenance.py` & `h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/test_provenance.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_snt.py` & `h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/test_snt.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/standard_names/test_transformations_and_affixes.py` & `h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/standard_names/test_transformations_and_affixes.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/test_standard_attributes.py` & `h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/test_standard_attributes.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/standard_attributes/test_standard_names.py` & `h5rdmtoolbox-1.3.1/tests/conventions/standard_attributes/test_standard_names.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/test_conventions.py` & `h5rdmtoolbox-1.3.1/tests/conventions/test_conventions.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/test_engmeta.py` & `h5rdmtoolbox-1.3.1/tests/conventions/test_engmeta.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/test_ontology.py` & `h5rdmtoolbox-1.3.1/tests/conventions/test_ontology.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/test_references.py` & `h5rdmtoolbox-1.3.1/tests/conventions/test_references.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/test_toolbox_validators.py` & `h5rdmtoolbox-1.3.1/tests/conventions/test_toolbox_validators.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/conventions/test_utils.py` & `h5rdmtoolbox-1.3.1/tests/conventions/test_utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/database/test_find_rdf.py` & `h5rdmtoolbox-1.3.1/tests/database/test_find_rdf.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/database/test_hdfDB.py` & `h5rdmtoolbox-1.3.1/tests/database/test_hdfDB.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Test the mongoDB interface"""
 
 import h5py
 import numpy as np
+import pint
 import unittest
-
+from typing import List
 import h5rdmtoolbox as h5tbx
 from h5rdmtoolbox import database
 from h5rdmtoolbox.database import hdfdb
 from h5rdmtoolbox.database.hdfdb.query import _basename
 
 
 class TestHDFDB(unittest.TestCase):
@@ -22,16 +23,19 @@
             res = sorted(h5.find(['standard_name', 'units']))
             self.assertEqual(res[0].name, '/temp')
             self.assertEqual(res[1].name, '/vel/u')
 
     def test_find_in_files(self):
         with h5tbx.File(attrs=dict(name='root group')) as h51:
             h51.create_group('grp')
+            h51.create_dataset('x', data=[10, 20, 30], make_scale=True)
             h51.create_dataset('dataset', data=np.array([1, 2, 3]),
-                               attrs=dict(units='m/s'))
+                               attrs=dict(units='m/s'),
+                               attach_scale='x')
+            h51.find('units')
 
         with h5tbx.File() as h52:
             h52.create_group('grp', attrs=dict(name='grp name'))
             h52.create_dataset('dataset', data=np.array([3, 2, 1]),
                                attrs=dict(units='mm/s'))
 
         res = list(h5tbx.database.find([h51.hdf_filename, h52.hdf_filename],
@@ -554,7 +558,66 @@
 
         res = h5tbx.database.rdf_find(h5.hdf_filename,
                                       rdf_predicate=FOAF.firstName,
                                       rdf_subject='https://example.org/John')
         res_list = sorted(list(res), key=lambda x: x.name)
         self.assertEqual(len(res_list), 1)
         self.assertEqual(res_list[0].name, '/contact2')
+
+    def test_dtype_kind(self):
+        with h5tbx.File() as h5:
+            h5.create_string_dataset('strds', data='hallo')
+            h5.create_dataset('f32', shape=(3, 4), dtype='float32')
+            h5.create_dataset('f64', shape=(3, 4), dtype='float64')
+            h5.create_dataset('i32', shape=(3, 4), dtype='int32')
+
+            res = h5.find({'$dtype': lambda x: x.kind == 'S'})
+            for r in res:
+                self.assertEqual(r.name, '/strds')
+            numerical_datasets = h5.find({'$dtype': lambda x: x.kind in ('f', 'i', 'u')})
+            self.assertEqual(len(list(numerical_datasets)), 3)
+
+    def test_custom_find(self):
+        with h5tbx.File() as h5:
+            h5.create_dataset('u', data=4.3, attrs={'units': 'm/s', 'standard_name': 'x_velocity'})
+            h5.create_dataset('v', data=4.3, attrs={'units': 'm/s', 'standard_name': 'v_velocity'})  # invalid sn
+            h5.create_dataset('w', data=4.3, attrs={'units': 'invalid',
+                                                    'standard_name': 'z_velocity'})
+
+            ureg = pint.UnitRegistry()
+
+            def _validate_unit(units: str):
+                if units is None:
+                    return False
+
+                if units in ('', ' '):
+                    return True
+                try:
+                    ureg.parse_units(units)
+                    return True
+                except pint.UndefinedUnitError:
+                    return False
+
+            def _valid_standard_name(sn, list_of_sn:List[str]):
+                return sn in list_of_sn
+
+            res = h5.find({'units': lambda x: _validate_unit(x)})
+            self.assertEqual(len(res), 2)
+
+            res = h5.find({'standard_name': lambda x: _valid_standard_name(x, ['x_velocity',
+                                                                               'y_velocity',
+                                                                               'z_velocity'])})
+            self.assertEqual(len(res), 2)
+
+    def test_in(self):
+        with h5tbx.File() as h5:
+            h5.attrs['standard_name'] = 'Steady State'
+            res = h5.find({'standard_name': {'$in': ['Transient', 'Steady State']}})
+            self.assertEqual(len(res), 1)
+        with h5tbx.File() as h5:
+            h5.attrs['standard_name'] = 'Transient'
+            res = h5.find({'standard_name': {'$in': ['Transient', 'Steady State']}})
+            self.assertEqual(len(res), 1)
+        with h5tbx.File() as h5:
+            h5.attrs['standard_name'] = 'Transient2'
+            res = h5.find({'standard_name': {'$in': ['Transient', 'Steady State']}})
+            self.assertEqual(len(res), 0)
```

### Comparing `h5rdmtoolbox-1.3.0a1/tests/database/test_mongo.py` & `h5rdmtoolbox-1.3.1/tests/database/test_mongo.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/layouts/test_core.py` & `h5rdmtoolbox-1.3.1/tests/layouts/test_core.py`

 * *Files 20% similar despite different names*

```diff
@@ -75,14 +75,32 @@
         spec1_copy = lay.add(hdfdb.FileDB.find, flt={'$name': '/u'}, n=1)
         self.assertEqual(spec1, spec1_copy)
         self.assertFalse(spec1.__eq__(lay))
         self.assertEqual(spec1.called, False)
         with self.assertRaises(ValueError):
             spec1.n_successes
 
+    # def test_units_exists(self):
+    #     with h5tbx.File() as h5:
+    #         ds = h5.create_dataset('a', shape=(3, 4), dtype='float32')
+    #         ds.attrs['units'] = 'm/s'
+    #     lay = layout.Layout()
+    #     spec_all_dataset = lay.add(
+    #         hdfdb.FileDB.find,
+    #         flt={},
+    #         objfilter='dataset',
+    #         n={'$gte': 1},
+    #         description='At least one dataset exists'
+    #     )
+    #     spec_all_dataset.add(hdfdb.FileDB.find,
+    #                          flt={'units': {'$exists': True}},
+    #                          n=1,
+    #                          description='units exists')
+    #     res = lay.validate(h5.hdf_filename)
+
     def test_alternative_specification(self):
         """Expecting exactly one u, but if not found, exactly one v."""
         lay = layout.Layout()
         main_spec = lay.add(hdfdb.FileDB.find, flt={'$name': '/u'}, n=1, description='u exists')
         main_spec.add_alternative(hdfdb.FileDB.find, flt={'$name': '/v'}, n=1, description='v exists if u does not')
         # with h5tbx.File() as h5:
         #     h5.create_dataset('u', shape=(3, 4), dtype='float32')
@@ -95,15 +113,15 @@
         #     res = lay.validate(h5)
         #     self.assertTrue(res.is_valid())
 
         with h5tbx.File() as h5:
             # neither u nor v exist, should fail!
             h5.create_dataset('w', shape=(3, 4), dtype='float32')
             res = lay.validate(h5)
-            res.print_summary()
+            res.print_summary(exclude_keys='target_name')
             self.assertFalse(res.is_valid())
 
         lay = layout.Layout()
         main_spec = lay.add(hdfdb.FileDB.find, flt={'$name': '/u'}, n=None)
         with self.assertRaises(ValueError):
             main_spec.add_alternative(hdfdb.FileDB.find, flt={'$name': '/v'}, n=1)
 
@@ -219,34 +237,33 @@
             res = lay.validate(h5.filename)
             self.assertTrue(spec_number_of_specific_datasets.failed)
             self.assertEqual(spec_number_of_specific_datasets.n_fails, 1)
 
     def test_all_dtypes(self):
         filename = h5tbx.utils.generate_temporary_filename(suffix='.hdf')
         with h5py.File(filename, 'w') as h5:
-            ds = h5.create_dataset('u', shape=(3, 4), dtype='float32')
-            h5.create_dataset('a/u', shape=(3, 4), dtype='float64')
-            h5.create_dataset('a/v', shape=(3, 4), dtype='float32')
-            h5.create_dataset('a/b/c/u', shape=(3, 4), dtype='float64')
+            ds = h5.create_dataset('f32', shape=(3, 4), dtype='float32')
+            h5.create_dataset('a/f64', shape=(3, 4), dtype='float64')
+            h5.create_dataset('a/f32', shape=(3, 4), dtype='float32')
+            h5.create_dataset('a/b/c/f64', shape=(3, 4), dtype='float64')
 
             # there are 2 datasets with dtype float32 and 2 with float64
             # thus specification which checks float32 should fail twice
 
             lay = layout.Layout()
             spec_all_ds = lay.add(hdfdb.FileDB.find,
                                   description='Any dataset',
                                   n=None,  # optional
                                   recursive=True,
                                   flt={'$shape': {'$exists': True}},
                                   objfilter='dataset')  # all datasets
             spec_all_ds_are_float32 = spec_all_ds.add(
                 hdfdb.FileDB.find,
                 description='Is float32',
-                flt={'$dtype': np.dtype(
-                    '<f4')},
+                flt={'$dtype': np.dtype('<f4')},
                 n=1)  # applies all these on spec_all_ds results. So must be true per dataset (n=1)
 
             with self.assertRaises(RuntimeError):
                 lay(h5)
 
             res = lay.validate(h5)
             res.print_summary()
@@ -269,28 +286,77 @@
             h5.create_dataset('a/b/c/u', shape=(3, 4), dtype='float32')
 
             res = lay.validate(h5)
             self.assertTrue(res.is_valid())
             self.assertTrue(spec_all_ds.is_valid())
             self.assertTrue(spec_all_ds_are_float32.is_valid())
 
-
     def test_layout_with_rdf_find(self):
         from h5rdmtoolbox import database
         lay = layout.Layout()
         spec = lay.add(database.rdf_find, rdf_predicate="https://schema.org/name", n=1)
 
         with h5tbx.File() as h5:
             h5.attrs['name', 'https://schema.org/name'] = 'test'
 
         res = lay.validate(h5.hdf_filename)
         self.assertTrue(res.is_valid())
 
-
         lay = layout.Layout()
         spec = lay.add(database.rdf_find, rdf_predicate="https://schema.org/firstName", n=1)
 
         with h5tbx.File() as h5:
             h5.attrs['name', 'https://schema.org/name'] = 'test'
 
         res = lay.validate(h5.hdf_filename)
-        self.assertFalse(res.is_valid())
+        self.assertFalse(res.is_valid())
+
+    def test_rebase(self):
+        with h5tbx.File() as h5:
+            h5.create_group('setup')
+            h5['setup'].attrs['standard_name'] = 'Steady State'
+            h5.create_dataset('TIME', data=[1, 2, 3], attrs={'units': 's'})
+
+        lay = layout.Layout()
+        spec = lay.add(hdfdb.FileDB.find,
+                       flt={'standard_name': {'$in': ['Transient', 'Steady State']}},
+                       n=1)
+        spec.add(hdfdb.FileDB.find,
+                 rebase=True,  # start search from the root
+                 flt={'$name': '/TIME', 'units': 's', '$ndim': 1},
+                 n=1)
+
+        res = lay.validate(h5.hdf_filename)
+        self.assertTrue(res.is_valid())
+        with h5tbx.File() as h5:
+            h5.create_group('setup')
+            h5['setup'].attrs['standard_name'] = 'None of the above'
+            h5.create_dataset('TIME', data=[1, 2, 3], attrs={'units': 's'})
+
+        lay = layout.Layout()
+        spec = lay.add(hdfdb.FileDB.find,
+                       flt={'standard_name': {'$in': ['Transient', 'Steady State']}},
+                       n=None)
+        spec.add(hdfdb.FileDB.find,
+                 rebase=True,  # start search from the root
+                 flt={'$name': '/TIME', 'units': 's', '$ndim': 1},
+                 n=1)
+
+        res = lay.validate(h5.hdf_filename)
+        self.assertTrue(res.is_valid())
+
+        with h5tbx.File() as h5:
+            h5.create_group('setup')
+            h5['setup'].attrs['standard_name'] = 'Steady State'
+            # h5.create_dataset('TIME', data=[1, 2, 3], attrs={'units': 's'})
+
+        lay = layout.Layout()
+        spec = lay.add(hdfdb.FileDB.find,
+                       flt={'standard_name': {'$in': ['Transient', 'Steady State']}},
+                       n=1)
+        spec.add(hdfdb.FileDB.find,
+                 rebase=True,  # start search from the root
+                 flt={'$name': '/TIME', 'units': 's', '$ndim': 1},
+                 n=1)
+
+        res = lay.validate(h5.hdf_filename)
+        self.assertFalse(res.is_valid())
```

### Comparing `h5rdmtoolbox-1.3.0a1/tests/layouts/test_docs.py` & `h5rdmtoolbox-1.3.1/tests/layouts/test_docs.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/repository/test_zenodo.py` & `h5rdmtoolbox-1.3.1/tests/repository/test_zenodo.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/test_config.py` & `h5rdmtoolbox-1.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/test_extensions.py` & `h5rdmtoolbox-1.3.1/tests/test_extensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
-import numpy as np
 import unittest
+
+import numpy as np
 import xarray as xr
 
 import h5rdmtoolbox as h5tbx
 # noinspection PyUnresolvedReferences
 from h5rdmtoolbox.extensions import normalize, vector, magnitude, units
 
 
@@ -59,14 +60,24 @@
                 h5.Vector(u='u', v=6.5)
 
             vec = h5.Vector(uu='u', vv='v')[:]
             self.assertListEqual(list(vec.data_vars), ['uu', 'vv'])
             self.assertEqual(vec['uu'][0], 1)
             self.assertEqual(vec['vv'][0], 2)
 
+            vec = h5.Vector(u='u', v='v').isel(dim_0=slice(None, None, None), dim_1=slice(None, None, None))
+            self.assertIsInstance(vec, xr.Dataset)
+            self.assertTrue('u' in vec.data_vars)
+            self.assertTrue('v' in vec.data_vars)
+            self.assertEqual(vec['u'][0], 1)
+            self.assertEqual(vec['v'][0], 2)
+
+            with self.assertRaises(KeyError):
+                h5.Vector(u='u', v='v').sel(dim_0=5, dim_1=2)
+
     def test_normalize_issue_with_time_vector(self):
         with h5tbx.File() as h5:
             h5.create_dataset('x', data=[1, 2, 3], make_scale=True)
             now = datetime.datetime.now()
             h5.create_time_dataset('t',
                                    data=[now, now + datetime.timedelta(seconds=1), now + datetime.timedelta(seconds=2)],
                                    make_scale=True)
```

### Comparing `h5rdmtoolbox-1.3.0a1/tests/test_identifiers.py` & `h5rdmtoolbox-1.3.1/tests/test_identifiers.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/test_plotting.py` & `h5rdmtoolbox-1.3.1/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/test_repr.py` & `h5rdmtoolbox-1.3.1/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/test_user.py` & `h5rdmtoolbox-1.3.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/test_utils.py` & `h5rdmtoolbox-1.3.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/test_version.py` & `h5rdmtoolbox-1.3.1/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/test_xarray_export.py` & `h5rdmtoolbox-1.3.1/tests/test_xarray_export.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_core.py` & `h5rdmtoolbox-1.3.1/tests/wrapper/test_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import datetime
-import h5py
 import json
-import numpy as np
-import pandas as pd
 import pathlib
 import unittest
-import xarray as xr
 from datetime import datetime, timedelta
+
+import h5py
+import numpy as np
+import pandas as pd
+import xarray as xr
 from dateutil.parser import parse
 from numpy import linspace as ls
 
 import h5rdmtoolbox as h5tbx
 from h5rdmtoolbox import __version__
+# noinspection PyUnresolvedReferences
+from h5rdmtoolbox.extensions import units
 from h5rdmtoolbox.wrapper import h5yaml
 from h5rdmtoolbox.wrapper.h5attr import AttributeString
 
 logger = h5tbx.set_loglevel('ERROR')
 
 __this_dir__ = pathlib.Path(__file__).parent
 
@@ -140,14 +143,24 @@
             h5tbx.set_config(ignore_none=True)
             h5.attrs['none_attr'] = None
             self.assertFalse('none_attr' in h5)
             h5tbx.set_config(ignore_none=False)
             h5.attrs['none_attr'] = None
             self.assertEqual(h5.attrs['none_attr'], 'None')
 
+    def test_filename_attr(self):
+        with h5tbx.File() as h5:
+
+            h5.create_dataset('ds', data=np.arange(10))
+            h5['ds'].attrs['filename'] = '/path/to/file.csv'
+            self.assertEqual(h5['ds'].attrs['filename'], '/path/to/file.csv')
+
+            h5.attrs['filename'] = '/path/to/file.csv'
+            self.assertEqual(h5.attrs['filename'], '/path/to/file.csv')
+
     def test_rootparent(self):
         with h5tbx.File() as h5:
             g = h5.create_group('g')
             self.assertEqual(h5, g.rootparent)
             self.assertEqual(h5, h5['g'].rootparent)
             self.assertEqual(h5, h5.rootparent)
 
@@ -195,14 +208,20 @@
 
         df.to_csv(csv_filename1, index=None)
 
         with h5tbx.File() as h5:
             with self.assertRaises(ValueError):
                 h5.create_datasets_from_csv(csv_filenames=csv_filename1, combine_opt='invlaid')
             h5.create_datasets_from_csv(csv_filenames=csv_filename1)
+            self.assertEqual(pathlib.Path(h5['x'].attrs['source_filename']).resolve().absolute(),
+                             csv_filename1.resolve().absolute())
+            self.assertEqual(h5['x'].attrs['source_filename_hash_md5'], h5tbx.utils.get_checksum(csv_filename1))
+            self.assertEqual(pathlib.Path(h5['y'].attrs['source_filename']).resolve().absolute(),
+                             csv_filename1.resolve().absolute())
+            self.assertEqual(h5['y'].attrs['source_filename_hash_md5'], h5tbx.utils.get_checksum(csv_filename1))
             self.assertEqual(h5['x'].shape, (4,))
             self.assertEqual(h5['y'].shape, (4,))
             np.testing.assert_equal(h5['x'][:], np.array([1, 5, 10, 0]))
             np.testing.assert_equal(h5['y'][:], np.array([-3, 20, 0, 11.5]))
 
         with h5tbx.File() as h5:
             h5.create_dataset_from_csv(csv_filename=csv_filename1)
@@ -227,46 +246,51 @@
         csv_filename2 = h5tbx.utils.generate_temporary_filename(suffix='.csv')
 
         df2 = -1 * df
         df2.to_csv(csv_filename2, index=None)
 
         # test concatenate
         with h5tbx.File() as h5:
-            h5.create_datasets_from_csv(csv_filenames=(csv_filename1, csv_filename2),
+            h5.create_datasets_from_csv(csv_filenames=[csv_filename1, csv_filename2],
                                         combine_opt='concatenate')
             self.assertEqual(h5['x'].shape, (8,))
+            filenames = sorted([pathlib.Path(f).resolve().absolute() for f in h5['y'].attrs['source_filename']])
+            ref_filenames = sorted([csv_filename1.resolve().absolute(), csv_filename2.resolve().absolute()])
+            self.assertEqual(filenames, ref_filenames)
+            self.assertEqual(h5['y'].attrs['source_filename_hash_md5'],
+                             [h5tbx.utils.get_checksum(csv_filename1), h5tbx.utils.get_checksum(csv_filename2)])
             self.assertEqual(h5['y'].shape, (8,))
 
         # test stack
         with h5tbx.File() as h5:
-            h5.create_datasets_from_csv(csv_filenames=(csv_filename1, csv_filename2),
+            h5.create_datasets_from_csv(csv_filenames=[csv_filename1, csv_filename2],
                                         combine_opt='stack', axis=0)
             self.assertEqual(h5['x'].shape, (2, 4))
             np.testing.assert_equal(df['x'].values, h5['x'].values[0, :])
             np.testing.assert_equal(df2['x'].values, h5['x'].values[1, :])
             np.testing.assert_equal(df['y'].values, h5['y'].values[0, :])
             np.testing.assert_equal(df2['y'].values, h5['y'].values[1, :])
 
         with h5tbx.File() as h5:
-            h5.create_datasets_from_csv(csv_filenames=(csv_filename1, csv_filename2),
+            h5.create_datasets_from_csv(csv_filenames=[csv_filename1, csv_filename2],
                                         combine_opt='stack',
                                         axis=-1)
             self.assertEqual(h5['x'].shape, (4, 2))
             self.assertEqual(h5['y'].shape, (4, 2))
 
         with h5tbx.File() as h5:
-            h5.create_datasets_from_csv(csv_filenames=(csv_filename1, csv_filename2),
+            h5.create_datasets_from_csv(csv_filenames=[csv_filename1, csv_filename2],
                                         combine_opt='stack',
                                         axis=0,
                                         shape=(2, 2))
             self.assertEqual(h5['x'].shape, (2, 2, 2))
             self.assertEqual(h5['y'].shape, (2, 2, 2))
 
         with h5tbx.File() as h5:
-            h5.create_datasets_from_csv(csv_filenames=(csv_filename1, csv_filename2),
+            h5.create_datasets_from_csv(csv_filenames=[csv_filename1, csv_filename2],
                                         combine_opt='stack',
                                         axis=-1,
                                         shape=(2, 2))
             self.assertEqual(h5['x'].shape, (2, 2, 2))
             self.assertEqual(h5['y'].shape, (2, 2, 2))
 
     def test_slicing(self):
@@ -523,23 +547,23 @@
                 obj.attrs['an_attr'] = 'a_string'
                 self.assertEqual(obj.attrs['an_attr'], 'a_string')
                 obj.attrs['mean'] = 1.2
                 self.assertEqual(obj.attrs['mean'], 1.2)
 
                 # testing links:
                 obj.attrs['link_to_group'] = h5['/']
-                self.assertEqual(obj.attrs['link_to_group'], h5['/'])
-                self.assertIsInstance(obj.attrs['link_to_group'], h5py.Group)
+                self.assertEqual(obj.attrs['link_to_group'], '/')
+                self.assertIsInstance(obj.attrs['link_to_group'], str)
                 obj.attrs['link_to_ds'] = ds
                 self.assertEqual(obj.attrs['link_to_ds'], ds)
-                self.assertIsInstance(obj.attrs['link_to_ds'], h5py.Dataset)
+                self.assertIsInstance(obj.attrs['link_to_ds'], str)
                 obj.attrs['attribute_of_links_to_ds'] = {'ds': ds, 'grp': grp, 'astr': 'test', 'afloat': 3.1}
                 self.assertIsInstance(obj.attrs['attribute_of_links_to_ds'], dict)
-                self.assertIsInstance(obj.attrs['attribute_of_links_to_ds']['ds'], h5py.Dataset)
-                self.assertIsInstance(obj.attrs['attribute_of_links_to_ds']['grp'], h5py.Group)
+                self.assertIsInstance(obj.attrs['attribute_of_links_to_ds']['ds'], str)
+                self.assertIsInstance(obj.attrs['attribute_of_links_to_ds']['grp'], str)
                 self.assertIsInstance(obj.attrs['attribute_of_links_to_ds']['astr'], str)
                 self.assertIsInstance(obj.attrs['attribute_of_links_to_ds']['afloat'], float)
 
                 # testing units
                 test_vals = ('1.2m', '1.2 m', '1.2 [m]', '1.2 (m)')
                 for test_val in test_vals:
                     obj.attrs['mean_with_unit'] = test_val
@@ -655,36 +679,57 @@
             self.assertEqual('m', h5['ds2'].attrs['units'])
 
             h5.create_dataset('ds3', data=xr.DataArray([1, 2, 3]),
                               compression='gzip', compression_opts=1, attach_scale='time')
             self.assertEqual(1, len(h5['ds3'].dims[0].keys()))
             self.assertEqual('/time', h5['ds3'].dims[0][0].name)
 
+    def test_create_dataset_from_xr2(self):
+        da = xr.DataArray(name='pressure', data=[1, 2, 3])
+        da = da.assign_coords(x=4.3)
+
+        with h5tbx.File() as h5:
+            h5['pressure'] = da
+            # print(h5['pressure'].coords)
+            # h5.pressure.assign_coords(x=h5['x'])
+            # h5.pressure.attrs['COORDINATES'] = 'x'
+            p = h5.pressure[()]
+        self.assertEqual(p.x.data, 4.3)
+        self.assertTrue('x' in p.coords)
+
+        with h5tbx.File() as h5:
+            h5['pressure'] = xr.DataArray(name='pressure', data=[1, 2, 3])
+            h5['x'] = xr.DataArray(name='x', data=4.3)
+            h5['pressure'].assign_coord(h5['x'])
+            p = h5.pressure[()]
+        self.assertEqual(p.x.data, 4.3)
+        self.assertTrue('x' in p.coords)
+
     def test_create_dataset_scale_issues(self):
         with h5tbx.File() as h5:
             with self.assertRaises(ValueError):
                 h5.create_dataset('flag', data=[1, 0, 1], dtype='int8', make_scale=True, attach_scale='time')
 
     def test_coords(self):
         with h5tbx.File() as h5:
             h5.create_dataset('time', data=[1, 2, 3], make_scale=True)
             h5.create_dataset('vel', data=[1.5, 2.5, 3.5], attach_scales='time')
             h5.create_dataset('vel_no_scale', data=[1.5, 2.5, 3.5])
-            self.assertIsInstance(h5['vel'].coords(), dict)
-            self.assertEqual('time', list(h5['vel'].coords().keys())[0])
-            self.assertEqual({'time': h5['time']}, h5['vel'].coords())
-            self.assertEqual({}, h5['vel_no_scale'].coords())
+            self.assertIsInstance(h5['vel'].coords, dict)
+            self.assertEqual('time', list(h5['vel'].coords.keys())[0])
+            self.assertEqual({'time': h5['time']}, h5['vel'].coords)
+            self.assertEqual({}, h5['vel_no_scale'].coords)
 
         # multiple dims:
         with h5tbx.File() as h5:
             h5.create_dataset('x1', data=[1, 2, 3], make_scale=True)
             h5.create_dataset('x2', data=[10, 20, 30], make_scale=True)
             h5.create_dataset('data', data=[-1, 0, 1], attach_scales=('x1',))
             h5['data'].dims[0].attach_scale(h5['x2'])
-            self.assertEqual({'x1': h5['x1'], 'x2': h5['x2']}, h5['data'].coords())
+            self.assertEqual({'x1': h5['x1'], 'x2': h5['x2']}, h5['data'].coords)
 
     def test_isel_sel(self):
         with h5tbx.File() as h5:
             h5.create_dataset('time', data=[1, 2, 3], make_scale=True)
             h5.create_dataset('vel', data=[1.5, 2.5, 3.5], attach_scales='time')
             np.testing.assert_equal(h5['vel'].values[0:2], h5['vel'].isel(time=slice(0, 2)).values)
             self.assertEqual(3.5, float(h5['vel'].isel(time=2)))
@@ -694,14 +739,22 @@
             self.assertEqual(2.5, float(h5['vel'].sel(time=2.0)))
             with self.assertRaises(ValueError):
                 h5['vel'].sel(time=1.2)
             with self.assertRaises(NotImplementedError):
                 h5['vel'].sel(time=1.2, method='invalid')
             self.assertEqual(1.5, float(h5['vel'].sel(time=1.2, method='nearest')))
 
+    def test_isel_multiple_coords_per_axis(self):
+        with h5tbx.File() as h5:
+            h5.create_dataset('time', data=[1, 2, 3], make_scale=True)
+            h5.create_dataset('another_time', data=[1, 2, 3], make_scale=True)
+            h5.create_dataset('vel', data=[1.5, 2.5, 3.5], attach_scales=(('time', 'another_time'),))
+            v0 = h5.vel.isel(another_time=0)[()]
+            h5.dumps()
+
     def test_unit_conversion_interface(self):
         with h5tbx.File() as h5:
             h5.create_dataset('time', data=[1, 2, 3], attrs=dict(units='s'), make_scale=True)
             h5.create_dataset('vel', data=[1.5, 2.5, 3.5], attrs=dict(units='m/s'), attach_scales='time')
             # print(h5['vel'].to_units('m/s', time='h'))
             ret = h5['vel'].to_units('mm/s', time='h').sel(time=1.2, method='nearest')
             self.assertEqual(1.5 * 1000, float(ret))
@@ -723,15 +776,14 @@
             x = h5.create_dataset('x', data=ls(0, 10, 7), make_scale=True)
             h5.create_dataset('data',
                               shape=(10, 5, 7), attach_scales=('time', 'y', 'x'))
             np.testing.assert_equal(h5['data'][0, 0, [0, 2]],
                                     h5['data'].values[0, 0, [0, 2]])
             np.testing.assert_equal(h5['data'].isel(time=0, y=0, x=[0, 2]),
                                     h5['data'].values[0, 0, [0, 2]])
-            h5.dump()
 
         filename = h5.hdf_filename
 
         with h5tbx.File(filename) as h5:
             d = h5['data'].sel(
                 x=[4.3, 10.9],
                 time=0.2,
@@ -874,13 +926,13 @@
     def test_attr_group_link_and_xarray(self):
         with h5tbx.File() as h5:
             grp = h5.create_group('my_grp')
             ds = h5.create_dataset(name='ds', data=4)
 
             ds.attrs['link to grp'] = grp
 
-            self.assertIsInstance(ds.attrs['link to grp'], h5py.Group)
+            self.assertIsInstance(ds.attrs['link to grp'], str)
 
             da = ds[()]
             self.assertIsInstance(da, xr.DataArray)
             self.assertIsInstance(da.attrs['link to grp'], str)
             print(da)
```

### Comparing `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_dump.py` & `h5rdmtoolbox-1.3.1/tests/wrapper/test_dump.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_file.py` & `h5rdmtoolbox-1.3.1/tests/wrapper/test_file.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_h5ext.py` & `h5rdmtoolbox-1.3.1/tests/wrapper/test_h5ext.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_jsonld.py` & `h5rdmtoolbox-1.3.1/tests/wrapper/test_jsonld.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,20 @@
         logger.setLevel(LEVEL)
         for h in logger.handlers:
             h.setLevel(LEVEL)
 
     def tearDown(self):
         pathlib.Path('test.hdf').unlink(missing_ok=True)
 
+    def test_dump_type(self):
+        with h5tbx.File() as h5:
+            grp = h5.create_group('grp')
+            grp.rdf.type = 'https://example.org/MyGroup'
+            print(h5.dump_jsonld(indent=2))
+
     def test_build_node_list(self):
 
         g = rdflib.Graph()
         base_node = rdflib.BNode()
         g.add((base_node, rdflib.RDF.type, HDF5.Attribute))
         list_node_int = build_node_list(g, [1, 2, 3])
         g.add((base_node, HDF5.value, list_node_int))
```

### Comparing `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_lazy.py` & `h5rdmtoolbox-1.3.1/tests/wrapper/test_lazy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import unittest
 
 import h5rdmtoolbox as h5tbx
 
 
 class TestLazy(unittest.TestCase):
 
+    def test_lazy_on_datasets_with_coords(self):
+        with h5tbx.File() as h5:
+            h5.create_dataset('x', data=[-1, 0, 1], make_scale=True)
+            h5.create_dataset('y', data=5)
+            h5.create_dataset('time', data=[0, 1, 2], make_scale=True)
+            h5.create_dataset('data', data=[10, 20, 30],
+                              attach_scale=(('x', 'time'),))
+            h5.data.assign_coord(h5.y)
+            h5tbx.lazy(h5.data)
+
     def test_lazyObject(self):
         self.assertEqual(h5tbx.lazy(None), None)
 
         with self.assertRaises(TypeError):
             h5tbx.lazy(1)
 
         with h5tbx.File() as h5:
```

### Comparing `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_namespaces.py` & `h5rdmtoolbox-1.3.1/tests/wrapper/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_rdf.py` & `h5rdmtoolbox-1.3.1/tests/wrapper/test_rdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from ontolutils.namespacelib import M4I, OBO
 from rdflib import FOAF
 
 import h5rdmtoolbox as h5tbx
 from h5rdmtoolbox import Attribute
 from h5rdmtoolbox import jsonld
 from h5rdmtoolbox import use
+from h5rdmtoolbox.wrapper.h5attr import AttrDescriptionError
 from h5rdmtoolbox.wrapper.rdf import RDFError
 from h5rdmtoolbox.wrapper.rdf import RDF_PREDICATE_ATTR_NAME
-from h5rdmtoolbox.wrapper.h5attr import AttrDescriptionError
 
 
 class TestRDF(unittest.TestCase):
 
     def setUp(self) -> None:
         """setup"""
         use(None)
@@ -32,14 +32,26 @@
             h5.attrs['orcid', M4I.orcidId] = rdfobj
             self.assertEqual(h5.rdf.object['orcid'], 'https://orcid.org/0000-0001-8729-0482')
 
         self.assertEqual(rdfobj.__repr__(),
                          'Attribute(0000-0001-8729-0482, ' \
                          'rdf_object=https://orcid.org/0000-0001-8729-0482)')
 
+    def test_rdf_special_values(self):
+        """e.g. lists, ..."""
+        with h5tbx.File() as h5:
+            h5.attrs['flags'] = Attribute([1, 2, 3], rdf_predicate='https://example.org/hasFlags')
+            self.assertEqual(h5.rdf['flags'].predicate, 'https://example.org/hasFlags')
+            self.assertListEqual(list(h5.attrs['flags']), [1, 2, 3])
+
+        with h5tbx.File() as h5:
+            h5.attrs['flags'] = Attribute({'valid': 1, 'invalid': 2}, rdf_predicate='https://example.org/hasFlags')
+            self.assertEqual(h5.rdf['flags'].predicate, 'https://example.org/hasFlags')
+            self.assertDictEqual(h5.attrs['flags'], {'valid': 1, 'invalid': 2})
+
     def test_rdf_object_thing(self):
         """A RDF object can be an URI or RDF object or a ontolutils.Thing object.
         Idea behind it is to assign complex object through a single attribute, like a standard names that
         are defined in a standard name table and have no distinct IRI themselves
         """
 
         with h5tbx.File(mode='w') as h5:
@@ -236,15 +248,15 @@
             grp = h5.create_group('contact_person')
             grp.rdf.subject = FOAF.Person
 
             method_grp = h5.create_group('a_method')
             method_grp.rdf.subject = M4I.Method
             method_grp.attrs['has_participants', OBO.RO_0000057] = h5['contact_person']  # has participants
 
-            self.assertEqual(method_grp.attrs['has_participants'], h5['contact_person'])
+            self.assertEqual(method_grp.attrs['has_participants'], h5['contact_person'].name)
 
             grp.attrs['arbitrary'] = 'arbitrary'
             self.assertEqual(grp.rdf.predicate.get('arbitrary', 'invalid'), 'invalid')
 
             with self.assertRaises(KeyError):
                 grp.rdf.predicate['firstName'] = FOAF.firstName
             with self.assertRaises(KeyError):
```

### Comparing `h5rdmtoolbox-1.3.0a1/tests/wrapper/test_xr2df.py` & `h5rdmtoolbox-1.3.1/tests/wrapper/test_xr2df.py`

 * *Files identical despite different names*

