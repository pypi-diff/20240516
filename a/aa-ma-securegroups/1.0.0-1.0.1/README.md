# Comparing `tmp/aa_ma_securegroups-1.0.0.tar.gz` & `tmp/aa_ma_securegroups-1.0.1.tar.gz`

## Comparing `aa_ma_securegroups-1.0.0.tar` & `aa_ma_securegroups-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,48 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/__init__.py
--rw-r--r--   0        0        0     7039 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/admin.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/apps.py
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/auth_hooks.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/memberaudit.py
--rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/models.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/django.pot
--rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4926 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6515 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4781 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8981 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5488 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/migrations/0001_initial.py
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/migrations/0002_alter_skillpointfilter_skill_point_threshold_and_more.py
--rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/migrations/0003_add_corporation_role_filter_and_more.py
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/migrations/0004_timeincorporationfilter_corporationtitlefilter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/tests/__init__.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/tests/factories.py
--rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/tests/test_admin.py
--rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/tests/test_integration.py
--rw-r--r--   0        0        0    37664 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/memberaudit_securegroups/tests/test_models.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/LICENSE
--rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/README.md
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    50568 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/__init__.py
+-rw-r--r--   0        0        0     7039 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/admin.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/apps.py
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/auth_hooks.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/memberaudit.py
+-rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/models.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/django.pot
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4622 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3354 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4831 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6590 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5054 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6044 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/migrations/0001_initial.py
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/migrations/0002_alter_skillpointfilter_skill_point_threshold_and_more.py
+-rw-r--r--   0        0        0     5699 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/migrations/0003_add_corporation_role_filter_and_more.py
+-rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/migrations/0004_timeincorporationfilter_corporationtitlefilter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/tests/__init__.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/tests/factories.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/tests/test_admin.py
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/tests/test_integration.py
+-rw-r--r--   0        0        0    37664 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/memberaudit_securegroups/tests/test_models.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/LICENSE
+-rw-r--r--   0        0        0     8141 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/README.md
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    50568 2020-02-02 00:00:00.000000 aa_ma_securegroups-1.0.1/PKG-INFO
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/admin.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/admin.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/auth_hooks.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/memberaudit.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/memberaudit.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/models.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/models.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/django.pot` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/django.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-16 13:00+0100\n"
+"POT-Creation-Date: 2024-03-20 17:15+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/de/LC_MESSAGES/django.mo` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/de/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-member-audit-secure-groups/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Active character: "
 msgid_plural "Active characters: "
 msgstr[0] "Aktiver Charakter: "
 msgstr[1] "Aktive Charaktere: "
 
 msgid "Activity [Last {inactivity_threshold}]"
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/de/LC_MESSAGES/django.po` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/de/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 13:00+0100\n"
-"PO-Revision-Date: 2024-03-16 12:02+0000\n"
+"PO-Revision-Date: 2024-05-10 14:08+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-member-audit-secure-groups/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.4.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: memberaudit_securegroups/admin.py:83
 #, python-brace-format
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] "{inactivity_threshold:d} Tag"
 msgstr[1] "{inactivity_threshold:d} Tage"
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/es/LC_MESSAGES/django.mo` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/es/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Spanish (Alliance Auth Apps)\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-member-audit-secure-groups-integration/es/>\n"
+"apps/aa-member-audit-secure-groups/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Activity [Last {inactivity_threshold}]"
 msgstr "Actividad [por última vez {inactivity_threshold}]"
 
 msgid "All characters have been added to {MEMBERAUDIT_APP_NAME}"
 msgstr "Todos los personajes están añadidos en {MEMBERAUDIT_APP_NAME}"
 
@@ -24,35 +24,28 @@
 
 msgid "Maximum allowable inactivity, in <strong>days</strong>."
 msgstr "Inactividad máxima permitida, en <strong> días </strong>."
 
 msgid "Member Audit Asset"
 msgstr "Auditoría de Bienes de los Miembros"
 
