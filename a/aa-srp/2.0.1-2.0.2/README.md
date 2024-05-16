# Comparing `tmp/aa_srp-2.0.1.tar.gz` & `tmp/aa_srp-2.0.2.tar.gz`

## Comparing `aa_srp-2.0.1.tar` & `aa_srp-2.0.2.tar`

### file list

```diff
@@ -1,134 +1,137 @@
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/__init__.py
--rw-r--r--   0        0        0     8177 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/admin.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/app_settings.py
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/apps.py
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/auth_hooks.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/constants.py
--rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/form.py
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/managers.py
--rw-r--r--   0        0        0    14672 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/models.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/providers.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/urls.py
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/discord/channel_message.py
--rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/discord/direct_message.py
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/helper/character.py
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/helper/eve_images.py
--rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/helper/icons.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/helper/notification.py
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/helper/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/.gitkeep
--rw-r--r--   0        0        0    24464 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/django.pot
--rw-r--r--   0        0        0    24539 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    16893 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    31013 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27658 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    25241 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24641 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24474 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14818 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    30132 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    24456 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24884 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/pl_PL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    22094 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    36736 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    24534 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/sk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27056 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    15552 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    30235 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/management/commands/aasrp_load_eve.py
--rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/management/commands/aasrp_migrate_srp_data.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0001_initial.py
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0002_relations_update.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0003_aasrprequest_reject_info.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0004_aasrpusersettings.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0005_insurance.py
--rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0006_related_names.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0007_aasrprequestcomment_comment_time_and_more.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0008_aasrprequestcomment_new_status_and_more.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0009_add_fleet_type_to_srp_link.py
--rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0010_model_changes.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0011_default_settings.py
--rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0012_alter_fleettype_options_alter_insurance_options_and_more.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/0013_setting_loss_value_source.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/migrations/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/css/aa-srp-form.css
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/css/aa-srp-form.min.css
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/css/aa-srp-form.min.css.map
--rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/css/aa-srp.css
--rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/css/aa-srp.min.css
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/css/aa-srp.min.css.map
--rw-r--r--   0        0        0    11066 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-dashboard.js
--rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js.map
--rw-r--r--   0        0        0    16669 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-view-requests.js
--rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js
--rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js.map
--rw-r--r--   0        0        0    21204 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.css
--rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css
--rw-r--r--   0        0        0    25994 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css.map
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/clear.png
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/loading.gif
--rw-r--r--   0        0        0   219767 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.js
--rw-r--r--   0        0        0    75550 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js
--rw-r--r--   0        0        0    98885 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js.map
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/base.html
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/dashboard.html
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/link-add.html
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/link-edit.html
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/request-srp.html
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/view-requests.html
--rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/bundles/aa-srp-css.html
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/bundles/aa-srp-dashboard-js.html
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/bundles/aa-srp-form-css.html
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/bundles/aa-srp-view-requests-js.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/bundles/x-editable-css.html
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/bundles/x-editable-js.html
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/accept-rejected-request.html
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/accept-request.html
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/delete-request.html
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/mark-complete.html
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/reject-request.html
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/request-details.html
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/navigation.html
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/srp-links.html
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/tabs-content.html
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/tabs-navigation.html
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/user-settings.html
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/user-srp-requests.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/form/required-field-hint.html
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/link-add/form.html
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/link-edit/form.html
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/request-srp/fleet-details.html
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/request-srp/form.html
--rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/view-requests/overview.html
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templates/aasrp/partials/view-requests/requests.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templatetags/__init__.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/templatetags/aasrp.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/tests/__init__.py
--rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/tests/test_access.py
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/tests/test_auth_hooks.py
--rw-r--r--   0        0        0    11016 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/tests/test_helper_character.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/tests/test_installed_modules.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/tests/test_model_setting.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/tests/test_models.py
--rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/tests/test_templatetags.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/tests/utils.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/views/__init__.py
--rw-r--r--   0        0        0    24294 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/views/ajax.py
--rw-r--r--   0        0        0    19103 2020-02-02 00:00:00.000000 aa_srp-2.0.1/aasrp/views/general.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_srp-2.0.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_srp-2.0.1/LICENSE
--rw-r--r--   0        0        0    11465 2020-02-02 00:00:00.000000 aa_srp-2.0.1/README.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 aa_srp-2.0.1/pyproject.toml
--rw-r--r--   0        0        0    53992 2020-02-02 00:00:00.000000 aa_srp-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/__init__.py
+-rw-r--r--   0        0        0     8177 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/admin.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/app_settings.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/apps.py
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/auth_hooks.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/constants.py
+-rw-r--r--   0        0        0     7390 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/form.py
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/managers.py
+-rw-r--r--   0        0        0    14672 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/models.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/providers.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/urls.py
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/discord/channel_message.py
+-rw-r--r--   0        0        0     6468 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/discord/direct_message.py
+-rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/helper/character.py
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/helper/eve_images.py
+-rw-r--r--   0        0        0    12271 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/helper/icons.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/helper/notification.py
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/helper/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/.gitkeep
+-rw-r--r--   0        0        0    24464 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/django.pot
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24756 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    16893 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    31010 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27670 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    25240 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24647 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24474 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14818 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    30139 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24541 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24948 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    21804 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    36756 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24752 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27068 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    15552 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    30232 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/management/commands/aasrp_load_eve.py
+-rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/management/commands/aasrp_migrate_srp_data.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0002_relations_update.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0003_aasrprequest_reject_info.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0004_aasrpusersettings.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0005_insurance.py
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0006_related_names.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0007_aasrprequestcomment_comment_time_and_more.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0008_aasrprequestcomment_new_status_and_more.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0009_add_fleet_type_to_srp_link.py
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0010_model_changes.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0011_default_settings.py
+-rw-r--r--   0        0        0    11040 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0012_alter_fleettype_options_alter_insurance_options_and_more.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/0013_setting_loss_value_source.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/migrations/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/css/aa-srp-form.css
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/css/aa-srp-form.min.css
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/css/aa-srp-form.min.css.map
+-rw-r--r--   0        0        0     2222 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/css/aa-srp.css
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/css/aa-srp.min.css
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/css/aa-srp.min.css.map
+-rw-r--r--   0        0        0    11066 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-dashboard.js
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js.map
+-rw-r--r--   0        0        0    16669 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-view-requests.js
+-rw-r--r--   0        0        0     6321 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js.map
+-rw-r--r--   0        0        0    21204 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.css
+-rw-r--r--   0        0        0    17789 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css
+-rw-r--r--   0        0        0    25994 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css.map
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/clear.png
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/loading.gif
+-rw-r--r--   0        0        0   219767 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.js
+-rw-r--r--   0        0        0    75550 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js
+-rw-r--r--   0        0        0    98885 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js.map
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/base.html
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/dashboard.html
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/link-add.html
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/link-edit.html
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/request-srp.html
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/view-requests.html
+-rw-r--r--   0        0        0     4642 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/bundles/aa-srp-css.html
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/bundles/aa-srp-dashboard-js.html
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/bundles/aa-srp-form-css.html
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/bundles/aa-srp-view-requests-js.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/bundles/x-editable-css.html
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/bundles/x-editable-js.html
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/accept-rejected-request.html
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/accept-request.html
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/delete-request.html
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/mark-complete.html
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/reject-request.html
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/request-details.html
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/navigation.html
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/srp-links.html
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/tabs-content.html
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/tabs-navigation.html
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/user-settings.html
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/user-srp-requests.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/form/required-field-hint.html
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/link-add/form.html
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/link-edit/form.html
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/request-srp/fleet-details.html
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/request-srp/form.html
+-rw-r--r--   0        0        0     3260 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/view-requests/overview.html
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templates/aasrp/partials/view-requests/requests.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templatetags/__init__.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/templatetags/aasrp.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/tests/__init__.py
+-rw-r--r--   0        0        0     9678 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/tests/test_access.py
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0    11016 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/tests/test_helper_character.py
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/tests/test_installed_modules.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/tests/test_model_setting.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/tests/test_models.py
+-rw-r--r--   0        0        0    15384 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/tests/test_templatetags.py
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/tests/utils.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/views/__init__.py
+-rw-r--r--   0        0        0    24294 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/views/ajax.py
+-rw-r--r--   0        0        0    19103 2020-02-02 00:00:00.000000 aa_srp-2.0.2/aasrp/views/general.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_srp-2.0.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_srp-2.0.2/LICENSE
+-rw-r--r--   0        0        0    11465 2020-02-02 00:00:00.000000 aa_srp-2.0.2/README.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 aa_srp-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0    53992 2020-02-02 00:00:00.000000 aa_srp-2.0.2/PKG-INFO
```

