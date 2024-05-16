# Comparing `tmp/allianceauth_afat-3.0.0b3.tar.gz` & `tmp/allianceauth_afat-3.0.1.tar.gz`

## Comparing `allianceauth_afat-3.0.0b3.tar` & `allianceauth_afat-3.0.1.tar`

### file list

```diff
@@ -1,173 +1,181 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/__init__.py
--rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/admin.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/app_settings.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/apps.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/auth_hooks.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/constants.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/forms.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/managers.py
--rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/models.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/providers.py
--rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tasks.py
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/urls.py
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/utils.py
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/helper/fatlinks.py
--rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/helper/time.py
--rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/helper/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/.gitkeep
--rw-r--r--   0        0        0    32113 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/django.pot
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/de/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0    25445 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    42914 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/es/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    34543 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/fr_FR/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    32576 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/it_IT/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    32437 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/ja/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    32240 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/ko_KR/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    33035 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/ru/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0    32170 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    49843 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    34042 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/zh_Hans/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    33103 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/management/commands/afat_import_from_allianceauth_fat.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0001_initial.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0002_manualfat.py
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0003_auto_20180911_0831.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0004_clickfatduration.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0005_auto_20200816_2042.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0006_auto_20200820_2013.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0007_auto_20200826_1537.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0008_auto_20200912_1116.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0009_auto_20200925_2206.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0010_permissoins_update_20201002_1909.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0011_change_meta_options_on_manualafat_20201003_2222.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0012_manualafat_created_at.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0013_basic_module_access_permissions.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0014_auto_20201224_0930.py
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0015_afatlink_character.py
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0016_permissions_overhaul.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0017_remove_soft_deletion.py
--rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0018_auto_20210420_2016.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0019_add_several_indices.py
--rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0020_auto_20210617_1037.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0021_alter_afatlink_fleet.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0022_afatlink_esi_error_count.py
--rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/0023_the_big_rename.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/migrations/__init__.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/css/afat.css
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/css/afat.min.css
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/css/afat.min.css.map
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-dashboard.js
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-dashboard.min.js
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-dashboard.min.js.map
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-datatables-common.js
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-datatables-common.min.js
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-datatables-common.min.js.map
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlink-details.js
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlink-details.min.js
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlink-details.min.js.map
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlist.js
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlist.min.js
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlist.min.js.map
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-logs.js
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-logs.min.js
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-logs.min.js.map
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-statistics.js
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-statistics.min.js
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-statistics.min.js.map
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat.js
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat.min.js
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat.min.js.map
--rw-r--r--   0        0        0   159639 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/libs/Chart.js/2.7.2/chart.min.js
--rw-r--r--   0        0        0   205125 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/libs/Chart.js/4.4.1/chart.umd.js
--rw-r--r--   0        0        0   953492 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/static/afat/libs/Chart.js/4.4.1/chart.umd.js.map
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/base.html
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/bundles/afat-css.html
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/bundles/afat-dashboard-js.html
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/bundles/afat-datatables-common-js.html
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/bundles/afat-fatlink-details-js.html
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/bundles/afat-fatlist-js.html
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/bundles/afat-js.html
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/bundles/afat-logs-js.html
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/bundles/afat-statistics-js.html
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/bundles/chartjs-js.html
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/modals/general.html
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/common/navigation/month-navigation.html
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/common/navigation/tab-character.html
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/common/navigation/tab.html
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/common/navigation/top-menu.html
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/common/navigation/year-navigation.html
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/dashboard/tabs-navigation.html
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/dashboard/tabs/fatlinks.html
--rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/dashboard/tabs/fats.html
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/fatlink-list-legend.html
--rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/open-esi-fleets.html
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/add/clickable-link.html
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/add/esi-link.html
--rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/fatlink-info.html
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/tabs-navigation.html
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/tabs/fats.html
--rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/form/required-field-hint.html
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/alliance/tabs-navigation.html
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/alliance/tabs/corporations.html
--rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/alliance/tabs/graphs.html
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/character/tabs-navigation.html
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/character/tabs/graphs.html
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/character/tabs/raw_data.html
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/corporation/tabs-navigation.html
--rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/corporation/tabs/graphs.html
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/corporation/tabs/member.html
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/overview/tabs-navigation.html
--rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/overview/tabs/corps.html
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/overview/tabs/mine.html
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/dashboard/dashboard.html
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/fatlinks/fatlinks-overview.html
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/logs/logs-overview.html
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-alliance-year-overview.html
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-alliance.html
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-character.html
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-corporation-year-overview.html
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-corporation.html
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-overview.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templatetags/__init__.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/templatetags/afat.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/__init__.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/test_access.py
--rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/test_helpers.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/test_templatetags.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/test_views_dashboard.py
--rw-r--r--   0        0        0    11270 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/test_views_fatlinks.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/test_views_logs.py
--rw-r--r--   0        0        0    17641 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/test_views_statistics.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/fixtures/allianceauth.json
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/fixtures/generate_fat_links.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/fixtures/load_allianceauth.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/tests/fixtures/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/views/__init__.py
--rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/views/dashboard.py
--rw-r--r--   0        0        0    36705 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/views/fatlinks.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/views/logs.py
--rw-r--r--   0        0        0    21807 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/afat/views/statistics.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/LICENSE
--rw-r--r--   0        0        0    13092 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/README.md
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/pyproject.toml
--rw-r--r--   0        0        0    55375 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/__init__.py
+-rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/admin.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/app_settings.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/apps.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/auth_hooks.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/constants.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/forms.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/managers.py
+-rw-r--r--   0        0        0     9167 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/models.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/providers.py
+-rw-r--r--   0        0        0     8530 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tasks.py
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/urls.py
+-rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/utils.py
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/helper/fatlinks.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/helper/time.py
+-rw-r--r--   0        0        0     9716 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/helper/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/.gitkeep
+-rw-r--r--   0        0        0    33266 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/django.pot
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    33621 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/de/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0    25858 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    44235 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/es/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    35755 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/fr_FR/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    34367 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/it_IT/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    33596 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/ja/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    33386 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/ko_KR/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     4411 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    34942 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    33354 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    33957 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/ru/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0    29816 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    53015 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    33617 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    35233 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/zh_Hans/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    34814 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/management/commands/afat_import_from_allianceauth_fat.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0002_manualfat.py
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0003_auto_20180911_0831.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0004_clickfatduration.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0005_auto_20200816_2042.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0006_auto_20200820_2013.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0007_auto_20200826_1537.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0008_auto_20200912_1116.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0009_auto_20200925_2206.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0010_permissoins_update_20201002_1909.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0011_change_meta_options_on_manualafat_20201003_2222.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0012_manualafat_created_at.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0013_basic_module_access_permissions.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0014_auto_20201224_0930.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0015_afatlink_character.py
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0016_permissions_overhaul.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0017_remove_soft_deletion.py
+-rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0018_auto_20210420_2016.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0019_add_several_indices.py
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0020_auto_20210617_1037.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0021_alter_afatlink_fleet.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0022_afatlink_esi_error_count.py
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/0023_the_big_rename.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/migrations/__init__.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/css/afat.css
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/css/afat.min.css
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/css/afat.min.css.map
+-rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-dashboard.js
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-dashboard.min.js
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-dashboard.min.js.map
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-datatables-common.js
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-datatables-common.min.js
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-datatables-common.min.js.map
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlink-details.js
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlink-details.min.js
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlink-details.min.js.map
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlist.js
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlist.min.js
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlist.min.js.map
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-logs.js
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-logs.min.js
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-logs.min.js.map
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-statistics.js
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-statistics.min.js
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-statistics.min.js.map
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat.js
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat.min.js
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/javascript/afat.min.js.map
+-rw-r--r--   0        0        0   159639 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/libs/Chart.js/2.7.2/chart.min.js
+-rw-r--r--   0        0        0   205125 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/libs/Chart.js/4.4.1/chart.umd.js
+-rw-r--r--   0        0        0   953492 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/static/afat/libs/Chart.js/4.4.1/chart.umd.js.map
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/base.html
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/bundles/afat-css.html
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/bundles/afat-dashboard-js.html
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/bundles/afat-datatables-common-js.html
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/bundles/afat-fatlink-details-js.html
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/bundles/afat-fatlist-js.html
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/bundles/afat-js.html
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/bundles/afat-logs-js.html
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/bundles/afat-statistics-js.html
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/bundles/chartjs-js.html
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/modals/general.html
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/common/navigation/month-navigation.html
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/common/navigation/tab-character.html
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/common/navigation/tab.html
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/common/navigation/top-menu.html
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/common/navigation/year-navigation.html
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/dashboard/tabs-navigation.html
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/dashboard/tabs/fatlinks.html
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/dashboard/tabs/fats.html
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/fatlink-list-legend.html
+-rw-r--r--   0        0        0     3464 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/open-esi-fleets.html
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/add/clickable-link.html
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/add/esi-link.html
+-rw-r--r--   0        0        0     4961 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/fatlink-info.html
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/tabs-navigation.html
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/tabs/fats.html
+-rw-r--r--   0        0        0     3655 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/form/required-field-hint.html
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/alliance/tabs-navigation.html
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/alliance/tabs/corporations.html
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/alliance/tabs/graphs.html
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/character/tabs-navigation.html
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/character/tabs/graphs.html
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/character/tabs/raw_data.html
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/corporation/tabs-navigation.html
+-rw-r--r--   0        0        0     5309 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/corporation/tabs/graphs.html
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/corporation/tabs/member.html
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/overview/tabs-navigation.html
+-rw-r--r--   0        0        0     6034 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/overview/tabs/corps.html
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/overview/tabs/mine.html
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/dashboard/dashboard.html
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/fatlinks/fatlinks-overview.html
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/logs/logs-overview.html
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-alliance-year-overview.html
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-alliance.html
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-character.html
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-corporation-year-overview.html
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-corporation.html
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-overview.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templatetags/__init__.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/templatetags/afat.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/__init__.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/test_access.py
+-rw-r--r--   0        0        0    15411 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/test_helpers.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/test_views_dashboard.py
+-rw-r--r--   0        0        0    11270 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/test_views_fatlinks.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/test_views_logs.py
+-rw-r--r--   0        0        0    17641 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/test_views_statistics.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/fixtures/allianceauth.json
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/fixtures/generate_fat_links.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/fixtures/load_allianceauth.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/tests/fixtures/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/views/__init__.py
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/views/dashboard.py
+-rw-r--r--   0        0        0    36705 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/views/fatlinks.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/views/logs.py
+-rw-r--r--   0        0        0    21807 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/afat/views/statistics.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/LICENSE
+-rw-r--r--   0        0        0    13443 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/README.md
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0    55776 2020-02-02 00:00:00.000000 allianceauth_afat-3.0.1/PKG-INFO
```

### Comparing `allianceauth_afat-3.0.0b3/afat/admin.py` & `allianceauth_afat-3.0.1/afat/admin.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/app_settings.py` & `allianceauth_afat-3.0.1/afat/app_settings.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/auth_hooks.py` & `allianceauth_afat-3.0.1/afat/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/forms.py` & `allianceauth_afat-3.0.1/afat/forms.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/managers.py` & `allianceauth_afat-3.0.1/afat/managers.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/models.py` & `allianceauth_afat-3.0.1/afat/models.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tasks.py` & `allianceauth_afat-3.0.1/afat/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/urls.py` & `allianceauth_afat-3.0.1/afat/urls.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/utils.py` & `allianceauth_afat-3.0.1/afat/utils.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/helper/fatlinks.py` & `allianceauth_afat-3.0.1/afat/helper/fatlinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/helper/time.py` & `allianceauth_afat-3.0.1/afat/helper/time.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/helper/views.py` & `allianceauth_afat-3.0.1/afat/helper/views.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/django.pot` & `allianceauth_afat-3.0.1/afat/locale/cs/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,38 @@
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
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-03-20 16:54+0100\n"
+"PO-Revision-Date: 2024-05-10 14:14+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Czech <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/allianceauth-afat/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
 msgstr ""
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
 msgid "Fleet type"
 msgstr ""
 
 #: afat/admin.py:169
 msgid "Is enabled"
 msgstr ""
 
@@ -41,56 +42,64 @@
 
 #: afat/admin.py:213
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: afat/admin.py:223
 #, python-brace-format
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: afat/admin.py:229
 msgid "Deactivate selected fleet types"
 msgstr ""
 
 #: afat/admin.py:258
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: afat/admin.py:268
 #, python-brace-format
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: afat/apps.py:20
 #, python-brace-format
 msgid "AFAT - Another Fleet Activity Tracker v{__version__}"
 msgstr ""
 
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
 msgstr ""
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 msgid "Fleet name"
 msgstr ""
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
 msgstr ""
 
@@ -99,22 +108,22 @@
 msgstr ""
 
 #: afat/forms.py:62
 msgid "Character Name"
 msgstr ""
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
 msgstr ""
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
 msgstr ""
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
 msgstr ""
 
@@ -125,61 +134,61 @@
 #: afat/helper/time.py:115
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+msgid "ESI"
 msgstr ""
 
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr ""
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 msgid "Stop tracking"
 msgstr ""
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
 msgstr ""
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
 msgstr ""
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
 msgstr ""
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr ""
@@ -265,687 +274,723 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr ""
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr ""
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr ""
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr ""
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr ""
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr ""
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr ""
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr ""
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr ""
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr ""
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr ""
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr ""
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr ""
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr ""
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr ""
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr ""
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr ""
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr ""
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr ""
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr ""
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
 msgid "Fleet activity tracking"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
+msgstr ""
+
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr ""
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr ""
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:14
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+msgid "Create a FAT link using ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr ""
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
-msgstr ""
-
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
 "\n"
 "                You currently have %(open_esi_fleets)s active ESI fleets "
 "under the following characters:\n"
 "            "
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
 "            "
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: afat/templates/afat/partials/form/required_field_hint.html:4
+#: afat/templates/afat/partials/form/required-field-hint.html:4
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr ""
 
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
 msgid "Member corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
 msgid "Corporation statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
 msgid "Corporation performance"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+msgid "Ship Types"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+msgid "Average # of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
-msgid "FATs by time of day"
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
+msgid "FATs by time of day"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
-msgstr ""
-
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+msgid "Click on an alliance name to see their corporations"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+msgid "Alliance statistics for"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+msgid "Corporation statistics for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr ""
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
+#: afat/templates/afat/view/logs/logs-overview.html:6
 msgid "Fleet activity tracking logs"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
-msgstr ""
-
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
 msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, python-format
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
+
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
 msgid "Fleet activity tracking statistics"
 msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
 msgid "Fleet activity"
 msgstr ""
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
 msgstr ""
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
 msgstr ""
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
 msgstr ""
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
 msgstr ""
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
 msgstr ""
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
 msgstr ""
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
 msgstr ""
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
 msgstr ""
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
 msgstr ""
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
 msgstr ""
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
 msgstr ""
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
 msgstr ""
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
@@ -1108,54 +1153,54 @@
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
 msgstr ""
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
 msgstr ""
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
 msgstr ""
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
 msgstr ""
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
 msgstr ""
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
 msgstr ""
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
 msgstr ""
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr ""
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/de/LC_MESSAGES/django.mo` & `allianceauth_afat-3.0.1/afat/locale/de/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,39 +7,40 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/allianceauth-afat/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 "\n"
 "                    Diese Option wird die Flotte automatisch registrieren "
 "und tracken. Es muss kein Link in der Flotte geteilt werden.<br><b>Nutze "
 "diese Option wenn Du der Flottenkommandant bist</b>, ansonsten nutze die "
 "Option für klickbare FAT-Links.\n"
 "                "
 
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 "\n"
 "                    Piloten die Deiner Flotte beitreten werden automatisch "
 "zu diesem FAT-Link hinzugefügt bis die Flotte geschlossen in Eve wird (Du "
@@ -82,21 +83,31 @@
 "\n"
 "                Du hast aktuell %(open_esi_fleets)s aktive ESI Flotten mit "
 "den folgenden Charakteren:\n"
 "            "
 
 msgid ""
 "\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
 "        "
-msgstr ""
+msgid_plural ""
 "\n"
-"            Logs werden nur für %(log_duration)s Tage gespeichert. Danach "
-"werden sie automatisch gelöscht.\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+"\n"
+"            Logs werden für %(log_duration)s Tage gespeichert. Danach werden "
+"sie automatisch gelöscht.\n"
+"        "
+msgstr[1] ""
+"\n"
+"            Logs werden für %(log_duration)s Tage gespeichert. Danach werden "
+"sie automatisch gelöscht.\n"
 "        "
 
 msgid "# of FATs"
 msgstr "Anz. FATs"
 
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr "<h4>Fehler!</h4><p>Datumsinformationen nicht komplett.</p>"
@@ -359,20 +370,26 @@
 
 msgid "Add manual FAT"
 msgstr "Manuellen FAT hinzufügen"
 
 msgid "All FAT links"
 msgstr "Alle FAT-Links"
 
+msgid "Alliance statistics for"
+msgstr "Allianz-Statistik für"
+
 msgid "April"
 msgstr "April"
 
 msgid "August"
 msgstr "August"
 
+msgid "Average # of FATs"
+msgstr "Durchschnittliche Anz. FATs"
+
 msgid "Average FATs by corporation"
 msgstr "Durchschnittliche FATs nach Corporation"
 
 msgid "Avg FATs"
 msgstr "Durschn. FATs"
 
 msgid "Can access the AFAT module"
@@ -410,21 +427,27 @@
 
 msgid "Character this FAT link has been created with"
 msgstr "Der Charakter durch den dieser FAT-Link erstellt wurde"
 
 msgid "Character who registered this FAT"
 msgstr "Charakter welcher diesen FAT registriert hat"
 
+msgid "Click on an alliance name to see their corporations"
+msgstr "Klicke auf eine Allianz um deren Corporations zu sehen"
+
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr ""
 "Klicke hier um das automatische Tracking mittels ESI für diese Flotte zu "
 "stoppen und den FAT-Link zu schließen."
 
