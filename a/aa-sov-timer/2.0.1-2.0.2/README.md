# Comparing `tmp/aa_sov_timer-2.0.1.tar.gz` & `tmp/aa_sov_timer-2.0.2.tar.gz`

## Comparing `aa_sov_timer-2.0.1.tar` & `aa_sov_timer-2.0.2.tar`

### file list

```diff
@@ -1,76 +1,84 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/apps.py
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/auth_hooks.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/constants.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/models.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/providers.py
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tasks.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/urls.py
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/.gitkeep
--rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/django.pot
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5436 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5608 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4938 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4263 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/management/commands/__init__.py
--rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/management/commands/sovtimer_load_initial_data.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/0001_initial.py
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/0002_aasovtimercampaigns_aasovtimerstructures.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/0003_auto_20201113_1033.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/0004_auto_20201113_1856.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/0005_auto_20201114_0720.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/0006_rename_models.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/0007_cleanup_models.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/0008_fix_campaign_attackers_score.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/0009_alter_campaign_options_and_more.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/migrations/__init__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/css/aa-sov-timer.css
--rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/css/aa-sov-timer.min.css
--rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/css/aa-sov-timer.min.css.map
--rw-r--r--   0        0        0    33122 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.codepoints
--rw-r--r--   0        0        0   285724 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.ttf
--rw-r--r--   0        0        0   110560 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.woff2
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/font/materialicons/v103/README.md
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/images/zkillboard.png
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/js/aa-sov-timer.js
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/js/aa-sov-timer.min.js
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/static/sovtimer/js/aa-sov-timer.min.js.map
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/base.html
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/dashboard.html
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/bundles/aa-sov-timer-css.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/bundles/aa-sov-timer-js.html
--rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/partials/dashboard/table.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/partials/header/h1.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/templatetags/__init__.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/templatetags/sovtimer.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/__init__.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/test_ajax_calls.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/test_integration.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/test_templatetags.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/utils.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/fixtures/allianceauth.json
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/fixtures/load_allianceauth.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/fixtures/load_sovtimer.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/fixtures/sovtimer.json
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/sovtimer/tests/fixtures/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/LICENSE
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/README.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    49701 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/apps.py
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/auth_hooks.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/constants.py
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/models.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/providers.py
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tasks.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/urls.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/.gitkeep
+-rw-r--r--   0        0        0     3852 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/django.pot
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2255 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/management/commands/__init__.py
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/management/commands/sovtimer_load_initial_data.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/0002_aasovtimercampaigns_aasovtimerstructures.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/0003_auto_20201113_1033.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/0004_auto_20201113_1856.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/0005_auto_20201114_0720.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/0006_rename_models.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/0007_cleanup_models.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/0008_fix_campaign_attackers_score.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/0009_alter_campaign_options_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/migrations/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/css/aa-sov-timer.css
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/css/aa-sov-timer.min.css
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/css/aa-sov-timer.min.css.map
+-rw-r--r--   0        0        0    33122 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.codepoints
+-rw-r--r--   0        0        0   285724 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.ttf
+-rw-r--r--   0        0        0   110560 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.woff2
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/font/materialicons/v103/README.md
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/images/zkillboard.png
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/js/aa-sov-timer.js
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/js/aa-sov-timer.min.js
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/static/sovtimer/js/aa-sov-timer.min.js.map
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/base.html
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/dashboard.html
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/bundles/aa-sov-timer-css.html
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/bundles/aa-sov-timer-js.html
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/partials/dashboard/table.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/partials/header/h1.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/templatetags/__init__.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/templatetags/sovtimer.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/__init__.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/test_ajax_calls.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/test_integration.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/utils.py
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/fixtures/allianceauth.json
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/fixtures/load_allianceauth.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/fixtures/load_sovtimer.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/fixtures/sovtimer.json
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/sovtimer/tests/fixtures/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/LICENSE
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/README.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    49701 2020-02-02 00:00:00.000000 aa_sov_timer-2.0.2/PKG-INFO
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/auth_hooks.py` & `aa_sov_timer-2.0.2/sovtimer/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/models.py` & `aa_sov_timer-2.0.2/sovtimer/models.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/tasks.py` & `aa_sov_timer-2.0.2/sovtimer/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/views.py` & `aa_sov_timer-2.0.2/sovtimer/views.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/django.pot` & `aa_sov_timer-2.0.2/sovtimer/locale/django.pot`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-16 00:17+0100\n"
+"POT-Creation-Date: 2024-03-20 17:11+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/de/LC_MESSAGES/django.mo` & `aa_sov_timer-2.0.2/sovtimer/locale/de/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-sov-timer/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "ADM"
 msgstr "ADM"
 
 msgid "Active campaign"
 msgstr "Aktive Kampagne"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/de/LC_MESSAGES/django.po` & `aa_sov_timer-2.0.2/sovtimer/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 00:17+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"PO-Revision-Date: 2024-05-10 14:12+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-sov-timer/de/>\n"
