# Comparing `tmp/slidge-0.1.2.tar.gz` & `tmp/slidge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slidge-0.1.2.tar", max compression
+gzip compressed data, was "slidge-0.1.3.tar", max compression
```

## Comparing `slidge-0.1.2.tar` & `slidge-0.1.3.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0    34523 2024-05-15 04:30:01.982549 slidge-0.1.2/LICENSE
--rw-r--r--   0        0        0     3706 2024-05-15 04:30:01.982549 slidge-0.1.2/README.md
--rw-r--r--   0        0        0     2088 2024-05-15 04:30:17.436757 slidge-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1624 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/__init__.py
--rw-r--r--   0        0        0     5804 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/__main__.py
--rw-r--r--   0        0        0      613 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/__init__.py
--rw-r--r--   0        0        0     9188 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/adhoc.py
--rw-r--r--   0        0        0     5759 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/admin.py
--rw-r--r--   0        0        0    13073 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/base.py
--rw-r--r--   0        0        0       99 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/categories.py
--rw-r--r--   0        0        0     9975 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/chat_command.py
--rw-r--r--   0        0        0     6014 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/register.py
--rw-r--r--   0        0        0     8781 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/command/user.py
--rw-r--r--   0        0        0      191 2024-05-15 04:30:01.995969 slidge-0.1.2/slidge/contact/__init__.py
--rw-r--r--   0        0        0    16101 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/contact/contact.py
--rw-r--r--   0        0        0     7489 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/contact/roster.py
--rw-r--r--   0        0        0       68 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/__init__.py
--rw-r--r--   0        0        0     5443 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/cache.py
--rw-r--r--   0        0        0     7392 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/config.py
--rw-r--r--   0        0        0       58 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/__init__.py
--rw-r--r--   0        0        0    34645 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/base.py
--rw-r--r--   0        0        0     1919 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/caps.py
--rw-r--r--   0        0        0     1352 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/delivery_receipt.py
--rw-r--r--   0        0        0     2230 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/disco.py
--rw-r--r--   0        0        0     2471 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/mam.py
--rw-r--r--   0        0        0     1033 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/muc_admin.py
--rw-r--r--   0        0        0     1753 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/ping.py
--rw-r--r--   0        0        0     2732 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/presence.py
--rw-r--r--   0        0        0     1619 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/registration.py
--rw-r--r--   0        0        0     3518 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/search.py
--rw-r--r--   0        0        0    29193 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/session_dispatcher.py
--rw-r--r--   0        0        0     4639 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/gateway/vcard_temp.py
--rw-r--r--   0        0        0      368 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/__init__.py
--rw-r--r--   0        0        0    17808 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/attachment.py
--rw-r--r--   0        0        0     5493 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/avatar.py
--rw-r--r--   0        0        0      702 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/base.py
--rw-r--r--   0        0        0     3935 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/disco.py
--rw-r--r--   0        0        0      913 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/lock.py
--rw-r--r--   0        0        0    14790 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/message.py
--rw-r--r--   0        0        0     5606 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/message_maker.py
--rw-r--r--   0        0        0     7216 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/presence.py
--rw-r--r--   0        0        0     1302 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/mixins/recipient.py
--rw-r--r--   0        0        0    18268 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/pubsub.py
--rw-r--r--   0        0        0    26134 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/core/session.py
--rw-r--r--   0        0        0      258 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/__init__.py
--rw-r--r--   0        0        0     3426 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/archive.py
--rw-r--r--   0        0        0     5944 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/bookmarks.py
--rw-r--r--   0        0        0    14908 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/participant.py
--rw-r--r--   0        0        0    38972 2024-05-15 04:30:01.999324 slidge-0.1.2/slidge/group/room.py
--rw-r--r--   0        0        0      334 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/migration.py
--rw-r--r--   0        0        0        0 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/py.typed
--rw-r--r--   0        0        0     1777 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/__init__.py
--rw-r--r--   0        0        0      290 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/link_preview/__init__.py
--rw-r--r--   0        0        0      448 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/link_preview/link_preview.py
--rw-r--r--   0        0        0     2664 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/link_preview/stanza.py
--rw-r--r--   0        0        0     1545 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/roster.py
--rw-r--r--   0        0        0      325 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0077/__init__.py
--rw-r--r--   0        0        0    10431 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0077/register.py
--rw-r--r--   0        0        0     2410 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0077/stanza.py
--rw-r--r--   0        0        0      107 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0100/__init__.py
--rw-r--r--   0        0        0     4501 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0100/gateway.py
--rw-r--r--   0        0        0      232 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0100/stanza.py
--rw-r--r--   0        0        0      319 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0153/__init__.py
--rw-r--r--   0        0        0      735 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0153/stanza.py
--rw-r--r--   0        0        0      658 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0153/vcard_avatar.py
--rw-r--r--   0        0        0      109 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0264/__init__.py
--rw-r--r--   0        0        0      864 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0264/stanza.py
--rw-r--r--   0        0        0      456 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0264/thumbnail.py
--rw-r--r--   0        0        0       98 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0292/__init__.py
--rw-r--r--   0        0        0     3113 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0292/vcard4.py
--rw-r--r--   0        0        0      368 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0313/__init__.py
--rw-r--r--   0        0        0     9211 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0313/mam.py
--rw-r--r--   0        0        0    10249 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0313/stanza.py
--rw-r--r--   0        0        0      104 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0317/__init__.py
--rw-r--r--   0        0        0      290 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0317/hats.py
--rw-r--r--   0        0        0      659 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0317/stanza.py
--rw-r--r--   0        0        0      180 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0356_old/__init__.py
--rw-r--r--   0        0        0     5338 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0356_old/privilege.py
--rw-r--r--   0        0        0     1229 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0356_old/stanza.py
--rw-r--r--   0        0        0      284 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0424/__init__.py
--rw-r--r--   0        0        0     2448 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0424/retraction.py
--rw-r--r--   0        0        0      753 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0424/stanza.py
--rw-r--r--   0        0        0      158 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0490/__init__.py
--rw-r--r--   0        0        0     1527 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0490/mds.py
--rw-r--r--   0        0        0      443 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/slixfix/xep_0490/stanza.py
--rw-r--r--   0        0        0      301 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/__init__.py
--rw-r--r--   0        0        0     1686 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/archive_msg.py
--rw-r--r--   0        0        0     6613 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/conf.py
--rw-r--r--   0        0        0     6604 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/db.py
--rw-r--r--   0        0        0     2682 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/schema.sql
--rw-r--r--   0        0        0    16517 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/sql.py
--rw-r--r--   0        0        0    10688 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/test.py
--rw-r--r--   0        0        0     4689 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/types.py
--rw-r--r--   0        0        0     8587 2024-05-15 04:30:02.002679 slidge-0.1.2/slidge/util/util.py
--rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 slidge-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-16 18:23:54.463529 slidge-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3706 2024-05-16 18:23:54.463529 slidge-0.1.3/README.md
+-rw-r--r--   0        0        0     2088 2024-05-16 18:24:09.103529 slidge-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1624 2024-05-16 18:23:54.480195 slidge-0.1.3/slidge/__init__.py
+-rw-r--r--   0        0        0     5804 2024-05-16 18:23:54.480195 slidge-0.1.3/slidge/__main__.py
+-rw-r--r--   0        0        0      613 2024-05-16 18:23:54.480195 slidge-0.1.3/slidge/command/__init__.py
+-rw-r--r--   0        0        0     9188 2024-05-16 18:23:54.480195 slidge-0.1.3/slidge/command/adhoc.py
+-rw-r--r--   0        0        0     5759 2024-05-16 18:23:54.480195 slidge-0.1.3/slidge/command/admin.py
+-rw-r--r--   0        0        0    13073 2024-05-16 18:23:54.480195 slidge-0.1.3/slidge/command/base.py
+-rw-r--r--   0        0        0       99 2024-05-16 18:23:54.480195 slidge-0.1.3/slidge/command/categories.py
+-rw-r--r--   0        0        0     9975 2024-05-16 18:23:54.480195 slidge-0.1.3/slidge/command/chat_command.py
+-rw-r--r--   0        0        0     6014 2024-05-16 18:23:54.480195 slidge-0.1.3/slidge/command/register.py
+-rw-r--r--   0        0        0     8781 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/command/user.py
+-rw-r--r--   0        0        0      191 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/contact/__init__.py
+-rw-r--r--   0        0        0    16101 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/contact/contact.py
+-rw-r--r--   0        0        0     7489 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/contact/roster.py
+-rw-r--r--   0        0        0       68 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/__init__.py
+-rw-r--r--   0        0        0     5443 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/cache.py
+-rw-r--r--   0        0        0     7392 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/config.py
+-rw-r--r--   0        0        0       58 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/__init__.py
+-rw-r--r--   0        0        0    34645 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/base.py
+-rw-r--r--   0        0        0     1919 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/caps.py
+-rw-r--r--   0        0        0     1352 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/delivery_receipt.py
+-rw-r--r--   0        0        0     2230 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/disco.py
+-rw-r--r--   0        0        0     2471 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/mam.py
+-rw-r--r--   0        0        0     1033 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/muc_admin.py
+-rw-r--r--   0        0        0     1753 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/ping.py
+-rw-r--r--   0        0        0     2732 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/presence.py
+-rw-r--r--   0        0        0     1619 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/registration.py
+-rw-r--r--   0        0        0     3518 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/search.py
+-rw-r--r--   0        0        0    29641 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/session_dispatcher.py
+-rw-r--r--   0        0        0     4639 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/gateway/vcard_temp.py
+-rw-r--r--   0        0        0      368 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/mixins/__init__.py
+-rw-r--r--   0        0        0    17808 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/mixins/attachment.py
+-rw-r--r--   0        0        0     5493 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/mixins/avatar.py
+-rw-r--r--   0        0        0      702 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/mixins/base.py
+-rw-r--r--   0        0        0     3935 2024-05-16 18:23:54.483529 slidge-0.1.3/slidge/core/mixins/disco.py
+-rw-r--r--   0        0        0      913 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/core/mixins/lock.py
+-rw-r--r--   0        0        0    14790 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/core/mixins/message.py
+-rw-r--r--   0        0        0     5606 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/core/mixins/message_maker.py
+-rw-r--r--   0        0        0     7216 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/core/mixins/presence.py
+-rw-r--r--   0        0        0     1302 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/core/mixins/recipient.py
+-rw-r--r--   0        0        0    18268 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/core/pubsub.py
+-rw-r--r--   0        0        0    26134 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/core/session.py
+-rw-r--r--   0        0        0      258 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/group/__init__.py
+-rw-r--r--   0        0        0     3426 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/group/archive.py
+-rw-r--r--   0        0        0     5944 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/group/bookmarks.py
+-rw-r--r--   0        0        0    14947 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/group/participant.py
+-rw-r--r--   0        0        0    38972 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/group/room.py
+-rw-r--r--   0        0        0      334 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/migration.py
+-rw-r--r--   0        0        0        0 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/py.typed
+-rw-r--r--   0        0        0     1777 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/link_preview/__init__.py
+-rw-r--r--   0        0        0      448 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/link_preview/link_preview.py
+-rw-r--r--   0        0        0     2664 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/link_preview/stanza.py
+-rw-r--r--   0        0        0     1545 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/roster.py
+-rw-r--r--   0        0        0      325 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/xep_0077/__init__.py
+-rw-r--r--   0        0        0    10431 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/xep_0077/register.py
+-rw-r--r--   0        0        0     2410 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/xep_0077/stanza.py
+-rw-r--r--   0        0        0      107 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/xep_0100/__init__.py
+-rw-r--r--   0        0        0     4501 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/xep_0100/gateway.py
+-rw-r--r--   0        0        0      232 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/xep_0100/stanza.py
+-rw-r--r--   0        0        0      319 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/xep_0153/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-16 18:23:54.486862 slidge-0.1.3/slidge/slixfix/xep_0153/stanza.py
+-rw-r--r--   0        0        0      658 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0153/vcard_avatar.py
+-rw-r--r--   0        0        0      109 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0264/__init__.py
+-rw-r--r--   0        0        0      864 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0264/stanza.py
+-rw-r--r--   0        0        0      456 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0264/thumbnail.py
+-rw-r--r--   0        0        0       98 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0292/__init__.py
+-rw-r--r--   0        0        0     3113 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0292/vcard4.py
+-rw-r--r--   0        0        0      368 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0313/__init__.py
+-rw-r--r--   0        0        0     9211 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0313/mam.py
+-rw-r--r--   0        0        0    10249 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0313/stanza.py
+-rw-r--r--   0        0        0      104 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0317/__init__.py
+-rw-r--r--   0        0        0      290 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0317/hats.py
+-rw-r--r--   0        0        0      659 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0317/stanza.py
+-rw-r--r--   0        0        0      180 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0356_old/__init__.py
+-rw-r--r--   0        0        0     5338 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0356_old/privilege.py
+-rw-r--r--   0        0        0     1229 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0356_old/stanza.py
+-rw-r--r--   0        0        0      284 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0424/__init__.py
+-rw-r--r--   0        0        0     2448 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0424/retraction.py
+-rw-r--r--   0        0        0      753 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0424/stanza.py
+-rw-r--r--   0        0        0      158 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0490/__init__.py
+-rw-r--r--   0        0        0     1527 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0490/mds.py
+-rw-r--r--   0        0        0      443 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/slixfix/xep_0490/stanza.py
+-rw-r--r--   0        0        0      301 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/util/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/util/archive_msg.py
+-rw-r--r--   0        0        0     6613 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/util/conf.py
+-rw-r--r--   0        0        0     6604 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/util/db.py
+-rw-r--r--   0        0        0     2682 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/util/schema.sql
+-rw-r--r--   0        0        0    16517 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/util/sql.py
+-rw-r--r--   0        0        0    10688 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/util/test.py
+-rw-r--r--   0        0        0     4689 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/util/types.py
+-rw-r--r--   0        0        0     8587 2024-05-16 18:23:54.490195 slidge-0.1.3/slidge/util/util.py
+-rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 slidge-0.1.3/PKG-INFO
```

### Comparing `slidge-0.1.2/LICENSE` & `slidge-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/README.md` & `slidge-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/pyproject.toml` & `slidge-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slidge"
-version = "0.1.2"
+version = "0.1.3"
 description = "XMPP bridging framework"
 authors = ["Nicolas Cedilnik <nicoco@nicoco.fr>"]
 readme = "README.md"
 license = "AGPL-3.0-or-later"
 homepage = "https://sr.ht/~nicoco/slidge/"
 repository = "https://git.sr.ht/~nicoco/slidge/"
 documentation = "https://slidge.im/"