### Comparing `aa_srp-2.0.1/aasrp/admin.py` & `aa_srp-2.0.2/aasrp/admin.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/app_settings.py` & `aa_srp-2.0.2/aasrp/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/auth_hooks.py` & `aa_srp-2.0.2/aasrp/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/constants.py` & `aa_srp-2.0.2/aasrp/constants.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/form.py` & `aa_srp-2.0.2/aasrp/form.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/managers.py` & `aa_srp-2.0.2/aasrp/managers.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/models.py` & `aa_srp-2.0.2/aasrp/models.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/urls.py` & `aa_srp-2.0.2/aasrp/urls.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/discord/channel_message.py` & `aa_srp-2.0.2/aasrp/discord/channel_message.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/discord/direct_message.py` & `aa_srp-2.0.2/aasrp/discord/direct_message.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/helper/character.py` & `aa_srp-2.0.2/aasrp/helper/character.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/helper/eve_images.py` & `aa_srp-2.0.2/aasrp/helper/eve_images.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/helper/icons.py` & `aa_srp-2.0.2/aasrp/helper/icons.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/helper/notification.py` & `aa_srp-2.0.2/aasrp/helper/notification.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/locale/django.pot` & `aa_srp-2.0.2/aasrp/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/locale/cs/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/nl/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

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
 "POT-Creation-Date: 2024-03-20 17:08+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-srp/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
-"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr ""
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
```

### Comparing `aa_srp-2.0.1/aasrp/locale/de/LC_MESSAGES/django.mo` & `aa_srp-2.0.2/aasrp/locale/de/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-srp/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "\n"
 "                            This SRP link still has "
 "%(number_pending_requests)s pending\n"
 "                            SRP request. Are you absolutely certain you want "
 "to mark\n"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/de/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 01:12+0100\n"
