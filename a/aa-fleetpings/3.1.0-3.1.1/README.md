# Comparing `tmp/aa_fleetpings-3.1.0.tar.gz` & `tmp/aa_fleetpings-3.1.1.tar.gz`

## Comparing `aa_fleetpings-3.1.0.tar` & `aa_fleetpings-3.1.1.tar`

### file list

```diff
@@ -1,105 +1,108 @@
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/__init__.py
--rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/admin.py
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/app_settings.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/apps.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/auth_hooks.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/constants.py
--rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/form.py
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/managers.py
--rw-r--r--   0        0        0    17339 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/models.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/urls.py
--rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/views.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/helper/discord_webhook.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/helper/eve_images.py
--rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/helper/ping_context.py
--rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/django.pot
--rw-r--r--   0        0        0    14074 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14326 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20019 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11722 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15662 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13804 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20501 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    13991 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14556 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    17350 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23594 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14069 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10965 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24522 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14386 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12854 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0001_initial.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0003_fleetdoctrine_link.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0004_auto_20200915_1617.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0008_auto_20210114_1733.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py
--rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0011_settings_and_verbose_names.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0013_fleetcomm_channel.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0014_update_models.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/migrations/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/css/fleetpings.css
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/css/fleetpings.min.css
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/css/fleetpings.min.css.map
--rw-r--r--   0        0        0    19511 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.js
--rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.min.js
--rw-r--r--   0        0        0     8936 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.min.js.map
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/LICENSE
--rw-r--r--   0        0        0    34864 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.js
--rw-r--r--   0        0        0    12465 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js
--rw-r--r--   0        0        0    53322 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js.map
--rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/readme.md
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/base.html
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/index.html
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/bundles/fleetpings-css.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/bundles/fleetpings-js.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/form.html
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-comms.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-formup-location.html
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-type-loop.html
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/ping-channel.html
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/ping-targets-loop.html
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/header/page-header.html
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/ping/ping.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templatetags/__init__.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/templatetags/fleetpings.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/__init__.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_access.py
--rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_ajax_calls.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_helper_eve_images.py
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_installed_modules.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_discprdpingtarget.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleetcomm.py
--rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleetdoctrine.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleettype.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_formuplocation.py
--rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_setting.py
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_model_webhook.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/test_templatetags.py
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/fleetpings/tests/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/LICENSE
--rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/README.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    51307 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/__init__.py
+-rw-r--r--   0        0        0     8449 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/admin.py
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/app_settings.py
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/apps.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/auth_hooks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/constants.py
+-rw-r--r--   0        0        0     6099 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/form.py
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/managers.py
+-rw-r--r--   0        0        0    17339 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/models.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/urls.py
+-rw-r--r--   0        0        0    13953 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/views.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/helper/discord_webhook.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/helper/eve_images.py
+-rw-r--r--   0        0        0     8647 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/helper/ping_context.py
+-rw-r--r--   0        0        0    13944 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/django.pot
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14168 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14326 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20013 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10896 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22910 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3925 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15662 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14088 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14081 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    13804 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20473 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14083 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14556 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    16463 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23622 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14164 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10085 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24543 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16332 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12854 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0001_initial.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0002_webhook_is_embed_description_change.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0003_fleetdoctrine_link.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0004_auto_20200915_1617.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0005_fleettype_restricted_to_group.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0008_auto_20210114_1733.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py
+-rw-r--r--   0        0        0    12638 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0011_settings_and_verbose_names.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0013_fleetcomm_channel.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0014_update_models.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/migrations/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/css/fleetpings.css
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/css/fleetpings.min.css
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/css/fleetpings.min.css.map
+-rw-r--r--   0        0        0    19511 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/js/fleetpings.js
+-rw-r--r--   0        0        0     7565 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/js/fleetpings.min.js
+-rw-r--r--   0        0        0     8936 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/js/fleetpings.min.js.map
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/LICENSE
+-rw-r--r--   0        0        0    34864 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.js
+-rw-r--r--   0        0        0    12465 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js
+-rw-r--r--   0        0        0    53322 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js.map
+-rw-r--r--   0        0        0    11530 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/readme.md
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/base.html
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/index.html
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/bundles/fleetpings-css.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/bundles/fleetpings-js.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/form.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/fleet-comms.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/fleet-formup-location.html
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/fleet-type-loop.html
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/ping-channel.html
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/ping-targets-loop.html
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/header/page-header.html
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/ping/ping.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templatetags/__init__.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/templatetags/fleetpings.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/__init__.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_access.py
+-rw-r--r--   0        0        0    12747 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_ajax_calls.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_helper_eve_images.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_installed_modules.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_model_discprdpingtarget.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_model_fleetcomm.py
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_model_fleetdoctrine.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_model_fleettype.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_model_formuplocation.py
+-rw-r--r--   0        0        0     2778 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_model_setting.py
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_model_webhook.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/test_templatetags.py
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/fleetpings/tests/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/LICENSE
+-rw-r--r--   0        0        0     8656 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/README.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0    51307 2020-02-02 00:00:00.000000 aa_fleetpings-3.1.1/PKG-INFO
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/admin.py` & `aa_fleetpings-3.1.1/fleetpings/admin.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/app_settings.py` & `aa_fleetpings-3.1.1/fleetpings/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/auth_hooks.py` & `aa_fleetpings-3.1.1/fleetpings/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/form.py` & `aa_fleetpings-3.1.1/fleetpings/form.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/managers.py` & `aa_fleetpings-3.1.1/fleetpings/managers.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/models.py` & `aa_fleetpings-3.1.1/fleetpings/models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/urls.py` & `aa_fleetpings-3.1.1/fleetpings/urls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/views.py` & `aa_fleetpings-3.1.1/fleetpings/views.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/helper/discord_webhook.py` & `aa_fleetpings-3.1.1/fleetpings/helper/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/helper/eve_images.py` & `aa_fleetpings-3.1.1/fleetpings/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/helper/ping_context.py` & `aa_fleetpings-3.1.1/fleetpings/helper/ping_context.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/django.pot` & `aa_fleetpings-3.1.1/fleetpings/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/cs/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:04+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/de/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.1/fleetpings/locale/de/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "\n"
 "                <code>@everyone</code>\n"
 "                includes also all the people in this channel who are offline "
 "and\n"
 "                possibly asleep at the moment and might be waking up when "
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/de/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: 2024-04-21 13:51+0000\n"
+"PO-Revision-Date: 2024-05-10 14:04+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-fleetpings/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr "Flotten-Ankündigungen"
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
@@ -122,34 +122,33 @@
 msgstr "Flottenstart"
 
 #: fleetpings/form.py:124
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
 msgstr ""
-"Um dieses Feld zu aktivieren, mach es entweder zu einem Pre-Ping "
-"(Kontrollkästchen oben) oder deaktiviere „Flottenstart "
-"JETZT“ (Kontrollkästchen unten)."
+"Um dieses Feld zu aktivieren, mach es entweder zu einem Pre-Ping ("
+"Kontrollkästchen oben) oder deaktiviere „Flottenstart JETZT“ ("
+"Kontrollkästchen unten)."
 
 #: fleetpings/form.py:130
 msgid "Formup timestamp"
 msgstr "Flottenstart Zeitstempel"
 
 #: fleetpings/form.py:136
 msgid "Formup NOW"
 msgstr "Flottenstart JETZT"
 
 #: fleetpings/form.py:138
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
 msgstr ""
-"Wenn dieses Kontrollkästchen aktiviert ist, wird der Flottenstart auf "
-"„JETZT“ gesetzt. und die Zeit im obigen Feld (falls vorhanden) wird "
-"ignoriert."
+"Wenn dieses Kontrollkästchen aktiviert ist, wird der Flottenstart auf „JETZT“"
+" gesetzt. und die Zeit im obigen Feld (falls vorhanden) wird ignoriert."
 
 #: fleetpings/form.py:144 fleetpings/models.py:168
 msgid "Fleet comms"
 msgstr "Flottenkommunikationen"
 
 #: fleetpings/form.py:163
 msgid "Webhook embed color"
@@ -354,16 +353,15 @@
 #: fleetpings/models.py:499
 msgid "Name of the channel this webhook posts to"
 msgstr "Name des Kanals in dem dieser Webhook postet"
 
 #: fleetpings/models.py:509
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
-msgstr ""
-"URL des Webhooks, z. B.: https://discord.com/api/webhooks/123456/abcdef"
+msgstr "URL des Webhooks, z. B.: https://discord.com/api/webhooks/123456/abcdef"
 
 #: fleetpings/models.py:529
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 "Wenn Du möchtest, kannst Du hier Anmerkungen zu diesem Webhook hinzufügen"
 
 #: fleetpings/models.py:537
@@ -418,16 +416,16 @@
 "hinzugefügt."
 
 #: fleetpings/models.py:622
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
-"Standard Pingziele nutzen. Wenn angehakt, werden die Standard Pingziele "
-"(@everyone and @here) dem Dropdown im Formular hinzugefügt."
+"Standard Pingziele nutzen. Wenn angehakt, werden die Standard Pingziele (@"
+"everyone and @here) dem Dropdown im Formular hinzugefügt."
 
 #: fleetpings/models.py:632
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
 msgstr ""
 "Sollen die Doktrinen aus dem Fittings Modul genutzt werden? Hinweis: das "
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/es/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.1/fleetpings/locale/es/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,38 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
-
-msgid ""
-"\n"
-"                    <code>@everyone</code>\n"
-"                    includes also all the people in this channel who are "
-"offline and\n"
-"                    possibly asleep at the moment and might be waking up "
-"when their\n"
-"                    mobile devices ping. Or they wake up hours later to "
-"irrelevant\n"
-"                    pings by the time they open Discord.\n"
-"                "
-msgstr ""
-"\n"
-"                    <code>@everyone</code>\n"
-"                    incluye también a todas las personas en este canal que "
-"están fuera de línea y\n"
-"                    posiblemente dormidas en este momento y podrían estar "
-"despertando mediante sus\n"
-"                    dispositivos móviles para pings. O se despiertan horas "
-"más tarde con cosas irrelevantes\n"
-"                    con los pings en el momento en que abren Discord.\n"
-"                "
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> engaña muy bien por lo general."
 
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr "El Enlace a la página de la doctrina, si tiene."
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/es/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
-# Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023.
+# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: 2023-10-25 07:04+0000\n"
-"Last-Translator: Geovanny David Morales De la cruz "
-"<moralesgeovanny1996@gmail.com>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/es/>\n"
+"PO-Revision-Date: 2024-05-10 14:04+0000\n"
+"Last-Translator: Geovanny David Morales De la cruz <moralesgeovanny1996@gmail"
+".com>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr "Pings de Flotas"
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.1/fleetpings/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Êtes-vous sûr d'avoir lié Discord à votre Alliance Auth ?"
 
 msgid "Can access this app"
 msgstr "Peut accéder à cette application"
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/fr_FR/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 # Matthias P <randomusernetcom@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: 2024-04-17 23:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:04+0000\n"
 "Last-Translator: Matthias P <randomusernetcom@gmail.com>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/fr/>\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/it_IT/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/ja/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: 2023-09-24 13:14+0000\n"
+"PO-Revision-Date: 2024-05-10 14:04+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/it/>\n"
-"Language: it_IT\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/ja/>\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/ja/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/nl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: 2023-09-24 13:14+0000\n"
+"PO-Revision-Date: 2024-05-10 14:05+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/ja/>\n"
-"Language: ja\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.1/fleetpings/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetpings/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "\n"
 "                <code>@everyone</code>\n"
 "                includes also all the people in this channel who are offline "
 "and\n"
 "                possibly asleep at the moment and might be waking up when "
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/ko_KR/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Author50CO <tkddlschry@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Author50CO <tkddlschry@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 # Mind of the Raven <okanieva@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: 2024-03-22 01:11+0000\n"
-"Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/ko/>\n"
+"PO-Revision-Date: 2024-05-10 14:04+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr "함대 핑"
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
@@ -72,16 +72,15 @@
 #: fleetpings/form.py:27
 msgid "Discord Markdown"
 msgstr "디스코드 마크다운"
 
 #: fleetpings/form.py:34
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
-msgstr ""
-"힌트: {discord_markdown_link}를 사용해 텍스트 양식을 변경할 수 있습니다."
+msgstr "힌트: {discord_markdown_link}를 사용해 텍스트 양식을 변경할 수 있습니다."
 
 #: fleetpings/form.py:78
 msgid "Who do you want to ping?"
 msgstr "핑을 보낼까요?"
 
 #: fleetpings/form.py:83
 msgid "Pre-Ping"
@@ -127,17 +126,16 @@
 msgid "Formup time"
 msgstr "폼업 시간"
 
 #: fleetpings/form.py:124
 msgid ""
 "To enable this field, either make it a pre-ping (checkbox above) or uncheck "
 "\"Formup NOW\" (checkbox below)."
-msgstr ""
-"이 창을 활성화하려면, 예고 핑을 활성화하거나(위 체크박스), “지금 폼업하기” 체"
-"크 박스를 해제하세요."
+msgstr "이 창을 활성화하려면, 예고 핑을 활성화하거나(위 체크박스), “지금 폼업하기” "
+"체크 박스를 해제하세요."
 
 #: fleetpings/form.py:130
 #, fuzzy
 #| msgid "Formup Timestamp"
 msgid "Formup timestamp"
 msgstr "폼업 타임스탬프"
 
@@ -145,17 +143,16 @@
 msgid "Formup NOW"
 msgstr "지금 폼업"
 
 #: fleetpings/form.py:138
 msgid ""
 "If this checkbox is active, formup time will be set to \"NOW\" and the time "
 "in the field above (if any is set) will be ignored."
-msgstr ""
-"이 체크박스가 활성화되어 있으면, 폼업 시간이 “지금” 으로 설정되며 위쪽에 설정"
-"된 시간을 무시합니다."
+msgstr "이 체크박스가 활성화되어 있으면, 폼업 시간이 “지금” 으로 설정되며 위쪽에 "
+"설정된 시간을 무시합니다."
 
 #: fleetpings/form.py:144 fleetpings/models.py:168
 msgid "Fleet comms"
 msgstr "함대 음성채널"
 
 #: fleetpings/form.py:163
 #, fuzzy
@@ -175,16 +172,15 @@
 msgid "Create SRP link"
 msgstr "SRP 링크 생성"
 
 #: fleetpings/form.py:177
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
-msgstr ""
-"이 체크박스가 활성화되어 있으면, 이 함대에 대한 SRP 링크가 생성됩니다. <br> "
+msgstr "이 체크박스가 활성화되어 있으면, 이 함대에 대한 SRP 링크가 생성됩니다. <br> "
 "확실하지 않은 경우 체크하지 마세요."
 
 #: fleetpings/form.py:183
 msgid "Additional information"
 msgstr "추가 정보"
 
 #: fleetpings/form.py:190
@@ -195,17 +191,16 @@
 msgid "Create Optimer"
 msgstr "옵 타이머 생성"
 
 #: fleetpings/form.py:201
 msgid ""
 "If this checkbox is active, a fleet operations timer for this pre-ping will "
 "be created."
-msgstr ""
-"이 체크박스가 활성화되어 있으면, 이 예고 핑에 대한 함대 옵 타이머가 생성됩니"
-"다."
+msgstr "이 체크박스가 활성화되어 있으면, 이 예고 핑에 대한 함대 옵 타이머가 "
+"생성됩니다."
 
 #: fleetpings/form.py:207
 msgid "Duration"
 msgstr ""
 
 #: fleetpings/form.py:208
 msgid "How long approximately will the fleet be?"
@@ -305,16 +300,15 @@
 msgid "Formup locations"
 msgstr "폼업 위치"
 
 #: fleetpings/models.py:322
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
-msgstr ""
-"핑을 보낼 디스코드 역할. (설명: 디스코드와 연동된 Auth 그룹이어야 합니다.)"
+msgstr "핑을 보낼 디스코드 역할. (설명: 디스코드와 연동된 Auth 그룹이어야 합니다.)"
 
 #: fleetpings/models.py:326
 msgid "Group name"
 msgstr "그룹 이름"
 
 #: fleetpings/models.py:334
 msgid "ID of the Discord role to ping"
@@ -381,16 +375,15 @@
 msgid "Webhooks"
 msgstr "웹훅"
 
 #: fleetpings/models.py:576
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
-msgstr ""
-"잘못된 웹훅 URL. 알려진 디스코드의 웹훅 URL 형태와 일치하지 않습니다. 웹훅 "
+msgstr "잘못된 웹훅 URL. 알려진 디스코드의 웹훅 URL 형태와 일치하지 않습니다. 웹훅 "
 "URL을 확인해 주세요."
 
 #: fleetpings/models.py:596
 msgid "Use default fleet types"
 msgstr "기본 함대 종류 사용"
 
 #: fleetpings/models.py:599
@@ -411,45 +404,44 @@
 
 #: fleetpings/models.py:611
 msgid ""
 "Whether to use default fleet types. If checked, the default fleet types "
 "(Roaming, Home Defense, StratOP, and CTA) will be added to the Fleet Type "
 "dropdown."
 msgstr ""
-"기본 함대 종류를 사용할지 여부 설정. 활성화된 경우, 기본 함대 종류(로밍, 기"
-"지 방어, 스트랫 옵, CTA)가 함대 종류 드롭다운 메뉴에 추가됩니다."
+"기본 함대 종류를 사용할지 여부 설정. 활성화된 경우, 기본 함대 종류(로밍, "
+"기지 방어, 스트랫 옵, CTA)가 함대 종류 드롭다운 메뉴에 추가됩니다."
 
 #: fleetpings/models.py:622
 msgid ""
 "Whether to use default ping targets. If checked, the default ping targets "
 "(@everyone and @here) will be added to the Ping Target dropdown."
 msgstr ""
-"기본 핑 역할 사용 여부 설정. 활성화된 경우, 기본 핑 역할 (@everyone 과 "
-"@here) 가 핑 역할 드롭다운에 추가됩니다."
+"기본 핑 역할 사용 여부 설정. 활성화된 경우, 기본 핑 역할 (@everyone 과 @here)"
+" 가 핑 역할 드롭다운에 추가됩니다."
 
 #: fleetpings/models.py:632
 msgid ""
 "Whether to use the doctrines from the Fittings modules in the doctrine "
 "dropdown. Note: The fittings module needs to be installed for this."
-msgstr ""
-"독트린 드롭다운에서 해당 독트린의 피팅 모듈 사용 여부 설정. 설명: 피팅 모듈"
-"이 설치되어 있어야 합니다."
+msgstr "독트린 드롭다운에서 해당 독트린의 피팅 모듈 사용 여부 설정. 설명: 피팅 "
+"모듈이 설치되어 있어야 합니다."
 
 #: fleetpings/models.py:642
 msgid ""
 "Whether to verify webhooks URLs or not. Note: When unchecked, webhook URLs "
 "will not be verified, so the app can be used with non-Discord webhooks as "
 "well. When disabling webhook verification and using non-Discord webhooks, it "
 "is up to you to make sure your webhook understands a payload that is "
 "formatted for Discord webhooks."
 msgstr ""
-"웹훅 URL 검사여부 설정. 설명: 체크가 해제되어 있을 경우 URL을 검사하지 않습니"
-"다, 따라서 디스코드가 아닌 URL도 사용할 수 있습니다. 웹훅 검사를 해제하고 디"
-"스코드가 아닌 웹훅을 사용할 경우, 웹훅이 전송할 부하를 감당할 수 있을지의 판"
-"단여부는 사용자의 몫입니다."
+"웹훅 URL 검사여부 설정. 설명: 체크가 해제되어 있을 경우 URL을 검사하지 "
+"않습니다, 따라서 디스코드가 아닌 URL도 사용할 수 있습니다. 웹훅 검사를 "
+"해제하고 디스코드가 아닌 웹훅을 사용할 경우, 웹훅이 전송할 부하를 감당할 수 "
+"있을지의 판단여부는 사용자의 몫입니다."
 
 #: fleetpings/models.py:655
 msgid "Default highlight color for the webhook embed."
 msgstr "웹훅 embed 기본 하이라이트 색상."
 
 #: fleetpings/models.py:667
 #, fuzzy
@@ -479,41 +471,39 @@
 
 #: fleetpings/templates/fleetpings/index.html:51
 msgid ""
 "Mandatory information is missing. To create an optimer, you need to provide "
 "all of the following information:<br>» FC name<br>» Fleet name<br>» Formup "
 "location<br>» Formup time<br>» Ships / Doctrine"
 msgstr ""
-"필수 정보가 누락되었습니다. 옵 타이머를 생성하려면, 다음 정보를 모두 제공해"
-"야 합니다:<br>» FC 이름<br>» 플릿 이름<br>» 폼업 지역<br>» 폼업 시각<br>» 함"
-"선/독트린"
+"필수 정보가 누락되었습니다. 옵 타이머를 생성하려면, 다음 정보를 모두 "
+"제공해야 합니다:<br>» FC 이름<br>» 플릿 이름<br>» 폼업 지역<br>» 폼업 "
+"시각<br>» 함선/독트린"
 
 #: fleetpings/templates/fleetpings/index.html:56
 msgid ""
 "Mandatory information is missing. To create an SRP link, you need to provide "
 "all of the following information:<br>» Fleet name<br>» Ships / Doctrine"
 msgstr ""
-"필수 정보가 누락되었습니다. SRP 항목을 생성하려면, 다음 정보를 기입해야 합니"
-"다:<br>» 함대 이름<br>» 함선 / 독트린"
+"필수 정보가 누락되었습니다. SRP 항목을 생성하려면, 다음 정보를 기입해야 "
+"합니다:<br>» 함대 이름<br>» 함선 / 독트린"
 
 #: fleetpings/templates/fleetpings/index.html:60
 msgid ""
 "Error! Your ping was not copied to your clipboard. Maybe your browser "
 "doesn&apos;t support this feature."
-msgstr ""
-"오류! 핑이 클립보드에 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 않"
-"을 수도 있습니다."
+msgstr "오류! 핑이 클립보드에 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 "
+"않을 수도 있습니다."
 
 #: fleetpings/templates/fleetpings/index.html:61
 msgid ""
 "Success! Your ping text has been copied to your clipboard. Now be a good FC "
 "and throw it in your chat so you actually get some people in fleet."
-msgstr ""
-"성공! 핑이 클립보드에 복사되었습니다. 채팅창에 핑을 붙여넣어 사람을 모아보세"
-"요."
+msgstr "성공! 핑이 클립보드에 복사되었습니다. 채팅창에 핑을 붙여넣어 사람을 "
+"모아보세요."
 
 #: fleetpings/templates/fleetpings/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
@@ -551,17 +541,16 @@
 "                    또는 몇 시간 뒤 일어나서 디스코드를 열었을 때\n"
 "                    별로 중요하지 않은 내용의 핑을 볼 수도 있습니다.\n"
 "            "
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
 msgid ""
 "Notification spam is a real thing and might entice people to mute channels."
-msgstr ""
-"알람 스팸은 실제로 존재하며 사람들이 채널 알람을 끄게 되는 이유가 될 수 있습"
-"니다."
+msgstr "알람 스팸은 실제로 존재하며 사람들이 채널 알람을 끄게 되는 이유가 될 수 "
+"있습니다."
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:24
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> 는 사용해도 좋습니다."
 
 #: fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html:3
 msgid "Please select"
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/nl/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/sk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:05+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/pl_PL/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.1/fleetpings/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-fleetpings/pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Additional information"
 msgstr "Dodatkowe informacje"
 
 msgid "Discord Markdown"
 msgstr "Discord Markdown"
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/pl_PL/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: 2024-04-07 13:07+0000\n"
+"PO-Revision-Date: 2024-05-10 14:05+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Polish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/pl/>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/pl/>\n"
 "Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/ru/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.1/fleetpings/locale/ru/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,37 +8,15 @@
 "apps/aa-fleetpings/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
-
-msgid ""
-"\n"
-"                    <code>@everyone</code>\n"
-"                    includes also all the people in this channel who are "
-"offline and\n"
-"                    possibly asleep at the moment and might be waking up "
-"when their\n"
-"                    mobile devices ping. Or they wake up hours later to "
-"irrelevant\n"
-"                    pings by the time they open Discord.\n"
-"                "
-msgstr ""
-"\n"
-"                    <code>@everyone</code>\n"
-"                    обозначает всех людей в канале, включая тех кто "
-"offline,\n"
-"                    возможно сейчас спит и будет разбужен звуком\n"
-"                    мобильного устройств. Или они проснуться через несколько "
-"часов\n"
-"                    и увидят неактуальные пинги в Discord.\n"
-"                "
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> обычно решает задачу."
 
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr "Ссылка на страницу формата."
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/ru/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# Nikolay <nick.postnikov@gmail.com>, 2023.
-# Max <mark25@inbox.ru>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Nikolay <nick.postnikov@gmail.com>, 2023, 2024.
+# Max <mark25@inbox.ru>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: 2023-10-03 11:34+0000\n"
-"Last-Translator: Max <mark25@inbox.ru>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/ru/>\n"
+"PO-Revision-Date: 2024-05-10 14:05+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr "Анонсы флота"
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
@@ -170,16 +170,16 @@
 msgstr "Создание SRP ссылки"
 
 #: fleetpings/form.py:177
 msgid ""
 "If this checkbox is active, a SRP link specific for this fleet will be "
 "created.<br>Leave blank if unsure."
 msgstr ""
-"Если флажок активен, специальная ссылка для компенса будет создана."
-"<br>Оставьте неактивным, если не уверены."
+"Если флажок активен, специальная ссылка для компенса будет "
+"создана.<br>Оставьте неактивным, если не уверены."
 
 #: fleetpings/form.py:183
 msgid "Additional information"
 msgstr "Дополнительная информация"
 
 #: fleetpings/form.py:190
 msgid "Feel free to add some more information about the fleet …"
@@ -542,16 +542,16 @@
 "                mobile devices ping. Or they wake up hours later to "
 "irrelevant\n"
 "                pings by the time they open Discord.\n"
 "            "
 msgstr ""
 "\n"
 "                    <code>@everyone</code>\n"
-"                    обозначает всех людей в канале, включая тех кто "
-"offline,\n"
+"                    обозначает всех людей в канале, включая тех кто offline,"
+"\n"
 "                    возможно сейчас спит и будет разбужен звуком\n"
 "                    мобильного устройств. Или они проснуться через несколько "
 "часов\n"
 "                    и увидят неактуальные пинги в Discord.\n"
 "                "
 
 #: fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html:20
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/sk/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
-#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:05+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Czech <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 msgid "Fleet Pings"
 msgstr ""
 
 #: fleetpings/admin.py:114 fleetpings/models.py:167
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/uk/LC_MESSAGES/django.mo` & `aa_fleetpings-3.1.1/fleetpings/locale/uk/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,34 +8,15 @@
 "apps/aa-fleetpings/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.4.2\n"
-
-msgid ""
-"\n"
-"                    <code>@everyone</code>\n"
-"                    includes also all the people in this channel who are "
-"offline and\n"
-"                    possibly asleep at the moment and might be waking up "
-"when their\n"
-"                    mobile devices ping. Or they wake up hours later to "
-"irrelevant\n"
-"                    pings by the time they open Discord.\n"
-"                "
-msgstr ""
-"\n"
-"                    <code>@everyone</code> включає всіх людей в цьому "
-"каналі, які не в мережі, можливо сплять в цей момент, але можуть "
-"прокинутися, коли їх мобільні пристрої сповіщатимуть. Або вони прокинуться "
-"годинами пізніше до непотрібних повідомлень, коли вони відкриють Discord.\n"
-"                "
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "<code>@here</code> usually does the trick just fine."
 msgstr "<code>@here</code> зазвичай чудово справляється з цим завданням."
 
 msgid "A link to a doctrine page for this doctrine if you have."
 msgstr "Посилання на сторінку доктрини для цієї доктрини, якщо вона у вас є."
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/locale/uk/LC_MESSAGES/django.po` & `aa_fleetpings-3.1.1/fleetpings/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Kristof <kristof@teh.ninja>, 2023.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# "Andrii M." <elfleg0las88@gmail.com>, 2023.
+# Kristof <kristof@teh.ninja>, 2023, 2024.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# "Andrii M." <elfleg0las88@gmail.com>, 2023, 2024.
 # Madz Cooper <i.sviridjuk@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-21 09:10+0200\n"
-"PO-Revision-Date: 2024-03-02 23:10+0000\n"
-"Last-Translator: Madz Cooper <i.sviridjuk@gmail.com>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetpings/uk/>\n"
+"PO-Revision-Date: 2024-05-10 14:05+0000\n"
+"Last-Translator: \"Andrii M.\" <elfleg0las88@gmail.com>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetpings/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: fleetpings/__init__.py:10 fleetpings/templates/fleetpings/base.html:6
 #: fleetpings/templates/fleetpings/base.html:10
 #, fuzzy
 #| msgid "Fleet Ping Tool"
 msgid "Fleet Pings"
 msgstr "Інструмент пінгування флоту"
@@ -410,16 +410,16 @@
 msgid "Name of the channel this webhook posts to"
 msgstr "Назва каналу, на який публікується цей веб-хук"
 
 #: fleetpings/models.py:509
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
-"URL-адреса цього веб-хука, наприклад, https://discord.com/api/"
-"webhooks/123456/abcdef"
+"URL-адреса цього веб-хука, наприклад, https://discord.com/api/webhooks/"
+"123456/abcdef"
 
 #: fleetpings/models.py:529
 msgid "You can add notes about this webhook here if you want"
 msgstr "Ви можете додати примітки про цей вебхук тут, якщо хочете"
 
 #: fleetpings/models.py:537
 msgid "Whether this webhook is active or not"
```

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0001_initial.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0002_webhook_is_embed_description_change.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0002_webhook_is_embed_description_change.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0003_fleetdoctrine_link.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0003_fleetdoctrine_link.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0004_auto_20200915_1617.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0004_auto_20200915_1617.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0005_fleettype_restricted_to_group.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0005_fleettype_restricted_to_group.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0006_fleetdoctrine_restricted_to_group.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0007_mysql8_default_value_fixes_20201003_1232.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0008_auto_20210114_1733.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0008_auto_20210114_1733.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0009_remove_webhook_is_embedded_remove_webhook_type_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0010_use_ellipsis_character_in_strings.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0011_settings_and_verbose_names.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0011_settings_and_verbose_names.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0012_migrate_app_settings_from_local_py_to_database.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0013_fleetcomm_channel.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0013_fleetcomm_channel.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0014_update_models.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0014_update_models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py` & `aa_fleetpings-3.1.1/fleetpings/migrations/0015_alter_discordpingtarget_options_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.js` & `aa_fleetpings-3.1.1/fleetpings/static/fleetpings/js/fleetpings.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.min.js` & `aa_fleetpings-3.1.1/fleetpings/static/fleetpings/js/fleetpings.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/js/fleetpings.min.js.map` & `aa_fleetpings-3.1.1/fleetpings/static/fleetpings/js/fleetpings.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/LICENSE` & `aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.js` & `aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js` & `aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js.map` & `aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/autocomplete.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/readme.md` & `aa_fleetpings-3.1.1/fleetpings/static/fleetpings/libs/bootstrap5-autocomplete/1.1.25/readme.md`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/base.html` & `aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/base.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/index.html` & `aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/index.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/form.html` & `aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/form.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html` & `aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/hints/ping-everyone.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html` & `aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/fleet-doctrine.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html` & `aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/fleet-type.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html` & `aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/form/segments/ping-targets.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html` & `aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/ping/copy-paste-text.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templates/fleetpings/partials/ping/ping.html` & `aa_fleetpings-3.1.1/fleetpings/templates/fleetpings/partials/ping/ping.html`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/templatetags/fleetpings.py` & `aa_fleetpings-3.1.1/fleetpings/templatetags/fleetpings.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_access.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_ajax_calls.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_auth_hooks.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_helper_eve_images.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_helper_eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_installed_modules.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_model_discprdpingtarget.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_model_discprdpingtarget.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleetcomm.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_model_fleetcomm.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleetdoctrine.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_model_fleetdoctrine.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_model_fleettype.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_model_fleettype.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_model_formuplocation.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_model_formuplocation.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_model_setting.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_model_setting.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_model_webhook.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_model_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/test_templatetags.py` & `aa_fleetpings-3.1.1/fleetpings/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/fleetpings/tests/utils.py` & `aa_fleetpings-3.1.1/fleetpings/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/LICENSE` & `aa_fleetpings-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/README.md` & `aa_fleetpings-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/pyproject.toml` & `aa_fleetpings-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_fleetpings-3.1.0/PKG-INFO` & `aa_fleetpings-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-fleetpings
-Version: 3.1.0
+Version: 3.1.1
 Summary: Fleet Ping Tool for Alliance Auth supporting pings via webhooks to Discord.
 Project-URL: Changelog, https://github.com/ppfeufer/aa-fleetpings/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-fleetpings/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-fleetpings
 Project-URL: Source, https://github.com/ppfeufer/aa-fleetpings.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-fleetpings/issues
```

