# Comparing `tmp/aa_bulletin_board-2.0.0b1.tar.gz` & `tmp/aa_bulletin_board-2.0.1.tar.gz`

## Comparing `aa_bulletin_board-2.0.0b1.tar` & `aa_bulletin_board-2.0.1.tar`

### file list

```diff
@@ -1,75 +1,83 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/apps.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/auth_hooks.py
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/forms.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/helpers.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/managers.py
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/models.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/urls.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/views.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/django.pot
--rw-r--r--   0        0        0     3248 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5916 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4785 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6130 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7208 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0001_initial.py
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0002_alter_bulletin_slug.py
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0003_group_restrictions.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0004_model_translation.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0005_alter_general_options.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0006_switch_to_ckeditor_5.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/__init__.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css.map
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.js
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.min.js
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.min.js.map
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.js
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.min.js
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.min.js.map
--rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js
--rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/base.html
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html
--rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-css.html
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-equal-height-js.html
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-oembed-js.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/bundles/ckeditor5-css.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/bundles/ckeditor5-js.html
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-css.html
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-js.html
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/partials/header/page-header.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templatetags/__init__.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/templatetags/aa_bulletin_board.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/__init__.py
--rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_access.py
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     8633 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_bulletins.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_templatetags.py
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_user_interface.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/LICENSE
--rw-r--r--   0        0        0    15752 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/README.md
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    58165 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/__init__.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/apps.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/auth_hooks.py
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/forms.py
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/helpers.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/managers.py
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/models.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/urls.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/views.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/django.pot
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5077 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3404 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6162 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6452 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4951 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4966 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4159 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5896 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0001_initial.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0002_alter_bulletin_slug.py
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0003_group_restrictions.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0004_model_translation.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0005_alter_general_options.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0006_switch_to_ckeditor_5.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/__init__.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css.map
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.js
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.min.js
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.min.js.map
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.js
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.min.js
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.min.js.map
+-rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js
+-rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/base.html
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-css.html
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-equal-height-js.html
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/bundles/aa-bulletin-board-oembed-js.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/bundles/ckeditor5-css.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/bundles/ckeditor5-js.html
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-css.html
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/bundles/sumoselect-js.html
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/partials/header/page-header.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templatetags/__init__.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/templatetags/aa_bulletin_board.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/tests/__init__.py
+-rw-r--r--   0        0        0     6874 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_access.py
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     8633 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_bulletins.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_templatetags.py
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_user_interface.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/aa_bulletin_board/tests/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/LICENSE
+-rw-r--r--   0        0        0    15795 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/README.md
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    58207 2020-02-02 00:00:00.000000 aa_bulletin_board-2.0.1/PKG-INFO
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/auth_hooks.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/auth_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         """
         Setup menu entry for sidebar
         """
 
         MenuItemHook.__init__(
             self,
             text=__title__,
-            classes="fas fa-clipboard-list",
+            classes="fa-solid fa-clipboard-list",
             url_name="aa_bulletin_board:dashboard",
             navactive=["aa_bulletin_board:"],
         )
 
     def render(self, request):
         """
         Check if the user has the permission to view this app
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/forms.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/forms.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/helpers.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/managers.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/managers.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/models.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/models.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/urls.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/urls.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/views.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/views.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/django.pot` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,166 +1,175 @@
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
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-03-15 18:14+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-bulletin-board/it/>\n"
+"Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr ""
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr ""
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
 msgstr ""
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
 msgstr ""
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
 msgstr ""
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr ""
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
 msgstr ""
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr ""
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr ""
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+msgid "No bulletins found."
+msgstr ""
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 msgid "Edit bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 msgid "Create new bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 msgid "Update bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 msgid "Create bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 msgid "Add bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr ""
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr ""
 
-#: aa_bulletin_board/views.py:167
-#, python-brace-format
-msgid "Bulletin \"{bulletin__title}\" updated."
+#: aa_bulletin_board/views.py:168
+msgid "The bulletin you are trying to edit does not exist."
 msgstr ""
 
-#: aa_bulletin_board/views.py:186
-msgid "The bulletin you are trying to edit does not exist."
+#: aa_bulletin_board/views.py:195
+#, python-brace-format
+msgid "Bulletin \"{bulletin__title}\" updated."
 msgstr ""
 
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr ""
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 msgid "The bulletin you are trying to delete does not exist."
 msgstr ""
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/de/LC_MESSAGES/django.mo` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/de/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-bulletin-board/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Add bulletin"
 msgstr "Bulletin hinzufügen"
 
 msgid "Back"
 msgstr "Zurück"
 
@@ -76,14 +76,17 @@
 
 msgid "Group restrictions"
 msgstr "Gruppenbeschränkungen"
 
 msgid "Join our team of translators!"
 msgstr "Tritt unserm Team von Übersetzern bei!"
 
+msgid "No bulletins found."
+msgstr "Keine Bulletins gefunden."
+
 msgid "Read more"
 msgstr "Weiter lesen"
 
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
@@ -115,7 +118,10 @@
 msgstr "Bulletin aktualisieren"
 
 msgid "Updated"
 msgstr "Aktualisiert"
 
 msgid "User"
 msgstr "Nutzer"
+
+msgid "You have forgotten the content!"
+msgstr "Du hast den Inhalt vergessen!"
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/de/LC_MESSAGES/django.po` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,135 +1,143 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: 2023-10-01 11:43+0000\n"
+"POT-Creation-Date: 2024-03-15 18:14+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-bulletin-board/de/>\n"
+"Language-Team: German <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-bulletin-board/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr "Bulletin Board"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr "Bulletin Board v{__version__}"
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 "Beschränkt dieses Bulletin auf bestimmte Gruppen. Wenn keine "
 "Gruppenbeschränkungen bestehen, kann jeder der Zugriff auf dieses Modul hat, "
 "dieses Bulletin lesen."
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr "Du hast den Inhalt vergessen!"
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
 msgstr "Kann auf diese App zugreifen"
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
 msgstr "Kann Bulletins verwalten (hinzufügen/ändern/entfernen)"
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
 msgstr "Titel"
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr "Inhalt"
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr "Erstellt"
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr "Aktualisiert"
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
 msgstr "Nutzer"
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
 msgstr "Gruppenbeschränkungen"
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr "Bulletin"
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr "Bulletins"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr "Zurück"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr "Bearbeiten"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
 msgstr "Löschen"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
 msgstr[0] "Dieses Bulletin ist auf die folgende Gruppe beschränkt:"
 msgstr[1] "Dieses Bulletin ist auf die folgenden Gruppen beschränkt:"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr "Weiter lesen"
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+msgid "No bulletins found."
+msgstr "Keine Bulletins gefunden."
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 msgid "Edit bulletin"
 msgstr "Bulletin bearbeiten"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 msgid "Create new bulletin"
 msgstr "Neuen Bulletin erstellen"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 msgid "Update bulletin"
 msgstr "Bulletin aktualisieren"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 msgid "Create bulletin"
 msgstr "Bulletin erstellen"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 msgid "Add bulletin"
 msgstr "Bulletin hinzufügen"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -137,36 +145,36 @@
 "Du möchtest helfen diese App in Deine Sprache zu übersetzen oder die "
 "bestehende Übersetzung verbessern?"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Tritt unserm Team von Übersetzern bei!"
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr "Bulletin „{bulletin__title}“ erstellt."
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr ""
 "Dieses Bulletin existiert entweder nicht oder Du hast keinen Zugriff darauf."
 
-#: aa_bulletin_board/views.py:167
+#: aa_bulletin_board/views.py:168
+msgid "The bulletin you are trying to edit does not exist."
+msgstr "Das Bulletin das Du bearbeiten möchtest scheint nicht zu existieren."
+
+#: aa_bulletin_board/views.py:195
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" updated."
 msgstr "Bulletin „{bulletin__title}“ aktualisiert."
 
-#: aa_bulletin_board/views.py:186
-msgid "The bulletin you are trying to edit does not exist."
-msgstr "Das Bulletin das Du bearbeiten möchtest scheint nicht zu existieren."
-
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr "Bulletin „{bulletin.title}“ gelöscht."
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 msgid "The bulletin you are trying to delete does not exist."
 msgstr "Das Bulletin das Du versuchst zu löschen scheint nicht zu existieren."
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/es/LC_MESSAGES/django.mo` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/es/LC_MESSAGES/django.mo`

 * *Files 14% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-bulletin-board/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Back"
 msgstr "Atrás"
 
 msgid "Bulletin"
 msgstr "Anuncio"
 