```

### Comparing `slidge-0.1.2/slidge/__init__.py` & `slidge-0.1.3/slidge/__init__.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/__main__.py` & `slidge-0.1.3/slidge/__main__.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/command/__init__.py` & `slidge-0.1.3/slidge/command/__init__.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/command/adhoc.py` & `slidge-0.1.3/slidge/command/adhoc.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/command/admin.py` & `slidge-0.1.3/slidge/command/admin.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/command/base.py` & `slidge-0.1.3/slidge/command/base.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/command/chat_command.py` & `slidge-0.1.3/slidge/command/chat_command.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/command/register.py` & `slidge-0.1.3/slidge/command/register.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/command/user.py` & `slidge-0.1.3/slidge/command/user.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/contact/contact.py` & `slidge-0.1.3/slidge/contact/contact.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/contact/roster.py` & `slidge-0.1.3/slidge/contact/roster.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/cache.py` & `slidge-0.1.3/slidge/core/cache.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/config.py` & `slidge-0.1.3/slidge/core/config.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/base.py` & `slidge-0.1.3/slidge/core/gateway/base.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/caps.py` & `slidge-0.1.3/slidge/core/gateway/caps.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/delivery_receipt.py` & `slidge-0.1.3/slidge/core/gateway/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/disco.py` & `slidge-0.1.3/slidge/core/gateway/disco.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/mam.py` & `slidge-0.1.3/slidge/core/gateway/mam.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/muc_admin.py` & `slidge-0.1.3/slidge/core/gateway/muc_admin.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/ping.py` & `slidge-0.1.3/slidge/core/gateway/ping.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/presence.py` & `slidge-0.1.3/slidge/core/gateway/presence.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/registration.py` & `slidge-0.1.3/slidge/core/gateway/registration.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/search.py` & `slidge-0.1.3/slidge/core/gateway/search.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/gateway/session_dispatcher.py` & `slidge-0.1.3/slidge/core/gateway/session_dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -444,14 +444,23 @@
                 mc["reactions"]["id"] = xmpp_id
                 await entity.echo(mc)
         elif isinstance(entity, LegacyContact):
             for xmpp_id in multi:
                 entity.react(legacy_id, emojis, xmpp_id=xmpp_id, carbon=True)
 
     async def on_presence(self, p: Presence):
