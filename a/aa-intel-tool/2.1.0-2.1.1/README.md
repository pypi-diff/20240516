# Comparing `tmp/aa_intel_tool-2.1.0.tar.gz` & `tmp/aa_intel_tool-2.1.1.tar.gz`

## Comparing `aa_intel_tool-2.1.0.tar` & `aa_intel_tool-2.1.1.tar`

### file list

```diff
@@ -1,130 +1,133 @@
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/__init__.py
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/admin.py
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/app_settings.py
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/apps.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/auth_hooks.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/constants.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/exceptions.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/form.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/models.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tasks.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/urls.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/helper/data_structure.py
--rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/helper/eve_character.py
--rw-r--r--   0        0        0    15632 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/django.pot
--rw-r--r--   0        0        0    15707 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18871 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16800 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18980 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15721 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    19059 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    15624 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15951 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    11779 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    21861 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    15702 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15925 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/management/commands/aa_intel_tool_load_eve_types.py
--rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/migrations/0001_initial.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/migrations/0002_alter_scan_raw_data.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/migrations/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/__init__.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/general.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/helper/db.py
--rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/module/chatlist.py
--rw-r--r--   0        0        0    13148 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/module/dscan.py
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/parser/module/fleetcomp.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/scripts/drop_tables.sql
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.css
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css.map
--rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.js
--rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js.map
--rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.js
--rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js
--rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js.map
--rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.js
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js.map
--rw-r--r--   0        0        0    23339 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.js
--rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js.map
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.js
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js.map
--rw-r--r--   0        0        0     8525 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.js
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js
--rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js.map
--rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.js
--rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js.map
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.js
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.min.js
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.min.js.map
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/base.html
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-chatscan-js.html
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-css.html
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-dscan-js.html
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-fleetcomp-js.html
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js.html
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/index/form.html
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/buttons.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/evetime.html
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid.html
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown.html
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/system-information.html
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/index.html
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templatetags/__init__.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/templatetags/aa_intel_tool.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/__init__.py
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_access.py
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_admin.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_app_settings.py
--rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_auth_hooks.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_helper_data_structures.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_models.py
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_parser.py
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_parser_helper_db.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test_templatetags.py
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/utils.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/chatscan-faulty.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/chatscan.txt
--rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan-german-client.txt
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan-russian-client.txt
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan.txt
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/fleetcomp.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/views/__init__.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/views/ajax.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/aa_intel_tool/views/general.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/.gitignore
--rw-r--r--   0        0        0    35151 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/LICENSE
--rw-r--r--   0        0        0    12916 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/README.md
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    55219 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/__init__.py
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/admin.py
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/app_settings.py
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/apps.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/auth_hooks.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/constants.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/exceptions.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/form.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/models.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tasks.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/urls.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/helper/data_structure.py
+-rw-r--r--   0        0        0     5134 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/helper/eve_character.py
+-rw-r--r--   0        0        0    15632 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/django.pot
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15879 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8931 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18877 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16820 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18972 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15721 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15675 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8735 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    19048 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15716 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15990 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    11779 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    21878 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15931 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15944 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/management/commands/aa_intel_tool_load_eve_types.py
+-rw-r--r--   0        0        0     4339 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/migrations/0001_initial.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/migrations/0002_alter_scan_raw_data.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/migrations/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/parser/__init__.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/parser/general.py
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/parser/helper/db.py
+-rw-r--r--   0        0        0    10666 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/parser/module/chatlist.py
+-rw-r--r--   0        0        0    13148 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/parser/module/dscan.py
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/parser/module/fleetcomp.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/scripts/drop_tables.sql
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.css
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css.map
+-rw-r--r--   0        0        0    10594 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.js
+-rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js.map
+-rw-r--r--   0        0        0    12512 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.js
+-rw-r--r--   0        0        0     4320 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js
+-rw-r--r--   0        0        0     4932 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js.map
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.js
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js.map
+-rw-r--r--   0        0        0    23333 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.js
+-rw-r--r--   0        0        0     8143 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js.map
+-rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.js
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js.map
+-rw-r--r--   0        0        0     8519 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.js
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js.map
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.js
+-rw-r--r--   0        0        0     3723 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js.map
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.js
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.min.js
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool.min.js.map
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/base.html
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-chatscan-js.html
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-css.html
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-dscan-js.html
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-fleetcomp-js.html
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js.html
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/index/form.html
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/buttons.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/evetime.html
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid.html
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown.html
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/system-information.html
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/views/index.html
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templatetags/__init__.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/templatetags/aa_intel_tool.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/__init__.py
+-rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test_access.py
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test_admin.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test_app_settings.py
+-rw-r--r--   0        0        0     2451 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test_helper_data_structures.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test_models.py
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test_parser.py
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test_parser_helper_db.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/utils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test-data/chatscan-faulty.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test-data/chatscan.txt
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test-data/dscan-german-client.txt
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test-data/dscan-russian-client.txt
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test-data/dscan.txt
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/tests/test-data/fleetcomp.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/views/__init__.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/views/ajax.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/aa_intel_tool/views/general.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/.gitignore
+-rw-r--r--   0        0        0    35151 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/LICENSE
+-rw-r--r--   0        0        0    12916 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/README.md
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    55219 2020-02-02 00:00:00.000000 aa_intel_tool-2.1.1/PKG-INFO
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/admin.py` & `aa_intel_tool-2.1.1/aa_intel_tool/admin.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/app_settings.py` & `aa_intel_tool-2.1.1/aa_intel_tool/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/auth_hooks.py` & `aa_intel_tool-2.1.1/aa_intel_tool/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/constants.py` & `aa_intel_tool-2.1.1/aa_intel_tool/constants.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/exceptions.py` & `aa_intel_tool-2.1.1/aa_intel_tool/exceptions.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/models.py` & `aa_intel_tool-2.1.1/aa_intel_tool/models.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tasks.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/urls.py` & `aa_intel_tool-2.1.1/aa_intel_tool/urls.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/helper/eve_character.py` & `aa_intel_tool-2.1.1/aa_intel_tool/helper/eve_character.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/django.pot` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/cs/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/cs/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

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
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Czech <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
@@ -184,14 +185,16 @@
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
 #: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
