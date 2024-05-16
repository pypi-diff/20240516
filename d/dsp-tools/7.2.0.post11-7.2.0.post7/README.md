# Comparing `tmp/dsp_tools-7.2.0.post11.tar.gz` & `tmp/dsp_tools-7.2.0.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_tools-7.2.0.post11.tar", max compression
+gzip compressed data, was "dsp_tools-7.2.0.post7.tar", max compression
```

## Comparing `dsp_tools-7.2.0.post11.tar` & `dsp_tools-7.2.0.post7.tar`

### file list

```diff
@@ -1,118 +1,117 @@
--rw-r--r--   0        0        0    35149 2024-05-16 09:35:20.972461 dsp_tools-7.2.0.post11/LICENSE
--rw-r--r--   0        0        0     4941 2024-05-16 09:35:20.988461 dsp_tools-7.2.0.post11/docs/index.md
--rw-r--r--   0        0        0     8460 2024-05-16 09:35:53.320598 dsp_tools-7.2.0.post11/pyproject.toml
--rw-r--r--   0        0        0       41 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/cli/__init__.py
--rw-r--r--   0        0        0     8102 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/cli/call_action.py
--rw-r--r--   0        0        0    13719 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/cli/create_parsers.py
--rw-r--r--   0        0        0     9909 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/cli/entry_point.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/__init__.py
--rw-r--r--   0        0        0    15987 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/lists.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/models/__init__.py
--rw-r--r--   0        0        0    14898 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/models/input_error.py
--rw-r--r--   0        0        0     4018 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/models/list_node.py
--rw-r--r--   0        0        0      501 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/models/list_node_name.py
--rw-r--r--   0        0        0    29990 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/new_lists.py
--rw-r--r--   0        0        0     9829 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/project.py
--rw-r--r--   0        0        0    13571 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/properties.py
--rw-r--r--   0        0        0    11887 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/resources.py
--rw-r--r--   0        0        0    11866 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/utils.py
--rw-r--r--   0        0        0      466 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2xml/__init__.py
--rw-r--r--   0        0        0    21361 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
--rw-r--r--   0        0        0    80208 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
--rw-r--r--   0        0        0     1981 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2xml/propertyelement.py
--rw-r--r--   0        0        0     8275 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/id2iri.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/ingest_xmlupload/__init__.py
--rw-r--r--   0        0        0     2876 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
--rw-r--r--   0        0        0     2351 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
--rw-r--r--   0        0        0     4891 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/ingest_xmlupload/user_information.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/create/__init__.py
--rw-r--r--   0        0        0    45642 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/create/project_create.py
--rw-r--r--   0        0        0     8243 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/create/project_create_lists.py
--rw-r--r--   0        0        0    19703 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/create/project_validate.py
--rw-r--r--   0        0        0     5743 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/get.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/__init__.py
--rw-r--r--   0        0        0    12173 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/context.py
--rw-r--r--   0        0        0     8379 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/group.py
--rw-r--r--   0        0        0      850 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/helpers.py
--rw-r--r--   0        0        0    14910 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/listnode.py
--rw-r--r--   0        0        0      245 2024-05-16 09:35:20.992461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/model.py
--rw-r--r--   0        0        0    12710 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/ontology.py
--rw-r--r--   0        0        0    11594 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/project.py
--rw-r--r--   0        0        0      306 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/project_definition.py
--rw-r--r--   0        0        0    17215 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/propertyclass.py
--rw-r--r--   0        0        0    28164 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/resourceclass.py
--rw-r--r--   0        0        0    17030 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/user.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/resume_xmlupload/__init__.py
--rw-r--r--   0        0        0     3719 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
--rw-r--r--   0        0        0     4177 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/rosetta.py
--rw-r--r--   0        0        0    16102 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/start_stack.py
--rw-r--r--   0        0        0     1134 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/template.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/__init__.py
--rw-r--r--   0        0        0     2350 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/ark2iri.py
--rw-r--r--   0        0        0    10356 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
--rw-r--r--   0        0        0      625 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/iri_resolver.py
--rw-r--r--   0        0        0     3587 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/list_client.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/deserialise/__init__.py
--rw-r--r--   0        0        0     6448 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/deserialise/deserialise_value.py
--rw-r--r--   0        0        0     3560 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py
--rw-r--r--   0        0        0     5199 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/deserialise/xmlresource.py
--rw-r--r--   0        0        0     1334 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
--rw-r--r--   0        0        0     1551 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/namespace_context.py
--rw-r--r--   0        0        0     5549 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
--rw-r--r--   0        0        0     6752 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
--rw-r--r--   0        0        0     2388 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/permission.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/serialise/__init__.py
--rw-r--r--   0        0        0     1273 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/serialise/jsonld_serialiser.py
--rw-r--r--   0        0        0     1302 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/serialise/serialise_value.py
--rw-r--r--   0        0        0      812 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/sipi.py
--rw-r--r--   0        0        0      730 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/upload_state.py
--rw-r--r--   0        0        0     3466 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/ontology_client.py
--rw-r--r--   0        0        0     3135 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/project_client.py
--rw-r--r--   0        0        0     4653 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
--rw-r--r--   0        0        0    17072 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/resource_create_client.py
--rw-r--r--   0        0        0     4626 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/resource_multimedia.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/__init__.py
--rw-r--r--   0        0        0    12372 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
--rw-r--r--   0        0        0     2452 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/graph_models.py
--rw-r--r--   0        0        0     5754 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
--rw-r--r--   0        0        0     3375 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/stash_models.py
--rw-r--r--   0        0        0     4158 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
--rw-r--r--   0        0        0     7676 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
--rw-r--r--   0        0        0     2175 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/upload_config.py
--rw-r--r--   0        0        0      858 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
--rw-r--r--   0        0        0    18711 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/xmlupload.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/models/__init__.py
--rw-r--r--   0        0        0      949 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/models/custom_warnings.py
--rw-r--r--   0        0        0     2876 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/models/datetimestamp.py
--rw-r--r--   0        0        0     2785 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/models/exceptions.py
--rw-r--r--   0        0        0     8457 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/models/langstring.py
--rw-r--r--   0        0        0     1777 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/models/projectContext.py
--rw-r--r--   0        0        0        0 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/py.typed
--rw-r--r--   0        0        0     1488 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/0100-template-repo/template.json
--rw-r--r--   0        0        0     1036 2024-05-16 09:35:20.996461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/0100-template-repo/template.xml
--rw-r--r--   0        0        0    29742 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/data.xsd
--rw-r--r--   0        0        0     2770 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/lists-only.json
--rw-r--r--   0        0        0    42680 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/project.json
--rw-r--r--   0        0        0    32411 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/properties-only.json
--rw-r--r--   0        0        0     4240 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/resources-only.json
--rw-r--r--   0        0        0       61 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/start-stack/docker-compose.override.yml
--rw-r--r--   0        0        0     3281 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/start-stack/docker-compose.yml
--rw-r--r--   0        0        0      164 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/resources/start-stack/start-stack-config.yml
--rw-r--r--   0        0        0        0 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/__init__.py
--rw-r--r--   0        0        0     1030 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/connection.py
--rw-r--r--   0        0        0    14152 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/connection_live.py
--rw-r--r--   0        0        0     4554 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/date_util.py
--rw-r--r--   0        0        0      457 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/iri_util.py
--rw-r--r--   0        0        0     1157 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/logger_config.py
--rw-r--r--   0        0        0      705 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/set_encoder.py
--rw-r--r--   0        0        0     5754 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/shared.py
--rw-r--r--   0        0        0      547 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/uri_util.py
--rw-r--r--   0        0        0      978 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/warnings_config.py
--rw-r--r--   0        0        0     4920 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/xml_utils.py
--rw-r--r--   0        0        0     7359 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/xml_validation.py
--rw-r--r--   0        0        0     2312 2024-05-16 09:35:21.000461 dsp_tools-7.2.0.post11/src/dsp_tools/utils/xml_validation_models.py
--rw-r--r--   0        0        0     6389 1970-01-01 00:00:00.000000 dsp_tools-7.2.0.post11/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-14 11:55:58.687635 dsp_tools-7.2.0.post7/LICENSE
+-rw-r--r--   0        0        0     4941 2024-05-14 11:55:58.703635 dsp_tools-7.2.0.post7/docs/index.md
+-rw-r--r--   0        0        0     8406 2024-05-14 11:56:27.899950 dsp_tools-7.2.0.post7/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/__init__.py
+-rw-r--r--   0        0        0     8102 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/call_action.py
+-rw-r--r--   0        0        0    13719 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/create_parsers.py
+-rw-r--r--   0        0        0     9909 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/cli/entry_point.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/__init__.py
+-rw-r--r--   0        0        0    15987 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/lists.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/__init__.py
+-rw-r--r--   0        0        0    14898 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/input_error.py
+-rw-r--r--   0        0        0     4018 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/list_node.py
+-rw-r--r--   0        0        0      501 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/list_node_name.py
+-rw-r--r--   0        0        0    29990 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/new_lists.py
+-rw-r--r--   0        0        0     9829 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/project.py
+-rw-r--r--   0        0        0    13232 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/properties.py
+-rw-r--r--   0        0        0    11887 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/resources.py
+-rw-r--r--   0        0        0    11866 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/utils.py
+-rw-r--r--   0        0        0      466 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/__init__.py
+-rw-r--r--   0        0        0    21361 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_cli.py
+-rw-r--r--   0        0        0    80208 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_lib.py
+-rw-r--r--   0        0        0     1981 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/propertyelement.py
+-rw-r--r--   0        0        0     8275 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/id2iri.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/__init__.py
+-rw-r--r--   0        0        0     2876 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py
+-rw-r--r--   0        0        0     2351 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py
+-rw-r--r--   0        0        0     4891 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/user_information.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/__init__.py
+-rw-r--r--   0        0        0    45642 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create.py
+-rw-r--r--   0        0        0     8243 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create_lists.py
+-rw-r--r--   0        0        0    19703 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_validate.py
+-rw-r--r--   0        0        0     5743 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/get.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/__init__.py
+-rw-r--r--   0        0        0    12173 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/context.py
+-rw-r--r--   0        0        0     8379 2024-05-14 11:55:58.707635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/group.py
+-rw-r--r--   0        0        0      850 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/helpers.py
+-rw-r--r--   0        0        0    14910 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/listnode.py
+-rw-r--r--   0        0        0      245 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/model.py
+-rw-r--r--   0        0        0    12710 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/ontology.py
+-rw-r--r--   0        0        0    11594 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/project.py
+-rw-r--r--   0        0        0      306 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/project_definition.py
+-rw-r--r--   0        0        0    17215 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/propertyclass.py
+-rw-r--r--   0        0        0    28164 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/resourceclass.py
+-rw-r--r--   0        0        0    17030 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/user.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/resume_xmlupload/__init__.py
+-rw-r--r--   0        0        0     3719 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py
+-rw-r--r--   0        0        0     4177 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/rosetta.py
+-rw-r--r--   0        0        0    16102 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/start_stack.py
+-rw-r--r--   0        0        0     1134 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/template.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/__init__.py
+-rw-r--r--   0        0        0     2350 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ark2iri.py
+-rw-r--r--   0        0        0    10356 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py
+-rw-r--r--   0        0        0      625 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/iri_resolver.py
+-rw-r--r--   0        0        0     3587 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/list_client.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/__init__.py
+-rw-r--r--   0        0        0     6448 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/deserialise_value.py
+-rw-r--r--   0        0        0     3560 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py
+-rw-r--r--   0        0        0     5199 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlresource.py
+-rw-r--r--   0        0        0     1334 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py
+-rw-r--r--   0        0        0     1464 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/namespace_context.py
+-rw-r--r--   0        0        0     5549 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py
+-rw-r--r--   0        0        0     6752 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py
+-rw-r--r--   0        0        0     2388 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/permission.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/serialise/__init__.py
+-rw-r--r--   0        0        0     1302 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/serialise/serialise_value.py
+-rw-r--r--   0        0        0      812 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/sipi.py
+-rw-r--r--   0        0        0      730 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/upload_state.py
+-rw-r--r--   0        0        0     3466 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ontology_client.py
+-rw-r--r--   0        0        0     3140 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/project_client.py
+-rw-r--r--   0        0        0     4653 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py
+-rw-r--r--   0        0        0    14771 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_create_client.py
+-rw-r--r--   0        0        0     4626 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_multimedia.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/__init__.py
+-rw-r--r--   0        0        0    12372 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py
+-rw-r--r--   0        0        0     2452 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/graph_models.py
+-rw-r--r--   0        0        0     5754 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py
+-rw-r--r--   0        0        0     3375 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_models.py
+-rw-r--r--   0        0        0     4158 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py
+-rw-r--r--   0        0        0     7676 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py
+-rw-r--r--   0        0        0     2175 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/upload_config.py
+-rw-r--r--   0        0        0      858 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py
+-rw-r--r--   0        0        0    19191 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/xmlupload.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/__init__.py
+-rw-r--r--   0        0        0      949 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/custom_warnings.py
+-rw-r--r--   0        0        0     2876 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/datetimestamp.py
+-rw-r--r--   0        0        0     2785 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/exceptions.py
+-rw-r--r--   0        0        0     8457 2024-05-14 11:55:58.711635 dsp_tools-7.2.0.post7/src/dsp_tools/models/langstring.py
+-rw-r--r--   0        0        0     1777 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/models/projectContext.py
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/py.typed
+-rw-r--r--   0        0        0     1488 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.json
+-rw-r--r--   0        0        0     1036 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.xml
+-rw-r--r--   0        0        0    29742 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/data.xsd
+-rw-r--r--   0        0        0     2770 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/lists-only.json
+-rw-r--r--   0        0        0    42680 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/project.json
+-rw-r--r--   0        0        0    32411 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/properties-only.json
+-rw-r--r--   0        0        0     4240 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/resources-only.json
+-rw-r--r--   0        0        0       61 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/docker-compose.override.yml
+-rw-r--r--   0        0        0     3281 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/docker-compose.yml
+-rw-r--r--   0        0        0      164 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/start-stack-config.yml
+-rw-r--r--   0        0        0        0 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/__init__.py
+-rw-r--r--   0        0        0     1030 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection.py
+-rw-r--r--   0        0        0    14126 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection_live.py
+-rw-r--r--   0        0        0     4554 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/date_util.py
+-rw-r--r--   0        0        0      457 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/iri_util.py
+-rw-r--r--   0        0        0     1157 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/logger_config.py
+-rw-r--r--   0        0        0      705 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/set_encoder.py
+-rw-r--r--   0        0        0     5754 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/shared.py
+-rw-r--r--   0        0        0      547 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/uri_util.py
+-rw-r--r--   0        0        0      978 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/warnings_config.py
+-rw-r--r--   0        0        0     4920 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_utils.py
+-rw-r--r--   0        0        0     7359 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation.py
+-rw-r--r--   0        0        0     2312 2024-05-14 11:55:58.715635 dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation_models.py
+-rw-r--r--   0        0        0     6388 1970-01-01 00:00:00.000000 dsp_tools-7.2.0.post7/PKG-INFO
```

### Comparing `dsp_tools-7.2.0.post11/LICENSE` & `dsp_tools-7.2.0.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/docs/index.md` & `dsp_tools-7.2.0.post7/docs/index.md`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/pyproject.toml` & `dsp_tools-7.2.0.post7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # See https://packaging.python.org/en/latest/guides/writing-pyproject-toml/#writing-pyproject-toml
 
 [tool.poetry]
 name = "dsp-tools"
-version = "7.2.0.post11"
+version = "7.2.0.post7"
 description = "DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server."
 authors = ["DaSCH - Swiss National Data and Service Center for the Humanities <info@dasch.swiss>"]
 readme = "docs/index.md"
 license = "GPL-3.0-only"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
@@ -130,15 +130,14 @@
 # see https://docs.pytest.org/en/latest/explanation/goodpractices.html#tests-outside-application-code
 pythonpath = [".", "src", "test"]
 
 
 [tool.mypy]
 show_column_numbers = true
 strict = true
-enable_error_code = ["possibly-undefined"]
 exclude = [
     "src/dsp_tools/models/datetimestamp.py",                  # TODO: activate this
     "src/dsp_tools/models/langstring.py",                     # TODO: activate this
     "src/dsp_tools/models/projectContext.py",                 # TODO: activate this
     "src/dsp_tools/commands/project/models/context.py",       # TODO: activate this
     "src/dsp_tools/commands/project/models/group.py",         # TODO: activate this
     "src/dsp_tools/commands/project/models/helpers.py",       # TODO: activate this
@@ -148,15 +147,15 @@
     "src/dsp_tools/commands/project/models/propertyclass.py", # TODO: activate this
     "src/dsp_tools/commands/project/models/resourceclass.py", # TODO: activate this
     "src/dsp_tools/commands/project/models/user.py",          # TODO: activate this
 ]
 
 
 [[tool.mypy.overrides]]
-module = ["jsonpath_ng.*", "viztracer.*", "pyld.*"]  # For these packages, no type stubs are available yet
+module = ["jsonpath_ng.*", "viztracer.*"]  # For these packages, no type stubs are available yet
 ignore_missing_imports = true
 
 
 [tool.ruff]
 line-length = 120
 target-version = "py312"
```

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/cli/call_action.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/cli/call_action.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/cli/create_parsers.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/cli/create_parsers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/cli/entry_point.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/cli/entry_point.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/lists.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/models/input_error.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/input_error.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/models/list_node.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/models/list_node.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/new_lists.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/new_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/project.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/properties.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,32 +205,24 @@
     no_attribute_check = col_must_or_not_empty_based_on_other_col(
         df=df,
         substring_list=no_attributes,
         substring_colname="gui_element",
         check_empty_colname="gui_attributes",
         must_have_value=False,
     )
