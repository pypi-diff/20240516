# Comparing `tmp/aa_forum-2.2.0.tar.gz` & `tmp/aa_forum-2.2.1.tar.gz`

## Comparing `aa_forum-2.2.0.tar` & `aa_forum-2.2.1.tar`

### file list

```diff
@@ -1,218 +1,221 @@
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/__init__.py
--rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/admin.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/app_settings.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/apps.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/auth_hooks.py
--rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/constants.py
--rw-r--r--   0        0        0    19631 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/forms.py
--rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/managers.py
--rw-r--r--   0        0        0    30251 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/models.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/signals.py
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/urls.py
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/helper/discord_messages.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/helper/eve_images.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/helper/forms.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/helper/pagination.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/helper/text.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/helper/user.py
--rw-r--r--   0        0        0    39481 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/django.pot
--rw-r--r--   0        0        0    39556 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    28897 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    52203 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    44946 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40664 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39660 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39532 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    41205 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    39473 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39830 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    58050 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    39551 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    40498 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    39849 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0001_initial.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0002_default_settings.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0003_board_discord_webhook.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0005_announcement_boards.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0006_reset_default_settings.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0007_change_settings_to_singleton.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0008_populate_default_settings.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0009_add_related_names.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0010_better_setting_names.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0011_userprofile.py
--rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0012_personal_messages.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0014_userprofile_discord_dm_on_new_personal_message.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0016_fix_quotation_marks.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/migrations/__init__.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/scripts/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/scripts/drop_tables.sql
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/scripts/fake_messages.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/LICENSE
--rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-cs.json
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-de.json
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-en.json
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-es.json
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-fr.json
--rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-it.json
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-ja.json
--rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-ko.json
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-nl.json
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-pl.json
--rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-ru.json
--rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-sk.json
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-uk.json
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-zh.json
--rw-r--r--   0        0        0    13668 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/css/aa-forum.css
--rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/css/aa-forum.min.css
--rw-r--r--   0        0        0    16294 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/css/aa-forum.min.css.map
--rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.js
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js.map
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js.map
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js
--rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md
--rw-r--r--   0        0        0    18931 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css
--rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css
--rw-r--r--   0        0        0   167106 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js
--rw-r--r--   0        0        0    76775 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js
--rw-r--r--   0        0        0   156955 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js
--rw-r--r--   0        0        0    73170 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE
--rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css
--rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css
--rw-r--r--   0        0        0    38867 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map
--rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js
--rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
--rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css
--rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/base.html
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/aa-forum-admin-js.html
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/aa-forum-bootstrap-js.html
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/aa-forum-ckeditor-js.html
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/aa-forum-css.html
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/aa-forum-dashboard-widgets-js.html
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/aa-forum-oembed-js.html
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/aa-forum-personal-messages-js.html
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/ckeditor5-css.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/ckeditor5-js.html
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/select2-css.html
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/select2-js.html
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/sumoselect-css.html
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/sumoselect-js.html
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
--rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/breadcrumb.html
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/menu.html
--rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/categories.html
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/new-category.html
--rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/settings-form.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/forum-index.html
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/board.html
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
--rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
--rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
--rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/menu/menu-admin.html
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/menu/menu-user.html
--rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html
--rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html
--rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/profile/form.html
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/search/pagination.html
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/search/search-form.html
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/search/search-result.html
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/widgets/unread-topics.html
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/administration/forum-settings.html
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/board.html
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/index.html
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/modify-message.html
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/new-topic.html
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/topic.html
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/personal-messages/inbox.html
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/personal-messages/new-message.html
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/profile/index.html
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/search/results.html
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templatetags/__init__.py
--rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/templatetags/aa_forum.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_app_settings.py
--rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_auth_hooks.py
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_helpers.py
--rw-r--r--   0        0        0    74867 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_integration.py
--rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_managers.py
--rw-r--r--   0        0        0    36507 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_models.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_signals.py
--rw-r--r--   0        0        0    29431 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_templatetags.py
--rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_views_admin.py
--rw-r--r--   0        0        0    51417 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/test_views_forum.py
--rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/tests/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/views/__init__.py
--rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/views/admin.py
--rw-r--r--   0        0        0    44779 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/views/forum.py
--rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/views/personal_messages.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/views/profile.py
--rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/views/search.py
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_forum-2.2.0/aa_forum/views/widgets.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_forum-2.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_forum-2.2.0/LICENSE
--rw-r--r--   0        0        0    20310 2020-02-02 00:00:00.000000 aa_forum-2.2.0/README.md
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 aa_forum-2.2.0/pyproject.toml
--rw-r--r--   0        0        0    63005 2020-02-02 00:00:00.000000 aa_forum-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/__init__.py
+-rw-r--r--   0        0        0     4129 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/admin.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/app_settings.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/apps.py
+-rw-r--r--   0        0        0     2536 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/auth_hooks.py
+-rw-r--r--   0        0        0     1579 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/constants.py
+-rw-r--r--   0        0        0    19631 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/forms.py
+-rw-r--r--   0        0        0     8652 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/managers.py
+-rw-r--r--   0        0        0    30251 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/models.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/signals.py
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/urls.py
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/discord_messages.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/eve_images.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/forms.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/pagination.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/text.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/helper/user.py
+-rw-r--r--   0        0        0    39481 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/django.pot
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39697 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    28897 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    52203 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    44964 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40657 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39666 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39532 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    41206 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39560 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1052 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39856 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    58064 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39693 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    40504 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    39847 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    12997 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0002_default_settings.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0003_board_discord_webhook.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0004_board_use_webhook_for_replies.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0005_announcement_boards.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0006_reset_default_settings.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0007_change_settings_to_singleton.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0008_populate_default_settings.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0009_add_related_names.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0010_better_setting_names.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0011_userprofile.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0012_personal_messages.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0014_userprofile_discord_dm_on_new_personal_message.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0016_fix_quotation_marks.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/migrations/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/scripts/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/scripts/drop_tables.sql
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/scripts/fake_messages.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/LICENSE
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-cs.json
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-de.json
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-en.json
+-rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-es.json
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-fr.json
+-rw-r--r--   0        0        0     5380 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-it.json
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ja.json
+-rw-r--r--   0        0        0     7894 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ko.json
+-rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-nl.json
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-pl.json
+-rw-r--r--   0        0        0     7350 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ru.json
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-sk.json
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-uk.json
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-zh.json
+-rw-r--r--   0        0        0    13668 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.css
+-rw-r--r--   0        0        0     7532 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.min.css
+-rw-r--r--   0        0        0    16294 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.min.css.map
+-rw-r--r--   0        0        0     7385 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.js
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.js
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-bootstrap.min.js.map
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.js
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-ckeditor.min.js.map
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js
+-rw-r--r--   0        0        0     1339 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md
+-rw-r--r--   0        0        0    18931 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css
+-rw-r--r--   0        0        0    16264 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css
+-rw-r--r--   0        0        0   167106 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js
+-rw-r--r--   0        0        0    76775 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js
+-rw-r--r--   0        0        0   156955 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js
+-rw-r--r--   0        0        0    73170 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE
+-rw-r--r--   0        0        0    34395 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css
+-rw-r--r--   0        0        0    29738 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css
+-rw-r--r--   0        0        0    38867 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map
+-rw-r--r--   0        0        0    34280 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js
+-rw-r--r--   0        0        0    22226 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js
+-rw-r--r--   0        0        0     9711 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css
+-rw-r--r--   0        0        0     7610 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/base.html
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-admin-js.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-bootstrap-js.html
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-ckeditor-js.html
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-css.html
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-dashboard-widgets-js.html
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-oembed-js.html
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/aa-forum-personal-messages-js.html
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/ckeditor5-css.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/ckeditor5-js.html
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/select2-css.html
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/select2-js.html
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/sumoselect-css.html
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/sumoselect-js.html
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/administration/delete-board.html
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/administration/delete-category.html
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html
+-rw-r--r--   0        0        0     2177 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/breadcrumb.html
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu.html
+-rw-r--r--   0        0        0     5941 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/board-loop.html
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/categories.html
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/category-loop.html
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/new-category.html
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/settings-form.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/form/required-field-hint.html
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/forum-index.html
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/mark-unread-button.html
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/board-index.html
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/board.html
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/new-topic-button.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/no-access.html
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/pagination.html
+-rw-r--r--   0        0        0     5965 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/topic.html
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html
+-rw-r--r--   0        0        0     5453 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/message.html
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html
+-rw-r--r--   0        0        0     4143 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/reply.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu/menu-admin.html
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu/menu-user.html
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html
+-rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html
+-rw-r--r--   0        0        0     2094 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html
+-rw-r--r--   0        0        0     4766 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html
+-rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/profile/form.html
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/pagination.html
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/search-form.html
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/search-result.html
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/widgets/unread-topics.html
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/administration/forum-settings.html
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/board.html
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/index.html
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/modify-message.html
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/modify-topic.html
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/new-topic.html
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/topic.html
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/unread-topics.html
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/inbox.html
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/new-message.html
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/profile/index.html
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/search/results.html
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templatetags/__init__.py
+-rw-r--r--   0        0        0     9950 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/templatetags/aa_forum.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_app_settings.py
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_helpers.py
+-rw-r--r--   0        0        0    74867 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_integration.py
+-rw-r--r--   0        0        0     7246 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_managers.py
+-rw-r--r--   0        0        0    36507 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_models.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_signals.py
+-rw-r--r--   0        0        0    29431 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_templatetags.py
+-rw-r--r--   0        0        0     8057 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_views_admin.py
+-rw-r--r--   0        0        0    51417 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/test_views_forum.py
+-rw-r--r--   0        0        0     7082 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/tests/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/__init__.py
+-rw-r--r--   0        0        0    18371 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/admin.py
+-rw-r--r--   0        0        0    44779 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/forum.py
+-rw-r--r--   0        0        0    13162 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/personal_messages.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/profile.py
+-rw-r--r--   0        0        0     2989 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/search.py
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 aa_forum-2.2.1/aa_forum/views/widgets.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_forum-2.2.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_forum-2.2.1/LICENSE
+-rw-r--r--   0        0        0    20310 2020-02-02 00:00:00.000000 aa_forum-2.2.1/README.md
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 aa_forum-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0    63005 2020-02-02 00:00:00.000000 aa_forum-2.2.1/PKG-INFO
```