+msgid "Close"
+msgstr "Schließen"
+
 msgid "Close ESI Fleet Tracking"
 msgstr "ESI Tracking beenden"
 
 msgid "Close ESI fleet tracking"
 msgstr "ESI-Tracking beenden"
 
 msgid "Confirm"
@@ -438,33 +461,29 @@
 
 msgid "Corporation performance"
 msgstr "Corporation-Performance"
 
 msgid "Corporation statistics"
 msgstr "Corporation-Statistik"
 
+msgid "Corporation statistics for"
+msgstr "Corporation-Statistik für"
+
 msgid "Corporations"
 msgstr "Corporations"
 
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
-msgstr ""
-"Corporations <small>(Klicke auf eine Allianz um deren Corporations zu "
-"sehen)</small>"
-
 msgid "Count"
 msgstr "Anzahl"
 
-msgid "Create FAT link using ESI"
-msgstr "ESI-Link erstellen"
-
 msgid "Create a FAT link"
 msgstr "FAT-Link erstellen"
 
+msgid "Create a FAT link using ESI"
+msgstr "ESI-Link erstellen"
+
 msgid "Create a clickable FAT link"
 msgstr "Klickbaren FAT-Link erstellen"
 
 msgid "Create link"
 msgstr "Link erstellen"
 
 msgid "Creator"
@@ -472,14 +491,17 @@
 
 msgid "Current month"
 msgstr "Aktueller Monat"
 
 msgid "Current year"
 msgstr "Aktuelles Jahr"
 
+msgid "Dashboard"
+msgstr "Dashboard"
+
 msgid "Deactivate selected fleet types"
 msgstr "Deaktiviere ausgewählte Flottenarten"
 
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
 msgstr[0] "{notifications_count} Flottenart deaktiviert"
 msgstr[1] "{notifications_count} Flottenarten deaktiviert"
@@ -505,14 +527,17 @@
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 "Du möchtest helfen diese App in Deine Sprache zu übersetzen oder die "
 "bestehende Übersetzung verbessern?"
 
+msgid "ESI"
+msgstr "ESI"
+
 msgid "ESI fleet ID"
 msgstr "ESI Flotten ID"
 
 msgid "Enter fleet name"
 msgstr "Flottenname hier eintragen"
 
 msgid "Eve time"
@@ -783,15 +808,15 @@
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 "Nur Charaktere mit kürzlichen FATs werden angezeigt. <small>(Letzte 10 FATs "
 "je Charakter)</small>"
 
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr "Nur Monate in denen auch FAT-Links registriert sind werden angezeigt."
 
 msgid "Participation has been tracked via ESI"
 msgstr "Teilnahme wurde mittels ESI verfolgt"
 
 msgid "Participation is being tracked via ESI"
 msgstr "Teilnahme wird mittels ESI verfolgt"
@@ -825,14 +850,17 @@
 
 msgid "Set name"
 msgstr "Name setzen"
 
 msgid "Ship"
 msgstr "Schiff"
 
+msgid "Ship Types"
+msgstr "Schiffstypen"
+
 msgid "Ship type"
 msgstr "Schiffstyp"
 
 msgid "Ship type overview"
 msgstr "Schiffsübersicht"
 
 msgid "Statistics"
@@ -886,17 +914,14 @@
 
 msgid "Thursday"
 msgstr "Donnerstag"
 
 msgid "Time"
 msgstr "Zeit"
 
-msgid "Toggle navigation"
-msgstr "Navigation umschalten"
-
 msgid "Tuesday"
 msgstr "Dienstag"
 
 msgid "User"
 msgstr "Nutzer"
 
 msgid "View log"
@@ -922,17 +947,14 @@
 
 msgid "Your monthly stats"
 msgstr "Deine monatliche Statistik"
 
 msgid "Your most recent FATs"
 msgstr "Deine neuesten FAT-Links"
 
-msgid "via ESI"
-msgstr "mittels ESI"
-
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 "{int(duration_years[0])} Jahre, {int(duration_days[0])} Tage, "
 "{int(duration_hours[0])} Stunden, {int(duration_minutes[0])} Minuten und "
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/de/LC_MESSAGES/django.po` & `allianceauth_afat-3.0.1/afat/locale/de/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Peter Pfeufer <rounon.dax@terra-nanotech.de>, 2022
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 #
 # Translators:
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: 2023-10-02 09:50+0000\n"
+"POT-Creation-Date: 2024-03-16 03:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:14+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/allianceauth-afat/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
 msgstr "Flottenaktivitäts-Tracking"
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
 msgid "Fleet type"
 msgstr "Flottenart"
 
 #: afat/admin.py:169
 msgid "Is enabled"
 msgstr "Ist aktiviert"
 
@@ -83,18 +82,18 @@
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
 msgstr "Dies ist ein Pflichtfeld"
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 msgid "Fleet name"
 msgstr "Flottenname"
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
 msgstr "Flottenname hier eintragen"
 
@@ -103,22 +102,22 @@
 msgstr "Flottenart (optional)"
 
 #: afat/forms.py:62
 msgid "Character Name"
 msgstr "Charaktername"
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
 msgstr "System"
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
 msgstr "Schiffstyp"
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
 msgstr "FAT-Link Ablaufzeit in Minuten"
 
@@ -132,68 +131,68 @@
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 "{int(duration_years[0])} Jahre, {int(duration_days[0])} Tage, "
 "{int(duration_hours[0])} Stunden, {int(duration_minutes[0])} Minuten und "
 "{int(duration_seconds[0])} Sekunden"
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
-msgstr "mittels ESI"
-
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+msgid "ESI"
+msgstr "ESI"
+
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr ""
 "Klicke hier um das automatische Tracking mittels ESI für diese Flotte zu "
 "stoppen und den FAT-Link zu schließen."
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
 "<p>Bist Du sicher das Du die ESI Flotte mit ID {fatlink.esi_fleet_id} von "
 "{fatlink.character.character_name} schließen möchtest?</p>"
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 msgid "Stop tracking"
 msgstr "Tracking stoppen"
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
 msgstr "Löschen"
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
 msgstr ""
 "<p>Bist Du sicher das Du den FAT-Link {fatlink_fleet} löschen möchtest?</p>"
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
 msgstr ""
 "<p>Bist Du sicher das Du {fat.character.character_name} von diesem FAT-Link "
 "löschen möchtest?</p>"
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
 msgstr "{log.fatlink_hash} (Gelöscht)"
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr "Kann auf das AFAT Modul zugreifen"
@@ -281,131 +280,179 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr "Ist die Flotte zu diesem FAT-Link in ESI verfügbar oder nicht"
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr "Wurde dieser FAT-Link wieder geöffnet?"
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr "FAT-Link"
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr "FAT-Links"
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr "FAT-Link Laufzeit"
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr "FAT-Link Laufzeiten"
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr "Charakter welcher diesen FAT registriert hat"
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr "Der FAT-Link zu dem der Charakter registriert ist"
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr "Das System in dem der Charakter ist"
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr "Das Schiff welches der Charakter geflogen ist"
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr "FAT"
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr "FATs"
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr "Fat-Link erstellt"
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr "Fat-Link geändert"
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr "Fat-Link entfernt"
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr "Fat-Link wieder geöffnet"
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr "FAT entfernt"
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr "Manueller FAT Eintrag hinzugefügt"
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr "Log"
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr "Logs"
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
 msgid "Fleet activity tracking"
 msgstr "Flottenaktivitäts-Tracking"
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
+msgstr "Schließen"
+
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
 msgstr "Abbrechen"
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr "Bestätigen"
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr "Vorheriger Monat"
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr "Nächster Monat"
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr "Aktueller Monat"
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr "Dashboard"
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr "Statistik"
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr "FAT-Link hinzufügen"
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr "Log ansehen"
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr "Vorheriger Monat"
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr "Nächstes Jahr"
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr "Aktuelles Jahr"
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr "Neueste FAT-Links <small>(letzten 10)</small>"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
 msgstr "Ersteller"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
 msgstr "EVE Zeit"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
 msgstr "Aktionen"
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr "Deine neuesten FAT-Links"
 
@@ -413,227 +460,227 @@
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 "Nur Charaktere mit kürzlichen FATs werden angezeigt. <small>(Letzte 10 FATs "
 "je Charakter)</small>"
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr "Ort"
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
 msgstr "Schiff"
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr "Keine Aktivität für Deine Charaktere registriert."
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr "Klickbaren FAT-Link erstellen"
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 "Diese Option erstellt einen klickbaren Link den Du in der Flotte teilen "
 "kannst."
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
 msgstr "Link erstellen"
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+msgid "Create a FAT link using ESI"
 msgstr "ESI-Link erstellen"
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 "\n"
 "                    Diese Option wird die Flotte automatisch registrieren "
 "und tracken. Es muss kein Link in der Flotte geteilt werden.<br><b>Nutze "
 "diese Option wenn Du der Flottenkommandant bist</b>, ansonsten nutze die "
 "Option für klickbare FAT-Links.\n"
 "                "
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 "\n"
 "                    Piloten die Deiner Flotte beitreten werden automatisch "
 "zu diesem FAT-Link hinzugefügt bis die Flotte geschlossen in Eve wird (Du "
 "verlässt die Flotte ingame) oder Du das Tracking hier stoppst.\n"
 "                "
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr "ESI-Link hinzufügen"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr "Link erstellt (Eve Zeit)"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr "Link läuft ab (Eve Zeit)"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr "Link abgelaufen (Eve Zeit)"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr "Teilnahme wird mittels ESI verfolgt"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 "<p>Bist Du sicher das Du die ESI Flotte mit ID %(esi_fleet_id)s von "
 "%(character_name)s schließen möchtest?</p>"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr "Teilnahme wurde mittels ESI verfolgt"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 "Dieser Link ist bereits angelaufen aber noch in der Nachfrist<br>von "
 "%(reopen_grace_time)s Minuten um ihn wieder zu öffnen."
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
 "<p>Bist Du sicher das Du diesen FAT-Link für weitere %(reopen_duration)s "
 "Minuten wieder öffnen willst?<br>FAT-Links können nur einmal wieder geöffnet "
 "werden!<br><em>(Diese Aktion wird geloggt)</em></p>"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr "Wieder öffnen"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr "FAT-Link wieder öffnen"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr "FAT-Link"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr "Kopier mich!"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr "ESI-Tracking beenden"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr "Name setzen"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr "Manueller FAT"
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
-msgstr ""
-"FATs für diesen FAT-Link <small>(alle 15 Sekunden aktualisiert)</small>"
+msgstr "FATs für diesen FAT-Link <small>(alle 15 Sekunden aktualisiert)</small>"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr "FATs für diesen FAT-Link"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
 msgstr "Charakter"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr "Schiffsübersicht"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
 msgstr "Anzahl"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
-msgstr "Manueller FAT"
-
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr ""
 "Es fehlen Piloten in der Liste dieses FATs? Nutze dieses Formular um sie "
 "manuell hinzuzufügen."
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr "Hinweis"
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr "Diese Aktion wird geloggt!"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr "Charaktername"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr "Manuellen FAT hinzufügen"
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr "Legende"
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr "Flotte ist momentan aktiv und FATs werden mittels ESI hinzugefügt"
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr "FATs wurden automatisch mittels ESI verfolgt"
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
@@ -648,19 +695,19 @@
 "            "
 msgstr[1] ""
 "\n"
 "                Du hast aktuell %(open_esi_fleets)s aktive ESI Flotten mit "
 "den folgenden Charakteren:\n"
 "            "
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr "ESI Flotten ID"
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
@@ -670,30 +717,30 @@
 "                Diese Flotte wird bereits automatisch verfolgt.\n"
 "            "
 msgstr[1] ""
 "\n"
 "                Diese Flotten werden bereits automatisch verfolgt.\n"
 "            "
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 "Du kannst jedoch weitere Flotten mit Deinen Alts starten, wenn Du möchtest."
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 "Hinweis: Informationen über registrierte Flotten können bis zu 5 Minuten "
 "verzögert sein."
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr "ESI Tracking beenden"
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -701,318 +748,301 @@
 "Du möchtest helfen diese App in Deine Sprache zu übersetzen oder die "
 "bestehende Übersetzung verbessern?"
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Tritt unserm Team von Übersetzern bei!"
 
-#: afat/templates/afat/partials/form/required_field_hint.html:4
+#: afat/templates/afat/partials/form/required-field-hint.html:4
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr "Mit einem Sternchen (*) gekennzeichnete Felder sind Pflichtfelder"
 
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr "Navigation umschalten"
-
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
-msgstr "Statistik"
-
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr "FAT-Link hinzufügen"
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr "Log ansehen"
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
-msgstr "Vorheriger Monat"
-
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
-msgstr "Nächster Monat"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
+msgstr "Grafiken"
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
-msgstr "Aktueller Monat"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
+msgstr "Corporations"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
 msgid "Member corporations"
 msgstr "Mitglieder-Corporations"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
 msgstr "Corporation"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr "Durschn. FATs"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
 msgid "Corporation statistics"
 msgstr "Corporation-Statistik"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr "FATs nach Schiffsart"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
 msgid "Corporation performance"
 msgstr "Corporation-Performance"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr "FATs nach Zeit"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr "FATs nach Wochentag"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+msgid "Ship Types"
+msgstr "Schiffstypen"
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr "Durchschnittliche FATs nach Corporation"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
-msgstr "Grafiken"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+msgid "Average # of FATs"
+msgstr "Durchschnittliche Anz. FATs"
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
+msgstr "Anz. FATs"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
-msgstr "Corporations"
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
+msgstr "Rohdaten"
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
 msgid "FATs by time of day"
 msgstr "FATs nach Tageszeit"
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
-msgstr "Anz. FATs"
-
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr "FATs für"
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
 msgstr "Name"
 
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
-msgstr "Rohdaten"
-
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr "Mitglieder"
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr "Charakterstatistik"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
-msgstr ""
-"Corporations <small>(Klicke auf eine Allianz um deren Corporations zu "
-"sehen)</small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
+msgstr "Meine Statistik"
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+msgid "Click on an alliance name to see their corporations"
+msgstr "Klicke auf eine Allianz um deren Corporations zu sehen"
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+msgid "Alliance statistics for"
+msgstr "Allianz-Statistik für"
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+msgid "Corporation statistics for"
+msgstr "Corporation-Statistik für"
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr "Deine monatliche Statistik"
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr "Nur Monate in denen auch FAT-Links registriert sind werden angezeigt."
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr ""
 "Nur Charaktere für die auch FAT-Links registriert sind werden angezeigt."
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
 msgstr "Monat"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr "FAT Anzahl"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr "Keine FATs für"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr "Keine FATs für dieses Jahr"
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr "Meine Statistik"
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr "Vorheriger Monat"
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr "Nächstes Jahr"
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr "Aktuelles Jahr"
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr "Kürzliche Aktivität"
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr "FAT-Link löschen"
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr "Keine FATs für"
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr "Keine FAT-Links"
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr "FAT-Link erstellen"
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr "FAT-Link Details"
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr "FAT löschen"
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr "Alle FAT-Links"
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
+#: afat/templates/afat/view/logs/logs-overview.html:6
 msgid "Fleet activity tracking logs"
 msgstr "Flottenaktivitäts-Tracking Logs"
 
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
-msgstr ""
-"\n"
-"            Logs werden nur für %(log_duration)s Tage gespeichert. Danach "
-"werden sie automatisch gelöscht.\n"
-"        "
-
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr "Zeit"
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr "Ereignis"
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
 msgstr "Nutzer"
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
 msgstr "Beschreibung"
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, python-format
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+"\n"
+"            Logs werden für %(log_duration)s Tage gespeichert. Danach werden "
+"sie automatisch gelöscht.\n"
+"        "
+msgstr[1] ""
+"\n"
+"            Logs werden für %(log_duration)s Tage gespeichert. Danach werden "
+"sie automatisch gelöscht.\n"
+"        "
+
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
 msgid "Fleet activity tracking statistics"
 msgstr "Flottenaktivitäts-Tracking Statistik"
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
 msgid "Fleet activity"
 msgstr "Flottenaktivität"
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
 msgstr "Januar"
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
 msgstr "Februar"
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
 msgstr "März"
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
 msgstr "April"
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
 msgstr "Mai"
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
 msgstr "Juni"
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
 msgstr "Juli"
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
 msgstr "August"
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
 msgstr "September"
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
 msgstr "Oktober"
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
 msgstr "November"
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
 msgstr "Dezember"
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
@@ -1213,73 +1243,73 @@
 "<h4>Erfolg!</h4><p>Der FAT für {character_name} wurde erfolgreich vom FAT-"
 "Link „{fatlink_hash}“ gelöscht.</p>"
 
 #: afat/views/fatlinks.py:1128
 msgid ""
 "<h4>Error!</h4><p>The hash you provided does not match with any FAT link.</p>"
 msgstr ""
-"<h4>Fehler!</h4><p>Der zur Verfügung gestellt Hash passt zu keinem FAT-Link."
-"</p>"
+"<h4>Fehler!</h4><p>Der zur Verfügung gestellt Hash passt zu keinem FAT-"
+"Link.</p>"
 
 #: afat/views/fatlinks.py:1174
 msgid "<h4>Success!</h4><p>The FAT link has been successfully re-opened.</p>"
 msgstr "<h4>Erfolg!</h4><p>Der FAT-Link wurde erfolgreich wieder geöffnet.</p>"
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 "<h4>Warnung!</h4><p>Dieser FAT-Link wurde bereits einmal wieder geöffnet. "
 "Dies kann nur einmal getan werden.</p>"
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
 "<h4>Warnung!</h4><p>Du hast nicht die Berechtigung die Statistiken für "
 "diesen Charakter zu sehen.</p>"
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr "<h4>Warnung!</h4><p>Datumsinformationen nicht komplett!</p>"
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
 "<h4>Warnung!</h4><p>Du hast nicht die Berechtigung die Statistiken für diese "
 "Corporation zu sehen.</p>"
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
 msgstr "Montag"
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
 msgstr "Dienstag"
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
 msgstr "Mittwoch"
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
 msgstr "Donnerstag"
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
 msgstr "Freitag"
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
 msgstr "Samstag"
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
 msgstr "Sonntag"
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr "<h4>Fehler!</h4><p>Datumsinformationen nicht komplett.</p>"
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/es/LC_MESSAGES/django.mo` & `allianceauth_afat-3.0.1/afat/locale/es/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/allianceauth-afat/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
 "<p>¿Está seguro de que desea cerrar la flota ESI con ID {fatlink."
 "esi_fleet_id} de {fatlink.character.character_name}?</p>"
