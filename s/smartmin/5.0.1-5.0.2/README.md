# Comparing `tmp/smartmin-5.0.1.tar.gz` & `tmp/smartmin-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartmin-5.0.1.tar", max compression
+gzip compressed data, was "smartmin-5.0.2.tar", max compression
```

## Comparing `smartmin-5.0.1.tar` & `smartmin-5.0.2.tar`

### file list

```diff
@@ -1,143 +1,143 @@
--rw-r--r--   0        0        0     1477 2024-04-17 12:06:57.596131 smartmin-5.0.1/LICENSE
--rw-r--r--   0        0        0     1700 2024-04-17 12:06:57.596131 smartmin-5.0.1/README.md
--rw-r--r--   0        0        0     1500 2024-04-17 12:06:57.596131 smartmin-5.0.1/pyproject.toml
--rw-r--r--   0        0        0       63 2024-04-17 12:06:57.596131 smartmin-5.0.1/smartmin/__init__.py
--rw-r--r--   0        0        0      748 2024-04-17 12:06:57.596131 smartmin-5.0.1/smartmin/backends.py
--rw-r--r--   0        0        0        0 2024-04-17 12:06:57.596131 smartmin-5.0.1/smartmin/csv_imports/__init__.py
--rw-r--r--   0        0        0     2790 2024-04-17 12:06:57.596131 smartmin-5.0.1/smartmin/csv_imports/migrations/0001_initial.py
--rw-r--r--   0        0        0      562 2024-04-17 12:06:57.596131 smartmin-5.0.1/smartmin/csv_imports/migrations/0002_auto_20161118_1920.py
--rw-r--r--   0        0        0      366 2024-04-17 12:06:57.596131 smartmin-5.0.1/smartmin/csv_imports/migrations/0003_importtask_task_status.py
--rw-r--r--   0        0        0      902 2024-04-17 12:06:57.596131 smartmin-5.0.1/smartmin/csv_imports/migrations/0004_auto_20170223_0917.py
--rw-r--r--   0        0        0     1183 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/csv_imports/migrations/0005_alter_importtask_created_by_and_more.py
--rw-r--r--   0        0        0        0 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/csv_imports/migrations/__init__.py
--rw-r--r--   0        0        0     2141 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/csv_imports/models.py
--rw-r--r--   0        0        0     1314 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/csv_imports/tasks.py
--rw-r--r--   0        0        0     1029 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/csv_imports/tests.py
--rw-r--r--   0        0        0      105 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/csv_imports/urls.py
--rw-r--r--   0        0        0      738 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/csv_imports/views.py
--rw-r--r--   0        0        0      696 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/email.py
--rw-r--r--   0        0        0     5887 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/management/commands/__init__.py
--rw-r--r--   0        0        0     8150 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/management/commands/collect_sql.py
--rw-r--r--   0        0        0     4412 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/management/commands/migrate_manual.py
--rw-r--r--   0        0        0     5067 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/management/tests.py
--rw-r--r--   0        0        0      405 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/middleware.py
--rw-r--r--   0        0        0      722 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/mixins.py
--rw-r--r--   0        0        0    13387 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/models.py
--rw-r--r--   0        0        0     1146 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/pdf.py
--rw-r--r--   0        0        0     1086 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/perms.py
--rw-r--r--   0        0        0    22818 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/css/bootstrap-datepicker3.css
--rwxr-xr-x   0        0        0    26132 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/css/bootstrap-theme.css
--rwxr-xr-x   0        0        0   147430 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/css/bootstrap.css
--rw-r--r--   0        0        0     3600 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/css/smartmin_styles.css
--rw-r--r--   0        0        0      194 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/css/styles.css
--rw-r--r--   0        0        0    20127 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0   108738 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    45404 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23424 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0    18028 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.woff2
--rwxr-xr-x   0        0        0      295 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/active.png
--rw-r--r--   0        0        0    45578 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/background.jpg
--rwxr-xr-x   0        0        0      277 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/button.png
--rw-r--r--   0        0        0      488 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/check.png
--rwxr-xr-x   0        0        0     4352 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/glyphicons-halflings-white.png
--rwxr-xr-x   0        0        0     4352 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/glyphicons-halflings.png
--rw-r--r--   0        0        0     1252 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/in.png
--rw-r--r--   0        0        0     1268 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/loc.png
--rw-r--r--   0        0        0     1928 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/nyaruka.png
--rw-r--r--   0        0        0     1252 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/out.png
--rw-r--r--   0        0        0       80 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/arrow-down.gif
--rw-r--r--   0        0        0      838 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/arrow-up.gif
--rw-r--r--   0        0        0       58 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/changelist-bg.gif
--rw-r--r--   0        0        0       75 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/changelist-bg_rtl.gif
--rw-r--r--   0        0        0      199 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/chooser-bg.gif
--rw-r--r--   0        0        0      212 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/chooser_stacked-bg.gif
--rw-r--r--   0        0        0      843 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/default-bg-reverse.gif
--rw-r--r--   0        0        0      844 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/default-bg.gif
--rw-r--r--   0        0        0       45 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/deleted-overlay.gif
--rw-r--r--   0        0        0      176 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon-no.gif
--rw-r--r--   0        0        0      130 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon-unknown.gif
--rw-r--r--   0        0        0      299 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon-yes.gif
--rw-r--r--   0        0        0      119 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon_addlink.gif
--rw-r--r--   0        0        0      145 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon_alert.gif
--rw-r--r--   0        0        0      192 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon_calendar.gif
--rw-r--r--   0        0        0      119 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon_changelink.gif
--rw-r--r--   0        0        0      390 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon_clock.gif
--rw-r--r--   0        0        0      181 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon_deletelink.gif
--rw-r--r--   0        0        0      319 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon_error.gif
--rw-r--r--   0        0        0      667 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon_searchbox.png
--rw-r--r--   0        0        0      341 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin/icon_success.gif
--rw-r--r--   0        0        0      477 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/inline-delete-8bit.png
--rw-r--r--   0        0        0      781 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/inline-delete.png
--rw-r--r--   0        0        0      447 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/inline-restore-8bit.png
--rw-r--r--   0        0        0      623 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/inline-restore.png
--rw-r--r--   0        0        0      102 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/inline-splitter-bg.gif
--rw-r--r--   0        0        0     3951 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/loading.gif
--rw-r--r--   0        0        0      116 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/nav-bg-grabber.gif
--rw-r--r--   0        0        0      186 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/nav-bg-reverse.gif
--rw-r--r--   0        0        0      273 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/nav-bg.gif
--rw-r--r--   0        0        0      606 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/selector-add.gif
--rw-r--r--   0        0        0      358 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/selector-addall.gif
--rw-r--r--   0        0        0      398 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/selector-remove.gif
--rw-r--r--   0        0        0      355 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/selector-removeall.gif
--rw-r--r--   0        0        0      552 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/selector-search.gif
--rw-r--r--   0        0        0      612 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/selector_stacked-add.gif
--rw-r--r--   0        0        0      401 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/selector_stacked-remove.gif
--rw-r--r--   0        0        0      197 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/tool-left.gif
--rw-r--r--   0        0        0      203 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/tool-left_over.gif
--rw-r--r--   0        0        0      198 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/tool-right.gif
--rw-r--r--   0        0        0      200 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/tool-right_over.gif
--rw-r--r--   0        0        0      932 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/tooltag-add.gif
--rw-r--r--   0        0        0      336 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/tooltag-add_over.gif
--rw-r--r--   0        0        0      351 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/tooltag-arrowright.gif
--rw-r--r--   0        0        0      354 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/smartmin/tooltag-arrowright_over.gif
--rw-r--r--   0        0        0     1795 2024-04-17 12:06:57.600131 smartmin-5.0.1/smartmin/static/img/smartmin.png
--rw-r--r--   0        0        0      837 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/sort.gif
--rw-r--r--   0        0        0      987 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/sort.png
--rw-r--r--   0        0        0     3606 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/sort_asc.png
--rw-r--r--   0        0        0      980 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/img/sort_dsc.png
--rw-r--r--   0        0        0    58701 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/js/bootstrap-datepicker.js
--rwxr-xr-x   0        0        0    36816 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/js/bootstrap.min.js
--rw-r--r--   0        0        0     6335 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/js/jquery.pjax.js
--rw-r--r--   0        0        0    97163 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/js/libs/jquery-1.12.4.min.js
--rw-r--r--   0        0        0    95786 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/js/libs/jquery.min.js
--rw-r--r--   0        0        0     5056 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/js/libs/jquery.url.js
--rw-r--r--   0        0        0        0 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/js/scripts.js
--rw-r--r--   0        0        0     2552 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/static/top.png
--rw-r--r--   0        0        0       69 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/base.html
--rw-r--r--   0        0        0      954 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/csv_imports/importtask_read.html
--rw-r--r--   0        0        0     5202 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/frame.html
--rw-r--r--   0        0        0     3440 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/base.html
--rw-r--r--   0        0        0       36 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/create.html
--rw-r--r--   0        0        0      793 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/delete_confirm.html
--rw-r--r--   0        0        0     1211 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/field.html
--rw-r--r--   0        0        0     2126 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/form.html
--rw-r--r--   0        0        0     5320 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/list.html
--rw-r--r--   0        0        0      131 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/pjax.html
--rw-r--r--   0        0        0     1098 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/read.html
--rw-r--r--   0        0        0      501 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/update.html
--rw-r--r--   0        0        0     1327 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/login.html
--rw-r--r--   0        0        0      312 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/no_user_email.txt
--rw-r--r--   0        0        0      400 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/user_email.txt
--rw-r--r--   0        0        0      125 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/user_expired.html
--rw-r--r--   0        0        0     1374 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/user_failed.html
--rw-r--r--   0        0        0      234 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/user_forget.html
--rw-r--r--   0        0        0      770 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/user_list.html
--rw-r--r--   0        0        0      375 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/user_newpassword.html
--rw-r--r--   0        0        0       34 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/user_recover.html
--rw-r--r--   0        0        0      523 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templates/smartmin/users/user_update.html
--rw-r--r--   0        0        0        0 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templatetags/__init__.py
--rw-r--r--   0        0        0     8428 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/templatetags/smartmin.py
--rw-r--r--   0        0        0     7874 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/tests.py
--rw-r--r--   0        0        0        0 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/users/__init__.py
--rw-r--r--   0        0        0     1208 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/users/middleware.py
--rw-r--r--   0        0        0     1917 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/users/migrations/0001_initial.py
--rw-r--r--   0        0        0      483 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/users/migrations/0002_remove_failed_logins.py
--rw-r--r--   0        0        0      548 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/users/migrations/0003_auto_20210219_1548.py
--rw-r--r--   0        0        0        0 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/users/migrations/__init__.py
--rw-r--r--   0        0        0     2663 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/users/models.py
--rw-r--r--   0        0        0      561 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/users/urls.py
--rw-r--r--   0        0        0    21127 2024-04-17 12:06:57.604131 smartmin-5.0.1/smartmin/users/views.py
--rw-r--r--   0        0        0    50992 2024-04-17 12:06:57.608131 smartmin-5.0.1/smartmin/views.py
--rw-r--r--   0        0        0     2192 2024-04-17 12:06:57.608131 smartmin-5.0.1/smartmin/widgets.py
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 smartmin-5.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1477 2024-05-16 19:09:43.849923 smartmin-5.0.2/LICENSE
+-rw-r--r--   0        0        0     1627 2024-05-16 19:09:43.849923 smartmin-5.0.2/README.md
+-rw-r--r--   0        0        0     1500 2024-05-16 19:09:43.849923 smartmin-5.0.2/pyproject.toml
+-rw-r--r--   0        0        0       63 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/__init__.py
+-rw-r--r--   0        0        0      748 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/backends.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/__init__.py
+-rw-r--r--   0        0        0     2790 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/migrations/0001_initial.py
+-rw-r--r--   0        0        0      562 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/migrations/0002_auto_20161118_1920.py
+-rw-r--r--   0        0        0      366 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/migrations/0003_importtask_task_status.py
+-rw-r--r--   0        0        0      902 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/migrations/0004_auto_20170223_0917.py
+-rw-r--r--   0        0        0     1183 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/migrations/0005_alter_importtask_created_by_and_more.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/migrations/__init__.py
+-rw-r--r--   0        0        0     2141 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/models.py
+-rw-r--r--   0        0        0     1314 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/tasks.py
+-rw-r--r--   0        0        0     1029 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/tests.py
+-rw-r--r--   0        0        0      105 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/urls.py
+-rw-r--r--   0        0        0      738 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/csv_imports/views.py
+-rw-r--r--   0        0        0      696 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/email.py
+-rw-r--r--   0        0        0     5887 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/management/commands/__init__.py
+-rw-r--r--   0        0        0     8150 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/management/commands/collect_sql.py
+-rw-r--r--   0        0        0     4412 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/management/commands/migrate_manual.py
+-rw-r--r--   0        0        0     5067 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/management/tests.py
+-rw-r--r--   0        0        0      405 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/middleware.py
+-rw-r--r--   0        0        0      722 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/mixins.py
+-rw-r--r--   0        0        0    13387 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/models.py
+-rw-r--r--   0        0        0     1146 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/pdf.py
+-rw-r--r--   0        0        0     1086 2024-05-16 19:09:43.849923 smartmin-5.0.2/smartmin/perms.py
+-rw-r--r--   0        0        0    22818 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/css/bootstrap-datepicker3.css
+-rwxr-xr-x   0        0        0    26132 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/css/bootstrap-theme.css
+-rwxr-xr-x   0        0        0   147430 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/css/bootstrap.css
+-rw-r--r--   0        0        0     3600 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/css/smartmin_styles.css
+-rw-r--r--   0        0        0      194 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/css/styles.css
+-rw-r--r--   0        0        0    20127 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0   108738 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    45404 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23424 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    18028 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.woff2
+-rwxr-xr-x   0        0        0      295 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/active.png
+-rw-r--r--   0        0        0    45578 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/background.jpg
+-rwxr-xr-x   0        0        0      277 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/button.png
+-rw-r--r--   0        0        0      488 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/check.png
+-rwxr-xr-x   0        0        0     4352 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/glyphicons-halflings-white.png
+-rwxr-xr-x   0        0        0     4352 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/glyphicons-halflings.png
+-rw-r--r--   0        0        0     1252 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/in.png
+-rw-r--r--   0        0        0     1268 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/loc.png
+-rw-r--r--   0        0        0     1928 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/nyaruka.png
+-rw-r--r--   0        0        0     1252 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/out.png
+-rw-r--r--   0        0        0       80 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/arrow-down.gif
+-rw-r--r--   0        0        0      838 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/arrow-up.gif
+-rw-r--r--   0        0        0       58 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/changelist-bg.gif
+-rw-r--r--   0        0        0       75 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/changelist-bg_rtl.gif
+-rw-r--r--   0        0        0      199 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/chooser-bg.gif
+-rw-r--r--   0        0        0      212 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/chooser_stacked-bg.gif
+-rw-r--r--   0        0        0      843 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/default-bg-reverse.gif
+-rw-r--r--   0        0        0      844 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/default-bg.gif
+-rw-r--r--   0        0        0       45 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/deleted-overlay.gif
+-rw-r--r--   0        0        0      176 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon-no.gif
+-rw-r--r--   0        0        0      130 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon-unknown.gif
+-rw-r--r--   0        0        0      299 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon-yes.gif
+-rw-r--r--   0        0        0      119 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon_addlink.gif
+-rw-r--r--   0        0        0      145 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon_alert.gif
+-rw-r--r--   0        0        0      192 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon_calendar.gif
+-rw-r--r--   0        0        0      119 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon_changelink.gif
+-rw-r--r--   0        0        0      390 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon_clock.gif
+-rw-r--r--   0        0        0      181 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon_deletelink.gif
+-rw-r--r--   0        0        0      319 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon_error.gif
+-rw-r--r--   0        0        0      667 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon_searchbox.png
+-rw-r--r--   0        0        0      341 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/icon_success.gif
+-rw-r--r--   0        0        0      477 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/inline-delete-8bit.png
+-rw-r--r--   0        0        0      781 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/inline-delete.png
+-rw-r--r--   0        0        0      447 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/inline-restore-8bit.png
+-rw-r--r--   0        0        0      623 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/inline-restore.png
+-rw-r--r--   0        0        0      102 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/inline-splitter-bg.gif
+-rw-r--r--   0        0        0     3951 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/loading.gif
+-rw-r--r--   0        0        0      116 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/nav-bg-grabber.gif
+-rw-r--r--   0        0        0      186 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/nav-bg-reverse.gif
+-rw-r--r--   0        0        0      273 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/nav-bg.gif
+-rw-r--r--   0        0        0      606 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/selector-add.gif
+-rw-r--r--   0        0        0      358 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/selector-addall.gif
+-rw-r--r--   0        0        0      398 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/selector-remove.gif
+-rw-r--r--   0        0        0      355 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/selector-removeall.gif
+-rw-r--r--   0        0        0      552 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/selector-search.gif
+-rw-r--r--   0        0        0      612 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/selector_stacked-add.gif
+-rw-r--r--   0        0        0      401 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/selector_stacked-remove.gif
+-rw-r--r--   0        0        0      197 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/tool-left.gif
+-rw-r--r--   0        0        0      203 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/tool-left_over.gif
+-rw-r--r--   0        0        0      198 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/tool-right.gif
+-rw-r--r--   0        0        0      200 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/tool-right_over.gif
+-rw-r--r--   0        0        0      932 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/tooltag-add.gif
+-rw-r--r--   0        0        0      336 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/tooltag-add_over.gif
+-rw-r--r--   0        0        0      351 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/tooltag-arrowright.gif
+-rw-r--r--   0        0        0      354 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin/tooltag-arrowright_over.gif
+-rw-r--r--   0        0        0     1795 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/smartmin.png
+-rw-r--r--   0        0        0      837 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/sort.gif
+-rw-r--r--   0        0        0      987 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/sort.png
+-rw-r--r--   0        0        0     3606 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/sort_asc.png
+-rw-r--r--   0        0        0      980 2024-05-16 19:09:43.853923 smartmin-5.0.2/smartmin/static/img/sort_dsc.png
+-rw-r--r--   0        0        0    58701 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/static/js/bootstrap-datepicker.js
+-rwxr-xr-x   0        0        0    36816 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0     6335 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/static/js/jquery.pjax.js
+-rw-r--r--   0        0        0    97163 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/static/js/libs/jquery-1.12.4.min.js
+-rw-r--r--   0        0        0    95786 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/static/js/libs/jquery.min.js
+-rw-r--r--   0        0        0     5056 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/static/js/libs/jquery.url.js
+-rw-r--r--   0        0        0        0 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/static/js/scripts.js
+-rw-r--r--   0        0        0     2552 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/static/top.png
+-rw-r--r--   0        0        0       69 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/base.html
+-rw-r--r--   0        0        0      954 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/csv_imports/importtask_read.html
+-rw-r--r--   0        0        0     5202 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/frame.html
+-rw-r--r--   0        0        0     3440 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/base.html
+-rw-r--r--   0        0        0       36 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/create.html
+-rw-r--r--   0        0        0      793 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/delete_confirm.html
+-rw-r--r--   0        0        0     1211 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/field.html
+-rw-r--r--   0        0        0     2126 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/form.html
+-rw-r--r--   0        0        0     5320 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/list.html
+-rw-r--r--   0        0        0      131 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/pjax.html
+-rw-r--r--   0        0        0     1098 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/read.html
+-rw-r--r--   0        0        0      501 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/update.html
+-rw-r--r--   0        0        0     1327 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/login.html
+-rw-r--r--   0        0        0      312 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/no_user_email.txt
+-rw-r--r--   0        0        0      400 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/user_email.txt
+-rw-r--r--   0        0        0      125 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/user_expired.html
+-rw-r--r--   0        0        0     1374 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/user_failed.html
+-rw-r--r--   0        0        0      234 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/user_forget.html
+-rw-r--r--   0        0        0      770 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/user_list.html
+-rw-r--r--   0        0        0      375 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/user_newpassword.html
+-rw-r--r--   0        0        0       34 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/user_recover.html
+-rw-r--r--   0        0        0      523 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templates/smartmin/users/user_update.html
+-rw-r--r--   0        0        0        0 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templatetags/__init__.py
+-rw-r--r--   0        0        0     8428 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/templatetags/smartmin.py
+-rw-r--r--   0        0        0     7874 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/tests.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/users/__init__.py
+-rw-r--r--   0        0        0     1208 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/users/middleware.py
+-rw-r--r--   0        0        0     1917 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/users/migrations/0001_initial.py
+-rw-r--r--   0        0        0      483 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/users/migrations/0002_remove_failed_logins.py
+-rw-r--r--   0        0        0      548 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/users/migrations/0003_auto_20210219_1548.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/users/migrations/__init__.py
+-rw-r--r--   0        0        0     2663 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/users/models.py
+-rw-r--r--   0        0        0      561 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/users/urls.py
+-rw-r--r--   0        0        0    21127 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/users/views.py
+-rw-r--r--   0        0        0    51106 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/views.py
+-rw-r--r--   0        0        0     2192 2024-05-16 19:09:43.857923 smartmin-5.0.2/smartmin/widgets.py
+-rw-r--r--   0        0        0     2709 1970-01-01 00:00:00.000000 smartmin-5.0.2/PKG-INFO
```

### Comparing `smartmin-5.0.1/LICENSE` & `smartmin-5.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/README.md` & `smartmin-5.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 - CRUDL operations at the object level, that is, Create, Read, Update, Delete and List, permissions and views are based 
   around this
 - URL automapping via the the CRUDL objects, this should keep things very very DRY
 
 About Versions
 ==============
 