-    final_series = _get_final_series(mandatory_check, no_attribute_check)
-    return {"gui_attributes": final_series} if final_series is not None else None
-
-
-def _get_final_series(
-    mandatory_check: pd.Series[bool] | None, no_attribute_check: pd.Series[bool] | None
-) -> pd.Series[bool] | None:
-    final_series: pd.Series[bool] = pd.Series()
     match mandatory_check, no_attribute_check:
         case None, None:
             return None
         case pd.Series(), pd.Series():
-            final_series = pd.Series(np.logical_or(mandatory_check, no_attribute_check))  # type: ignore[arg-type]
+            final_series: pd.Series[bool] = pd.Series(np.logical_or(mandatory_check, no_attribute_check))  # type: ignore[arg-type]
         case pd.Series(), None:
             final_series = mandatory_check  # type: ignore[assignment]
-        case None, pd.Series():
-            final_series = no_attribute_check  # type: ignore[assignment]
-    return final_series
+        case None, pd.Series:
+            final_series = no_attribute_check
+    return {"gui_attributes": final_series}
 
 
 def _row2prop(df_row: pd.Series[Any], row_num: int, excelfile: str) -> dict[str, Any]:
     _property = {x: df_row[x] for x in mandatory_properties} | {
         "labels": get_labels(df_row=df_row),
         "super": [s.strip() for s in df_row["super"].split(",")],
     }