@@ -157,29 +157,23 @@
 
 msgid "This field is mandatory"
 msgstr "Este campo es obligatorio"
 
 msgid "Thursday"
 msgstr "Jueves"
 
-msgid "Toggle navigation"
-msgstr "Alternar la navegación"
-
 msgid "Tuesday"
 msgstr "Martes"
 
 msgid "User"
 msgstr "Usuario"
 
 msgid "Wednesday"
 msgstr "Miércoles"
 
-msgid "via ESI"
-msgstr "vía ESI"
-
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 "{int(duration_years[0])} años, {int(duration_days[0])} días, "
 "{int(duration_hours[0])} horas, {int(duration_minutos[0])} minutos y "
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/es/LC_MESSAGES/django.po` & `allianceauth_afat-3.0.1/afat/locale/es/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"POT-Creation-Date: 2024-03-16 03:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:14+0000\n"
 "Last-Translator: Zigor Fernandez Moreno <sietehierros@gmail.com>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/allianceauth-afat/es/>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/allianceauth-afat/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
 msgstr "Seguimiento de la Actividad de Flota"
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
 #, fuzzy
 #| msgid "Fleet Type"
 msgid "Fleet type"
 msgstr "Tipo de Flota"
 
 #: afat/admin.py:169
 msgid "Is enabled"
@@ -82,18 +81,18 @@
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
 msgstr "Este campo es obligatorio"
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 #, fuzzy
 #| msgid "Fleet Name"
 msgid "Fleet name"
 msgstr "Nombre de la flota"
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
@@ -106,22 +105,22 @@
 msgstr "Tipo de flota (opcional)"
 
 #: afat/forms.py:62
 msgid "Character Name"
 msgstr ""
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
 msgstr "Sistema"
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
 msgstr "Tipo de Nave"
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
 msgstr "Tiempo de vencimiento del enlace FAT en minutos"
 
@@ -135,67 +134,69 @@
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 "{int(duration_years[0])} años, {int(duration_days[0])} días, "
 "{int(duration_hours[0])} horas, {int(duration_minutos[0])} minutos y "
 "{int(duration_segundos[0 ])} segundos"
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+#, fuzzy
+#| msgid "via ESI"
+msgid "ESI"
 msgstr "vía ESI"
 
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr ""
 "Al hacer clic aquí se detendrá el seguimiento automático a través de ESI "
 "para esta flota y se cerrará el enlace FAT asociado."
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
 "<p>¿Está seguro de que desea cerrar la flota ESI con ID {fatlink."
 "esi_fleet_id} de {fatlink.character.character_name}?</p>"
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 #, fuzzy
 #| msgid "Stop Tracking"
 msgid "Stop tracking"
 msgstr "Dejar de Rastrear"
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
 msgstr "Borrar"
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
 msgstr ""
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
 msgstr ""
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr ""
@@ -286,379 +287,428 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr ""
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr ""
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr ""
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr ""
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr ""
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr ""
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr ""
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr ""
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr ""
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr ""
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr ""
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr ""
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr ""
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr ""
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr ""
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr ""
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr ""
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr ""
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr ""
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr ""
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
 #, fuzzy
 #| msgid "Fleet Activity Tracking"
 msgid "Fleet activity tracking"
 msgstr "Seguimiento de la Actividad de Flota"
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
+msgstr ""
+
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr ""
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr ""
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
 msgstr "Creador"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:14
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+msgid "Create a FAT link using ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr ""
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
-msgstr ""
-
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
 "\n"
 "                You currently have %(open_esi_fleets)s active ESI fleets "
 "under the following characters:\n"
 "            "
 msgstr[0] ""
 msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
 "            "
 msgstr[0] ""
 msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -666,317 +716,300 @@
 "¿Quieres ayudar a traducir esta aplicación a tu idioma o mejorar la "
 "traducción existente?"
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "¡Únete a nuestro equipo de traductores!"
 
-#: afat/templates/afat/partials/form/required_field_hint.html:4
+#: afat/templates/afat/partials/form/required-field-hint.html:4
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr "Los campos marcados con un asterisco son obligatorios"
 
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr "Alternar la navegación"
-
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
 msgid "Member corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
 msgid "Corporation statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
 msgid "Corporation performance"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+#, fuzzy
+#| msgid "Ship type"
+msgid "Ship Types"
+msgstr "Tipo de Nave"
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+msgid "Average # of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
-msgid "FATs by time of day"
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
+msgid "FATs by time of day"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
 msgstr "Nombre"
 
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
-msgstr ""
-
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+msgid "Click on an alliance name to see their corporations"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+msgid "Alliance statistics for"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+msgid "Corporation statistics for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr ""
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
+#: afat/templates/afat/view/logs/logs-overview.html:6
 #, fuzzy
 #| msgid "Fleet Activity Tracking"
 msgid "Fleet activity tracking logs"
 msgstr "Seguimiento de la Actividad de Flota"
 
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
-msgstr ""
-
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
 msgstr "Usuario"
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
 msgstr "Descripción"
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, python-format
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+msgstr[1] ""
+
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
 #, fuzzy
 #| msgid "Fleet Activity Tracking"
 msgid "Fleet activity tracking statistics"
 msgstr "Seguimiento de la Actividad de Flota"
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
 #, fuzzy
 #| msgid "Fleet Activity Tracking"
 msgid "Fleet activity"
 msgstr "Seguimiento de la Actividad de Flota"
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
 msgstr "Enero"
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
 msgstr "Febrero"
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
 msgstr "Marzo"
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
 msgstr "Abril"
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
 msgstr "Mayo"
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
 msgstr "Junio"
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
 msgstr "Julio"
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
 msgstr "Agosto"
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
 msgstr "Septiembre"
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
 msgstr "Octubre"
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
 msgstr "Noviembre"
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
 msgstr "Diciembre"
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
@@ -1139,54 +1172,54 @@
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
 msgstr "Lunes"
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
 msgstr "Martes"
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
 msgstr "Miércoles"
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
 msgstr "Jueves"
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
 msgstr "Viernes"
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
 msgstr "Sábado"
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
 msgstr "Domingo"
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr ""
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/fr_FR/LC_MESSAGES/django.mo` & `allianceauth_afat-3.0.1/afat/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,87 +1,115 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: French (Alliance Auth Apps)\n"
+"Project-Id-Version: Polish (Alliance Auth Apps)\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/allianceauth-afat/fr/>\n"
-"Language: fr\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/allianceauth-afat/pl/>\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "April"
-msgstr "Avril"
+msgstr "Kwiecień"
 
 msgid "August"
-msgstr "Août"
+msgstr "Sierpień"
 
 msgid "December"
-msgstr "Décembre"
+msgstr "Grudzień"
+
+msgid "Delete"
+msgstr "Usuń"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
-"Voulez-vous aider à traduire cette application dans votre langue ou "
-"améliorer la traduction existante ?"
+"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
+"tłumaczenia?"
+
+msgid "Eve time"
+msgstr "Czas Gry"
 
 msgid "February"
-msgstr "Février"
+msgstr "Luty"
 
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "Les champs marqués d'un astérisque (*) sont obligatoires"
+msgstr "Pola z gwiazdką (*) są wymagane"
+
+msgid "Fleet Activity Tracking"
+msgstr "Śledzenie aktywności floty"
+
+msgid "Fleet type"
+msgstr "Typ floty"
+
+msgid "Fleet types"
+msgstr "Typy floty"
 
 msgid "Friday"
-msgstr "Vendredi"
+msgstr "Piątek"
+
+msgid "Is enabled"
+msgstr "Zaznaczony"
 
 msgid "January"
-msgstr "Janvier"
+msgstr "Styczeń"
 
 msgid "Join our team of translators!"
-msgstr "Rejoignez notre équipe de traducteurs !"
+msgstr "Dołącz do naszego zespołu tłumaczy!"
 
 msgid "July"
-msgstr "Juillet"
+msgstr "Lipiec"
 
 msgid "June"
-msgstr "Juin"
+msgstr "Czerwiec"
 
 msgid "March"
-msgstr "Mars"
+msgstr "Marzec"
 
 msgid "May"
-msgstr "Mai"
+msgstr "Maj"
 
 msgid "Monday"
-msgstr "Lundi"
+msgstr "Poniedziałek"
+
+msgid "Month"
+msgstr "Miesiąc"
 
 msgid "November"
-msgstr "Novembre"
+msgstr "Listopad"
 
 msgid "October"
-msgstr "Octobre"
+msgstr "Pażdziernik"
 
 msgid "Saturday"
-msgstr "Samedi"
+msgstr "Sobota"
 
 msgid "September"
-msgstr "Septembre"
+msgstr "Wrzesień"
+
+msgid "Ship type"
+msgstr "Typ statku"
 
 msgid "Sunday"
-msgstr "Dimanche"
+msgstr "Niedziela"
+
+msgid "System"
+msgstr "System Solarny"
 
 msgid "This field is mandatory"
-msgstr "Ce champ est obligatoire"
+msgstr "To pole jest wymagane"
 
 msgid "Thursday"
-msgstr "Jeudi"
+msgstr "Czwartek"
 
 msgid "Tuesday"
-msgstr "Mardi"
+msgstr "Wtorek"
 
 msgid "Wednesday"
-msgstr "Mercredi"
+msgstr "Środa"
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/fr_FR/LC_MESSAGES/django.po` & `allianceauth_afat-3.0.1/afat/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 7% similar despite different names*