@@ -77,14 +77,19 @@
 
 msgid "The bulletin you are trying to delete does not exist."
 msgstr "El anuncio que intenta eliminar no existe."
 
 msgid "The bulletin you are trying to edit does not exist."
 msgstr "El anuncio que intenta editar no existe."
 
+msgid "This bulletin is restricted to the following group:"
+msgid_plural "This bulletin is restricted to the following groups:"
+msgstr[0] "Este anuncio está restringido a los siguiente grupo:"
+msgstr[1] "Este anuncio está restringido a los siguientes grupos:"
+
 msgid "Title"
 msgstr "Título"
 
 msgid "Updated"
 msgstr "Actualizado"
 
 msgid "User"
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/es/LC_MESSAGES/django.po` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,147 +1,155 @@
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
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: 2023-10-25 07:04+0000\n"
+"POT-Creation-Date: 2024-03-15 18:14+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
 "Last-Translator: Geovanny David Morales De la cruz <moralesgeovanny1996@gmail"
 ".com>\n"
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-bulletin-board/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr "Tablón de Anuncios"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr "Tablón de Anuncios v{__version__}"
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 "Restringir este anuncio a ciertos grupos. Si no existen restricciones de "
 "grupo, todos los que tengan acceso a este módulo pueden leer este anuncio."
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr ""
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
 msgstr "Puede acceder esta aplicacion"
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
 msgstr ""
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
 msgstr "Título"
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr "Contenido"
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr "Creado"
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr "Actualizado"
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
 msgstr "Usuario"
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
 msgstr "Restricciones de grupo"
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr "Anuncio"
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr "Anuncios"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr "Atrás"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr "Editar"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
 msgstr "Borrar"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
-#, fuzzy
-#| msgid "This bulletin is restricted to the following group(s):"
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
-msgstr[0] "Este anuncio está restringido a los siguientes grupos:"
+msgstr[0] "Este anuncio está restringido a los siguiente grupo:"
 msgstr[1] "Este anuncio está restringido a los siguientes grupos:"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr "Leer más"
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+#, fuzzy
+#| msgid "Bulletin Board"
+msgid "No bulletins found."
+msgstr "Tablón de Anuncios"
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 #, fuzzy
 #| msgid "Edit Bulletin"
 msgid "Edit bulletin"
 msgstr "Editar Anuncio"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 #, fuzzy
 #| msgid "Create New Bulletin"
 msgid "Create new bulletin"
 msgstr "Crear nuevo Anuncio"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 #, fuzzy
 #| msgid "Update Bulletin"
 msgid "Update bulletin"
 msgstr "Actualizar Anuncio"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 #, fuzzy
 #| msgid "Create Bulletin"
 msgid "Create bulletin"
 msgstr "Crear Anuncio"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 #, fuzzy
 #| msgid "Add Bulletin"
 msgid "Add bulletin"
 msgstr "Agregar Anuncio"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
@@ -151,39 +159,39 @@
 "¿Quieres ayudar a traducir esta aplicación a tu idioma o mejorar la "
 "traducción existente?"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "¡Únete a nuestro equipo de traductores!"
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr "Se ha creado el Anuncio «{bulletin__title}»."
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 #, fuzzy
 #| msgid ""
 #| "The bulletin you are looking for does not exist, or you don't have access "
 #| "to it."
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr "El anuncio que busca no existe, o no tiene acceso a él."
 
-#: aa_bulletin_board/views.py:167
+#: aa_bulletin_board/views.py:168
+msgid "The bulletin you are trying to edit does not exist."
+msgstr "El anuncio que intenta editar no existe."
+
+#: aa_bulletin_board/views.py:195
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" updated."
 msgstr "Se ha actualizado el Anuncio «{bulletin__title}»."
 
-#: aa_bulletin_board/views.py:186
-msgid "The bulletin you are trying to edit does not exist."
-msgstr "El anuncio que intenta editar no existe."
-
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr "Se ha eliminado el Anuncio «{bulletin.title}»."
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 msgid "The bulletin you are trying to delete does not exist."
 msgstr "El anuncio que intenta eliminar no existe."
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,21 +7,24 @@
 "Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-bulletin-board/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Can access this app"
 msgstr "Peut accéder à cette application"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 "Voulez-vous aider à traduire cette application dans votre langue ou "
 "améliorer la traduction existante ?"
 
+msgid "Group restrictions"
+msgstr "Restrictions de groupe"
+
 msgid "Join our team of translators!"
 msgstr "Rejoignez notre équipe de traducteurs !"
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,131 +3,139 @@
 # This file is distributed under the same license as the PACKAGE package.
 # erka Ekanon <M6musicT@hotmail.fr>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: 2024-01-12 19:05+0000\n"
+"POT-Creation-Date: 2024-03-15 18:14+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: French <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-bulletin-board/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr ""
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr ""
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
 msgstr "Peut accéder à cette application"
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
 msgstr ""
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
 msgstr ""
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr ""
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
 msgstr ""
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
-msgstr ""
+msgstr "Restrictions de groupe"
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr ""
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr ""
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+msgid "No bulletins found."
+msgstr ""
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 msgid "Edit bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 msgid "Create new bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 msgid "Update bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 msgid "Create bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 msgid "Add bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -135,35 +143,35 @@
 "Voulez-vous aider à traduire cette application dans votre langue ou "
 "améliorer la traduction existante ?"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Rejoignez notre équipe de traducteurs !"
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr ""
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr ""
 
-#: aa_bulletin_board/views.py:167
-#, python-brace-format
-msgid "Bulletin \"{bulletin__title}\" updated."
+#: aa_bulletin_board/views.py:168
+msgid "The bulletin you are trying to edit does not exist."
 msgstr ""
 
-#: aa_bulletin_board/views.py:186
-msgid "The bulletin you are trying to edit does not exist."
+#: aa_bulletin_board/views.py:195
+#, python-brace-format
+msgid "Bulletin \"{bulletin__title}\" updated."
 msgstr ""
 
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr ""
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 msgid "The bulletin you are trying to delete does not exist."
 msgstr ""
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/it_IT/LC_MESSAGES/django.po` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/sk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,165 +3,176 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"POT-Creation-Date: 2024-03-20 17:29+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-bulletin-board/it/>\n"
-"Language: it_IT\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-bulletin-board/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
-
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"X-Generator: Weblate 5.5.3\n"
+
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr ""
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr ""
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
 msgstr ""
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
 msgstr ""
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
 msgstr ""
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr ""
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
 msgstr ""
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr ""
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr ""
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+msgid "No bulletins found."
+msgstr ""
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 msgid "Edit bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 msgid "Create new bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 msgid "Update bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 msgid "Create bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 msgid "Add bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr ""
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr ""
 
-#: aa_bulletin_board/views.py:167
-#, python-brace-format
-msgid "Bulletin \"{bulletin__title}\" updated."
+#: aa_bulletin_board/views.py:168
+msgid "The bulletin you are trying to edit does not exist."
 msgstr ""
 
