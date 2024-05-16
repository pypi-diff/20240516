# Comparing `tmp/aa_fleetfinder-2.0.0b1.tar.gz` & `tmp/aa_fleetfinder-2.0.1.tar.gz`

## Comparing `aa_fleetfinder-2.0.0b1.tar` & `aa_fleetfinder-2.0.1.tar`

### file list

```diff
@@ -1,63 +1,71 @@
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/__init__.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/apps.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/auth_hooks.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/constants.py
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/models.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/providers.py
--rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/tasks.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/urls.py
--rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/views.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/django.pot
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6722 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7252 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/migrations/0001_initial.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/migrations/0002_esi_error_handling_and_verbose_names.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/migrations/0003_alter_fleet_fleet_commander_alter_fleet_groups_and_more.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/migrations/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/css/fleetfinder.css
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/css/fleetfinder.min.css.map
--rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.css
--rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.min.css
--rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.min.css.map
--rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/js/slimselect.min.js
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/base.html
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/create-fleet.html
--rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/dashboard.html
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/edit-fleet.html
--rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/fleet-details.html
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/join-fleet.html
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templatetags/__init__.py
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/templatetags/fleetfinder.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/tests/__init__.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/tests/test_access.py
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/tests/test_auth_hooks.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/tests/test_templatetags.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/fleetfinder/tests/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/LICENSE
--rw-r--r--   0        0        0     5833 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/README.md
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    48097 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/__init__.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/apps.py
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/auth_hooks.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/constants.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/models.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/providers.py
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/tasks.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/urls.py
+-rw-r--r--   0        0        0    10061 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/views.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/django.pot
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6002 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7257 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2879 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5915 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3315 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6176 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8145 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7239 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/migrations/0001_initial.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/migrations/0002_esi_error_handling_and_verbose_names.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/migrations/0003_alter_fleet_fleet_commander_alter_fleet_groups_and_more.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/migrations/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/css/fleetfinder.css
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/css/fleetfinder.min.css
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/css/fleetfinder.min.css.map
+-rw-r--r--   0        0        0    11846 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.css
+-rw-r--r--   0        0        0     9397 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.min.css
+-rw-r--r--   0        0        0    14992 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.min.css.map
+-rw-r--r--   0        0        0    36199 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/js/slimselect.min.js
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/base.html
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/create-fleet.html
+-rw-r--r--   0        0        0     4575 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/dashboard.html
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/edit-fleet.html
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/fleet-details.html
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/join-fleet.html
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/bundles/css/fleetfinder-css.html
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/bundles/css/slim-select-css.html
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/bundles/js/slim-select-js.html
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templatetags/__init__.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/templatetags/fleetfinder.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/tests/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/tests/test_access.py
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/fleetfinder/tests/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/LICENSE
+-rw-r--r--   0        0        0     5908 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/README.md
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    48171 2020-02-02 00:00:00.000000 aa_fleetfinder-2.0.1/PKG-INFO
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/auth_hooks.py` & `aa_fleetfinder-2.0.1/fleetfinder/auth_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     """
 
     def __init__(self):
         # Setup menu entry for sidebar
         MenuItemHook.__init__(
             self,
             text=__title__,
-            classes="fas fa-users",
+            classes="fa-solid fa-users",
             url_name="fleetfinder:dashboard",
             navactive=["fleetfinder:"],
         )
 
     def render(self, request):
         """
         Render app pages
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/models.py` & `aa_fleetfinder-2.0.1/fleetfinder/models.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/tasks.py` & `aa_fleetfinder-2.0.1/fleetfinder/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/urls.py` & `aa_fleetfinder-2.0.1/fleetfinder/urls.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/views.py` & `aa_fleetfinder-2.0.1/fleetfinder/views.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/de/LC_MESSAGES/django.mo` & `aa_fleetfinder-2.0.1/fleetfinder/locale/de/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetfinder/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>ESI hat den folgenden Fehler zurückgegeben: "
 "{esi_error_message}</p>"
 
@@ -97,14 +97,17 @@
 
 msgid "Fleet members"
 msgstr "Flottenmitglieder"
 
 msgid "Fleet name"
 msgstr "Flottenname"
 
+msgid "Fleets available to you"
+msgstr "Für Dich verfügbare Flotten"
+
 msgid "Free move"
 msgstr "Freie Bewegung"
 
 msgid "Group restrictions"
 msgstr "Gruppenbeschränkungen"
 
 msgid "Join"
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/de/LC_MESSAGES/django.po` & `aa_fleetfinder-2.0.1/fleetfinder/locale/uk/LC_MESSAGES/django.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,225 +1,243 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "Andrii M." <elfleg0las88@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Kristof <kristof@teh.ninja>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-24 16:26+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetfinder/de/>\n"
-"Language: de\n"
+"POT-Creation-Date: 2024-03-15 20:22+0100\n"
+"PO-Revision-Date: 2024-05-10 14:03+0000\n"
+"Last-Translator: Kristof <kristof@teh.ninja>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetfinder/uk/>\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
-
-#: __init__.py:12 models.py:24 templates/fleetfinder/base.html:5
+"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
+"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"X-Generator: Weblate 5.5.3\n"
+
+#: fleetfinder/__init__.py:9 fleetfinder/models.py:24
+#: fleetfinder/templates/fleetfinder/base.html:6
+#: fleetfinder/templates/fleetfinder/base.html:10
+#: fleetfinder/templates/fleetfinder/create-fleet.html:7
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:7
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
+#: fleetfinder/templates/fleetfinder/join-fleet.html:7
 msgid "Fleet Finder"
-msgstr "Flottenfinder"
+msgstr "Пошук флоту"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
-#: apps.py:21
+#: fleetfinder/apps.py:21
 #, python-brace-format
 msgid "Fleet Finder v{__version__}"
-msgstr "Flottenfinder v{__version__}"
+msgstr "Пошук флоту v{__version__}"
 
-#: models.py:28
+#: fleetfinder/models.py:28
 msgid "Can access the Fleet Finder app"
-msgstr "Kann auf die Flottenfinder App zugreifen"
+msgstr ""
 
-#: models.py:44
+#: fleetfinder/models.py:44
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
 msgstr ""
-"Der FC ist nicht mehr in der registrierten Flotte oder die Flotte ist nicht "
-"länger verfügbar."
+"ФлітКом не знаходиться в зареєстрованому флоті або флот вже не доступний."
 
-#: models.py:46
+#: fleetfinder/models.py:46
 msgid "Registered fleet seems to be no longer available."
-msgstr "Die registrierte Flotte scheint nicht mehr verfügbar zu sein."
+msgstr "Зареєстрований флот, здається, більше не доступний."
 
-#: models.py:47
+#: fleetfinder/models.py:47
 msgid "FC is no longer the fleet boss."
-msgstr "Der FC ist nicht länger Flottenchef."
+msgstr "ФлітКом більше не бос флоту."
 
-#: models.py:48
+#: fleetfinder/models.py:48
 msgid "FC switched to another fleet."
-msgstr "Der FC wechselte zu einer anderen Flotte."
+msgstr "ФлітКом перейшов до іншого флоту."
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:30
-#: templates/fleetfinder/dashboard.html:18
-#: templates/fleetfinder/edit-fleet.html:30
+#: fleetfinder/models.py:51 fleetfinder/templates/fleetfinder/dashboard.html:18
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:10
+#, fuzzy
+#| msgid "Fleet Name"
 msgid "Fleet name"
-msgstr "Flottenname"
+msgstr "Назва флоту"
 
-#: models.py:59 templates/fleetfinder/dashboard.html:17
+#: fleetfinder/models.py:59 fleetfinder/templates/fleetfinder/dashboard.html:17
+#, fuzzy
+#| msgid "Fleet Commander"
 msgid "Fleet commander"
-msgstr "Flottenkommandant"
+msgstr "Командувач флотом"
 
-#: models.py:61
+#: fleetfinder/models.py:61
 msgid "Creation date and time"
-msgstr "Erstellungsdatum und -uhrzeit"
+msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:65
-#: templates/fleetfinder/edit-fleet.html:61
+#: fleetfinder/models.py:62
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:37
 msgid "Fleet MOTD"
-msgstr "Flotten MOTD"
+msgstr "«Шапка» флоту"
 
-#: models.py:63
+#: fleetfinder/models.py:63
+#, fuzzy
+#| msgid "Enable Free Move"
 msgid "Free move"
-msgstr "Freie Bewegung"
+msgstr "Дозволити вільне переміщення"
 
-#: models.py:69 templates/fleetfinder/create-fleet.html:42
-#: templates/fleetfinder/edit-fleet.html:42
+#: fleetfinder/models.py:69
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:32
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all who have access to this module."
 msgstr ""
-"Nur die ausgewählten Gruppen haben Zugriff zu dieser Flotte. Wenn keine "
-"Gruppen ausgewählt sind, ist die Flotte für alle die Zugriff auf dieses "
-"Modul haben verfügbar."
 
-#: models.py:73
+#: fleetfinder/models.py:73
 msgid "Group restrictions"
-msgstr "Gruppenbeschränkungen"
+msgstr "Групові обмеження"
 
-#: models.py:81
+#: fleetfinder/models.py:81
 msgid "Last ESI error"
-msgstr "Letzter ESI Fehler"
+msgstr ""
 
-#: models.py:85
+#: fleetfinder/models.py:85
 msgid "Last ESI error time"
-msgstr "Zeitpunkt des letzten ESI Fehlers"
+msgstr ""
 
-#: models.py:88
+#: fleetfinder/models.py:88
 msgid "ESI error count"
-msgstr "Anzahl der ESI Fehler"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:6
-#: templates/fleetfinder/create-fleet.html:14
-#: templates/fleetfinder/partials/header/header-navigation.html:23
+#: fleetfinder/templates/fleetfinder/create-fleet.html:6
+#: fleetfinder/templates/fleetfinder/create-fleet.html:14
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:27
+#, fuzzy
+#| msgid "Create Fleet"
 msgid "Create fleet"
-msgstr "Flotte erstellen"
-
-#: templates/fleetfinder/create-fleet.html:39
-#: templates/fleetfinder/edit-fleet.html:39
-msgid "Select groups"
-msgstr "Gruppenauswahl"
-
-#: templates/fleetfinder/create-fleet.html:75
-#: templates/fleetfinder/edit-fleet.html:71
-msgid "Enable free move"
-msgstr "Freie Bewegung aktivieren"
+msgstr "Створити флот"
 
-#: templates/fleetfinder/create-fleet.html:77
-#: templates/fleetfinder/edit-fleet.html:73
-msgid "Submit"
-msgstr "Absenden"
-
-#: templates/fleetfinder/dashboard.html:9
-#: templates/fleetfinder/partials/header/header-navigation.html:14
-msgid "Available fleets"
-msgstr "Verfügbare Flotten"
+#: fleetfinder/templates/fleetfinder/dashboard.html:9
+msgid "Fleets available to you"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:19
+#: fleetfinder/templates/fleetfinder/dashboard.html:19
+#, fuzzy
+#| msgid "Create Fleet"
 msgid "Created at"
-msgstr "Erstellt um"
+msgstr "Створити флот"
 
-#: templates/fleetfinder/dashboard.html:20
+#: fleetfinder/templates/fleetfinder/dashboard.html:20
 msgid "Join"
-msgstr "Beitreten"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:23
+#: fleetfinder/templates/fleetfinder/dashboard.html:23
 msgid "Details"
-msgstr "Details"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:24
+#: fleetfinder/templates/fleetfinder/dashboard.html:24
 msgid "Edit"
-msgstr "Bearbeiten"
+msgstr "Редагувати"
 
-#: templates/fleetfinder/edit-fleet.html:6
-#: templates/fleetfinder/edit-fleet.html:14
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:6
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:14
 msgid "Edit fleet"
-msgstr "Flotte bearbeiten"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:6
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
+#, fuzzy
+#| msgid "Fleet Finder"
 msgid "Fleet details"
-msgstr "Flottendetails"
+msgstr "Пошук флоту"
 
-#: templates/fleetfinder/fleet-details.html:15
+#: fleetfinder/templates/fleetfinder/fleet-details.html:15
 msgid "Fleet composition"
-msgstr "Flottenzusammensetzung"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:23
-#: templates/fleetfinder/fleet-details.html:47
+#: fleetfinder/templates/fleetfinder/fleet-details.html:23
+#: fleetfinder/templates/fleetfinder/fleet-details.html:47
 msgid "Ship class"
-msgstr "Schiffsklasse"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:24
+#: fleetfinder/templates/fleetfinder/fleet-details.html:24
 msgid "Count"
-msgstr "Anzahl"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:38
+#: fleetfinder/templates/fleetfinder/fleet-details.html:38
+#, fuzzy
+#| msgid "Fleet Commander"
 msgid "Fleet members"
-msgstr "Flottenmitglieder"
+msgstr "Командувач флотом"
 
-#: templates/fleetfinder/fleet-details.html:46
+#: fleetfinder/templates/fleetfinder/fleet-details.html:46
 msgid "Name"
-msgstr "Name"
+msgstr "Назва"
 
-#: templates/fleetfinder/fleet-details.html:48
+#: fleetfinder/templates/fleetfinder/fleet-details.html:48
 msgid "System"
-msgstr "System"
+msgstr "Система"
 
-#: templates/fleetfinder/join-fleet.html:6 views.py:79
+#: fleetfinder/templates/fleetfinder/join-fleet.html:6 fleetfinder/views.py:91
 msgid "Join fleet"
-msgstr "Flotte beitreten"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:14
+#: fleetfinder/templates/fleetfinder/join-fleet.html:14
 msgid "Fleet invitation"
-msgstr "Flotteneinladung"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:24
+#: fleetfinder/templates/fleetfinder/join-fleet.html:25
 msgid "Select the characters to invite"
-msgstr "Wähle einzuladende Charaktere"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:33
+#: fleetfinder/templates/fleetfinder/join-fleet.html:35
 msgid "Send fleet invites"
-msgstr "Flotteneinladungen senden"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:15
+msgid "Select groups"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:46
+#, fuzzy
+#| msgid "Enable Free Move"
+msgid "Enable free move"
+msgstr "Дозволити вільне переміщення"
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:49
+msgid "Submit"
+msgstr "Відправити"
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:5
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
-"Du möchtest helfen diese App in Deine Sprache zu übersetzen oder die "
-"bestehende Übersetzung verbessern?"
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:8
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "Tritt unserm Team von Übersetzern bei!"
+msgstr ""
 
-#: templates/fleetfinder/partials/header/header-navigation.html:7
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:6
+#, fuzzy
+#| msgid "Available Fleets"
+msgid "Available fleets"
+msgstr "Доступні флоти"
+
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:17
 msgid "Toggle navigation"
-msgstr "Navigation umschalten"
+msgstr ""
 
-#: views.py:92
+#: fleetfinder/views.py:104
 msgid "View fleet details"
-msgstr "Flottendetails anzeigen"
+msgstr ""
 
-#: views.py:99
+#: fleetfinder/views.py:113
 msgid "Edit fleet advert"
-msgstr "Flottenanzeige bearbeiten"
+msgstr ""
 
-#: views.py:243
+#: fleetfinder/views.py:279
 #, python-brace-format
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
-"<h4>Fehler!</h4><p>ESI hat den folgenden Fehler zurückgegeben: "
-"{esi_error_message}</p>"
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/es/LC_MESSAGES/django.mo` & `aa_fleetfinder-2.0.1/fleetfinder/locale/es/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetfinder/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
 "<h4>Error!</h4><p>El ESI devolvió el siguiente error: {esi_error_message}</p>"
 
 msgid "Creation date and time"
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/es/LC_MESSAGES/django.po` & `aa_fleetfinder-2.0.1/fleetfinder/locale/django.pot`

 * *Files 26% similar despite different names*