+        if p.get_plugin("muc_join", check=True):
+            # handled in on_groupchat_join
+            # without this early return, since we switch from and to in this
+            # presence stanza, on_groupchat_join ends up trying to instantiate
+            # a MUC with the user's JID, which in turn leads to slidge sending
+            # a (error) presence from=the user's JID, which terminates the
+            # XML stream.
+            return
+
         session = await self.__get_session(p)
 
         pto = p.get_to()
         if pto == self.xmpp.boundjid.bare:
             # NB: get_type() returns either a proper presence type or
             #     a presence show if available. Weird, weird, weird slix.
             if (ptype := p.get_type()) not in _USEFUL_PRESENCES:
```

### Comparing `slidge-0.1.2/slidge/core/gateway/vcard_temp.py` & `slidge-0.1.3/slidge/core/gateway/vcard_temp.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/mixins/attachment.py` & `slidge-0.1.3/slidge/core/mixins/attachment.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/mixins/avatar.py` & `slidge-0.1.3/slidge/core/mixins/avatar.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/mixins/base.py` & `slidge-0.1.3/slidge/core/mixins/base.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/mixins/disco.py` & `slidge-0.1.3/slidge/core/mixins/disco.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/mixins/lock.py` & `slidge-0.1.3/slidge/core/mixins/lock.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/mixins/message.py` & `slidge-0.1.3/slidge/core/mixins/message.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/mixins/message_maker.py` & `slidge-0.1.3/slidge/core/mixins/message_maker.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/mixins/presence.py` & `slidge-0.1.3/slidge/core/mixins/presence.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/mixins/recipient.py` & `slidge-0.1.3/slidge/core/mixins/recipient.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/pubsub.py` & `slidge-0.1.3/slidge/core/pubsub.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/core/session.py` & `slidge-0.1.3/slidge/core/session.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/group/archive.py` & `slidge-0.1.3/slidge/group/archive.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/group/bookmarks.py` & `slidge-0.1.3/slidge/group/bookmarks.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/group/participant.py` & `slidge-0.1.3/slidge/group/participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
         self.send_last_presence(force=True, no_cache_online=True)
 
     def __update_jid(self, unescaped_nickname: Optional[str]):
         j: JID = copy(self.muc.jid)
 
         if self.is_system:
             self.jid = j