+"Language-Team: German <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-sov-timer/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: sovtimer/__init__.py:9
 msgid "Sovereignty Timers"
 msgstr "Souveränitäts-Timer"
 
 #: sovtimer/apps.py:20
 #, python-brace-format
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/es/LC_MESSAGES/django.mo` & `aa_sov_timer-2.0.2/sovtimer/locale/es/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-sov-timer/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "ADM"
 msgstr "ADM"
 
 msgid "Attackers making progress"
 msgstr "Progreso del Atacante"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/es/LC_MESSAGES/django.po` & `aa_sov_timer-2.0.2/sovtimer/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 00:17+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"PO-Revision-Date: 2024-05-10 14:12+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-sov-timer/es/>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-sov-timer/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: sovtimer/__init__.py:9
 msgid "Sovereignty Timers"
 msgstr "Temporizadores de Soberanía"
 
 #: sovtimer/apps.py:20
 #, python-brace-format
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_sov_timer-2.0.2/sovtimer/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,18 +7,24 @@
 "Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-sov-timer/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 "Voulez-vous aider à traduire cette application dans votre langue ou "
 "améliorer la traduction existante ?"
 
 msgid "Join our team of translators!"
 msgstr "Rejoignez notre équipe de traducteurs !"
+
+msgid "System"
+msgstr "Système"
+
+msgid "Type"
+msgstr "Type"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/fr_FR/LC_MESSAGES/django.po` & `aa_sov_timer-2.0.2/sovtimer/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # erka Ekanon <M6musicT@hotmail.fr>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
+# Matthias P <randomusernetcom@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 00:17+0100\n"
-"PO-Revision-Date: 2024-01-12 19:05+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-sov-timer/fr/>\n"
+"PO-Revision-Date: 2024-05-10 14:12+0000\n"
+"Last-Translator: Matthias P <randomusernetcom@gmail.com>\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-sov-timer/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: sovtimer/__init__.py:9
 msgid "Sovereignty Timers"
 msgstr ""
 
 #: sovtimer/apps.py:20
 #, python-brace-format
@@ -60,15 +61,15 @@
 #: sovtimer/models.py:139
 msgid "Sovereignty campaigns"
 msgstr ""
 
 #: sovtimer/templates/sovtimer/dashboard.html:15
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:27
 msgid "System"
-msgstr ""
+msgstr "Système"
 
 #: sovtimer/templates/sovtimer/dashboard.html:16
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:28
 msgid "Constellation"
 msgstr ""
 
 #: sovtimer/templates/sovtimer/dashboard.html:17
@@ -114,15 +115,15 @@
 
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:18
 msgid "Timers active:"
 msgstr ""
 
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:26
 msgid "Type"
