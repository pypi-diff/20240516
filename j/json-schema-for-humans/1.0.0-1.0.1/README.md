# Comparing `tmp/json_schema_for_humans-1.0.0.tar.gz` & `tmp/json_schema_for_humans-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_schema_for_humans-1.0.0.tar", max compression
+gzip compressed data, was "json_schema_for_humans-1.0.1.tar", max compression
```

## Comparing `json_schema_for_humans-1.0.0.tar` & `json_schema_for_humans-1.0.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0      560 2024-05-03 20:42:56.131221 json_schema_for_humans-1.0.0/LICENSE.md
--rw-r--r--   0        0        0    10150 2024-05-03 20:42:56.131221 json_schema_for_humans-1.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/__init__.py
--rw-r--r--   0        0        0     3990 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/cli.py
--rw-r--r--   0        0        0     1911 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/const.py
--rw-r--r--   0        0        0     6086 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/generate.py
--rw-r--r--   0        0        0     7505 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/generation_configuration.py
--rw-r--r--   0        0        0     8592 2024-05-03 20:42:56.159222 json_schema_for_humans-1.0.0/json_schema_for_humans/jinja_filters.py
--rw-r--r--   0        0        0    18895 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/md_template.py
--rw-r--r--   0        0        0        0 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/__init__.py
--rw-r--r--   0        0        0    30645 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/intermediate_representation.py
--rw-r--r--   0        0        0     3323 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_importer.py
--rw-r--r--   0        0        0      970 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_keyword.py
--rw-r--r--   0        0        0    23120 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_node.py
--rw-r--r--   0        0        0     2987 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_to_render.py
--rw-r--r--   0        0        0     3588 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/template_renderer.py
--rw-r--r--   0        0        0      799 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/badge_type.html
--rw-r--r--   0        0        0     1162 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/base.html
--rw-r--r--   0        0        0      673 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/breadcrumbs.html
--rw-r--r--   0        0        0     4563 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/content.html
--rw-r--r--   0        0        0      210 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/macro_restriction.html
--rw-r--r--   0        0        0     6357 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/schema_doc.css
--rw-r--r--   0        0        0     1994 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_array.html
--rw-r--r--   0        0        0     1886 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_conditional_subschema.html
--rw-r--r--   0        0        0      529 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_description.html
--rw-r--r--   0        0        0      823 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_examples.html
--rw-r--r--   0        0        0      186 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_not.html
--rw-r--r--   0        0        0     2057 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_properties.html
--rw-r--r--   0        0        0      451 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_undocumented_required_properties.html
--rw-r--r--   0        0        0      707 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/tabbed_section.html
--rw-r--r--   0        0        0      799 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/badge_type.html
--rw-r--r--   0        0        0     2017 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/base.html
--rw-r--r--   0        0        0      716 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/breadcrumbs.html
--rw-r--r--   0        0        0     4862 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/content.html
--rw-r--r--   0        0        0      210 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/macro_restriction.html
--rw-r--r--   0        0        0     6415 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.css
--rw-r--r--   0        0        0     2567 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.js
--rw-r--r--   0        0        0     1259 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.min.js
--rw-r--r--   0        0        0     1990 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_array.html
--rw-r--r--   0        0        0     2038 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_conditional_subschema.html
--rw-r--r--   0        0        0      652 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_description.html
--rw-r--r--   0        0        0      823 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_examples.html
--rw-r--r--   0        0        0      186 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_not.html
--rw-r--r--   0        0        0     2824 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_properties.html
--rw-r--r--   0        0        0      451 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_undocumented_required_properties.html
--rw-r--r--   0        0        0     1141 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/tabbed_section.html
--rw-r--r--   0        0        0      799 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/badge_type.html
--rw-r--r--   0        0        0     1560 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/base.html
--rw-r--r--   0        0        0      716 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/breadcrumbs.html
--rw-r--r--   0        0        0     4946 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/content.html
--rw-r--r--   0        0        0   155758 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/css/bootstrap-4.3.1.min.css
--rw-r--r--   0        0        0     6411 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/css/overpass300,400,600,800.css
--rw-r--r--   0        0        0     6415 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/css/schema_doc.css
--rw-r--r--   0        0        0    27348 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GhU9vyww.woff2
--rw-r--r--   0        0        0    38720 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GlU9s.woff2
--rw-r--r--   0        0        0    16688 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GoU9vyww.woff2
--rw-r--r--   0        0        0     7480 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GqU9vyww.woff2
--rw-r--r--   0        0        0    37468 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GrU9vyww.woff2
--rw-r--r--   0        0        0    58072 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/js/bootstrap-4.3.1.min.js
--rw-r--r--   0        0        0    88145 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/js/jquery-3.4.1.min.js
--rw-r--r--   0        0        0     1259 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/js/schema_doc.min.js
--rw-r--r--   0        0        0      210 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/macro_restriction.html
--rw-r--r--   0        0        0     1990 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_array.html
--rw-r--r--   0        0        0     2038 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_conditional_subschema.html
--rw-r--r--   0        0        0      652 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_description.html
--rw-r--r--   0        0        0      823 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_examples.html
--rw-r--r--   0        0        0      186 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_not.html
--rw-r--r--   0        0        0     2824 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_properties.html
--rw-r--r--   0        0        0      451 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_undocumented_required_properties.html
--rw-r--r--   0        0        0     1141 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/tabbed_section.html
--rw-r--r--   0        0        0      616 2024-05-03 20:42:56.163221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/base.md
--rw-r--r--   0        0        0      287 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/breadcrumbs.md
--rw-r--r--   0        0        0     3122 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/content.md
--rw-r--r--   0        0        0     1436 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_array.md
--rw-r--r--   0        0        0      951 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_conditional_subschema.md
--rw-r--r--   0        0        0      101 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_description.md
--rw-r--r--   0        0        0      479 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_examples.md
--rw-r--r--   0        0        0      177 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_not.md
--rw-r--r--   0        0        0      125 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_one_of.md
--rw-r--r--   0        0        0     1323 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_properties_details.md
--rw-r--r--   0        0        0      314 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_undocumented_required_properties.md
--rw-r--r--   0        0        0      446 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/tabbed_section.md
--rw-r--r--   0        0        0      615 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/base.md
--rw-r--r--   0        0        0      306 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/breadcrumbs.md
--rw-r--r--   0        0        0     3031 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/content.md
--rw-r--r--   0        0        0     1436 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_array.md
--rw-r--r--   0        0        0      951 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_conditional_subschema.md
--rw-r--r--   0        0        0      101 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_description.md
--rw-r--r--   0        0        0      190 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_examples.md
--rw-r--r--   0        0        0      177 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_not.md
--rw-r--r--   0        0        0      125 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_one_of.md
--rw-r--r--   0        0        0     1400 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_properties_details.md
--rw-r--r--   0        0        0      314 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_undocumented_required_properties.md
--rw-r--r--   0        0        0      504 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/tabbed_section.md
--rw-r--r--   0        0        0     3786 2024-05-03 20:42:56.167221 json_schema_for_humans-1.0.0/json_schema_for_humans/templating_utils.py
--rw-r--r--   0        0        0     1875 2024-05-03 20:43:14.543290 json_schema_for_humans-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11651 1970-01-01 00:00:00.000000 json_schema_for_humans-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      560 2024-05-06 17:52:24.821240 json_schema_for_humans-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0    10150 2024-05-06 17:52:24.821240 json_schema_for_humans-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/__init__.py
+-rw-r--r--   0        0        0     3990 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/cli.py
+-rw-r--r--   0        0        0     1911 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/const.py
+-rw-r--r--   0        0        0     6086 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/generate.py
+-rw-r--r--   0        0        0     7505 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/generation_configuration.py
+-rw-r--r--   0        0        0     8592 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/jinja_filters.py
+-rw-r--r--   0        0        0    18895 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/md_template.py
+-rw-r--r--   0        0        0        0 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/schema/__init__.py
+-rw-r--r--   0        0        0    30645 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/schema/intermediate_representation.py
+-rw-r--r--   0        0        0     3323 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/schema/schema_importer.py
+-rw-r--r--   0        0        0      970 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/schema/schema_keyword.py
+-rw-r--r--   0        0        0    23120 2024-05-06 17:52:24.849240 json_schema_for_humans-1.0.1/json_schema_for_humans/schema/schema_node.py
+-rw-r--r--   0        0        0     2987 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/schema/schema_to_render.py
+-rw-r--r--   0        0        0     3588 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/template_renderer.py
+-rw-r--r--   0        0        0      799 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/badge_type.html
+-rw-r--r--   0        0        0     1162 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/base.html
+-rw-r--r--   0        0        0      673 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/breadcrumbs.html
+-rw-r--r--   0        0        0     4563 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/content.html
+-rw-r--r--   0        0        0      210 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/macro_restriction.html
+-rw-r--r--   0        0        0     6357 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/schema_doc.css
+-rw-r--r--   0        0        0     1994 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_array.html
+-rw-r--r--   0        0        0     1886 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_conditional_subschema.html
+-rw-r--r--   0        0        0      529 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_description.html
+-rw-r--r--   0        0        0      823 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_examples.html
+-rw-r--r--   0        0        0      186 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_not.html
+-rw-r--r--   0        0        0     2057 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_properties.html
+-rw-r--r--   0        0        0      451 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_undocumented_required_properties.html
+-rw-r--r--   0        0        0      707 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/tabbed_section.html
+-rw-r--r--   0        0        0      799 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/badge_type.html
+-rw-r--r--   0        0        0     2017 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/base.html
+-rw-r--r--   0        0        0      716 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/breadcrumbs.html
+-rw-r--r--   0        0        0     4862 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/content.html
+-rw-r--r--   0        0        0      210 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/macro_restriction.html
+-rw-r--r--   0        0        0     6415 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/schema_doc.css
+-rw-r--r--   0        0        0     2567 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/schema_doc.js
+-rw-r--r--   0        0        0     1259 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/schema_doc.min.js
+-rw-r--r--   0        0        0     1990 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_array.html
+-rw-r--r--   0        0        0     2038 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_conditional_subschema.html
+-rw-r--r--   0        0        0      652 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_description.html
+-rw-r--r--   0        0        0      823 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_examples.html
+-rw-r--r--   0        0        0      186 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_not.html
+-rw-r--r--   0        0        0     2824 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_properties.html
+-rw-r--r--   0        0        0      451 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_undocumented_required_properties.html
+-rw-r--r--   0        0        0     1141 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/tabbed_section.html
+-rw-r--r--   0        0        0      799 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/badge_type.html
+-rw-r--r--   0        0        0     1560 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/base.html
+-rw-r--r--   0        0        0      716 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/breadcrumbs.html
+-rw-r--r--   0        0        0     4946 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/content.html
+-rw-r--r--   0        0        0   155758 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/css/bootstrap-4.3.1.min.css
+-rw-r--r--   0        0        0     6411 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/css/overpass300,400,600,800.css
+-rw-r--r--   0        0        0     6415 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/css/schema_doc.css
+-rw-r--r--   0        0        0    27348 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GhU9vyww.woff2
+-rw-r--r--   0        0        0    38720 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GlU9s.woff2
+-rw-r--r--   0        0        0    16688 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GoU9vyww.woff2
+-rw-r--r--   0        0        0     7480 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GqU9vyww.woff2
+-rw-r--r--   0        0        0    37468 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GrU9vyww.woff2
+-rw-r--r--   0        0        0    58072 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/js/bootstrap-4.3.1.min.js
+-rw-r--r--   0        0        0    88145 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/js/jquery-3.4.1.min.js
+-rw-r--r--   0        0        0     1259 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/js/schema_doc.min.js
+-rw-r--r--   0        0        0      210 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/macro_restriction.html
+-rw-r--r--   0        0        0     1990 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_array.html
+-rw-r--r--   0        0        0     2038 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_conditional_subschema.html
+-rw-r--r--   0        0        0      652 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_description.html
+-rw-r--r--   0        0        0      823 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_examples.html
+-rw-r--r--   0        0        0      186 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_not.html
+-rw-r--r--   0        0        0     2824 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_properties.html
+-rw-r--r--   0        0        0      451 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_undocumented_required_properties.html
+-rw-r--r--   0        0        0     1141 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/tabbed_section.html
+-rw-r--r--   0        0        0      616 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/base.md
+-rw-r--r--   0        0        0      287 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/breadcrumbs.md
+-rw-r--r--   0        0        0     3122 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/content.md
+-rw-r--r--   0        0        0     1436 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_array.md
+-rw-r--r--   0        0        0      951 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_conditional_subschema.md
+-rw-r--r--   0        0        0      101 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_description.md
+-rw-r--r--   0        0        0      479 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_examples.md
+-rw-r--r--   0        0        0      177 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_not.md
+-rw-r--r--   0        0        0      125 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_one_of.md
+-rw-r--r--   0        0        0     1323 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_properties_details.md
+-rw-r--r--   0        0        0      314 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_undocumented_required_properties.md
+-rw-r--r--   0        0        0      446 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/tabbed_section.md
+-rw-r--r--   0        0        0      615 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/base.md
+-rw-r--r--   0        0        0      306 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/breadcrumbs.md
+-rw-r--r--   0        0        0     3031 2024-05-06 17:52:24.853240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/content.md
+-rw-r--r--   0        0        0     1436 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_array.md
+-rw-r--r--   0        0        0      951 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_conditional_subschema.md
+-rw-r--r--   0        0        0      101 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_description.md
+-rw-r--r--   0        0        0      190 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_examples.md
+-rw-r--r--   0        0        0      177 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_not.md
+-rw-r--r--   0        0        0      125 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_one_of.md
+-rw-r--r--   0        0        0     1400 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_properties_details.md
+-rw-r--r--   0        0        0      314 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_undocumented_required_properties.md
+-rw-r--r--   0        0        0      504 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/tabbed_section.md
+-rw-r--r--   0        0        0     3786 2024-05-06 17:52:24.857240 json_schema_for_humans-1.0.1/json_schema_for_humans/templating_utils.py
+-rw-r--r--   0        0        0     1874 2024-05-06 17:52:55.709447 json_schema_for_humans-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11469 1970-01-01 00:00:00.000000 json_schema_for_humans-1.0.1/PKG-INFO
```

### Comparing `json_schema_for_humans-1.0.0/LICENSE.md` & `json_schema_for_humans-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/README.md` & `json_schema_for_humans-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/cli.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/cli.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/const.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/const.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/generate.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/generate.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/generation_configuration.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/generation_configuration.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/jinja_filters.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/jinja_filters.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/md_template.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/md_template.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/schema/intermediate_representation.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/schema/intermediate_representation.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_importer.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/schema/schema_importer.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_keyword.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/schema/schema_keyword.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_node.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/schema/schema_node.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/schema/schema_to_render.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/schema/schema_to_render.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/template_renderer.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/template_renderer.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/badge_type.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/badge_type.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/base.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/base.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/breadcrumbs.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/content.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/content.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/schema_doc.css` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/schema_doc.css`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_array.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_array.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_conditional_subschema.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_conditional_subschema.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_description.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_description.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_examples.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_examples.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/section_properties.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/section_properties.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/flat/tabbed_section.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/flat/tabbed_section.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/badge_type.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/badge_type.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/base.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/base.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/breadcrumbs.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/content.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/content.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.css` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/schema_doc.css`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.js` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/schema_doc.js`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/schema_doc.min.js` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_array.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_array.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_conditional_subschema.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_conditional_subschema.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_description.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_description.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_examples.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_examples.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/section_properties.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/section_properties.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js/tabbed_section.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js/tabbed_section.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/badge_type.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/badge_type.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/base.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/base.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/breadcrumbs.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/content.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/content.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/css/bootstrap-4.3.1.min.css` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/css/bootstrap-4.3.1.min.css`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/css/overpass300,400,600,800.css` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/css/overpass300,400,600,800.css`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/css/schema_doc.css` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/css/schema_doc.css`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GhU9vyww.woff2` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GhU9vyww.woff2`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GlU9s.woff2` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GlU9s.woff2`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GoU9vyww.woff2` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GoU9vyww.woff2`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GqU9vyww.woff2` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GqU9vyww.woff2`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GrU9vyww.woff2` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/font/qFdH35WCmI96Ajtm81GrU9vyww.woff2`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/js/bootstrap-4.3.1.min.js` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/js/bootstrap-4.3.1.min.js`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/js/jquery-3.4.1.min.js` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/js/schema_doc.min.js` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/js/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_array.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_array.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_conditional_subschema.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_conditional_subschema.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_description.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_description.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_examples.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_examples.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/section_properties.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/section_properties.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/js_offline/tabbed_section.html` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/js_offline/tabbed_section.html`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/base.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/base.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/content.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/content.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_array.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_array.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_conditional_subschema.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_conditional_subschema.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md/section_properties_details.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md/section_properties_details.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/base.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/base.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/content.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/content.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_array.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_array.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_conditional_subschema.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_conditional_subschema.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templates/md_nested/section_properties_details.md` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templates/md_nested/section_properties_details.md`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/json_schema_for_humans/templating_utils.py` & `json_schema_for_humans-1.0.1/json_schema_for_humans/templating_utils.py`

 * *Files identical despite different names*