+            self._nickname_no_illegal = ""
             return
 
         nickname = unescaped_nickname
 
         if nickname:
             nickname = self._nickname_no_illegal = strip_illegal_chars(nickname)
         else:
@@ -209,15 +210,14 @@
         p["muc"]["item"]["nick"] = self.jid.resource
         self._send(p)
 
         self._nickname = new_nickname
 
         kwargs["status_codes"] = set()
         p = self._make_presence(ptype="available", last_seen=last_seen, **kwargs)
-        self.__add_nick_element(p)
         self._send(p)
 
         if old:
             self.muc.rename_participant(old, new_nickname)
 
     def _make_presence(
         self,
@@ -297,14 +297,15 @@
         self,
         stanza: MessageOrPresenceTypeVar,
         full_jid: Optional[JID] = None,
         archive_only=False,
         **send_kwargs,
     ) -> MessageOrPresenceTypeVar:
         stanza["occupant-id"]["id"] = self.__occupant_id
+        self.__add_nick_element(stanza)
         if isinstance(stanza, Presence):
             if stanza["type"] == "unavailable" and not self.__presence_sent:
                 return stanza  # type:ignore
             self.__presence_sent = True
         if full_jid:
             stanza["to"] = full_jid
             self.__send_presence_if_needed(stanza, full_jid, archive_only)