```diff
@@ -1,252 +1,220 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-24 16:26+0200\n"
-"PO-Revision-Date: 2023-09-28 10:42+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetfinder/es/>\n"
-"Language: es\n"
+"POT-Creation-Date: 2024-03-20 17:23+0100\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
 
-#: __init__.py:12 models.py:24 templates/fleetfinder/base.html:5
+#: fleetfinder/__init__.py:9 fleetfinder/models.py:24
+#: fleetfinder/templates/fleetfinder/base.html:6
+#: fleetfinder/templates/fleetfinder/base.html:10
+#: fleetfinder/templates/fleetfinder/create-fleet.html:7
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:7
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
+#: fleetfinder/templates/fleetfinder/join-fleet.html:7
 msgid "Fleet Finder"
-msgstr "Buscador de Flotas"
+msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
-#: apps.py:21
+#: fleetfinder/apps.py:21
 #, python-brace-format
 msgid "Fleet Finder v{__version__}"
-msgstr "Buscador de Flotas v{__version__}"
+msgstr ""
 
-#: models.py:28
+#: fleetfinder/models.py:28
 msgid "Can access the Fleet Finder app"
 msgstr ""
 
-#: models.py:44
+#: fleetfinder/models.py:44
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
 msgstr ""
-"El FC ya no está en la flota registrada o la flota ya no está disponible."
 
-#: models.py:46
+#: fleetfinder/models.py:46
 msgid "Registered fleet seems to be no longer available."
-msgstr "Parece que la flota registrada ya no está disponible."
+msgstr ""
 
-#: models.py:47
+#: fleetfinder/models.py:47
 msgid "FC is no longer the fleet boss."
-msgstr "El FC ya no es el jefe de flota."
+msgstr ""
 
-#: models.py:48
+#: fleetfinder/models.py:48
 msgid "FC switched to another fleet."
-msgstr "El FC se cambió a otra flota."
+msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:30
-#: templates/fleetfinder/dashboard.html:18
-#: templates/fleetfinder/edit-fleet.html:30
-#, fuzzy
-#| msgid "Fleet Name"
+#: fleetfinder/models.py:51 fleetfinder/templates/fleetfinder/dashboard.html:18
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:10
 msgid "Fleet name"
-msgstr "Nombre de la Flota"
+msgstr ""
 
-#: models.py:59 templates/fleetfinder/dashboard.html:17
-#, fuzzy
-#| msgid "Fleet Commander"
+#: fleetfinder/models.py:59 fleetfinder/templates/fleetfinder/dashboard.html:17
 msgid "Fleet commander"
-msgstr "Comandante de Flota"
+msgstr ""
 
-#: models.py:61
+#: fleetfinder/models.py:61
 msgid "Creation date and time"
-msgstr "Crear la fecha y hora"
+msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:65
-#: templates/fleetfinder/edit-fleet.html:61
+#: fleetfinder/models.py:62
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:37
 msgid "Fleet MOTD"
-msgstr "MOTD de la Flota"
+msgstr ""
 
-#: models.py:63
+#: fleetfinder/models.py:63
 msgid "Free move"
-msgstr "Movimiento libre"
+msgstr ""
 
-#: models.py:69 templates/fleetfinder/create-fleet.html:42
-#: templates/fleetfinder/edit-fleet.html:42
+#: fleetfinder/models.py:69
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:32
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all who have access to this module."
 msgstr ""
-"Solo los grupos seleccionados tendrán acceso a la flota. Si no se selecciona "
-"ningún grupo, la flota estará disponible para todos los que tengan acceso a "
-"este módulo."
 
-#: models.py:73
+#: fleetfinder/models.py:73
 msgid "Group restrictions"
-msgstr "Restricciones de grupo"
+msgstr ""
 
-#: models.py:81
+#: fleetfinder/models.py:81
 msgid "Last ESI error"
-msgstr "Último error del ESI"
+msgstr ""
 
-#: models.py:85
+#: fleetfinder/models.py:85
 msgid "Last ESI error time"
-msgstr "Hora del último error del ESI"
+msgstr ""
 
-#: models.py:88
+#: fleetfinder/models.py:88
 msgid "ESI error count"
-msgstr "Recuento de errores del ESI"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:6
-#: templates/fleetfinder/create-fleet.html:14
-#: templates/fleetfinder/partials/header/header-navigation.html:23
-#, fuzzy
-#| msgid "Create Fleet"
+#: fleetfinder/templates/fleetfinder/create-fleet.html:6
+#: fleetfinder/templates/fleetfinder/create-fleet.html:14
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:27
 msgid "Create fleet"
-msgstr "Crear Flota"
-
-#: templates/fleetfinder/create-fleet.html:39
-#: templates/fleetfinder/edit-fleet.html:39
-#, fuzzy
-#| msgid "Select Groups"
-msgid "Select groups"
-msgstr "Grupos Seleccionados"
-
-#: templates/fleetfinder/create-fleet.html:75
-#: templates/fleetfinder/edit-fleet.html:71
-#, fuzzy
-#| msgid "Enable Free Move"
-msgid "Enable free move"
-msgstr "Habilitar Movimiento Libre"
-
-#: templates/fleetfinder/create-fleet.html:77
-#: templates/fleetfinder/edit-fleet.html:73
-msgid "Submit"
-msgstr "Enviar"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:9
-#: templates/fleetfinder/partials/header/header-navigation.html:14
-#, fuzzy
-#| msgid "Available Fleets"
-msgid "Available fleets"
-msgstr "Flotas Disponibles"
+#: fleetfinder/templates/fleetfinder/dashboard.html:9
+msgid "Fleets available to you"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:19
-#, fuzzy
-#| msgid "Created At"
+#: fleetfinder/templates/fleetfinder/dashboard.html:19
 msgid "Created at"
-msgstr "Creado En"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:20
+#: fleetfinder/templates/fleetfinder/dashboard.html:20
 msgid "Join"
-msgstr "Unirse"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:23
+#: fleetfinder/templates/fleetfinder/dashboard.html:23
 msgid "Details"
-msgstr "Detalles"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:24
+#: fleetfinder/templates/fleetfinder/dashboard.html:24
 msgid "Edit"
-msgstr "Editar"
+msgstr ""
 
-#: templates/fleetfinder/edit-fleet.html:6
-#: templates/fleetfinder/edit-fleet.html:14
-#, fuzzy
-#| msgid "Edit Fleet"
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:6
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:14
 msgid "Edit fleet"
-msgstr "Editar la Flota"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:6
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
 msgid "Fleet details"
-msgstr "Detalles de la Flota"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:15
+#: fleetfinder/templates/fleetfinder/fleet-details.html:15
 msgid "Fleet composition"
-msgstr "Composición de Flota"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:23
-#: templates/fleetfinder/fleet-details.html:47
-#, fuzzy
-#| msgid "Ship Name"
+#: fleetfinder/templates/fleetfinder/fleet-details.html:23
+#: fleetfinder/templates/fleetfinder/fleet-details.html:47
 msgid "Ship class"
-msgstr "Nombre de la Nave"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:24
+#: fleetfinder/templates/fleetfinder/fleet-details.html:24
 msgid "Count"
 msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:38
-#, fuzzy
-#| msgid "Fleet Members"
+#: fleetfinder/templates/fleetfinder/fleet-details.html:38
 msgid "Fleet members"
-msgstr "Miembros de la Flota"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:46
+#: fleetfinder/templates/fleetfinder/fleet-details.html:46
 msgid "Name"
-msgstr "Nombre"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:48
+#: fleetfinder/templates/fleetfinder/fleet-details.html:48
 msgid "System"
-msgstr "Sistema"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:6 views.py:79
-#, fuzzy
-#| msgid "Join Fleet"
+#: fleetfinder/templates/fleetfinder/join-fleet.html:6 fleetfinder/views.py:91
 msgid "Join fleet"
-msgstr "Unirse a la Flota"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:14
-#, fuzzy
-#| msgid "Fleet Invitation"
+#: fleetfinder/templates/fleetfinder/join-fleet.html:14
 msgid "Fleet invitation"
-msgstr "Invitación a la Flota"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:24
+#: fleetfinder/templates/fleetfinder/join-fleet.html:25
 msgid "Select the characters to invite"
-msgstr "Selecciona los personajes a invitar"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:33
+#: fleetfinder/templates/fleetfinder/join-fleet.html:35
 msgid "Send fleet invites"
-msgstr "Enviar invitaciones de Flota"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:15
+msgid "Select groups"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:46
+msgid "Enable free move"
+msgstr ""
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:5
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:49
+msgid "Submit"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
-"¿Quieres ayudar a traducir esta aplicación a tu idioma o mejorar la "
-"traducción existente?"
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:8
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "¡Únete a nuestro equipo de traductores!"
+msgstr ""
 
-#: templates/fleetfinder/partials/header/header-navigation.html:7
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:6
+msgid "Available fleets"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:17
 msgid "Toggle navigation"
-msgstr "Alternar la navegación"
+msgstr ""
 
-#: views.py:92
-#, fuzzy
-#| msgid "View Fleet Details"
+#: fleetfinder/views.py:104
 msgid "View fleet details"
-msgstr "Ver detalles de la Flota"
+msgstr ""
 
-#: views.py:99
-#, fuzzy
-#| msgid "Edit Fleet Advert"
+#: fleetfinder/views.py:113
 msgid "Edit fleet advert"
-msgstr "Editar Anuncio de la Flota"
+msgstr ""
 
-#: views.py:243
+#: fleetfinder/views.py:279
 #, python-brace-format
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
-"<h4>Error!</h4><p>El ESI devolvió el siguiente error: {esi_error_message}</p>"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/it_IT/LC_MESSAGES/django.po` & `aa_fleetfinder-2.0.1/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,217 +1,224 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-#
+# Dehao Wu <wudehao2000@163.com>, 2024.
+# Faer Yili <yilifaer@gmail.com>, 2024.
+# SAM_FPS <sam_fps@163.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-24 16:26+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
-"Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-fleetfinder/it/>\n"
-"Language: it_IT\n"
+"POT-Creation-Date: 2024-03-15 20:22+0100\n"
+"PO-Revision-Date: 2024-05-16 13:20+0000\n"
+"Last-Translator: SAM_FPS <sam_fps@163.com>\n"
+"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetfinder/zh_Hans/>\n"
+"Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 5.5.5\n"
 
-#: __init__.py:12 models.py:24 templates/fleetfinder/base.html:5
+#: fleetfinder/__init__.py:9 fleetfinder/models.py:24
+#: fleetfinder/templates/fleetfinder/base.html:6
+#: fleetfinder/templates/fleetfinder/base.html:10
+#: fleetfinder/templates/fleetfinder/create-fleet.html:7
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:7
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
+#: fleetfinder/templates/fleetfinder/join-fleet.html:7
 msgid "Fleet Finder"
-msgstr ""
+msgstr "舰队搜寻器"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
-#: apps.py:21
+#: fleetfinder/apps.py:21
 #, python-brace-format
 msgid "Fleet Finder v{__version__}"
-msgstr ""
+msgstr "舰队搜寻器v{__version__}"
 
-#: models.py:28
+#: fleetfinder/models.py:28
 msgid "Can access the Fleet Finder app"
-msgstr ""
+msgstr "可以访问舰队搜寻器应用程序"
 
-#: models.py:44
+#: fleetfinder/models.py:44
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
-msgstr ""
+msgstr "舰队指挥官不在已注册的舰队中或舰队不再可用。"
 
-#: models.py:46
+#: fleetfinder/models.py:46
 msgid "Registered fleet seems to be no longer available."
-msgstr ""
+msgstr "已登记的舰队似乎不再可用。"
 
-#: models.py:47
+#: fleetfinder/models.py:47
 msgid "FC is no longer the fleet boss."
-msgstr ""
+msgstr "舰队指挥官不再是舰队统帅。"
 
-#: models.py:48
+#: fleetfinder/models.py:48
 msgid "FC switched to another fleet."
-msgstr ""
+msgstr "舰队指挥官转到了另一个舰队。"
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:30
-#: templates/fleetfinder/dashboard.html:18
-#: templates/fleetfinder/edit-fleet.html:30
+#: fleetfinder/models.py:51 fleetfinder/templates/fleetfinder/dashboard.html:18
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:10
 msgid "Fleet name"
-msgstr ""
+msgstr "舰队名字"
 
-#: models.py:59 templates/fleetfinder/dashboard.html:17
+#: fleetfinder/models.py:59 fleetfinder/templates/fleetfinder/dashboard.html:17
 msgid "Fleet commander"
-msgstr ""
+msgstr "舰队指挥官"
 
-#: models.py:61
+#: fleetfinder/models.py:61
 msgid "Creation date and time"
-msgstr ""
+msgstr "创建日期和时间"
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:65
-#: templates/fleetfinder/edit-fleet.html:61
+#: fleetfinder/models.py:62
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:37
 msgid "Fleet MOTD"
-msgstr ""
+msgstr "舰队置顶信息"
 
-#: models.py:63
+#: fleetfinder/models.py:63
 msgid "Free move"
-msgstr ""
+msgstr "自由移动"
 
-#: models.py:69 templates/fleetfinder/create-fleet.html:42
-#: templates/fleetfinder/edit-fleet.html:42
+#: fleetfinder/models.py:69
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:32
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all who have access to this module."
-msgstr ""
+msgstr "只有选定的群组才能进入舰队。如果没有选择群组，舰队将对所有访问此模块的人可用"
+"。"
 
-#: models.py:73
+#: fleetfinder/models.py:73
 msgid "Group restrictions"
-msgstr ""
+msgstr "组别限制"
 
-#: models.py:81
+#: fleetfinder/models.py:81
 msgid "Last ESI error"
-msgstr ""
+msgstr "上一次ESI错误"
 
-#: models.py:85
+#: fleetfinder/models.py:85
 msgid "Last ESI error time"
-msgstr ""
+msgstr "最后一次ESI错误时间"
 
-#: models.py:88
+#: fleetfinder/models.py:88
 msgid "ESI error count"
-msgstr ""
+msgstr "ESI错误计数"
 
-#: templates/fleetfinder/create-fleet.html:6
-#: templates/fleetfinder/create-fleet.html:14
-#: templates/fleetfinder/partials/header/header-navigation.html:23
+#: fleetfinder/templates/fleetfinder/create-fleet.html:6
+#: fleetfinder/templates/fleetfinder/create-fleet.html:14
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:27
 msgid "Create fleet"
-msgstr ""
-
-#: templates/fleetfinder/create-fleet.html:39
-#: templates/fleetfinder/edit-fleet.html:39
-msgid "Select groups"
-msgstr ""
+msgstr "创建舰队"
 
-#: templates/fleetfinder/create-fleet.html:75
-#: templates/fleetfinder/edit-fleet.html:71
-msgid "Enable free move"
-msgstr ""
+#: fleetfinder/templates/fleetfinder/dashboard.html:9
+msgid "Fleets available to you"
+msgstr "您有权访问的舰队"
 
-#: templates/fleetfinder/create-fleet.html:77
-#: templates/fleetfinder/edit-fleet.html:73
-msgid "Submit"
-msgstr ""
-
-#: templates/fleetfinder/dashboard.html:9
-#: templates/fleetfinder/partials/header/header-navigation.html:14
-msgid "Available fleets"
-msgstr ""
-
-#: templates/fleetfinder/dashboard.html:19
+#: fleetfinder/templates/fleetfinder/dashboard.html:19
 msgid "Created at"
-msgstr ""
+msgstr "创建于"
 
-#: templates/fleetfinder/dashboard.html:20
+#: fleetfinder/templates/fleetfinder/dashboard.html:20
 msgid "Join"
-msgstr ""
+msgstr "加入"
 
-#: templates/fleetfinder/dashboard.html:23
+#: fleetfinder/templates/fleetfinder/dashboard.html:23
 msgid "Details"
-msgstr ""
+msgstr "细节"
 
-#: templates/fleetfinder/dashboard.html:24
+#: fleetfinder/templates/fleetfinder/dashboard.html:24
 msgid "Edit"
-msgstr ""
+msgstr "编辑"
 
-#: templates/fleetfinder/edit-fleet.html:6
-#: templates/fleetfinder/edit-fleet.html:14
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:6
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:14
 msgid "Edit fleet"
-msgstr ""
+msgstr "编辑舰队"
 
-#: templates/fleetfinder/fleet-details.html:6
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
 msgid "Fleet details"
-msgstr ""
+msgstr "舰队细节"
 
-#: templates/fleetfinder/fleet-details.html:15
+#: fleetfinder/templates/fleetfinder/fleet-details.html:15
 msgid "Fleet composition"
-msgstr ""
+msgstr "舰队组成"
 
-#: templates/fleetfinder/fleet-details.html:23
-#: templates/fleetfinder/fleet-details.html:47
+#: fleetfinder/templates/fleetfinder/fleet-details.html:23
+#: fleetfinder/templates/fleetfinder/fleet-details.html:47
 msgid "Ship class"
-msgstr ""
+msgstr "舰船等级"
 
-#: templates/fleetfinder/fleet-details.html:24
+#: fleetfinder/templates/fleetfinder/fleet-details.html:24
 msgid "Count"
-msgstr ""
+msgstr "计数"
 
-#: templates/fleetfinder/fleet-details.html:38
+#: fleetfinder/templates/fleetfinder/fleet-details.html:38
 msgid "Fleet members"
-msgstr ""
+msgstr "舰队成员"
 
-#: templates/fleetfinder/fleet-details.html:46
+#: fleetfinder/templates/fleetfinder/fleet-details.html:46
 msgid "Name"
-msgstr ""
+msgstr "名字"
 
-#: templates/fleetfinder/fleet-details.html:48
+#: fleetfinder/templates/fleetfinder/fleet-details.html:48
 msgid "System"
-msgstr ""
+msgstr "星系"
 
-#: templates/fleetfinder/join-fleet.html:6 views.py:79
+#: fleetfinder/templates/fleetfinder/join-fleet.html:6 fleetfinder/views.py:91
 msgid "Join fleet"
-msgstr ""
+msgstr "加入舰队"
 
-#: templates/fleetfinder/join-fleet.html:14
+#: fleetfinder/templates/fleetfinder/join-fleet.html:14
 msgid "Fleet invitation"
-msgstr ""
+msgstr "舰队邀请"
 
-#: templates/fleetfinder/join-fleet.html:24
+#: fleetfinder/templates/fleetfinder/join-fleet.html:25
 msgid "Select the characters to invite"
-msgstr ""
+msgstr "选择要邀请的角色"
 
-#: templates/fleetfinder/join-fleet.html:33
+#: fleetfinder/templates/fleetfinder/join-fleet.html:35
 msgid "Send fleet invites"
-msgstr ""
+msgstr "发送舰队邀请"
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:5
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:15
+msgid "Select groups"
+msgstr "选择群组"
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:46
+msgid "Enable free move"
+msgstr "允许自由行动"
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:49
+msgid "Submit"
+msgstr "提交"
+
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr ""
+msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:8
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr ""
+msgstr "加入我们的翻译团队吧！"
+
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:6
+msgid "Available fleets"
+msgstr "可用的舰队"
 
-#: templates/fleetfinder/partials/header/header-navigation.html:7
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:17
 msgid "Toggle navigation"
-msgstr ""
+msgstr "切换导航"
 
-#: views.py:92
+#: fleetfinder/views.py:104
 msgid "View fleet details"
-msgstr ""
+msgstr "查看船队详情"
 
-#: views.py:99
+#: fleetfinder/views.py:113
 msgid "Edit fleet advert"
-msgstr ""
+msgstr "编辑舰队宣传信息"
 
-#: views.py:243
+#: fleetfinder/views.py:279
 #, python-brace-format
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
-msgstr ""
+msgstr "<h4>错误!</h4><p>ESI返回如下错误:{esi_error_message}</p>"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_fleetfinder-2.0.1/fleetfinder/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 16% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,26 +7,32 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-fleetfinder/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr "<h4>오류!</h4><p>ESI가 다음 오류를 출력함:{esi_error_message}</p>"
 
 msgid "Can access the Fleet Finder app"
 msgstr "Fleet Finder App을 이용할 수 있음"
 
 msgid "Count"
 msgstr "갯수"
 
+msgid "Create fleet"
+msgstr "함대 생성"
+
+msgid "Created at"
+msgstr "생성된 시각"
+
 msgid "Creation date and time"
 msgstr "생성 날짜 및 시간"
 
 msgid "Details"
 msgstr "세부 내용"
 
 msgid ""
@@ -64,25 +70,31 @@
 
 msgid "Fleet composition"
 msgstr "함대 구성"
 
 msgid "Fleet details"
 msgstr "함대 세부 사항"
 
+msgid "Fleet name"
+msgstr "함대 이름"
+
+msgid "Fleets available to you"
+msgstr "참여 가능한 플릿"
+
 msgid "Free move"
 msgstr "자유 이동"
 
 msgid "Group restrictions"
 msgstr "그룹 제한"
 
 msgid "Join"
 msgstr "참가"
 
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
 msgid "Last ESI error"
 msgstr "최근 ESI 오류"
 
 msgid "Last ESI error time"
 msgstr "최근 ESI 오류 시각"
 
@@ -108,11 +120,11 @@
 msgid "Ship class"
 msgstr "함급"
 
 msgid "Submit"
 msgstr "전송"
 
 msgid "System"
-msgstr "성계"
+msgstr "시스템"
 
 msgid "Toggle navigation"
 msgstr "토글 메뉴"
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/ko_KR/LC_MESSAGES/django.po` & `aa_fleetfinder-2.0.1/fleetfinder/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 27% similar despite different names*

```diff
@@ -1,243 +1,222 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Author50CO <tkddlschry@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-24 16:26+0200\n"
-"PO-Revision-Date: 2023-12-29 10:04+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetfinder/ko/>\n"
-"Language: ko_KR\n"
+"POT-Creation-Date: 2024-03-15 20:22+0100\n"
+"PO-Revision-Date: 2024-05-10 14:03+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetfinder/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: __init__.py:12 models.py:24 templates/fleetfinder/base.html:5
+#: fleetfinder/__init__.py:9 fleetfinder/models.py:24
+#: fleetfinder/templates/fleetfinder/base.html:6
+#: fleetfinder/templates/fleetfinder/base.html:10
+#: fleetfinder/templates/fleetfinder/create-fleet.html:7
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:7
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
+#: fleetfinder/templates/fleetfinder/join-fleet.html:7
 msgid "Fleet Finder"