-msgstr ""
+msgstr "Type"
 
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:31
 msgid "ADM"
 msgstr ""
 
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:32
 msgid "Start"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/it_IT/LC_MESSAGES/django.po` & `aa_sov_timer-2.0.2/sovtimer/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 00:17+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"PO-Revision-Date: 2024-05-10 14:12+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-sov-timer/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-sov-timer/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: sovtimer/__init__.py:9
 msgid "Sovereignty Timers"
 msgstr ""
 
 #: sovtimer/apps.py:20
 #, python-brace-format
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/ja/LC_MESSAGES/django.mo` & `aa_sov_timer-2.0.2/sovtimer/locale/ja/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,14 +7,14 @@
 "Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-sov-timer/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "No"
 msgstr "いいえ"
 
 msgid "Yes"
 msgstr "はい"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/ja/LC_MESSAGES/django.po` & `aa_sov_timer-2.0.2/sovtimer/locale/ja/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

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
 "POT-Creation-Date: 2024-03-16 00:17+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"PO-Revision-Date: 2024-05-10 14:12+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-sov-timer/ja/>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-sov-timer/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: sovtimer/__init__.py:9
 msgid "Sovereignty Timers"
 msgstr ""
 
 #: sovtimer/apps.py:20
 #, python-brace-format
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_sov_timer-2.0.2/sovtimer/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,75 +7,84 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-sov-timer/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "ADM"
 msgstr "ADM"
 
 msgid "Attackers making progress"
 msgstr "공격자 우세"
 
+msgid "Can access the Sovereignty Timer module"
+msgstr "소버린티 타이머 모듈에 접근할 수 있는 권한"
+
 msgid "Constellation"
-msgstr "성좌"
+msgstr "컨스털레이션"
 
 msgid "Defenders making progress"
 msgstr "방어자 우세"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
 msgid "Neither side has made any progress yet"
 msgstr "양 측 모두 진행하지 못하고 있습니다"
 
 msgid "No"
 msgstr "아니요"
 
 msgid "Owner / Defender"
 msgstr "소유자 / 방어자"
 
 msgid "Progress"
 msgstr "진행도"
 
 msgid "Region"
-msgstr "지역"
+msgstr "리전"
 
 msgid "Remaining"
 msgstr "남은 시간"
 
 msgid "Sovereignty Timer"
 msgstr "소버린티 타이머"
 
 msgid "Sovereignty Timer v{__version__}"
 msgstr "소버린티 타이머 v{__version__}"
 
 msgid "Sovereignty Timers"
 msgstr "소버린티 타이머"
 
+msgid "Sovereignty campaign"
+msgstr "소버린티 캠페인"
+
 msgid "Start"
 msgstr "시작 시각"
 
 msgid "System"
-msgstr "성계"
+msgstr "시스템"
 
 msgid ""
 "The sovereignty timer list is automatically updated every 30 seconds. "
 "Progress for any active campaigns will be shown as <i>Previous - Trend - "
 "Current</i>."
 msgstr ""
 "소버린티 타이머 리스트는 30초마다 자동으로 업데이트 됩니다. 진행 중인 캠페인"
 "의 진행도는 <i>이전 - 변화량 - 현재</i>로 표시됩니다."
 
+msgid "Timers total:"
+msgstr "타이머 수:"
+
 msgid "Type"
 msgstr "종류"
 
 msgid "Yes"
 msgstr "예"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/ko_KR/LC_MESSAGES/django.po` & `aa_sov_timer-2.0.2/sovtimer/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
-# Author50CO <tkddlschry@gmail.com>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Author50CO <tkddlschry@gmail.com>, 2023, 2024.
+# Mind of the Raven <okanieva@gmail.com>, 2024.
+# Rodpold Shard <rodpold@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 00:17+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
-"Last-Translator: Author50CO <tkddlschry@gmail.com>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-sov-timer/ko/>\n"
+"PO-Revision-Date: 2024-05-10 14:12+0000\n"
+"Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-sov-timer/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: sovtimer/__init__.py:9
 msgid "Sovereignty Timers"
 msgstr "소버린티 타이머"
 
 #: sovtimer/apps.py:20
 #, python-brace-format
@@ -30,24 +32,22 @@
 
 #: sovtimer/models.py:33 sovtimer/templates/sovtimer/base.html:6
 #: sovtimer/templates/sovtimer/base.html:10
 msgid "Sovereignty Timer"
 msgstr "소버린티 타이머"
 
 #: sovtimer/models.py:36
-#, fuzzy
-#| msgid "Sovereignty Timer"
 msgid "Can access the Sovereignty Timer module"