@@ -293,14 +296,16 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
@@ -318,14 +323,16 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
 msgid ""
 "Please keep in mind, parsing large amounts of data can take some time. Be "
 "patient, CCP's API is not the fastest to answer …"
 msgstr ""
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/de/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/de/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-intel-tool/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "(System Error) Something unexpected happened."
 msgstr "(Systemfehler) Es ist etwas Unerwartetes passiert."
 
 msgid ": activate to sort column ascending"
 msgstr ": aktivieren, um die Spalte aufsteigend zu sortieren"
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/de/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2023-10-04 15:46+0000\n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/de/>\n"
+"Language-Team: German <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/es/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/es/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-intel-tool/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "A parser error occurred » {message}"
 msgstr "Se produjo un error del analizador » {message}"
 
 msgid "Alliance list"
 msgstr "Lista de Alianzas"
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/es/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/es/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

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
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2023-10-25 07:04+0000\n"
-"Last-Translator: Geovanny David Morales De la cruz "
-"<moralesgeovanny1996@gmail.com>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/es/>\n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
+"Last-Translator: Geovanny David Morales De la cruz <moralesgeovanny1996@gmail"
+".com>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-intel-tool/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "(System Error) Something unexpected happened."
 msgstr "(System Error) un imprévu est arrivé."
 
 msgid ": activate to sort column ascending"
 msgstr ": activer pour trier les colonnes par ordre croissant"
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 # Matthias P <randomusernetcom@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2024-04-17 22:13+0000\n"
-"Last-Translator: Matthias P <randomusernetcom@gmail.com>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/fr/>\n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2023-10-04 15:46+0000\n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/ja/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2023-10-04 15:46+0000\n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/ja/>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-intel-tool/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "(System Error) Something unexpected happened."
 msgstr "(성계 오류) 예측하지 못한 오류 발생."
 
 msgid ": activate to sort column ascending"
 msgstr ": 열 오름차순으로 정렬 활성화"
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Author50CO <tkddlschry@gmail.com>, 2023.
+# Author50CO <tkddlschry@gmail.com>, 2023, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2023.
 # Mind of the Raven <okanieva@gmail.com>, 2024.
 # Rodpold Shard <rodpold@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2024-03-22 00:11+0000\n"
-"Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/ko/>\n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
+"Last-Translator: Rodpold Shard <rodpold@gmail.com>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
@@ -158,17 +158,16 @@
 #: aa_intel_tool/models.py:152 aa_intel_tool/models.py:153
 msgid "Scan data"
 msgstr "스캔 데이터"
 
 #: aa_intel_tool/parser/general.py:46
 msgid ""
 "No suitable parser found. Input is not a supported intel type or malformed …"