-msgstr "함대 찾기"
+msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
-#: apps.py:21
+#: fleetfinder/apps.py:21
 #, python-brace-format
 msgid "Fleet Finder v{__version__}"
-msgstr "함대 찾기 v{__version__}"
+msgstr ""
 
-#: models.py:28
+#: fleetfinder/models.py:28
 msgid "Can access the Fleet Finder app"
-msgstr "Fleet Finder App을 이용할 수 있음"
+msgstr ""
 
-#: models.py:44
+#: fleetfinder/models.py:44
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
-msgstr "함대 지휘관이 지정된 함대에 없거나 함대 참가가 더 이상 불가능합니다."
+msgstr ""
 
-#: models.py:46
+#: fleetfinder/models.py:46
 msgid "Registered fleet seems to be no longer available."
-msgstr "지정된 함대가 참가가 더 이상 불가능합니다."
+msgstr ""
 
-#: models.py:47
+#: fleetfinder/models.py:47
 msgid "FC is no longer the fleet boss."
-msgstr "함대 지휘관이 더 이상 함대 소유자가 아닙니다."
+msgstr ""
 
-#: models.py:48
+#: fleetfinder/models.py:48
 msgid "FC switched to another fleet."
-msgstr "함대 지휘관이 다른 함대로 바꿨습니다."
+msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:30
-#: templates/fleetfinder/dashboard.html:18
-#: templates/fleetfinder/edit-fleet.html:30
-#, fuzzy
-#| msgid "Fleet Name"
+#: fleetfinder/models.py:51 fleetfinder/templates/fleetfinder/dashboard.html:18
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:10
 msgid "Fleet name"