### Comparing `aa_forum-2.2.0/aa_forum/admin.py` & `aa_forum-2.2.1/aa_forum/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/app_settings.py` & `aa_forum-2.2.1/aa_forum/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/apps.py` & `aa_forum-2.2.1/aa_forum/apps.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/auth_hooks.py` & `aa_forum-2.2.1/aa_forum/auth_hooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,17 +67,17 @@
 
             # Render the menu item
             return MenuItemHook.render(self, request=request)
 
         return ""
 
 
-class UnreadTopicsDashboardHook(DashboardItemHook):
+class AaForumDashboardWidgets(DashboardItemHook):
     """
-    This class adds the unread topics widget to the Alliance Auth dashboard
+    This class adds the AA Forum dashboard widgets to the Alliance Auth dashboard.
     """
 
     def __init__(self):
         # Setup dashboard widget
         DashboardItemHook.__init__(self=self, view_function=dashboard_widgets, order=5)
 
 
@@ -102,16 +102,16 @@
     :rtype:
     """
 
     return UrlHook(urls=urls, namespace="aa_forum", base_url=r"^forum/")
 
 
 @hooks.register("dashboard_hook")
-def register_esi_hook():
+def register_dashboard_widgets():
     """
     Register our dashboard hook
 
     :return: The hook
