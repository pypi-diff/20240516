# Comparing `tmp/aa_rss_to_discord-2.0.0b2.tar.gz` & `tmp/aa_rss_to_discord-2.0.1.tar.gz`

## Comparing `aa_rss_to_discord-2.0.0b2.tar` & `aa_rss_to_discord-2.0.1.tar`

### file list

```diff
@@ -1,37 +1,45 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/admin.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/apps.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/auth_hooks.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/constants.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/managers.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/models.py
--rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/tasks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/discordbot/cogs/__init__.py
--rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/discordbot/cogs/rss.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/django.pot
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/migrations/0001_initial.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/migrations/0002_enable_disable_rss_feeds.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/migrations/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/LICENSE
--rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/README.md
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/pyproject.toml
--rw-r--r--   0        0        0    50397 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/admin.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/apps.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/auth_hooks.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/constants.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/managers.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/models.py
+-rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/tasks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/discordbot/cogs/__init__.py
+-rw-r--r--   0        0        0     8461 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/discordbot/cogs/rss.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/django.pot
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/migrations/0001_initial.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/migrations/0002_enable_disable_rss_feeds.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/aa_rss_to_discord/migrations/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/LICENSE
+-rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/README.md
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    50396 2020-02-02 00:00:00.000000 aa_rss_to_discord-2.0.1/PKG-INFO
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/models.py` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/models.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/tasks.py` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/discordbot/cogs/rss.py` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/discordbot/cogs/rss.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/django.pot` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/django.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-15 18:12+0100\n"
+"POT-Creation-Date: 2024-03-20 17:13+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.mo` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo`

 * *Files 23% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,29 +1,30 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: German (Alliance Auth Apps)\n"
+"Project-Id-Version: Russian (Alliance Auth Apps)\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-rss-to-discord/de/>\n"
-"Language: de\n"
+"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-rss-to-discord/ru/>\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
+"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Last Item"
-msgstr "Letztes Element"
+msgstr "Последний элемент"
 
 msgid "Last Items"
-msgstr "Letzte Elemente"
+msgstr "Последние элементы"
 
 msgid "RSS Feed"
-msgstr "RSS Feed"
+msgstr "RSS лента"
 
 msgid "RSS Feeds"
-msgstr "RSS Feeds"
+msgstr "RSS ленты"
 
 msgid "RSS to Discord"
-msgstr "RSS zu Discord"
+msgstr "RSS к Дискорду"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/de/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

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
 "POT-Creation-Date: 2023-11-15 18:12+0100\n"
-"PO-Revision-Date: 2023-11-16 18:04+0000\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: German <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-rss-to-discord/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_rss_to_discord/__init__.py:9
 msgid "RSS to Discord"
 msgstr "RSS zu Discord"
 
 #: aa_rss_to_discord/models.py:41
 msgid "RSS Feed"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/es/LC_MESSAGES/django.mo` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/es/LC_MESSAGES/django.mo`

 * *Files 22% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-rss-to-discord/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Last Item"
 msgstr "Último artículo"
 
 msgid "Last Items"
 msgstr "Últimos artículos"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/es/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
+# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-11-15 18:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
 "Last-Translator: Zigor Fernandez Moreno <sietehierros@gmail.com>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-rss-to-discord/es/>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-rss-to-discord/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_rss_to_discord/__init__.py:9
 msgid "RSS to Discord"
 msgstr ""
 
 #: aa_rss_to_discord/models.py:41
 msgid "RSS Feed"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-11-15 18:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: French <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-rss-to-discord/fr/>\n"
+"Language-Team: French <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-rss-to-discord/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_rss_to_discord/__init__.py:9
 msgid "RSS to Discord"
 msgstr ""
 
 #: aa_rss_to_discord/models.py:41
 msgid "RSS Feed"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/it_IT/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-11-15 18:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-rss-to-discord/it/>\n"
+"Language-Team: Italian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-rss-to-discord/it/>\n"
 "Language: it_IT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_rss_to_discord/__init__.py:9
 msgid "RSS to Discord"
 msgstr ""
 
 #: aa_rss_to_discord/models.py:41
 msgid "RSS Feed"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/nl/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-15 18:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"POT-Creation-Date: 2024-03-20 17:13+0100\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-rss-to-discord/ja/>\n"
-"Language: ja\n"
+"Language-Team: Dutch <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-rss-to-discord/nl/>\n"
+"Language: nl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=2; plural=n != 1;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_rss_to_discord/__init__.py:9
 msgid "RSS to Discord"
 msgstr ""
 
 #: aa_rss_to_discord/models.py:41
 msgid "RSS Feed"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ko_KR/LC_MESSAGES/django.po` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Author50CO <tkddlschry@gmail.com>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-15 18:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