```

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/resources.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/resources.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2json/utils.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2json/utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2xml/excel2xml_cli.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_cli.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2xml/excel2xml_lib.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/excel2xml_lib.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/excel2xml/propertyelement.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/excel2xml/propertyelement.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/id2iri.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/id2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/apply_ingest_id.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/upload_xml.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/ingest_xmlupload/user_information.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/ingest_xmlupload/user_information.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/create/project_create.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/create/project_create_lists.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_create_lists.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/create/project_validate.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/create/project_validate.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/get.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/get.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/context.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/context.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/group.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/group.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/helpers.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/helpers.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/listnode.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/listnode.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/ontology.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/project.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/project.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/propertyclass.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/propertyclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/resourceclass.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/resourceclass.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/project/models/user.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/project/models/user.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/resume_xmlupload/resume_xmlupload.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/rosetta.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/rosetta.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/start_stack.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/start_stack.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/template.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/template.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/ark2iri.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ark2iri.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/check_consistency_with_ontology.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/iri_resolver.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/iri_resolver.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/list_client.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/list_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/deserialise/deserialise_value.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/deserialise_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlpermission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/deserialise/xmlresource.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/deserialise/xmlresource.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/formatted_text_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/namespace_context.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/namespace_context.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,20 @@
+from dataclasses import dataclass
+from dataclasses import field
+
 from rdflib.namespace import Namespace
 
 
+@dataclass
+class NamespaceContext:
+    onto_dict: dict[str, Namespace]
+    knora_api: Namespace = field(default=Namespace("http://api.knora.org/ontology/knora-api/v2#"))
+    salsah_gui: Namespace = field(default=Namespace("http://api.knora.org/ontology/salsah-gui/v2#"))
+
+
 def get_default_json_ld_context() -> dict[str, str]:
     """
     Returns the JSON-LD context as a dictionary.
 
     Returns:
         JSON-LD context as a dictionary.
     """
@@ -14,22 +24,14 @@
         "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
         "rdfs": "http://www.w3.org/2000/01/rdf-schema#",
         "owl": "http://www.w3.org/2002/07/owl#",
         "xsd": "http://www.w3.org/2001/XMLSchema#",
     }
 
 
-def make_namespace_dict_from_onto_names(ontos: dict[str, str]) -> dict[str, Namespace]:
-    """Provided a dictionary of ontology names and IRIs, returns a dictionary of Namespace objects."""
-    ontos = correct_project_context_namespaces(ontos)
-    namespaces = {k: Namespace(v) for k, v in ontos.items()}
-    namespaces.update({"knora-api": Namespace("http://api.knora.org/ontology/knora-api/v2#")})
-    return namespaces
-
-
 def correct_project_context_namespaces(ontos: dict[str, str]) -> dict[str, str]:
     """Add the hashtag to make it a valid namespace."""
     return {k: f"{v}#" for k, v in ontos.items()}
 
 
 def get_json_ld_context_for_project(ontos: dict[str, str]) -> dict[str, str]:
     """Provided a dictionary of ontology names and IRIs, returns a JSON-LD context for the project."""
```

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_lookup_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/ontology_problem_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/permission.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/permission.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/serialise/serialise_value.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/serialise/serialise_value.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/sipi.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/sipi.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/models/upload_state.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/models/upload_state.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/ontology_client.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/ontology_client.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/project_client.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/project_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,23 +54,22 @@
 def _get_project_info_from_server(con: Connection, shortcode: str) -> ProjectInfo:
     project_iri = _get_project_iri_from_server(con, shortcode)
     ontologies = _get_ontologies_from_server(con, project_iri)
     return ProjectInfo(project_iri=project_iri, ontology_iris=ontologies)
 
 
 def _get_project_iri_from_server(con: Connection, shortcode: str) -> str:
