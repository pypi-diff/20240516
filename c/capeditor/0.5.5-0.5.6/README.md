# Comparing `tmp/capeditor-0.5.5.tar.gz` & `tmp/capeditor-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capeditor-0.5.5.tar", last modified: Wed May  8 13:47:46 2024, max compression
+gzip compressed data, was "capeditor-0.5.6.tar", last modified: Thu May 16 07:22:11 2024, max compression
```

## Comparing `capeditor-0.5.5.tar` & `capeditor-0.5.6.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.551011 capeditor-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 13:47:42.000000 capeditor-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-08 13:47:46.551011 capeditor-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-08 13:47:42.000000 capeditor-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.531011 capeditor-0.5.5/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/cap_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/caputils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.531011 capeditor-0.5.5/capeditor/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/forms/capimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/locale/am/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.535011 capeditor-0.5.5/capeditor/locale/am/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/am/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/am/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.535011 capeditor-0.5.5/capeditor/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.535011 capeditor-0.5.5/capeditor/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.535011 capeditor-0.5.5/capeditor/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.535011 capeditor-0.5.5/capeditor/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/locale/sw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.535011 capeditor-0.5.5/capeditor/locale/sw/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/sw/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/locale/sw/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.535011 capeditor-0.5.5/capeditor/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/migrations/0002_alter_capsetting_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/migrations/0003_capsetting_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/migrations/0004_predefinedalertarea.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/migrations/0005_alter_capsetting_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.535011 capeditor-0.5.5/capeditor/pubsub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/pubsub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/pubsub/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/pubsub/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/pubsub/publish.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/renderers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/static/capeditor/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.539011 capeditor-0.5.5/capeditor/static/capeditor/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/css/cap_detail_page.css
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/css/import_cap_preview.css
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/css/mapbox-gl-draw.css
--rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/css/maplibre-gl.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.539011 capeditor-0.5.5/capeditor/static/capeditor/css/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/css/widget/boundary-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/css/widget/circle-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/css/widget/polygon-widget.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.539011 capeditor-0.5.5/capeditor/static/capeditor/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.543011 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.543011 capeditor-0.5.5/capeditor/static/capeditor/images/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/images/alert.png
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/images/alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/images/area.png
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/images/certainty.png
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/images/extreme.png
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/images/minor.png
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/images/moderate.png
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/images/severe.png
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/images/urgency.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.547011 capeditor-0.5.5/capeditor/static/capeditor/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/cap_accordion.js
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/conditional_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/mapbox-gl-draw.js
--rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/maplibre-gl.js
--rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/turf.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.547011 capeditor-0.5.5/capeditor/static/capeditor/js/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/widget/circle-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/static/capeditor/js/widget/polygon-widget.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.527011 capeditor-0.5.5/capeditor/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.547011 capeditor-0.5.5/capeditor/templates/capeditor/
--rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/cap_alert_page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.551011 capeditor-0.5.5/capeditor/templates/capeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/icons/cap-alert-full.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/icons/cap-alert.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/load_cap_alert.html
--rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/preview_cap_alert.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.551011 capeditor-0.5.5/capeditor/templates/capeditor/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/widgets/circle_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/templates/capeditor/widgets/polygon_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-08 13:47:42.000000 capeditor-0.5.5/capeditor/wagtail_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:47:46.551011 capeditor-0.5.5/capeditor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-08 13:47:46.000000 capeditor-0.5.5/capeditor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-08 13:47:46.000000 capeditor-0.5.5/capeditor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:47:46.000000 capeditor-0.5.5/capeditor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-08 13:47:46.000000 capeditor-0.5.5/capeditor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 13:47:46.000000 capeditor-0.5.5/capeditor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-08 13:47:42.000000 capeditor-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-08 13:47:46.551011 capeditor-0.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.101181 capeditor-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 07:22:03.000000 capeditor-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-16 07:22:11.101181 capeditor-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10180 2024-05-16 07:22:03.000000 capeditor-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.077180 capeditor-0.5.6/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/cap_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11628 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/caputils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.081180 capeditor-0.5.6/capeditor/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/forms/capimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6749 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/locale/am/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.081180 capeditor-0.5.6/capeditor/locale/am/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/am/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29781 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/am/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.081180 capeditor-0.5.6/capeditor/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    22416 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    29076 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.081180 capeditor-0.5.6/capeditor/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    18681 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25400 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.081180 capeditor-0.5.6/capeditor/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19764 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.081180 capeditor-0.5.6/capeditor/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19747 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    26511 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/locale/sw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.081180 capeditor-0.5.6/capeditor/locale/sw/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    19084 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/sw/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/locale/sw/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.085180 capeditor-0.5.6/capeditor/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/migrations/0002_alter_capsetting_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/migrations/0003_capsetting_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/migrations/0004_predefinedalertarea.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/migrations/0005_alter_capsetting_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15560 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.085180 capeditor-0.5.6/capeditor/pubsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/pubsub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/pubsub/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/pubsub/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/pubsub/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/static/capeditor/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.085180 capeditor-0.5.6/capeditor/static/capeditor/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/css/cap_detail_page.css
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/css/import_cap_preview.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/css/mapbox-gl-draw.css
+-rw-r--r--   0 runner    (1001) docker     (127)    70882 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/css/maplibre-gl.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.085180 capeditor-0.5.6/capeditor/static/capeditor/css/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/css/widget/boundary-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/css/widget/circle-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/css/widget/polygon-draw-widget.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/css/widget/polygon-widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.085180 capeditor-0.5.6/capeditor/static/capeditor/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.093180 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   168060 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   174108 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167336 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   171508 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   170504 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   167000 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173172 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168644 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   173416 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168260 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   168488 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   172860 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/fonts/mapbox-gl-draw.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.093180 capeditor-0.5.6/capeditor/static/capeditor/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/images/alert.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/images/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/images/area.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/images/certainty.png
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/images/extreme.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/images/minor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/images/moderate.png
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/images/severe.png
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/images/urgency.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.097180 capeditor-0.5.6/capeditor/static/capeditor/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/cap_accordion.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/conditional_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)    79103 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/mapbox-gl-draw.js
+-rw-r--r--   0 runner    (1001) docker     (127)   704176 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/maplibre-gl.js
+-rw-r--r--   0 runner    (1001) docker     (127)   604610 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/turf.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.097180 capeditor-0.5.6/capeditor/static/capeditor/js/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8619 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/widget/circle-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/widget/circle-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/widget/polygon-draw-widget.js
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/static/capeditor/js/widget/polygon-widget.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.073180 capeditor-0.5.6/capeditor/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.097180 capeditor-0.5.6/capeditor/templates/capeditor/
+-rw-r--r--   0 runner    (1001) docker     (127)    17275 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/cap_alert_page.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.097180 capeditor-0.5.6/capeditor/templates/capeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/icons/cap-alert-full.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/icons/cap-alert.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/load_cap_alert.html
+-rw-r--r--   0 runner    (1001) docker     (127)    20436 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/preview_cap_alert.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.101181 capeditor-0.5.6/capeditor/templates/capeditor/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/widgets/boundary_polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/widgets/circle_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/widgets/polygon_draw_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/templates/capeditor/widgets/polygon_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-16 07:22:03.000000 capeditor-0.5.6/capeditor/wagtail_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:22:11.101181 capeditor-0.5.6/capeditor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11407 2024-05-16 07:22:11.000000 capeditor-0.5.6/capeditor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-05-16 07:22:11.000000 capeditor-0.5.6/capeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:22:11.000000 capeditor-0.5.6/capeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-16 07:22:11.000000 capeditor-0.5.6/capeditor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 07:22:11.000000 capeditor-0.5.6/capeditor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 07:22:03.000000 capeditor-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-16 07:22:11.101181 capeditor-0.5.6/setup.cfg
```

### Comparing `capeditor-0.5.5/PKG-INFO` & `capeditor-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.5
+Version: 0.5.6
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `capeditor-0.5.5/README.md` & `capeditor-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/blocks.py` & `capeditor-0.5.6/capeditor/blocks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/cap_settings.py` & `capeditor-0.5.6/capeditor/cap_settings.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/caputils.py` & `capeditor-0.5.6/capeditor/caputils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/constants.py` & `capeditor-0.5.6/capeditor/constants.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/forms/capimporter.py` & `capeditor-0.5.6/capeditor/forms/capimporter.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/forms/fields.py` & `capeditor-0.5.6/capeditor/forms/fields.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/forms/widgets.py` & `capeditor-0.5.6/capeditor/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/am/LC_MESSAGES/django.mo` & `capeditor-0.5.6/capeditor/locale/am/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/am/LC_MESSAGES/django.po` & `capeditor-0.5.6/capeditor/locale/am/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/ar/LC_MESSAGES/django.mo` & `capeditor-0.5.6/capeditor/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/ar/LC_MESSAGES/django.po` & `capeditor-0.5.6/capeditor/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/en/LC_MESSAGES/django.mo` & `capeditor-0.5.6/capeditor/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/en/LC_MESSAGES/django.po` & `capeditor-0.5.6/capeditor/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/es/LC_MESSAGES/django.mo` & `capeditor-0.5.6/capeditor/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/es/LC_MESSAGES/django.po` & `capeditor-0.5.6/capeditor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/fr/LC_MESSAGES/django.mo` & `capeditor-0.5.6/capeditor/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/fr/LC_MESSAGES/django.po` & `capeditor-0.5.6/capeditor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/sw/LC_MESSAGES/django.mo` & `capeditor-0.5.6/capeditor/locale/sw/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/locale/sw/LC_MESSAGES/django.po` & `capeditor-0.5.6/capeditor/locale/sw/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/migrations/0001_initial.py` & `capeditor-0.5.6/capeditor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/migrations/0002_alter_capsetting_options_and_more.py` & `capeditor-0.5.6/capeditor/migrations/0002_alter_capsetting_options_and_more.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/migrations/0003_capsetting_logo.py` & `capeditor-0.5.6/capeditor/migrations/0003_capsetting_logo.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/migrations/0004_predefinedalertarea.py` & `capeditor-0.5.6/capeditor/migrations/0004_predefinedalertarea.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/models.py` & `capeditor-0.5.6/capeditor/models.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/pubsub/base.py` & `capeditor-0.5.6/capeditor/pubsub/base.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/pubsub/mqtt.py` & `capeditor-0.5.6/capeditor/pubsub/mqtt.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/pubsub/publish.py` & `capeditor-0.5.6/capeditor/pubsub/publish.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/renderers.py` & `capeditor-0.5.6/capeditor/renderers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/serializers.py` & `capeditor-0.5.6/capeditor/serializers.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/css/cap_detail_page.css` & `capeditor-0.5.6/capeditor/static/capeditor/css/cap_detail_page.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/css/import_cap_preview.css` & `capeditor-0.5.6/capeditor/static/capeditor/css/import_cap_preview.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/css/mapbox-gl-draw.css` & `capeditor-0.5.6/capeditor/static/capeditor/css/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/css/maplibre-gl.css` & `capeditor-0.5.6/capeditor/static/capeditor/css/maplibre-gl.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/css/widget/circle-widget.css` & `capeditor-0.5.6/capeditor/static/capeditor/css/widget/circle-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/css/widget/polygon-widget.css` & `capeditor-0.5.6/capeditor/static/capeditor/css/widget/polygon-widget.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/fonts/mapbox-gl-draw.css` & `capeditor-0.5.6/capeditor/static/capeditor/fonts/mapbox-gl-draw.css`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/images/alert.png` & `capeditor-0.5.6/capeditor/static/capeditor/images/alert.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/images/alert.svg` & `capeditor-0.5.6/capeditor/static/capeditor/images/alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/images/area.png` & `capeditor-0.5.6/capeditor/static/capeditor/images/area.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/images/certainty.png` & `capeditor-0.5.6/capeditor/static/capeditor/images/certainty.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/images/extreme.png` & `capeditor-0.5.6/capeditor/static/capeditor/images/extreme.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/images/minor.png` & `capeditor-0.5.6/capeditor/static/capeditor/images/minor.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/images/moderate.png` & `capeditor-0.5.6/capeditor/static/capeditor/images/moderate.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/images/severe.png` & `capeditor-0.5.6/capeditor/static/capeditor/images/severe.png`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/cap_accordion.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/cap_accordion.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/conditional_fields.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/conditional_fields.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/mapbox-gl-draw.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/mapbox-gl-draw.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/maplibre-gl.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/maplibre-gl.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/turf.min.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/turf.min.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/widget/boundary-polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/widget/boundary-polygon-widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -305,15 +305,15 @@
                     const name = boundary[`name_${level}`]
 
                     if (name) {
                         this.areaDescInput.val(name)
                     }
 
                     const truncatedFeature = turf.truncate(feature, {
-                        precision: 2,
+                        precision: 6,
                         coordinates: 2,
                         mutate: true
                     })
 
                     this.setSourceData(truncatedFeature)
                 })
             }
```

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/widget/circle-widget-telepath.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/widget/circle-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/widget/circle-widget.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/widget/circle-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/widget/hazard-event-type-widget.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/widget/polygon-draw-widget.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/widget/polygon-draw-widget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -179,15 +179,15 @@
         }
 
         if (combinedFeatures) {
             const feature = combinedFeatures.features[0]
 
 
             const truncatedFeature = turf.truncate(feature, {
-                precision: 2,
+                precision: 6,
                 coordinates: 2,
                 mutate: true
             })
 
             this.setValue(JSON.stringify(truncatedFeature.geometry))
 
         } else {
```

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/widget/polygon-widget-telepath.js`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/static/capeditor/js/widget/polygon-widget.js` & `capeditor-0.5.6/capeditor/static/capeditor/js/widget/polygon-widget.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -332,15 +332,15 @@
 
 
 PolygonWidget.prototype.setDrawData = function(featureGeom) {
     if (featureGeom) {
 
         // truncate geometry
         const geometry = turf.truncate(featureGeom, {
-            precision: 2,
+            precision: 6,
             coordinates: 2,
             mutate: true
         })
 
         const bbox = turf.bbox(geometry)
         const bounds = [
             [bbox[0], bbox[1]],
```

### Comparing `capeditor-0.5.5/capeditor/templates/capeditor/cap_alert_page.html` & `capeditor-0.5.6/capeditor/templates/capeditor/cap_alert_page.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/templates/capeditor/icons/cap-alert-full.svg` & `capeditor-0.5.6/capeditor/templates/capeditor/icons/cap-alert-full.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/templates/capeditor/icons/cap-alert.svg` & `capeditor-0.5.6/capeditor/templates/capeditor/icons/cap-alert.svg`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/templates/capeditor/load_cap_alert.html` & `capeditor-0.5.6/capeditor/templates/capeditor/load_cap_alert.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/templates/capeditor/preview_cap_alert.html` & `capeditor-0.5.6/capeditor/templates/capeditor/preview_cap_alert.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/templates/capeditor/widgets/circle_widget.html` & `capeditor-0.5.6/capeditor/templates/capeditor/widgets/circle_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html` & `capeditor-0.5.6/capeditor/templates/capeditor/widgets/hazard_event_type_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/templates/capeditor/widgets/polygon_draw_widget.html` & `capeditor-0.5.6/capeditor/templates/capeditor/widgets/polygon_draw_widget.html`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/utils.py` & `capeditor-0.5.6/capeditor/utils.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/views.py` & `capeditor-0.5.6/capeditor/views.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor/wagtail_hooks.py` & `capeditor-0.5.6/capeditor/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/capeditor.egg-info/PKG-INFO` & `capeditor-0.5.6/capeditor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capeditor
-Version: 0.5.5
+Version: 0.5.6
 Summary: Wagtail based CAP composer
 Home-page: https://github.com/wmo-raf/cap-composer
 Author: Grace Amondi, Erick Otenyo
 Author-email: miswa.grace@gmail.com, otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `capeditor-0.5.5/capeditor.egg-info/SOURCES.txt` & `capeditor-0.5.6/capeditor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `capeditor-0.5.5/setup.cfg` & `capeditor-0.5.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = capeditor
-version = 0.5.5
+version = 0.5.6
 description = Wagtail based CAP composer
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/cap-composer
 author = Grace Amondi, Erick Otenyo
 author_email = miswa.grace@gmail.com, otenyo.erick@gmail.com
 license = MIT
```