```diff
@@ -1,188 +1,186 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# MxdHana <236833425@qq.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: 2024-02-06 07:10+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/allianceauth-afat/fr/>\n"
-"Language: fr_FR\n"
+"POT-Creation-Date: 2024-03-16 03:08+0100\n"
+"PO-Revision-Date: 2024-05-16 05:20+0000\n"
+"Last-Translator: MxdHana <236833425@qq.com>\n"
+"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/allianceauth-afat/zh_Hans/>\n"
+"Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 5.5.5\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
-msgstr ""
+msgstr "舰队活动历史"
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
 msgid "Fleet type"
-msgstr ""
+msgstr "舰队类型"
 
 #: afat/admin.py:169
 msgid "Is enabled"
-msgstr ""
+msgstr "已启用"
 
 #: afat/admin.py:184
 msgid "Activate selected fleet types"
-msgstr ""
+msgstr "激活选定的舰队类型"
 
 #: afat/admin.py:213
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "未成功激活 {failed} 舰队类型"
 
 #: afat/admin.py:223
 #, python-brace-format
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "激活 {notifications_count} 舰队类型"
 
 #: afat/admin.py:229
 msgid "Deactivate selected fleet types"
-msgstr ""
+msgstr "停用选定的舰队类型"
 
 #: afat/admin.py:258
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "激活 {failed} 舰队类型失败"
 
 #: afat/admin.py:268
 #, python-brace-format
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "未激活 {notifications_count} 舰队类型"
 
 #: afat/apps.py:20
 #, python-brace-format
 msgid "AFAT - Another Fleet Activity Tracker v{__version__}"
 msgstr ""
 
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
-msgstr "Ce champ est obligatoire"
+msgstr "这个字段是必填的"
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 msgid "Fleet name"
-msgstr ""
+msgstr "舰队名字"
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
-msgstr ""
+msgstr "输入舰队名称"
 
 #: afat/forms.py:49 afat/forms.py:91
 msgid "Fleet type (optional)"
-msgstr ""
+msgstr "舰队类型（可选）"
 
 #: afat/forms.py:62
 msgid "Character Name"
-msgstr ""
+msgstr "角色名称"
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
-msgstr ""
+msgstr "星系"
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
-msgstr ""
+msgstr "舰船类型"
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
-msgstr ""
+msgstr "FAT链接过期时间（分钟）"
 
 #: afat/forms.py:100
 msgid "Expiry time in minutes"
-msgstr ""
+msgstr "失效时间（分钟）"
 
 #: afat/helper/time.py:115
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
-msgstr ""
-
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+msgid "ESI"
+msgstr "ESI"
+
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
-msgstr ""
+msgstr "点击此处将停止通过ESI对该船队的自动跟踪，并关闭相关的FAT链接。"
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
+"<p>你确定要关闭{fatlink.character.character_name}关于ID{fatlink."
+"esi_fleet_id}的ESI舰队么？</p>"
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 msgid "Stop tracking"
-msgstr ""
+msgstr "停止跟踪"
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
-msgstr ""
+msgstr "删除"
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
-msgstr ""
+msgstr "<p>您确定要删除FAT链接{fatlink_fleet}吗？</p>"
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
-msgstr ""
+msgstr "<p>您确定要把{fat.character.character_name}从这个FAT链接中删除吗？</p>"
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
-msgstr ""
+msgstr "{log.fatlink_hash}（删除）"
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr ""
 
 #: afat/models.py:67
 msgid "Can manage the AFAT module"
@@ -210,19 +208,19 @@
 
 #: afat/models.py:94
 msgid "Descriptive name of the fleet type"
 msgstr ""
 
 #: afat/models.py:100
 msgid "Whether this fleet type is active or not"
-msgstr ""
+msgstr "无论这个舰队类型是否活跃"
 
 #: afat/models.py:110
 msgid "Fleet types"
-msgstr ""
+msgstr "舰队类型"
 
 #: afat/models.py:134
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
 msgstr ""
 
 #: afat/models.py:136
@@ -265,691 +263,726 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr ""
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr ""
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr ""
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr ""
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr ""
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr ""
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr ""
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr ""
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr ""
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr ""
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr ""
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr ""
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr ""
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr ""
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr ""
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr ""
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr ""
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr ""
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr ""
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr ""
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
+#, fuzzy
+#| msgid "Fleet Activity Tracking"
 msgid "Fleet activity tracking"
-msgstr ""
+msgstr "舰队活动历史"
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
+msgstr "关闭"
+
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
-msgstr ""
+msgstr "取消"
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr ""
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr ""
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
-msgstr ""
+msgstr "创建者"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
-msgstr ""
+msgstr "行动"
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:14
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
-msgstr ""
+msgstr "舰船"
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
-msgstr ""
+msgstr "创建链接"
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+msgid "Create a FAT link using ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr ""
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
-msgstr ""
+msgstr "角色"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
-msgstr ""
-
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
 "\n"
 "                You currently have %(open_esi_fleets)s active ESI fleets "
 "under the following characters:\n"
 "            "
 msgstr[0] ""
-msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
 "            "
 msgstr[0] ""
-msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr ""
-"Voulez-vous aider à traduire cette application dans votre langue ou "
-"améliorer la traduction existante ?"
+msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "Rejoignez notre équipe de traducteurs !"
+msgstr "加入我们的翻译团队吧！"
 
-#: afat/templates/afat/partials/form/required_field_hint.html:4
+#: afat/templates/afat/partials/form/required-field-hint.html:4
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "Les champs marqués d'un astérisque (*) sont obligatoires"
+msgstr "带有(*)星号符号的字段是必填的"
 
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
 msgid "Member corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
 msgid "Corporation statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
 msgid "Corporation performance"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+#, fuzzy
+#| msgid "Ship type"
+msgid "Ship Types"
+msgstr "舰船类型"
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+msgid "Average # of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
-msgid "FATs by time of day"
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
+msgid "FATs by time of day"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
-msgstr ""
-
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
-msgstr ""
+msgstr "名字"
 
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+msgid "Click on an alliance name to see their corporations"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+msgid "Alliance statistics for"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+msgid "Corporation statistics for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
-msgstr ""
+msgstr "月"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr ""
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
+#: afat/templates/afat/view/logs/logs-overview.html:6
+#, fuzzy
+#| msgid "Fleet Activity Tracking"
 msgid "Fleet activity tracking logs"
-msgstr ""
-
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
-msgstr ""
+msgstr "舰队活动历史"
 
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
-msgstr ""
+msgstr "用户"
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
 msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, python-format
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
+#, fuzzy
+#| msgid "Fleet Activity Tracking"
 msgid "Fleet activity tracking statistics"
-msgstr ""
+msgstr "舰队活动历史"
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
+#, fuzzy
+#| msgid "Fleet Activity Tracking"
 msgid "Fleet activity"
-msgstr ""
+msgstr "舰队活动历史"
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
-msgstr "Janvier"
+msgstr "一月"
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
-msgstr "Février"
+msgstr "二月"
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
-msgstr "Mars"
+msgstr "三月"
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
-msgstr "Avril"
+msgstr "四月"
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
-msgstr "Mai"
+msgstr "五月"
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
-msgstr "Juin"
+msgstr "六月"
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
-msgstr "Juillet"
+msgstr "七月"
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
-msgstr "Août"
+msgstr "八月"
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
-msgstr "Septembre"
+msgstr "九月"
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
-msgstr "Octobre"
+msgstr "十月"
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
-msgstr "Novembre"
+msgstr "十一月"
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
-msgstr "Décembre"
+msgstr "十二月"
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
 msgstr ""
 
@@ -1110,54 +1143,54 @@
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
-msgstr "Lundi"
+msgstr "周一"
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
-msgstr "Mardi"
+msgstr "周二"
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
-msgstr "Mercredi"
+msgstr "周三"
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
-msgstr "Jeudi"
+msgstr "周四"
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
-msgstr "Vendredi"
+msgstr "星期五"
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
-msgstr "Samedi"
+msgstr "周六"
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
-msgstr "Dimanche"
+msgstr "星期日"
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr ""
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/it_IT/LC_MESSAGES/django.mo` & `allianceauth_afat-3.0.1/afat/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/allianceauth-afat/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "April"
 msgstr "Aprile"
 
 msgid "August"
 msgstr "Agosto"
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/it_IT/LC_MESSAGES/django.po` & `allianceauth_afat-3.0.1/afat/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,185 +1,184 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Author50CO <tkddlschry@gmail.com>, 2023, 2024.
+# Mind of the Raven <okanieva@gmail.com>, 2024.
+# Hue Radient <seataoji@gmail.com>, 2024.
+# Rodpold Shard <rodpold@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/allianceauth-afat/it/>\n"
-"Language: it_IT\n"
+"POT-Creation-Date: 2024-03-16 03:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:14+0000\n"
+"Last-Translator: Rodpold Shard <rodpold@gmail.com>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/allianceauth-afat/ko/>\n"
+"Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
-msgstr ""
+msgstr "플릿 활동 기록"
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
 msgid "Fleet type"
-msgstr ""
+msgstr "함대 종류"
 
 #: afat/admin.py:169
 msgid "Is enabled"
-msgstr ""
+msgstr "활성화"
 
 #: afat/admin.py:184
 msgid "Activate selected fleet types"
-msgstr ""
+msgstr "선택된 플릿유형 활성화"
 
 #: afat/admin.py:213
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "{failed} 함대 종류를 활성화 할 수 없습니다"
 
 #: afat/admin.py:223
 #, python-brace-format
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "{notifications_count} 개의 함대 종류가 활성화 되었습니다"
 
 #: afat/admin.py:229
 msgid "Deactivate selected fleet types"
-msgstr ""
+msgstr "선택된 플릿을 필터에서 제외"
 
 #: afat/admin.py:258
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "{failed} 개의 함대 종류 비활성화에 실패 했습니다"
 
 #: afat/admin.py:268
 #, python-brace-format
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
-msgstr[0] ""
-msgstr[1] ""
+msgstr[0] "{notifications_count} 개의 함대 종류 비활성화됨"
 
 #: afat/apps.py:20
 #, python-brace-format
 msgid "AFAT - Another Fleet Activity Tracker v{__version__}"
 msgstr ""
 
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
-msgstr "Questo campo è obbligatorio"
+msgstr "필수 항목입니다"
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 msgid "Fleet name"
-msgstr ""
+msgstr "함대 이름"
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
-msgstr ""
+msgstr "함대 이름 입력"
 
 #: afat/forms.py:49 afat/forms.py:91
 msgid "Fleet type (optional)"
-msgstr ""
+msgstr "함대 종류 (선택)"
 
 #: afat/forms.py:62
 msgid "Character Name"
-msgstr ""
+msgstr "캐릭터 이름"
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
-msgstr ""
+msgstr "성계"
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
-msgstr ""
+msgstr "함선 종류"
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
 msgstr ""
 
 #: afat/forms.py:100
 msgid "Expiry time in minutes"
-msgstr ""
+msgstr "만료 시간"
 
 #: afat/helper/time.py:115
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+msgid "ESI"
 msgstr ""
 
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
-msgstr ""
+msgstr "이곳을 클릭하면 ESI를 통한 플릿 추적이 중단되고 FAT 링크가 만료됩니다."
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 msgid "Stop tracking"
-msgstr ""
+msgstr "함대 종료"
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
-msgstr ""
+msgstr "삭제"
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
 msgstr ""
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
 msgstr ""
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr ""
@@ -210,32 +209,32 @@
 
 #: afat/models.py:94
 msgid "Descriptive name of the fleet type"
 msgstr ""
 
 #: afat/models.py:100
 msgid "Whether this fleet type is active or not"
-msgstr ""
+msgstr "함대 종류 활성화 여부"
 
 #: afat/models.py:110
 msgid "Fleet types"
-msgstr ""
+msgstr "함대 종류"
 
 #: afat/models.py:134
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
-msgstr ""
+msgstr "함대 지휘관이 지정된 함대에 없거나 함대 참가가 더 이상 불가능합니다."
 
 #: afat/models.py:136
 msgid "Registered fleet seems to be no longer available."
-msgstr ""
+msgstr "지정된 함대가 참가가 더 이상 불가능합니다."
 
 #: afat/models.py:137
 msgid "FC is no longer the fleet boss."
-msgstr ""
+msgstr "함대 지휘관이 더 이상 함대 소유자가 아닙니다."
 
 #: afat/models.py:142
 msgid "When was this FAT link created"
 msgstr ""
 
 #: afat/models.py:149
 msgid "The FAT link fleet name"
@@ -265,689 +264,726 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr ""
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr ""
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr ""
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr ""
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr ""
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr ""
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr ""
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr ""
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr ""
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr ""
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr ""
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr ""
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr ""
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr ""
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr ""
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr ""
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr ""
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr ""
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr ""
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr ""
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
 msgid "Fleet activity tracking"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
+msgstr "닫기"
+
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
-msgstr ""
+msgstr "취소"
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr ""
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr ""
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
-msgstr ""
+msgstr "생성자"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
-msgstr ""
+msgstr "이브 표준시간"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:14
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
-msgstr ""
+msgstr "함선"
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+msgid "Create a FAT link using ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr ""
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
-msgstr ""
+msgstr "캐릭터"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
-msgstr ""
-
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
-msgstr ""
+msgstr "갯수"
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
 "\n"
 "                You currently have %(open_esi_fleets)s active ESI fleets "
 "under the following characters:\n"
 "            "
 msgstr[0] ""
-msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
 "            "
 msgstr[0] ""
-msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr ""
+msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr ""
+msgstr "번역가 팀에 참여하세요!"
 
-#: afat/templates/afat/partials/form/required_field_hint.html:4
+#: afat/templates/afat/partials/form/required-field-hint.html:4
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "I campi contrassegnati da un asterisco (*) sono obbligatori"
-
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
+msgstr "별표 (*) 표시된 항목은 필수 항목입니다"
 
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
+#, fuzzy
+#| msgid "Corporation"
 msgid "Member corporations"
-msgstr ""
+msgstr "코퍼레이션"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
-msgstr ""
+msgstr "코퍼레이션"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
+#, fuzzy
+#| msgid "Corporation"
 msgid "Corporation statistics"
-msgstr ""
+msgstr "코퍼레이션"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
+#, fuzzy
+#| msgid "Corporation"
 msgid "Corporation performance"
-msgstr ""
+msgstr "코퍼레이션"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+#, fuzzy
+#| msgid "Ship type"
+msgid "Ship Types"
+msgstr "함선 종류"
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+msgid "Average # of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
-msgid "FATs by time of day"
-msgstr ""
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
+msgstr "원본 데이터"
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
+msgid "FATs by time of day"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
-msgstr ""
-
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
-msgstr ""
+msgstr "이름"
 
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
 msgstr ""
 
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+msgid "Click on an alliance name to see their corporations"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+msgid "Alliance statistics for"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+#, fuzzy
+#| msgid "Corporation"
+msgid "Corporation statistics for"
+msgstr "코퍼레이션"
+
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
-msgstr ""
+msgstr "월"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr ""
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
+#: afat/templates/afat/view/logs/logs-overview.html:6
 msgid "Fleet activity tracking logs"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
-msgstr ""
-
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
-msgstr ""
+msgstr "사용자"
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
-msgstr ""
+msgstr "설명"
+
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, python-format
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
 msgid "Fleet activity tracking statistics"
 msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
 msgid "Fleet activity"
 msgstr ""
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
-msgstr "Gennaio"
+msgstr "1월"
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
-msgstr "Febbraio"
+msgstr "2월"
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
-msgstr "Marzo"
+msgstr "3월"
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
-msgstr "Aprile"
+msgstr "4월"
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
-msgstr "Maggio"
+msgstr "5월"
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
-msgstr "Giugno"
+msgstr "6월"
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
-msgstr "Luglio"
+msgstr "7월"
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
-msgstr "Agosto"
+msgstr "8월"
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
-msgstr "Settembre"
+msgstr "9월"
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
-msgstr "Ottobre"
+msgstr "10월"
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
-msgstr "Novembre"
+msgstr "11월"
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
-msgstr "Dicembre"
+msgstr "12월"
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
 msgstr ""
 
@@ -1108,54 +1144,54 @@
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
-msgstr "Lunedi"
+msgstr "월요일"
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
-msgstr "Martedì"
+msgstr "화요일"
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
-msgstr "Mercoledì"
+msgstr "수요일"
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
-msgstr "Giovedì"
+msgstr "목요일"
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
-msgstr "Venerdì"
+msgstr "금요일"
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
-msgstr "Sabato"
+msgstr "토요일"
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
-msgstr "Domenica"
+msgstr "일요일"
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr ""
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/ja/LC_MESSAGES/django.mo` & `allianceauth_afat-3.0.1/afat/locale/ja/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/allianceauth-afat/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "April"
 msgstr "4月"
 
 msgid "August"
 msgstr "8月"
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/ja/LC_MESSAGES/django.po` & `allianceauth_afat-3.0.1/afat/locale/django.pot`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/allianceauth-afat/ja/>\n"
-"Language: ja\n"
+"POT-Creation-Date: 2024-03-20 16:56+0100\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
 msgstr ""
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
 msgid "Fleet type"
 msgstr ""
 
 #: afat/admin.py:169
 msgid "Is enabled"
 msgstr ""
 
@@ -40,53 +39,57 @@
 msgstr ""
 
 #: afat/admin.py:213
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
 msgstr[0] ""
+msgstr[1] ""
 
 #: afat/admin.py:223
 #, python-brace-format
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
 msgstr[0] ""
+msgstr[1] ""
 
 #: afat/admin.py:229
 msgid "Deactivate selected fleet types"
 msgstr ""
 
 #: afat/admin.py:258
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
 msgstr[0] ""
+msgstr[1] ""
 
 #: afat/admin.py:268
 #, python-brace-format
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
 msgstr[0] ""
+msgstr[1] ""
 
 #: afat/apps.py:20
 #, python-brace-format
 msgid "AFAT - Another Fleet Activity Tracker v{__version__}"
 msgstr ""
 
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
 msgstr ""
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 msgid "Fleet name"
 msgstr ""
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
 msgstr ""
 
@@ -95,22 +98,22 @@
 msgstr ""
 
 #: afat/forms.py:62
 msgid "Character Name"
 msgstr ""
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
 msgstr ""
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
 msgstr ""
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
 msgstr ""
 
@@ -121,61 +124,61 @@
 #: afat/helper/time.py:115
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+msgid "ESI"
 msgstr ""
 
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr ""
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 msgid "Stop tracking"
 msgstr ""
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
 msgstr ""
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
 msgstr ""
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
 msgstr ""
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr ""
@@ -261,687 +264,719 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr ""
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr ""
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr ""
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr ""
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr ""
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr ""
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr ""
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr ""
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr ""
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr ""
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr ""
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr ""
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr ""
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr ""
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr ""
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr ""
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr ""
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr ""
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr ""
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr ""
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
 msgid "Fleet activity tracking"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
+msgstr ""
+
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr ""
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr ""
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:14
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+msgid "Create a FAT link using ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr ""
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
-msgstr ""
-
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
 "\n"
 "                You currently have %(open_esi_fleets)s active ESI fleets "
 "under the following characters:\n"
 "            "
 msgstr[0] ""
+msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
 "            "
 msgstr[0] ""
+msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: afat/templates/afat/partials/form/required_field_hint.html:4
+#: afat/templates/afat/partials/form/required-field-hint.html:4
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr ""
 
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
 msgid "Member corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
 msgid "Corporation statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
 msgid "Corporation performance"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+msgid "Ship Types"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+msgid "Average # of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
-msgid "FATs by time of day"
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
+msgid "FATs by time of day"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
-msgstr ""
-
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+msgid "Click on an alliance name to see their corporations"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+msgid "Alliance statistics for"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+msgid "Corporation statistics for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
-msgstr "月"
+msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr ""
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
+#: afat/templates/afat/view/logs/logs-overview.html:6
 msgid "Fleet activity tracking logs"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
-msgstr ""
-
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
 msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, python-format
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+msgstr[1] ""
+
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
 msgid "Fleet activity tracking statistics"
 msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
 msgid "Fleet activity"
 msgstr ""
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
-msgstr "1月"
+msgstr ""
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
-msgstr "2月"
+msgstr ""
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
-msgstr "3月"
+msgstr ""
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
-msgstr "4月"
+msgstr ""
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
-msgstr "5月"
+msgstr ""
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
-msgstr "6月"
+msgstr ""
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
-msgstr "7月"
+msgstr ""
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
-msgstr "8月"
+msgstr ""
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
-msgstr "9月"
+msgstr ""
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
-msgstr "10月"
+msgstr ""
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
-msgstr "11月"
+msgstr ""
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
-msgstr "12月"
+msgstr ""
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
 msgstr ""
 
@@ -1102,54 +1137,54 @@
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
-msgstr "月曜日"
+msgstr ""
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
-msgstr "火曜日"
+msgstr ""
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
-msgstr "水曜日"
+msgstr ""
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
-msgstr "木曜日"
+msgstr ""
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
-msgstr "金曜日"
+msgstr ""
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
-msgstr "土曜日"
+msgstr ""
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
-msgstr "日曜日"
+msgstr ""
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/ko_KR/LC_MESSAGES/django.po` & `allianceauth_afat-3.0.1/afat/locale/uk/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,121 +1,137 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
-# Author50CO <tkddlschry@gmail.com>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# "Andrii M." <elfleg0las88@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: 2024-01-07 20:04+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/allianceauth-afat/ko/>\n"
-"Language: ko_KR\n"
+"POT-Creation-Date: 2024-03-16 03:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:14+0000\n"
+"Last-Translator: \"Andrii M.\" <elfleg0las88@gmail.com>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/allianceauth-afat/uk/>\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
+"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
-msgstr "플릿 활동 기록"
+msgstr "Відстежування активності у флоті"
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
+#, fuzzy
+#| msgid "Fleet Type"
 msgid "Fleet type"
-msgstr "함대 종류"
+msgstr "Тип флоту"
 
 #: afat/admin.py:169
 msgid "Is enabled"
-msgstr "활성화"
+msgstr "Дозволено"
 
 #: afat/admin.py:184
 msgid "Activate selected fleet types"
-msgstr ""
+msgstr "Активуйте обрані типи флотів"
 
 #: afat/admin.py:213
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: afat/admin.py:223
 #, python-brace-format
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: afat/admin.py:229
 msgid "Deactivate selected fleet types"
-msgstr ""
+msgstr "Деактивувати обрані типи флотів"
 
 #: afat/admin.py:258
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: afat/admin.py:268
 #, python-brace-format
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: afat/apps.py:20
 #, python-brace-format
 msgid "AFAT - Another Fleet Activity Tracker v{__version__}"
 msgstr ""
 
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
-msgstr "필수 항목입니다"
+msgstr "Це поле обовʼязкове"
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 #, fuzzy
 #| msgid "Fleet Name"
 msgid "Fleet name"
-msgstr "함대 이름"
+msgstr "Назва флоту"
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
 msgstr ""
 
 #: afat/forms.py:49 afat/forms.py:91
+#, fuzzy
+#| msgid "Fleet Type (optional)"
 msgid "Fleet type (optional)"
-msgstr ""
+msgstr "Тип флоту (необов'язково)"
 
 #: afat/forms.py:62
 msgid "Character Name"
 msgstr ""
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
-msgstr "성계"
+msgstr "Система"
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
-msgstr "함선 종류"
+msgstr ""
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
 msgstr ""
 
 #: afat/forms.py:100
 msgid "Expiry time in minutes"
@@ -124,61 +140,61 @@
 #: afat/helper/time.py:115
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+msgid "ESI"
 msgstr ""
 
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr ""
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 msgid "Stop tracking"
 msgstr ""
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
-msgstr "삭제"
+msgstr "Видалити"
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
 msgstr ""
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
 msgstr ""
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr ""
@@ -204,37 +220,42 @@
 msgstr ""
 
 #: afat/models.py:77
 msgid "AFAT"
 msgstr ""
 
 #: afat/models.py:94
+#, fuzzy
+#| msgid "Deactivate selected fleet types"
 msgid "Descriptive name of the fleet type"
-msgstr ""
+msgstr "Деактивувати обрані типи флотів"
 
 #: afat/models.py:100
 msgid "Whether this fleet type is active or not"
 msgstr ""
 
 #: afat/models.py:110
+#, fuzzy
+#| msgid "Fleet Type"
 msgid "Fleet types"
-msgstr "함대 종류"
+msgstr "Тип флоту"
 
 #: afat/models.py:134
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
-msgstr "함대 지휘관이 지정된 함대에 없거나 함대 참가가 더 이상 불가능합니다."
+msgstr ""
+"ФлітКом не знаходиться в зареєстрованому флоті або флот вже не доступний."
 
 #: afat/models.py:136
 msgid "Registered fleet seems to be no longer available."
-msgstr "지정된 함대가 참가가 더 이상 불가능합니다."
+msgstr "Зареєстрований флот, здається, більше не доступний."
 
 #: afat/models.py:137
 msgid "FC is no longer the fleet boss."
-msgstr "함대 지휘관이 더 이상 함대 소유자가 아닙니다."
+msgstr "ФлітКом більше не бос флоту."
 
 #: afat/models.py:142
 msgid "When was this FAT link created"
 msgstr ""
 
 #: afat/models.py:149
 msgid "The FAT link fleet name"
@@ -264,693 +285,733 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr ""
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr ""
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr ""
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr ""
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr ""
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr ""
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr ""
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr ""
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr ""
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr ""
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr ""
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr ""
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr ""
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr ""
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr ""
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr ""
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr ""
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr ""
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr ""
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr ""
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
+#, fuzzy
+#| msgid "Fleet Activity Tracking"
 msgid "Fleet activity tracking"
