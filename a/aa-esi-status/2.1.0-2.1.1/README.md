# Comparing `tmp/aa_esi_status-2.1.0.tar.gz` & `tmp/aa_esi_status-2.1.1.tar.gz`

## Comparing `aa_esi_status-2.1.0.tar` & `aa_esi_status-2.1.1.tar`

### file list

```diff
@@ -1,56 +1,64 @@
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/apps.py
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/auth_hooks.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/constants.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/models.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/urls.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/.gitkeep
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/django.pot
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     3284 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/migrations/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/static/esistatus/css/esistatus.css
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/static/esistatus/css/esistatus.min.css
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/static/esistatus/css/esistatus.min.css.map
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.js
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js.map
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templates/esistatus/base.html
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templates/esistatus/dashboard-widget.html
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templates/esistatus/index.html
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templates/esistatus/bundles/esistatus-dashboard-widget-js.html
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templates/esistatus/partials/endpoints.html
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templates/esistatus/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templates/esistatus/partials/header/page-header.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templatetags/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/templatetags/esistatus.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/tests/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/tests/test_access.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/tests/test_auth_hooks.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/tests/test_templatetags.py
--rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/tests/test_views.py
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/esistatus/tests/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/LICENSE
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/pyproject.toml
--rw-r--r--   0        0        0    49019 2020-02-02 00:00:00.000000 aa_esi_status-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/apps.py
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/auth_hooks.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/constants.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/models.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/urls.py
+-rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/.gitkeep
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/django.pot
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2950 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     3296 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/migrations/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/css/esistatus.css
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/css/esistatus.min.css
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/css/esistatus.min.css.map
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.js
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js.map
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/base.html
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/dashboard-widget.html
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/index.html
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/bundles/esistatus-dashboard-widget-js.html
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/endpoints.html
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/header/page-header.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templatetags/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/templatetags/esistatus.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/test_access.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/test_templatetags.py
+-rw-r--r--   0        0        0     6548 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/test_views.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/esistatus/tests/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/LICENSE
+-rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0    49019 2020-02-02 00:00:00.000000 aa_esi_status-2.1.1/PKG-INFO
```