-"PO-Revision-Date: 2024-03-16 10:04+0000\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-srp/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr "Schiffserstattung"
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
@@ -432,16 +432,15 @@
 #: aasrp/templates/aasrp/partials/view-requests/overview.html:16
 msgid "Requests"
 msgstr "Anfragen"
 
 #: aasrp/models.py:394
 #, python-brace-format
 msgid "{character_name} ({user_name}) SRP request for: {ship} ({request_code})"
-msgstr ""
-"{character_name} ({user_name}) SRP Anfrage für: {ship} ({request_code})"
+msgstr "{character_name} ({user_name}) SRP Anfrage für: {ship} ({request_code})"
 
 #: aasrp/models.py:412 aasrp/models.py:473
 msgid "SRP request"
 msgstr "SRP Anfrage"
 
 #: aasrp/models.py:415
 msgid "Insurance level"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/es/LC_MESSAGES/django.mo` & `aa_srp-2.0.2/aasrp/locale/es/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-srp/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Activate selected fleet types"
 msgstr "Activar tipos de flota seleccionados"
 
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
 msgstr[0] "Tipo de flota activa {notifications_count}"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/es/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/es/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
 # Mak3rco <depormanuf1@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 01:12+0100\n"
-"PO-Revision-Date: 2024-04-08 17:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
 "Last-Translator: Mak3rco <depormanuf1@gmail.com>\n"
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-srp/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.3\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr "Reemplazo de Naves"
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
```

### Comparing `aa_srp-2.0.1/aasrp/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_srp-2.0.2/aasrp/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/locale/fr_FR/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 01:12+0100\n"
-"PO-Revision-Date: 2024-05-08 16:13+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: French <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-srp/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/it_IT/LC_MESSAGES/django.mo` & `aa_srp-2.0.2/aasrp/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,14 +7,14 @@
 "Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-srp/it/>\n"
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

### Comparing `aa_srp-2.0.1/aasrp/locale/it_IT/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/it_IT/LC_MESSAGES/django.po`

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
 "POT-Creation-Date: 2024-03-16 01:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-srp/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-srp/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr ""
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
```

### Comparing `aa_srp-2.0.1/aasrp/locale/ja/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/ja/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 01:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-srp/ja/>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-srp/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr ""
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
```

### Comparing `aa_srp-2.0.1/aasrp/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_srp-2.0.2/aasrp/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-srp/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "\n"
 "                        Are you sure you want to mark this SRP link as "
 "completed and\n"
 "                        close it for good? Be aware that once it's "
 "completed,\n"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/ko_KR/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Author50CO <tkddlschry@gmail.com>, 2023.
+# Author50CO <tkddlschry@gmail.com>, 2023, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 # Mind of the Raven <okanieva@gmail.com>, 2024.
 # Rodpold Shard <rodpold@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 01:12+0100\n"