-#: aa_bulletin_board/views.py:186
-msgid "The bulletin you are trying to edit does not exist."
+#: aa_bulletin_board/views.py:195
+#, python-brace-format
+msgid "Bulletin \"{bulletin__title}\" updated."
 msgstr ""
 
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr ""
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 msgid "The bulletin you are trying to delete does not exist."
 msgstr ""
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ja/LC_MESSAGES/django.po` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ja/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,164 +3,172 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"POT-Creation-Date: 2024-03-15 18:14+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-bulletin-board/ja/>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-bulletin-board/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr ""
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr ""
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
 msgstr ""
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
 msgstr ""
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
 msgstr ""
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr ""
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
 msgstr ""
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr ""
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
 msgstr[0] ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr ""
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+msgid "No bulletins found."
+msgstr ""
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 msgid "Edit bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 msgid "Create new bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 msgid "Update bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 msgid "Create bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 msgid "Add bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr ""
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr ""
 
-#: aa_bulletin_board/views.py:167
-#, python-brace-format
-msgid "Bulletin \"{bulletin__title}\" updated."
+#: aa_bulletin_board/views.py:168
+msgid "The bulletin you are trying to edit does not exist."
 msgstr ""
 
-#: aa_bulletin_board/views.py:186
-msgid "The bulletin you are trying to edit does not exist."
+#: aa_bulletin_board/views.py:195
+#, python-brace-format
+msgid "Bulletin \"{bulletin__title}\" updated."
 msgstr ""
 
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr ""
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 msgid "The bulletin you are trying to delete does not exist."
 msgstr ""
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-bulletin-board/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Back"
 msgstr "뒤로"
 
 msgid "Bulletin"
 msgstr "불레틴"
 
@@ -36,14 +36,17 @@
 
 msgid "Bulletins"
 msgstr "불레틴"
 
 msgid "Can access this app"
 msgstr "서비스에 접근할 수 있습니다"
 
+msgid "Can manage (add/change/remove) bulletins"
+msgstr "게시판 (추가/변경/삭제) 관리 권한"
+
 msgid "Content"
 msgstr "내용"
 
 msgid "Created"
 msgstr "생성 날짜"
 
 msgid "Delete"
@@ -57,15 +60,15 @@
 msgid "Edit"
 msgstr "수정"
 
 msgid "Group restrictions"
 msgstr "그룹 제한"
 
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
 msgid "Read more"
 msgstr "더보기"
 
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
@@ -83,7 +86,10 @@
 msgstr "제목"
 
 msgid "Updated"
 msgstr "업데이트 날짜"
 
 msgid "User"
 msgstr "사용자"
+
+msgid "You have forgotten the content!"
+msgstr "내용을 잊어버리셨군요!"
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,184 +1,196 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Author50CO <tkddlschry@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Author50CO <tkddlschry@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Mind of the Raven <okanieva@gmail.com>, 2024.
+# Rodpold Shard <rodpold@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: 2023-12-29 09:04+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"POT-Creation-Date: 2024-03-15 18:14+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
+"Last-Translator: Rodpold Shard <rodpold@gmail.com>\n"
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-bulletin-board/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr "불레틴 보드"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr "불레틴 보드 v{__version__}"
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 "불레틴 보드의 항목을 그룹별로 열람을 제한할 수 있습니다. 그룹 제한이 없다면, "
 "모듈의 접근 권한이 있는 모든 사용자가 이 항목을 열람할 수 있습니다."
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr "내용을 잊어버리셨군요!"
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
 msgstr "서비스에 접근할 수 있습니다"
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
-msgstr ""
+msgstr "게시판 (추가/변경/삭제) 관리 권한"
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
 msgstr "제목"
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr "내용"
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr "생성 날짜"
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr "업데이트 날짜"
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
 msgstr "사용자"
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
 msgstr "그룹 제한"
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr "불레틴"
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr "불레틴"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr "뒤로"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr "수정"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
 msgstr "삭제"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 #, fuzzy
 #| msgid "This bulletin is restricted to the following group(s):"
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
 msgstr[0] "이 불레틴은 다음 그룹(들)만 열람할 수 있습니다:"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr "더보기"
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+#, fuzzy
+#| msgid "Bulletin Board"
+msgid "No bulletins found."
+msgstr "불레틴 보드"
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 #, fuzzy
 #| msgid "Edit Bulletin"
 msgid "Edit bulletin"
 msgstr "불레틴 수정"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 #, fuzzy
 #| msgid "Create New Bulletin"
 msgid "Create new bulletin"
 msgstr "새 불레틴 생성"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 #, fuzzy
 #| msgid "Update Bulletin"
 msgid "Update bulletin"
 msgstr "불레틴 업데이트"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 #, fuzzy
 #| msgid "Create Bulletin"
 msgid "Create bulletin"
 msgstr "불레틴 생성"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 #, fuzzy
 #| msgid "Add Bulletin"
 msgid "Add bulletin"
 msgstr "불레틴 추가"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr "불레틴 “{bulletin__title}” 생성됨."
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 #, fuzzy
 #| msgid ""
 #| "The bulletin you are looking for does not exist, or you don't have access "
 #| "to it."
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr "찾는 불레틴이 없거나, 열람 권한이 없습니다."
 
-#: aa_bulletin_board/views.py:167
+#: aa_bulletin_board/views.py:168
+msgid "The bulletin you are trying to edit does not exist."
+msgstr "수정하려는 불레틴이 없습니다."
+
+#: aa_bulletin_board/views.py:195
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" updated."
 msgstr "불레틴 “{bulletin__title}” 업데이트됨."
 
-#: aa_bulletin_board/views.py:186
-msgid "The bulletin you are trying to edit does not exist."
-msgstr "수정하려는 불레틴이 없습니다."
-
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr "불레틴 “{bulletin.title}” 삭제됨."
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 msgid "The bulletin you are trying to delete does not exist."
 msgstr "삭제하려는 불레틴이 없습니다."
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ru/LC_MESSAGES/django.mo` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ru/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-bulletin-board/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Add bulletin"
 msgstr "Добавить бюллетень"
 
 msgid "Back"
 msgstr "Назад"
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/ru/LC_MESSAGES/django.po` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,139 +1,149 @@
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
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: 2023-10-03 11:01+0000\n"
-"Last-Translator: Max <mark25@inbox.ru>\n"
+"POT-Creation-Date: 2024-03-15 18:14+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-bulletin-board/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr "Доска бюллетеней"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr "Доска бюллетеней v{__version__}"
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 "Ограничить доступ к бюллетеню для конкретных групп. Если ограничение не "
 "задано, у всех пользователей модуля есть доступ к бюллетеню."
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr ""
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
 msgstr "Имеет доступ к приложению"
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
 msgstr "Может управлять (добавлять/изменять/удалять) бюллетенями"
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
 msgstr "Заглавие"
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr "Содержимое"
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr "Создан"
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr "Обновлен"
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
 msgstr "Пользователь"
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
 msgstr "Ограничения групп"
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr "Бюллетень"
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr "Бюллетени"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr "Назад"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr "Редактировать"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
 msgstr "Удалить"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
 msgstr[0] "Этот бюллетень доступен следующей группе:"
 msgstr[1] "Этот бюллетень доступен следующим группам:"
 msgstr[2] "Этот бюллетень доступен следующим группам:"
 msgstr[3] "Этот бюллетень доступен следующим группам:"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr "Читать"
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+#, fuzzy
+#| msgid "Bulletin Board"
+msgid "No bulletins found."
+msgstr "Доска бюллетеней"
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 msgid "Edit bulletin"
 msgstr "Редактировать бюллетень"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 msgid "Create new bulletin"
 msgstr "Создание нового бюллетеня"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 msgid "Update bulletin"
 msgstr "Обновить бюллетень"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 msgid "Create bulletin"
 msgstr "Создать бюллетень"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 msgid "Add bulletin"
 msgstr "Добавить бюллетень"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -141,35 +151,35 @@
 "Вы хотите помочь перевести это приложение на ваш язык или улучшить текущий "
 "перевод?"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Присоединяйтесь к нашей команде переводчиков!"
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr "Бюллетень «{bulletin__title}» создан."
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr "Запрошенный бюллетень не существует или у Вас нет доступа."
 
-#: aa_bulletin_board/views.py:167
+#: aa_bulletin_board/views.py:168
+msgid "The bulletin you are trying to edit does not exist."
+msgstr "Бюллетень, который вы пытаетесь отредактировать, не существует."
+
+#: aa_bulletin_board/views.py:195
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" updated."
 msgstr "Бюллетень «{bulletin__title}» обновлен."
 
-#: aa_bulletin_board/views.py:186
-msgid "The bulletin you are trying to edit does not exist."
-msgstr "Бюллетень, который вы пытаетесь отредактировать, не существует."
-
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr "Бюллетень «{bulletin.title}» удален."
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 msgid "The bulletin you are trying to delete does not exist."
 msgstr "Бюллетень, который вы пытаетесь удалить, не существует."
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/uk/LC_MESSAGES/django.mo` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/uk/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-bulletin-board/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Back"
 msgstr "Повернутися"
 
 msgid "Bulletin"
 msgstr "Інформаційний бюлетень"
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/uk/LC_MESSAGES/django.po` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/uk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,150 +1,160 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
-# "Andrii M." <elfleg0las88@gmail.com>, 2023.
-# Kristof <kristof@teh.ninja>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# "Andrii M." <elfleg0las88@gmail.com>, 2023, 2024.
+# Kristof <kristof@teh.ninja>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: 2023-10-02 15:43+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"POT-Creation-Date: 2024-03-15 18:14+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
+"Last-Translator: Kristof <kristof@teh.ninja>\n"
 "Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-bulletin-board/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr "Дошка оголошень"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr "Дошка оголошень v{__version__}"
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 "Обмежте доступ до цього бюлетеня для певних груп. Якщо не встановлено жодних "
 "групових обмежень, кожен, хто має доступ до цього модуля, зможе прочитати "
 "цей бюлетень."
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr ""
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
 msgstr ""
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
 msgstr ""
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
 msgstr "Заголовок"
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr "Вміст"
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr "Створено"
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr ""
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
 msgstr ""
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
 msgstr "Групові обмеження"
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr "Інформаційний бюлетень"
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr "Інформаційні бюлетені"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr "Повернутися"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr "Редагувати"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
 msgstr "Видалити"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 #, fuzzy
 #| msgid "This bulletin is restricted to the following group(s):"
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
 msgstr[0] "Доступ до цього бюлетеня обмежений для наступних груп:"
 msgstr[1] "Доступ до цього бюлетеня обмежений для наступних груп:"
 msgstr[2] "Доступ до цього бюлетеня обмежений для наступних груп:"
 msgstr[3] "Доступ до цього бюлетеня обмежений для наступних груп:"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr "Читати далі"
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+#, fuzzy
+#| msgid "Bulletin Board"
+msgid "No bulletins found."
+msgstr "Дошка оголошень"
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 #, fuzzy
 #| msgid "Edit Bulletin"
 msgid "Edit bulletin"
 msgstr "Редагувати бюлетень"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 #, fuzzy
 #| msgid "Create New Bulletin"
 msgid "Create new bulletin"
 msgstr "Створити новий бюлетень"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 #, fuzzy
 #| msgid "Update Bulletin"
 msgid "Update bulletin"
 msgstr "Бюлетень оновлень"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 #, fuzzy
 #| msgid "Create Bulletin"
 msgid "Create bulletin"
 msgstr "Створити бюлетень"
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 #, fuzzy
 #| msgid "Add Bulletin"
 msgid "Add bulletin"
 msgstr "Додати інформаційний бюлетень"
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
@@ -152,43 +162,43 @@
 "existing translation?"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr "Створено бюлетень «{bulletin__title}»."
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 #, fuzzy
 #| msgid ""
 #| "The bulletin you are looking for does not exist, or you don't have access "
 #| "to it."
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr "Бюлетень, який ви шукаєте, не існує, або у вас немає до нього доступу."
 
-#: aa_bulletin_board/views.py:167
-#, python-brace-format
-msgid "Bulletin \"{bulletin__title}\" updated."
-msgstr "Оновлено бюлетень «{bulletin__title}»."
-
-#: aa_bulletin_board/views.py:186
+#: aa_bulletin_board/views.py:168
 #, fuzzy
 #| msgid "The bulletin you are trying to edit for does not exist."
 msgid "The bulletin you are trying to edit does not exist."
 msgstr "Бюлетень, який ви намагаєтеся відредагувати, не існує."
 
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:195
+#, python-brace-format
+msgid "Bulletin \"{bulletin__title}\" updated."
+msgstr "Оновлено бюлетень «{bulletin__title}»."
+
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr "Бюлетень «{bulletin.title}» вилучено."
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 #, fuzzy
 #| msgid "The bulletin you are trying to delete for does not exist."
 msgid "The bulletin you are trying to delete does not exist."
 msgstr "Зведення, яке ви намагаєтеся видалити, не існує."
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_bulletin_board-2.0.1/aa_bulletin_board/locale/nl/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,166 +1,175 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Faer Yili <yilifaer@gmail.com>, 2024.
-# Dehao Wu <wudehao2000@163.com>, 2024.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:56+0200\n"
-"PO-Revision-Date: 2024-01-11 21:04+0000\n"
-"Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
-"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-bulletin-board/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"POT-Creation-Date: 2024-03-20 17:29+0100\n"
+"PO-Revision-Date: 2024-05-10 13:57+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-bulletin-board/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_bulletin_board/__init__.py:12 aa_bulletin_board/models.py:67
-#: aa_bulletin_board/templates/aa_bulletin_board/base.html:5
+#: aa_bulletin_board/__init__.py:9 aa_bulletin_board/models.py:67
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/base.html:10
 #: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:5
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:6
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:8
 msgid "Bulletin Board"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_bulletin_board/apps.py:21
 #, python-brace-format
 msgid "Bulletin Board v{__version__}"
 msgstr ""
 
-#: aa_bulletin_board/forms.py:71
+#: aa_bulletin_board/forms.py:65
 msgid ""
 "Restrict this bulletin to certain groups. If no group restrictions are in "
 "place, everyone who has access to this module can read this bulletin."
 msgstr ""
 
+#: aa_bulletin_board/forms.py:112
+msgid "You have forgotten the content!"
+msgstr ""
+
 #: aa_bulletin_board/models.py:71
 msgid "Can access this app"
-msgstr "允许访问此软件"
+msgstr ""
 
 #: aa_bulletin_board/models.py:72
 msgid "Can manage (add/change/remove) bulletins"
 msgstr ""
 
 #: aa_bulletin_board/models.py:81
 msgid "Title"
-msgstr "头衔"
+msgstr ""
 
-#: aa_bulletin_board/models.py:83
+#: aa_bulletin_board/models.py:84
 msgid "Content"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been created
-#: aa_bulletin_board/models.py:88
+#: aa_bulletin_board/models.py:90
 msgid "Created"
 msgstr ""
 
 #. Translators: This is the date and time the bulletin has been updated
-#: aa_bulletin_board/models.py:94
+#: aa_bulletin_board/models.py:96
 msgid "Updated"
 msgstr ""
 
-#: aa_bulletin_board/models.py:103
+#: aa_bulletin_board/models.py:105
 msgid "User"
-msgstr "用户"
+msgstr ""
 
-#: aa_bulletin_board/models.py:109
+#: aa_bulletin_board/models.py:111
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_bulletin_board/models.py:120
+#: aa_bulletin_board/models.py:122
 msgid "Bulletin"
 msgstr ""
 
-#: aa_bulletin_board/models.py:121
+#: aa_bulletin_board/models.py:123
 msgid "Bulletins"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:18
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:16
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:34
 msgid "Back"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:21
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:39
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:19
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
 msgid "Edit"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:22
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:40
+#: aa_bulletin_board/templates/aa_bulletin_board/bulletin.html:20
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:37
 msgid "Delete"
-msgstr "删除"
+msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:24
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:17
 msgid "This bulletin is restricted to the following group:"
 msgid_plural "This bulletin is restricted to the following groups:"
 msgstr[0] ""
+msgstr[1] ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:36
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:33
 msgid "Read more"
 msgstr ""
 
+#: aa_bulletin_board/templates/aa_bulletin_board/dashboard.html:47
+msgid "No bulletins found."
+msgstr ""
+
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:11
 msgid "Edit bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:14
 #: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:25
 msgid "Create new bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:45
 msgid "Update bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:49
+#: aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html:47
 msgid "Create bulletin"
 msgstr ""
 
-#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:6
+#: aa_bulletin_board/templates/aa_bulletin_board/partials/common/bulletin-board-management.html:7
 msgid "Add bulletin"
 msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
+msgstr ""
 
 #: aa_bulletin_board/templates/aa_bulletin_board/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "加入我们的翻译团队吧！"
+msgstr ""
 
-#: aa_bulletin_board/views.py:82
+#: aa_bulletin_board/views.py:98
 #, python-brace-format
 msgid "Bulletin \"{bulletin__title}\" created."
 msgstr ""
 
-#: aa_bulletin_board/views.py:125
+#: aa_bulletin_board/views.py:141
 msgid ""
 "The bulletin you are looking for does either not exist, or you don't have "
 "access to it."
 msgstr ""
 
-#: aa_bulletin_board/views.py:167
-#, python-brace-format
-msgid "Bulletin \"{bulletin__title}\" updated."
+#: aa_bulletin_board/views.py:168
+msgid "The bulletin you are trying to edit does not exist."
 msgstr ""
 
-#: aa_bulletin_board/views.py:186
-msgid "The bulletin you are trying to edit does not exist."
+#: aa_bulletin_board/views.py:195
+#, python-brace-format
+msgid "Bulletin \"{bulletin__title}\" updated."
 msgstr ""
 
-#: aa_bulletin_board/views.py:210
+#: aa_bulletin_board/views.py:227
 #, python-brace-format
 msgid "Bulletin \"{bulletin.title}\" deleted."
 msgstr ""
 
-#: aa_bulletin_board/views.py:217
+#: aa_bulletin_board/views.py:234
 msgid "The bulletin you are trying to delete does not exist."
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0001_initial.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0003_group_restrictions.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0003_group_restrictions.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0004_model_translation.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0004_model_translation.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0005_alter_general_options.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0005_alter_general_options.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/migrations/0006_switch_to_ckeditor_5.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/migrations/0006_switch_to_ckeditor_5.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.css`

 * *Files 4% similar despite different names*

