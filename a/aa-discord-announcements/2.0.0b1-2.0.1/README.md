# Comparing `tmp/aa_discord_announcements-2.0.0b1.tar.gz` & `tmp/aa_discord_announcements-2.0.1.tar.gz`

## Comparing `aa_discord_announcements-2.0.0b1.tar` & `aa_discord_announcements-2.0.1.tar`

### file list

```diff
@@ -1,67 +1,75 @@
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/__init__.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/admin.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/app_settings.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/apps.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/auth_hooks.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/constants.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/forms.py
--rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/models.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/urls.py
--rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/views.py
--rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/helper/announcement_context.py
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/helper/discord_webhook.py
--rw-r--r--   0        0        0     7024 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/django.pot
--rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9415 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4836 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10071 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7447 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6997 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10667 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10180 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/migrations/0001_initial.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/migrations/0002_translation_updates.py
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/migrations/0003_fix_pseudo_plural_in_help_text.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/migrations/0004_alter_pingtarget_options.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/migrations/__init__.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css.map
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js.map
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/base.html
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/index.html
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templatetags/__init__.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/templatetags/aa_discord_announcements.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/__init__.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_access.py
--rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_ajax_calls.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_installed_modules.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_models.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_templatetags.py
--rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/LICENSE
--rw-r--r--   0        0        0     6029 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/README.md
--rw-r--r--   0        0        0     2062 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    48579 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/__init__.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/admin.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/app_settings.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/apps.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/auth_hooks.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/constants.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/forms.py
+-rw-r--r--   0        0        0     6560 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/models.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/urls.py
+-rw-r--r--   0        0        0     5010 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/views.py
+-rw-r--r--   0        0        0     3671 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/helper/announcement_context.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/helper/discord_webhook.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/django.pot
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5799 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4838 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10090 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5626 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9467 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7220 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7171 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5021 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9661 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7612 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6997 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10684 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4100 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10384 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5383 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/migrations/0001_initial.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/migrations/0002_translation_updates.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/migrations/0003_fix_pseudo_plural_in_help_text.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/migrations/0004_alter_pingtarget_options.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/migrations/__init__.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.css
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css.map
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js.map
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/base.html
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/index.html
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-css.html
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/bundles/discord-announcements-js.html
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/copy-paste-text.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templatetags/__init__.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/templatetags/aa_discord_announcements.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/tests/__init__.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_access.py
+-rw-r--r--   0        0        0     4964 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_ajax_calls.py
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_installed_modules.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_models.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1501 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/aa_discord_announcements/tests/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/LICENSE
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/README.md
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    48652 2020-02-02 00:00:00.000000 aa_discord_announcements-2.0.1/PKG-INFO
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/admin.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/admin.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/apps.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/apps.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/auth_hooks.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/auth_hooks.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
 
     def __init__(self):
         # setup menu entry for sidebar
         MenuItemHook.__init__(
             self,
             text=__title__,
-            classes="far fa-bell",
+            classes="fa-regular fa-bell",
             url_name="aa_discord_announcements:index",
             navactive=["aa_discord_announcements:"],
         )
 
     def render(self, request):
         """
         Check if the user has the permission to view this app
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/forms.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/forms.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/models.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/urls.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/urls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/views.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/views.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/helper/announcement_context.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/helper/announcement_context.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/helper/discord_webhook.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/helper/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/django.pot` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/django.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
+"POT-Creation-Date: 2024-03-20 17:28+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr ""
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
@@ -84,145 +84,145 @@
 msgid "Your announcement …"
 msgstr ""
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
 msgstr ""
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 msgid "Discord ID"
 msgstr ""
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr ""
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
 msgstr ""
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:127
+#: aa_discord_announcements/models.py:131
 msgid "Discord ping target"
 msgstr ""
 
-#: aa_discord_announcements/models.py:128
+#: aa_discord_announcements/models.py:132
 msgid "Discord ping targets"
 msgstr ""
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr ""
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr ""
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 msgid "Announcement details"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 msgid "Formatted announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 msgid "Copy announcement text"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 msgid "Create announcement"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
 