-"PO-Revision-Date: 2024-03-21 17:11+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
+"Last-Translator: Author50CO <tkddlschry@gmail.com>\n"
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-srp/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr "SRP"
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
```

### Comparing `aa_srp-2.0.1/aasrp/locale/nl/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/cs/LC_MESSAGES/django.po`

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
 "POT-Creation-Date: 2024-03-20 17:08+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Czech <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-srp/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr ""
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
@@ -53,39 +55,47 @@
 
 #: aasrp/admin.py:286
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aasrp/admin.py:296
 #, python-brace-format
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aasrp/admin.py:302
 msgid "Deactivate selected fleet types"
 msgstr ""
 
 #: aasrp/admin.py:331
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aasrp/admin.py:341
 #, python-brace-format
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aasrp/apps.py:21
 #, python-brace-format
 msgid "AA Ship Replacement v{__version__}"
 msgstr ""
 
@@ -669,14 +679,16 @@
 "%(number_pending_requests)s pending\n"
 "                            SRP requests. Are you absolutely certain you "
 "want to mark\n"
 "                            this SRP link as completed?\n"
 "                        "
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aasrp/templates/aasrp/modals/view-requests/reject-request.html:18
 msgid "Are you sure you want to reject this SRP request?"
 msgstr ""
 
 #: aasrp/templates/aasrp/partials/dashboard/navigation.html:6
 msgid "View all"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/pl_PL/LC_MESSAGES/django.mo` & `aa_srp-2.0.2/aasrp/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-srp/pl/>\n"
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
 
 msgid "Delete"
 msgstr "Usuń"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/pl_PL/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/sk/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
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
 "POT-Creation-Date: 2024-03-20 17:08+0100\n"
-"PO-Revision-Date: 2024-04-07 13:07+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-srp/pl/>\n"
-"Language: pl_PL\n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-srp/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
-"|| n%100>=20) ? 1 : 2;\n"
-"X-Generator: Weblate 5.4.3\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr ""
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
@@ -38,55 +39,63 @@
 msgid "Requestor"
 msgstr ""
 
 #: aasrp/admin.py:229 aasrp/models.py:126 aasrp/models.py:183
 #: aasrp/templates/aasrp/partials/dashboard/srp-links.html:19
 #: aasrp/templates/aasrp/partials/request-srp/fleet-details.html:17
 msgid "Fleet type"
-msgstr "Typ floty"
+msgstr ""
 
 #: aasrp/admin.py:242 aasrp/models.py:117
 msgid "Is enabled"
-msgstr "Zaznaczony"
+msgstr ""
 
 #: aasrp/admin.py:257
 msgid "Activate selected fleet types"
 msgstr ""
 
 #: aasrp/admin.py:286
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aasrp/admin.py:296
 #, python-brace-format
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aasrp/admin.py:302
 msgid "Deactivate selected fleet types"
 msgstr ""
 
 #: aasrp/admin.py:331
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aasrp/admin.py:341
 #, python-brace-format
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aasrp/apps.py:21
 #, python-brace-format
 msgid "AA Ship Replacement v{__version__}"
 msgstr ""
 
@@ -96,15 +105,15 @@
 "your request reviser.\n"
 "Please make sure to always add the SRP code and the request code with your "
 "inquiry."
 msgstr ""
 
 #: aasrp/form.py:37
 msgid "This field is mandatory"
-msgstr "To pole jest wymagane"
+msgstr ""
 
 #: aasrp/form.py:53
 #: aasrp/templates/aasrp/partials/request-srp/fleet-details.html:13
 #: aasrp/templates/aasrp/partials/view-requests/overview.html:27
 msgid "Fleet name"
 msgstr ""
 
@@ -141,15 +150,15 @@
 msgstr ""
 
 #: aasrp/form.py:114 aasrp/models.py:348 aasrp/models.py:442
 #: aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html:82
 #: aasrp/templates/aasrp/dashboard.html:97
 #: aasrp/templates/aasrp/view-requests.html:81
 msgid "Additional information"
-msgstr "Dodatkowe informacje"
+msgstr ""
 
 #: aasrp/form.py:116
 msgid ""
 "Please tell us about the circumstances of your untimely demise. Who was the "
 "FC, what doctrine was called, have changes to the fit been requested and so "
 "on. Be as detailed as you can."
 msgstr ""
@@ -291,15 +300,15 @@
 
 #: aasrp/models.py:116
 msgid "Whether this fleet type is active or not"
 msgstr ""
 
 #: aasrp/models.py:127
 msgid "Fleet types"
-msgstr "Typy floty"
+msgstr ""
 
 #: aasrp/models.py:150
 msgid "Active"
 msgstr ""
 
 #: aasrp/models.py:151
 msgid "Closed"
@@ -323,15 +332,15 @@
 #: aasrp/templates/aasrp/partials/view-requests/overview.html:50
 msgid "SRP code"
 msgstr ""
 
 #: aasrp/models.py:169
 #: aasrp/templates/aasrp/partials/view-requests/overview.html:32
 msgid "Fleet commander"
-msgstr "Dowódca floty"
+msgstr ""
 
 #: aasrp/models.py:182
 msgid "The SRP link fleet type, if it's set"
 msgstr ""
 
 #: aasrp/models.py:188
 msgid "AAR link"
@@ -383,15 +392,15 @@
 #: aasrp/templates/aasrp/view-requests.html:69
 #: aasrp/templates/aasrp/view-requests.html:78
 msgid "Character"
 msgstr ""
 
 #: aasrp/models.py:333 aasrp/models.py:342
 msgid "Ship type"
-msgstr "Typ statku"
+msgstr ""
 
 #: aasrp/models.py:354 aasrp/templates/aasrp/dashboard.html:73
 #: aasrp/templates/aasrp/view-requests.html:67
 msgid "Request status"
 msgstr ""
 
 #: aasrp/models.py:356
@@ -613,15 +622,15 @@
 #: aasrp/templates/aasrp/modals/view-requests/reject-request.html:35
 msgid "Cancel"
 msgstr ""
 
 #: aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html:25
 #: aasrp/templates/aasrp/modals/view-requests/delete-request.html:29
 msgid "Delete"
-msgstr "Usuń"
+msgstr ""
 
 #: aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html:25
 msgid "Disable"
 msgstr ""
 
 #: aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html:25
 msgid "Enable"
@@ -670,14 +679,16 @@
 "%(number_pending_requests)s pending\n"
 "                            SRP requests. Are you absolutely certain you "
 "want to mark\n"
 "                            this SRP link as completed?\n"
 "                        "
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: aasrp/templates/aasrp/modals/view-requests/reject-request.html:18
 msgid "Are you sure you want to reject this SRP request?"
 msgstr ""
 
 #: aasrp/templates/aasrp/partials/dashboard/navigation.html:6
 msgid "View all"
@@ -747,24 +758,22 @@
 msgstr ""
 
 #: aasrp/templates/aasrp/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
-"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
-"tłumaczenia?"
 
 #: aasrp/templates/aasrp/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "Dołącz do naszego zespołu tłumaczy!"
+msgstr ""
 
 #: aasrp/templates/aasrp/partials/form/required-field-hint.html:5
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr "Pola z gwiazdką (*) są wymagane"
+msgstr ""
 
 #: aasrp/templates/aasrp/partials/link-add/form.html:7
 msgid "SRP link details"
 msgstr ""
 
 #: aasrp/templates/aasrp/partials/link-add/form.html:21
 msgid "Create link"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_srp-2.0.1/aasrp/locale/ru/LC_MESSAGES/django.mo` & `aa_srp-2.0.2/aasrp/locale/ru/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-srp/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "\n"
 "                            This SRP link still has "
 "%(number_pending_requests)s pending\n"
 "                            SRP request. Are you absolutely certain you want "
 "to mark\n"
@@ -306,20 +306,14 @@
 msgstr ""
 "Найдите ваш килл на {ZKILLBOARD_BASE_URL} или {EVETOOLS_KILLBOARD_BASE_URL} "
 "и скопируйте ссылку сюда."
 
 msgid "Fitted value (Ship and Fitting)"
 msgstr "Стоимость оснастки корабля (Корабль и оснастка)"
 
-msgid "Fleet"
-msgstr "Флот"
-
-msgid "Fleet ISK cost"
-msgstr "Стоимость флота ISK"
-
 msgid "Fleet commander"
 msgstr "Командир флота"
 
 msgid "Fleet name"
 msgstr "Название флота"
 
 msgid "Fleet time"
@@ -484,17 +478,14 @@
 
 msgid "SRP link \"{srp_link.srp_code}\" created"
 msgstr "SRP ссылка «{srp_link.srp_code}» создана"
 
 msgid "SRP link details"
 msgstr "Информация о SRP ссылке"
 
-msgid "SRP link edit"
-msgstr "Редактирование SRP ссылки"
-
 msgid "SRP link marked as completed"
 msgstr "SRP ссылка помечена как завершенная"
 
 msgid "SRP link name"
 msgstr "Название SRP ссылки"
 
 msgid "SRP link {srp_code} (re-)activated."
@@ -520,17 +511,14 @@
 
 msgid "SRP request"
 msgstr "SRP запрос"
 
 msgid "SRP request added"
 msgstr "SRP запрос добавлен"
 
-msgid "SRP request added."
-msgstr "SRP запрос добавлен."
-
 msgid "SRP request approved"
 msgstr "SRP запрос удовлетворен"
 
 msgid "SRP request details"
 msgstr "Детали SRP запроса"
 
 msgid "SRP request has been approved"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/ru/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/ru/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# Nikolay <nick.postnikov@gmail.com>, 2023.
-# Max <mark25@inbox.ru>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Nikolay <nick.postnikov@gmail.com>, 2023, 2024.
+# Max <mark25@inbox.ru>, 2023, 2024.
 # Dromiel <dimhry@yandex.ru>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 01:12+0100\n"
-"PO-Revision-Date: 2024-01-17 18:05+0000\n"
-"Last-Translator: Dromiel <dimhry@yandex.ru>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-srp/ru/>\n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-srp/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr "Компенсация боевых потерь (SRP)"
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
@@ -219,16 +219,15 @@
 msgid "Comment"
 msgstr "Комментарий"
 
 #: aasrp/form.py:223
 msgid ""
 "Please provide the reason why this former rejected SRP request is now "
 "accepted."
-msgstr ""
-"Укажите причину удовлетворения SRP запроса, который ранее был отклонен."
+msgstr "Укажите причину удовлетворения SRP запроса, который ранее был отклонен."
 
 #: aasrp/form.py:238
 msgid ""
 "Disable notifications. (Auth and Discord, if a relevant module is installed)"
 msgstr "Отключить уведомления. (Auth и Discord при установленных модулях)"
 
 #: aasrp/helper/character.py:48
```