-msgstr ""
-"지원하는 파서를 찾을 수 없습니다. 지원하지 않는 인텔 타입이거나, 잘못된 형식"
-"입니다…"
+msgstr "지원하는 파서를 찾을 수 없습니다. 지원하지 않는 인텔 타입이거나, 잘못된 "
+"형식입니다…"
 
 #: aa_intel_tool/parser/general.py:80
 msgid "No data to parse …"
 msgstr "가져올 데이터가 없습니다…"
 
 #: aa_intel_tool/parser/module/chatlist.py:68
 msgid "Something went wrong while fetching the character information from ESI."
@@ -186,17 +185,16 @@
 #, python-brace-format
 msgid ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
-msgstr[0] ""
-"챗 스캔 파일럿 수는 최대 {max_allowed_pilots}명으로 제한되어 있습니다. 입력"
-"한 파일럿 수가 제한을 초과합니다."
+msgstr[0] "챗 스캔 파일럿 수는 최대 {max_allowed_pilots}명으로 제한되어 있습니다. "
+"입력한 파일럿 수가 제한을 초과합니다."
 
 #: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr "전방위 스캐너 모듈이 비활성화된 상태입니다."
 
 #: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
@@ -206,17 +204,16 @@
 msgid "Permalink successfully copied"
 msgstr "고유링크가 성공적으로 복사되었습니다"
 
 #: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:10
 msgid ""
 "Something went wrong. Nothing copied. Maybe your browser does not support "
 "this function."
-msgstr ""
-"뭔가 잘못됐습니다. 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 않을 수"
-"도 있습니다."
+msgstr "뭔가 잘못됐습니다. 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 않을 "
+"수도 있습니다."
 
 #: aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html:15
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:4
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:3
 msgid "Unaffiliated / No Alliance"
 msgstr "얼라이언스 없음"
@@ -328,16 +325,15 @@
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] "스캔 당 최대 %(max_pilots)s명으로 제한되어 있습니다."
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
 msgid ""
 "Please keep in mind, parsing large amounts of data can take some time. Be "
 "patient, CCP's API is not the fastest to answer …"
-msgstr ""
-"기억해주세요, 큰 데이터를 가져오는 데에는 시간이 걸립니다. CCP의 API는 느린 "
+msgstr "기억해주세요, 큰 데이터를 가져오는 데에는 시간이 걸립니다. CCP의 API는 느린 "
 "것으로 유명합니다, 조금만 기다려 주세요 …"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
 msgstr "전송"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/nl/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/sk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

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
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
@@ -183,14 +185,16 @@
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
 #: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
@@ -292,14 +296,16 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
@@ -317,14 +323,16 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
 msgid ""
 "Please keep in mind, parsing large amounts of data can take some time. Be "
 "patient, CCP's API is not the fastest to answer …"
 msgstr ""
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-intel-tool/pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 "Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
 "tłumaczenia?"
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/nl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2024.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2024-03-29 15:11+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Polish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/pl/>\n"
-"Language: pl_PL\n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.4.2\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
@@ -299,20 +299,18 @@
 msgstr[1] ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
-"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
-"tłumaczenia?"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "Dołącz do naszego zespołu tłumaczy!"
+msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:10
 msgid "What can I paste?"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:16
 msgid "Chat member list"
@@ -461,15 +459,15 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
 msgid "Total mass (in kg):"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
-msgstr "Typ statku"
+msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/evetime.html:5
 msgid "Scan taken at (Eve time)"
@@ -489,15 +487,15 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:6
 msgid "Who is flying what"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:22
 msgid "System"
-msgstr "System Solarny"
+msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/ru/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/ru/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-intel-tool/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "(System Error) Something unexpected happened."
 msgstr "(Системная ошибка) Случилось что-то непредвиденное."
 
 msgid ": activate to sort column ascending"
 msgstr ": активируйте для сортировки по возрастанию"
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/ru/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Nikolay <nick.postnikov@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
-# Max <mark25@inbox.ru>, 2023.
+# Nikolay <nick.postnikov@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Max <mark25@inbox.ru>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2023-10-04 15:47+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/ru/>\n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/sk/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
-#, fuzzy
+# Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/pl/>\n"
+"Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
@@ -184,14 +184,15 @@
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilot "
 "per scan. Your list of pilots exceeds this limit."
 msgid_plural ""
 "Chat scans are currently limited to a maximum of {max_allowed_pilots} pilots "
 "per scan. Your list of pilots exceeds this limit."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: aa_intel_tool/parser/module/dscan.py:350
 msgid "The D-Scan module is currently disabled."
 msgstr ""
 
 #: aa_intel_tool/parser/module/fleetcomp.py:111
 msgid "The fleet composition module is currently disabled."
@@ -293,24 +294,27 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/body/scan-retention-note.html:5
 #, python-format
 msgid "Scans will be deleted after %(scan_retention_time)s day."
 msgid_plural "Scans will be deleted after %(scan_retention_time)s days."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