-    url = f"/admin/projects/shortcode/{shortcode}"
     try:
+        url = f"/admin/projects/shortcode/{shortcode}"
         res = con.get(url)
+        iri: str = res["project"]["id"]
     except BaseError as e:
         raise UserError(f"A project with shortcode {shortcode} could not be found on the DSP server") from e
-
-    iri: str | None = res.get("project", {}).get("id")
-    if not iri:
-        raise BaseError(f"Unexpected response from server: {res}")
+    except KeyError as e:
+        raise BaseError(f"Unexpected response from server: {res}") from e
     return iri
 
 
 def _get_ontologies_from_server(con: Connection, project_iri: str) -> list[str]:
     try:
         iri = quote_plus(project_iri)
         url = f"/v2/ontologies/metadata/{iri}"
```

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/read_validate_xml_file.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/resource_create_client.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_create_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,45 +2,34 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any
 from typing import assert_never
 from typing import cast
 
 from loguru import logger
-from rdflib import RDF
-from rdflib import BNode
-from rdflib import Graph
-from rdflib import Literal
-from rdflib import Namespace
-from rdflib import URIRef
 
 from dsp_tools.commands.xmlupload.ark2iri import convert_ark_v0_to_resource_iri
 from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
 from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLProperty
 from dsp_tools.commands.xmlupload.models.deserialise.deserialise_value import XMLValue
 from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import BitstreamInfo
 from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.models.formatted_text_value import FormattedTextValue
 from dsp_tools.commands.xmlupload.models.namespace_context import get_json_ld_context_for_project
-from dsp_tools.commands.xmlupload.models.namespace_context import make_namespace_dict_from_onto_names
 from dsp_tools.commands.xmlupload.models.permission import Permissions
-from dsp_tools.commands.xmlupload.models.serialise.jsonld_serialiser import serialise_property_graph
 from dsp_tools.commands.xmlupload.models.serialise.serialise_value import SerialiseProperty
 from dsp_tools.commands.xmlupload.models.serialise.serialise_value import SerialiseURI
 from dsp_tools.commands.xmlupload.models.serialise.serialise_value import SerialiseValue
 from dsp_tools.models.exceptions import BaseError
-from dsp_tools.models.exceptions import InputError
 from dsp_tools.models.exceptions import PermissionNotExistsError
 from dsp_tools.models.exceptions import UserError
 from dsp_tools.utils.connection import Connection
 from dsp_tools.utils.date_util import parse_date_string
 from dsp_tools.utils.iri_util import is_resource_iri
 
-KNORA_API = Namespace("http://api.knora.org/ontology/knora-api/v2#")
-
 
 @dataclass(frozen=True)
 class ResourceCreateClient:
     """client class that creates resources on a DSP server."""
 
     con: Connection
     project_iri: str
@@ -65,21 +54,19 @@
         return cast(str, res["@id"])
 
     def _make_resource_with_values(
         self,
         resource: XMLResource,
         bitstream_information: BitstreamInfo | None,
     ) -> dict[str, Any]:
-        res_bnode = BNode()
-        namespaces = make_namespace_dict_from_onto_names(self.project_onto_dict)
         res = self._make_resource(
             resource=resource,
             bitstream_information=bitstream_information,
         )
-        vals = self._make_values(resource, res_bnode, namespaces)
+        vals = self._make_values(resource)
         res.update(vals)
         return res
 
     def _make_resource(
         self,
         resource: XMLResource,
         bitstream_information: BitstreamInfo | None,
@@ -108,53 +95,38 @@
                 "@type": "xsd:dateTimeStamp",
                 "@value": str(resource.creation_date),
             }
         if bitstream_information:
             res.update(_make_bitstream_file_value(bitstream_information))
         return res
 
-    def _make_values(self, resource: XMLResource, res_bnode: BNode, namespaces: dict[str, Namespace]) -> dict[str, Any]:
+    def _make_values(self, resource: XMLResource) -> dict[str, Any]:
         def prop_name(p: XMLProperty) -> str:
             if p.valtype != "resptr":
                 return p.name
             elif p.name == "knora-api:isSegmentOf" and resource.restype == "knora-api:VideoSegment":
                 return "knora-api:isVideoSegmentOfValue"
             elif p.name == "knora-api:isSegmentOf" and resource.restype == "knora-api:AudioSegment":
                 return "knora-api:isAudioSegmentOfValue"
             else:
                 return f"{p.name}Value"
 
         def make_values(p: XMLProperty) -> list[dict[str, Any]]:
             return [self._make_value(v, p.valtype) for v in p.values]
 
         properties_serialised = {}
-        properties_graph = Graph()
-        last_prop_name = None
 
         for prop in resource.properties:
             match prop.valtype:
                 case "uri":
                     properties_serialised.update(_serialise_uri_prop(prop, self.permissions_lookup))
-                case "integer":
-                    int_prop_name = self._get_absolute_prop_iri(prop.name, namespaces)
-                    int_graph = _make_integer_prop(prop, res_bnode, int_prop_name, self.permissions_lookup)
-                    properties_graph += int_graph
-                    last_prop_name = int_prop_name
                 case _:
                     properties_serialised.update({prop_name(prop): make_values(prop)})
-        if last_prop_name:
-            serialised_graph_props = serialise_property_graph(properties_graph, last_prop_name)
-            properties_serialised.update(serialised_graph_props)
-        return properties_serialised
 
-    def _get_absolute_prop_iri(self, prefixed_prop: str, namespaces: dict[str, Namespace]) -> URIRef:
-        prefix, prop = prefixed_prop.split(":", maxsplit=1)
-        if not (namespace := namespaces.get(prefix)):
-            raise InputError(f"Could not find namespace for prefix: {prefix}")
-        return namespace[prop]
+        return properties_serialised
 
     def _make_value(self, value: XMLValue, value_type: str) -> dict[str, Any]:
         match value_type:
             case "boolean":
                 res = _make_boolean_value(value)
             case "color":
                 res = _make_color_value(value)
@@ -162,14 +134,16 @@
                 res = _make_date_value(value)
             case "decimal":
                 res = _make_decimal_value(value)
             case "geometry":
                 res = _make_geometry_value(value)
             case "geoname":
                 res = _make_geoname_value(value)
+            case "integer":
+                res = _make_integer_value(value)
             case "interval":
                 res = _make_interval_value(value)
             case "resptr":
                 res = _make_link_value(value, self.iri_resolver)
             case "list":
                 res = _make_list_value(value, self.listnode_lookup)
             case "text":
@@ -298,37 +272,20 @@
 def _make_geoname_value(value: XMLValue) -> dict[str, Any]:
     return {
         "@type": "knora-api:GeonameValue",
         "knora-api:geonameValueAsGeonameCode": value.value,
     }
 
 
-def _make_integer_prop(
-    prop: XMLProperty, res_bn: BNode, prop_name: URIRef, permissions_lookup: dict[str, Permissions]
-) -> Graph:
-    g = Graph()
-    for value in prop.values:
-        single_val_bn = BNode()
-        g.add((res_bn, prop_name, single_val_bn))
-        g += _make_integer_value(value, single_val_bn, permissions_lookup)
-    return g
-
-
-def _make_integer_value(value: XMLValue, val_bn: BNode, permissions_lookup: dict[str, Permissions]) -> Graph:
+def _make_integer_value(value: XMLValue) -> dict[str, Any]:
     s = _assert_is_string(value.value)
-    g = Graph()
-    g.add((val_bn, RDF.type, KNORA_API.IntValue))
-    g.add((val_bn, KNORA_API.intValueAsInt, Literal(int(s))))
-    if value.permissions:
-        if not (per := permissions_lookup.get(value.permissions)):
-            raise PermissionNotExistsError(f"Could not find permissions for value: {value.permissions}")
-        g.add((val_bn, KNORA_API.hasPermissions, Literal(str(per))))
-    if value.comment:
-        g.add((val_bn, KNORA_API.valueHasComment, Literal(value.comment)))
-    return g
+    return {
+        "@type": "knora-api:IntValue",
+        "knora-api:intValueAsInt": int(s),
+    }
 
 
 def _make_interval_value(value: XMLValue) -> dict[str, Any]:
     s = _assert_is_string(value.value)
     match s.split(":", 1):
         case [start, end]:
             return {
```

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/resource_multimedia.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/resource_multimedia.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/construct_and_analyze_graph.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/graph_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/graph_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_circular_references.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/stash_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/stash_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_resptr_props.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/stash/upload_stashed_xml_texts.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/upload_config.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/upload_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/write_diagnostic_info.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/commands/xmlupload/xmlupload.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/commands/xmlupload/xmlupload.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from lxml import etree
 
 from dsp_tools.commands.xmlupload.check_consistency_with_ontology import do_xml_consistency_check_with_ontology
 from dsp_tools.commands.xmlupload.iri_resolver import IriResolver
 from dsp_tools.commands.xmlupload.list_client import ListClient
 from dsp_tools.commands.xmlupload.list_client import ListClientLive
 from dsp_tools.commands.xmlupload.models.deserialise.xmlpermission import XmlPermission