### Comparing `aa_srp-2.0.1/aasrp/locale/sk/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

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
 "POT-Creation-Date: 2024-03-20 17:08+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-srp/pl/>\n"
+"Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
-">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr ""
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
@@ -38,55 +38,59 @@
 msgid "Requestor"
 msgstr ""
 
 #: aasrp/admin.py:229 aasrp/models.py:126 aasrp/models.py:183
 #: aasrp/templates/aasrp/partials/dashboard/srp-links.html:19
 #: aasrp/templates/aasrp/partials/request-srp/fleet-details.html:17
 msgid "Fleet type"
-msgstr ""
+msgstr "Typ floty"
 
 #: aasrp/admin.py:242 aasrp/models.py:117
 msgid "Is enabled"
-msgstr ""
+msgstr "Zaznaczony"
 
 #: aasrp/admin.py:257
 msgid "Activate selected fleet types"
 msgstr ""
 
 #: aasrp/admin.py:286
 #, python-brace-format
 msgid "Failed to activate {failed} fleet type"
 msgid_plural "Failed to activate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: aasrp/admin.py:296
 #, python-brace-format
 msgid "Activated {notifications_count} fleet type"
 msgid_plural "Activated {notifications_count} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: aasrp/admin.py:302
 msgid "Deactivate selected fleet types"
 msgstr ""
 
 #: aasrp/admin.py:331
 #, python-brace-format
 msgid "Failed to deactivate {failed} fleet type"
 msgid_plural "Failed to deactivate {failed} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: aasrp/admin.py:341
 #, python-brace-format
 msgid "Deactivated {notifications_count} fleet type"
 msgid_plural "Deactivated {notifications_count} fleet types"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #. Translators: This is the app name and version, which will appear in the Django Backend
 #: aasrp/apps.py:21
 #, python-brace-format
 msgid "AA Ship Replacement v{__version__}"
 msgstr ""
 
@@ -96,15 +100,15 @@
 "your request reviser.\n"
 "Please make sure to always add the SRP code and the request code with your "
 "inquiry."
 msgstr ""
 
 #: aasrp/form.py:37
 msgid "This field is mandatory"
-msgstr ""
+msgstr "To pole jest wymagane"
 
 #: aasrp/form.py:53
 #: aasrp/templates/aasrp/partials/request-srp/fleet-details.html:13
 #: aasrp/templates/aasrp/partials/view-requests/overview.html:27
 msgid "Fleet name"
 msgstr ""
 