+"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
+"tłumaczenia?"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr ""
+msgstr "Dołącz do naszego zespołu tłumaczy!"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:10
 msgid "What can I paste?"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:16
 msgid "Chat member list"
@@ -318,14 +322,15 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:21
 #, python-format
 msgid "Limited to a maximum of %(max_pilots)s pilot per scan."
 msgid_plural "Limited to a maximum of %(max_pilots)s pilots per scan."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:40
 msgid ""
 "Please keep in mind, parsing large amounts of data can take some time. Be "
 "patient, CCP's API is not the fastest to answer …"
 msgstr ""
 
@@ -459,15 +464,15 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
 msgid "Total mass (in kg):"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
-msgstr ""
+msgstr "Typ statku"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:36
 msgid "No data."
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/evetime.html:5
 msgid "Scan taken at (Eve time)"
@@ -487,15 +492,15 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:6
 msgid "Who is flying what"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:22
 msgid "System"
-msgstr ""
+msgstr "System Solarny"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/uk/LC_MESSAGES/django.mo` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/uk/LC_MESSAGES/django.mo`

 * *Files 19% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,14 +8,14 @@
 "apps/aa-intel-tool/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Submit"
 msgstr "Відправити"
 
 msgid "System"
 msgstr "Система"
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/uk/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2023-10-04 15:47+0000\n"
+"PO-Revision-Date: 2024-05-10 14:07+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-intel-tool/uk/>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-intel-tool/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_intel_tool-2.1.1/aa_intel_tool/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Dehao Wu <wudehao2000@163.com>, 2024.
 # Faer Yili <yilifaer@gmail.com>, 2024.
+# SAM_FPS <sam_fps@163.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-20 22:33+0200\n"
-"PO-Revision-Date: 2024-01-11 21:04+0000\n"
-"Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
+"PO-Revision-Date: 2024-05-16 13:20+0000\n"
+"Last-Translator: SAM_FPS <sam_fps@163.com>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-intel-tool/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.5\n"
 
 #: aa_intel_tool/__init__.py:9
 #: aa_intel_tool/templates/aa_intel_tool/base.html:6
 #: aa_intel_tool/templates/aa_intel_tool/base.html:10
 #: aa_intel_tool/templates/aa_intel_tool/views/index.html:8
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html:5
 #: aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html:5
@@ -56,15 +57,15 @@
 msgid "D-Scan"
 msgstr ""
 
 #: aa_intel_tool/constants.py:70 aa_intel_tool/models.py:23
 #: aa_intel_tool/models.py:123
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:33
 msgid "Fleet composition"
-msgstr ""
+msgstr "舰队组成"
 
 #: aa_intel_tool/exceptions.py:34
 #, python-brace-format
 msgid "A parser error occurred » {message}"
 msgstr ""
 
 #: aa_intel_tool/form.py:20
@@ -324,15 +325,15 @@
 msgid ""
 "Please keep in mind, parsing large amounts of data can take some time. Be "
 "patient, CCP's API is not the fastest to answer …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:51
 msgid "Submit"
-msgstr ""
+msgstr "提交"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:56
 msgid "Working on it, please be patient …"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/index/form.html:58
 msgid "Detecting the intel type"
@@ -366,15 +367,15 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:18
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:24
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:21
 msgid "Count"
-msgstr ""
+msgstr "计数"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html:29
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html:25
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:37
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:30
@@ -448,15 +449,15 @@
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown.html:17
 msgid "Off grid"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:21
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:19
 msgid "Ship class"
-msgstr ""
+msgstr "舰船等级"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html:30
 msgid "Total mass (in kg):"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html:18
 msgid "Ship type"
@@ -468,15 +469,15 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/evetime.html:5
 msgid "Scan taken at (Eve time)"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html:8
 msgid "Fleet details"
-msgstr ""
+msgstr "舰队细节"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html:12
 msgid "Pilots in fleet"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html:19
 msgid "Ship classes"
@@ -484,15 +485,15 @@
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:6
 msgid "Who is flying what"
 msgstr ""
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html:22
 msgid "System"