-msgstr "함대 이름"
+msgstr ""
 
-#: models.py:59 templates/fleetfinder/dashboard.html:17
+#: fleetfinder/models.py:59 fleetfinder/templates/fleetfinder/dashboard.html:17
 msgid "Fleet commander"
-msgstr "함대 지휘관"
+msgstr ""
 
-#: models.py:61
+#: fleetfinder/models.py:61
 msgid "Creation date and time"
-msgstr "생성 날짜 및 시간"
+msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:65
-#: templates/fleetfinder/edit-fleet.html:61
+#: fleetfinder/models.py:62
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:37
 msgid "Fleet MOTD"
-msgstr "함대 공지 사항"
+msgstr ""
 
-#: models.py:63
+#: fleetfinder/models.py:63
 msgid "Free move"
-msgstr "자유 이동"
+msgstr ""
 
-#: models.py:69 templates/fleetfinder/create-fleet.html:42
-#: templates/fleetfinder/edit-fleet.html:42
+#: fleetfinder/models.py:69
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:32
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all who have access to this module."
 msgstr ""
-"선택한 그룹만이 함대에 참가할 수 있습니다. 선택된 그룹이 없을 경우 해당 모듈"
-"을 사용 가능한 모든 유저가 참가 가능합니다."
 
-#: models.py:73
+#: fleetfinder/models.py:73
 msgid "Group restrictions"