@@ -141,15 +145,15 @@
 msgstr ""
 
 #: aasrp/form.py:114 aasrp/models.py:348 aasrp/models.py:442
 #: aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html:82
 #: aasrp/templates/aasrp/dashboard.html:97
 #: aasrp/templates/aasrp/view-requests.html:81
 msgid "Additional information"
-msgstr ""
+msgstr "Dodatkowe informacje"
 
 #: aasrp/form.py:116
 msgid ""
 "Please tell us about the circumstances of your untimely demise. Who was the "
 "FC, what doctrine was called, have changes to the fit been requested and so "
 "on. Be as detailed as you can."
 msgstr ""
@@ -291,15 +295,15 @@
 
 #: aasrp/models.py:116
 msgid "Whether this fleet type is active or not"
 msgstr ""
 
 #: aasrp/models.py:127
 msgid "Fleet types"
-msgstr ""
+msgstr "Typy floty"
 
 #: aasrp/models.py:150
 msgid "Active"
 msgstr ""
 
 #: aasrp/models.py:151
 msgid "Closed"
@@ -323,15 +327,15 @@
 #: aasrp/templates/aasrp/partials/view-requests/overview.html:50
 msgid "SRP code"
 msgstr ""
 
 #: aasrp/models.py:169
 #: aasrp/templates/aasrp/partials/view-requests/overview.html:32
 msgid "Fleet commander"
-msgstr ""
+msgstr "Dowódca floty"
 
 #: aasrp/models.py:182
 msgid "The SRP link fleet type, if it's set"
 msgstr ""
 
 #: aasrp/models.py:188
 msgid "AAR link"
@@ -383,15 +387,15 @@
 #: aasrp/templates/aasrp/view-requests.html:69
 #: aasrp/templates/aasrp/view-requests.html:78
 msgid "Character"
 msgstr ""
 
 #: aasrp/models.py:333 aasrp/models.py:342
 msgid "Ship type"
-msgstr ""
+msgstr "Typ statku"
 
 #: aasrp/models.py:354 aasrp/templates/aasrp/dashboard.html:73
 #: aasrp/templates/aasrp/view-requests.html:67
 msgid "Request status"
 msgstr ""
 
 #: aasrp/models.py:356
@@ -613,15 +617,15 @@
 #: aasrp/templates/aasrp/modals/view-requests/reject-request.html:35
 msgid "Cancel"
 msgstr ""
 
 #: aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html:25
 #: aasrp/templates/aasrp/modals/view-requests/delete-request.html:29
 msgid "Delete"
-msgstr ""
+msgstr "Usuń"
 
 #: aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html:25
 msgid "Disable"
 msgstr ""
 
 #: aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html:25
 msgid "Enable"
@@ -670,14 +674,15 @@
 "%(number_pending_requests)s pending\n"
 "                            SRP requests. Are you absolutely certain you "
 "want to mark\n"
 "                            this SRP link as completed?\n"
 "                        "
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: aasrp/templates/aasrp/modals/view-requests/reject-request.html:18
 msgid "Are you sure you want to reject this SRP request?"
 msgstr ""
 
 #: aasrp/templates/aasrp/partials/dashboard/navigation.html:6
 msgid "View all"
@@ -747,22 +752,24 @@
 msgstr ""
 
 #: aasrp/templates/aasrp/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
+"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
+"tłumaczenia?"
 
 #: aasrp/templates/aasrp/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr ""
+msgstr "Dołącz do naszego zespołu tłumaczy!"
 
 #: aasrp/templates/aasrp/partials/form/required-field-hint.html:5
 msgid "Fields marked with an asterisk (*) are mandatory"
-msgstr ""
+msgstr "Pola z gwiazdką (*) są wymagane"
 
 #: aasrp/templates/aasrp/partials/link-add/form.html:7
 msgid "SRP link details"
 msgstr ""
 
 #: aasrp/templates/aasrp/partials/link-add/form.html:21
 msgid "Create link"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_srp-2.0.1/aasrp/locale/uk/LC_MESSAGES/django.mo` & `aa_srp-2.0.2/aasrp/locale/uk/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-srp/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Activate selected fleet types"
 msgstr "Активувати обрані типи флотів"
 
 msgid "Creator"
 msgstr "Автор"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/uk/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/uk/LC_MESSAGES/django.po`

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
 "POT-Creation-Date: 2024-03-16 01:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
 "Last-Translator: \"Andrii M.\" <elfleg0las88@gmail.com>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-srp/uk/>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-srp/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr "Компенсація корабля"
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
```

### Comparing `aa_srp-2.0.1/aasrp/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_srp-2.0.2/aasrp/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-srp/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "\n"
 "                            This SRP link still has "
 "%(number_pending_requests)s pending\n"
 "                            SRP request. Are you absolutely certain you want "
 "to mark\n"
```

### Comparing `aa_srp-2.0.1/aasrp/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_srp-2.0.2/aasrp/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 # Dehao Wu <wudehao2000@163.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 01:12+0100\n"
-"PO-Revision-Date: 2024-03-22 12:56+0000\n"
+"PO-Revision-Date: 2024-05-10 14:11+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-srp/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aasrp/__init__.py:9 aasrp/templates/aasrp/base.html:6
 #: aasrp/templates/aasrp/base.html:10
 msgid "Ship Replacement"
 msgstr "补损"
 
 #: aasrp/admin.py:140 aasrp/models.py:199 aasrp/models.py:322