```diff
@@ -15,30 +15,29 @@
     .aa-bulletin-board .cards-equal-height .card-bulletin-excerpt {
         margin-bottom: 0.5rem;
         width: 100%;
     }
 
     .aa-bulletin-board .card-bulletin-excerpt .card-body {
         height: 200px;
-        -webkit-mask-image: linear-gradient(rgb(0 0 0), transparent);
         mask-image: linear-gradient(rgb(0 0 0), transparent);
         overflow: hidden;
         padding: 1rem;
     }
 
     .aa-bulletin-board .card-bulletin-excerpt .card-footer-read-more-button {
         padding: 0.625rem 1rem;
     }
 
     .aa-bulletin-board .django-ckeditor-widget {
         display: initial !important;
     }
 
     .aa-bulletin-board img {
-        height: auto !important; /* to override inline style added by CKeditor */
+        height: auto !important; /* to override inline style added by CKEditor */
         max-width: 100%;
     }
 }
 
 /* SumoSelect
 ------------------------------------------------------------------------------------- */
 @media all {
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css`

 * *Files 4% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-@media all{.aa-bulletin-board-header-addition{display:block}.aa-bulletin-board .cards-equal-height{display:flex;flex-wrap:wrap}.aa-bulletin-board .cards-equal-height .card{width:100%}.aa-bulletin-board .cards-equal-height .card-bulletin-excerpt{margin-bottom:.5rem;width:100%}.aa-bulletin-board .card-bulletin-excerpt .card-body{height:200px;-webkit-mask-image:linear-gradient(rgb(0 0 0),transparent);mask-image:linear-gradient(rgb(0 0 0),transparent);overflow:hidden;padding:1rem}.aa-bulletin-board .card-bulletin-excerpt .card-footer-read-more-button{padding:.625rem 1rem}.aa-bulletin-board .django-ckeditor-widget{display:initial!important}.aa-bulletin-board img{height:auto!important;max-width:100%}.aa-bulletin-board .SumoSelect p{border-radius:var(--bs-border-radius);height:auto}.aa-bulletin-board .SumoSelect{color:rgb(54 54 54);display:inherit}.aa-bulletin-board .SumoSelect>.CaptionCont>label>i{background-image:none}.aa-bulletin-board .SumoSelect>.CaptionCont>span.placeholder{background-color:transparent;color:rgb(62 68 76);opacity:1}}@media all and (min-width:768px){.aa-bulletin-board .cards-equal-height .card-bulletin-excerpt{width:calc(100%/2)}}@media all and (min-width:1200px){.aa-bulletin-board .cards-equal-height .card-bulletin-excerpt{width:calc(100%/3)}}@media all{.aa-bulletin-board figure.media .oembed-video{height:auto;max-width:100%;overflow:hidden;padding-bottom:56.25%;position:relative}.aa-bulletin-board figure.media .oembed-video>iframe{height:100%;left:0;max-height:100vh;position:absolute;top:0;width:100%}.aa-bulletin-board .ck-rounded-corners{--ck-border-radius:var(--bs-border-radius)}.aa-bulletin-board .ck-editor__editable{color:initial}.aa-bulletin-board .ck-word-count{color:var(--bs-secondary-color)!important;--bs-text-opacity:1}}