-msgid "Member Audit Secure Groups Integration v{__version__}"
-msgstr ""
-"Integración de la Auditoria de Miembros de los Grupos Seguros v{__version__}"
-
 msgid "Member Audit Skill Points [{skill_point_threshold}]"
 msgstr "Auditoría de Miembro Puntos de Habilidad [{skill_point_threshold}]"
 
 msgid "Member Audit Skill Set"
 msgstr "Auditoría de Miembro Conjunto de Habilidades"
 
 msgid "Minimum allowable age, in <strong>days</strong>."
 msgstr "Edad mínima permitida, en <strong>días</strong>."
 
 msgid "Missing character: "
 msgid_plural "Missing characters: "
 msgstr[0] "Personaje que falta: "
 msgstr[1] "Personajes que faltan: "
 
-msgid "Not all of your characters are added to {MEMBERAUDIT_APP_NAME}"
-msgstr "No todos tus personajes están añadidos en {MEMBERAUDIT_APP_NAME}"
-
 msgid "The filter description that is shown to end users."
 msgstr "La descripción del filtro que se muestra a los usuarios finales."
 
 msgid "User must possess <strong>one</strong> of the selected assets."
 msgstr ""
 "El usuario debe tener <strong>uno</strong> de los bienes seleccionados."
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/es/LC_MESSAGES/django.po` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PACKAGE package.
 # Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 13:00+0100\n"
-"PO-Revision-Date: 2023-09-24 13:14+0000\n"
+"PO-Revision-Date: 2024-05-10 14:08+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-member-audit-secure-groups-integration/es/>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-member-audit-secure-groups/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: memberaudit_securegroups/admin.py:83
 #, python-brace-format
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] "día {inactivity_threshold:d}"
 msgstr[1] "días {inactivity_threshold:d}"
@@ -92,16 +92,15 @@
 #, fuzzy, python-brace-format
 #| msgid "Character Age [{age_threshold}]"
 msgid "Character age [{age_threshold}]"
 msgstr "Edad del Personaje [{age_threshold}]"
 
 #: memberaudit_securegroups/models.py:316
 msgid "User must possess <strong>one</strong> of the selected assets."
-msgstr ""
-"El usuario debe tener <strong>uno</strong> de los bienes seleccionados."
+msgstr "El usuario debe tener <strong>uno</strong> de los bienes seleccionados."
 
 #: memberaudit_securegroups/models.py:326
 msgid "Member Audit Asset"
 msgstr "Auditoría de Bienes de los Miembros"
 
 #: memberaudit_securegroups/models.py:404
 msgid "Compliance"
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/fr_FR/LC_MESSAGES/django.po` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/nl/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-03-16 13:00+0100\n"
-"PO-Revision-Date: 2023-09-24 13:14+0000\n"
+"POT-Creation-Date: 2024-03-20 17:15+0100\n"
+"PO-Revision-Date: 2024-05-10 14:08+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-member-audit-secure-groups-integration/fr/>\n"
-"Language: fr_FR\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-member-audit-secure-groups/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: memberaudit_securegroups/admin.py:83
 #, python-brace-format
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] ""
 msgstr[1] ""
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/it_IT/LC_MESSAGES/django.po` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 13:00+0100\n"
-"PO-Revision-Date: 2023-09-24 13:14+0000\n"
+"PO-Revision-Date: 2024-05-10 14:08+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-member-audit-secure-groups-integration/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-member-audit-secure-groups/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: memberaudit_securegroups/admin.py:83
 #, python-brace-format
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] ""
 msgstr[1] ""
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ja/LC_MESSAGES/django.po` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ja/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 13:00+0100\n"
-"PO-Revision-Date: 2023-09-24 13:14+0000\n"
+"PO-Revision-Date: 2024-05-10 14:08+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-member-audit-secure-groups-integration/ja/>\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-member-audit-secure-groups/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: memberaudit_securegroups/admin.py:83
 #, python-brace-format
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] ""
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 26% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,22 +7,29 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-member-audit-secure-groups/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
+
+msgid "Active character: "
+msgid_plural "Active characters: "
+msgstr[0] "활동중인 캐릭터: "
 
 msgid "Activity [Last {inactivity_threshold}]"
 msgstr "활동 [최근 {inactivity_threshold}]"
 
 msgid "All characters have been added to {MEMBERAUDIT_APP_NAME}"
 msgstr "모든 캐릭터가 {MEMBERAUDIT_APP_NAME}에 등록되었습니다"
 
+msgid "Character age [{age_threshold}]"
+msgstr "캐릭터 나이 [{age_threshold}]"
+
 msgid "Compliance"
 msgstr "준수 사항"
 
 msgid "Maximum allowable inactivity, in <strong>days</strong>."
 msgstr "허용 최대 미접속 기간, <strong>일</strong> 단위."
 
 msgid "Member Audit Asset"