### Comparing `json_schema_for_humans-1.0.0/pyproject.toml` & `json_schema_for_humans-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json-schema-for-humans"
-version = "1.0.0"
+version = "1.0.1"
 description = "Generate static HTML documentation from JSON schemas"
 authors = ["Denis Blanchette <tools@coveo.com>", "AbdulRahman Al Hamali <tools@coveo.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/coveooss/json-schema-for-humans"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -30,31 +30,30 @@
 Jinja2 = ">3"
 markdown2 = "^2.4.1"
 Pygments = "^2.10.0"
 pytz = "*"
 PyYAML = ">=5.4.1,<7"
 requests = "^2.31.0"
 MarkupSafe = "^2.0"
-types-beautifulsoup4 = "^4.12.0.20240229"
-types-pyyaml = "^6.0.12.20240311"
-types-pytz = "^2024.1.0.20240417"
-
 
 
 [tool.poetry.scripts]
 generate-schema-doc = "json_schema_for_humans.cli:main"
 
 
 [tool.poetry.group.dev.dependencies]
 beautifulsoup4 = "^4.10.0"
 black = "^22.10"
 pytest = "^6.2.5"
 mypy = "^1.10.0"
 types-requests = "^2.31.0"
 types-pygments = "^2.17.0.20240310"
+types-beautifulsoup4 = "^4.12.0.20240229"
+types-pyyaml = "^6.0.12.20240311"
+types-pytz = "^2024.1.0.20240417"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `json_schema_for_humans-1.0.0/PKG-INFO` & `json_schema_for_humans-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-schema-for-humans
-Version: 1.0.0
+Version: 1.0.1
 Summary: Generate static HTML documentation from JSON schemas
 Home-page: https://github.com/coveooss/json-schema-for-humans
 License: Apache-2.0
 Author: Denis Blanchette
 Author-email: tools@coveo.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -24,17 +24,14 @@
 Requires-Dist: Pygments (>=2.10.0,<3.0.0)
 Requires-Dist: click (>=8.0.1,<9.0.0)
 Requires-Dist: dataclasses-json (>=0.5.6,<0.6.0)
 Requires-Dist: htmlmin (>=0.1.12,<0.2.0)
 Requires-Dist: markdown2 (>=2.4.1,<3.0.0)
 Requires-Dist: pytz
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: types-beautifulsoup4 (>=4.12.0.20240229,<5.0.0.0)
-Requires-Dist: types-pytz (>=2024.1.0.20240417,<2025.0.0.0)
-Requires-Dist: types-pyyaml (>=6.0.12.20240311,<7.0.0.0)
 Project-URL: Repository, https://github.com/coveooss/json-schema-for-humans
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/json-schema-for-humans.svg)](https://badge.fury.io/py/json-schema-for-humans)
 
 # JSON Schema for Humans
```