-msgstr ""
+msgstr "星系"
 
 #: aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html:8
 msgid "Participation details"
 msgstr ""
 
 #: aa_intel_tool/views/general.py:53
 msgid "The provided data could not be parsed."
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/management/commands/aa_intel_tool_load_eve_types.py` & `aa_intel_tool-2.1.1/aa_intel_tool/management/commands/aa_intel_tool_load_eve_types.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/migrations/0001_initial.py` & `aa_intel_tool-2.1.1/aa_intel_tool/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/parser/general.py` & `aa_intel_tool-2.1.1/aa_intel_tool/parser/general.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/parser/helper/db.py` & `aa_intel_tool-2.1.1/aa_intel_tool/parser/helper/db.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/parser/module/chatlist.py` & `aa_intel_tool-2.1.1/aa_intel_tool/parser/module/chatlist.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/parser/module/dscan.py` & `aa_intel_tool-2.1.1/aa_intel_tool/parser/module/dscan.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/parser/module/fleetcomp.py` & `aa_intel_tool-2.1.1/aa_intel_tool/parser/module/fleetcomp.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.css` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.css`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css.map` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/css/aa-intel-tool.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js.map` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan-highlight.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js.map` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-chatscan.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js.map` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan-highlight.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/* global aaIntelToolJsL10n, aaIntelToolJsOptions, addDscanHightlight, removeDscanHightlight, changeDscanStickyHighlight, fetchAjaxData, shipInfoPanel, Intl */
+/* global aaIntelToolJsL10n, aaIntelToolJsOptions, addDscanHightlight, removeDscanHightlight, changeDscanStickyHighlight, fetchAjaxData, shipInfoPanel */
 
 $(() => {
     'use strict';
 
     const elementShipClassesAllTable = $('table.aa-intel-dscan-ship-classes-all-list');
     const elementDscanCountAll = $('span#aa-intel-dscan-all-count');
     const elementDscanMassAll = $('span#aa-intel-dscan-all-mass');
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js.map` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-dscan.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js.map` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition-highlight.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/* global fetchAjaxData, aaIntelToolJsOptions, aaIntelToolJsL10n, shipInfoPanel, pilotInfoPanel, addFleetcompositionHightlight, removeFleetcompositionHightlight, Intl */
+/* global fetchAjaxData, aaIntelToolJsOptions, aaIntelToolJsL10n, shipInfoPanel, pilotInfoPanel, addFleetcompositionHightlight, removeFleetcompositionHightlight */
 
 $(() => {
     'use strict';
 
     const elementShipClassesTable = $('table.aa-intel-dscan-ship-classes-ship-classes-list');
     const elementShipClassesMass = $('span#aa-intel-dscan-ship-classes-mass');
     const elementShipTypesTable = $('table.aa-intel-dscan-ship-types-list');
```

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js.map` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-fleetcomposition.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js.map` & `aa_intel_tool-2.1.1/aa_intel_tool/static/aa_intel_tool/javascript/aa-intel-tool-scan-result-common.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/base.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/base.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-fleetcomp-js.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-fleetcomp-js.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/bundles/aa-intel-tool-js-l10n.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/index/form.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/index/form.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/buttons.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/buttons.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/alliances.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/corporations.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/chatlist/pilots.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/interesting-on-grid/items.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-classes.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/dscan/ships-breakdown/ship-types.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/participation.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/partials/scan/fleetcomp/fleet-details/pilots.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/index.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/views/index.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/views/scan/chatlist.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/views/scan/dscan.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html` & `aa_intel_tool-2.1.1/aa_intel_tool/templates/aa_intel_tool/views/scan/fleetcomp.html`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/templatetags/aa_intel_tool.py` & `aa_intel_tool-2.1.1/aa_intel_tool/templatetags/aa_intel_tool.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_access.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_admin.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_app_settings.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_auth_hooks.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_helper_data_structures.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test_helper_data_structures.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_models.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_parser.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_parser_helper_db.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test_parser_helper_db.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test_templatetags.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/utils.py` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan-german-client.txt` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test-data/dscan-german-client.txt`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan-russian-client.txt` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test-data/dscan-russian-client.txt`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/tests/test-data/dscan.txt` & `aa_intel_tool-2.1.1/aa_intel_tool/tests/test-data/dscan.txt`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/views/ajax.py` & `aa_intel_tool-2.1.1/aa_intel_tool/views/ajax.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/aa_intel_tool/views/general.py` & `aa_intel_tool-2.1.1/aa_intel_tool/views/general.py`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/LICENSE` & `aa_intel_tool-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/README.md` & `aa_intel_tool-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/pyproject.toml` & `aa_intel_tool-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_intel_tool-2.1.0/PKG-INFO` & `aa_intel_tool-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-intel-tool
-Version: 2.1.0
+Version: 2.1.1
 Summary: A simple parser for D-Scans and more for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-intel-tool/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-intel-tool/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-intel-tool
 Project-URL: Source, https://github.com/ppfeufer/aa-intel-tool.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-intel-tool/issues
```