-msgstr "소버린티 타이머"
+msgstr "소버린티 타이머 모듈에 접근할 수 있는 권한"
 
 #: sovtimer/models.py:73
 #, fuzzy
 #| msgid "Sovereignty Timer"
 msgid "Sovereignty structure"
-msgstr "소버린티 타이머"
+msgstr "소버린티 구조물"
 
 #: sovtimer/models.py:74
 #, fuzzy
 #| msgid "Sovereignty Timers"
 msgid "Sovereignty structures"
 msgstr "소버린티 타이머"
 
@@ -60,39 +60,37 @@
 #: sovtimer/models.py:112
 #, fuzzy
 #| msgid "TCU Defense"
 msgid "TCU defense"
 msgstr "TCU 방어"
 
 #: sovtimer/models.py:138
-#, fuzzy
-#| msgid "Sovereignty Campaign List"
 msgid "Sovereignty campaign"
-msgstr "소버린티 캠페인 목록"
+msgstr "소버린티 캠페인"
 
 #: sovtimer/models.py:139
 #, fuzzy
 #| msgid "Sovereignty Campaign List"
 msgid "Sovereignty campaigns"
 msgstr "소버린티 캠페인 목록"
 
 #: sovtimer/templates/sovtimer/dashboard.html:15
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:27
 msgid "System"
-msgstr "성계"
+msgstr "시스템"
 
 #: sovtimer/templates/sovtimer/dashboard.html:16
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:28
 msgid "Constellation"
-msgstr "성좌"
+msgstr "컨스털레이션"
 
 #: sovtimer/templates/sovtimer/dashboard.html:17
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:29
 msgid "Region"
-msgstr "지역"
+msgstr "리전"
 
 #: sovtimer/templates/sovtimer/dashboard.html:18
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:30
 msgid "Owner / Defender"
 msgstr "소유자 / 방어자"
 
 #: sovtimer/templates/sovtimer/dashboard.html:19
@@ -111,26 +109,24 @@
 
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:4
 msgid ""
 "The sovereignty timer list is automatically updated every 30 seconds. "
 "Progress for any active campaigns will be shown as <i>Previous - Trend - "
 "Current</i>."
 msgstr ""
-"소버린티 타이머 리스트는 30초마다 자동으로 업데이트 됩니다. 진행 중인 캠페인"
-"의 진행도는 <i>이전 - 변화량 - 현재</i>로 표시됩니다."
+"소버린티 타이머 리스트는 30초마다 자동으로 업데이트 됩니다. 진행 중인 "
+"캠페인의 진행도는 <i>이전 - 변화량 - 현재</i>로 표시됩니다."
 
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:10
 #, fuzzy
 #| msgid "Sovereignty Campaign List"
 msgid "Sovereignty campaign list"
 msgstr "소버린티 캠페인 목록"
 
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:16
-#, fuzzy
-#| msgid "Timers Total:"
 msgid "Timers total:"
 msgstr "타이머 수:"
 
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:17
 #, fuzzy
 #| msgid "Timers Upcoming (< 4hrs):"
 msgid "Timers upcoming (< 4hrs):"