@@ -340,19 +341,19 @@
                     (
                         f"Public group but no contact JID associated to {self.jid} in"
                         f" {self}"
                     ),
                 )
         return item
 
-    def __add_nick_element(self, p: Presence):
+    def __add_nick_element(self, stanza: Union[Presence, Message]):
         if (nick := self._nickname_no_illegal) != self.jid.resource:
             n = self.xmpp.plugin["xep_0172"].stanza.UserNick()
             n["nick"] = nick
-            p.append(n)
+            stanza.append(n)
 
     def _get_last_presence(self) -> Optional[CachedPresence]:
         own = super()._get_last_presence()
         if own is None and self.contact:
             return self.contact._get_last_presence()
         return own
 
@@ -396,15 +397,14 @@
         p = self._make_presence(
             status_codes=codes,
             user_full_jid=full_jid,
             **kwargs,  # type:ignore
         )
         if presence_id:
             p["id"] = presence_id
-        self.__add_nick_element(p)
         self._send(p, full_jid)
 
     def leave(self):
         """
         Call this when the participant leaves the room
         """
         self.muc.remove_participant(self)
```

### Comparing `slidge-0.1.2/slidge/group/room.py` & `slidge-0.1.3/slidge/group/room.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/__init__.py` & `slidge-0.1.3/slidge/slixfix/__init__.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/link_preview/stanza.py` & `slidge-0.1.3/slidge/slixfix/link_preview/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/roster.py` & `slidge-0.1.3/slidge/slixfix/roster.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0077/register.py` & `slidge-0.1.3/slidge/slixfix/xep_0077/register.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0077/stanza.py` & `slidge-0.1.3/slidge/slixfix/xep_0077/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0100/gateway.py` & `slidge-0.1.3/slidge/slixfix/xep_0100/gateway.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0153/stanza.py` & `slidge-0.1.3/slidge/slixfix/xep_0153/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0153/vcard_avatar.py` & `slidge-0.1.3/slidge/slixfix/xep_0153/vcard_avatar.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0264/stanza.py` & `slidge-0.1.3/slidge/slixfix/xep_0264/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0292/vcard4.py` & `slidge-0.1.3/slidge/slixfix/xep_0292/vcard4.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0313/mam.py` & `slidge-0.1.3/slidge/slixfix/xep_0313/mam.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0313/stanza.py` & `slidge-0.1.3/slidge/slixfix/xep_0313/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0317/stanza.py` & `slidge-0.1.3/slidge/slixfix/xep_0317/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0356_old/privilege.py` & `slidge-0.1.3/slidge/slixfix/xep_0356_old/privilege.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0356_old/stanza.py` & `slidge-0.1.3/slidge/slixfix/xep_0356_old/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0424/retraction.py` & `slidge-0.1.3/slidge/slixfix/xep_0424/retraction.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0424/stanza.py` & `slidge-0.1.3/slidge/slixfix/xep_0424/stanza.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/slixfix/xep_0490/mds.py` & `slidge-0.1.3/slidge/slixfix/xep_0490/mds.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/util/archive_msg.py` & `slidge-0.1.3/slidge/util/archive_msg.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/util/conf.py` & `slidge-0.1.3/slidge/util/conf.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/util/db.py` & `slidge-0.1.3/slidge/util/db.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/util/schema.sql` & `slidge-0.1.3/slidge/util/schema.sql`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/util/sql.py` & `slidge-0.1.3/slidge/util/sql.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/util/test.py` & `slidge-0.1.3/slidge/util/test.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/util/types.py` & `slidge-0.1.3/slidge/util/types.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/slidge/util/util.py` & `slidge-0.1.3/slidge/util/util.py`

 * *Files identical despite different names*

### Comparing `slidge-0.1.2/PKG-INFO` & `slidge-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slidge
-Version: 0.1.2
+Version: 0.1.3
 Summary: XMPP bridging framework
 Home-page: https://sr.ht/~nicoco/slidge/
 License: AGPL-3.0-or-later
 Author: Nicolas Cedilnik
 Author-email: nicoco@nicoco.fr
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