-    :rtype: UnreadTopicsDashboardHook
+    :rtype: AaForumDashboardWidgets
     """
 
-    return UnreadTopicsDashboardHook()
+    return AaForumDashboardWidgets()
```

### Comparing `aa_forum-2.2.0/aa_forum/constants.py` & `aa_forum-2.2.1/aa_forum/constants.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/forms.py` & `aa_forum-2.2.1/aa_forum/forms.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/managers.py` & `aa_forum-2.2.1/aa_forum/managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/models.py` & `aa_forum-2.2.1/aa_forum/models.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/signals.py` & `aa_forum-2.2.1/aa_forum/signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/urls.py` & `aa_forum-2.2.1/aa_forum/urls.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/helper/discord_messages.py` & `aa_forum-2.2.1/aa_forum/helper/discord_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/helper/eve_images.py` & `aa_forum-2.2.1/aa_forum/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/helper/forms.py` & `aa_forum-2.2.1/aa_forum/helper/forms.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/helper/pagination.py` & `aa_forum-2.2.1/aa_forum/helper/pagination.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/helper/text.py` & `aa_forum-2.2.1/aa_forum/helper/text.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/helper/user.py` & `aa_forum-2.2.1/aa_forum/helper/user.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/locale/django.pot` & `aa_forum-2.2.1/aa_forum/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/locale/cs/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/cs/LC_MESSAGES/django.po`

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
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Czech <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
 "<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
@@ -691,14 +692,16 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
@@ -1028,14 +1031,16 @@
 
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/de/LC_MESSAGES/django.mo` & `aa_forum-2.2.1/aa_forum/locale/de/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-forum/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] "%(counter)s Resultat"
 msgstr[1] "%(counter)s Resultate"
 
 msgid ""
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/de/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 # Peter Pfeufer, 2022
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2024-04-04 07:56+0000\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-forum/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
@@ -1169,31 +1169,31 @@
 msgid "<h4>Success!</h4><p>Settings updated.</p>"
 msgstr "<h4>Erfolg!</h4><p>Einstellungen aktualisiert.</p>"
 
 #: aa_forum/views/admin.py:597 aa_forum/views/personal_messages.py:122
 #: aa_forum/views/personal_messages.py:249 aa_forum/views/profile.py:70
 msgid "<h4>Error!</h4><p>Something went wrong, please check your input.</p>"
 msgstr ""
-"<h4>Fehler!</h4><p>Etwas ist schief gelaufen, bitte überprüfe Deine Eingabe."
-"</p>"
+"<h4>Fehler!</h4><p>Etwas ist schief gelaufen, bitte überprüfe Deine "
+"Eingabe.</p>"
 
 #: aa_forum/views/forum.py:232
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to visit does either not exist, "
 "or you don't have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Board, das Du aufrufen willst, existiert entweder "
 "nicht oder Du hast keinen Zugriff darauf.</p>"
 
 #: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
-"<h4>Fehler!</h4><p>Die Kategorie, in der Du posten willst, existiert nicht.</"
-"p>"
+"<h4>Fehler!</h4><p>Die Kategorie, in der Du posten willst, existiert "
+"nicht.</p>"
 
 #: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 "<h4>Fehler!</h4><p>Das Board, in dem Du posten willst, existiert entweder "
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/es/LC_MESSAGES/django.mo` & `aa_forum-2.2.1/aa_forum/locale/es/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-forum/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Boards"
 msgstr "Tableros"
 
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/es/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
-# Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
+# Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023, 2024.
 # Mak3rco <depormanuf1@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2024-04-08 17:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Mak3rco <depormanuf1@gmail.com>\n"
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-forum/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_forum-2.2.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-forum/fr/>\n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "AA Forum v{__version__}"
 msgstr "AA Forum v{__version__}"
 
 msgid "Category name"
 msgstr "Nom de la catégorie"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/fr_FR/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 # Matthias P <randomusernetcom@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2024-04-17 23:13+0000\n"
-"Last-Translator: Matthias P <randomusernetcom@gmail.com>\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: French <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-forum/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/it_IT/LC_MESSAGES/django.mo` & `aa_forum-2.2.1/aa_forum/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,14 +7,14 @@
 "Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-forum/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Fields marked with an asterisk (*) are mandatory"
 msgstr "I campi contrassegnati da un asterisco (*) sono obbligatori"
 
 msgid "This field is mandatory"
 msgstr "Questo campo è obbligatorio"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/it_IT/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

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
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2023-10-02 09:34+0000\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-forum/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/ja/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2023-10-02 09:34+0000\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-forum/ja/>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_forum-2.2.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-forum/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "AA Forum v{__version__}"
 msgstr "AA 포럼 v{__version__}"
 
 msgid "Board description (optional)"
 msgstr "게시판 설명(선택사항)"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/ko_KR/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Author50CO <tkddlschry@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Author50CO <tkddlschry@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 # Mind of the Raven <okanieva@gmail.com>, 2024.
 # Rodpold Shard <rodpold@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2024-03-21 17:11+0000\n"
-"Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-forum/ko/>\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
+"Last-Translator: Rodpold Shard <rodpold@gmail.com>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
@@ -75,16 +75,16 @@
 msgstr "게시판"
 
 #: aa_forum/forms.py:198
 msgid ""
 "Boards to be created with this category (One board per line). These boards "
 "will have no group restrictions, so you have to add them later where needed."
 msgstr ""
-"이 카테고리로(한 줄당 한 게시판) 게시판이 생성됩니다. 이 게시판은 그룹 제한"
-"이 없기 때문에 필요하면 나중에 추가할 수 있습니다."
+"이 카테고리로(한 줄당 한 게시판) 게시판이 생성됩니다. 이 게시판은 그룹 "
+"제한이 없기 때문에 필요하면 나중에 추가할 수 있습니다."
 
 #: aa_forum/forms.py:251
 msgid "Board name"
 msgstr "게시판 이름"
 
 #: aa_forum/forms.py:255
 msgid "Description"
@@ -100,16 +100,16 @@
 
 #: aa_forum/forms.py:269
 msgid ""
 "This will restrict access to this board to the selected groups. If no groups "
 "are selected, everyone who can access the forum can also access this board. "
 "(This setting is optional)"
 msgstr ""
-"이렇게 진행할 경우 게시판 접근 권한이 선택한 그룹으로 제한됩니다. 선택하지 않"
-"을 경우 모든 사람이 이 게시판에 접근할 수 있습니다. (선택사항)"
+"이렇게 진행할 경우 게시판 접근 권한이 선택한 그룹으로 제한됩니다. 선택하지 "
+"않을 경우 모든 사람이 이 게시판에 접근할 수 있습니다. (선택사항)"
 
 #: aa_forum/forms.py:277
 msgid "Discord webhook (optional)"
 msgstr ""
 
 #: aa_forum/forms.py:279
 msgid ""
@@ -122,16 +122,15 @@
 msgstr ""
 
 #: aa_forum/forms.py:294
 msgid ""
 "When activated every reply to any topic in this board will be posted to the "
 "defined Discord channel. (Child boards are excluded) Chose wisely! (Default: "
 "NO)"
-msgstr ""
-"활성화할 경우 이 게시판 내 모든 게시글의 모든 답변이 정의된 디스코드 채널에 "
+msgstr "활성화할 경우 이 게시판 내 모든 게시글의 모든 답변이 정의된 디스코드 채널에 "
 "게시됩니다. (기본값:꺼짐)"
 
 #: aa_forum/forms.py:302
 msgid "Mark board as \"Announcement Board\""
 msgstr "선택된 게시글을 공지사항으로 등록"
 
 #: aa_forum/forms.py:304
@@ -870,17 +869,16 @@
 msgstr "편집일:"
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:14
 #: aa_forum/templates/aa_forum/partials/forum/topic/reply.html:15
 msgid ""
 "Note: You are not on the last page of this topic and may miss the most "
 "recent replies."
-msgstr ""
-"참고 : 현재 이 게시글의 마지막 페이지에 있지 않음으로 최신 답글을 놓칠 수 있"
-"습니다."
+msgstr "참고 : 현재 이 게시글의 마지막 페이지에 있지 않음으로 최신 답글을 놓칠 수 "
+"있습니다."
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html:27
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:21
 msgid "Modify"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html:7
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/nl/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/nl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,27 @@
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
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo` & `aa_forum-2.2.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-forum/pl/>\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Delete"
 msgstr "Usuń"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/pl_PL/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2024-04-01 09:51+0000\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Polish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-forum/pl/>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/pl/>\n"
 "Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
 "|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
@@ -693,14 +693,15 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
@@ -1030,14 +1031,15 @@
 
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/ru/LC_MESSAGES/django.mo` & `aa_forum-2.2.1/aa_forum/locale/ru/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-forum/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] "%(counter)s Результат"
 msgstr[1] "%(counter)s Результата"
 msgstr[2] "%(counter)s Результатов"
 msgstr[3] "%(counter)s Результатов"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/ru/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
-# Nikolay <nick.postnikov@gmail.com>, 2023.
-# Max <mark25@inbox.ru>, 2023.
+# Nikolay <nick.postnikov@gmail.com>, 2023, 2024.
+# Max <mark25@inbox.ru>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2024-03-21 17:11+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-forum/ru/>\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
@@ -355,16 +355,17 @@
 #: aa_forum/models.py:394
 #, python-brace-format
 msgid ""
 "<h4>Warning!</h4><p>There is already a topic with the exact same subject in "
 "this board.</p><p>See here: <a href=\"{self.topic_url}\">{self._topic."
 "subject}</a></p>"
 msgstr ""
-"<h4>Предупреждение!</h4><p>На доске уже есть тема с таким же названием.</"
-"p><p>См.: <a href=\"{self.topic_url}\">{self._topic.subject}</a></p>"
+"<h4>Предупреждение!</h4><p>На доске уже есть тема с таким же "
+"названием.</p><p>См.: <a href=\"{self.topic_url}\">{self._topic."
+"subject}</a></p>"
 
 #: aa_forum/models.py:625
 msgid "topic"
 msgstr "тема"
 
 #: aa_forum/models.py:626
 msgid "topics"
@@ -1160,16 +1161,16 @@
 "<h4>Ошибка!</h4><p>Доска, на которую вы пытаетесь попасть, не существует или "
 "Вам не доступна.</p>"
 
 #: aa_forum/views/forum.py:293
 msgid ""
 "<h4>Error!</h4><p>The category you were trying to post in does not exist.</p>"
 msgstr ""
-"<h4>Ошибка!</h4><p>Категория, в которую в попытались написать, не существует."
-"</p>"
+"<h4>Ошибка!</h4><p>Категория, в которую в попытались написать, не "
+"существует.</p>"
 
 #: aa_forum/views/forum.py:320
 msgid ""
 "<h4>Error!</h4><p>The board you were trying to post in does either not "
 "exist, or you don't have access to it.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Доска, на которую вы пытаетесь написать, не существует "
@@ -1302,16 +1303,16 @@
 "<h4>Успех!</h4><p>Сообщение удалено.</p><p>Это было стартовое сообщение "
 "темы, так что вся тема также удалена.</p>"
 
 #: aa_forum/views/personal_messages.py:110
 #, python-brace-format
 msgid "<h4>Success!</h4><p>Message to {recipient_main_char} sent.</p>"
 msgstr ""
-"<h4>Успех!</h4><p>Сообщение пользователю {recipient_main_char} отправлено.</"
-"p>"
+"<h4>Успех!</h4><p>Сообщение пользователю {recipient_main_char} "
+"отправлено.</p>"
 
 #: aa_forum/views/personal_messages.py:202
 msgid ""
 "<h4>Error!</h4><p>The message you were trying to reply to does either not "
 "exist or you are not the recipient.</p>"
 msgstr ""
 "<h4>Ошибка!</h4><p>Сообщение, на которое Вы пытаетесь ответить, не "
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/sk/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/sk/LC_MESSAGES/django.po`

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
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
 ">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
@@ -691,14 +692,16 @@
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:33
 msgid "This board is restricted to the following group:"
 msgid_plural "This board is restricted to the following groups:"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:41
 msgid "Child boards:"
 msgstr ""
 
 #: aa_forum/templates/aa_forum/partials/forum/board/board.html:50
 #: aa_forum/templates/aa_forum/partials/forum/board/topic.html:29
@@ -1028,14 +1031,16 @@
 
 #: aa_forum/templates/aa_forum/view/search/results.html:21
 #, python-format
 msgid "%(counter)s Result"
 msgid_plural "%(counter)s Results"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aa_forum/templates/aa_forum/view/search/results.html:31
 msgid "Nothing found …"
 msgstr ""
 
 #: aa_forum/templatetags/aa_forum.py:111
 msgid "Timezone conversion"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/uk/LC_MESSAGES/django.mo` & `aa_forum-2.2.1/aa_forum/locale/uk/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-forum/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Boards"
 msgstr "Дошки"
 
 msgid "Delete"
 msgstr "Видалити"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/uk/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/uk/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# "Andrii M." <elfleg0las88@gmail.com>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# "Andrii M." <elfleg0las88@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2023-10-02 09:34+0000\n"
-"Last-Translator: \"Andrii M.\" <elfleg0las88@gmail.com>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-forum/uk/>\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-forum/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_forum-2.2.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-forum/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Cancel"
 msgstr "取消"
 
 msgid "Category name"
 msgstr "分类名称"
```

### Comparing `aa_forum-2.2.0/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_forum-2.2.1/aa_forum/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # Dehao Wu <wudehao2000@163.com>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-04-03 14:16+0200\n"
-"PO-Revision-Date: 2024-03-22 12:56+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"PO-Revision-Date: 2024-05-10 14:06+0000\n"
+"Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-forum/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_forum/__init__.py:9 aa_forum/templates/aa_forum/base.html:6
 #: aa_forum/templates/aa_forum/base.html:10
 #: aa_forum/templates/aa_forum/view/administration/categories-and-boards.html:7
 #: aa_forum/templates/aa_forum/view/administration/forum-settings.html:7
 #: aa_forum/templates/aa_forum/view/forum/board.html:6
 #: aa_forum/templates/aa_forum/view/forum/index.html:7
```

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0001_initial.py` & `aa_forum-2.2.1/aa_forum/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0002_default_settings.py` & `aa_forum-2.2.1/aa_forum/migrations/0002_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0004_board_use_webhook_for_replies.py` & `aa_forum-2.2.1/aa_forum/migrations/0004_board_use_webhook_for_replies.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0005_announcement_boards.py` & `aa_forum-2.2.1/aa_forum/migrations/0005_announcement_boards.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0006_reset_default_settings.py` & `aa_forum-2.2.1/aa_forum/migrations/0006_reset_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0007_change_settings_to_singleton.py` & `aa_forum-2.2.1/aa_forum/migrations/0007_change_settings_to_singleton.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0008_populate_default_settings.py` & `aa_forum-2.2.1/aa_forum/migrations/0008_populate_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0009_add_related_names.py` & `aa_forum-2.2.1/aa_forum/migrations/0009_add_related_names.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0010_better_setting_names.py` & `aa_forum-2.2.1/aa_forum/migrations/0010_better_setting_names.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0011_userprofile.py` & `aa_forum-2.2.1/aa_forum/migrations/0011_userprofile.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0012_personal_messages.py` & `aa_forum-2.2.1/aa_forum/migrations/0012_personal_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py` & `aa_forum-2.2.1/aa_forum/migrations/0013_personal_messages_migrate_zero_fix.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py` & `aa_forum-2.2.1/aa_forum/migrations/0015_alter_board_use_webhook_for_replies.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0016_fix_quotation_marks.py` & `aa_forum-2.2.1/aa_forum/migrations/0016_fix_quotation_marks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py` & `aa_forum-2.2.1/aa_forum/migrations/0017_ckeditor5_and_dashboard_widgets.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/scripts/drop_tables.sql` & `aa_forum-2.2.1/aa_forum/scripts/drop_tables.sql`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/scripts/fake_messages.py` & `aa_forum-2.2.1/aa_forum/scripts/fake_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/LICENSE` & `aa_forum-2.2.1/aa_forum/search/stopwords/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-cs.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-cs.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-de.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-de.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-en.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-en.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-es.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-es.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-fr.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-fr.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-it.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-it.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-ja.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ja.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-ko.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ko.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-nl.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-nl.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-pl.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-pl.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-ru.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-ru.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-sk.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-sk.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-uk.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-uk.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/search/stopwords/stopwords-zh.json` & `aa_forum-2.2.1/aa_forum/search/stopwords/stopwords-zh.json`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/css/aa-forum.css` & `aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/css/aa-forum.min.css` & `aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/css/aa-forum.min.css.map` & `aa_forum-2.2.1/aa_forum/static/aa_forum/css/aa-forum.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-admin.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-desktop-widgets.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-oembed.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map` & `aa_forum-2.2.1/aa_forum/static/aa_forum/javascript/aa-forum-personal-messages.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2/4.1.0-rc1/js/select2.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/select2-bootstrap-5-theme/1.3.0/select2-bootstrap-5-theme.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/jquery.sumoselect.min.js`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css` & `aa_forum-2.2.1/aa_forum/static/aa_forum/libs/sumoselect/3.4.8/sumoselect.min.css`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/base.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/base.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/ajax-render/personal-messages/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/select2-css.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/select2-css.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/bundles/svg/aa-forum-icons.svg`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/administration/delete-board.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/administration/delete-board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/administration/delete-category.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/administration/delete-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-lock-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-change-sticky-state.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/board/topic-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/forum/topic/message-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/modals/personal-messages/message-delete.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/breadcrumb.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/board-loop.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/board-loop.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/categories.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/categories.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/category-loop.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/category-loop.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/new-category.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/new-category.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/administration/settings-form.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/administration/settings-form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/unread-topic-buttons.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/board-index.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/board-index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/board.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/pagination.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/board/topic.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/board/topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/message-author.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/message.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/modify-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/reply.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/reply.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/forum/topic/unread-topics.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/menu/menu-admin.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu/menu-admin.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/menu/menu-user.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/menu/menu-user.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sidebar.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/messages.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/inbox/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/new-message/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/reply-message/message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/messages.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/personal-messages/sent-messages/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/profile/form.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/profile/form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/search/pagination.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/pagination.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/partials/search/search-form.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/partials/search/search-form.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/administration/categories-and-boards.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/board.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/board.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/index.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/modify-message.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/modify-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/modify-topic.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/modify-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/new-topic.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/new-topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/topic.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/topic.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/forum/unread-topics.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/forum/unread-topics.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/personal-messages/inbox.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/inbox.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/personal-messages/new-message.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/new-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/reply-message.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/personal-messages/sent-messages.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/profile/index.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/profile/index.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/search/results.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/search/results.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html` & `aa_forum-2.2.1/aa_forum/templates/aa_forum/view/widgets/dashboard-widgets.html`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/templatetags/aa_forum.py` & `aa_forum-2.2.1/aa_forum/templatetags/aa_forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_app_settings.py` & `aa_forum-2.2.1/aa_forum/tests/test_app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_auth_hooks.py` & `aa_forum-2.2.1/aa_forum/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_helpers.py` & `aa_forum-2.2.1/aa_forum/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_integration.py` & `aa_forum-2.2.1/aa_forum/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_managers.py` & `aa_forum-2.2.1/aa_forum/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_models.py` & `aa_forum-2.2.1/aa_forum/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_signals.py` & `aa_forum-2.2.1/aa_forum/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_templatetags.py` & `aa_forum-2.2.1/aa_forum/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_views_admin.py` & `aa_forum-2.2.1/aa_forum/tests/test_views_admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/test_views_forum.py` & `aa_forum-2.2.1/aa_forum/tests/test_views_forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/tests/utils.py` & `aa_forum-2.2.1/aa_forum/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/views/admin.py` & `aa_forum-2.2.1/aa_forum/views/admin.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/views/forum.py` & `aa_forum-2.2.1/aa_forum/views/forum.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/views/personal_messages.py` & `aa_forum-2.2.1/aa_forum/views/personal_messages.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/views/profile.py` & `aa_forum-2.2.1/aa_forum/views/profile.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/views/search.py` & `aa_forum-2.2.1/aa_forum/views/search.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/aa_forum/views/widgets.py` & `aa_forum-2.2.1/aa_forum/views/widgets.py`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/LICENSE` & `aa_forum-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/README.md` & `aa_forum-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/pyproject.toml` & `aa_forum-2.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_forum-2.2.0/PKG-INFO` & `aa_forum-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-forum
-Version: 2.2.0
+Version: 2.2.1
 Summary: Simple forum for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-forum/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-forum/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-forum
 Project-URL: Source, https://github.com/ppfeufer/aa-forum.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-forum/issues
```