@@ -166,15 +162,15 @@
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: sovtimer/templates/sovtimer/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
 #: sovtimer/views.py:163
 msgid "Neither side has made any progress yet"
 msgstr "양 측 모두 진행하지 못하고 있습니다"
 
 #: sovtimer/views.py:171
 msgid "Defenders making progress"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/ru/LC_MESSAGES/django.mo` & `aa_sov_timer-2.0.2/sovtimer/locale/ru/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-sov-timer/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "ADM"
 msgstr "АДМ"
 
 msgid "Active campaign"
 msgstr "Активная кампания"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/ru/LC_MESSAGES/django.po` & `aa_sov_timer-2.0.2/sovtimer/locale/ru/LC_MESSAGES/django.po`

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
 "POT-Creation-Date: 2024-03-16 00:17+0100\n"
-"PO-Revision-Date: 2023-10-03 16:43+0000\n"
+"PO-Revision-Date: 2024-05-10 14:12+0000\n"
 "Last-Translator: Max <mark25@inbox.ru>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-sov-timer/ru/>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-sov-timer/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: sovtimer/__init__.py:9
 msgid "Sovereignty Timers"
 msgstr "Таймеры суверенитета"
 
 #: sovtimer/apps.py:20
 #, python-brace-format
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/uk/LC_MESSAGES/django.mo` & `aa_sov_timer-2.0.2/sovtimer/locale/uk/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-sov-timer/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Constellation"
 msgstr "Сузірʼя"
 
 msgid "Owner / Defender"
 msgstr "Власник / Захисник"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/uk/LC_MESSAGES/django.po` & `aa_sov_timer-2.0.2/sovtimer/locale/uk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "Andrii M." <elfleg0las88@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# "Andrii M." <elfleg0las88@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 00:17+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"PO-Revision-Date: 2024-05-10 14:12+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-sov-timer/uk/>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-sov-timer/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: sovtimer/__init__.py:9
 msgid "Sovereignty Timers"
 msgstr "Таймера суверенітету"
 
 #: sovtimer/apps.py:20
 #, python-brace-format
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_sov_timer-2.0.2/sovtimer/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,28 +7,43 @@
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-sov-timer/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
+
+msgid "Constellation"
+msgstr "星座"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
 msgid "Join our team of translators!"
 msgstr "加入我们的翻译团队吧！"
 
 msgid "No"
 msgstr "不"
 
+msgid "Owner / Defender"
+msgstr "拥有者/防御方"
+
+msgid "Region"
+msgstr "星域"
+
 msgid "Sovereignty Timer"
 msgstr "主权宣布设施计时器"
 
+msgid "Sovereignty Timer v{__version__}"
+msgstr "主权宣布设施计时器{__version__}"
+
 msgid "Sovereignty Timers"
 msgstr "主权宣布设施计时器"
 
+msgid "System"
+msgstr "星系"
+
 msgid "Yes"
 msgstr "是"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_sov_timer-2.0.2/sovtimer/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 # Faer Yili <yilifaer@gmail.com>, 2024.
 # Dehao Wu <wudehao2000@163.com>, 2024.
+# MxdHana <236833425@qq.com>, 2024.
+# SAM_FPS <sam_fps@163.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 00:17+0100\n"
-"PO-Revision-Date: 2024-01-11 21:04+0000\n"
-"Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
+"PO-Revision-Date: 2024-05-15 09:21+0000\n"
+"Last-Translator: SAM_FPS <sam_fps@163.com>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-sov-timer/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: sovtimer/__init__.py:9
 msgid "Sovereignty Timers"
 msgstr "主权宣布设施计时器"
 
 #: sovtimer/apps.py:20
 #, python-brace-format
 msgid "Sovereignty Timer v{__version__}"
-msgstr ""
+msgstr "主权宣布设施计时器{__version__}"
 
 #: sovtimer/models.py:33 sovtimer/templates/sovtimer/base.html:6
 #: sovtimer/templates/sovtimer/base.html:10
 msgid "Sovereignty Timer"
 msgstr "主权宣布设施计时器"
 
 #: sovtimer/models.py:36
@@ -61,30 +63,30 @@
 #: sovtimer/models.py:139
 msgid "Sovereignty campaigns"
 msgstr ""
 
 #: sovtimer/templates/sovtimer/dashboard.html:15
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:27
 msgid "System"
-msgstr ""
+msgstr "星系"
 
 #: sovtimer/templates/sovtimer/dashboard.html:16
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:28
 msgid "Constellation"
-msgstr ""
+msgstr "星座"
 
 #: sovtimer/templates/sovtimer/dashboard.html:17
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:29
 msgid "Region"
-msgstr ""
+msgstr "星域"
 
 #: sovtimer/templates/sovtimer/dashboard.html:18
 #: sovtimer/templates/sovtimer/partials/dashboard/table.html:30
 msgid "Owner / Defender"
-msgstr ""
+msgstr "拥有者/防御方"
 
 #: sovtimer/templates/sovtimer/dashboard.html:19
 msgid "Active campaign"
 msgstr ""
 
 #: sovtimer/templates/sovtimer/dashboard.html:20 sovtimer/views.py:161
 msgid "Yes"
```