@@ -133,16 +133,16 @@
 
 #: aasrp/form.py:107
 #, python-brace-format
 msgid ""
 "Find your kill mail on {ZKILLBOARD_BASE_URL} or "
 "{EVETOOLS_KILLBOARD_BASE_URL} and paste the link here."
 msgstr ""
-"找到你的舰船KB，点击右上角三个点，点击 {ZKILLBOARD_BASE_URL} 并将其复制到这"
-"里，或者 {EVETOOLS_KILLBOARD_BASE_URL} 复制到这里。"
+"找到你的舰船KB，点击右上角三个点，点击 {ZKILLBOARD_BASE_URL} "
+"并将其复制到这里，或者 {EVETOOLS_KILLBOARD_BASE_URL} 复制到这里。"
 
 #: aasrp/form.py:114 aasrp/models.py:348 aasrp/models.py:442
 #: aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html:82
 #: aasrp/templates/aasrp/dashboard.html:97
 #: aasrp/templates/aasrp/view-requests.html:81
 msgid "Additional information"
 msgstr "附加说明"
@@ -511,17 +511,16 @@
 msgstr "总价值(舰船，装配，货柜中的货物)"
 
 #: aasrp/models.py:567
 msgid ""
 "The source for the loss value of a killmail. Fitted value is the value of "
 "the ship and its fitting. Total value is the value of the ship, its fitting "
 "and the cargo. (Default: Total value)"
-msgstr ""
-"一个击毁报告的损失价值来源。装配价值是指这条船和它装备的价值。总价值是指船"
-"只、其装备还有货舱内货物的价值。(默认:总价值)"
+msgstr "一个击毁报告的损失价值来源。装配价值是指这条船和它装备的价值。总价值是指船只"
+"、其装备还有货舱内货物的价值。(默认:总价值)"
 
 #: aasrp/models.py:584
 msgid "Setting"
 msgstr "设置"
 
 #: aasrp/models.py:585
 #: aasrp/templates/aasrp/partials/dashboard/tabs-navigation.html:41
@@ -658,16 +657,17 @@
 "                        close it for good? Be aware that once it's "
 "completed,\n"
 "                        your pilots can no longer file SRP requests for\n"
 "                        this link / fleet.\n"
 "                    "
 msgstr ""
 "\n"
-"                        你确定你要将这个舰船补损链接标记为已完成并将其关闭"
-"吗？一旦完成，这个飞行员将不能再次使用这个链接递交舰船补损请求\n"
+"                        "
+"你确定你要将这个舰船补损链接标记为已完成并将其关闭吗？一旦完成，"
+"这个飞行员将不能再次使用这个链接递交舰船补损请求\n"
 "                    "
 
 #: aasrp/templates/aasrp/modals/view-requests/mark-complete.html:27
 #, python-format
 msgid ""
 "\n"
 "                            This SRP link still has "
@@ -682,16 +682,16 @@
 "%(number_pending_requests)s pending\n"
 "                            SRP requests. Are you absolutely certain you "
 "want to mark\n"
 "                            this SRP link as completed?\n"
 "                        "
 msgstr[0] ""
 "\n"
-"                            这个舰船补损链接仍然"
-"有%(number_pending_requests)s 在发送\n"
+"                            这个舰船补损链接仍然有%(number_pending_requests)"
+"s 在发送\n"
 "舰船请求。 你确定要将其标记成已完成状态吗？\n"
 "                        "
 
 #: aasrp/templates/aasrp/modals/view-requests/reject-request.html:18
 msgid "Are you sure you want to reject this SRP request?"
 msgstr "你确定你要拒绝这个舰船更换请求吗？"
 
@@ -908,25 +908,24 @@
 #: aasrp/views/general.py:400
 #, python-brace-format
 msgid ""
 "Your kill mail link ({submitted_killmail_link}) is invalid or the zKillboard "
 "API is not answering at the moment. Please make sure you are using either "
 "{ZKILLBOARD_BASE_URL} or {EVETOOLS_KILLBOARD_BASE_URL}"
 msgstr ""
-"你的击杀报告链接 {submitted_killmail_link} 是无效的或者KB网上目前没有你的数"
-"据。请确保你使用了正确的 {ZKILLBOARD_BASE_URL} 或者是 "
-"{EVETOOLS_KILLBOARD_BASE_URL}"
+"你的击杀报告链接 {submitted_killmail_link} "
+"是无效的或者KB网上目前没有你的数据。请确保你使用了正确的 "
+"{ZKILLBOARD_BASE_URL} 或者是 {EVETOOLS_KILLBOARD_BASE_URL}"
 
 #: aasrp/views/general.py:431
 #, python-brace-format
 msgid ""
 "Character {victim_id} does not belong to your Auth account. Please add this "
 "character as an alt to your main and try again."
-msgstr ""
-"角色 {victim_id} 不属于你的Auth账户。请将此角色添加到主角色中，然后再试一次。"
+msgstr "角色 {victim_id} 不属于你的Auth账户。请将此角色添加到主角色中，然后再试一次。"
 
 #: aasrp/views/general.py:484
 msgid "SRP link marked as completed"
 msgstr "舰船补损链接已被标记成完成状态"
 
 #: aasrp/views/general.py:570
 #, python-brace-format