-"Last-Translator: Author50CO <tkddlschry@gmail.com>\n"
-"Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-rss-to-discord/ko/>\n"
-"Language: ko_KR\n"
+"POT-Creation-Date: 2024-03-20 17:13+0100\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-rss-to-discord/pl/>\n"
+"Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_rss_to_discord/__init__.py:9
 msgid "RSS to Discord"
 msgstr ""
 
 #: aa_rss_to_discord/models.py:41
 msgid "RSS Feed"
-msgstr "RSS 피드"
+msgstr ""
 
 #: aa_rss_to_discord/models.py:42
 msgid "RSS Feeds"
-msgstr "RSS 피드"
+msgstr ""
 
 #: aa_rss_to_discord/models.py:69
 msgid "Last Item"
-msgstr "마지막 항목"
+msgstr ""
 
 #: aa_rss_to_discord/models.py:70
 msgid "Last Items"
-msgstr "마지막 항목"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.mo` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/uk/LC_MESSAGES/django.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,30 +1,27 @@
 msgid ""
 msgstr ""
-"Project-Id-Version: Russian (Alliance Auth Apps)\n"
+"Project-Id-Version: Ukrainian (Alliance Auth Apps)\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-rss-to-discord/ru/>\n"
-"Language: ru\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
+"apps/aa-rss-to-discord/uk/>\n"
+"Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Last Item"
-msgstr "Последний элемент"
+msgstr "Останній елемент"
 
 msgid "Last Items"
-msgstr "Последние элементы"
+msgstr "Останні Елемети"
 
 msgid "RSS Feed"
-msgstr "RSS лента"
+msgstr "RSS-канал"
 
 msgid "RSS Feeds"
-msgstr "RSS ленты"
-
-msgid "RSS to Discord"
-msgstr "RSS к Дискорду"
+msgstr "RSS-канали"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/ru/LC_MESSAGES/django.po` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/cs/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Nikolay <nick.postnikov@gmail.com>, 2023.
-# Dromiel <dimhry@yandex.ru>, 2024.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-11-15 18:12+0100\n"
-"PO-Revision-Date: 2024-01-17 18:05+0000\n"
-"Last-Translator: Dromiel <dimhry@yandex.ru>\n"
-"Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-rss-to-discord/ru/>\n"
-"Language: ru\n"
+"POT-Creation-Date: 2024-03-20 17:13+0100\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Czech <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-rss-to-discord/cs/>\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
-"n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.3.1\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n "
+"<= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_rss_to_discord/__init__.py:9
 msgid "RSS to Discord"
-msgstr "RSS к Дискорду"
+msgstr ""
 
 #: aa_rss_to_discord/models.py:41
 msgid "RSS Feed"
-msgstr "RSS лента"
+msgstr ""
 
 #: aa_rss_to_discord/models.py:42
 msgid "RSS Feeds"
-msgstr "RSS ленты"
+msgstr ""
 
 #: aa_rss_to_discord/models.py:69
 msgid "Last Item"