### Comparing `aa_sov_timer-2.0.1/sovtimer/management/commands/sovtimer_load_initial_data.py` & `aa_sov_timer-2.0.2/sovtimer/management/commands/sovtimer_load_initial_data.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/migrations/0001_initial.py` & `aa_sov_timer-2.0.2/sovtimer/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/migrations/0002_aasovtimercampaigns_aasovtimerstructures.py` & `aa_sov_timer-2.0.2/sovtimer/migrations/0002_aasovtimercampaigns_aasovtimerstructures.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/migrations/0003_auto_20201113_1033.py` & `aa_sov_timer-2.0.2/sovtimer/migrations/0003_auto_20201113_1033.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/migrations/0004_auto_20201113_1856.py` & `aa_sov_timer-2.0.2/sovtimer/migrations/0004_auto_20201113_1856.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/migrations/0005_auto_20201114_0720.py` & `aa_sov_timer-2.0.2/sovtimer/migrations/0005_auto_20201114_0720.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/migrations/0006_rename_models.py` & `aa_sov_timer-2.0.2/sovtimer/migrations/0006_rename_models.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/migrations/0007_cleanup_models.py` & `aa_sov_timer-2.0.2/sovtimer/migrations/0007_cleanup_models.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/migrations/0009_alter_campaign_options_and_more.py` & `aa_sov_timer-2.0.2/sovtimer/migrations/0009_alter_campaign_options_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/css/aa-sov-timer.css` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/css/aa-sov-timer.css`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/css/aa-sov-timer.min.css` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/css/aa-sov-timer.min.css`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/css/aa-sov-timer.min.css.map` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/css/aa-sov-timer.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.codepoints` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.codepoints`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.ttf` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.ttf`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.woff2` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/font/materialicons/v103/MaterialIcons-Regular.woff2`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/font/materialicons/v103/README.md` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/font/materialicons/v103/README.md`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/js/aa-sov-timer.js` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/js/aa-sov-timer.js`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/js/aa-sov-timer.min.js` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/js/aa-sov-timer.min.js`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/static/sovtimer/js/aa-sov-timer.min.js.map` & `aa_sov_timer-2.0.2/sovtimer/static/sovtimer/js/aa-sov-timer.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/base.html` & `aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/base.html`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/dashboard.html` & `aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/templates/sovtimer/partials/dashboard/table.html` & `aa_sov_timer-2.0.2/sovtimer/templates/sovtimer/partials/dashboard/table.html`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/templatetags/sovtimer.py` & `aa_sov_timer-2.0.2/sovtimer/templatetags/sovtimer.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/tests/test_ajax_calls.py` & `aa_sov_timer-2.0.2/sovtimer/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/tests/test_integration.py` & `aa_sov_timer-2.0.2/sovtimer/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/tests/test_templatetags.py` & `aa_sov_timer-2.0.2/sovtimer/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/tests/utils.py` & `aa_sov_timer-2.0.2/sovtimer/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/tests/fixtures/allianceauth.json` & `aa_sov_timer-2.0.2/sovtimer/tests/fixtures/allianceauth.json`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/tests/fixtures/load_allianceauth.py` & `aa_sov_timer-2.0.2/sovtimer/tests/fixtures/load_allianceauth.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/tests/fixtures/load_sovtimer.py` & `aa_sov_timer-2.0.2/sovtimer/tests/fixtures/load_sovtimer.py`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/sovtimer/tests/fixtures/sovtimer.json` & `aa_sov_timer-2.0.2/sovtimer/tests/fixtures/sovtimer.json`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/LICENSE` & `aa_sov_timer-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/README.md` & `aa_sov_timer-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/pyproject.toml` & `aa_sov_timer-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_sov_timer-2.0.1/PKG-INFO` & `aa_sov_timer-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-sov-timer
-Version: 2.0.1
+Version: 2.0.2
 Summary: Sov Campaign Timer for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-sov-timer/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-sov-timer/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-sov-timer
 Project-URL: Source, https://github.com/ppfeufer/aa-sov-timer.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-sov-timer/issues
```