### Comparing `aa_esi_status-2.1.0/esistatus/auth_hooks.py` & `aa_esi_status-2.1.1/esistatus/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/views.py` & `aa_esi_status-2.1.1/esistatus/views.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/locale/django.pot` & `aa_esi_status-2.1.1/esistatus/locale/cs/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
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
-"POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
-"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: LANGUAGE <LL@li.org>\n"
-"Language: \n"
+"POT-Creation-Date: 2024-03-20 17:26+0100\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Czech <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-esi-status/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr ""
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/de/LC_MESSAGES/django.mo` & `aa_esi_status-2.1.1/esistatus/locale/de/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-esi-status/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Can access this app"
 msgstr "Kann auf diese App zugreifen"
 
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/de/LC_MESSAGES/django.po` & `aa_esi_status-2.1.1/esistatus/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2024-03-16 08:53+0000\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-esi-status/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr "ESI Status"
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/es/LC_MESSAGES/django.mo` & `aa_esi_status-2.1.1/esistatus/locale/es/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-esi-status/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Can access this app"
 msgstr "Puede acceder esta aplicacion"
 
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/es/LC_MESSAGES/django.po` & `aa_esi_status-2.1.1/esistatus/locale/es/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
-# Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023.
+# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
+# Geovanny David Morales De la cruz <moralesgeovanny1996@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2023-10-25 07:04+0000\n"
-"Last-Translator: Geovanny David Morales De la cruz "
-"<moralesgeovanny1996@gmail.com>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-esi-status/es/>\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
+"Last-Translator: Geovanny David Morales De la cruz <moralesgeovanny1996@gmail"
+".com>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-esi-status/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr "Estado del ESI"
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/fr_FR/LC_MESSAGES/django.mo` & `aa_esi_status-2.1.1/esistatus/locale/fr_FR/LC_MESSAGES/django.mo`

 * *Files 18% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,40 +7,46 @@
 "Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-esi-status/fr/>\n"
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
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 "Impossible de lire le statut ESI. Veuillez essayer de recharger la page. Si "
 "cela ne résout pas le problème, il est possible que le statut ESI soit "
 "complètement en panne."
 
+msgid "Detailed ESI status"
+msgstr "Statut ESI détaillé"
+
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 "Voulez-vous aider à traduire cette application dans votre langue ou "
 "améliorer la traduction existante ?"
 
 msgid "ESI Status"
 msgstr "Statut ESI"
 
 msgid "ESI Status v{__version__}"
 msgstr "Statut ESI v{__version__}"
 
+msgid "EVE Online status"
+msgstr "Status EVE Online"
+
 msgid "Green Endpoints"
 msgstr "Points de terminaison verts"
 
 msgid "Join our team of translators!"
 msgstr "Rejoignez notre équipe de traducteurs !"
 
 msgid "Red Endpoints"
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/fr_FR/LC_MESSAGES/django.po` & `aa_esi_status-2.1.1/esistatus/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # erka Ekanon <M6musicT@hotmail.fr>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2024-01-12 19:05+0000\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-esi-status/fr/>\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-esi-status/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr "Statut ESI"
@@ -56,22 +56,20 @@
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 "Impossible de lire le statut ESI. Veuillez essayer de recharger la page. Si "
 "cela ne résout pas le problème, il est possible que le statut ESI soit "
 "complètement en panne."
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
-#, fuzzy
-#| msgid "ESI Status"
 msgid "Detailed ESI status"
-msgstr "Statut ESI"
+msgstr "Statut ESI détaillé"
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:26
 msgid "EVE Online status"
-msgstr ""
+msgstr "Status EVE Online"
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 "Voulez-vous aider à traduire cette application dans votre langue ou "
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/it_IT/LC_MESSAGES/django.po` & `aa_esi_status-2.1.1/esistatus/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-esi-status/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-esi-status/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr ""
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/ja/LC_MESSAGES/django.po` & `aa_esi_status-2.1.1/esistatus/locale/ja/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-esi-status/ja/>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-esi-status/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr ""
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_esi_status-2.1.1/esistatus/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 13% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,41 +7,47 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-esi-status/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Can access this app"
 msgstr "서비스에 접근할 수 있습니다"
 
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 "ESI 상태를 읽을 수 없습니다. 페이지를 새로고침 해 보세요. 그래도 읽어올 수 없"
 "는 경우, ESI가 완전히 다운됐을 수도 있습니다."
 
+msgid "Detailed ESI status"
+msgstr "ESI 상태"
+
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 msgid "ESI Status"
 msgstr "ESI 상태"
 
 msgid "ESI Status v{__version__}"
 msgstr "ESI 상태 v{__version__}"
 
+msgid "EVE Online status"
+msgstr "EVE Online 상태"
+
 msgid "Green Endpoints"
 msgstr "청색 엔드포인트"
 
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
 
 msgid "Red Endpoints"
 msgstr "적색 엔드포인트"
 
 msgid "Yellow Endpoints"
 msgstr "황색 엔드포인트"
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/ko_KR/LC_MESSAGES/django.po` & `aa_esi_status-2.1.1/esistatus/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
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
 "POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2023-12-29 10:04+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-esi-status/ko/>\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
+"Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-esi-status/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr "ESI 상태"
@@ -51,29 +52,27 @@
 msgstr "청색 엔드포인트"
 
 #: esistatus/templates/esistatus/index.html:25
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
-"ESI 상태를 읽을 수 없습니다. 페이지를 새로고침 해 보세요. 그래도 읽어올 수 없"
-"는 경우, ESI가 완전히 다운됐을 수도 있습니다."
+"ESI 상태를 읽을 수 없습니다. 페이지를 새로고침 해 보세요. 그래도 읽어올 수 "
+"없는 경우, ESI가 완전히 다운됐을 수도 있습니다."
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
-#, fuzzy
-#| msgid "ESI Status"
 msgid "Detailed ESI status"
 msgstr "ESI 상태"
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:26
 msgid "EVE Online status"
-msgstr ""
+msgstr "EVE Online 상태"
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr "번역가 팀에 참여하세요!"
+msgstr "번역팀에 참여하세요!"
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/ru/LC_MESSAGES/django.mo` & `aa_esi_status-2.1.1/esistatus/locale/ru/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-esi-status/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Can access this app"
 msgstr "Имеет доступ к приложению"
 
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/ru/LC_MESSAGES/django.po` & `aa_esi_status-2.1.1/esistatus/locale/ru/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Nikolay <nick.postnikov@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Nikolay <nick.postnikov@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-esi-status/ru/>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-esi-status/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr "Статус ESI"
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/uk/LC_MESSAGES/django.mo` & `aa_esi_status-2.1.1/esistatus/locale/uk/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-esi-status/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 "Не вдалося прочитати статус ESI. Будь ласка, спробуйте перезавантажити "
 "сторінку. Якщо це не допомогло, цілком можливо, що ESI може повністю вийти з "
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/uk/LC_MESSAGES/django.po` & `aa_esi_status-2.1.1/esistatus/locale/uk/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

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
 "POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2023-09-24 13:12+0000\n"
+"PO-Revision-Date: 2024-05-10 14:01+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-esi-status/uk/>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-esi-status/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr "Статус ESI"
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_esi_status-2.1.1/esistatus/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,31 +7,46 @@
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-esi-status/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Can access this app"
-msgstr "允许访问此软件"
+msgstr "能够访问此应用程序"
 
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
 msgstr ""
 "无法读取 ESI 状态。 请尝试重新加载页面。 如果这没有解决，ESI 可能完全失效了。"
 
+msgid "Detailed ESI status"
+msgstr "ESI详细状态"
+
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
 msgid "ESI Status"
 msgstr "esi状态"
 
 msgid "ESI Status v{__version__}"
 msgstr "esi 状态 {__version__}"
 
+msgid "EVE Online status"
+msgstr "EVE Online状态"
+
+msgid "Green Endpoints"
+msgstr "绿色终端"
+
 msgid "Join our team of translators!"
 msgstr "加入我们的翻译团队吧！"
+
+msgid "Red Endpoints"
+msgstr "红色终端"
+
+msgid "Yellow Endpoints"
+msgstr "黄色终端"
```