+msgstr "Відстежування активності у флоті"
+
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr ""
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr ""
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
-msgstr "생성자"
+msgstr "Автор"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
-msgstr "이브 표준시간"
+msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:14
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+msgid "Create a FAT link using ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr ""
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
-msgstr "갯수"
-
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
 "\n"
 "                You currently have %(open_esi_fleets)s active ESI fleets "
 "under the following characters:\n"
 "            "
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
 "            "
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
+msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
-
-#: afat/templates/afat/partials/form/required_field_hint.html:4
-msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "별표 (*) 표시된 항목은 필수 항목입니다"
-
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr "토글 메뉴"
-
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
+#: afat/templates/afat/partials/form/required-field-hint.html:4
+msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
-#, fuzzy
-#| msgid "Corporation"
 msgid "Member corporations"
-msgstr "코퍼레이션"
+msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
-msgstr "코퍼레이션"
+msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
-#, fuzzy
-#| msgid "Corporation"
 msgid "Corporation statistics"
-msgstr "코퍼레이션"
+msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
-#, fuzzy
-#| msgid "Corporation"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
 msgid "Corporation performance"
-msgstr "코퍼레이션"
+msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+msgid "Ship Types"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+msgid "Average # of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
-msgid "FATs by time of day"
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
+msgid "FATs by time of day"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
-msgstr "이름"
-
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
-msgstr ""
+msgstr "Назва"
 
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+msgid "Click on an alliance name to see their corporations"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+msgid "Alliance statistics for"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+msgid "Corporation statistics for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
-msgstr "월"
+msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr ""
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
+#: afat/templates/afat/view/logs/logs-overview.html:6
+#, fuzzy
+#| msgid "Fleet Activity Tracking"
 msgid "Fleet activity tracking logs"
-msgstr ""
+msgstr "Відстежування активності у флоті"
 
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
-msgstr ""
-
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
-msgstr "사용자"
+msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
 msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, python-format
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
+
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
+#, fuzzy
+#| msgid "Fleet Activity Tracking"
 msgid "Fleet activity tracking statistics"
-msgstr ""
+msgstr "Відстежування активності у флоті"
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
+#, fuzzy
+#| msgid "Fleet Activity Tracking"
 msgid "Fleet activity"
-msgstr ""
+msgstr "Відстежування активності у флоті"
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
-msgstr "1월"
+msgstr "Січень"
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
-msgstr "2월"
+msgstr "Лютий"
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
-msgstr "3월"
+msgstr "Березень"
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
-msgstr "4월"
+msgstr "Квітень"
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
-msgstr "5월"
+msgstr "Травень"
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
-msgstr "6월"
+msgstr "Червень"
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
-msgstr "7월"
+msgstr "Липень"
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
-msgstr "8월"
+msgstr "Серпень"
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
-msgstr "9월"
+msgstr "Вересень"
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
-msgstr "10월"
+msgstr "Жовтень"
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
-msgstr "11월"
+msgstr "Листопад"
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
-msgstr "12월"
+msgstr "Грудень"
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
 msgstr ""
 
@@ -1111,54 +1172,54 @@
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
-msgstr "월요일"
+msgstr ""
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
-msgstr "화요일"
+msgstr ""
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
-msgstr "수요일"
+msgstr "Середа"
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
-msgstr "목요일"
+msgstr ""
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
-msgstr "금요일"
+msgstr "П'ятниця"
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
-msgstr "토요일"
+msgstr "Субота"
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
-msgstr "일요일"
+msgstr ""
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr ""
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/ru/LC_MESSAGES/django.mo` & `allianceauth_afat-3.0.1/afat/locale/ru/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,49 +8,15 @@
 "apps/allianceauth-afat/ru/>\n"
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
-"                    This option will automatically register and track the "
-"entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
-"this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
-"                    option.\n"
-"                "
-msgstr ""
-"\n"
-"                    Эта опция регистрирует БВ и автоматически учитывает всех "
-"пилотов флота.<br>\n"
-"<b>Используйте данную опцию только если Вы являетесь командующим флота</b>, "
-"иначе используйте опцию регистрации БВ с учетом по ссылке\n"
-"                "
-
-msgid ""
-"\n"
-"                    This will start tracking your fleet automatically and "
-"add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
-"                    (meaning you leave the fleet), or you stop the tracking "
-"here.\n"
-"                "
-msgstr ""
-"\n"
-"                    Эта опция начинает автоматическое отслеживание всех\n"
-"                    пилотов флота до закрытия флота в игре (в том числе\n"
-"                    выхода командующего из флота) или остановки отслеживания "
-"здесь.\n"
-"                "
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
@@ -100,25 +66,14 @@
 "            "
 msgstr[3] ""
 "\n"
 "                У Вас один активный ESI флот под управлением следующего "
 "пилота:\n"
 "            "
 
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
-msgstr ""
-"\n"
-"Записи журнала сохраняются в течение %(log_duration)s дней, после чего "
-"автоматически удаляются.\n"
-"        "
-
 msgid "# of FATs"
 msgstr "Количество флотов/ссылок"
 
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr "<h4>Ошибка!</h4><p>Информация о дате неполная.</p>"
 
 msgid ""
@@ -428,14 +383,17 @@
 msgstr "Пилот - участник БВ"
 
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr "Остановить ESI отслеживание флота и аннулировать ссылку РБВ."
 
+msgid "Close"
+msgstr "Закрыть"
+
 msgid "Close ESI Fleet Tracking"
 msgstr "Завершить ESI отслеживание"
 
 msgid "Close ESI fleet tracking"
 msgstr "Завершить ESI отслеживание"
 
 msgid "Confirm"
@@ -452,27 +410,17 @@
 
 msgid "Corporation statistics"
 msgstr "Статистика корпорации"
 
 msgid "Corporations"
 msgstr "Корпорации"
 
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
-msgstr ""
-"Корпорации <small>(Выберите название альянса, чтобы увидеть входящие в него "
-"корпорации)</small>"
-
 msgid "Count"
 msgstr "Количество"
 
-msgid "Create FAT link using ESI"
-msgstr "Регистрация Боевого Вылета, учет пилотов посредством ESI"
-
 msgid "Create a FAT link"
 msgstr "Создание линка"
 
 msgid "Create a clickable FAT link"
 msgstr "Регистрация Боевого Вылета, учет пилотов по ссылке"
 
 msgid "Create link"
@@ -795,17 +743,14 @@
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 "Показаны пилоты, у которых недавно были БВП. <small>(последние 10 БВП для "
 "пилота)</small>"
 
-msgid "Only months with FAT data of the selected year are shown."
-msgstr "Показаны месяцы выбранного года, в которых были БВП."
-
 msgid "Participation has been tracked via ESI"
 msgstr "Учет пилотов осуществлялся посредством ESI"
 
 msgid "Participation is being tracked via ESI"
 msgstr "Учет пилотов осуществляется посредством ESI"
 
 msgid "Previous month"
@@ -898,17 +843,14 @@
 
 msgid "Thursday"
 msgstr "Четверг"
 
 msgid "Time"
 msgstr "Время"
 
-msgid "Toggle navigation"
-msgstr "Переключить навигацию"
-
 msgid "Tuesday"
 msgstr "Вторник"
 
 msgid "User"
 msgstr "Пользователь"
 
 msgid "View log"
@@ -934,17 +876,14 @@
 
 msgid "Your monthly stats"
 msgstr "Ваша статистика за год"
 
 msgid "Your most recent FATs"
 msgstr "Ваши недавние БВП"
 
-msgid "via ESI"
-msgstr "ESI"
-
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 "{int(duration_years[0])} лет, {int(duration_days[0])} дней, "
 "{int(duration_hours[0])} часов, {int(duration_minutes[0])} минут и "
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/ru/LC_MESSAGES/django.po` & `allianceauth_afat-3.0.1/afat/locale/ru/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Nikolay <nick.postnikov@gmail.com>, 2023.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# Max <mark25@inbox.ru>, 2023.
+# Nikolay <nick.postnikov@gmail.com>, 2023, 2024.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Max <mark25@inbox.ru>, 2023, 2024.
 #
 # Translators:
 # Николай Постников, 2022
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: 2023-10-03 12:01+0000\n"
-"Last-Translator: Max <mark25@inbox.ru>\n"
+"POT-Creation-Date: 2024-03-16 03:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:14+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/allianceauth-afat/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
 msgstr "Учет Боевых Вылетов"
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
 msgid "Fleet type"
 msgstr "Тип флота"
 
 #: afat/admin.py:169
 msgid "Is enabled"
 msgstr "Разрешен"
 
@@ -94,18 +93,18 @@
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
 msgstr "Обязательное поле"
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 msgid "Fleet name"
 msgstr "Название флота"
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
 msgstr "Введите название флота"
 
@@ -114,22 +113,22 @@
 msgstr "Тип флота (не обязательно)"
 
 #: afat/forms.py:62
 msgid "Character Name"
 msgstr "Имя пилота"
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
 msgstr "Система"
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
 msgstr "Тип корабля"
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
 msgstr "Срок действия ссылки РБВ в минутах"
 
@@ -143,64 +142,66 @@
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 "{int(duration_years[0])} лет, {int(duration_days[0])} дней, "
 "{int(duration_hours[0])} часов, {int(duration_minutes[0])} минут и "
 "{int(duration_seconds[0])} секунд"
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+#, fuzzy
+#| msgid "via ESI"
+msgid "ESI"
 msgstr "ESI"
 
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr "Остановить ESI отслеживание флота и аннулировать ссылку РБВ."
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
-"<p>Действительно остановить ESI отслеживание флота с идентификатором "
-"{fatlink.esi_fleet_id} пилота {fatlink.character.character_name}?</p>"
+"<p>Действительно остановить ESI отслеживание флота с идентификатором {fatlink"
+".esi_fleet_id} пилота {fatlink.character.character_name}?</p>"
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 msgid "Stop tracking"
 msgstr "Остановить отслеживание"
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
 msgstr "Удалить"
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
 msgstr "<p>Действительно удалить ссылку РБВ {fatlink_fleet}?</p>"
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
 msgstr ""
 "<p>Действительно удалить {fat.character.character_name} из этого БВ?</p>"
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
 msgstr "{log.fatlink_hash} (Удалено)"
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr "Имеет доступ к модулю AFAT"
@@ -286,131 +287,179 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr "Флот этого БВ все еще доступен посредством ESI или нет"
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr "Ссылка РБВ была реактивирована?"
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr "Ссылка РБВ"
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr "Ссылки РБВ"
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr "Цикл жизни ссылки"
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr "Длительности БВ"
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr "Пилот - участник БВ"
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr "Использованная ссылка РБВ"
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr "Местонахождение пилота"
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr "Корабль пилота"
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr "БВП"
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr "БВП"
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr "Ссылка РБВ создана"
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr "Ссылка РБВ изменена"
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr "Ссылка РБВ удалена"
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr "Ссылка РБВ реактивирована"
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr "БВП аннулирован"
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr "Особая регистрация БВП"
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr "Журнал"
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr "Журнал"
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
 msgid "Fleet activity tracking"
 msgstr "Учет Боевых Вылетов"
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
+msgstr "Закрыть"
+
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
 msgstr "Отмена"
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr "Подтвердить"
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr "Предыдущий месяц"
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr "Следующий месяц"
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr "Текущий месяц"
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr "Статистика"
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr "Добавить ссылку"
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr "Открыть журнал"
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr "Предыдущий год"
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr "Следующий год"
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr "Текущий год"
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr "Недавние Боевые Вылеты <small>(последние 10)</small>"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
 msgstr "Создатель"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
 msgstr "Время Eve"
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
 msgstr "Действия"
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr "Ваши недавние БВП"
 
@@ -418,225 +467,250 @@
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 "Показаны пилоты, у которых недавно были БВП. <small>(последние 10 БВП для "
 "пилота)</small>"
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr "Местоположение"
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
 msgstr "Корабль"
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr "Для ваших пилотов БВП не найдены."
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr "Регистрация Боевого Вылета, учет пилотов по ссылке"
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 "Эта опция регистрирует БВ и формирует ссылку РБВ, предназначенную для учета "
 "пилотов."
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
 msgstr "Создать ссылку"
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+#, fuzzy
+#| msgid "Create FAT link using ESI"
+msgid "Create a FAT link using ESI"
 msgstr "Регистрация Боевого Вылета, учет пилотов посредством ESI"
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
+#, fuzzy
+#| msgid ""
+#| "\n"
+#| "                    This option will automatically register and track the "
+#| "entire fleet\n"
+#| "                    without fleet members having to click a link."
+#| "<br><b>Use this if you\n"
+#| "                    are Fleet Boss</b>, otherwise please use the "
+#| "clickable FAT link\n"
+#| "                    option.\n"
+#| "                "
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 "\n"
 "                    Эта опция регистрирует БВ и автоматически учитывает всех "
 "пилотов флота.<br>\n"
 "<b>Используйте данную опцию только если Вы являетесь командующим флота</b>, "
 "иначе используйте опцию регистрации БВ с учетом по ссылке\n"
 "                "
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
+#, fuzzy
+#| msgid ""
+#| "\n"
+#| "                    This will start tracking your fleet automatically and "
+#| "add pilots to\n"
+#| "                    it as they join until the fleet is either closed "
+#| "ingame\n"
+#| "                    (meaning you leave the fleet), or you stop the "
+#| "tracking here.\n"
+#| "                "
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 "\n"
 "                    Эта опция начинает автоматическое отслеживание всех\n"
 "                    пилотов флота до закрытия флота в игре (в том числе\n"
 "                    выхода командующего из флота) или остановки отслеживания "
 "здесь.\n"
 "                "
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr "Начать ESI отслеживание флота"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr "Время создания (Время EVE)"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr "Срок действия истекает (Время EVE)"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr "Срок действия истек (Время EVE)"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr "Учет пилотов осуществляется посредством ESI"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 "<p>Действительно прекратить ESI отслеживание флота с идентификатором "
 "%(esi_fleet_id)s пилота %(character_name)s</p>"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr "Учет пилотов осуществлялся посредством ESI"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 "Срок действия ссылки истек, но в течение <br>%(reopen_grace_time)s минут она "
 "может быть реактивирована."
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
-"<p>Действительно реактивировать ссылку на %(reopen_duration)s минут?"
-"<br>Ссылка может быть реактивирована только один раз!"
-"<br><em>(Предупреждение: данное действие будет занесено в журнал)</em></p>"
+"<p>Действительно реактивировать ссылку на %(reopen_duration)s "
+"минут?<br>Ссылка может быть реактивирована только один "
+"раз!<br><em>(Предупреждение: данное действие будет занесено в "
+"журнал)</em></p>"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr "Реактивировать"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr "Реактивировать ссылку РБВ"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr "Боевой Вылет"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr "Скопируй меня!"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr "Завершить ESI отслеживание"
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr "Задать имя"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr "Особая регистрация БВ"
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
 msgstr "частота проверки флота <small>(обновляется каждые 15 секунд)</small>"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr "частота проверки флота"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
 msgstr "Пилот"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr "Обзор типов кораблей"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
 msgstr "Количество"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
-msgstr "Особая регистрация БВ"
-
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr "Пилот отсутствует в списке? Используйте форму, чтобы добавить его."
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr "Примечание"
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr "Действие будет занесено в журнал!"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr "Имя пилота"
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr "Создать ссылку вручную"
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr "Условные обозначения"
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr "Флот активен и пилоты автоматически отслеживаются посредством ESI"
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr "Пилоты автоматически отслеживались посредством ESI"
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
@@ -661,19 +735,19 @@
 "            "
 msgstr[3] ""
 "\n"
 "                У Вас один активный ESI флот под управлением следующего "
 "пилота:\n"
 "            "
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr "ESI ID флота"
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
@@ -691,31 +765,31 @@
 "                Эти флоты отслеживаются автоматически.\n"
 "            "
 msgstr[3] ""
 "\n"
 "                Этот флот отслеживается автоматически.\n"
 "            "
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 "При необходимости, Вы можете создать новые флоты под командованием других "
 "пилотов."
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 "Примечание: информация о Ваших зарегистрированных флотах может задерживаться "
 "до 5 минут."
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr "Завершить ESI отслеживание"
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -723,317 +797,331 @@
 "Вы хотите помочь перевести это приложение на ваш язык или улучшить текущий "
 "перевод?"
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Присоединяйтесь к нашей команде переводчиков!"
 
-#: afat/templates/afat/partials/form/required_field_hint.html:4
+#: afat/templates/afat/partials/form/required-field-hint.html:4
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr "Поля, отмеченные (*) обязательны"
 
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr "Переключить навигацию"
-
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
-msgstr "Статистика"
-
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr "Добавить ссылку"
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr "Открыть журнал"
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
-msgstr "Предыдущий месяц"
-
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
-msgstr "Следующий месяц"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
+msgstr "Графики"
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
-msgstr "Текущий месяц"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
+msgstr "Корпорации"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
 msgid "Member corporations"
 msgstr "Корпорации-участницы"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
 msgstr "Корпорация"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr "Количество флотов/линков (в среднем)"
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
 msgid "Corporation statistics"
 msgstr "Статистика корпорации"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr "Ссылки флотов по типам кораблей"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
 msgid "Corporation performance"
 msgstr "Показатели корпорации"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr "по продолжительности"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr "Количество флотов/линков по дням недели"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+#, fuzzy