-msgstr "그룹 제한"
+msgstr ""
 
-#: models.py:81
+#: fleetfinder/models.py:81
 msgid "Last ESI error"
-msgstr "최근 ESI 오류"
+msgstr ""
 
-#: models.py:85
+#: fleetfinder/models.py:85
 msgid "Last ESI error time"
-msgstr "최근 ESI 오류 시각"
+msgstr ""
 
-#: models.py:88
+#: fleetfinder/models.py:88
 msgid "ESI error count"
-msgstr "ESI 오류 갯수"
+msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:6
-#: templates/fleetfinder/create-fleet.html:14
-#: templates/fleetfinder/partials/header/header-navigation.html:23
-#, fuzzy
-#| msgid "Create Fleet"
+#: fleetfinder/templates/fleetfinder/create-fleet.html:6
+#: fleetfinder/templates/fleetfinder/create-fleet.html:14
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:27
 msgid "Create fleet"
-msgstr "함대 생성"
-
-#: templates/fleetfinder/create-fleet.html:39
-#: templates/fleetfinder/edit-fleet.html:39
-#, fuzzy
-#| msgid "Select Groups"
-msgid "Select groups"
-msgstr "그룹 선택"
-
-#: templates/fleetfinder/create-fleet.html:75
-#: templates/fleetfinder/edit-fleet.html:71
-#, fuzzy
-#| msgid "Enable Free Move"
-msgid "Enable free move"
-msgstr "자유 이동 설정"
-
-#: templates/fleetfinder/create-fleet.html:77
-#: templates/fleetfinder/edit-fleet.html:73
-msgid "Submit"
-msgstr "전송"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:9
-#: templates/fleetfinder/partials/header/header-navigation.html:14
-#, fuzzy
-#| msgid "Available Fleets"
-msgid "Available fleets"
-msgstr "참가 가능한 함대"
+#: fleetfinder/templates/fleetfinder/dashboard.html:9
+msgid "Fleets available to you"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:19
-#, fuzzy
-#| msgid "Created At"
+#: fleetfinder/templates/fleetfinder/dashboard.html:19
 msgid "Created at"