-msgstr "Последний элемент"
+msgstr ""
 
 #: aa_rss_to_discord/models.py:70
 msgid "Last Items"
-msgstr "Последние элементы"
+msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/uk/LC_MESSAGES/django.po` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/uk/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

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
 "POT-Creation-Date: 2023-11-15 18:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-rss-to-discord/uk/>\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-rss-to-discord/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_rss_to_discord/__init__.py:9
 msgid "RSS to Discord"
 msgstr ""
 
 #: aa_rss_to_discord/models.py:41
 msgid "RSS Feed"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.mo` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Format-specific differences are supported for Gettext message catalogues but no file-specific differences were detected; falling back to a binary diff. file(1) reports: GNU message catalog (little endian), revision 0.0, 1 message, Project-Id-Version: Chinese (Simplified) (Alliance Auth Apps)*

 * *Files 22% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 00000190: 2f70 6c61 696e 3b20 6368 6172 7365 743d  /plain; charset=
 000001a0: 5554 462d 380a 436f 6e74 656e 742d 5472  UTF-8.Content-Tr
 000001b0: 616e 7366 6572 2d45 6e63 6f64 696e 673a  ansfer-Encoding:
 000001c0: 2038 6269 740a 506c 7572 616c 2d46 6f72   8bit.Plural-For
 000001d0: 6d73 3a20 6e70 6c75 7261 6c73 3d31 3b20  ms: nplurals=1; 
 000001e0: 706c 7572 616c 3d30 3b0a 582d 4765 6e65  plural=0;.X-Gene
 000001f0: 7261 746f 723a 2057 6562 6c61 7465 2035  rator: Weblate 5
-00000200: 2e30 2e32 0a00                           .0.2..
+00000200: 2e35 2e33 0a00                           .5.3..
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/locale/ja/LC_MESSAGES/django.po`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "POT-Creation-Date: 2023-11-15 18:12+0100\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"PO-Revision-Date: 2024-05-10 14:10+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
-"alliance-auth-apps/aa-rss-to-discord/zh_Hans/>\n"
-"Language: zh_Hans\n"
+"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-rss-to-discord/ja/>\n"
+"Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 #: aa_rss_to_discord/__init__.py:9
 msgid "RSS to Discord"
 msgstr ""
 
 #: aa_rss_to_discord/models.py:41
 msgid "RSS Feed"
```

### Comparing `aa_rss_to_discord-2.0.0b2/aa_rss_to_discord/migrations/0001_initial.py` & `aa_rss_to_discord-2.0.1/aa_rss_to_discord/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-2.0.0b2/LICENSE` & `aa_rss_to_discord-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-2.0.0b2/README.md` & `aa_rss_to_discord-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `aa_rss_to_discord-2.0.0b2/pyproject.toml` & `aa_rss_to_discord-2.0.1/pyproject.toml`

 * *Files 10% similar despite different names*

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
     "allianceauth-app-utils>=1.14.2",
     "allianceauth-discordbot>=3.0.5",
     "feedparser",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
     "coverage",
```

### Comparing `aa_rss_to_discord-2.0.0b2/PKG-INFO` & `aa_rss_to_discord-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aa-rss-to-discord
-Version: 2.0.0b2
+Version: 2.0.1
 Summary: Alliance Auth module to post news from RSS feeds to your Discord
 Project-URL: Changelog, https://github.com/ppfeufer/aa-rss-to-discord/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-rss-to-discord/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-rss-to-discord
 Project-URL: Source, https://github.com/ppfeufer/aa-rss-to-discord.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-rss-to-discord/issues
@@ -699,15 +699,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.14.2
 Requires-Dist: allianceauth-discordbot>=3.0.5
-Requires-Dist: allianceauth>=4.0.0b1
+Requires-Dist: allianceauth<5.0.0,>=4
 Requires-Dist: feedparser
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
 
 # Alliance Auth RSS to Discord<a name="alliance-auth-rss-to-discord"></a>
```