+@media all{.aa-bulletin-board-header-addition{display:block}.aa-bulletin-board .cards-equal-height{display:flex;flex-wrap:wrap}.aa-bulletin-board .cards-equal-height .card{width:100%}.aa-bulletin-board .cards-equal-height .card-bulletin-excerpt{margin-bottom:.5rem;width:100%}.aa-bulletin-board .card-bulletin-excerpt .card-body{height:200px;mask-image:linear-gradient(rgb(0 0 0),transparent);overflow:hidden;padding:1rem}.aa-bulletin-board .card-bulletin-excerpt .card-footer-read-more-button{padding:.625rem 1rem}.aa-bulletin-board .django-ckeditor-widget{display:initial!important}.aa-bulletin-board img{height:auto!important;max-width:100%}.aa-bulletin-board .SumoSelect p{border-radius:var(--bs-border-radius);height:auto}.aa-bulletin-board .SumoSelect{color:rgb(54 54 54);display:inherit}.aa-bulletin-board .SumoSelect>.CaptionCont>label>i{background-image:none}.aa-bulletin-board .SumoSelect>.CaptionCont>span.placeholder{background-color:transparent;color:rgb(62 68 76);opacity:1}}@media all and (min-width:768px){.aa-bulletin-board .cards-equal-height .card-bulletin-excerpt{width:calc(100%/2)}}@media all and (min-width:1200px){.aa-bulletin-board .cards-equal-height .card-bulletin-excerpt{width:calc(100%/3)}}@media all{.aa-bulletin-board figure.media .oembed-video{height:auto;max-width:100%;overflow:hidden;padding-bottom:56.25%;position:relative}.aa-bulletin-board figure.media .oembed-video>iframe{height:100%;left:0;max-height:100vh;position:absolute;top:0;width:100%}.aa-bulletin-board .ck-rounded-corners{--ck-border-radius:var(--bs-border-radius)}.aa-bulletin-board .ck-editor__editable{color:initial}.aa-bulletin-board .ck-word-count{color:var(--bs-secondary-color)!important;--bs-text-opacity:1}}
 /*# sourceMappingURL=aa-bulletin-board.min.css.map */
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css.map` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/css/aa-bulletin-board.min.css.map`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'mappings'": "'AAAA,A,WACI,kC,CACI,a,CAGJ,sC,CACI,Y,CACA,c,CAGJ,4C,CACI,U,CAGJ,6D,CACI,mB,CACA,U,CAGJ,oD,CACI,Y,CACA,kD,CACA,e,CACA,Y,CAGJ,uE,CACI,oB,CAGJ,0C,CACI,yB,CAGJ,sB,CACI,qB,CACA,c,CAOJ,gC,CACI,qC,CACA,W,CAGJ,8B,CACI,mB,CACA,e,CAGJ,mD,CACI,qB,CAGJ,4D,CACI,4B,CACA,mB,CACA,WAIR,A,iCACI,6D,CACI,oBAIR,A,kCACI,6D,CACI,oBAMR,A,WACI,6C,CACI,W,CACA,c,CACA,e,CACA,qB,CACA,iB,CAGJ,oD,CACI,W,CACA,M,CACA,gB,CACA,iB,CACA,K,CACA,U,CAOJ,sC,CACI,0C,CAGJ,uC,CACI,a,CAGJ,iC,CACI,yC,CAEA,qB'",*

 * * "'sourcesContent'": "[' […]*