-msgstr "생성된 시각"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:20
+#: fleetfinder/templates/fleetfinder/dashboard.html:20
 msgid "Join"
-msgstr "참가"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:23
+#: fleetfinder/templates/fleetfinder/dashboard.html:23
 msgid "Details"
-msgstr "세부 내용"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:24
+#: fleetfinder/templates/fleetfinder/dashboard.html:24
 msgid "Edit"
-msgstr "수정"
+msgstr ""
 
-#: templates/fleetfinder/edit-fleet.html:6
-#: templates/fleetfinder/edit-fleet.html:14
-#, fuzzy
-#| msgid "Edit Fleet"
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:6
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:14
 msgid "Edit fleet"
-msgstr "함대 수정"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:6
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
 msgid "Fleet details"
-msgstr "함대 세부 사항"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:15
+#: fleetfinder/templates/fleetfinder/fleet-details.html:15
 msgid "Fleet composition"
-msgstr "함대 구성"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:23
-#: templates/fleetfinder/fleet-details.html:47
+#: fleetfinder/templates/fleetfinder/fleet-details.html:23
+#: fleetfinder/templates/fleetfinder/fleet-details.html:47
 msgid "Ship class"
-msgstr "함급"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:24
+#: fleetfinder/templates/fleetfinder/fleet-details.html:24
 msgid "Count"
-msgstr "갯수"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:38
-#, fuzzy
-#| msgid "Fleet Members"
+#: fleetfinder/templates/fleetfinder/fleet-details.html:38
 msgid "Fleet members"
-msgstr "함대 멤버"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:46
+#: fleetfinder/templates/fleetfinder/fleet-details.html:46
 msgid "Name"
-msgstr "이름"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:48
+#: fleetfinder/templates/fleetfinder/fleet-details.html:48
 msgid "System"
-msgstr "성계"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:6 views.py:79
-#, fuzzy
-#| msgid "Join Fleet"
+#: fleetfinder/templates/fleetfinder/join-fleet.html:6 fleetfinder/views.py:91
 msgid "Join fleet"
-msgstr "함대 참가"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:14
-#, fuzzy
-#| msgid "Fleet Invitation"
+#: fleetfinder/templates/fleetfinder/join-fleet.html:14
 msgid "Fleet invitation"
-msgstr "함대 초대"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:24
+#: fleetfinder/templates/fleetfinder/join-fleet.html:25
 msgid "Select the characters to invite"
-msgstr "초대할 캐릭터를 선택하세요"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:33
+#: fleetfinder/templates/fleetfinder/join-fleet.html:35
 msgid "Send fleet invites"
-msgstr "함대 초대 보내기"
+msgstr ""
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:5
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:15
+msgid "Select groups"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:46
+msgid "Enable free move"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:49
+msgid "Submit"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
+msgstr ""
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:8
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr ""
 
-#: templates/fleetfinder/partials/header/header-navigation.html:7
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:6
+msgid "Available fleets"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:17
 msgid "Toggle navigation"
-msgstr "토글 메뉴"
+msgstr ""
 
-#: views.py:92
-#, fuzzy
-#| msgid "View Fleet Details"
+#: fleetfinder/views.py:104
 msgid "View fleet details"
-msgstr "함대 세부 내용 보기"
+msgstr ""
 
-#: views.py:99
-#, fuzzy
-#| msgid "Edit Fleet Advert"
+#: fleetfinder/views.py:113
 msgid "Edit fleet advert"
-msgstr "함대 광고 수정"
+msgstr ""
 