-Smartmin tries to stay in lock step with the latest Django versions. With each new Django LTS release we will release
+Smartmin tries to stay in lock step with the latest Django versions. With each new major Django release we will release
 a new Smartmin major version and we will reserve major changes (possibly breaking backwards compatibility) for such 
-releases. This includes updating to the latest version of Twitter Bootstrap.
+releases.
 
-The latest version is the 3.* series which supports the Django 3.2 LTS and 2.2 LTS.
+The latest version is the 5.* series which supports the Django 5.0 and 4.2.
 
 About
 =====
 
 The full documentation can be found at: http://readthedocs.org/docs/smartmin/en/latest/
 
 The official source code repository is: http://www.github.com/nyaruka/smartmin/
```

### Comparing `smartmin-5.0.1/pyproject.toml` & `smartmin-5.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartmin"
-version = "5.0.1"
+version = "5.0.2"
 description = "Scaffolding system for Django object management."
 authors = ["Nyaruka Ltd <code@nyaruka.com>"]
 readme = "README.md"
 license = "BSD"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
```

### Comparing `smartmin-5.0.1/smartmin/backends.py` & `smartmin-5.0.2/smartmin/backends.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/csv_imports/migrations/0001_initial.py` & `smartmin-5.0.2/smartmin/csv_imports/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/csv_imports/migrations/0002_auto_20161118_1920.py` & `smartmin-5.0.2/smartmin/csv_imports/migrations/0002_auto_20161118_1920.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/csv_imports/migrations/0004_auto_20170223_0917.py` & `smartmin-5.0.2/smartmin/csv_imports/migrations/0004_auto_20170223_0917.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/csv_imports/migrations/0005_alter_importtask_created_by_and_more.py` & `smartmin-5.0.2/smartmin/csv_imports/migrations/0005_alter_importtask_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/csv_imports/models.py` & `smartmin-5.0.2/smartmin/csv_imports/models.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/csv_imports/tasks.py` & `smartmin-5.0.2/smartmin/csv_imports/tasks.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/csv_imports/tests.py` & `smartmin-5.0.2/smartmin/csv_imports/tests.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/csv_imports/views.py` & `smartmin-5.0.2/smartmin/csv_imports/views.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/email.py` & `smartmin-5.0.2/smartmin/email.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/management/__init__.py` & `smartmin-5.0.2/smartmin/management/__init__.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/management/commands/collect_sql.py` & `smartmin-5.0.2/smartmin/management/commands/collect_sql.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/management/commands/migrate_manual.py` & `smartmin-5.0.2/smartmin/management/commands/migrate_manual.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/management/tests.py` & `smartmin-5.0.2/smartmin/management/tests.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/mixins.py` & `smartmin-5.0.2/smartmin/mixins.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/models.py` & `smartmin-5.0.2/smartmin/models.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/pdf.py` & `smartmin-5.0.2/smartmin/pdf.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/perms.py` & `smartmin-5.0.2/smartmin/perms.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/css/bootstrap-datepicker3.css` & `smartmin-5.0.2/smartmin/static/css/bootstrap-datepicker3.css`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/css/bootstrap-theme.css` & `smartmin-5.0.2/smartmin/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/css/bootstrap.css` & `smartmin-5.0.2/smartmin/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/css/smartmin_styles.css` & `smartmin-5.0.2/smartmin/static/css/smartmin_styles.css`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.eot` & `smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.svg` & `smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.ttf` & `smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.woff` & `smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/fonts/glyphicons-halflings-regular.woff2` & `smartmin-5.0.2/smartmin/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/background.jpg` & `smartmin-5.0.2/smartmin/static/img/background.jpg`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/glyphicons-halflings-white.png` & `smartmin-5.0.2/smartmin/static/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/glyphicons-halflings.png` & `smartmin-5.0.2/smartmin/static/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/in.png` & `smartmin-5.0.2/smartmin/static/img/in.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/loc.png` & `smartmin-5.0.2/smartmin/static/img/loc.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/nyaruka.png` & `smartmin-5.0.2/smartmin/static/img/nyaruka.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/out.png` & `smartmin-5.0.2/smartmin/static/img/out.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/arrow-up.gif` & `smartmin-5.0.2/smartmin/static/img/smartmin/arrow-up.gif`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/default-bg-reverse.gif` & `smartmin-5.0.2/smartmin/static/img/smartmin/default-bg-reverse.gif`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/default-bg.gif` & `smartmin-5.0.2/smartmin/static/img/smartmin/default-bg.gif`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/icon_searchbox.png` & `smartmin-5.0.2/smartmin/static/img/smartmin/icon_searchbox.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/inline-delete.png` & `smartmin-5.0.2/smartmin/static/img/smartmin/inline-delete.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/inline-restore.png` & `smartmin-5.0.2/smartmin/static/img/smartmin/inline-restore.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/loading.gif` & `smartmin-5.0.2/smartmin/static/img/smartmin/loading.gif`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/selector-add.gif` & `smartmin-5.0.2/smartmin/static/img/smartmin/selector-add.gif`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/selector-search.gif` & `smartmin-5.0.2/smartmin/static/img/smartmin/selector-search.gif`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/selector_stacked-add.gif` & `smartmin-5.0.2/smartmin/static/img/smartmin/selector_stacked-add.gif`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin/tooltag-add.gif` & `smartmin-5.0.2/smartmin/static/img/smartmin/tooltag-add.gif`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/smartmin.png` & `smartmin-5.0.2/smartmin/static/img/smartmin.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/sort.gif` & `smartmin-5.0.2/smartmin/static/img/sort.gif`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/sort.png` & `smartmin-5.0.2/smartmin/static/img/sort.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/sort_asc.png` & `smartmin-5.0.2/smartmin/static/img/sort_asc.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/img/sort_dsc.png` & `smartmin-5.0.2/smartmin/static/img/sort_dsc.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/js/bootstrap-datepicker.js` & `smartmin-5.0.2/smartmin/static/js/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/js/bootstrap.min.js` & `smartmin-5.0.2/smartmin/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/js/jquery.pjax.js` & `smartmin-5.0.2/smartmin/static/js/jquery.pjax.js`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/js/libs/jquery-1.12.4.min.js` & `smartmin-5.0.2/smartmin/static/js/libs/jquery-1.12.4.min.js`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/js/libs/jquery.min.js` & `smartmin-5.0.2/smartmin/static/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/js/libs/jquery.url.js` & `smartmin-5.0.2/smartmin/static/js/libs/jquery.url.js`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/static/top.png` & `smartmin-5.0.2/smartmin/static/top.png`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/csv_imports/importtask_read.html` & `smartmin-5.0.2/smartmin/templates/csv_imports/importtask_read.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/frame.html` & `smartmin-5.0.2/smartmin/templates/frame.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/base.html` & `smartmin-5.0.2/smartmin/templates/smartmin/base.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/delete_confirm.html` & `smartmin-5.0.2/smartmin/templates/smartmin/delete_confirm.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/field.html` & `smartmin-5.0.2/smartmin/templates/smartmin/field.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/form.html` & `smartmin-5.0.2/smartmin/templates/smartmin/form.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/list.html` & `smartmin-5.0.2/smartmin/templates/smartmin/list.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/read.html` & `smartmin-5.0.2/smartmin/templates/smartmin/read.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/users/login.html` & `smartmin-5.0.2/smartmin/templates/smartmin/users/login.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/users/user_failed.html` & `smartmin-5.0.2/smartmin/templates/smartmin/users/user_failed.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/users/user_list.html` & `smartmin-5.0.2/smartmin/templates/smartmin/users/user_list.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templates/smartmin/users/user_update.html` & `smartmin-5.0.2/smartmin/templates/smartmin/users/user_update.html`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/templatetags/smartmin.py` & `smartmin-5.0.2/smartmin/templatetags/smartmin.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/tests.py` & `smartmin-5.0.2/smartmin/tests.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/users/middleware.py` & `smartmin-5.0.2/smartmin/users/middleware.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/users/migrations/0001_initial.py` & `smartmin-5.0.2/smartmin/users/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/users/migrations/0003_auto_20210219_1548.py` & `smartmin-5.0.2/smartmin/users/migrations/0003_auto_20210219_1548.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/users/models.py` & `smartmin-5.0.2/smartmin/users/models.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/users/urls.py` & `smartmin-5.0.2/smartmin/users/urls.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/users/views.py` & `smartmin-5.0.2/smartmin/users/views.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/smartmin/views.py` & `smartmin-5.0.2/smartmin/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1142,15 +1142,15 @@
 
     def get_queryset(self):
         self.queryset = self.derive_queryset()
         return self.queryset
 
     def derive_success_message(self):
         # First check whether a default message has been set
-        if self.success_message is None:
+        if self.success_message is None and getattr(settings, "SMARTMIN_DEFAULT_MESSAGES", True):
             return "Your %s has been updated." % self.model._meta.verbose_name
         else:
             return self.success_message
 
     def pre_save(self, obj):
         # auto populate modified_by if it is present
         if self.request.user.id and self.request.user.id > 0 and hasattr(obj, "modified_by_id"):
@@ -1269,15 +1269,15 @@
             if hasattr(obj, "modified_by_id"):
                 obj.modified_by = self.request.user
 
         return obj
 
     def derive_success_message(self):
         # First check whether a default message has been set
-        if self.success_message is None:
+        if self.success_message is None and getattr(settings, "SMARTMIN_DEFAULT_MESSAGES", True):
             return _("Your new %s has been created.") % self.model._meta.verbose_name
         else:
             return self.success_message
 
     def derive_title(self):
         """
         Derives our title from our object
```