+#| msgid "Ship type"
+msgid "Ship Types"
+msgstr "Тип корабля"
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr "Среднее кол-во линков по корпорациям"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
-msgstr "Графики"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+#, fuzzy
+#| msgid "# of FATs"
+msgid "Average # of FATs"
+msgstr "Количество флотов/ссылок"
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
-msgstr "Корпорации"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
+msgstr "Количество флотов/ссылок"
+
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
+msgstr "Исходные данные"
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
 msgid "FATs by time of day"
 msgstr "Количество флотов/ссылок по времени суток"
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
-msgstr "Количество флотов/ссылок"
-
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr "Количество флотов/ссылок для"
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
 msgstr "Название"
 
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
-msgstr "Исходные данные"
-
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr "Участники"
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr "Статистика пилота"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
+msgstr "Мои показатели"
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+#, fuzzy
+#| msgid ""
+#| "Corporations <small>(Click on an alliance name to see their "
+#| "corporations)</small>"
+msgid "Click on an alliance name to see their corporations"
 msgstr ""
 "Корпорации <small>(Выберите название альянса, чтобы увидеть входящие в него "
 "корпорации)</small>"
 
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+#, fuzzy
+#| msgid "Character statistics"
+msgid "Alliance statistics for"
+msgstr "Статистика пилота"
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+#, fuzzy
+#| msgid "Corporation statistics"
+msgid "Corporation statistics for"
+msgstr "Статистика корпорации"
+
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr "Ваша статистика за год"
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+#, fuzzy
+#| msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr "Показаны месяцы выбранного года, в которых были БВП."
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr "Показаны пилоты, у которых были БВП в выбранном году."
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
 msgstr "Месяц"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr "кол-во ссылок"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr "Нет БВП для"
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr "Нет БВП за этот год"
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr "Мои показатели"
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr "Предыдущий год"
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr "Следующий год"
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr "Текущий год"
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr "Недавняя активность"
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr "Удаление линка"
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr "Отсутствуют недавние БВП для"
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr "Отсутствуют недавние БВП"
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr "Создание линка"
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr "Подробности линка"
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr "Завершение Боевого Вылета"
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr "Все линки"
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
+#: afat/templates/afat/view/logs/logs-overview.html:6
 msgid "Fleet activity tracking logs"
 msgstr "Журнал системы учёта активности во флотах"
 
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
-msgstr ""
-"\n"
-"Записи журнала сохраняются в течение %(log_duration)s дней, после чего "
-"автоматически удаляются.\n"
-"        "
-
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr "Время"
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr "Событие"
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
 msgstr "Пользователь"
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
 msgstr "Описание"
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, fuzzy, python-format
+#| msgid ""
+#| "\n"
+#| "            Logs are only kept for %(log_duration)s days. Logs older than "
+#| "that are removed automatically.\n"
+#| "        "
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+"\n"
+"Записи журнала сохраняются в течение %(log_duration)s дней, после чего "
+"автоматически удаляются.\n"
+"        "
+msgstr[1] ""
+"\n"
+"Записи журнала сохраняются в течение %(log_duration)s дней, после чего "
+"автоматически удаляются.\n"
+"        "
+msgstr[2] ""
+"\n"
+"Записи журнала сохраняются в течение %(log_duration)s дней, после чего "
+"автоматически удаляются.\n"
+"        "
+msgstr[3] ""
+"\n"
+"Записи журнала сохраняются в течение %(log_duration)s дней, после чего "
+"автоматически удаляются.\n"
+"        "
+
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
 msgid "Fleet activity tracking statistics"
 msgstr "Журнал Системы УБВ"
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
 msgid "Fleet activity"
 msgstr "Активность во флотах"
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
 msgstr "Январь"
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
 msgstr "Февраль"
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
 msgstr "Март"
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
 msgstr "Апрель"
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
 msgstr "Май"
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
 msgstr "Июнь"
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
 msgstr "Июль"
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
 msgstr "Август"
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
 msgstr "Сентябрь"
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
 msgstr "Октябрь"
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
 msgstr "Ноябрь"
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
 msgstr "Декабрь"
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
@@ -1177,16 +1265,16 @@
 "{character_name}<br>Система: {system}<br>Корабль: {shiptype}</p>"
 
 #: afat/views/fatlinks.py:817
 msgid ""
 "<h4>Oh No!</h4><p>Manual FAT processing failed! The character name you "
 "entered was not found.</p>"
 msgstr ""
-"<h4>Упс!</h4><p>Ошибка редактирования БВ! Пилот с введенным именем не найден."
-"</p>"
+"<h4>Упс!</h4><p>Ошибка редактирования БВ! Пилот с введенным именем не "
+"найден.</p>"
 
 #: afat/views/fatlinks.py:826
 msgid "<h4>Oh No!</h4><p>Something went wrong!</p>"
 msgstr "<h4>Упс!</h4><p>Что-то пошло не так!</p>"
 
 #: afat/views/fatlinks.py:949
 msgid ""
@@ -1226,73 +1314,73 @@
 "<h4>Успех!</h4><p>Регистрация БВП для {character_name} удалена из БВ флота "
 "«{fatlink_hash}».</p>"
 
 #: afat/views/fatlinks.py:1128
 msgid ""
 "<h4>Error!</h4><p>The hash you provided does not match with any FAT link.</p>"
 msgstr ""
-"<h4>Ошибка!</h4><p>Предоставленный hash не соответствует никакому БВ флота.</"
-"p>"
+"<h4>Ошибка!</h4><p>Предоставленный hash не соответствует никакому БВ "
+"флота.</p>"
 
 #: afat/views/fatlinks.py:1174
 msgid "<h4>Success!</h4><p>The FAT link has been successfully re-opened.</p>"
 msgstr "<h4>Успех!</h4><p>Ссылка РБВ успешно реактивирована.</p>"
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 "<h4>Внимание!</h4><p>Данная ссылка РБВ уже была реактивирована ранее. "
 "Возможна только одна реактивация ссылки РБВ!</p>"
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
-"<h4>Внимание!</h4><p>У Вас нет прав для просмотра статистики этого пилота.</"
-"p>"
+"<h4>Внимание!</h4><p>У Вас нет прав для просмотра статистики этого "
+"пилота.</p>"
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr "<h4>Внимание!</h4><p>Информация о дате неполная!</p>"
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
-"<h4>Внимание!</h4><p>У Вас нет прав для просмотра статистики этой корпорации."
-"</p>"
+"<h4>Внимание!</h4><p>У Вас нет прав для просмотра статистики этой "
+"корпорации.</p>"
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
 msgstr "Понедельник"
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
 msgstr "Вторник"
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
 msgstr "Среда"
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
 msgstr "Четверг"
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
 msgstr "Пятница"
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
 msgstr "Суббота"
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
 msgstr "Воскресенье"
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr "<h4>Ошибка!</h4><p>Информация о дате неполная.</p>"
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/uk/LC_MESSAGES/django.mo` & `allianceauth_afat-3.0.1/afat/locale/uk/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/allianceauth-afat/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Activate selected fleet types"
 msgstr "Активуйте обрані типи флотів"
 
 msgid "April"
 msgstr "Квітень"
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/uk/LC_MESSAGES/django.po` & `allianceauth_afat-3.0.1/afat/locale/sk/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# "Andrii M." <elfleg0las88@gmail.com>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
-"Last-Translator: \"Andrii M.\" <elfleg0las88@gmail.com>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/allianceauth-afat/uk/>\n"
-"Language: uk\n"
+"POT-Creation-Date: 2024-03-20 16:54+0100\n"
+"PO-Revision-Date: 2024-05-10 14:14+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/allianceauth-afat/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
-"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
-msgstr "Відстежування активності у флоті"
+msgstr ""
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
-#, fuzzy
-#| msgid "Fleet Type"
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
 msgid "Fleet type"
-msgstr "Тип флоту"
+msgstr ""
 
 #: afat/admin.py:169
 msgid "Is enabled"
-msgstr "Дозволено"
+msgstr ""
 
 #: afat/admin.py:184
 msgid "Activate selected fleet types"
-msgstr "Активуйте обрані типи флотів"
+msgstr ""
 
 #: afat/admin.py:213
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
@@ -59,15 +56,15 @@
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
 #: afat/admin.py:229
 msgid "Deactivate selected fleet types"
-msgstr "Деактивувати обрані типи флотів"
+msgstr ""
 
 #: afat/admin.py:258
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
@@ -87,50 +84,46 @@
 #, python-brace-format
 msgid "AFAT - Another Fleet Activity Tracker v{__version__}"
 msgstr ""
 
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
-msgstr "Це поле обовʼязкове"
+msgstr ""
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
-#, fuzzy
-#| msgid "Fleet Name"
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 msgid "Fleet name"
-msgstr "Назва флоту"
+msgstr ""
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
 msgstr ""
 
 #: afat/forms.py:49 afat/forms.py:91
-#, fuzzy
-#| msgid "Fleet Type (optional)"
 msgid "Fleet type (optional)"
-msgstr "Тип флоту (необов'язково)"
+msgstr ""
 
 #: afat/forms.py:62
 msgid "Character Name"
 msgstr ""
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
-msgstr "Система"
+msgstr ""
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
 msgstr ""
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
 msgstr ""
 
@@ -141,61 +134,61 @@
 #: afat/helper/time.py:115
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+msgid "ESI"
 msgstr ""
 
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr ""
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 msgid "Stop tracking"
 msgstr ""
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
-msgstr "Видалити"
+msgstr ""
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
 msgstr ""
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
 msgstr ""
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr ""
@@ -221,42 +214,37 @@
 msgstr ""
 
 #: afat/models.py:77
 msgid "AFAT"
 msgstr ""
 
 #: afat/models.py:94
-#, fuzzy
-#| msgid "Deactivate selected fleet types"
 msgid "Descriptive name of the fleet type"
-msgstr "Деактивувати обрані типи флотів"
+msgstr ""
 
 #: afat/models.py:100
 msgid "Whether this fleet type is active or not"
 msgstr ""
 
 #: afat/models.py:110
-#, fuzzy
-#| msgid "Fleet Type"
 msgid "Fleet types"
-msgstr "Тип флоту"
+msgstr ""
 
 #: afat/models.py:134
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
 msgstr ""
-"ФлітКом не знаходиться в зареєстрованому флоті або флот вже не доступний."
 
 #: afat/models.py:136
 msgid "Registered fleet seems to be no longer available."
-msgstr "Зареєстрований флот, здається, більше не доступний."
+msgstr ""
 
 #: afat/models.py:137
 msgid "FC is no longer the fleet boss."
-msgstr "ФлітКом більше не бос флоту."
+msgstr ""
 
 #: afat/models.py:142
 msgid "When was this FAT link created"
 msgstr ""
 
 #: afat/models.py:149
 msgid "The FAT link fleet name"
@@ -286,336 +274,383 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr ""
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr ""
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr ""
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr ""
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr ""
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr ""
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr ""
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr ""
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr ""
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr ""
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr ""
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr ""
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr ""
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr ""
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr ""
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr ""
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr ""
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr ""
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr ""
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr ""
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
-#, fuzzy
-#| msgid "Fleet Activity Tracking"
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
 msgid "Fleet activity tracking"
-msgstr "Відстежування активності у флоті"
+msgstr ""
+
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
+msgstr ""
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr ""
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr ""
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
-msgstr "Автор"
+msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:14
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+msgid "Create a FAT link using ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr ""
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
-msgstr ""
-
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
@@ -624,363 +659,340 @@
 "under the following characters:\n"
 "            "
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
 "            "
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: afat/templates/afat/partials/form/required_field_hint.html:4
+#: afat/templates/afat/partials/form/required-field-hint.html:4
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr ""
 
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
 msgid "Member corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
 msgid "Corporation statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
 msgid "Corporation performance"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+msgid "Ship Types"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+msgid "Average # of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
-msgid "FATs by time of day"
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
+msgid "FATs by time of day"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
-msgstr "Назва"
-
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
 msgstr ""
 
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+msgid "Click on an alliance name to see their corporations"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+msgid "Alliance statistics for"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+msgid "Corporation statistics for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr ""
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
-#, fuzzy
-#| msgid "Fleet Activity Tracking"
+#: afat/templates/afat/view/logs/logs-overview.html:6
 msgid "Fleet activity tracking logs"
-msgstr "Відстежування активності у флоті"
-
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
 msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
-#, fuzzy
-#| msgid "Fleet Activity Tracking"
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, python-format
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
+
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
 msgid "Fleet activity tracking statistics"
-msgstr "Відстежування активності у флоті"
+msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
-#, fuzzy
-#| msgid "Fleet Activity Tracking"
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
 msgid "Fleet activity"
-msgstr "Відстежування активності у флоті"
+msgstr ""
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
-msgstr "Січень"
+msgstr ""
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
-msgstr "Лютий"
+msgstr ""
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
-msgstr "Березень"
+msgstr ""
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
-msgstr "Квітень"
+msgstr ""
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
-msgstr "Травень"
+msgstr ""
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
-msgstr "Червень"
+msgstr ""
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
-msgstr "Липень"
+msgstr ""
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
-msgstr "Серпень"
+msgstr ""
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
-msgstr "Вересень"
+msgstr ""
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
-msgstr "Жовтень"
+msgstr ""
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
-msgstr "Листопад"
+msgstr ""
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
-msgstr "Грудень"
+msgstr ""
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
 msgstr ""
 