-#: views.py:243
+#: fleetfinder/views.py:279
 #, python-brace-format
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
-msgstr "<h4>오류!</h4><p>ESI가 다음 오류를 출력함:{esi_error_message}</p>"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/ru/LC_MESSAGES/django.mo` & `aa_fleetfinder-2.0.1/fleetfinder/locale/ru/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-fleetfinder/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>ESI вернул следующую ошибку: {esi_error_message}</p>"
 
 msgid "Available fleets"
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/uk/LC_MESSAGES/django.mo` & `aa_fleetfinder-2.0.1/fleetfinder/locale/uk/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-fleetfinder/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Edit"
 msgstr "Редагувати"
 
 msgid "FC is no longer the fleet boss."
 msgstr "ФлітКом більше не бос флоту."
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/uk/LC_MESSAGES/django.po` & `aa_fleetfinder-2.0.1/fleetfinder/locale/ja/LC_MESSAGES/django.po`

 * *Files 26% similar despite different names*

```diff
@@ -1,238 +1,222 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "Andrii M." <elfleg0las88@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
-# Kristof <kristof@teh.ninja>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-24 16:26+0200\n"
-"PO-Revision-Date: 2023-10-02 09:46+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetfinder/uk/>\n"
-"Language: uk\n"
+"POT-Creation-Date: 2024-03-15 20:22+0100\n"
+"PO-Revision-Date: 2024-05-10 14:03+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-fleetfinder/ja/>\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
-"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=1; plural=0;\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: __init__.py:12 models.py:24 templates/fleetfinder/base.html:5
+#: fleetfinder/__init__.py:9 fleetfinder/models.py:24
+#: fleetfinder/templates/fleetfinder/base.html:6
+#: fleetfinder/templates/fleetfinder/base.html:10
+#: fleetfinder/templates/fleetfinder/create-fleet.html:7
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:7
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
+#: fleetfinder/templates/fleetfinder/join-fleet.html:7
 msgid "Fleet Finder"
-msgstr "Пошук флоту"
+msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
-#: apps.py:21
+#: fleetfinder/apps.py:21
 #, python-brace-format
 msgid "Fleet Finder v{__version__}"
-msgstr "Пошук флоту v{__version__}"
+msgstr ""
 
-#: models.py:28
+#: fleetfinder/models.py:28
 msgid "Can access the Fleet Finder app"
 msgstr ""
 
-#: models.py:44
+#: fleetfinder/models.py:44
 msgid ""
 "FC is not in the registered fleet anymore or fleet is no longer available."
 msgstr ""
-"ФлітКом не знаходиться в зареєстрованому флоті або флот вже не доступний."
 
-#: models.py:46
+#: fleetfinder/models.py:46
 msgid "Registered fleet seems to be no longer available."
-msgstr "Зареєстрований флот, здається, більше не доступний."
+msgstr ""
 
-#: models.py:47
+#: fleetfinder/models.py:47
 msgid "FC is no longer the fleet boss."
-msgstr "ФлітКом більше не бос флоту."
+msgstr ""
 
-#: models.py:48
+#: fleetfinder/models.py:48
 msgid "FC switched to another fleet."
-msgstr "ФлітКом перейшов до іншого флоту."
+msgstr ""
 
-#: models.py:51 templates/fleetfinder/create-fleet.html:30
-#: templates/fleetfinder/dashboard.html:18
-#: templates/fleetfinder/edit-fleet.html:30
-#, fuzzy
-#| msgid "Fleet Name"
+#: fleetfinder/models.py:51 fleetfinder/templates/fleetfinder/dashboard.html:18
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:10
 msgid "Fleet name"
-msgstr "Назва флоту"
+msgstr ""
 
-#: models.py:59 templates/fleetfinder/dashboard.html:17
-#, fuzzy
-#| msgid "Fleet Commander"
+#: fleetfinder/models.py:59 fleetfinder/templates/fleetfinder/dashboard.html:17
 msgid "Fleet commander"
-msgstr "Командувач флотом"
+msgstr ""
 
-#: models.py:61
+#: fleetfinder/models.py:61
 msgid "Creation date and time"
 msgstr ""
 
-#: models.py:62 templates/fleetfinder/create-fleet.html:65
-#: templates/fleetfinder/edit-fleet.html:61
+#: fleetfinder/models.py:62
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:37
 msgid "Fleet MOTD"
-msgstr "«Шапка» флоту"
+msgstr ""
 
-#: models.py:63
-#, fuzzy
-#| msgid "Enable Free Move"
+#: fleetfinder/models.py:63
 msgid "Free move"
-msgstr "Дозволити вільне переміщення"
+msgstr ""
 
-#: models.py:69 templates/fleetfinder/create-fleet.html:42
-#: templates/fleetfinder/edit-fleet.html:42
+#: fleetfinder/models.py:69
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:32
 msgid ""
 "Only selected groups will have access to the fleet. If no groups are "
 "selected the fleet will be available to all who have access to this module."
 msgstr ""
 
-#: models.py:73
+#: fleetfinder/models.py:73
 msgid "Group restrictions"
-msgstr "Групові обмеження"
+msgstr ""
 
-#: models.py:81
+#: fleetfinder/models.py:81
 msgid "Last ESI error"
 msgstr ""
 
-#: models.py:85
+#: fleetfinder/models.py:85
 msgid "Last ESI error time"
 msgstr ""
 
-#: models.py:88
+#: fleetfinder/models.py:88
 msgid "ESI error count"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:6
-#: templates/fleetfinder/create-fleet.html:14
-#: templates/fleetfinder/partials/header/header-navigation.html:23
-#, fuzzy
-#| msgid "Create Fleet"
+#: fleetfinder/templates/fleetfinder/create-fleet.html:6
+#: fleetfinder/templates/fleetfinder/create-fleet.html:14
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:27
 msgid "Create fleet"
-msgstr "Створити флот"
-
-#: templates/fleetfinder/create-fleet.html:39
-#: templates/fleetfinder/edit-fleet.html:39
-msgid "Select groups"
 msgstr ""
 
-#: templates/fleetfinder/create-fleet.html:75
-#: templates/fleetfinder/edit-fleet.html:71
-#, fuzzy
-#| msgid "Enable Free Move"
-msgid "Enable free move"
-msgstr "Дозволити вільне переміщення"
-
-#: templates/fleetfinder/create-fleet.html:77
-#: templates/fleetfinder/edit-fleet.html:73
-msgid "Submit"
-msgstr "Відправити"
-
-#: templates/fleetfinder/dashboard.html:9
-#: templates/fleetfinder/partials/header/header-navigation.html:14
-#, fuzzy
-#| msgid "Available Fleets"
-msgid "Available fleets"
-msgstr "Доступні флоти"
+#: fleetfinder/templates/fleetfinder/dashboard.html:9
+msgid "Fleets available to you"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:19
-#, fuzzy
-#| msgid "Create Fleet"
+#: fleetfinder/templates/fleetfinder/dashboard.html:19
 msgid "Created at"
-msgstr "Створити флот"
+msgstr ""
 
-#: templates/fleetfinder/dashboard.html:20
+#: fleetfinder/templates/fleetfinder/dashboard.html:20
 msgid "Join"
 msgstr ""
 
-#: templates/fleetfinder/dashboard.html:23
+#: fleetfinder/templates/fleetfinder/dashboard.html:23
 msgid "Details"
 msgstr ""
 
-#: templates/fleetfinder/dashboard.html:24
+#: fleetfinder/templates/fleetfinder/dashboard.html:24
 msgid "Edit"
-msgstr "Редагувати"
+msgstr ""
 
-#: templates/fleetfinder/edit-fleet.html:6
-#: templates/fleetfinder/edit-fleet.html:14
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:6
+#: fleetfinder/templates/fleetfinder/edit-fleet.html:14
 msgid "Edit fleet"
 msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:6
-#, fuzzy
-#| msgid "Fleet Finder"
+#: fleetfinder/templates/fleetfinder/fleet-details.html:6
 msgid "Fleet details"
-msgstr "Пошук флоту"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:15
+#: fleetfinder/templates/fleetfinder/fleet-details.html:15
 msgid "Fleet composition"
 msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:23