### Comparing `smartmin-5.0.1/smartmin/widgets.py` & `smartmin-5.0.2/smartmin/widgets.py`

 * *Files identical despite different names*

### Comparing `smartmin-5.0.1/PKG-INFO` & `smartmin-5.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartmin
-Version: 5.0.1
+Version: 5.0.2
 Summary: Scaffolding system for Django object management.
 License: BSD
 Author: Nyaruka Ltd
 Author-email: code@nyaruka.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -43,19 +43,19 @@
 - CRUDL operations at the object level, that is, Create, Read, Update, Delete and List, permissions and views are based 
   around this
 - URL automapping via the the CRUDL objects, this should keep things very very DRY
 
 About Versions
 ==============
 
-Smartmin tries to stay in lock step with the latest Django versions. With each new Django LTS release we will release
+Smartmin tries to stay in lock step with the latest Django versions. With each new major Django release we will release
 a new Smartmin major version and we will reserve major changes (possibly breaking backwards compatibility) for such 
-releases. This includes updating to the latest version of Twitter Bootstrap.
+releases.
 
-The latest version is the 3.* series which supports the Django 3.2 LTS and 2.2 LTS.
+The latest version is the 5.* series which supports the Django 5.0 and 4.2.
 
 About
 =====
 
 The full documentation can be found at: http://readthedocs.org/docs/smartmin/en/latest/
 
 The official source code repository is: http://www.github.com/nyaruka/smartmin/
```