```diff
@@ -1,12 +1,12 @@
 {
     "file": "aa-bulletin-board.css",
-    "mappings": "AAAA,A,WACI,kC,CACI,a,CAGJ,sC,CACI,Y,CACA,c,CAGJ,4C,CACI,U,CAGJ,6D,CACI,mB,CACA,U,CAGJ,oD,CACI,Y,CACA,0D,CACA,kD,CACA,e,CACA,Y,CAGJ,uE,CACI,oB,CAGJ,0C,CACI,yB,CAGJ,sB,CACI,qB,CACA,c,CAOJ,gC,CACI,qC,CACA,W,CAGJ,8B,CACI,mB,CACA,e,CAGJ,mD,CACI,qB,CAGJ,4D,CACI,4B,CACA,mB,CACA,WAIR,A,iCACI,6D,CACI,oBAIR,A,kCACI,6D,CACI,oBAMR,A,WACI,6C,CACI,W,CACA,c,CACA,e,CACA,qB,CACA,iB,CAGJ,oD,CACI,W,CACA,M,CACA,gB,CACA,iB,CACA,K,CACA,U,CAOJ,sC,CACI,0C,CAGJ,uC,CACI,a,CAGJ,iC,CACI,yC,CAEA,qB",
+    "mappings": "AAAA,A,WACI,kC,CACI,a,CAGJ,sC,CACI,Y,CACA,c,CAGJ,4C,CACI,U,CAGJ,6D,CACI,mB,CACA,U,CAGJ,oD,CACI,Y,CACA,kD,CACA,e,CACA,Y,CAGJ,uE,CACI,oB,CAGJ,0C,CACI,yB,CAGJ,sB,CACI,qB,CACA,c,CAOJ,gC,CACI,qC,CACA,W,CAGJ,8B,CACI,mB,CACA,e,CAGJ,mD,CACI,qB,CAGJ,4D,CACI,4B,CACA,mB,CACA,WAIR,A,iCACI,6D,CACI,oBAIR,A,kCACI,6D,CACI,oBAMR,A,WACI,6C,CACI,W,CACA,c,CACA,e,CACA,qB,CACA,iB,CAGJ,oD,CACI,W,CACA,M,CACA,gB,CACA,iB,CACA,K,CACA,U,CAOJ,sC,CACI,0C,CAGJ,uC,CACI,a,CAGJ,iC,CACI,yC,CAEA,qB",
     "names": [],
     "sources": [
         "aa-bulletin-board.css"
     ],
     "sourcesContent": [
-        "@media all {\n    .aa-bulletin-board-header-addition {\n        display: block;\n    }\n\n    .aa-bulletin-board .cards-equal-height {\n        display: flex;\n        flex-wrap: wrap;\n    }\n\n    .aa-bulletin-board .cards-equal-height .card {\n        width: 100%;\n    }\n\n    .aa-bulletin-board .cards-equal-height .card-bulletin-excerpt {\n        margin-bottom: 0.5rem;\n        width: 100%;\n    }\n\n    .aa-bulletin-board .card-bulletin-excerpt .card-body {\n        height: 200px;\n        -webkit-mask-image: linear-gradient(rgb(0 0 0), transparent);\n        mask-image: linear-gradient(rgb(0 0 0), transparent);\n        overflow: hidden;\n        padding: 1rem;\n    }\n\n    .aa-bulletin-board .card-bulletin-excerpt .card-footer-read-more-button {\n        padding: 0.625rem 1rem;\n    }\n\n    .aa-bulletin-board .django-ckeditor-widget {\n        display: initial !important;\n    }\n\n    .aa-bulletin-board img {\n        height: auto !important; /* to override inline style added by CKeditor */\n        max-width: 100%;\n    }\n}\n\n/* SumoSelect\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-bulletin-board .SumoSelect p {\n        border-radius: var(--bs-border-radius);\n        height: auto;\n    }\n\n    .aa-bulletin-board .SumoSelect {\n        color: rgb(54 54 54);\n        display: inherit;\n    }\n\n    .aa-bulletin-board .SumoSelect > .CaptionCont > label > i {\n        background-image: none;\n    }\n\n    .aa-bulletin-board .SumoSelect > .CaptionCont > span.placeholder {\n        background-color: transparent;\n        color: rgb(62 68 76);\n        opacity: 1;\n    }\n}\n\n@media all and (min-width: 768px) {\n    .aa-bulletin-board .cards-equal-height .card-bulletin-excerpt {\n        width: calc(100% / 2);\n    }\n}\n\n@media all and (min-width: 1200px) {\n    .aa-bulletin-board .cards-equal-height .card-bulletin-excerpt {\n        width: calc(100% / 3);\n    }\n}\n\n/* Fix for oEmbed videos\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-bulletin-board figure.media .oembed-video {\n        height: auto;\n        max-width: 100%;\n        overflow: hidden;\n        padding-bottom: 56.25%;\n        position: relative;\n    }\n\n    .aa-bulletin-board figure.media .oembed-video > iframe {\n        height: 100%;\n        left: 0;\n        max-height: 100vh;\n        position: absolute;\n        top: 0;\n        width: 100%;\n    }\n}\n\n/* CKEditor 5 (WYSIWYG editor)\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-bulletin-board .ck-rounded-corners {\n        --ck-border-radius: var(--bs-border-radius);\n    }\n\n    .aa-bulletin-board .ck-editor__editable {\n        color: initial;\n    }\n\n    .aa-bulletin-board .ck-word-count {\n        color: var(--bs-secondary-color) !important;\n\n        --bs-text-opacity: 1;\n    }\n}\n"
+        "@media all {\n    .aa-bulletin-board-header-addition {\n        display: block;\n    }\n\n    .aa-bulletin-board .cards-equal-height {\n        display: flex;\n        flex-wrap: wrap;\n    }\n\n    .aa-bulletin-board .cards-equal-height .card {\n        width: 100%;\n    }\n\n    .aa-bulletin-board .cards-equal-height .card-bulletin-excerpt {\n        margin-bottom: 0.5rem;\n        width: 100%;\n    }\n\n    .aa-bulletin-board .card-bulletin-excerpt .card-body {\n        height: 200px;\n        mask-image: linear-gradient(rgb(0 0 0), transparent);\n        overflow: hidden;\n        padding: 1rem;\n    }\n\n    .aa-bulletin-board .card-bulletin-excerpt .card-footer-read-more-button {\n        padding: 0.625rem 1rem;\n    }\n\n    .aa-bulletin-board .django-ckeditor-widget {\n        display: initial !important;\n    }\n\n    .aa-bulletin-board img {\n        height: auto !important; /* to override inline style added by CKEditor */\n        max-width: 100%;\n    }\n}\n\n/* SumoSelect\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-bulletin-board .SumoSelect p {\n        border-radius: var(--bs-border-radius);\n        height: auto;\n    }\n\n    .aa-bulletin-board .SumoSelect {\n        color: rgb(54 54 54);\n        display: inherit;\n    }\n\n    .aa-bulletin-board .SumoSelect > .CaptionCont > label > i {\n        background-image: none;\n    }\n\n    .aa-bulletin-board .SumoSelect > .CaptionCont > span.placeholder {\n        background-color: transparent;\n        color: rgb(62 68 76);\n        opacity: 1;\n    }\n}\n\n@media all and (min-width: 768px) {\n    .aa-bulletin-board .cards-equal-height .card-bulletin-excerpt {\n        width: calc(100% / 2);\n    }\n}\n\n@media all and (min-width: 1200px) {\n    .aa-bulletin-board .cards-equal-height .card-bulletin-excerpt {\n        width: calc(100% / 3);\n    }\n}\n\n/* Fix for oEmbed videos\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-bulletin-board figure.media .oembed-video {\n        height: auto;\n        max-width: 100%;\n        overflow: hidden;\n        padding-bottom: 56.25%;\n        position: relative;\n    }\n\n    .aa-bulletin-board figure.media .oembed-video > iframe {\n        height: 100%;\n        left: 0;\n        max-height: 100vh;\n        position: absolute;\n        top: 0;\n        width: 100%;\n    }\n}\n\n/* CKEditor 5 (WYSIWYG editor)\n------------------------------------------------------------------------------------- */\n@media all {\n    .aa-bulletin-board .ck-rounded-corners {\n        --ck-border-radius: var(--bs-border-radius);\n    }\n\n    .aa-bulletin-board .ck-editor__editable {\n        color: initial;\n    }\n\n    .aa-bulletin-board .ck-word-count {\n        color: var(--bs-secondary-color) !important;\n\n        --bs-text-opacity: 1;\n    }\n}\n"
     ],
     "version": 3
 }
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.js` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.js`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.min.js.map` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-equal-height.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.js` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.js`

 * *Files 15% similar despite different names*

#### js-beautify {}