+from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import BitstreamInfo
 from dsp_tools.commands.xmlupload.models.deserialise.xmlresource import XMLResource
 from dsp_tools.commands.xmlupload.models.namespace_context import get_json_ld_context_for_project
 from dsp_tools.commands.xmlupload.models.permission import Permissions
 from dsp_tools.commands.xmlupload.models.sipi import Sipi
 from dsp_tools.commands.xmlupload.models.upload_state import UploadState
 from dsp_tools.commands.xmlupload.ontology_client import OntologyClientLive
 from dsp_tools.commands.xmlupload.project_client import ProjectClient
@@ -328,32 +329,28 @@
         )
         if not success:
             upload_state.failed_uploads.append(resource.res_id)
             return
     except KeyboardInterrupt:
         raise XmlUploadInterruptedError("KeyboardInterrupt during media file upload") from None
 
-    iri = None
     try:
-        iri = resource_create_client.create_resource(resource, media_info)
+        iri = _create_resource(resource, media_info, resource_create_client)
     except (PermanentTimeOutError, KeyboardInterrupt) as err:
         warnings.warn(DspToolsUserWarning(f"{type(err).__name__}: Tidying up, then exit..."))
         msg = (
             f"There was a {type(err).__name__} while trying to create resource '{resource.res_id}'.\n"
             f"It is unclear if the resource '{resource.res_id}' was created successfully or not.\n"
             f"Please check manually in the DSP-APP or DB.\n"
             f"In case of successful creation, call 'resume-xmlupload' with the flag "
             f"'--skip-first-resource' to prevent duplication.\n"
             f"If not, a normal 'resume-xmlupload' can be started."
         )
         logger.error(msg)
         raise XmlUploadInterruptedError(msg) from None