```

### Comparing `aa_srp-2.0.1/aasrp/management/commands/aasrp_load_eve.py` & `aa_srp-2.0.2/aasrp/management/commands/aasrp_load_eve.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/management/commands/aasrp_migrate_srp_data.py` & `aa_srp-2.0.2/aasrp/management/commands/aasrp_migrate_srp_data.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0001_initial.py` & `aa_srp-2.0.2/aasrp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0002_relations_update.py` & `aa_srp-2.0.2/aasrp/migrations/0002_relations_update.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0004_aasrpusersettings.py` & `aa_srp-2.0.2/aasrp/migrations/0004_aasrpusersettings.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0005_insurance.py` & `aa_srp-2.0.2/aasrp/migrations/0005_insurance.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0006_related_names.py` & `aa_srp-2.0.2/aasrp/migrations/0006_related_names.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0007_aasrprequestcomment_comment_time_and_more.py` & `aa_srp-2.0.2/aasrp/migrations/0007_aasrprequestcomment_comment_time_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0008_aasrprequestcomment_new_status_and_more.py` & `aa_srp-2.0.2/aasrp/migrations/0008_aasrprequestcomment_new_status_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0009_add_fleet_type_to_srp_link.py` & `aa_srp-2.0.2/aasrp/migrations/0009_add_fleet_type_to_srp_link.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0010_model_changes.py` & `aa_srp-2.0.2/aasrp/migrations/0010_model_changes.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0011_default_settings.py` & `aa_srp-2.0.2/aasrp/migrations/0011_default_settings.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0012_alter_fleettype_options_alter_insurance_options_and_more.py` & `aa_srp-2.0.2/aasrp/migrations/0012_alter_fleettype_options_alter_insurance_options_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/migrations/0013_setting_loss_value_source.py` & `aa_srp-2.0.2/aasrp/migrations/0013_setting_loss_value_source.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/css/aa-srp.css` & `aa_srp-2.0.2/aasrp/static/aasrp/css/aa-srp.css`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/css/aa-srp.min.css` & `aa_srp-2.0.2/aasrp/static/aasrp/css/aa-srp.min.css`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/css/aa-srp.min.css.map` & `aa_srp-2.0.2/aasrp/static/aasrp/css/aa-srp.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-dashboard.js` & `aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-dashboard.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js` & `aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js.map` & `aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-dashboard.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-view-requests.js` & `aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-view-requests.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js` & `aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js.map` & `aa_srp-2.0.2/aasrp/static/aasrp/javascript/aa-srp-view-requests.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.css` & `aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.css`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css` & `aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css.map` & `aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/css/bootstrap-editable.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/loading.gif` & `aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/img/loading.gif`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.js` & `aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js` & `aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js.map` & `aa_srp-2.0.2/aasrp/static/aasrp/libs/x-editable/1.5.4/bootstrap5-editable/js/bootstrap-editable.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/base.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/base.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/dashboard.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/dashboard.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/link-add.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/link-add.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/view-requests.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/view-requests.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/ajax-render/srp-request-additional-information.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/modals/dashboard/delete-srp-link.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/modals/dashboard/disable-srp-link.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/modals/dashboard/enable-srp-link.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/accept-rejected-request.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/accept-rejected-request.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/accept-request.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/accept-request.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/delete-request.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/delete-request.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/mark-complete.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/mark-complete.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/reject-request.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/reject-request.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/modals/view-requests/request-details.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/modals/view-requests/request-details.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/navigation.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/navigation.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/srp-links.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/srp-links.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/tabs-navigation.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/tabs-navigation.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/user-settings.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/user-settings.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/dashboard/user-srp-requests.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/dashboard/user-srp-requests.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/link-add/form.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/link-add/form.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/link-edit/form.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/link-edit/form.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/request-srp/fleet-details.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/request-srp/fleet-details.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/request-srp/form.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/request-srp/form.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/view-requests/overview.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/view-requests/overview.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templates/aasrp/partials/view-requests/requests.html` & `aa_srp-2.0.2/aasrp/templates/aasrp/partials/view-requests/requests.html`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/templatetags/aasrp.py` & `aa_srp-2.0.2/aasrp/templatetags/aasrp.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/tests/test_access.py` & `aa_srp-2.0.2/aasrp/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/tests/test_auth_hooks.py` & `aa_srp-2.0.2/aasrp/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/tests/test_helper_character.py` & `aa_srp-2.0.2/aasrp/tests/test_helper_character.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/tests/test_installed_modules.py` & `aa_srp-2.0.2/aasrp/tests/test_installed_modules.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/tests/test_model_setting.py` & `aa_srp-2.0.2/aasrp/tests/test_model_setting.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/tests/test_templatetags.py` & `aa_srp-2.0.2/aasrp/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/tests/utils.py` & `aa_srp-2.0.2/aasrp/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/views/ajax.py` & `aa_srp-2.0.2/aasrp/views/ajax.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/aasrp/views/general.py` & `aa_srp-2.0.2/aasrp/views/general.py`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/LICENSE` & `aa_srp-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/README.md` & `aa_srp-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/pyproject.toml` & `aa_srp-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_srp-2.0.1/PKG-INFO` & `aa_srp-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-srp
-Version: 2.0.1
+Version: 2.0.2
 Summary: Improved SRP Module for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-srp/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-srp/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-srp
 Project-URL: Source, https://github.com/ppfeufer/aa-srp.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-srp/issues
```