@@ -48,16 +55,22 @@
 msgstr "신청하는 사용자에게 보여지는 필터 설명."
 
 msgid "User must possess <strong>one</strong> of the selected assets."
 msgstr ""
 "사용자는 선택된 아이템 중 최소 <strong>한 개</strong> 이상의 아이템을 소유하"
 "고 있어야 합니다."
 
+msgid "When True, the filter will also include the users alt-characters."
+msgstr "활성화할 경우, 유저들의 알트 캐릭터를 포함하게 됩니다."
+
+msgid "When checked, the filter will also include the users alt-characters."
+msgstr "활성화할 경우, 유저들의 알트 캐릭터를 포함하게 됩니다."
+
 msgid "corporation role"
-msgstr "코퍼레이션 역할"
+msgstr "코퍼레이션 직책"
 
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] "{inactivity_threshold:d} 일"
 
 msgid "{self.age_threshold:d} day"
 msgid_plural "{self.age_threshold:d} days"
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/django.po` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Author50CO <tkddlschry@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Mind of the Raven <okanieva@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 13:00+0100\n"
-"PO-Revision-Date: 2023-12-29 10:04+0000\n"
+"PO-Revision-Date: 2024-05-10 14:08+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-member-audit-secure-groups/ko/>\n"
+"Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-member-audit-secure-groups/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: memberaudit_securegroups/admin.py:83
 #, python-brace-format
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] "{inactivity_threshold:d} 일"
 
 #: memberaudit_securegroups/admin.py:147
 msgid "corporation role"
-msgstr "코퍼레이션 역할"
+msgstr "코퍼레이션 직책"
 
 #: memberaudit_securegroups/apps.py:20
 #, python-brace-format
 msgid "Secure Groups (Member Audit Integration) v{__version__}"
 msgstr "멤버 관리 보안 그룹 인테그레이션 v{__version__}"
 
 #: memberaudit_securegroups/models.py:115
@@ -62,17 +63,14 @@
 
 #: memberaudit_securegroups/models.py:173
 #, python-brace-format
 msgid "Activity [Last {inactivity_threshold}]"
 msgstr "활동 [최근 {inactivity_threshold}]"
 
 #: memberaudit_securegroups/models.py:225
-#, fuzzy
-#| msgid "Active Character: "
-#| msgid_plural "Active Characters: "
 msgid "Active character: "
 msgid_plural "Active characters: "
 msgstr[0] "활동중인 캐릭터: "
 
 #: memberaudit_securegroups/models.py:242
 msgid "Minimum allowable age, in <strong>days</strong>."
 msgstr "허용 최소 캐릭터 나이, <strong>일</strong> 단위."
@@ -80,24 +78,22 @@
 #: memberaudit_securegroups/models.py:253
 #, python-brace-format
 msgid "{self.age_threshold:d} day"
 msgid_plural "{self.age_threshold:d} days"
 msgstr[0] "{self.age_threshold:d} 일"
 
 #: memberaudit_securegroups/models.py:258
-#, fuzzy, python-brace-format
-#| msgid "Character Age [{age_threshold}]"
+#, python-brace-format
 msgid "Character age [{age_threshold}]"
 msgstr "캐릭터 나이 [{age_threshold}]"
 
 #: memberaudit_securegroups/models.py:316
 msgid "User must possess <strong>one</strong> of the selected assets."
-msgstr ""
-"사용자는 선택된 아이템 중 최소 <strong>한 개</strong> 이상의 아이템을 소유하"
-"고 있어야 합니다."
+msgstr "사용자는 선택된 아이템 중 최소 <strong>한 개</strong> 이상의 아이템을 "
+"소유하고 있어야 합니다."
 
 #: memberaudit_securegroups/models.py:326
 msgid "Member Audit Asset"
 msgstr "아이템별 멤버 관리"
 
 #: memberaudit_securegroups/models.py:404
 msgid "Compliance"
@@ -119,15 +115,15 @@
 
 #: memberaudit_securegroups/models.py:490
 msgid "User must have a character with this role."
 msgstr ""
 
 #: memberaudit_securegroups/models.py:495
 msgid "When checked, the filter will also include the users alt-characters."
-msgstr ""
+msgstr "활성화할 경우, 유저들의 알트 캐릭터를 포함하게 됩니다."
 
 #: memberaudit_securegroups/models.py:505
 #, fuzzy
 #| msgid "Member Audit Skill Set"
 msgid "Member Audit Corporation Role"
 msgstr "스킬 셋 별 멤버 관리"
 
@@ -137,15 +133,15 @@
 
 #: memberaudit_securegroups/models.py:581
 msgid "User must have a character with this title."
 msgstr ""
 
 #: memberaudit_securegroups/models.py:586
 msgid "When True, the filter will also include the users alt-characters."
-msgstr ""
+msgstr "활성화할 경우, 유저들의 알트 캐릭터를 포함하게 됩니다."
 
 #: memberaudit_securegroups/models.py:596
 #, fuzzy
 #| msgid "Member Audit Skill Set"
 msgid "Member Audit Corporation Title"
 msgstr "스킬 셋 별 멤버 관리"
 
@@ -182,16 +178,15 @@
 #, fuzzy
 #| msgid ""
 #| "Users must possess all of the skills in <strong>one</strong> of the "
 #| "selected skillsets."
 msgid ""
 "Users must have a character who possess all of the skills in <strong>one</"
 "strong> of the selected skill sets."
-msgstr ""
-"사용자는 선택된 스킬 셋 중 <strong>한 개</strong> 이상의 스킬 셋을 완료해야 "
+msgstr "사용자는 선택된 스킬 셋 중 <strong>한 개</strong> 이상의 스킬 셋을 완료해야 "
 "합니다."
 
 #: memberaudit_securegroups/models.py:752
 msgid "Specify the type of character that needs to have the skill set."
 msgstr ""
 
 #: memberaudit_securegroups/models.py:790
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.mo` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.mo`

 * *Files 6% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-member-audit-secure-groups/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Active character: "
 msgid_plural "Active characters: "
 msgstr[0] "Активный персонаж: "
 msgstr[1] "Активные персонажи: "
 msgstr[2] "Активные персонажи: "
 msgstr[3] "Активные персонажи: "
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.po` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Nikolay <nick.postnikov@gmail.com>, 2023.
 # Max <mark25@inbox.ru>, 2023.