```diff
@@ -1,48 +1,46 @@
-/**
- * Replace oembed YouTube video with an iframe
- *
- * CKEditor5 oembed plugin is used to embed YouTube videos, and browsers cannot render the oembed element.
- * This function replaces the oembed element with an iframe and is using the YouTube-nocookie domain.
- *
- * @param {string} url The YouTube video URL
- * @returns {`<div class="oembed-video youtube-oembed-video"><iframe src="https://www.youtube-nocookie.com/embed/${string}" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`}
- */
-const youtubeOembedToIframe = (url) => {
+$(document).ready(() => {
     'use strict';
 
-    let videoId = url.split('v=')[1];
-    const ampersandPosition = videoId.indexOf('&');
-
-    if (ampersandPosition !== -1) {
-        videoId = videoId.substring(0, ampersandPosition);
-    }
-
-    return `<div class="oembed-video youtube-oembed-video"><iframe src="https://www.youtube-nocookie.com/embed/${videoId}" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`;
-};
+    /**
+     * Replace oembed YouTube video with an iframe
+     *
+     * CKEditor5 oembed plugin is used to embed YouTube videos, and browsers cannot render the oembed element.
+     * This function replaces the oembed element with an iframe and is using the YouTube-nocookie domain.
+     *
+     * @param {string} url The YouTube video URL
+     * @returns {`<div class="oembed-video youtube-oembed-video"><iframe src="${string}" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`}
+     */
+    const youtubeOembedToIframe = (url) => {
+        let videoId = url.split('v=')[1];
+        const ampersandPosition = videoId.indexOf('&');
+        const embedUrl = 'https://www.youtube-nocookie.com/embed/';
 
+        if (ampersandPosition !== -1) {
+            videoId = videoId.substring(0, ampersandPosition);
+        }
 
-/**
- * Look for oembed elements and replace them with iframes
- */
-const checkForOembed = () => {
-    'use strict';
+        const videoUrl = embedUrl + videoId;
 
-    // Find all oembed elements and loop through them
-    $('.ck-content figure.media oembed').each((index, element) => {
-        const source = $(element).attr('url');
-
-        // Check if the source is a YouTube video
-        if (source.includes('youtube.com/watch')) {
-            // Replace the oembed element with an iframe
-            $(element).replaceWith(youtubeOembedToIframe(source));
-        }
-    });
-};
+        return `<div class="oembed-video youtube-oembed-video"><iframe src="${videoUrl}" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe></div>`;
+    };
 
 
-$(document).ready(() => {
-    'use strict';
+    /**
+     * Look for oembed elements and replace them with iframes
+     */
+    const checkForOembed = () => {
+        // Find all oembed elements and loop through them
+        $('.ck-content figure.media oembed').each((index, element) => {
+            const source = $(element).attr('url');
+
+            // Check if the source is a YouTube video
+            if (source.includes('youtube.com/watch')) {
+                // Replace the oembed element with an iframe
+                $(element).replaceWith(youtubeOembedToIframe(source));
+            }
+        });
+    };
 
     // Run the checkForOembed function when the document is ready
     checkForOembed();
 });
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.min.js.map` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/javascript/aa-bulletin-board-oembed.min.js.map`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333333%*

 * *Differences: {"'mappings'": "'AAAAA,EAAEC,QAAQ,EAAEC,MAAM,KACd,aAWA,MAAMC,EAAwB,IAC1BC,IAAIC,EAAUC,EAAIC,MAAM,IAAI,EAAE,GAC9B,MAAMC,EAAoBH,EAAQI,QAAQ,GAAG,EACvCC,EAAW,0CAMXC,GAJoB,CAAC,IAAvBH,IACAH,EAAUA,EAAQO,UAAU,EAAGJ,CAAiB,GAGnCE,EAAWL,GAE5B,qEAAsEM,oHAC1E,EAMME,EAAiB,KAEnBb,EAAE,iCAAiC,EAAEc,KAAK,CAACC,EAAOC,KAC9C,MAAMC,EAASjB,EAAEgB,CAAO,EAAEE,KAAK,KAAK,EAGhCD,EAAOE,SAAS,mBAAmB,GAEnCnB,EAAEgB,CAAO,EAAEI,YAAYjB,EAAsBc,CAAM,CAAC,CAE5D,CAAC,CACL,EAGAJ,EAAe,CACnB,CAAC'",*

 * * "'names'": "{insert: [(0, '$'), (1, 'document' […]*

```diff
@@ -1,28 +1,30 @@
 {
-    "mappings": "AASA,MAAMA,sBAAwB,IAC1B,aAEAC,IAAIC,EAAUC,EAAIC,MAAM,IAAI,EAAE,GAC9B,MAAMC,EAAoBH,EAAQI,QAAQ,GAAG,EAM7C,4GAHIJ,EADsB,CAAC,IAAvBG,EACUH,EAAQK,UAAU,EAAGF,CAAiB,EAGyDH,oHACjH,EAMMM,eAAiB,KACnB,aAGAC,EAAE,iCAAiC,EAAEC,KAAK,CAACC,EAAOC,KAC9C,MAAMC,EAASJ,EAAEG,CAAO,EAAEE,KAAK,KAAK,EAGhCD,EAAOE,SAAS,mBAAmB,GAEnCN,EAAEG,CAAO,EAAEI,YAAYhB,sBAAsBa,CAAM,CAAC,CAE5D,CAAC,CACL,EAGAJ,EAAEQ,QAAQ,EAAEC,MAAM,KACd,aAGAV,eAAe,CACnB,CAAC",
+    "mappings": "AAAAA,EAAEC,QAAQ,EAAEC,MAAM,KACd,aAWA,MAAMC,EAAwB,IAC1BC,IAAIC,EAAUC,EAAIC,MAAM,IAAI,EAAE,GAC9B,MAAMC,EAAoBH,EAAQI,QAAQ,GAAG,EACvCC,EAAW,0CAMXC,GAJoB,CAAC,IAAvBH,IACAH,EAAUA,EAAQO,UAAU,EAAGJ,CAAiB,GAGnCE,EAAWL,GAE5B,qEAAsEM,oHAC1E,EAMME,EAAiB,KAEnBb,EAAE,iCAAiC,EAAEc,KAAK,CAACC,EAAOC,KAC9C,MAAMC,EAASjB,EAAEgB,CAAO,EAAEE,KAAK,KAAK,EAGhCD,EAAOE,SAAS,mBAAmB,GAEnCnB,EAAEgB,CAAO,EAAEI,YAAYjB,EAAsBc,CAAM,CAAC,CAE5D,CAAC,CACL,EAGAJ,EAAe,CACnB,CAAC",
     "names": [
+        "$",
+        "document",
+        "ready",
         "youtubeOembedToIframe",
         "let",
         "videoId",
         "url",
         "split",
         "ampersandPosition",
         "indexOf",
+        "embedUrl",
+        "videoUrl",
         "substring",
         "checkForOembed",
-        "$",
         "each",
         "index",
         "element",
         "source",
         "attr",
         "includes",
-        "replaceWith",
-        "document",
-        "ready"
+        "replaceWith"
     ],
     "sources": [
         "aa-bulletin-board-oembed.js"
     ],
     "version": 3
 }
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.js`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/jquery.sumoselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css` & `aa_bulletin_board-2.0.1/aa_bulletin_board/static/aa_bulletin_board/libs/sumoselect/3.4.8/sumoselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/base.html` & `aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/base.html`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html` & `aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/bulletin.html`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html` & `aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/dashboard.html`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                 <div class="card-bulletin-excerpt col-md-4 mb-4">
                     <div class="card">
                         <div class="card-header">
                             <div class="card-title mb-0 clearfix">
                                 <span>{{ bulletin.title }}</span>
                                 {% if bulletin.groups.all %}
                                     <i