### Comparing `aa_esi_status-2.1.0/esistatus/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_esi_status-2.1.1/esistatus/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Faer Yili <yilifaer@gmail.com>, 2024.
 # Peter Pfeufer <info@ppfeufer.de>, 2024.
 # Dehao Wu <wudehao2000@163.com>, 2024.
+# SAM_FPS <sam_fps@163.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-15 19:54+0100\n"
-"PO-Revision-Date: 2024-01-11 21:04+0000\n"
-"Last-Translator: Dehao Wu <wudehao2000@163.com>\n"
+"PO-Revision-Date: 2024-05-15 09:21+0000\n"
+"Last-Translator: SAM_FPS <sam_fps@163.com>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-esi-status/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: esistatus/__init__.py:9 esistatus/templates/esistatus/base.html:6
 #: esistatus/templates/esistatus/base.html:10
 #: esistatus/templates/esistatus/index.html:7
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:6
 msgid "ESI Status"
 msgstr "esi状态"
@@ -30,47 +31,44 @@
 #: esistatus/apps.py:20
 #, python-brace-format
 msgid "ESI Status v{__version__}"
 msgstr "esi 状态 {__version__}"
 
 #: esistatus/models.py:22
 msgid "Can access this app"
-msgstr "允许访问此软件"
+msgstr "能够访问此应用程序"
 
 #: esistatus/templates/esistatus/index.html:14
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:12
 msgid "Red Endpoints"
-msgstr ""
+msgstr "红色终端"
 
 #: esistatus/templates/esistatus/index.html:17
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:15
 msgid "Yellow Endpoints"
-msgstr ""
+msgstr "黄色终端"
 
 #: esistatus/templates/esistatus/index.html:20
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:18
 msgid "Green Endpoints"
-msgstr ""
+msgstr "绿色终端"
 
 #: esistatus/templates/esistatus/index.html:25
 msgid ""
 "Couldn't read the ESI status. Please try and reload the page. If that "
 "doesn't help, it is possible that ESI might be down entirely."
-msgstr ""
-"无法读取 ESI 状态。 请尝试重新加载页面。 如果这没有解决，ESI 可能完全失效了。"
+msgstr "无法读取 ESI 状态。 请尝试重新加载页面。 如果这没有解决，ESI 可能完全失效了。"
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:24
-#, fuzzy
-#| msgid "ESI Status"
 msgid "Detailed ESI status"
-msgstr "esi状态"
+msgstr "ESI详细状态"
 
 #: esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html:26
 msgid "EVE Online status"
-msgstr ""
+msgstr "EVE Online状态"
 
 #: esistatus/templates/esistatus/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
```

### Comparing `aa_esi_status-2.1.0/esistatus/migrations/0001_initial.py` & `aa_esi_status-2.1.1/esistatus/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.js` & `aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.js`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js` & `aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js.map` & `aa_esi_status-2.1.1/esistatus/static/esistatus/javascript/esistatus-dashboard-widget.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/templates/esistatus/base.html` & `aa_esi_status-2.1.1/esistatus/templates/esistatus/base.html`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/templates/esistatus/index.html` & `aa_esi_status-2.1.1/esistatus/templates/esistatus/index.html`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/templates/esistatus/partials/endpoints.html` & `aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/endpoints.html`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html` & `aa_esi_status-2.1.1/esistatus/templates/esistatus/partials/dashboard-widget/esi-status.html`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/templatetags/esistatus.py` & `aa_esi_status-2.1.1/esistatus/templatetags/esistatus.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/tests/test_access.py` & `aa_esi_status-2.1.1/esistatus/tests/test_access.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/tests/test_auth_hooks.py` & `aa_esi_status-2.1.1/esistatus/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/tests/test_templatetags.py` & `aa_esi_status-2.1.1/esistatus/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/tests/test_views.py` & `aa_esi_status-2.1.1/esistatus/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/esistatus/tests/utils.py` & `aa_esi_status-2.1.1/esistatus/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/LICENSE` & `aa_esi_status-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/README.md` & `aa_esi_status-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/pyproject.toml` & `aa_esi_status-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_esi_status-2.1.0/PKG-INFO` & `aa_esi_status-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-esi-status
-Version: 2.1.0
+Version: 2.1.1
 Summary: A simple status monitor for ESI
 Project-URL: Changelog, https://github.com/ppfeufer/aa-esi-status/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-esi-status/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-esi-status
 Project-URL: Source, https://github.com/ppfeufer/aa-esi-status.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-esi-status/issues
```