@@ -1141,54 +1153,54 @@
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
 msgstr ""
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
 msgstr ""
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
-msgstr "Середа"
+msgstr ""
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
 msgstr ""
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
-msgstr "П'ятниця"
+msgstr ""
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
-msgstr "Субота"
+msgstr ""
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
 msgstr ""
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `allianceauth_afat-3.0.0b3/afat/locale/zh_Hans/LC_MESSAGES/django.po` & `allianceauth_afat-3.0.1/afat/locale/nl/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,118 +1,122 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 15:53+0200\n"
-"PO-Revision-Date: 2024-02-06 07:10+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/allianceauth-afat/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"POT-Creation-Date: 2024-03-20 16:56+0100\n"
+"PO-Revision-Date: 2024-05-10 14:14+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/allianceauth-afat/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: afat/__init__.py:15 afat/app_settings.py:36
-#: afat/templates/afat/partials/menu.html:14
+#: afat/__init__.py:9 afat/app_settings.py:36
 msgid "Fleet Activity Tracking"
-msgstr "舰队活动历史"
+msgstr ""
 
 #: afat/admin.py:156 afat/models.py:109
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:13
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:43
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:38
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:11
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:33
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:28
 msgid "Fleet type"
-msgstr "舰队类型"
+msgstr ""
 
 #: afat/admin.py:169
 msgid "Is enabled"
-msgstr "已启用"
+msgstr ""
 
 #: afat/admin.py:184
 msgid "Activate selected fleet types"
-msgstr "激活选定的舰队类型"
+msgstr ""
 
 #: afat/admin.py:213
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
-msgstr[0] "未成功激活 {failed} 舰队类型"
+msgstr[0] ""
+msgstr[1] ""
 
 #: afat/admin.py:223
 #, python-brace-format
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
-msgstr[0] "激活 {notifications_count} 舰队类型"
+msgstr[0] ""
+msgstr[1] ""
 
 #: afat/admin.py:229
 msgid "Deactivate selected fleet types"
-msgstr "停用选定的舰队类型"
+msgstr ""
 
 #: afat/admin.py:258
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
-msgstr[0] "激活 {failed} 舰队类型失败"
+msgstr[0] ""
+msgstr[1] ""
 
 #: afat/admin.py:268
 #, python-brace-format
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
-msgstr[0] "未激活 {notifications_count} 舰队类型"
+msgstr[0] ""
+msgstr[1] ""
 
 #: afat/apps.py:20
 #, python-brace-format
 msgid "AFAT - Another Fleet Activity Tracker v{__version__}"
 msgstr ""
 
 #: afat/forms.py:25
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:4
 msgid "This field is mandatory"
-msgstr "这个字段是必填的"
+msgstr ""
 
 #: afat/forms.py:43 afat/forms.py:85 afat/forms.py:112
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:12
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:42
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:10
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:32
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:11
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:27
 msgid "Fleet name"
-msgstr "舰队名字"
+msgstr ""
 
 #: afat/forms.py:45 afat/forms.py:87
 msgid "Enter fleet name"
 msgstr ""
 
 #: afat/forms.py:49 afat/forms.py:91
 msgid "Fleet type (optional)"
-msgstr "舰队类型（可选）"
+msgstr ""
 
 #: afat/forms.py:62
 msgid "Character Name"
 msgstr ""
 
 #: afat/forms.py:67
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:41
 msgid "System"
 msgstr ""
 
 #: afat/forms.py:72
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:37
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:51
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:38
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:56
 msgid "Ship type"
-msgstr "舰船类型"
+msgstr ""
 
 #: afat/forms.py:97
 msgid "FAT link expiry time in minutes"
 msgstr ""
 
 #: afat/forms.py:100
 msgid "Expiry time in minutes"
@@ -121,61 +125,61 @@
 #: afat/helper/time.py:115
 msgid ""
 "{int(duration_years[0])} years, {int(duration_days[0])} days, "
 "{int(duration_hours[0])} hours, {int(duration_minutes[0])} minutes and "
 "{int(duration_seconds[0])} seconds"
 msgstr ""
 
-#: afat/helper/views.py:57 afat/helper/views.py:177
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:83
-msgid "via ESI"
+#: afat/helper/views.py:59 afat/helper/views.py:178
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:78
+msgid "ESI"
 msgstr ""
 
-#: afat/helper/views.py:88
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:34
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:33
+#: afat/helper/views.py:90
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:33
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:32
 msgid ""
 "Clicking here will stop the automatic tracking through ESI for this fleet "
 "and close the associated FAT link."
 msgstr ""
 
-#: afat/helper/views.py:91
+#: afat/helper/views.py:93
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID {fatlink.esi_fleet_id} "
 "from {fatlink.character.character_name}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:93
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:39
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:42
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:41
+#: afat/helper/views.py:95
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:38
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:41
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:40
 msgid "Stop tracking"
 msgstr ""
 
-#: afat/helper/views.py:121 afat/helper/views.py:188
+#: afat/helper/views.py:123 afat/helper/views.py:189
 msgid "Delete"
-msgstr "删除"
+msgstr ""
 
-#: afat/helper/views.py:123
+#: afat/helper/views.py:125
 #, python-brace-format
 msgid "<p>Are you sure you want to delete FAT link {fatlink_fleet}?</p>"
 msgstr ""
 
-#: afat/helper/views.py:190
+#: afat/helper/views.py:191
 #, python-brace-format
 msgid ""
 "<p>Are you sure you want to remove {fat.character.character_name} from this "
 "FAT link?</p>"
 msgstr ""
 
-#: afat/helper/views.py:242
+#: afat/helper/views.py:243
 #, python-brace-format
 msgid "{log.fatlink_hash} (Deleted)"
 msgstr ""
 
 #: afat/models.py:59
 msgid "Can access the AFAT module"
 msgstr ""
@@ -206,19 +210,19 @@
 
 #: afat/models.py:94
 msgid "Descriptive name of the fleet type"
 msgstr ""
 
 #: afat/models.py:100
 msgid "Whether this fleet type is active or not"
-msgstr "无论这个舰队类型是否活跃"
+msgstr ""
 
 #: afat/models.py:110
 msgid "Fleet types"
-msgstr "舰队类型"
+msgstr ""
 
 #: afat/models.py:134
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
 msgstr ""
 
 #: afat/models.py:136
@@ -261,695 +265,719 @@
 msgid "Whether the fleet to this FAT link is available in ESI or not"
 msgstr ""
 
 #: afat/models.py:192
 msgid "Has this FAT link being re-opened?"
 msgstr ""
 
-#: afat/models.py:212 afat/templates/afat/view/logs/logs_overview.html:32
+#: afat/models.py:212 afat/templates/afat/view/logs/logs-overview.html:24
 msgid "FAT link"
 msgstr ""
 
 #: afat/models.py:213
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:7
-#: afat/templates/afat/partials/menu.html:25
+#: afat/templates/afat/partials/common/navigation/top-menu.html:27
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:28
 msgid "FAT links"
 msgstr ""
 
-#: afat/models.py:271
+#: afat/models.py:270
 msgid "FAT link duration"
 msgstr ""
 
-#: afat/models.py:272
+#: afat/models.py:271
 msgid "FAT link durations"
 msgstr ""
 
-#: afat/models.py:285
+#: afat/models.py:284
 msgid "Character who registered this FAT"
 msgstr ""
 
-#: afat/models.py:292
+#: afat/models.py:291
 msgid "The FAT link the character registered at"
 msgstr ""
 
-#: afat/models.py:296
+#: afat/models.py:295
 msgid "The system the character is in"
 msgstr ""
 
-#: afat/models.py:303
+#: afat/models.py:302
 msgid "The ship the character was flying"
 msgstr ""
 
-#: afat/models.py:315
+#: afat/models.py:314
 msgid "FAT"
 msgstr ""
 
-#: afat/models.py:316
-#: afat/templates/afat/partials/dashboard/tabs_navigation.html:4
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:6
+#: afat/models.py:315
+#: afat/templates/afat/partials/dashboard/tabs-navigation.html:14
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:16
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:14
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:11
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:34
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:33
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:29
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:29
 msgid "FATs"
 msgstr ""
 
-#: afat/models.py:340
+#: afat/models.py:339
 msgid "FAT link created"
 msgstr ""
 
-#: afat/models.py:341
+#: afat/models.py:340
 msgid "FAT link changed"
 msgstr ""
 
-#: afat/models.py:342
+#: afat/models.py:341
 msgid "FAT link removed"
 msgstr ""
 
-#: afat/models.py:343
+#: afat/models.py:342
 msgid "FAT link re-opened"
 msgstr ""
 
-#: afat/models.py:345
+#: afat/models.py:344
 msgid "FAT removed"
 msgstr ""
 
-#: afat/models.py:346
+#: afat/models.py:345
 msgid "Manual FAT added"
 msgstr ""
 
-#: afat/models.py:372
+#: afat/models.py:371
 msgid "Log"
 msgstr ""
 
-#: afat/models.py:373 afat/templates/afat/view/logs/logs_overview.html:14
+#: afat/models.py:372 afat/templates/afat/view/logs/logs-overview.html:11
 msgid "Logs"
 msgstr ""
 
-#: afat/templates/afat/base.html:6
+#: afat/templates/afat/base.html:6 afat/templates/afat/base.html:11
 #: afat/templates/afat/view/dashboard/dashboard.html:7
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:6
-#: afat/templates/afat/view/statistics/statistics_overview.html:8
-#, fuzzy
-#| msgid "Fleet Activity Tracking"
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:6
+#: afat/templates/afat/view/statistics/statistics-overview.html:8
 msgid "Fleet activity tracking"
-msgstr "舰队活动历史"
+msgstr ""
+
+#: afat/templates/afat/modals/general.html:12
+msgid "Close"
+msgstr ""
 
-#: afat/templates/afat/modals/general.html:27
+#: afat/templates/afat/modals/general.html:25
 msgid "Cancel"
 msgstr ""
 
-#: afat/templates/afat/modals/general.html:28
+#: afat/templates/afat/modals/general.html:26
 msgid "Confirm"
 msgstr ""
 
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:5
+msgid "Previous month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:10
+msgid "Next month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/month-navigation.html:11
+msgid "Current month"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:9
+msgid "Dashboard"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:18
+#: afat/templates/afat/view/statistics/statistics-alliance.html:12
+#: afat/templates/afat/view/statistics/statistics-character.html:11
+#: afat/templates/afat/view/statistics/statistics-corporation.html:11
+#: afat/templates/afat/view/statistics/statistics-overview.html:13
+msgid "Statistics"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:37
+msgid "Add FAT link"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/top-menu.html:48
+msgid "View log"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:4
+msgid "Previous year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:9
+msgid "Next year"
+msgstr ""
+
+#: afat/templates/afat/partials/common/navigation/year-navigation.html:10
+msgid "Current year"
+msgstr ""
+
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:6
 msgid "Most recent FAT links <small>(latest 10)</small>"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:14
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:6
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:34
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:6
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:29
 msgid "Creator"
-msgstr "创建者"
+msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:15
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:46
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:41
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:14
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:35
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:30
 msgid "Eve time"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fatlinks.html:16
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:20
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:37
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:21
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:32
 msgid "Actions"
-msgstr "行动"
+msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:11
 msgid "Your most recent FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/dashboard/tabs/fats.html:14
 msgid ""
 "Only characters that have recent FATs are shown. <small>(latest 10 FATs per "
 "character)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:44
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:19
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:12
 msgid "Location"
 msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:45
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:40
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:13
 msgid "Ship"
-msgstr "舰船"
+msgstr ""
 
-#: afat/templates/afat/partials/dashboard/tabs/fats.html:67
+#: afat/templates/afat/partials/dashboard/tabs/fats.html:62
 msgid "No recent FAT activity registered for any of your characters."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:8
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:8
 msgid "Create a clickable FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:14
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:14
 msgid ""
 "This option will create a clickable link to share with your fleet members."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/clickable_link.html:35
+#: afat/templates/afat/partials/fatlinks/add/clickable-link.html:35
 msgid "Create link"
-msgstr "创建链接"
+msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:9
-msgid "Create FAT link using ESI"
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:9
+msgid "Create a FAT link using ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:15
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:15
 msgid ""
 "\n"
 "                    This option will automatically register and track the "
 "entire fleet\n"
-"                    without fleet members having to click a link.<br><b>Use "
+"                    without fleet members having to click a link. <b>Use "
 "this if you\n"
-"                    are Fleet Boss</b>, otherwise please use the clickable "
-"FAT link\n"
+"                    are the Fleet Boss</b>, otherwise please use the "
+"clickable FAT link\n"
 "                    option.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:24
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:24
 msgid ""
 "\n"
 "                    This will start tracking your fleet automatically and "
 "add pilots to\n"
-"                    it as they join until the fleet is either closed ingame\n"
+"                    it as they join until the fleet is either closed in-"
+"game\n"
 "                    (meaning you leave the fleet), or you stop the tracking "
 "here.\n"
 "                "
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/add/esi_link.html:48
+#: afat/templates/afat/partials/fatlinks/add/esi-link.html:48
 msgid "Add ESI link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:11
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:11
 msgid "Link created (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:17
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:17
 msgid "Link expires (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:19
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:19
 msgid "Link expired (Eve Time)"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:29
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:29
 msgid "Participation is being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:38
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:37
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:37
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:36
 #, python-format
 msgid ""
 "<p>Are you sure you want to close ESI fleet with ID %(esi_fleet_id)s from "
 "%(character_name)s</p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:46
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:45
 msgid "Participation has been tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:53
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:52
 #, python-format
 msgid ""
 "This link has already expired but is within the grace<br>time of "
 "%(reopen_grace_time)s minutes where it can be re-opened."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:61
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:60
 #, python-format
 msgid ""
 "<p>Are you sure you want to re-open this FAT link for another "
 "%(reopen_duration)s minutes?<br>FAT links can be re-opened only once!"
 "<br><em>(Be aware, this action will be logged)</em></p>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:62
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:61
 msgid "Re-Open"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:64
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:97
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:63
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:95
 msgid "Re-open FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:72
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:71
 msgid "FAT Link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:84
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:82
 msgid "Copy me!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_info.html:92
-#: afat/templates/afat/view/dashboard/dashboard.html:32
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:57
+#: afat/templates/afat/partials/fatlinks/details/fatlink-info.html:90
+#: afat/templates/afat/view/dashboard/dashboard.html:27
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:52
 msgid "Close ESI fleet tracking"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/fatlink_name_form.html:14
+#: afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html:14
 msgid "Set name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:7
+#: afat/templates/afat/partials/fatlinks/details/tabs-navigation.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
+msgid "Manual FAT"
+msgstr ""
+
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:8
 msgid "FATs for this FAT link <small>(updated every 15 seconds)</small>"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:9
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:10
 msgid "FATs for this FAT link"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:17
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:18
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:10
 msgid "Character"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:30
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:31
 msgid "Ship type overview"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:39
+#: afat/templates/afat/partials/fatlinks/details/tabs/fats.html:40
 msgid "Count"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:8
-#: afat/templates/afat/partials/fatlinks/details/tabs_navigation.html:7
-msgid "Manual FAT"
-msgstr ""
-
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:11
 msgid "Is someone missing from the list of FATs? Use this form to add them."
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "Note"
 msgstr ""
 
 #: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:13
 msgid "This action is logged!"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:21
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:22
 msgid "Character name"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:67
+#: afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html:73
 msgid "Add manual FAT"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:4
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:4
 msgid "Legend"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:5
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:5
 msgid ""
 "Fleet is currently active and FATs are automatically being tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/fatlink_list_legend.html:6
+#: afat/templates/afat/partials/fatlinks/fatlink-list-legend.html:6
 msgid "FATs have been automatically tracked via ESI"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:7
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:7
 #, python-format
 msgid ""
 "\n"
 "                You currently have an active ESI fleet under the following "
 "character:\n"
 "            "
 msgid_plural ""
 "\n"
 "                You currently have %(open_esi_fleets)s active ESI fleets "
 "under the following characters:\n"
 "            "
 msgstr[0] ""
+msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:25
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:25
 msgid "ESI fleet ID"
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:49
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:48
 msgid ""
 "\n"
 "                This fleet is already automatically tracked.\n"
 "            "
 msgid_plural ""
 "\n"
 "                These fleets are already automatically tracked.\n"
 "            "
 msgstr[0] ""
+msgstr[1] ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:55
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:54
 msgid ""
 "However, you can still open more fleets with other alts, if that&apos;s what "
 "you like to do."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:59
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:58
 msgid ""
 "Note: Information about your registered fleets might be delayed by up to 5 "
 "minutes."
 msgstr ""
 
-#: afat/templates/afat/partials/fatlinks/open_esi_fleets.html:63
+#: afat/templates/afat/partials/fatlinks/open-esi-fleets.html:62
 msgid "Close ESI Fleet Tracking"
 msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
+msgstr ""
 
 #: afat/templates/afat/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "加入我们的翻译团队吧！"
-
-#: afat/templates/afat/partials/form/required_field_hint.html:4
-msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "带有(*)星号符号的字段是必填的"
-
-#: afat/templates/afat/partials/menu.html:8
-msgid "Toggle navigation"
 msgstr ""
 
-#: afat/templates/afat/partials/menu.html:20
-#: afat/templates/afat/view/statistics/statistics_alliance.html:15
-#: afat/templates/afat/view/statistics/statistics_character.html:14
-#: afat/templates/afat/view/statistics/statistics_corporation.html:14
-#: afat/templates/afat/view/statistics/statistics_overview.html:16
-msgid "Statistics"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:31
-msgid "Add FAT link"
-msgstr ""
-
-#: afat/templates/afat/partials/menu.html:37
-msgid "View log"
-msgstr ""
-
-#: afat/templates/afat/partials/month_navigation.html:5
-msgid "Previous month"
+#: afat/templates/afat/partials/form/required-field-hint.html:4
+msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:10
-msgid "Next month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:4
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:4
+msgid "Graphs"
 msgstr ""
 
-#: afat/templates/afat/partials/month_navigation.html:11
-msgid "Current month"
+#: afat/templates/afat/partials/statistics/alliance/tabs-navigation.html:7
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:8
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:9
+msgid "Corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:7
 msgid "Member corporations"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:13
 msgid "Corporation"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:15
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:37
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:36
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:32
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:32
 msgid "Avg FATs"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/alliance/tabs/corporations.html:16
 msgid "Corporation statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:31
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:6
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:8
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:26
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:22
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:7
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:6
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:19
 msgid "FATs by ship type"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:13
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:9
 msgid "Corporation performance"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:18
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:55
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:13
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:64
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:12
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:79
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:9
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:62
 msgid "FATs by time"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:23
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:80
-#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:18
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:15
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:106
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:12
 #: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:89
 msgid "FATs by weekday"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:105
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:35
+msgid "Ship Types"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:51
 msgid "Average FATs by corporation"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:4
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:4
-msgid "Graphs"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:62
+msgid "Average # of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/alliance/tabs_navigation.html:5
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:11
-msgid "Corporations"
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:90
+#: afat/templates/afat/partials/statistics/alliance/tabs/graphs.html:117
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:44
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:73
+#: afat/templates/afat/partials/statistics/corporation/tabs/graphs.html:100
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:31
+msgid "# of FATs"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:28
-msgid "FATs by time of day"
+#: afat/templates/afat/partials/statistics/character/tabs-navigation.html:7
+msgid "Raw data"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:37
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:36
-msgid "# of FATs"
+#: afat/templates/afat/partials/statistics/character/tabs/graphs.html:33
+msgid "FATs by time of day"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:5
 msgid "FATs for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/character/tabs/raw_data.html:10
 msgid "Name"
-msgstr "名字"
-
-#: afat/templates/afat/partials/statistics/character/tabs_navigation.html:7
-msgid "Raw data"
 msgstr ""
 
+#: afat/templates/afat/partials/statistics/corporation/tabs-navigation.html:7
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:5
-#: afat/templates/afat/partials/statistics/corporation/tabs_navigation.html:5
 msgid "Members"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/corporation/tabs/member.html:12
 msgid "Character statistics"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:7
-msgid ""
-"Corporations <small>(Click on an alliance name to see their corporations)</"
-"small>"
+#: afat/templates/afat/partials/statistics/overview/tabs-navigation.html:4
+msgid "My Stats"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:10
+msgid "Click on an alliance name to see their corporations"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:35
+msgid "Alliance statistics for"
+msgstr ""
+
+#: afat/templates/afat/partials/statistics/overview/tabs/corps.html:61
+msgid "Corporation statistics for"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:7
 msgid "Your monthly stats"
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:10
-msgid "Only months with FAT data of the selected year are shown."
+msgid "Only months with FAT data for the selected year are shown."
 msgstr ""
 
 #: afat/templates/afat/partials/statistics/overview/tabs/mine.html:11
 msgid "Only characters that have FATs for the selected year are shown."
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:34
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:33
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:32
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:29
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:28
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:28
 msgid "Month"
-msgstr "月"
+msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:35
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:30
 msgid "FAT count"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:56
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:51
 msgid "No FATs for"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:64
+#: afat/templates/afat/partials/statistics/overview/tabs/mine.html:59
 msgid "No FATs for this year at all"
 msgstr ""
 
-#: afat/templates/afat/partials/statistics/overview/tabs_navigation.html:6
-msgid "My Stats"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:4
-msgid "Previous year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:9
-msgid "Next year"
-msgstr ""
-
-#: afat/templates/afat/partials/year_navigation.html:10
-msgid "Current year"
-msgstr ""
-
-#: afat/templates/afat/view/dashboard/dashboard.html:16
+#: afat/templates/afat/view/dashboard/dashboard.html:12
 msgid "Recent activity"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:29
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:54
+#: afat/templates/afat/view/dashboard/dashboard.html:24
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:49
 msgid "Delete FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:58
+#: afat/templates/afat/view/dashboard/dashboard.html:53
 msgid "No recent FATs for"
 msgstr ""
 
-#: afat/templates/afat/view/dashboard/dashboard.html:59
+#: afat/templates/afat/view/dashboard/dashboard.html:54
 msgid "No recent FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_add_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html:11
 msgid "Create a FAT link"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:11
 msgid "FAT link details"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_details_fatlink.html:34
+#: afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html:28
 msgid "Delete FAT"
 msgstr ""
 
-#: afat/templates/afat/view/fatlinks/fatlinks_overview.html:15
+#: afat/templates/afat/view/fatlinks/fatlinks-overview.html:11
 msgid "All FAT links"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:6
-#, fuzzy
-#| msgid "Fleet Activity Tracking"
+#: afat/templates/afat/view/logs/logs-overview.html:6
 msgid "Fleet activity tracking logs"
-msgstr "舰队活动历史"
-
-#: afat/templates/afat/view/logs/logs_overview.html:17
-#, python-format
-msgid ""
-"\n"
-"            Logs are only kept for %(log_duration)s days. Logs older than "
-"that are removed automatically.\n"
-"        "
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:29
+#: afat/templates/afat/view/logs/logs-overview.html:21
 msgid "Time"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:30
+#: afat/templates/afat/view/logs/logs-overview.html:22
 msgid "Event"
 msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:31
+#: afat/templates/afat/view/logs/logs-overview.html:23
 msgid "User"
-msgstr "用户"
+msgstr ""
 
-#: afat/templates/afat/view/logs/logs_overview.html:33
+#: afat/templates/afat/view/logs/logs-overview.html:25
 msgid "Description"
 msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance.html:7
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:7
-#: afat/templates/afat/view/statistics/statistics_character.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation.html:6
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:7
-#, fuzzy
-#| msgid "Fleet Activity Tracking"
+#: afat/templates/afat/view/logs/logs-overview.html:35
+#, python-format
+msgid ""
+"\n"
+"            Logs are kept for %(duration)s day. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgid_plural ""
+"\n"
+"            Logs are kept for %(duration)s days. Logs older than that are "
+"removed automatically.\n"
+"        "
+msgstr[0] ""
+msgstr[1] ""
+
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-alliance.html:7
+#: afat/templates/afat/view/statistics/statistics-character.html:6
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:7
+#: afat/templates/afat/view/statistics/statistics-corporation.html:6
 msgid "Fleet activity tracking statistics"
-msgstr "舰队活动历史"
+msgstr ""
 
-#: afat/templates/afat/view/statistics/statistics_alliance_year_overview.html:16
-#: afat/templates/afat/view/statistics/statistics_corporation_year_overview.html:16
-#, fuzzy
-#| msgid "Fleet Activity Tracking"
+#: afat/templates/afat/view/statistics/statistics-alliance-year-overview.html:12
+#: afat/templates/afat/view/statistics/statistics-corporation-year-overview.html:12
 msgid "Fleet activity"
-msgstr "舰队活动历史"
+msgstr ""
 
-#: afat/templatetags/filters.py:21
+#: afat/templatetags/afat.py:42
 msgid "January"
-msgstr "一月"
+msgstr ""
 
-#: afat/templatetags/filters.py:22
+#: afat/templatetags/afat.py:43
 msgid "February"
-msgstr "二月"
+msgstr ""
 
-#: afat/templatetags/filters.py:23
+#: afat/templatetags/afat.py:44
 msgid "March"
-msgstr "三月"
+msgstr ""
 
-#: afat/templatetags/filters.py:24
+#: afat/templatetags/afat.py:45
 msgid "April"
-msgstr "四月"
+msgstr ""
 
-#: afat/templatetags/filters.py:25
+#: afat/templatetags/afat.py:46
 msgid "May"
-msgstr "五月"
+msgstr ""
 
-#: afat/templatetags/filters.py:26
+#: afat/templatetags/afat.py:47
 msgid "June"
-msgstr "六月"
+msgstr ""
 
-#: afat/templatetags/filters.py:27
+#: afat/templatetags/afat.py:48
 msgid "July"
-msgstr "七月"
+msgstr ""
 
-#: afat/templatetags/filters.py:28
+#: afat/templatetags/afat.py:49
 msgid "August"
-msgstr "八月"
+msgstr ""
 
-#: afat/templatetags/filters.py:29
+#: afat/templatetags/afat.py:50
 msgid "September"
-msgstr "九月"
+msgstr ""
 
-#: afat/templatetags/filters.py:30
+#: afat/templatetags/afat.py:51
 msgid "October"
-msgstr "十月"
+msgstr ""
 
-#: afat/templatetags/filters.py:31
+#: afat/templatetags/afat.py:52
 msgid "November"
-msgstr "十一月"
+msgstr ""
 
-#: afat/templatetags/filters.py:32
+#: afat/templatetags/afat.py:53
 msgid "December"
-msgstr "十二月"
+msgstr ""
 
 #: afat/views/fatlinks.py:220
 msgid ""
 "<h4>Success!</h4><p>Clickable FAT link created!</p><p>Make sure to give your "
 "fleet members the link to click so that they get credit for this fleet.</p>"
 msgstr ""
 
@@ -1110,54 +1138,54 @@
 
 #: afat/views/fatlinks.py:1184
 msgid ""
 "<h4>Warning!</h4><p>This FAT link has already been re-opened. FAT links can "
 "be re-opened only once!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:221
+#: afat/views/statistics.py:235
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for this "
 "character.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:234
+#: afat/views/statistics.py:248
 msgid "<h4>Warning!</h4><p>Date information not complete!</p>"
 msgstr ""
 
-#: afat/views/statistics.py:349
+#: afat/views/statistics.py:369
 msgid ""
 "<h4>Warning!</h4><p>You do not have permission to view statistics for that "
 "corporation.</p>"
 msgstr ""
 
-#: afat/views/statistics.py:467 afat/views/statistics.py:701
+#: afat/views/statistics.py:487 afat/views/statistics.py:727
 msgid "Monday"
-msgstr "周一"
+msgstr ""
 
-#: afat/views/statistics.py:468 afat/views/statistics.py:702
+#: afat/views/statistics.py:488 afat/views/statistics.py:728
 msgid "Tuesday"
-msgstr "周二"
+msgstr ""
 
-#: afat/views/statistics.py:469 afat/views/statistics.py:703
+#: afat/views/statistics.py:489 afat/views/statistics.py:729
 msgid "Wednesday"
-msgstr "周三"
+msgstr ""
 
-#: afat/views/statistics.py:470 afat/views/statistics.py:704
+#: afat/views/statistics.py:490 afat/views/statistics.py:730
 msgid "Thursday"
-msgstr "周四"
+msgstr ""
 
-#: afat/views/statistics.py:471 afat/views/statistics.py:705
+#: afat/views/statistics.py:491 afat/views/statistics.py:731
 msgid "Friday"
-msgstr "星期五"
+msgstr ""
 
-#: afat/views/statistics.py:472 afat/views/statistics.py:706
+#: afat/views/statistics.py:492 afat/views/statistics.py:732
 msgid "Saturday"
-msgstr "周六"
+msgstr ""
 
-#: afat/views/statistics.py:473 afat/views/statistics.py:707
+#: afat/views/statistics.py:493 afat/views/statistics.py:733
 msgid "Sunday"
-msgstr "星期日"
+msgstr ""
 
-#: afat/views/statistics.py:584
+#: afat/views/statistics.py:610
 msgid "<h4>Error!</h4><p>Date information incomplete.</p>"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `allianceauth_afat-3.0.0b3/afat/management/commands/afat_import_from_allianceauth_fat.py` & `allianceauth_afat-3.0.1/afat/management/commands/afat_import_from_allianceauth_fat.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0001_initial.py` & `allianceauth_afat-3.0.1/afat/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0002_manualfat.py` & `allianceauth_afat-3.0.1/afat/migrations/0002_manualfat.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0003_auto_20180911_0831.py` & `allianceauth_afat-3.0.1/afat/migrations/0003_auto_20180911_0831.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0004_clickfatduration.py` & `allianceauth_afat-3.0.1/afat/migrations/0004_clickfatduration.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0005_auto_20200816_2042.py` & `allianceauth_afat-3.0.1/afat/migrations/0005_auto_20200816_2042.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0006_auto_20200820_2013.py` & `allianceauth_afat-3.0.1/afat/migrations/0006_auto_20200820_2013.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0008_auto_20200912_1116.py` & `allianceauth_afat-3.0.1/afat/migrations/0008_auto_20200912_1116.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0009_auto_20200925_2206.py` & `allianceauth_afat-3.0.1/afat/migrations/0009_auto_20200925_2206.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0010_permissoins_update_20201002_1909.py` & `allianceauth_afat-3.0.1/afat/migrations/0010_permissoins_update_20201002_1909.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0012_manualafat_created_at.py` & `allianceauth_afat-3.0.1/afat/migrations/0012_manualafat_created_at.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0013_basic_module_access_permissions.py` & `allianceauth_afat-3.0.1/afat/migrations/0013_basic_module_access_permissions.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0014_auto_20201224_0930.py` & `allianceauth_afat-3.0.1/afat/migrations/0014_auto_20201224_0930.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0015_afatlink_character.py` & `allianceauth_afat-3.0.1/afat/migrations/0015_afatlink_character.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0016_permissions_overhaul.py` & `allianceauth_afat-3.0.1/afat/migrations/0016_permissions_overhaul.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0017_remove_soft_deletion.py` & `allianceauth_afat-3.0.1/afat/migrations/0017_remove_soft_deletion.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0018_auto_20210420_2016.py` & `allianceauth_afat-3.0.1/afat/migrations/0018_auto_20210420_2016.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0019_add_several_indices.py` & `allianceauth_afat-3.0.1/afat/migrations/0019_add_several_indices.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0020_auto_20210617_1037.py` & `allianceauth_afat-3.0.1/afat/migrations/0020_auto_20210617_1037.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0022_afatlink_esi_error_count.py` & `allianceauth_afat-3.0.1/afat/migrations/0022_afatlink_esi_error_count.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/migrations/0023_the_big_rename.py` & `allianceauth_afat-3.0.1/afat/migrations/0023_the_big_rename.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/css/afat.css` & `allianceauth_afat-3.0.1/afat/static/afat/css/afat.css`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/css/afat.min.css` & `allianceauth_afat-3.0.1/afat/static/afat/css/afat.min.css`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/css/afat.min.css.map` & `allianceauth_afat-3.0.1/afat/static/afat/css/afat.min.css.map`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-dashboard.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-dashboard.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-dashboard.min.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-dashboard.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-dashboard.min.js.map` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-dashboard.min.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-datatables-common.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-datatables-common.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlink-details.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlink-details.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlink-details.min.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlink-details.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlink-details.min.js.map` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlink-details.min.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlist.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlist.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlist.min.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlist.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-fatlist.min.js.map` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-fatlist.min.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-logs.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-logs.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-logs.min.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-logs.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-logs.min.js.map` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-logs.min.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat-statistics.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat-statistics.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat.min.js` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/javascript/afat.min.js.map` & `allianceauth_afat-3.0.1/afat/static/afat/javascript/afat.min.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/libs/Chart.js/2.7.2/chart.min.js` & `allianceauth_afat-3.0.1/afat/static/afat/libs/Chart.js/2.7.2/chart.min.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/libs/Chart.js/4.4.1/chart.umd.js` & `allianceauth_afat-3.0.1/afat/static/afat/libs/Chart.js/4.4.1/chart.umd.js`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/static/afat/libs/Chart.js/4.4.1/chart.umd.js.map` & `allianceauth_afat-3.0.1/afat/static/afat/libs/Chart.js/4.4.1/chart.umd.js.map`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/base.html` & `allianceauth_afat-3.0.1/afat/templates/afat/base.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/modals/general.html` & `allianceauth_afat-3.0.1/afat/templates/afat/modals/general.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/common/navigation/month-navigation.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/common/navigation/month-navigation.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/common/navigation/tab-character.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/common/navigation/tab-character.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/common/navigation/top-menu.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/common/navigation/top-menu.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/common/navigation/year-navigation.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/common/navigation/year-navigation.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/dashboard/tabs-navigation.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/dashboard/tabs-navigation.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/dashboard/tabs/fatlinks.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/dashboard/tabs/fatlinks.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/dashboard/tabs/fats.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/dashboard/tabs/fats.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/open-esi-fleets.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/open-esi-fleets.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/add/clickable-link.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/add/clickable-link.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/add/esi-link.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/add/esi-link.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/fatlink-info.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/fatlink-info.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/fatlink-name-form.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/tabs-navigation.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/tabs-navigation.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/tabs/fats.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/tabs/fats.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/fatlinks/details/tabs/manualfat.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/alliance/tabs/corporations.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/alliance/tabs/corporations.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/alliance/tabs/graphs.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/alliance/tabs/graphs.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/character/tabs/graphs.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/character/tabs/graphs.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/character/tabs/raw_data.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/character/tabs/raw_data.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/corporation/tabs/graphs.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/corporation/tabs/graphs.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/corporation/tabs/member.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/corporation/tabs/member.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/overview/tabs-navigation.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/overview/tabs-navigation.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/overview/tabs/corps.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/overview/tabs/corps.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/partials/statistics/overview/tabs/mine.html` & `allianceauth_afat-3.0.1/afat/templates/afat/partials/statistics/overview/tabs/mine.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/dashboard/dashboard.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/dashboard/dashboard.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/fatlinks/fatlinks-add-fatlink.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/fatlinks/fatlinks-details-fatlink.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/fatlinks/fatlinks-overview.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/fatlinks/fatlinks-overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/logs/logs-overview.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/logs/logs-overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-alliance-year-overview.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-alliance-year-overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-alliance.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-alliance.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-character.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-character.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-corporation-year-overview.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-corporation-year-overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-corporation.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-corporation.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templates/afat/view/statistics/statistics-overview.html` & `allianceauth_afat-3.0.1/afat/templates/afat/view/statistics/statistics-overview.html`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/templatetags/afat.py` & `allianceauth_afat-3.0.1/afat/templatetags/afat.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/test_access.py` & `allianceauth_afat-3.0.1/afat/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/test_helpers.py` & `allianceauth_afat-3.0.1/afat/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/test_templatetags.py` & `allianceauth_afat-3.0.1/afat/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/test_views_dashboard.py` & `allianceauth_afat-3.0.1/afat/tests/test_views_dashboard.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/test_views_fatlinks.py` & `allianceauth_afat-3.0.1/afat/tests/test_views_fatlinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/test_views_logs.py` & `allianceauth_afat-3.0.1/afat/tests/test_views_logs.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/test_views_statistics.py` & `allianceauth_afat-3.0.1/afat/tests/test_views_statistics.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/fixtures/allianceauth.json` & `allianceauth_afat-3.0.1/afat/tests/fixtures/allianceauth.json`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/fixtures/generate_fat_links.py` & `allianceauth_afat-3.0.1/afat/tests/fixtures/generate_fat_links.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/tests/fixtures/load_allianceauth.py` & `allianceauth_afat-3.0.1/afat/tests/fixtures/load_allianceauth.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/views/dashboard.py` & `allianceauth_afat-3.0.1/afat/views/dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         .order_by("-created")[:10]
         .values_list("id", flat=True)
     )
 
     fatlinks = (
         FatLink.objects.filter(id__in=fatlink_ids)
         .order_by("-created")
-        .annotate_fats_count()
+        .annotate_fats_count()  # pylint: disable=duplicate-code
     )
 
     fatlink_rows = [
         convert_fatlinks_to_dict(
             request=request,
             fatlink=fatlink,
             close_esi_redirect=reverse(viewname="afat:dashboard"),
```

### Comparing `allianceauth_afat-3.0.0b3/afat/views/fatlinks.py` & `allianceauth_afat-3.0.1/afat/views/fatlinks.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/views/logs.py` & `allianceauth_afat-3.0.1/afat/views/logs.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/afat/views/statistics.py` & `allianceauth_afat-3.0.1/afat/views/statistics.py`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/LICENSE` & `allianceauth_afat-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `allianceauth_afat-3.0.0b3/README.md` & `allianceauth_afat-3.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,24 @@
 
 ### Add Fat Link View for FCs<a name="add-fat-link-view-for-fcs"></a>
 
 ![Add Fat Link View for FCs](https://raw.githubusercontent.com/ppfeufer/allianceauth-afat/master/docs/images/add-fatlink.png "Add Fat Link View for FCs")
 
 ## Installation<a name="installation"></a>
 
+> \[!NOTE\]
+>
+> **Alliance Auth AFAT >= 3.0.0 needs at least Alliance Auth v4.0.0!**
+>
+> Please make sure to update your Alliance Auth instance _before_ you install this
+> module or update to the latest version, otherwise an update to Alliance Auth will
+> be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `2.13.0`.
+
 ### Important<a name="important"></a>
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding. (See the official
 [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
 for details)
```

### Comparing `allianceauth_afat-3.0.0b3/pyproject.toml` & `allianceauth_afat-3.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,22 +28,23 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth>=4.0.0b2",
+    "allianceauth<5.0.0,>=4",
     "allianceauth-app-utils>=1.14.1",
     "unidecode>=1.3.4",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
     "coverage",
     "django-webtest",
```

### Comparing `allianceauth_afat-3.0.0b3/PKG-INFO` & `allianceauth_afat-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: allianceauth-afat
-Version: 3.0.0b3
+Version: 3.0.1
 Summary: Another Fleet Activity Tracking tool for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/allianceauth-afat/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/allianceauth-afat/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/allianceauth-afat
 Project-URL: Source, https://github.com/ppfeufer/allianceauth-afat.git
 Project-URL: Tracker, https://github.com/ppfeufer/allianceauth-afat/issues
@@ -693,19 +693,20 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.14.1
-Requires-Dist: allianceauth>=4.0.0b2
+Requires-Dist: allianceauth<5.0.0,>=4
 Requires-Dist: unidecode>=1.3.4
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
 
 # Alliance Auth AFAT — Another Fleet Activity Tracker<a name="alliance-auth-afat-%E2%80%94-another-fleet-activity-tracker"></a>
@@ -801,14 +802,24 @@
 
 ### Add Fat Link View for FCs<a name="add-fat-link-view-for-fcs"></a>
 
 ![Add Fat Link View for FCs](https://raw.githubusercontent.com/ppfeufer/allianceauth-afat/master/docs/images/add-fatlink.png "Add Fat Link View for FCs")
 
 ## Installation<a name="installation"></a>
 
+> \[!NOTE\]
+>
+> **Alliance Auth AFAT >= 3.0.0 needs at least Alliance Auth v4.0.0!**
+>
+> Please make sure to update your Alliance Auth instance _before_ you install this
+> module or update to the latest version, otherwise an update to Alliance Auth will
+> be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `2.13.0`.
+
 ### Important<a name="important"></a>
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding. (See the official
 [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
 for details)
```