-                                        class="far fa-eye-slash aa-bulletin-board-marker-group-restrictions float-end"
+                                        class="fa-regular fa-eye-slash aa-bulletin-board-marker-group-restrictions float-end"
                                         title="{% blocktranslate count group_count=bulletin.groups.all|length %}This bulletin is restricted to the following group:{% plural %}This bulletin is restricted to the following groups:{% endblocktranslate %}<br>{{ bulletin.groups.all|join:', ' }}"
                                         data-bs-toggle="tooltip"
                                         data-bs-html="true"
                                     ></i>
                                 {% endif %}
                             </div>
                         </div>
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html` & `aa_bulletin_board-2.0.1/aa_bulletin_board/templates/aa_bulletin_board/edit-bulletin.html`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/templatetags/aa_bulletin_board.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/templatetags/aa_bulletin_board.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_access.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_auth_hooks.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_auth_hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             character_id=1002,
             character_name="Bruce Wayne",
             permissions=["aa_bulletin_board.basic_access"],
         )
 
         cls.html_menu = f"""
             <li class="d-flex flex-wrap m-2 p-2 pt-0 pb-0 mt-0 mb-0 me-0 pe-0">
-                <i class="nav-link fas fa-clipboard-list fa-fw align-self-center me-3 "></i>
+                <i class="nav-link fa-solid fa-clipboard-list fa-fw align-self-center me-3 "></i>
                 <a class="nav-link flex-fill align-self-center me-auto" href="{reverse(viewname='aa_bulletin_board:dashboard')}">
                     Bulletin Board
                 </a>
             </li>
         """
 
     def login(self, user):
```

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_bulletins.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_bulletins.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_templatetags.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/test_user_interface.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/tests/test_user_interface.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/aa_bulletin_board/tests/utils.py` & `aa_bulletin_board-2.0.1/aa_bulletin_board/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/LICENSE` & `aa_bulletin_board-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_bulletin_board-2.0.0b1/README.md` & `aa_bulletin_board-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Simple bulletin board for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
 ______________________________________________________________________
 
 <!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=1 -->
 
 - [AA Bulletin Board](#aa-bulletin-board)
-  - [⚠️ Before You Install This Module ⚠️](#%E2%9A%A0%EF%B8%8F-before-you-install-this-module-%E2%9A%A0%EF%B8%8F)
+  - [Before You Install This Module](#before-you-install-this-module)
   - [Installation](#installation)
     - [Step 1: Install the Package](#step-1-install-the-package)
     - [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
       - [Settings in `/home/allianceserver/myauth/myauth/settings/local.py`](#settings-in-homeallianceservermyauthmyauthsettingslocalpy)
       - [Settings in `/home/allianceserver/myauth/myauth/urls.py`](#settings-in-homeallianceservermyauthmyauthurlspy)
     - [Step 3: Configure Your Webserver](#step-3-configure-your-webserver)
       - [Apache](#apache)
@@ -40,30 +40,32 @@
 
 <!-- mdformat-toc end -->
 
 ______________________________________________________________________
 
 ![AA Bulletin Board](https://raw.githubusercontent.com/ppfeufer/aa-bulletin-board/master/docs/images/presentation/aa-bulletin-board.jpg "AA Bulletin Board")
 
-## ⚠️ Before You Install This Module ⚠️<a name="%E2%9A%A0%EF%B8%8F-before-you-install-this-module-%E2%9A%A0%EF%B8%8F"></a>
+## Before You Install This Module<a name="before-you-install-this-module"></a>
 
 This app needs quite some configuration done before working properly. You need to
 modify your Apache/Nginx configuration as well as the global URL config of Alliance
 Auth. So please only install if you know what you're doing/feel comfortable to make
 these kinds of changes. For your own sanity, and mine :-)
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Bulletin Board needs at least Alliance Auth v4.0.0!**
+> **AA Bulletin Board >=2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.13.2`.
 
 **Important**: Please make sure you meet all preconditions before you proceed:
 
 - AA Bulletin Board is a plugin for Alliance Auth. If you don't have Alliance Auth
   running already, please install it first before proceeding. (see the official
   [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
   or details)
@@ -91,16 +93,16 @@
 INSTALLED_APPS += [
     "django_ckeditor_5",  # https://github.com/hvlads/django-ckeditor-5
     "aa_bulletin_board",  # https://github.com/ppfeufer/aa-bulletin-board
 ]
 
 # Django CKEditor 5 Configuration
 if "django_ckeditor_5" in INSTALLED_APPS:
-    MEDIA_URL = "/media/"
-    MEDIA_ROOT = os.path.join(BASE_DIR, "media/uploads")
+    MEDIA_URL = "/media/uploads/"
+    MEDIA_ROOT = "/var/www/myauth/media/uploads"
 
     customColorPalette = [
         {"color": "hsl(4, 90%, 58%)", "label": "Red"},
         {"color": "hsl(340, 82%, 52%)", "label": "Pink"},
         {"color": "hsl(291, 64%, 42%)", "label": "Purple"},
         {"color": "hsl(262, 52%, 47%)", "label": "Deep Purple"},
         {"color": "hsl(231, 48%, 48%)", "label": "Indigo"},
@@ -245,14 +247,15 @@
 you need to open `/home/allianceserver/myauth/myauth/urls.py` and change the
 following block right before the `handler` definitions:
 
 ```python
 from django.apps import apps  # Only if not already imported earlier
 from django.conf import settings  # Only if not already imported earlier
 from django.conf.urls.static import static  # Only if not already imported earlier
+from django.urls import path  # Only if not already imported earlier
 
 # If django_ckeditor_5 is loaded
 if apps.is_installed("django_ckeditor_5"):
     # URL configuration for CKEditor 5
     urlpatterns = (
         [
             path(
@@ -267,22 +270,22 @@
 ```
 
 After this, your `urls.py` should look similar to this:
 
 ```python
 from django.apps import apps
 from django.conf import settings
-from django.urls import include, re_path
 from django.conf.urls.static import static
+from django.urls import include, path, re_path
 
 from allianceauth import urls
 
 # Alliance auth urls
 urlpatterns = [
-    re_path(r"", include(urls)),
+    path(r"", include(urls)),
 ]
 
 # If django_ckeditor_5 is loaded
 if apps.is_installed("django_ckeditor_5"):
     # URL configuration for CKEditor 5
     urlpatterns = (
         [
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_bulletin_board-2.0.0b1/pyproject.toml` & `aa_bulletin_board-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

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
     "allianceauth-app-utils>=1.19.1",
     "django-ckeditor-5>=0.2.11",
     "unidecode",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
     "coverage",
```

### Comparing `aa_bulletin_board-2.0.0b1/PKG-INFO` & `aa_bulletin_board-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aa-bulletin-board
-Version: 2.0.0b1
+Version: 2.0.1
 Summary: A simple bulletin board for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-bulletin-board/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-bulletin-board/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-bulletin-board
 Project-URL: Source, https://github.com/ppfeufer/aa-bulletin-board.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-bulletin-board/issues
@@ -698,15 +698,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.19.1
-Requires-Dist: allianceauth>=4.0.0b1
+Requires-Dist: allianceauth<5.0.0,>=4
 Requires-Dist: django-ckeditor-5>=0.2.11
 Requires-Dist: unidecode
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Requires-Dist: faker; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
@@ -731,15 +731,15 @@
 Simple bulletin board for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth)
 
 ______________________________________________________________________
 
 <!-- mdformat-toc start --slug=github --maxlevel=6 --minlevel=1 -->
 
 - [AA Bulletin Board](#aa-bulletin-board)
-  - [⚠️ Before You Install This Module ⚠️](#%E2%9A%A0%EF%B8%8F-before-you-install-this-module-%E2%9A%A0%EF%B8%8F)
+  - [Before You Install This Module](#before-you-install-this-module)
   - [Installation](#installation)
     - [Step 1: Install the Package](#step-1-install-the-package)
     - [Step 2: Configure Alliance Auth](#step-2-configure-alliance-auth)
       - [Settings in `/home/allianceserver/myauth/myauth/settings/local.py`](#settings-in-homeallianceservermyauthmyauthsettingslocalpy)
       - [Settings in `/home/allianceserver/myauth/myauth/urls.py`](#settings-in-homeallianceservermyauthmyauthurlspy)
     - [Step 3: Configure Your Webserver](#step-3-configure-your-webserver)
       - [Apache](#apache)
@@ -753,30 +753,32 @@
 
 <!-- mdformat-toc end -->
 
 ______________________________________________________________________
 
 ![AA Bulletin Board](https://raw.githubusercontent.com/ppfeufer/aa-bulletin-board/master/docs/images/presentation/aa-bulletin-board.jpg "AA Bulletin Board")
 
-## ⚠️ Before You Install This Module ⚠️<a name="%E2%9A%A0%EF%B8%8F-before-you-install-this-module-%E2%9A%A0%EF%B8%8F"></a>
+## Before You Install This Module<a name="before-you-install-this-module"></a>
 
 This app needs quite some configuration done before working properly. You need to
 modify your Apache/Nginx configuration as well as the global URL config of Alliance
 Auth. So please only install if you know what you're doing/feel comfortable to make
 these kinds of changes. For your own sanity, and mine :-)
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Bulletin Board needs at least Alliance Auth v4.0.0!**
+> **AA Bulletin Board >=2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.13.2`.
 
 **Important**: Please make sure you meet all preconditions before you proceed:
 
 - AA Bulletin Board is a plugin for Alliance Auth. If you don't have Alliance Auth
   running already, please install it first before proceeding. (see the official
   [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html)
   or details)
@@ -804,16 +806,16 @@
 INSTALLED_APPS += [
     "django_ckeditor_5",  # https://github.com/hvlads/django-ckeditor-5
     "aa_bulletin_board",  # https://github.com/ppfeufer/aa-bulletin-board
 ]
 
 # Django CKEditor 5 Configuration
 if "django_ckeditor_5" in INSTALLED_APPS:
-    MEDIA_URL = "/media/"
-    MEDIA_ROOT = os.path.join(BASE_DIR, "media/uploads")
+    MEDIA_URL = "/media/uploads/"
+    MEDIA_ROOT = "/var/www/myauth/media/uploads"
 
     customColorPalette = [
         {"color": "hsl(4, 90%, 58%)", "label": "Red"},
         {"color": "hsl(340, 82%, 52%)", "label": "Pink"},
         {"color": "hsl(291, 64%, 42%)", "label": "Purple"},
         {"color": "hsl(262, 52%, 47%)", "label": "Deep Purple"},
         {"color": "hsl(231, 48%, 48%)", "label": "Indigo"},
@@ -958,14 +960,15 @@
 you need to open `/home/allianceserver/myauth/myauth/urls.py` and change the
 following block right before the `handler` definitions:
 
 ```python
 from django.apps import apps  # Only if not already imported earlier
 from django.conf import settings  # Only if not already imported earlier
 from django.conf.urls.static import static  # Only if not already imported earlier
+from django.urls import path  # Only if not already imported earlier
 
 # If django_ckeditor_5 is loaded
 if apps.is_installed("django_ckeditor_5"):
     # URL configuration for CKEditor 5
     urlpatterns = (
         [
             path(
@@ -980,22 +983,22 @@
 ```
 
 After this, your `urls.py` should look similar to this:
 
 ```python
 from django.apps import apps
 from django.conf import settings
-from django.urls import include, re_path
 from django.conf.urls.static import static
+from django.urls import include, path, re_path
 
 from allianceauth import urls
 
 # Alliance auth urls
 urlpatterns = [
-    re_path(r"", include(urls)),
+    path(r"", include(urls)),
 ]
 
 # If django_ckeditor_5 is loaded
 if apps.is_installed("django_ckeditor_5"):
     # URL configuration for CKEditor 5
     urlpatterns = (
         [
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