@@ -230,14 +230,14 @@
 msgid "Don't ping"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr ""
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
 msgstr ""
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
 msgstr ""
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Additionally configured announcement targets"
 msgstr "Zusätzlich konfigurierte Ankündigungsziele"
 
 msgid "Announcement channel"
 msgstr "Ankündigungskanal"
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/de/LC_MESSAGES/django.po` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
-"PO-Revision-Date: 2023-10-01 14:43+0000\n"
+"POT-Creation-Date: 2024-03-15 19:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:00+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr "Discord-Ankündigungen"
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr "Gruppenname"
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr "Gruppenbeschränkungen"
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr "Discord-Kanal"
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr "Webhook URL"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
@@ -86,145 +86,144 @@
 msgid "Your announcement …"
 msgstr "Deine Ankündigung …"
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr "Du solltest zunächst den Discord Service installieren …"
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 "Bist Du sicher das Du Deinen Discord Server mit Alliance Auth verbunden hast?"
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "Diese Gruppe wurde bisher noch nicht zu Discord synchronisiert."
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
 msgstr "Kann auf diese App zugreifen"
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Name der Discord Rolle zum Pingen. (Hinweis: Dies muss eine Auth Gruppe sein "
 "die zu Discord synchronisiert wurde.)"
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 msgid "Discord ID"
 msgstr "Discord ID"
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr "ID der Discord Rolle zum Pingen"
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 msgid "Restrict ping rights to the following groups …"
 msgstr "Beschränkt die Ping-Rechte auf die folgenden Gruppen …"
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr "Notizen"
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 "Wenn Du möchtest, kannst Du hier Anmerkungen zu dieser Konfiguration "
 "hinzufügen"
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
 msgstr "Ist aktiviert"
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr "Ist dieses Pingziel aktiv oder nicht"
 
-#: aa_discord_announcements/models.py:127
+#: aa_discord_announcements/models.py:131
 msgid "Discord ping target"
 msgstr "Discord Pingziel"
 
-#: aa_discord_announcements/models.py:128
+#: aa_discord_announcements/models.py:132
 msgid "Discord ping targets"
 msgstr "Discord Pingziele"
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr "Name des Kanals in dem dieser Webhook postet"
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
-msgstr ""
-"URL des Webhooks, z. B.: https://discord.com/api/webhooks/123456/abcdef"
+msgstr "URL des Webhooks, z. B.: https://discord.com/api/webhooks/123456/abcdef"
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 "Wenn Du möchtest, kannst Du hier Anmerkungen zu diesem Webhook hinzufügen"
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr "Ist dieser Webhook aktiv oder nicht"
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr "Webhook"
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr "Webhooks"
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Ungültige Webhook-URL. Die eingegebene Webhook-URL stimmt mit keinem "
 "bekannten Format für einen Discord-Webhook überein. Bitte überprüfe die "
 "Webhook-URL."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 msgid "Announcement details"
 msgstr "Ankündigungsdetails"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 msgid "Formatted announcement text"
 msgstr "Formatierter Text der Ankündigung"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
 msgstr ""
 "Pflichtangaben fehlen.<br>Um eine Ankündigung zu erstellen, müssen folgende "
 "Felder ausgefüllt sein:<br>» Ankündigungstext"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 "Fehler! Die Ankündigung wurde nicht in Ihre Zwischenablage kopiert. "
 "Möglicherweise unterstützt Dein Browser diese Funktion nicht."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Erfolg! Der Ankündigungstext wurde in die Zwischenablage kopiert."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr "Noch keine Ankündigung erstellt …"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 msgid "Copy announcement text"
 msgstr "Kopiere Ankündigungstext"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -232,15 +231,15 @@
 "Du möchtest helfen diese App in Deine Sprache zu übersetzen oder die "
 "bestehende Übersetzung verbessern?"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Tritt unserm Team von Übersetzern bei!"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 msgid "Create announcement"
 msgstr "Ankündigung erstellen"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr "Keiner, einfach nur den Text formatieren"
 
@@ -248,14 +247,14 @@
 msgid "Don't ping"
 msgstr "Nicht pingen"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr "Zusätzlich konfigurierte Ankündigungsziele"
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
 msgstr "Formular ungültig. Bitte die Angaben prüfen."
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
 msgstr "Keine Formulardaten übermittelt."
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Additionally configured announcement targets"
 msgstr "Destinos adicionales del anuncio configurado"
 
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "¿Está seguro de que tiene su Discord vinculado a su Alliance Auth?"
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/es/LC_MESSAGES/django.po` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/es/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
-# Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
+# Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
-"PO-Revision-Date: 2023-10-25 07:04+0000\n"
+"POT-Creation-Date: 2024-03-15 19:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:00+0000\n"
 "Last-Translator: Geovanny David Morales De la cruz <moralesgeovanny1996@gmail"
 ".com>\n"
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr "Anuncios de Discord"
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr "Nombre del grupo"
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr "Restricciones de grupo"
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr "Canal de Discord"
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr "URL del webhook"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
@@ -94,153 +94,153 @@
 msgid "Your announcement …"
 msgstr "Tu anuncio …"
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr "Es posible que desee instalar primero el servicio de Discord …"
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "¿Está seguro de que tiene su Discord vinculado a su Alliance Auth?"
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "Este grupo aún no se ha sincronizado con Discord."
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
 msgstr "Puede acceder esta aplicacion"
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Nombre del rol de Discord para hacer ping. (Nota: debe ser un grupo de "
 "autenticación sincronizado con Discord.)"
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 msgid "Discord ID"
 msgstr "ID de Discord"
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr "ID del rol de Discord para hacer ping"
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 msgid "Restrict ping rights to the following groups …"
 msgstr "Restringir los derechos de ping a los siguientes grupos…"
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr "Notas"
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr "Puede agregar aquí notas sobre esta configuración si lo desea"
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
 msgstr "Está habilitado"
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr "Si el destino de este ping está habilitado o no"
 
-#: aa_discord_announcements/models.py:127
+#: aa_discord_announcements/models.py:131
 #, fuzzy
 #| msgid "Discord Ping Target"
 msgid "Discord ping target"
 msgstr "Destino del Ping de Discord"
 
-#: aa_discord_announcements/models.py:128
+#: aa_discord_announcements/models.py:132
 #, fuzzy
 #| msgid "Discord Ping Targets"
 msgid "Discord ping targets"
 msgstr "Destinos del Ping de Discord"
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr "Nombre del canal en el que publica este webhook"
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL de este webhook, p.ej. https://discord.com/api/webhooks/123456/abcdef"
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr "Puede agregar aquí notas sobre este webhook si lo desea"
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr "Si este webhook está activo o no"
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr "Webhook"
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr "Webhooks"
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "URL de webhook no válida. La URL del webhook que ingresó no coincide con "
 "ningún formato conocido para un webhook de Discord. Compruebe la URL del "
 "webhook."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 #, fuzzy
 #| msgid "Announcement Details"
 msgid "Announcement details"
 msgstr "Detalles del anuncio"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 #, fuzzy
 #| msgid "Formatted Announcement Text"
 msgid "Formatted announcement text"
 msgstr "Formato del Texto del Anuncio"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 #, fuzzy
 #| msgid ""
 #| "Mandatory information is missing.<br>To create an announcement, you need "
 #| "to fill out the following fields:<br>» Announcement Text"
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
 msgstr ""
 "Falta información obligatoria.<br>Para crear un anuncio, debe completar los "
 "siguientes campos:<br>» Texto del anuncio"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 "¡Error! Su anuncio no se copió en su portapapeles. Tal vez su navegador no "
 "admita esta función."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "¡Éxito! El texto de su anuncio se ha copiado en su portapapeles."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr "Aún no se ha creado ningún anuncio…"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 #, fuzzy
 #| msgid "Copy Announcement Text"
 msgid "Copy announcement text"
 msgstr "Copiar el Texto del Anuncio"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
@@ -250,15 +250,15 @@
 "¿Quieres ayudar a traducir esta aplicación a tu idioma o mejorar la "
 "traducción existente?"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "¡Únete a nuestro equipo de traductores!"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 #, fuzzy
 #| msgid "Create Announcement"
 msgid "Create announcement"
 msgstr "Crear un Anuncio"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
@@ -270,14 +270,14 @@
 msgid "Don't ping"
 msgstr "No hacer Ping"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr "Destinos adicionales del anuncio configurado"
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
 msgstr "Formulario inválido. Por favor, compruebe su entrada."
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
 msgstr "No se enviaron datos del formulario."
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/fr_FR/LC_MESSAGES/django.po` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
-# erka Ekanon <M6musicT@hotmail.fr>, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
-"PO-Revision-Date: 2024-01-12 19:05+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-discord-announcements/fr/>\n"
-"Language: fr_FR\n"
+"POT-Creation-Date: 2024-03-20 17:28+0100\n"
+"PO-Revision-Date: 2024-05-10 14:00+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-discord-announcements/pl/>\n"
+"Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
-
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.5.3\n"
+
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr ""
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
 msgstr ""
 
 #: aa_discord_announcements/forms.py:21
 msgid "This field is mandatory"
-msgstr "Ce champ est obligatoire"
+msgstr "To pole jest wymagane"
 
 #: aa_discord_announcements/forms.py:42
 msgid "Discord Markdown"
-msgstr ""
+msgstr "Discord Markdown"
 
 #: aa_discord_announcements/forms.py:49
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
 
 #: aa_discord_announcements/forms.py:61
@@ -86,147 +86,149 @@
 msgid "Your announcement …"
 msgstr ""
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
-msgstr "Peut accéder à cette application"
+msgstr ""
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
+"Nazwa Discord role do pingowania. (Notatka: Musi być w Auth group, które "
+"jest zsynchronizowane z Discord.)"
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 msgid "Discord ID"
 msgstr ""
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr ""
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
-msgstr ""
+msgstr "Zaznaczony"
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:127
+#: aa_discord_announcements/models.py:131
 msgid "Discord ping target"
 msgstr ""
 
-#: aa_discord_announcements/models.py:128
+#: aa_discord_announcements/models.py:132
 msgid "Discord ping targets"
 msgstr ""
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr ""
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr ""
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 msgid "Announcement details"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 msgid "Formatted announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 msgid "Copy announcement text"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
-"Voulez-vous aider à traduire cette application dans votre langue ou "
-"améliorer la traduction existante ?"
+"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
+"tłumaczenia?"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "Rejoignez notre équipe de traducteurs !"
+msgstr "Dołącz do naszego zespołu tłumaczy!"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 msgid "Create announcement"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
 
@@ -234,14 +236,14 @@
 msgid "Don't ping"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr ""
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
-msgstr ""
+msgstr "Formularz niepoprawny. Sprawdź dane."
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
-msgstr ""
+msgstr "Nie wysłano danych formularza."
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,11 +7,11 @@
 "Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "This field is mandatory"
 msgstr "Questo campo è obbligatorio"
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"POT-Creation-Date: 2024-03-15 19:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:00+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-discord-announcements/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-discord-announcements/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr ""
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
@@ -85,145 +85,145 @@
 msgid "Your announcement …"
 msgstr ""
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
 msgstr ""
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 msgid "Discord ID"
 msgstr ""
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr ""
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
 msgstr ""
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:127
+#: aa_discord_announcements/models.py:131
 msgid "Discord ping target"
 msgstr ""
 
-#: aa_discord_announcements/models.py:128
+#: aa_discord_announcements/models.py:132
 msgid "Discord ping targets"
 msgstr ""
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr ""
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr ""
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 msgid "Announcement details"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 msgid "Formatted announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 msgid "Copy announcement text"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 msgid "Create announcement"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
 
@@ -231,14 +231,14 @@
 msgid "Don't ping"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr ""
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
 msgstr ""
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
 msgstr ""
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ja/LC_MESSAGES/django.po` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/nl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,47 +3,47 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"POT-Creation-Date: 2024-03-20 17:28+0100\n"
+"PO-Revision-Date: 2024-05-10 14:00+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-discord-announcements/ja/>\n"
-"Language: ja\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-discord-announcements/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr ""
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
@@ -86,145 +86,145 @@
 msgid "Your announcement …"
 msgstr ""
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
 msgstr ""
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 msgid "Discord ID"
 msgstr ""
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr ""
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
 msgstr ""
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:127
+#: aa_discord_announcements/models.py:131
 msgid "Discord ping target"
 msgstr ""
 
-#: aa_discord_announcements/models.py:128
+#: aa_discord_announcements/models.py:132
 msgid "Discord ping targets"
 msgstr ""
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr ""
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr ""
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 msgid "Announcement details"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 msgid "Formatted announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 msgid "Copy announcement text"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 msgid "Create announcement"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
 
@@ -232,14 +232,14 @@
 msgid "Don't ping"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr ""
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
 msgstr ""
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
 msgstr ""
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,40 +7,55 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-discord-announcements/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Additionally configured announcement targets"
 msgstr "추가된 공지 역할"
 
+msgid "Announcement channel"
+msgstr "공지 채널"
+
+msgid "Announcement target"
+msgstr "공지 대상"
+
+msgid "Announcement text"
+msgstr "공지 내용"
+
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "디스코드가 Alliance Auth와 연동되어 있나요?"
 
 msgid "Can access this app"
 msgstr "서비스에 접근할 수 있습니다"
 
 msgid "Discord Announcements"
 msgstr "디스코드 공지"
 
 msgid "Discord Announcements v{__version__}"
 msgstr "디스코드 공지 v{__version__}"
 
 msgid "Discord ID"
-msgstr "역할 ID"
+msgstr "디스코드 ID"
 
 msgid "Discord Markdown"
 msgstr "디스코드 마크다운"
 
 msgid "Discord channel"
 msgstr "디스코드 채널"
 
+msgid "Discord ping target"
+msgstr "디스코드 핑 대상자"
+
+msgid "Discord ping targets"
+msgstr "디스코드 핑 대상자"
+
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
@@ -72,15 +87,15 @@
 "잘못된 웹훅 URL. 알려진 디스코드의 웹훅 URL 형태와 일치하지 않습니다. 웹훅 "
 "URL을 확인해 주세요."
 
 msgid "Is enabled"
 msgstr "활성화"
 
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "핑을 보낼 디스코드 역할. (설명: 디스코드와 연동된 Auth 그룹이어야 합니다.)"
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Author50CO <tkddlschry@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Author50CO <tkddlschry@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Mind of the Raven <okanieva@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
-"PO-Revision-Date: 2023-12-29 09:04+0000\n"
+"POT-Creation-Date: 2024-03-15 19:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:00+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr "디스코드 공지"
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr "그룹 이름"
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr "그룹 제한"
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr "디스코드 채널"
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr "웹훅 URL"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
@@ -56,203 +57,188 @@
 #: aa_discord_announcements/forms.py:42
 msgid "Discord Markdown"
 msgstr "디스코드 마크다운"
 
 #: aa_discord_announcements/forms.py:49
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
-msgstr ""
-"힌트: {discord_markdown_link}를 사용해 텍스트 양식을 변경할 수 있습니다."
+msgstr "힌트: {discord_markdown_link}를 사용해 텍스트 양식을 변경할 수 있습니다."
 
 #: aa_discord_announcements/forms.py:61
-#, fuzzy
-#| msgid "Announcement Target"
 msgid "Announcement target"
-msgstr "공지사항 핑"
+msgstr "공지 대상"
 
 #: aa_discord_announcements/forms.py:63
 msgid "Who do you want to ping?"
 msgstr "핑을 보낼까요?"
 
 #: aa_discord_announcements/forms.py:67
-#, fuzzy
-#| msgid "Announcement Channel"
 msgid "Announcement channel"
 msgstr "공지 채널"
 
 #: aa_discord_announcements/forms.py:69
 msgid "Select a channel to send the announcement to automatically."
 msgstr "공지사항을 자동으로 보낼 채널을 선택하세요."
 
 #: aa_discord_announcements/forms.py:73
-#, fuzzy
-#| msgid "Announcement Text"
 msgid "Announcement text"
 msgstr "공지 내용"
 
 #: aa_discord_announcements/forms.py:79
 msgid "Your announcement …"
 msgstr "공지 내용을 입력하세요…"
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr "디스코드 서비스를 먼저 설치해주세요…"
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "디스코드가 Alliance Auth와 연동되어 있나요?"
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "이 그룹은 아직 디스코드와 연동되어 있지 않습니다."
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
 msgstr "서비스에 접근할 수 있습니다"
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
-msgstr ""
-"핑을 보낼 디스코드 역할. (설명: 디스코드와 연동된 Auth 그룹이어야 합니다.)"
+msgstr "핑을 보낼 디스코드 역할. (설명: 디스코드와 연동된 Auth 그룹이어야 합니다.)"
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 msgid "Discord ID"
-msgstr "역할 ID"
+msgstr "디스코드 ID"
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr "핑을 보낼 역할의 디스코드 역할 ID"
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 msgid "Restrict ping rights to the following groups …"
 msgstr "다음 그룹만 핑을 보낼 수 있습니다…"
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr "설명"
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr "해당 설정에 대한 설명을 남길 수 있습니다"
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
 msgstr "활성화"
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr "핑 타겟 활성화 및 비활성화"
 
-#: aa_discord_announcements/models.py:127
-#, fuzzy
-#| msgid "Discord Ping Target"
+#: aa_discord_announcements/models.py:131
 msgid "Discord ping target"
-msgstr "핑 보낼 디스코드 역할"
+msgstr "디스코드 핑 대상자"
 
-#: aa_discord_announcements/models.py:128
-#, fuzzy
-#| msgid "Discord Ping Targets"
+#: aa_discord_announcements/models.py:132
 msgid "Discord ping targets"
-msgstr "핑 보낼 디스코드 역할"
+msgstr "디스코드 핑 대상자"
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr "웹훅과 연결된 채널 이름"
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr "웹훅의 URL, 예시) https://discord.com/api/webhooks/123456/abcdef"
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr "웹훅에 대한 설명을 남길 수 있습니다"
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr "웹훅 활성화 및 비활성화"
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr "웹훅"
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr "웹훅"
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
-msgstr ""
-"잘못된 웹훅 URL. 알려진 디스코드의 웹훅 URL 형태와 일치하지 않습니다. 웹훅 "
+msgstr "잘못된 웹훅 URL. 알려진 디스코드의 웹훅 URL 형태와 일치하지 않습니다. 웹훅 "
 "URL을 확인해 주세요."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 #, fuzzy
 #| msgid "Announcement Details"
 msgid "Announcement details"
 msgstr "공지 세부 사항"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 #, fuzzy
 #| msgid "Formatted Announcement Text"
 msgid "Formatted announcement text"
 msgstr "양식 적용된 공지 텍스트"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 #, fuzzy
 #| msgid ""
 #| "Mandatory information is missing.<br>To create an announcement, you need "
 #| "to fill out the following fields:<br>» Announcement Text"
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
-msgstr ""
-"필수 항목이 비어있습니다. <br>공지를 작성하려면, 다음 항목을 작성해야 합니다:"
-"<br>» 공지 내용"
+msgstr "필수 항목이 비어있습니다. <br>공지를 작성하려면, 다음 항목을 작성해야 "
+"합니다:<br>» 공지 내용"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
-msgstr ""
-"오류! 공지가 클립보드에 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 않"
-"을 수도 있습니다."
+msgstr "오류! 공지가 클립보드에 복사되지 않았습니다. 브라우저가 이 기능을 지원하지 "
+"않을 수도 있습니다."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "성공! 공지사항이 클립보드에 복사되었습니다."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr "공지사항이 없습니다…"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 #, fuzzy
 #| msgid "Copy Announcement Text"
 msgid "Copy announcement text"
 msgstr "공지 내용 복사"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 #, fuzzy
 #| msgid "Create Announcement"
 msgid "Create announcement"
 msgstr "공지 생성"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
@@ -264,14 +250,14 @@
 msgid "Don't ping"
 msgstr "핑 없음"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr "추가된 공지 역할"
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
 msgstr "잘못된 양식. 내용을 확인해 주세요."
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
 msgstr "양식 데이터가 없습니다."
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Additionally configured announcement targets"
 msgstr "Дополнительно сконфигурированные цели объявлений"
 
 msgid "Announcement channel"
 msgstr "Канал объявления"
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/ru/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,51 @@
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
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
-"PO-Revision-Date: 2023-10-03 16:43+0000\n"
+"POT-Creation-Date: 2024-03-15 19:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:00+0000\n"
 "Last-Translator: Max <mark25@inbox.ru>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-discord-announcements/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr "Объявления Discord"
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr "Имя группы"
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr "Ограничения групп"
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr "Канал Discord"
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr "Вебхук URL"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
@@ -90,140 +90,140 @@
 msgid "Your announcement …"
 msgstr "Ваше объявление …"
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr "Возможно, Вам следует сначала установить сервис Discord …"
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Вы уверены, что Ваш Discord связан с Вашим Alliance Auth?"
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "Эта группа не была синхронизирована с Discord."
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
 msgstr "Имеет доступ к приложению"
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Имя роли Discord для пинга. (Примечание: Это должна быть синхронизированная "
 "с Discord группа Auth.)"
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 msgid "Discord ID"
 msgstr "Идентификатор Discord"
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr "ID роли Discord для пинга"
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 msgid "Restrict ping rights to the following groups …"
 msgstr "Ограничить право пинговать для следующих групп …"
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr "Примечания"
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr "Здесь Вы можете добавить примечания для этой конфигурации"
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
 msgstr "Разрешен"
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr "Разрешена или нет цель пинга"
 
-#: aa_discord_announcements/models.py:127
+#: aa_discord_announcements/models.py:131
 msgid "Discord ping target"
 msgstr "Цель пинга Discrod"
 
-#: aa_discord_announcements/models.py:128
+#: aa_discord_announcements/models.py:132
 msgid "Discord ping targets"
 msgstr "Цели пинга Discord"
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr "Название канала, в который вебхук отправляет сообщения"
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 "URL этого вебхука, например https://discord.com/api/webhooks/123456/abcdef"
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr "Здесь Вы можете добавить примечания для этого вебхука"
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr "Активен или нет вебхук"
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr "Вебхук"
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr "Вебхуки"
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Некорректный URL вебхука. Введенный URL не совпадает с известными форматами "
 "вебхуков Discord. Пожалуйста, проверьте URL."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 msgid "Announcement details"
 msgstr "Детали анонса"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 msgid "Formatted announcement text"
 msgstr "Отформатированный текст анонса"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
 msgstr ""
 "Отсутствует необходимая информация. <br>Для создания анонса необходимо "
 "заполнить следующие поля:<br>» Текст анонса"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 "Ошибка! Объявление не было скопировано в буфер обмена. Вероятно Ваш браузер "
 "не предоставляет такую функциональность."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr "Успех! Объявление скопировано в буфер обмена."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr "Объявлений нет …"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 msgid "Copy announcement text"
 msgstr "Скопировать текст анонса"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -231,15 +231,15 @@
 "Вы хотите помочь перевести это приложение на ваш язык или улучшить текущий "
 "перевод?"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Присоединяйтесь к нашей команде переводчиков!"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 msgid "Create announcement"
 msgstr "Создать анонс"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr "Нет, только отформатируй"
 
@@ -247,14 +247,14 @@
 msgid "Don't ping"
 msgstr "Без пинга"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr "Дополнительно сконфигурированные цели объявлений"
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
 msgstr "Форма некорректна. Проверьте введенные данные."
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
 msgstr "Данные формы не отправлены."
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.mo`

 * *Files 8% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,34 +8,36 @@
 "apps/aa-discord-announcements/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Ви впевнені, що ваш Discord пов'язаний з вашим Alliance Auth?"
 
 msgid "Discord channel"
 msgstr "Канал діскорду"
 
-msgid "Don't Ping"
-msgstr "Не пінгувати"
-
 msgid "Form invalid. Please check your input."
 msgstr "Форма невірна. Будь ласка, перевірте свої дані."
 
 msgid "Group name"
 msgstr "Назва групи"
 
 msgid "Group restrictions"
 msgstr "Групові обмеження"
 
+msgid "Hint: You can use {discord_markdown_link} to format the text."
+msgstr ""
+"Підказка: Ви можете використовувати {discord_markdown_link} для форматування "
+"тексту."
+
 msgid "ID of the Discord role to ping"
 msgstr "Ідентифікатор ролі Discord для пінгування"
 
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/uk/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Kristof <kristof@teh.ninja>, 2023.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# "Andrii M." <elfleg0las88@gmail.com>, 2023.
+# Kristof <kristof@teh.ninja>, 2023, 2024.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# "Andrii M." <elfleg0las88@gmail.com>, 2023, 2024.
+# Madz Cooper <i.sviridjuk@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"POT-Creation-Date: 2024-03-15 19:08+0100\n"
+"PO-Revision-Date: 2024-05-10 14:00+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-discord-announcements/uk/>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-discord-announcements/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr "Назва групи"
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr "Групові обмеження"
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr "Канал діскорду"
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr "Веб-хук URL"
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
@@ -61,14 +62,16 @@
 msgid "Discord Markdown"
 msgstr "Discord markdown"
 
 #: aa_discord_announcements/forms.py:49
 #, python-brace-format
 msgid "Hint: You can use {discord_markdown_link} to format the text."
 msgstr ""
+"Підказка: Ви можете використовувати {discord_markdown_link} для форматування "
+"тексту."
 
 #: aa_discord_announcements/forms.py:61
 #, fuzzy
 #| msgid "Announcement Text"
 msgid "Announcement target"
 msgstr "Текст оголошення"
 
@@ -98,150 +101,150 @@
 msgid "Your announcement …"
 msgstr "Ваше оголошення…"
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr "Можливо, ви захочете спочатку встановити службу Discord …"
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr "Ви впевнені, що ваш Discord пов'язаний з вашим Alliance Auth?"
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr "Цю групу ще не синхронізовано з Discord."
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
 msgstr ""
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 "Ім'я ролі Discord, яку потрібно пінгувати. (Примітка: це має бути група "
 "Auth, яка синхронізована з Discord.)"
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 #, fuzzy
 #| msgid "Discord Markdown"
 msgid "Discord ID"
 msgstr "Discord markdown"
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr "Ідентифікатор ролі Discord для пінгування"
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 #, fuzzy
 #| msgid "Restrict ping rights to the following group(s) …"
 msgid "Restrict ping rights to the following groups …"
 msgstr "Обмежити права на пінг для наступних груп …"
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr ""
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr "Ви можете додати примітки про цю конфігурацію тут, якщо хочете"
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
 msgstr "Дозволено"
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:127
+#: aa_discord_announcements/models.py:131
 #, fuzzy
 #| msgid "Discord Ping Target"
 msgid "Discord ping target"
 msgstr "Ціль для пінгу в Discord"
 
-#: aa_discord_announcements/models.py:128
+#: aa_discord_announcements/models.py:132
 #, fuzzy
 #| msgid "Discord Ping Targets"
 msgid "Discord ping targets"
 msgstr "Цілі для пінгу в Discord"
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr "Назва каналу, на який публікується цей веб-хук"
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
-"URL-адреса цього веб-хука, наприклад, https://discord.com/api/"
-"webhooks/123456/abcdef"
+"URL-адреса цього веб-хука, наприклад, https://discord.com/api/webhooks/"
+"123456/abcdef"
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr "Ви можете додати примітки про цей вебхук тут, якщо хочете"
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr "Активний цей вебхук чи ні"
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr "Веб-хук"
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr "Веб-хуки"
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 "Неправильна URL-адреса веб-хука. Введена вами URL-адреса веб-хука не "
 "відповідає жодному з відомих форматів веб-хуків Discord. Будь ласка, "
 "перевірте URL-адресу веб-хука."
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 #, fuzzy
 #| msgid "Announcement Text"
 msgid "Announcement details"
 msgstr "Текст оголошення"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 #, fuzzy
 #| msgid "Announcement Text"
 msgid "Formatted announcement text"
 msgstr "Текст оголошення"
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 #, fuzzy
 #| msgid "Announcement Text"
 msgid "Copy announcement text"
 msgstr "Текст оголошення"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
@@ -249,15 +252,15 @@
 "existing translation?"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 #, fuzzy
 #| msgid "Your announcement…"
 msgid "Create announcement"
 msgstr "Ваше оголошення…"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
@@ -269,14 +272,14 @@
 msgid "Don't ping"
 msgstr "Не пінгувати"
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr ""
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
 msgstr "Форма невірна. Будь ласка, перевірте свої дані."
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
 msgstr "Не подано жодних даних."
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_discord_announcements-2.0.1/aa_discord_announcements/locale/sk/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,62 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Dehao Wu <wudehao2000@163.com>, 2024.
-# Faer Yili <yilifaer@gmail.com>, 2024.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-09-30 16:29+0200\n"
-"PO-Revision-Date: 2024-01-11 21:04+0000\n"
-"Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
-"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-discord-announcements/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"POT-Creation-Date: 2024-03-20 17:28+0100\n"
+"PO-Revision-Date: 2024-05-10 14:00+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-discord-announcements/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
-
-#: aa_discord_announcements/__init__.py:12
-#: aa_discord_announcements/templates/aa_discord_announcements/base.html:5
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:6
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"X-Generator: Weblate 5.5.3\n"
+
+#: aa_discord_announcements/__init__.py:9
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:6
+#: aa_discord_announcements/templates/aa_discord_announcements/base.html:10
 msgid "Discord Announcements"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:79
+#: aa_discord_announcements/admin.py:32 aa_discord_announcements/models.py:83
 msgid "Group name"
 msgstr ""
 
 #: aa_discord_announcements/admin.py:38 aa_discord_announcements/admin.py:72
-#: aa_discord_announcements/models.py:102
-#: aa_discord_announcements/models.py:194
+#: aa_discord_announcements/models.py:106
+#: aa_discord_announcements/models.py:198
 msgid "Group restrictions"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:172
+#: aa_discord_announcements/admin.py:61 aa_discord_announcements/models.py:176
 msgid "Discord channel"
 msgstr ""
 
-#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:180
+#: aa_discord_announcements/admin.py:66 aa_discord_announcements/models.py:184
 msgid "Webhook URL"
 msgstr ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aa_discord_announcements/apps.py:21
 #, python-brace-format
 msgid "Discord Announcements v{__version__}"
 msgstr ""
 
 #: aa_discord_announcements/forms.py:21
 msgid "This field is mandatory"
-msgstr "这个字段是必填的"
+msgstr ""
 
 #: aa_discord_announcements/forms.py:42
 msgid "Discord Markdown"
 msgstr ""
 
 #: aa_discord_announcements/forms.py:49
 #, python-brace-format
@@ -86,145 +87,145 @@
 msgid "Your announcement …"
 msgstr ""
 
 #: aa_discord_announcements/models.py:37
 msgid "You might want to install the Discord service first …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:44
+#: aa_discord_announcements/models.py:45
 msgid "Are you sure you have your Discord linked to your Alliance Auth?"
 msgstr ""
 
-#: aa_discord_announcements/models.py:48
+#: aa_discord_announcements/models.py:51
 msgid "This group has not been synced to Discord yet."
 msgstr ""
 
-#: aa_discord_announcements/models.py:65
+#: aa_discord_announcements/models.py:69
 msgid "Can access this app"
-msgstr "允许访问此软件"
+msgstr ""
 
-#: aa_discord_announcements/models.py:82
+#: aa_discord_announcements/models.py:86
 msgid ""
 "Name of the Discord role to ping. (Note: This must be an Auth group that is "
 "synced to Discord.)"
 msgstr ""
 
-#: aa_discord_announcements/models.py:93
+#: aa_discord_announcements/models.py:97
 msgid "Discord ID"
 msgstr ""
 
-#: aa_discord_announcements/models.py:94
+#: aa_discord_announcements/models.py:98
 msgid "ID of the Discord role to ping"
 msgstr ""
 
-#: aa_discord_announcements/models.py:103
-#: aa_discord_announcements/models.py:195
+#: aa_discord_announcements/models.py:107
+#: aa_discord_announcements/models.py:199
 msgid "Restrict ping rights to the following groups …"
 msgstr ""
 
-#: aa_discord_announcements/models.py:110
-#: aa_discord_announcements/models.py:202
+#: aa_discord_announcements/models.py:114
+#: aa_discord_announcements/models.py:206
 msgid "Notes"
 msgstr ""
 
-#: aa_discord_announcements/models.py:111
+#: aa_discord_announcements/models.py:115
 msgid "You can add notes about this configuration here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:118
-#: aa_discord_announcements/models.py:210
+#: aa_discord_announcements/models.py:122
+#: aa_discord_announcements/models.py:214
 msgid "Is enabled"
-msgstr "已启用"
+msgstr ""
 
-#: aa_discord_announcements/models.py:119
+#: aa_discord_announcements/models.py:123
 msgid "Whether this ping target is enabled or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:127
+#: aa_discord_announcements/models.py:131
 msgid "Discord ping target"
 msgstr ""
 
-#: aa_discord_announcements/models.py:128
+#: aa_discord_announcements/models.py:132
 msgid "Discord ping targets"
 msgstr ""
 
-#: aa_discord_announcements/models.py:173
+#: aa_discord_announcements/models.py:177
 msgid "Name of the channel this webhook posts to"
 msgstr ""
 
-#: aa_discord_announcements/models.py:183
+#: aa_discord_announcements/models.py:187
 msgid ""
 "URL of this webhook, e.g. https://discord.com/api/webhooks/123456/abcdef"
 msgstr ""
 
-#: aa_discord_announcements/models.py:203
+#: aa_discord_announcements/models.py:207
 msgid "You can add notes about this webhook here if you want"
 msgstr ""
 
-#: aa_discord_announcements/models.py:211
+#: aa_discord_announcements/models.py:215
 msgid "Whether this webhook is active or not"
 msgstr ""
 
-#: aa_discord_announcements/models.py:219
+#: aa_discord_announcements/models.py:223
 msgid "Webhook"
 msgstr ""
 
-#: aa_discord_announcements/models.py:220
+#: aa_discord_announcements/models.py:224
 msgid "Webhooks"
 msgstr ""
 
-#: aa_discord_announcements/models.py:236
+#: aa_discord_announcements/models.py:240
 msgid ""
 "Invalid webhook URL. The webhook URL you entered does not match any known "
 "format for a Discord webhook. Please check the webhook URL."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:15
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:10
 msgid "Announcement details"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:26
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:21
 msgid "Formatted announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:46
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:41
 msgid ""
 "Mandatory information is missing.<br>To create an announcement, you need to "
 "fill out the following fields:<br>» Announcement text"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:49
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:44
 msgid ""
 "Error! Your announcement was not copied to your clipboard. Maybe your "
 "browser doesn&apos;t support this feature."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/index.html:50
+#: aa_discord_announcements/templates/aa_discord_announcements/index.html:45
 msgid "Success! Your announcement text has been copied to your clipboard."
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:5
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:6
 msgid "No announcement created yet …"
 msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:22
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html:23
 msgid "Copy announcement text"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
-msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
+msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "加入我们的翻译团队吧！"
+msgstr ""
 
-#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:27
+#: aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html:22
 msgid "Create announcement"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-channel.html:3
 msgid "None, just format it for me"
 msgstr ""
 
@@ -232,14 +233,14 @@
 msgid "Don't ping"
 msgstr ""
 
 #: aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html:9
 msgid "Additionally configured announcement targets"
 msgstr ""
 
-#: aa_discord_announcements/views.py:154
+#: aa_discord_announcements/views.py:158
 msgid "Form invalid. Please check your input."
 msgstr ""
 
-#: aa_discord_announcements/views.py:156
+#: aa_discord_announcements/views.py:160
 msgid "No form data submitted."
 msgstr ""
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/migrations/0001_initial.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/migrations/0002_translation_updates.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/migrations/0002_translation_updates.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/migrations/0003_fix_pseudo_plural_in_help_text.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/migrations/0003_fix_pseudo_plural_in_help_text.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/migrations/0004_alter_pingtarget_options.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/migrations/0004_alter_pingtarget_options.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css.map` & `aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/css/aa-discord-announcements.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js` & `aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js` & `aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js.map` & `aa_discord_announcements-2.0.1/aa_discord_announcements/static/aa_discord_announcements/javascript/aa-discord-announcements.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/base.html` & `aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/base.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/index.html` & `aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/index.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html` & `aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/partials/announcement/announcement.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html` & `aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/form.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html` & `aa_discord_announcements-2.0.1/aa_discord_announcements/templates/aa_discord_announcements/partials/form/segments/announcement-targets.html`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/templatetags/aa_discord_announcements.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/templatetags/aa_discord_announcements.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_access.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_ajax_calls.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_ajax_calls.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_auth_hooks.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_auth_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
             character_id=1002,
             character_name="Bruce Wayne",
             permissions=["aa_discord_announcements.basic_access"],
         )
 
         cls.html_menu = f"""
             <li class="d-flex flex-wrap m-2 p-2 pt-0 pb-0 mt-0 mb-0 me-0 pe-0">
-                <i class="nav-link far fa-bell fa-fw align-self-center me-3 "></i>
+                <i class="nav-link fa-regular fa-bell fa-fw align-self-center me-3 "></i>
                 <a class="nav-link flex-fill align-self-center me-auto" href="{reverse('aa_discord_announcements:index')}">
                     Discord Announcements
                 </a>
             </li>
         """
 
     def test_render_hook_success(self):
```

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_installed_modules.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_models.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/test_templatetags.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/aa_discord_announcements/tests/utils.py` & `aa_discord_announcements-2.0.1/aa_discord_announcements/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/LICENSE` & `aa_discord_announcements-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_discord_announcements-2.0.0b1/README.md` & `aa_discord_announcements-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,21 @@
 
 ______________________________________________________________________
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Discord Announcements needs at least Alliance Auth v4.0.0**.
+> **AA Discord Announcements >=2.0.0 needs at least Alliance Auth v4.0.0**.
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.4.2`.
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding.
 (See the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
 
 > \[!NOTE\]
 >
```

### Comparing `aa_discord_announcements-2.0.0b1/pyproject.toml` & `aa_discord_announcements-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
 ]
 dynamic = [
     "version",
 ]
 dependencies = [
-    "allianceauth>=4.0.0b1",
+    "allianceauth<5.0.0,>=4",
     "allianceauth-app-utils>=1.13",
     "dhooks-lite>=0.6.1",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
     "coverage",
     "django-webtest",
```

### Comparing `aa_discord_announcements-2.0.0b1/PKG-INFO` & `aa_discord_announcements-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aa-discord-announcements
-Version: 2.0.0b1
+Version: 2.0.1
 Summary: Discord Announcements via Alliance Auth. Write announcements and manage who can write announcements on your corporation or alliance Discord through Alliance Auth.
 Project-URL: Changelog, https://github.com/ppfeufer/aa-discord-announcements/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-discord-announcements/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-discord-announcements
 Project-URL: Source, https://github.com/ppfeufer/aa-discord-announcements.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-discord-announcements/issues
@@ -698,15 +698,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.13
-Requires-Dist: allianceauth>=4.0.0b1
+Requires-Dist: allianceauth<5.0.0,>=4
 Requires-Dist: dhooks-lite>=0.6.1
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Requires-Dist: faker; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
 
@@ -751,19 +751,21 @@
 
 ______________________________________________________________________
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Discord Announcements needs at least Alliance Auth v4.0.0**.
+> **AA Discord Announcements >=2.0.0 needs at least Alliance Auth v4.0.0**.
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.4.2`.
 
 This app is a plugin for Alliance Auth. If you don't have Alliance Auth running already,
 please install it first before proceeding.
 (See the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/allianceauth.html) for details)
 
 > \[!NOTE\]
 >
```