-#: templates/fleetfinder/fleet-details.html:47
+#: fleetfinder/templates/fleetfinder/fleet-details.html:23
+#: fleetfinder/templates/fleetfinder/fleet-details.html:47
 msgid "Ship class"
 msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:24
+#: fleetfinder/templates/fleetfinder/fleet-details.html:24
 msgid "Count"
 msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:38
-#, fuzzy
-#| msgid "Fleet Commander"
+#: fleetfinder/templates/fleetfinder/fleet-details.html:38
 msgid "Fleet members"
-msgstr "Командувач флотом"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:46
+#: fleetfinder/templates/fleetfinder/fleet-details.html:46
 msgid "Name"
-msgstr "Назва"
+msgstr ""
 
-#: templates/fleetfinder/fleet-details.html:48
+#: fleetfinder/templates/fleetfinder/fleet-details.html:48
 msgid "System"
-msgstr "Система"
+msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:6 views.py:79
+#: fleetfinder/templates/fleetfinder/join-fleet.html:6 fleetfinder/views.py:91
 msgid "Join fleet"
 msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:14
+#: fleetfinder/templates/fleetfinder/join-fleet.html:14
 msgid "Fleet invitation"
 msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:24
+#: fleetfinder/templates/fleetfinder/join-fleet.html:25
 msgid "Select the characters to invite"
 msgstr ""
 
-#: templates/fleetfinder/join-fleet.html:33
+#: fleetfinder/templates/fleetfinder/join-fleet.html:35
 msgid "Send fleet invites"
 msgstr ""
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:5
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:15
+msgid "Select groups"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:46
+msgid "Enable free move"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html:49
+msgid "Submit"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
-#: templates/fleetfinder/partials/footer/app-translation-footer.html:8
+#: fleetfinder/templates/fleetfinder/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: templates/fleetfinder/partials/header/header-navigation.html:7
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:6
+msgid "Available fleets"
+msgstr ""
+
+#: fleetfinder/templates/fleetfinder/partials/header/header-navigation.html:17
 msgid "Toggle navigation"
 msgstr ""
 
-#: views.py:92
+#: fleetfinder/views.py:104
 msgid "View fleet details"
 msgstr ""
 
-#: views.py:99
+#: fleetfinder/views.py:113
 msgid "Edit fleet advert"
 msgstr ""
 
-#: views.py:243
+#: fleetfinder/views.py:279
 #, python-brace-format
 msgid ""
 "<h4>Error!</h4><p>ESI returned the following error: {esi_error_message}</p>"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_fleetfinder-2.0.1/fleetfinder/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,31 +1,34 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Chinese (Simplified) (Alliance Auth Apps)\n"
+"Project-Id-Version: Polish (Alliance Auth Apps)\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-fleetfinder/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-fleetfinder/pl/>\n"
+"Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
+msgstr ""
+"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
+"tłumaczenia?"
 
 msgid "Fleet commander"
-msgstr "舰队指挥"
-
-msgid "Fleet name"
-msgstr "舰队名字"
+msgstr "Dowódca floty"
 
 msgid "Join our team of translators!"
-msgstr "加入我们的翻译团队吧！"
+msgstr "Dołącz do naszego zespołu tłumaczy!"
+
+msgid "System"
+msgstr "System Solarny"
 
-msgid "Name"
-msgstr "名字"
+msgid "Toggle navigation"
+msgstr "Przełącz nawigacje"
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/migrations/0001_initial.py` & `aa_fleetfinder-2.0.1/fleetfinder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/migrations/0002_esi_error_handling_and_verbose_names.py` & `aa_fleetfinder-2.0.1/fleetfinder/migrations/0002_esi_error_handling_and_verbose_names.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/migrations/0003_alter_fleet_fleet_commander_alter_fleet_groups_and_more.py` & `aa_fleetfinder-2.0.1/fleetfinder/migrations/0003_alter_fleet_fleet_commander_alter_fleet_groups_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.css` & `aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.min.css` & `aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.min.css.map` & `aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/css/slimselect.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/js/slimselect.min.js` & `aa_fleetfinder-2.0.1/fleetfinder/static/fleetfinder/libs/slim-select/2.6.0/js/slimselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/base.html` & `aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/base.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/create-fleet.html` & `aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/create-fleet.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/dashboard.html` & `aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/edit-fleet.html` & `aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/edit-fleet.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/fleet-details.html` & `aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/fleet-details.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/join-fleet.html` & `aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/join-fleet.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html` & `aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/partials/body/form-fleet-details.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html` & `aa_fleetfinder-2.0.1/fleetfinder/templates/fleetfinder/partials/header/header-navigation.html`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/templatetags/fleetfinder.py` & `aa_fleetfinder-2.0.1/fleetfinder/templatetags/fleetfinder.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/tests/test_access.py` & `aa_fleetfinder-2.0.1/fleetfinder/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/tests/test_auth_hooks.py` & `aa_fleetfinder-2.0.1/fleetfinder/tests/test_auth_hooks.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             character_id=1002,
             character_name="Bruce Wayne",
             permissions=["fleetfinder.access_fleetfinder"],
         )
 
         cls.html_menu = f"""
             <li class="d-flex flex-wrap m-2 p-2 pt-0 pb-0 mt-0 mb-0 me-0 pe-0">
-                <i class="nav-link fas fa-users fa-fw align-self-center me-3 "></i>
+                <i class="nav-link fa-solid fa-users fa-fw align-self-center me-3 "></i>
                 <a class="nav-link flex-fill align-self-center me-auto" href="{reverse(viewname='fleetfinder:dashboard')}">
                     Fleet Finder
                 </a>
             </li>
         """
 
     def test_render_hook_success(self):
```

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/tests/test_templatetags.py` & `aa_fleetfinder-2.0.1/fleetfinder/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/fleetfinder/tests/utils.py` & `aa_fleetfinder-2.0.1/fleetfinder/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/LICENSE` & `aa_fleetfinder-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_fleetfinder-2.0.0b1/README.md` & `aa_fleetfinder-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,21 @@
 
 ______________________________________________________________________
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Fleet Finder needs at least Alliance Auth v4.0.0!**
+> **AA Fleet Finder >= 2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.5.2`.
 
 ### Step 1: Install the Package<a name="step-1-install-the-package"></a>
 
 Make sure you're in the virtual environment (venv) of your Alliance Auth installation Then install the latest release directly from PyPi.
 
 ```shell
 pip install aa-fleetfinder
```

### Comparing `aa_fleetfinder-2.0.0b1/pyproject.toml` & `aa_fleetfinder-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth>=4.0.0b1",
+    "allianceauth<5.0.0,>=4",
     "allianceauth-app-utils>=1.14.2",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
     "coverage",
     "django-webtest",
 ]
```

### Comparing `aa_fleetfinder-2.0.0b1/PKG-INFO` & `aa_fleetfinder-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aa-fleetfinder
-Version: 2.0.0b1
+Version: 2.0.1
 Summary: Fleet finder plugin for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-fleetfinder/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-fleetfinder/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-fleetfinder
 Project-URL: Source, https://github.com/ppfeufer/aa-fleetfinder.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-fleetfinder/issues
@@ -698,15 +698,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.14.2
-Requires-Dist: allianceauth>=4.0.0b1
+Requires-Dist: allianceauth<5.0.0,>=4
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
 
 # AA Fleet Finder<a name="aa-fleet-finder"></a>
 
@@ -746,19 +746,21 @@
 
 ______________________________________________________________________
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Fleet Finder needs at least Alliance Auth v4.0.0!**
+> **AA Fleet Finder >= 2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.5.2`.
 
 ### Step 1: Install the Package<a name="step-1-install-the-package"></a>
 
 Make sure you're in the virtual environment (venv) of your Alliance Auth installation Then install the latest release directly from PyPi.
 
 ```shell
 pip install aa-fleetfinder
```