-    except Exception as err:  # noqa: BLE001 (blind-except)
-        err_msg = err.message if isinstance(err, BaseError) else None
-        _handle_resource_creation_failure(resource, err_msg)
 
     try:
         _tidy_up_resource_creation_idempotent(upload_state, iri, resource)
         _interrupt_if_indicated(upload_state, creation_attempts_of_this_round)
     except KeyboardInterrupt:
         warnings.warn(DspToolsUserWarning("KeyboardInterrupt: Tidying up, then exit..."))
         _tidy_up_resource_creation_idempotent(upload_state, iri, resource)
@@ -389,25 +386,38 @@
         if resource.res_id not in upload_state.failed_uploads:
             upload_state.failed_uploads.append(resource.res_id)
 
     if resource in upload_state.pending_resources:
         upload_state.pending_resources.remove(resource)
 
 
-def _handle_resource_creation_failure(resource: XMLResource, err_msg: str | None) -> None:
-    msg = f"{datetime.now()}: WARNING: Unable to create resource '{resource.label}' (ID: '{resource.res_id}')"
-    if err_msg:
-        msg = f"{msg}: {err_msg}"
-    print(msg)
-    log_msg = (
-        f"Unable to create resource '{resource.label}' ({resource.res_id})\n"
-        f"Resource details:\n{vars(resource)}\n"
-        f"Property details:\n" + "\n".join([str(vars(prop)) for prop in resource.properties])
-    )
-    logger.exception(log_msg)
+def _create_resource(
+    resource: XMLResource,
+    bitstream_information: BitstreamInfo | None,
+    resource_create_client: ResourceCreateClient,
+) -> str | None:
+    try:
+        return resource_create_client.create_resource(resource, bitstream_information)
+    except PermanentTimeOutError as err:
+        # The following block catches all exceptions and handles them in a generic way.
+        # Because the calling function needs to know that this was a PermanentTimeOutError, we need to catch and
+        # raise it here.
+        raise err
+    except Exception as err:  # noqa: BLE001 (blind-except)
+        msg = f"{datetime.now()}: WARNING: Unable to create resource '{resource.label}' (ID: '{resource.res_id}')"
+        if isinstance(err, BaseError):
+            msg = f"{msg}: {err.message}"
+        print(msg)
+        log_msg = (
+            f"Unable to create resource '{resource.label}' ({resource.res_id})\n"
+            f"Resource details:\n{vars(resource)}\n"
+            f"Property details:\n" + "\n".join([str(vars(prop)) for prop in resource.properties])
+        )
+        logger.exception(log_msg)
+        return None
 
 
 def _handle_upload_error(err: BaseException, upload_state: UploadState) -> None:
     """
     In case the xmlupload must be interrupted,
     e.g. because of an error that could not be handled,
     or due to keyboard interrupt,
```

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/models/custom_warnings.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/custom_warnings.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/models/datetimestamp.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/datetimestamp.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/models/exceptions.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/models/langstring.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/langstring.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/models/projectContext.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/models/projectContext.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/resources/0100-template-repo/template.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/resources/0100-template-repo/template.xml` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/0100-template-repo/template.xml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/data.xsd` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/data.xsd`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/lists-only.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/lists-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/project.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/project.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/properties-only.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/properties-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/resources/schema/resources-only.json` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/schema/resources-only.json`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/resources/start-stack/docker-compose.yml` & `dsp_tools-7.2.0.post7/src/dsp_tools/resources/start-stack/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/connection.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/connection_live.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/connection_live.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from dataclasses import dataclass
 from dataclasses import field
 from datetime import datetime
 from functools import partial
 from importlib.metadata import version
 from typing import Any
 from typing import Literal
-from typing import Never
 from typing import Optional
 from typing import cast
 
 import regex
 from loguru import logger
 from requests import ReadTimeout
 from requests import RequestException
@@ -311,15 +310,15 @@
         print(f"{datetime.now()}: {msg}")
         if exc_info:
             logger.opt(exception=True).error(f"{msg} ({retry_counter=:})")
         else:
             logger.error(f"{msg} ({retry_counter=:})")
         time.sleep(2**retry_counter)
 
-    def _log_and_raise_timeouts(self, error: TimeoutError | ReadTimeout) -> Never:
+    def _log_and_raise_timeouts(self, error: TimeoutError | ReadTimeout) -> None:
         msg = f"A '{error.__class__.__name__}' occurred during the connection to the DSP server."
         print(f"{datetime.now()}: {msg}")
         logger.exception(msg)
         raise PermanentTimeOutError(msg) from None
 
     def _log_response(self, response: Response) -> None:
         dumpobj: dict[str, Any] = {
```

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/date_util.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/date_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/logger_config.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/logger_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/set_encoder.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/set_encoder.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/shared.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/shared.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/uri_util.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/uri_util.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/warnings_config.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/warnings_config.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/xml_utils.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/xml_validation.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/src/dsp_tools/utils/xml_validation_models.py` & `dsp_tools-7.2.0.post7/src/dsp_tools/utils/xml_validation_models.py`

 * *Files identical despite different names*

### Comparing `dsp_tools-7.2.0.post11/PKG-INFO` & `dsp_tools-7.2.0.post7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-tools
-Version: 7.2.0.post11
+Version: 7.2.0.post7
 Summary: DSP-TOOLS is a Python package with a command line interface that helps you interact with a DaSCH service platform (DSP) server.
 Home-page: https://www.dasch.swiss/
 License: GPL-3.0-only
 Author: DaSCH - Swiss National Data and Service Center for the Humanities
 Author-email: info@dasch.swiss
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