-# Ruslan Virchich <ruslan.virchich@gmail.com>, 2023.
+# Ruslan Virchich <ruslan.virchich@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 13:00+0100\n"
-"PO-Revision-Date: 2023-11-17 18:04+0000\n"
+"PO-Revision-Date: 2024-05-10 14:08+0000\n"
 "Last-Translator: Ruslan Virchich <ruslan.virchich@gmail.com>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-member-audit-secure-groups/ru/>\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-member-audit-secure-groups/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: memberaudit_securegroups/admin.py:83
 #, python-brace-format
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] "{inactivity_threshold:d} день"
 msgstr[1] "{inactivity_threshold:d} дня"
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/uk/LC_MESSAGES/django.po` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/uk/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # "Andrii M." <elfleg0las88@gmail.com>, 2023.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 13:00+0100\n"
-"PO-Revision-Date: 2023-09-24 13:14+0000\n"
-"Last-Translator: \"Andrii M.\" <elfleg0las88@gmail.com>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-member-audit-secure-groups-integration/uk/>\n"
+"PO-Revision-Date: 2024-05-10 14:08+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-member-audit-secure-groups/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: memberaudit_securegroups/admin.py:83
 #, python-brace-format
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] ""
 msgstr[1] ""
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: Chinese (Simplified) (Alliance Auth Apps)*

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 00000000: de12 0495 0000 0000 0100 0000 1c00 0000  ................
 00000010: 2400 0000 0300 0000 2c00 0000 0000 0000  $.......,.......
-00000020: 3800 0000 e401 0000 3900 0000 0100 0000  8.......9.......
+00000020: 3800 0000 f101 0000 3900 0000 0100 0000  8.......9.......
 00000030: 0000 0000 0000 0000 0050 726f 6a65 6374  .........Project
-00000040: 2d49 642d 5665 7273 696f 6e3a 2043 6869  -Id-Version: Chi
-00000050: 6e65 7365 2028 5369 6d70 6c69 6669 6564  nese (Simplified
-00000060: 2920 2841 6c6c 6961 6e63 6520 4175 7468  ) (Alliance Auth
-00000070: 2041 7070 7329 0a52 6570 6f72 742d 4d73   Apps).Report-Ms
-00000080: 6769 642d 4275 6773 2d54 6f3a 200a 504f  gid-Bugs-To: .PO
-00000090: 2d52 6576 6973 696f 6e2d 4461 7465 3a20  -Revision-Date: 
-000000a0: 5945 4152 2d4d 4f2d 4441 2048 4f3a 4d49  YEAR-MO-DA HO:MI
-000000b0: 2b5a 4f4e 450a 4c61 7374 2d54 7261 6e73  +ZONE.Last-Trans
-000000c0: 6c61 746f 723a 2046 554c 4c20 4e41 4d45  lator: FULL NAME
-000000d0: 203c 454d 4149 4c40 4144 4452 4553 533e   <EMAIL@ADDRESS>
-000000e0: 0a4c 616e 6775 6167 652d 5465 616d 3a20  .Language-Team: 
-000000f0: 4368 696e 6573 6520 2853 696d 706c 6966  Chinese (Simplif
-00000100: 6965 6429 203c 6874 7470 733a 2f2f 7765  ied) <https://we
-00000110: 626c 6174 652e 7070 6665 7566 6572 2e64  blate.ppfeufer.d
-00000120: 652f 7072 6f6a 6563 7473 2f61 6c6c 6961  e/projects/allia
-00000130: 6e63 652d 6175 7468 2d61 7070 732f 6161  nce-auth-apps/aa
-00000140: 2d6d 656d 6265 722d 6175 6469 742d 7365  -member-audit-se
-00000150: 6375 7265 2d67 726f 7570 732d 696e 7465  cure-groups-inte
-00000160: 6772 6174 696f 6e2f 7a68 5f48 616e 732f  gration/zh_Hans/
-00000170: 3e0a 4c61 6e67 7561 6765 3a20 7a68 5f48  >.Language: zh_H
-00000180: 616e 730a 4d49 4d45 2d56 6572 7369 6f6e  ans.MIME-Version
-00000190: 3a20 312e 300a 436f 6e74 656e 742d 5479  : 1.0.Content-Ty
-000001a0: 7065 3a20 7465 7874 2f70 6c61 696e 3b20  pe: text/plain; 
-000001b0: 6368 6172 7365 743d 5554 462d 380a 436f  charset=UTF-8.Co
-000001c0: 6e74 656e 742d 5472 616e 7366 6572 2d45  ntent-Transfer-E
-000001d0: 6e63 6f64 696e 673a 2038 6269 740a 506c  ncoding: 8bit.Pl
-000001e0: 7572 616c 2d46 6f72 6d73 3a20 6e70 6c75  ural-Forms: nplu
-000001f0: 7261 6c73 3d31 3b20 706c 7572 616c 3d30  rals=1; plural=0
-00000200: 3b0a 582d 4765 6e65 7261 746f 723a 2057  ;.X-Generator: W
-00000210: 6562 6c61 7465 2035 2e30 2e32 0a00       eblate 5.0.2..
+00000040: 2d49 642d 5665 7273 696f 6e3a 2050 6f6c  -Id-Version: Pol
+00000050: 6973 6820 2841 6c6c 6961 6e63 6520 4175  ish (Alliance Au
+00000060: 7468 2041 7070 7329 0a52 6570 6f72 742d  th Apps).Report-
+00000070: 4d73 6769 642d 4275 6773 2d54 6f3a 200a  Msgid-Bugs-To: .
+00000080: 504f 2d52 6576 6973 696f 6e2d 4461 7465  PO-Revision-Date
+00000090: 3a20 5945 4152 2d4d 4f2d 4441 2048 4f3a  : YEAR-MO-DA HO:
+000000a0: 4d49 2b5a 4f4e 450a 4c61 7374 2d54 7261  MI+ZONE.Last-Tra
+000000b0: 6e73 6c61 746f 723a 2046 554c 4c20 4e41  nslator: FULL NA
+000000c0: 4d45 203c 454d 4149 4c40 4144 4452 4553  ME <EMAIL@ADDRES
+000000d0: 533e 0a4c 616e 6775 6167 652d 5465 616d  S>.Language-Team
+000000e0: 3a20 506f 6c69 7368 203c 6874 7470 733a  : Polish <https:
+000000f0: 2f2f 7765 626c 6174 652e 7070 6665 7566  //weblate.ppfeuf
+00000100: 6572 2e64 652f 7072 6f6a 6563 7473 2f61  er.de/projects/a
+00000110: 6c6c 6961 6e63 652d 6175 7468 2d61 7070  lliance-auth-app
+00000120: 732f 6161 2d6d 656d 6265 722d 6175 6469  s/aa-member-audi
+00000130: 742d 7365 6375 7265 2d67 726f 7570 732f  t-secure-groups/
+00000140: 706c 2f3e 0a4c 616e 6775 6167 653a 2070  pl/>.Language: p
+00000150: 6c0a 4d49 4d45 2d56 6572 7369 6f6e 3a20  l.MIME-Version: 
+00000160: 312e 300a 436f 6e74 656e 742d 5479 7065  1.0.Content-Type
+00000170: 3a20 7465 7874 2f70 6c61 696e 3b20 6368  : text/plain; ch
+00000180: 6172 7365 743d 5554 462d 380a 436f 6e74  arset=UTF-8.Cont
+00000190: 656e 742d 5472 616e 7366 6572 2d45 6e63  ent-Transfer-Enc
+000001a0: 6f64 696e 673a 2038 6269 740a 506c 7572  oding: 8bit.Plur
+000001b0: 616c 2d46 6f72 6d73 3a20 6e70 6c75 7261  al-Forms: nplura
+000001c0: 6c73 3d33 3b20 706c 7572 616c 3d6e 3d3d  ls=3; plural=n==
+000001d0: 3120 3f20 3020 3a20 6e25 3130 3e3d 3220  1 ? 0 : n%10>=2 
+000001e0: 2626 206e 2531 303c 3d34 2026 2620 286e  && n%10<=4 && (n
+000001f0: 2531 3030 3c31 3020 7c7c 206e 2531 3030  %100<10 || n%100
+00000200: 3e3d 3230 2920 3f20 3120 3a20 323b 0a58  >=20) ? 1 : 2;.X
+00000210: 2d47 656e 6572 6174 6f72 3a20 5765 626c  -Generator: Webl
+00000220: 6174 6520 352e 352e 330a 00              ate 5.5.3..
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2024-03-16 13:00+0100\n"
-"PO-Revision-Date: 2023-09-24 13:14+0000\n"
+"PO-Revision-Date: 2024-05-10 14:08+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-member-audit-secure-groups-integration/zh_Hans/>\n"
+"alliance-auth-apps/aa-member-audit-secure-groups/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: memberaudit_securegroups/admin.py:83
 #, python-brace-format
 msgid "{inactivity_threshold:d} day"
 msgid_plural "{inactivity_threshold:d} days"
 msgstr[0] ""
```

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/migrations/0001_initial.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/migrations/0002_alter_skillpointfilter_skill_point_threshold_and_more.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/migrations/0002_alter_skillpointfilter_skill_point_threshold_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/migrations/0003_add_corporation_role_filter_and_more.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/migrations/0003_add_corporation_role_filter_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/migrations/0004_timeincorporationfilter_corporationtitlefilter.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/migrations/0004_timeincorporationfilter_corporationtitlefilter.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/tests/factories.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/tests/test_admin.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/tests/test_integration.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/memberaudit_securegroups/tests/test_models.py` & `aa_ma_securegroups-1.0.1/memberaudit_securegroups/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/LICENSE` & `aa_ma_securegroups-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/README.md` & `aa_ma_securegroups-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/pyproject.toml` & `aa_ma_securegroups-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_ma_securegroups-1.0.0/PKG-INFO` & `aa_ma_securegroups-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aa-ma-securegroups
-Version: 1.0.0
+Version: 1.0.1
 Summary: Member Audit Secure Groups integration for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-ma-securegroups/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-ma-securegroups/blob/master/README.md
 Project-URL: Homepage, https://github.com/ppfeufer/aa-ma-securegroups
 Project-URL: Source, https://github.com/ppfeufer/aa-ma-securegroups.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-ma-securegroups/issues
 Author-email: Peter Pfeufer <develop@ppfeufer.de>, Erik Kalkoken <kalkoken87@gmail.com>, Rebecca Murphy <rebecca@rcmurphy.me>
```

