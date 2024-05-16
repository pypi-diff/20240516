# Comparing `tmp/an-website-24.4.tar.gz` & `tmp/an-website-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "an-website-24.4.tar", last modified: Mon Apr  1 01:23:30 2024, max compression
+gzip compressed data, was "an-website-24.5.tar", last modified: Thu May 16 06:02:26 2024, max compression
```

## Comparing `an-website-24.4.tar` & `an-website-24.5.tar`

### file list

```diff
@@ -1,468 +1,468 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.712376 an-website-24.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-01 01:23:01.000000 an-website-24.4/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    34351 2024-04-01 01:23:01.000000 an-website-24.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-01 01:23:01.000000 an-website-24.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-01 01:23:30.712376 an-website-24.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-01 01:23:01.000000 an-website-24.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-01 01:23:30.000000 an-website-24.4/REVISION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.636376 an-website-24.4/an_website/
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-01 01:23:01.000000 an-website-24.4/an_website/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-01 01:23:01.000000 an-website-24.4/an_website/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.636376 an-website-24.4/an_website/backdoor/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-01 01:23:01.000000 an-website-24.4/an_website/backdoor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-04-01 01:23:01.000000 an-website-24.4/an_website/backdoor/backdoor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23349 2024-04-01 01:23:01.000000 an-website-24.4/an_website/backdoor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   800629 2024-04-01 01:23:01.000000 an-website-24.4/an_website/ca-bundle.crt
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-01 01:23:01.000000 an-website-24.4/an_website/ca-license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.636376 an-website-24.4/an_website/commitment/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-01 01:23:01.000000 an-website-24.4/an_website/commitment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-01 01:23:01.000000 an-website-24.4/an_website/commitment/commitment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.636376 an-website-24.4/an_website/contact/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-01 01:23:01.000000 an-website-24.4/an_website/contact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9383 2024-04-01 01:23:01.000000 an-website-24.4/an_website/contact/contact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.636376 an-website-24.4/an_website/currency_converter/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-01 01:23:01.000000 an-website-24.4/an_website/currency_converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9496 2024-04-01 01:23:01.000000 an-website-24.4/an_website/currency_converter/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.636376 an-website-24.4/an_website/discord/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-01 01:23:01.000000 an-website-24.4/an_website/discord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-01 01:23:01.000000 an-website-24.4/an_website/discord/discord.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.624376 an-website-24.4/an_website/elasticsearch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.624376 an-website-24.4/an_website/elasticsearch/component_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.644376 an-website-24.4/an_website/elasticsearch/component_templates/ecs/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/agent.json
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/base.json
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/client.json
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/cloud.json
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/container.json
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/data_stream.json
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/destination.json
--rw-r--r--   0 runner    (1001) docker     (127)     7487 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/dll.json
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/dns.json
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/ecs.json
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/email.json
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/error.json
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/event.json
--rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/file.json
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/group.json
--rw-r--r--   0 runner    (1001) docker     (127)     6913 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/host.json
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/http.json
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/log.json
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/network.json
--rw-r--r--   0 runner    (1001) docker     (127)     6135 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/observer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/orchestrator.json
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/organization.json
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/package.json
--rw-r--r--   0 runner    (1001) docker     (127)    59330 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/process.json
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/registry.json
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/related.json
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/rule.json
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/server.json
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/service.json
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/source.json
--rw-r--r--   0 runner    (1001) docker     (127)    73278 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/threat.json
--rw-r--r--   0 runner    (1001) docker     (127)    11965 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/tls.json
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/tracing.json
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/url.json
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/user.json
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/user_agent.json
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/component_templates/ecs/vulnerability.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.644376 an-website-24.4/an_website/elasticsearch/index_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/index_templates/reporting.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.644376 an-website-24.4/an_website/elasticsearch/index_templates/shortener/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/index_templates/shortener/shorten.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.644376 an-website-24.4/an_website/elasticsearch/ingest_pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/ingest_pipelines/reporting.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.644376 an-website-24.4/an_website/elasticsearch/ingest_pipelines/shortener/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-01 01:23:01.000000 an-website-24.4/an_website/elasticsearch/ingest_pipelines/shortener/shorten.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.644376 an-website-24.4/an_website/element_web_link/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-01 01:23:01.000000 an-website-24.4/an_website/element_web_link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-01 01:23:01.000000 an-website-24.4/an_website/element_web_link/element_web_link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/emoji_chat/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-01 01:23:01.000000 an-website-24.4/an_website/emoji_chat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-01 01:23:01.000000 an-website-24.4/an_website/emoji_chat/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-01 01:23:01.000000 an-website-24.4/an_website/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-01 01:23:01.000000 an-website-24.4/an_website/endpoints/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/example/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-01 01:23:01.000000 an-website-24.4/an_website/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-01 01:23:01.000000 an-website-24.4/an_website/example/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-01 01:23:01.000000 an-website-24.4/an_website/fake_orjson.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/hangman_solver/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-01 01:23:01.000000 an-website-24.4/an_website/hangman_solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-04-01 01:23:01.000000 an-website-24.4/an_website/hangman_solver/hangman_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-01 01:23:01.000000 an-website-24.4/an_website/hangman_solver/wordgame_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/host_info/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-01 01:23:01.000000 an-website-24.4/an_website/host_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-01 01:23:01.000000 an-website-24.4/an_website/host_info/host_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/js_licenses/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-01 01:23:01.000000 an-website-24.4/an_website/js_licenses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-01 01:23:01.000000 an-website-24.4/an_website/js_licenses/js_licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/kangaroo_comics/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-01 01:23:01.000000 an-website-24.4/an_website/kangaroo_comics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-01 01:23:01.000000 an-website-24.4/an_website/kangaroo_comics/comics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/lolwut/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-01 01:23:01.000000 an-website-24.4/an_website/lolwut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-01 01:23:01.000000 an-website-24.4/an_website/lolwut/lolwut.py
--rw-r--r--   0 runner    (1001) docker     (127)    42730 2024-04-01 01:23:01.000000 an-website-24.4/an_website/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/main_page/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-01 01:23:01.000000 an-website-24.4/an_website/main_page/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-01 01:23:01.000000 an-website-24.4/an_website/main_page/main_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.648376 an-website-24.4/an_website/patches/
--rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-04-01 01:23:01.000000 an-website-24.4/an_website/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-01 01:23:01.000000 an-website-24.4/an_website/patches/braille.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-01 01:23:01.000000 an-website-24.4/an_website/patches/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.652376 an-website-24.4/an_website/ping/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-01 01:23:01.000000 an-website-24.4/an_website/ping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-01 01:23:01.000000 an-website-24.4/an_website/ping/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    62500 2024-04-01 01:23:01.000000 an-website-24.4/an_website/primes.bin
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:01.000000 an-website-24.4/an_website/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.652376 an-website-24.4/an_website/quotes/
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/create.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1437 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/edit.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.652376 an-website-24.4/an_website/quotes/files/
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/files/StempelNichtWitzig.png
--rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/files/StempelWitzig.png
--rw-r--r--   0 runner    (1001) docker     (127)    42308 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/files/bg.png
--rw-r--r--   0 runner    (1001) docker     (127)    50944 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/files/oswald.regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7514 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.652376 an-website-24.4/an_website/quotes/quote_of_the_day/
--rw-r--r--   0 runner    (1001) docker     (127)     5687 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/quote_of_the_day/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/quote_of_the_day/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/quote_of_the_day/store.py
--rw-r--r--   0 runner    (1001) docker     (127)    17654 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/quotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/share.py
--rw-r--r--   0 runner    (1001) docker     (127)    25686 2024-04-01 01:23:01.000000 an-website-24.4/an_website/quotes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.652376 an-website-24.4/an_website/random_text/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-01 01:23:01.000000 an-website-24.4/an_website/random_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-01 01:23:01.000000 an-website-24.4/an_website/random_text/random_text.py
--rw-r--r--   0 runner    (1001) docker     (127)  3039490 2024-04-01 01:23:01.000000 an-website-24.4/an_website/random_text/words.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.660376 an-website-24.4/an_website/redirect/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-01 01:23:01.000000 an-website-24.4/an_website/redirect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-01 01:23:01.000000 an-website-24.4/an_website/redirect/redirect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.660376 an-website-24.4/an_website/reporting/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-01 01:23:01.000000 an-website-24.4/an_website/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8680 2024-04-01 01:23:01.000000 an-website-24.4/an_website/reporting/reporting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.660376 an-website-24.4/an_website/search/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 01:23:01.000000 an-website-24.4/an_website/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-04-01 01:23:01.000000 an-website-24.4/an_website/search/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.660376 an-website-24.4/an_website/services/
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-01 01:23:01.000000 an-website-24.4/an_website/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-01 01:23:01.000000 an-website-24.4/an_website/services/services.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.660376 an-website-24.4/an_website/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-01 01:23:01.000000 an-website-24.4/an_website/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-01 01:23:01.000000 an-website-24.4/an_website/settings/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.660376 an-website-24.4/an_website/snow/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-01 01:23:01.000000 an-website-24.4/an_website/snow/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.660376 an-website-24.4/an_website/soundboard/
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7982 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.672376 an-website-24.4/an_website/soundboard/files/
--rw-r--r--   0 runner    (1001) docker     (127)    50432 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/dietmar-ich_hab_seine_hausaufgaben_aufgegessen.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    70592 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/fw-ihr_linken_intellektuellen_fuzzies.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    43007 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/gott-das_ist_privat.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    81459 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/gott-so_so_du_hast_also_keine_eier.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    48858 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/jesus-guck_mal_was_ich_kann.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    53986 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-aber_nicht_zu_lidl.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    74486 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-alles_kapitalismus_alles_nestle_alles_haehnchen.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    28211 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-das_ist_freiwillig.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    84635 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-finsterstes_mittelalter_alter.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    46007 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-hallo.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    72923 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-hier_sind_wir_jetzt_unterhalte_uns.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    41997 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-i_love_it.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    49865 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-ich_bin_kommunist.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    59749 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-ich_darf_nich_und_ich_will_nich.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    90810 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-im_so_happy_for_no_reason_but_i_dont_care.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    48353 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-ja_ja.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    56648 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-kein_problem_ich_hab_zeit.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    47101 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-koestlich.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   113893 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-man_darf_nie_aufhoeren_alles_kritisch_zu_hinterfragen.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    48043 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-ohh_hee.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    70477 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-this_kinda_feels_really_really_awesome.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   191215 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-wir_kaempfen_fuer_eine_gerechte_weltordnung_brot_fuer_alle_und_die_aechtung_von_sogennanntem_musikfernsehen.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    57217 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-wir_sind_keine_intellektuellen.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    51169 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kaenguru-wolln_wir_uns_dutzen.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    38466 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/kuh-ahamumumu.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   120162 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-du_bist_also_teil_der_juedisch-bolschewistischen_weltverschwoerung.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    39036 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-fuer_nichts_und_wieder_nichts.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    67629 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-i_am_bored.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   134445 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-i_am_bored_in_the_usa.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    89930 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-im_just_here_for_the_famous_breakfast.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    33069 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-ja_herzlich_willkommen.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    39663 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-sprich_bitte_nur_fuer_dich.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   189292 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-ueber_mich_hat_die_zeit_geschrieben_dass_ich_der_wahrscheinlich_einflussreichste_linke_interlektulelle_deutschlands_sei.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   127434 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-und_da_ist_mir_aufgefallen_dass_ich_keine_eier_hab.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    56423 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-und_mich_dann_auch_noch_beschneiden_lassen.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    48303 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-von_mir_aus.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    44620 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/muk-yeah.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/psychiater-aha.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    43250 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/sarah-hey_thats_cool.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    46290 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/sarah-i_love_life.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   155900 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/sarah-thats_amazing_its_like_you_know_i_dont_know_kind_of_like_whatever_and_stuff.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    61219 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/sarah-the_world_is_so_beautiful.mp3
--rw-r--r--   0 runner    (1001) docker     (127)   138254 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/sarah-well_thats_just_like_you_know_amazing.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    68839 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/files/sarah-yes_its_just_perfect.mp3
--rw-r--r--   0 runner    (1001) docker     (127)    48809 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/info.json
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-04-01 01:23:01.000000 an-website-24.4/an_website/soundboard/soundboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.672376 an-website-24.4/an_website/static/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/.env
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.676376 an-website-24.4/an_website/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/ansi2html.css
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/ansi2html.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     5793 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/base.css
--rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/base.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/comic.css
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/comic.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/emoji_chat.css
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/emoji_chat.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/error.css
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/error.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/form.css
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/form.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/kangaroo_comics.css
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/kangaroo_comics.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/main_page.css
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/main_page.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.680376 an-website-24.4/an_website/static/css/quotes/
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/quotes/generator.css
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/quotes/generator.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/quotes/info.css
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/quotes/info.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/quotes/quotes.css
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/quotes/quotes.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/quotes/share.css
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/quotes/share.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/redirect.css
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/redirect.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    52690 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/snow.css
--rw-r--r--   0 runner    (1001) docker     (127)    42520 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/snow.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/soundboard.css
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/soundboard.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/table.css
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/table.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.680376 an-website-24.4/an_website/static/css/themes/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/blue.css
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/blue.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/christmas.css
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/christmas.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/default.css
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/default.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/fun.css
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/fun.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/green.css
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/green.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/light.css
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/light.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/light_blue.css
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/light_blue.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/orange.css
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/orange.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/pink.css
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/pink.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/purple.css
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/purple.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/yellow.css
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/themes/yellow.css.map
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/uptime.css
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/css/uptime.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     9109 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/favicon.jxl
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.684376 an-website-24.4/an_website/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/fonts/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    33916 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/fonts/comic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/fonts/comicmono.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/fonts/cursedtimerulil-aznm.woff2
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/humans.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)  1047428 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/2020-11-03.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/hamburger-menu-icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    23613 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/kangarooface.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/netcup-oekostrom2.jxl
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/netcup-oekostrom2.png
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/report.svg
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/rss.svg
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/save.svg
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/share.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/img/stamps/
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/stamps/nichtwitzig.small.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/img/stamps/witzig.small.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.628376 an-website-24.4/an_website/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/js/currency_converter/
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/currency_converter/converter.js
--rw-r--r--   0 runner    (1001) docker     (127)     8735 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/currency_converter/converter.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/js/emoji_chat/
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/emoji_chat/chat.js
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/emoji_chat/chat.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/js/hangman_solver/
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/hangman_solver/hangman_solver.js
--rw-r--r--   0 runner    (1001) docker     (127)    17899 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/hangman_solver/hangman_solver.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/js/kangaroo_comics/
--rw-r--r--   0 runner    (1001) docker     (127)     7854 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/kangaroo_comics/comics.js
--rw-r--r--   0 runner    (1001) docker     (127)    22712 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/kangaroo_comics/comics.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/js/quotes/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/quotes/create.js
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/quotes/create.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/quotes/quotes.js
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/quotes/quotes.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/js/search/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/search/search.js
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/search/search.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/js/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/settings/settings.js
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/settings/settings.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/js/snow/
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/snow/snow.js
--rw-r--r--   0 runner    (1001) docker     (127)     5306 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/snow/snow.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.688376 an-website-24.4/an_website/static/js/swapped_words/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/swapped_words/swap.js
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/swapped_words/swap.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.692376 an-website-24.4/an_website/static/js/uptime/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/uptime/uptime.js
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/uptime/uptime.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.692376 an-website-24.4/an_website/static/js/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/utils/better_ui.js
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/utils/better_ui.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/utils/dynload.js
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/utils/dynload.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/utils/utils.js
--rw-r--r--   0 runner    (1001) docker     (127)     6498 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/utils/utils.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.692376 an-website-24.4/an_website/static/js/vendored/
--rw-r--r--   0 runner    (1001) docker     (127)    95822 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/vendored/vanilla.js
--rw-r--r--   0 runner    (1001) docker     (127)   534836 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/js/vendored/vanilla.js.map
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-01 01:23:01.000000 an-website-24.4/an_website/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.692376 an-website-24.4/an_website/swapped_words/
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-01 01:23:01.000000 an-website-24.4/an_website/swapped_words/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-01 01:23:01.000000 an-website-24.4/an_website/swapped_words/config.sw
--rw-r--r--   0 runner    (1001) docker     (127)    12837 2024-04-01 01:23:01.000000 an-website-24.4/an_website/swapped_words/config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-01 01:23:01.000000 an-website-24.4/an_website/swapped_words/swap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.692376 an-website-24.4/an_website/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/ansi2html.html
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/error.html
--rw-r--r--   0 runner    (1001) docker     (127)     4802 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.696376 an-website-24.4/an_website/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/EXAMPLE.html
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/contact.html
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/converter.html
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/emoji_chat.html
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/empty.html
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/endpoints.html
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/hangman_solver.html
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/ip.html
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/js_licenses.html
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/kangaroo_comics.html
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/main_page.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.700376 an-website-24.4/an_website/templates/pages/quotes/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/quotes/author_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/quotes/create1.html
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/quotes/create2.html
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/quotes/generator.html
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/quotes/info.html
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/quotes/main_page.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/quotes/quote_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/quotes/quotes.html
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/quotes/share.html
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/redirect.html
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/search.html
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/services.html
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/settings.html
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/soundboard.html
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/swapped_words.html
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/troet.html
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/uptime.html
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/version.html
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/pages/wordgame_solver.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.700376 an-website-24.4/an_website/templates/rss/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/rss/quote_of_the_day.xml
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-01 01:23:01.000000 an-website-24.4/an_website/templates/rss/soundboard.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.700376 an-website-24.4/an_website/troet/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-01 01:23:01.000000 an-website-24.4/an_website/troet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-01 01:23:01.000000 an-website-24.4/an_website/troet/troet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.700376 an-website-24.4/an_website/update/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-01 01:23:01.000000 an-website-24.4/an_website/update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-01 01:23:01.000000 an-website-24.4/an_website/update/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.700376 an-website-24.4/an_website/uptime/
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-01 01:23:01.000000 an-website-24.4/an_website/uptime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-04-01 01:23:01.000000 an-website-24.4/an_website/uptime/uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.704376 an-website-24.4/an_website/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40385 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/base_request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/better_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/data_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9034 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/static_file_from_traversable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6753 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/static_file_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    25599 2024-04-01 01:23:01.000000 an-website-24.4/an_website/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.704376 an-website-24.4/an_website/vendored/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.704376 an-website-24.4/an_website/vendored/apm-rum/
--rw-r--r--   0 runner    (1001) docker     (127)   579743 2024-04-01 01:23:01.000000 an-website-24.4/an_website/vendored/apm-rum/elastic-apm-rum.umd.js
--rw-r--r--   0 runner    (1001) docker     (127)    61332 2024-04-01 01:23:01.000000 an-website-24.4/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   263069 2024-04-01 01:23:01.000000 an-website-24.4/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    56683 2024-04-01 01:23:01.000000 an-website-24.4/an_website/vendored/media-types.json
--rw-r--r--   0 runner    (1001) docker     (127)   205599 2024-04-01 01:23:01.000000 an-website-24.4/an_website/vendored/mime-db.json
--rwxr-xr-x   0 runner    (1001) docker     (127)   255236 2024-04-01 01:23:01.000000 an-website-24.4/an_website/vendored/screenfetch
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.704376 an-website-24.4/an_website/version/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-01 01:23:01.000000 an-website-24.4/an_website/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-04-01 01:23:01.000000 an-website-24.4/an_website/version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.704376 an-website-24.4/an_website/whats_my_ip/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-01 01:23:01.000000 an-website-24.4/an_website/whats_my_ip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-01 01:23:01.000000 an-website-24.4/an_website/whats_my_ip/ip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.708376 an-website-24.4/an_website/wiki/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-01 01:23:01.000000 an-website-24.4/an_website/wiki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-01 01:23:01.000000 an-website-24.4/an_website/wiki/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.708376 an-website-24.4/an_website.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-01 01:23:30.000000 an-website-24.4/an_website.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16466 2024-04-01 01:23:30.000000 an-website-24.4/an_website.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 01:23:30.000000 an-website-24.4/an_website.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 01:23:30.000000 an-website-24.4/an_website.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 01:23:28.000000 an-website-24.4/an_website.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-01 01:23:30.000000 an-website-24.4/an_website.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 01:23:30.000000 an-website-24.4/an_website.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     1750 2024-04-01 01:23:01.000000 an-website-24.4/build-oci-image.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.708376 an-website-24.4/example-configurations/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-01 01:23:01.000000 an-website-24.4/example-configurations/config.ini.default
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-01 01:23:01.000000 an-website-24.4/example-configurations/config.ini.example
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.708376 an-website-24.4/example-configurations/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-01 01:23:01.000000 an-website-24.4/example-configurations/nginx/an-website.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.708376 an-website-24.4/example-configurations/supervisord/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-01 01:23:01.000000 an-website-24.4/example-configurations/supervisord/an_website.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-04-01 01:23:01.000000 an-website-24.4/pip-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-01 01:23:01.000000 an-website-24.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 01:23:30.712376 an-website-24.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3612 2024-04-01 01:23:01.000000 an-website-24.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 01:23:30.708376 an-website-24.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_backdoor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_christmas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_commitment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_currency_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3476 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_hangman_solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_quotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_random_text.py
--rw-r--r--   0 runner    (1001) docker     (127)    18637 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_request_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_swapped_words.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_traversable_static_file_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_troet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_uptime.py
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-04-01 01:23:01.000000 an-website-24.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.543903 an-website-24.5/
+-rw-r--r--   0 runner    (1001) docker     (118)     1843 2024-05-16 06:02:16.000000 an-website-24.5/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (118)    34351 2024-05-16 06:02:16.000000 an-website-24.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (118)      246 2024-05-16 06:02:16.000000 an-website-24.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (118)     8194 2024-05-16 06:02:26.542904 an-website-24.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (118)     3443 2024-05-16 06:02:16.000000 an-website-24.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (118)       40 2024-05-16 06:02:26.000000 an-website-24.5/REVISION.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.473903 an-website-24.5/an_website/
+-rw-r--r--   0 runner    (1001) docker     (118)     3742 2024-05-16 06:02:16.000000 an-website-24.5/an_website/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2004 2024-05-16 06:02:16.000000 an-website-24.5/an_website/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.475903 an-website-24.5/an_website/backdoor/
+-rw-r--r--   0 runner    (1001) docker     (118)     1225 2024-05-16 06:02:16.000000 an-website-24.5/an_website/backdoor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)    12974 2024-05-16 06:02:16.000000 an-website-24.5/an_website/backdoor/backdoor.py
+-rwxr-xr-x   0 runner    (1001) docker     (118)    23349 2024-05-16 06:02:16.000000 an-website-24.5/an_website/backdoor/client.py
+-rw-r--r--   0 runner    (1001) docker     (118)   800629 2024-05-16 06:02:16.000000 an-website-24.5/an_website/ca-bundle.crt
+-rw-r--r--   0 runner    (1001) docker     (118)      197 2024-05-16 06:02:16.000000 an-website-24.5/an_website/ca-license.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.475903 an-website-24.5/an_website/commitment/
+-rw-r--r--   0 runner    (1001) docker     (118)      829 2024-05-16 06:02:16.000000 an-website-24.5/an_website/commitment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4699 2024-05-16 06:02:16.000000 an-website-24.5/an_website/commitment/commitment.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.476903 an-website-24.5/an_website/contact/
+-rw-r--r--   0 runner    (1001) docker     (118)      861 2024-05-16 06:02:16.000000 an-website-24.5/an_website/contact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9383 2024-05-16 06:02:16.000000 an-website-24.5/an_website/contact/contact.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.476903 an-website-24.5/an_website/currency_converter/
+-rw-r--r--   0 runner    (1001) docker     (118)      843 2024-05-16 06:02:16.000000 an-website-24.5/an_website/currency_converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9496 2024-05-16 06:02:16.000000 an-website-24.5/an_website/currency_converter/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.476903 an-website-24.5/an_website/discord/
+-rw-r--r--   0 runner    (1001) docker     (118)      859 2024-05-16 06:02:16.000000 an-website-24.5/an_website/discord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6019 2024-05-16 06:02:16.000000 an-website-24.5/an_website/discord/discord.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.463903 an-website-24.5/an_website/elasticsearch/
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.462903 an-website-24.5/an_website/elasticsearch/component_templates/
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.483903 an-website-24.5/an_website/elasticsearch/component_templates/ecs/
+-rw-r--r--   0 runner    (1001) docker     (118)    11358 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (118)      581 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (118)     1016 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/agent.json
+-rw-r--r--   0 runner    (1001) docker     (118)      481 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/base.json
+-rw-r--r--   0 runner    (1001) docker     (118)     5211 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/client.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1996 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/cloud.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2344 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/container.json
+-rw-r--r--   0 runner    (1001) docker     (118)      528 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/data_stream.json
+-rw-r--r--   0 runner    (1001) docker     (118)     5221 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/destination.json
+-rw-r--r--   0 runner    (1001) docker     (118)     7487 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/dll.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2406 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/dns.json
+-rw-r--r--   0 runner    (1001) docker     (118)      378 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/ecs.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2992 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/email.json
+-rw-r--r--   0 runner    (1001) docker     (118)      875 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/error.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2761 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/event.json
+-rw-r--r--   0 runner    (1001) docker     (118)    17010 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/file.json
+-rw-r--r--   0 runner    (1001) docker     (118)      589 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/group.json
+-rw-r--r--   0 runner    (1001) docker     (118)     6913 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/host.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2327 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/http.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2217 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/log.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2169 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/network.json
+-rw-r--r--   0 runner    (1001) docker     (118)     6135 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/observer.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1506 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/orchestrator.json
+-rw-r--r--   0 runner    (1001) docker     (118)      627 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/organization.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1618 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/package.json
+-rw-r--r--   0 runner    (1001) docker     (118)    59330 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/process.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1110 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/registry.json
+-rw-r--r--   0 runner    (1001) docker     (118)      656 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/related.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1347 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/rule.json
+-rw-r--r--   0 runner    (1001) docker     (118)     5211 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/server.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1341 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/service.json
+-rw-r--r--   0 runner    (1001) docker     (118)     5211 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/source.json
+-rw-r--r--   0 runner    (1001) docker     (118)    73278 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/threat.json
+-rw-r--r--   0 runner    (1001) docker     (118)    11965 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/tls.json
+-rw-r--r--   0 runner    (1001) docker     (118)      724 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/tracing.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1914 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/url.json
+-rw-r--r--   0 runner    (1001) docker     (118)     6976 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/user.json
+-rw-r--r--   0 runner    (1001) docker     (118)     2182 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/user_agent.json
+-rw-r--r--   0 runner    (1001) docker     (118)     1966 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/component_templates/ecs/vulnerability.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.483903 an-website-24.5/an_website/elasticsearch/index_templates/
+-rw-r--r--   0 runner    (1001) docker     (118)      824 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/index_templates/reporting.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.484903 an-website-24.5/an_website/elasticsearch/index_templates/shortener/
+-rw-r--r--   0 runner    (1001) docker     (118)      385 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/index_templates/shortener/shorten.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.484903 an-website-24.5/an_website/elasticsearch/ingest_pipelines/
+-rw-r--r--   0 runner    (1001) docker     (118)      336 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/ingest_pipelines/reporting.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.484903 an-website-24.5/an_website/elasticsearch/ingest_pipelines/shortener/
+-rw-r--r--   0 runner    (1001) docker     (118)      285 2024-05-16 06:02:16.000000 an-website-24.5/an_website/elasticsearch/ingest_pipelines/shortener/shorten.json
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.484903 an-website-24.5/an_website/element_web_link/
+-rw-r--r--   0 runner    (1001) docker     (118)      836 2024-05-16 06:02:16.000000 an-website-24.5/an_website/element_web_link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1243 2024-05-16 06:02:16.000000 an-website-24.5/an_website/element_web_link/element_web_link.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.485903 an-website-24.5/an_website/emoji_chat/
+-rw-r--r--   0 runner    (1001) docker     (118)      816 2024-05-16 06:02:16.000000 an-website-24.5/an_website/emoji_chat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)    12091 2024-05-16 06:02:16.000000 an-website-24.5/an_website/emoji_chat/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.485903 an-website-24.5/an_website/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (118)      837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4254 2024-05-16 06:02:16.000000 an-website-24.5/an_website/endpoints/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.485903 an-website-24.5/an_website/example/
+-rw-r--r--   0 runner    (1001) docker     (118)      812 2024-05-16 06:02:16.000000 an-website-24.5/an_website/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2666 2024-05-16 06:02:16.000000 an-website-24.5/an_website/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4469 2024-05-16 06:02:16.000000 an-website-24.5/an_website/fake_orjson.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.486903 an-website-24.5/an_website/hangman_solver/
+-rw-r--r--   0 runner    (1001) docker     (118)      846 2024-05-16 06:02:16.000000 an-website-24.5/an_website/hangman_solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5079 2024-05-16 06:02:16.000000 an-website-24.5/an_website/hangman_solver/hangman_solver.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3978 2024-05-16 06:02:16.000000 an-website-24.5/an_website/hangman_solver/wordgame_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.486903 an-website-24.5/an_website/host_info/
+-rw-r--r--   0 runner    (1001) docker     (118)      838 2024-05-16 06:02:16.000000 an-website-24.5/an_website/host_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5245 2024-05-16 06:02:16.000000 an-website-24.5/an_website/host_info/host_info.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.486903 an-website-24.5/an_website/js_licenses/
+-rw-r--r--   0 runner    (1001) docker     (118)      860 2024-05-16 06:02:16.000000 an-website-24.5/an_website/js_licenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3513 2024-05-16 06:02:16.000000 an-website-24.5/an_website/js_licenses/js_licenses.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.487903 an-website-24.5/an_website/kangaroo_comics/
+-rw-r--r--   0 runner    (1001) docker     (118)      851 2024-05-16 06:02:16.000000 an-website-24.5/an_website/kangaroo_comics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2421 2024-05-16 06:02:16.000000 an-website-24.5/an_website/kangaroo_comics/comics.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.487903 an-website-24.5/an_website/lolwut/
+-rw-r--r--   0 runner    (1001) docker     (118)      832 2024-05-16 06:02:16.000000 an-website-24.5/an_website/lolwut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3186 2024-05-16 06:02:16.000000 an-website-24.5/an_website/lolwut/lolwut.py
+-rw-r--r--   0 runner    (1001) docker     (118)    42730 2024-05-16 06:02:16.000000 an-website-24.5/an_website/main.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.487903 an-website-24.5/an_website/main_page/
+-rw-r--r--   0 runner    (1001) docker     (118)      833 2024-05-16 06:02:16.000000 an-website-24.5/an_website/main_page/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1801 2024-05-16 06:02:16.000000 an-website-24.5/an_website/main_page/main_page.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.488903 an-website-24.5/an_website/patches/
+-rw-r--r--   0 runner    (1001) docker     (118)    12034 2024-05-16 06:02:16.000000 an-website-24.5/an_website/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1738 2024-05-16 06:02:16.000000 an-website-24.5/an_website/patches/braille.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3944 2024-05-16 06:02:16.000000 an-website-24.5/an_website/patches/json.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.488903 an-website-24.5/an_website/ping/
+-rw-r--r--   0 runner    (1001) docker     (118)      832 2024-05-16 06:02:16.000000 an-website-24.5/an_website/ping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1644 2024-05-16 06:02:16.000000 an-website-24.5/an_website/ping/ping.py
+-rw-r--r--   0 runner    (1001) docker     (118)    62500 2024-05-16 06:02:16.000000 an-website-24.5/an_website/primes.bin
+-rw-r--r--   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:16.000000 an-website-24.5/an_website/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.490903 an-website-24.5/an_website/quotes/
+-rw-r--r--   0 runner    (1001) docker     (118)     6032 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9977 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/create.py
+-rwxr-xr-x   0 runner    (1001) docker     (118)     1437 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/edit.sh
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.490903 an-website-24.5/an_website/quotes/files/
+-rw-r--r--   0 runner    (1001) docker     (118)     5101 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/files/StempelNichtWitzig.png
+-rw-r--r--   0 runner    (1001) docker     (118)     3058 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/files/StempelWitzig.png
+-rw-r--r--   0 runner    (1001) docker     (118)    42308 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/files/bg.png
+-rw-r--r--   0 runner    (1001) docker     (118)    50944 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/files/oswald.regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (118)     2800 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/generator.py
+-rw-r--r--   0 runner    (1001) docker     (118)    12882 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/image.py
+-rw-r--r--   0 runner    (1001) docker     (118)     7514 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/info.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.491903 an-website-24.5/an_website/quotes/quote_of_the_day/
+-rw-r--r--   0 runner    (1001) docker     (118)     5687 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/quote_of_the_day/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2509 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/quote_of_the_day/data.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5544 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/quote_of_the_day/store.py
+-rw-r--r--   0 runner    (1001) docker     (118)    17654 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/quotes.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1574 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/share.py
+-rw-r--r--   0 runner    (1001) docker     (118)    26353 2024-05-16 06:02:16.000000 an-website-24.5/an_website/quotes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.491903 an-website-24.5/an_website/random_text/
+-rw-r--r--   0 runner    (1001) docker     (118)      839 2024-05-16 06:02:16.000000 an-website-24.5/an_website/random_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4126 2024-05-16 06:02:16.000000 an-website-24.5/an_website/random_text/random_text.py
+-rw-r--r--   0 runner    (1001) docker     (118)  3039490 2024-05-16 06:02:16.000000 an-website-24.5/an_website/random_text/words.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.494903 an-website-24.5/an_website/redirect/
+-rw-r--r--   0 runner    (1001) docker     (118)      837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/redirect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2514 2024-05-16 06:02:16.000000 an-website-24.5/an_website/redirect/redirect.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.495903 an-website-24.5/an_website/reporting/
+-rw-r--r--   0 runner    (1001) docker     (118)      837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     8680 2024-05-16 06:02:16.000000 an-website-24.5/an_website/reporting/reporting.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.495903 an-website-24.5/an_website/search/
+-rw-r--r--   0 runner    (1001) docker     (118)      847 2024-05-16 06:02:16.000000 an-website-24.5/an_website/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9733 2024-05-16 06:02:16.000000 an-website-24.5/an_website/search/search.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.495903 an-website-24.5/an_website/services/
+-rw-r--r--   0 runner    (1001) docker     (118)      866 2024-05-16 06:02:16.000000 an-website-24.5/an_website/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3716 2024-05-16 06:02:16.000000 an-website-24.5/an_website/services/services.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.496903 an-website-24.5/an_website/settings/
+-rw-r--r--   0 runner    (1001) docker     (118)      846 2024-05-16 06:02:16.000000 an-website-24.5/an_website/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4739 2024-05-16 06:02:16.000000 an-website-24.5/an_website/settings/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.496903 an-website-24.5/an_website/snow/
+-rw-r--r--   0 runner    (1001) docker     (118)     1111 2024-05-16 06:02:16.000000 an-website-24.5/an_website/snow/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.496903 an-website-24.5/an_website/soundboard/
+-rw-r--r--   0 runner    (1001) docker     (118)     3334 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     7982 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/data.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.506903 an-website-24.5/an_website/soundboard/files/
+-rw-r--r--   0 runner    (1001) docker     (118)    50432 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/dietmar-ich_hab_seine_hausaufgaben_aufgegessen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    70592 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/fw-ihr_linken_intellektuellen_fuzzies.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    43007 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/gott-das_ist_privat.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    81459 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/gott-so_so_du_hast_also_keine_eier.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48858 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/jesus-guck_mal_was_ich_kann.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    53986 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-aber_nicht_zu_lidl.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    74486 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-alles_kapitalismus_alles_nestle_alles_haehnchen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    28211 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-das_ist_freiwillig.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    84635 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-finsterstes_mittelalter_alter.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    46007 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-hallo.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    72923 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-hier_sind_wir_jetzt_unterhalte_uns.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    41997 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-i_love_it.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    49865 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-ich_bin_kommunist.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    59749 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-ich_darf_nich_und_ich_will_nich.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    90810 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-im_so_happy_for_no_reason_but_i_dont_care.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48353 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-ja_ja.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    56648 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-kein_problem_ich_hab_zeit.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    47101 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-koestlich.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   113893 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-man_darf_nie_aufhoeren_alles_kritisch_zu_hinterfragen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48043 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-ohh_hee.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    70477 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-this_kinda_feels_really_really_awesome.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   191215 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-wir_kaempfen_fuer_eine_gerechte_weltordnung_brot_fuer_alle_und_die_aechtung_von_sogennanntem_musikfernsehen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    57217 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-wir_sind_keine_intellektuellen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    51169 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kaenguru-wolln_wir_uns_dutzen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    38466 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/kuh-ahamumumu.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   120162 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-du_bist_also_teil_der_juedisch-bolschewistischen_weltverschwoerung.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    39036 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-fuer_nichts_und_wieder_nichts.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    67629 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-i_am_bored.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   134445 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-i_am_bored_in_the_usa.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    89930 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-im_just_here_for_the_famous_breakfast.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    33069 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-ja_herzlich_willkommen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    39663 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-sprich_bitte_nur_fuer_dich.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   189292 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-ueber_mich_hat_die_zeit_geschrieben_dass_ich_der_wahrscheinlich_einflussreichste_linke_interlektulelle_deutschlands_sei.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   127434 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-und_da_ist_mir_aufgefallen_dass_ich_keine_eier_hab.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    56423 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-und_mich_dann_auch_noch_beschneiden_lassen.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48303 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-von_mir_aus.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    44620 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/muk-yeah.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    25452 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/psychiater-aha.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    43250 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-hey_thats_cool.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    46290 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-i_love_life.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   155900 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-thats_amazing_its_like_you_know_i_dont_know_kind_of_like_whatever_and_stuff.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    61219 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-the_world_is_so_beautiful.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)   138254 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-well_thats_just_like_you_know_amazing.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    68839 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/files/sarah-yes_its_just_perfect.mp3
+-rw-r--r--   0 runner    (1001) docker     (118)    48809 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (118)     5010 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/info.json
+-rw-r--r--   0 runner    (1001) docker     (118)     6481 2024-05-16 06:02:16.000000 an-website-24.5/an_website/soundboard/soundboard.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.507903 an-website-24.5/an_website/static/
+-rw-r--r--   0 runner    (1001) docker     (118)      199 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/.env
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.511903 an-website-24.5/an_website/static/css/
+-rw-r--r--   0 runner    (1001) docker     (118)      144 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/ansi2html.css
+-rw-r--r--   0 runner    (1001) docker     (118)      329 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/ansi2html.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)     5793 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (118)    13928 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/base.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      437 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/comic.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1034 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/comic.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      358 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/emoji_chat.css
+-rw-r--r--   0 runner    (1001) docker     (118)      771 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/emoji_chat.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      210 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/error.css
+-rw-r--r--   0 runner    (1001) docker     (118)      510 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/error.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      750 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/form.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1682 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/form.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      599 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/kangaroo_comics.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1424 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/kangaroo_comics.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      174 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/main_page.css
+-rw-r--r--   0 runner    (1001) docker     (118)      424 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/main_page.css.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.513903 an-website-24.5/an_website/static/css/quotes/
+-rw-r--r--   0 runner    (1001) docker     (118)      480 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/generator.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1043 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/generator.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      549 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/info.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1317 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/info.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)     2205 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/quotes.css
+-rw-r--r--   0 runner    (1001) docker     (118)     4984 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/quotes.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      806 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/share.css
+-rw-r--r--   0 runner    (1001) docker     (118)     2038 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/quotes/share.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      436 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/redirect.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1076 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/redirect.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)    52690 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/snow.css
+-rw-r--r--   0 runner    (1001) docker     (118)    42520 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/snow.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      479 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/soundboard.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1074 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/soundboard.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      492 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/table.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1051 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/table.css.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.516903 an-website-24.5/an_website/static/css/themes/
+-rw-r--r--   0 runner    (1001) docker     (118)      342 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/blue.css
+-rw-r--r--   0 runner    (1001) docker     (118)      779 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/blue.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      786 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/christmas.css
+-rw-r--r--   0 runner    (1001) docker     (118)     1889 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/christmas.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      345 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/default.css
+-rw-r--r--   0 runner    (1001) docker     (118)      782 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/default.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      384 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/fun.css
+-rw-r--r--   0 runner    (1001) docker     (118)      810 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/fun.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      347 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/green.css
+-rw-r--r--   0 runner    (1001) docker     (118)      784 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/green.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      355 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/light.css
+-rw-r--r--   0 runner    (1001) docker     (118)      792 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/light.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      360 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/light_blue.css
+-rw-r--r--   0 runner    (1001) docker     (118)      797 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/light_blue.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      342 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/orange.css
+-rw-r--r--   0 runner    (1001) docker     (118)      779 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/orange.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      341 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/pink.css
+-rw-r--r--   0 runner    (1001) docker     (118)      778 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/pink.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      343 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/purple.css
+-rw-r--r--   0 runner    (1001) docker     (118)      780 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/purple.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      341 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/yellow.css
+-rw-r--r--   0 runner    (1001) docker     (118)      778 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/themes/yellow.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)      250 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/uptime.css
+-rw-r--r--   0 runner    (1001) docker     (118)      599 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/css/uptime.css.map
+-rw-r--r--   0 runner    (1001) docker     (118)     9109 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/favicon.jxl
+-rw-r--r--   0 runner    (1001) docker     (118)    12948 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.517903 an-website-24.5/an_website/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (118)      538 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/fonts/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (118)    33916 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/fonts/comic.woff2
+-rw-r--r--   0 runner    (1001) docker     (118)    12152 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/fonts/comicmono.woff2
+-rw-r--r--   0 runner    (1001) docker     (118)     4120 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/fonts/cursedtimerulil-aznm.woff2
+-rw-r--r--   0 runner    (1001) docker     (118)      377 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/humans.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.520903 an-website-24.5/an_website/static/img/
+-rw-r--r--   0 runner    (1001) docker     (118)  1047428 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/2020-11-03.jpg
+-rw-r--r--   0 runner    (1001) docker     (118)      763 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (118)      258 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      405 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/close.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      467 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/hamburger-menu-icon.svg
+-rw-r--r--   0 runner    (1001) docker     (118)    23613 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/kangarooface.svg
+-rw-r--r--   0 runner    (1001) docker     (118)    24121 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (118)     1444 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/netcup-oekostrom2.jxl
+-rw-r--r--   0 runner    (1001) docker     (118)     2592 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/netcup-oekostrom2.png
+-rw-r--r--   0 runner    (1001) docker     (118)      161 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      197 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/report.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      589 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/rss.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      597 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/save.svg
+-rw-r--r--   0 runner    (1001) docker     (118)      472 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/share.svg
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.520903 an-website-24.5/an_website/static/img/stamps/
+-rw-r--r--   0 runner    (1001) docker     (118)     8849 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/stamps/nichtwitzig.small.svg
+-rw-r--r--   0 runner    (1001) docker     (118)     5797 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/img/stamps/witzig.small.svg
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.468903 an-website-24.5/an_website/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.521903 an-website-24.5/an_website/static/js/currency_converter/
+-rw-r--r--   0 runner    (1001) docker     (118)     2021 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/currency_converter/converter.js
+-rw-r--r--   0 runner    (1001) docker     (118)     8735 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/currency_converter/converter.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.521903 an-website-24.5/an_website/static/js/emoji_chat/
+-rw-r--r--   0 runner    (1001) docker     (118)     3023 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/emoji_chat/chat.js
+-rw-r--r--   0 runner    (1001) docker     (118)    11583 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/emoji_chat/chat.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.521903 an-website-24.5/an_website/static/js/hangman_solver/
+-rw-r--r--   0 runner    (1001) docker     (118)     3978 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/hangman_solver/hangman_solver.js
+-rw-r--r--   0 runner    (1001) docker     (118)    17899 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/hangman_solver/hangman_solver.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.522904 an-website-24.5/an_website/static/js/kangaroo_comics/
+-rw-r--r--   0 runner    (1001) docker     (118)     7855 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/kangaroo_comics/comics.js
+-rw-r--r--   0 runner    (1001) docker     (118)    22718 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/kangaroo_comics/comics.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.522904 an-website-24.5/an_website/static/js/quotes/
+-rw-r--r--   0 runner    (1001) docker     (118)      485 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/quotes/create.js
+-rw-r--r--   0 runner    (1001) docker     (118)     1634 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/quotes/create.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)     3144 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/quotes/quotes.js
+-rw-r--r--   0 runner    (1001) docker     (118)    12154 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/quotes/quotes.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.523903 an-website-24.5/an_website/static/js/search/
+-rw-r--r--   0 runner    (1001) docker     (118)      790 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/search/search.js
+-rw-r--r--   0 runner    (1001) docker     (118)     2600 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/search/search.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.523903 an-website-24.5/an_website/static/js/settings/
+-rw-r--r--   0 runner    (1001) docker     (118)     1440 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/settings/settings.js
+-rw-r--r--   0 runner    (1001) docker     (118)     4676 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/settings/settings.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.523903 an-website-24.5/an_website/static/js/snow/
+-rw-r--r--   0 runner    (1001) docker     (118)     1219 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/snow/snow.js
+-rw-r--r--   0 runner    (1001) docker     (118)     5306 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/snow/snow.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.524903 an-website-24.5/an_website/static/js/swapped_words/
+-rw-r--r--   0 runner    (1001) docker     (118)     1274 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/swapped_words/swap.js
+-rw-r--r--   0 runner    (1001) docker     (118)     4000 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/swapped_words/swap.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.524903 an-website-24.5/an_website/static/js/uptime/
+-rw-r--r--   0 runner    (1001) docker     (118)      585 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/uptime/uptime.js
+-rw-r--r--   0 runner    (1001) docker     (118)     2236 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/uptime/uptime.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.525903 an-website-24.5/an_website/static/js/utils/
+-rw-r--r--   0 runner    (1001) docker     (118)     1165 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/better_ui.js
+-rw-r--r--   0 runner    (1001) docker     (118)     3610 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/better_ui.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)     2923 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/dynload.js
+-rw-r--r--   0 runner    (1001) docker     (118)    10506 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/dynload.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)     1995 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/utils.js
+-rw-r--r--   0 runner    (1001) docker     (118)     6498 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/utils/utils.js.map
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.525903 an-website-24.5/an_website/static/js/vendored/
+-rw-r--r--   0 runner    (1001) docker     (118)    95822 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/vendored/vanilla.js
+-rw-r--r--   0 runner    (1001) docker     (118)   534836 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/js/vendored/vanilla.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)      354 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (118)       77 2024-05-16 06:02:16.000000 an-website-24.5/an_website/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.526903 an-website-24.5/an_website/swapped_words/
+-rw-r--r--   0 runner    (1001) docker     (118)     1794 2024-05-16 06:02:16.000000 an-website-24.5/an_website/swapped_words/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)      926 2024-05-16 06:02:16.000000 an-website-24.5/an_website/swapped_words/config.sw
+-rw-r--r--   0 runner    (1001) docker     (118)    12837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/swapped_words/config_file.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6238 2024-05-16 06:02:16.000000 an-website-24.5/an_website/swapped_words/swap.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.527903 an-website-24.5/an_website/templates/
+-rw-r--r--   0 runner    (1001) docker     (118)      559 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/ansi2html.html
+-rw-r--r--   0 runner    (1001) docker     (118)     3650 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (118)      557 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/error.html
+-rw-r--r--   0 runner    (1001) docker     (118)     4964 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (118)     3004 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/header.html
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.530903 an-website-24.5/an_website/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (118)      392 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/EXAMPLE.html
+-rw-r--r--   0 runner    (1001) docker     (118)      985 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/contact.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1854 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/converter.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1130 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/emoji_chat.html
+-rw-r--r--   0 runner    (1001) docker     (118)       70 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/empty.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1128 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/endpoints.html
+-rw-r--r--   0 runner    (1001) docker     (118)     3405 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/hangman_solver.html
+-rw-r--r--   0 runner    (1001) docker     (118)      116 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/ip.html
+-rw-r--r--   0 runner    (1001) docker     (118)      804 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/js_licenses.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1064 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/kangaroo_comics.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1973 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/main_page.html
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.532904 an-website-24.5/an_website/templates/pages/quotes/
+-rw-r--r--   0 runner    (1001) docker     (118)      343 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/author_info.html
+-rw-r--r--   0 runner    (1001) docker     (118)     2210 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/create1.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1843 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/create2.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1349 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/generator.html
+-rw-r--r--   0 runner    (1001) docker     (118)     2284 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/info.html
+-rw-r--r--   0 runner    (1001) docker     (118)     2960 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/main_page.html
+-rw-r--r--   0 runner    (1001) docker     (118)      196 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/quote_info.html
+-rw-r--r--   0 runner    (1001) docker     (118)     7157 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/quotes.html
+-rw-r--r--   0 runner    (1001) docker     (118)     6779 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/quotes/share.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1183 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/redirect.html
+-rw-r--r--   0 runner    (1001) docker     (118)      990 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/search.html
+-rw-r--r--   0 runner    (1001) docker     (118)      968 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/services.html
+-rw-r--r--   0 runner    (1001) docker     (118)     4530 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/settings.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1057 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/soundboard.html
+-rw-r--r--   0 runner    (1001) docker     (118)     1843 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/swapped_words.html
+-rw-r--r--   0 runner    (1001) docker     (118)      841 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/troet.html
+-rw-r--r--   0 runner    (1001) docker     (118)      930 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/uptime.html
+-rw-r--r--   0 runner    (1001) docker     (118)      847 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/version.html
+-rw-r--r--   0 runner    (1001) docker     (118)      964 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/pages/wordgame_solver.html
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.532904 an-website-24.5/an_website/templates/rss/
+-rw-r--r--   0 runner    (1001) docker     (118)     1108 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/rss/quote_of_the_day.xml
+-rw-r--r--   0 runner    (1001) docker     (118)      495 2024-05-16 06:02:16.000000 an-website-24.5/an_website/templates/rss/soundboard.xml
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.532904 an-website-24.5/an_website/troet/
+-rw-r--r--   0 runner    (1001) docker     (118)      833 2024-05-16 06:02:16.000000 an-website-24.5/an_website/troet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2761 2024-05-16 06:02:16.000000 an-website-24.5/an_website/troet/troet.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.533903 an-website-24.5/an_website/update/
+-rw-r--r--   0 runner    (1001) docker     (118)      837 2024-05-16 06:02:16.000000 an-website-24.5/an_website/update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4490 2024-05-16 06:02:16.000000 an-website-24.5/an_website/update/update.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.533903 an-website-24.5/an_website/uptime/
+-rw-r--r--   0 runner    (1001) docker     (118)      863 2024-05-16 06:02:16.000000 an-website-24.5/an_website/uptime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6967 2024-05-16 06:02:16.000000 an-website-24.5/an_website/uptime/uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.535904 an-website-24.5/an_website/utils/
+-rw-r--r--   0 runner    (1001) docker     (118)     1679 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)    40385 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/base_request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9147 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/better_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6771 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/data_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (118)     7845 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4964 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (118)     8104 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (118)     9034 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4751 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/search.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6982 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/static_file_from_traversable.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6753 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/static_file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5326 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/token.py
+-rw-r--r--   0 runner    (1001) docker     (118)    25599 2024-05-16 06:02:16.000000 an-website-24.5/an_website/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.536903 an-website-24.5/an_website/vendored/
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.537903 an-website-24.5/an_website/vendored/apm-rum/
+-rw-r--r--   0 runner    (1001) docker     (118)   579743 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.js
+-rw-r--r--   0 runner    (1001) docker     (118)    61332 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js
+-rw-r--r--   0 runner    (1001) docker     (118)   263069 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js.map
+-rw-r--r--   0 runner    (1001) docker     (118)    56683 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/media-types.json
+-rw-r--r--   0 runner    (1001) docker     (118)   205599 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/mime-db.json
+-rwxr-xr-x   0 runner    (1001) docker     (118)   255236 2024-05-16 06:02:16.000000 an-website-24.5/an_website/vendored/screenfetch
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.538904 an-website-24.5/an_website/version/
+-rw-r--r--   0 runner    (1001) docker     (118)      836 2024-05-16 06:02:16.000000 an-website-24.5/an_website/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3862 2024-05-16 06:02:16.000000 an-website-24.5/an_website/version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.538904 an-website-24.5/an_website/whats_my_ip/
+-rw-r--r--   0 runner    (1001) docker     (118)      845 2024-05-16 06:02:17.000000 an-website-24.5/an_website/whats_my_ip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2496 2024-05-16 06:02:17.000000 an-website-24.5/an_website/whats_my_ip/ip.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.538904 an-website-24.5/an_website/wiki/
+-rw-r--r--   0 runner    (1001) docker     (118)      848 2024-05-16 06:02:17.000000 an-website-24.5/an_website/wiki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1883 2024-05-16 06:02:17.000000 an-website-24.5/an_website/wiki/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.542904 an-website-24.5/an_website.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (118)     8194 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (118)    16466 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (118)        1 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (118)      109 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (118)        1 2024-05-16 06:02:23.000000 an-website-24.5/an_website.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (118)     1861 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (118)       11 2024-05-16 06:02:26.000000 an-website-24.5/an_website.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (118)     1750 2024-05-16 06:02:17.000000 an-website-24.5/build-oci-image.sh
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.539903 an-website-24.5/example-configurations/
+-rw-r--r--   0 runner    (1001) docker     (118)     1528 2024-05-16 06:02:17.000000 an-website-24.5/example-configurations/config.ini.default
+-rw-r--r--   0 runner    (1001) docker     (118)     2328 2024-05-16 06:02:17.000000 an-website-24.5/example-configurations/config.ini.example
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.539903 an-website-24.5/example-configurations/nginx/
+-rw-r--r--   0 runner    (1001) docker     (118)     1874 2024-05-16 06:02:17.000000 an-website-24.5/example-configurations/nginx/an-website.conf
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.539903 an-website-24.5/example-configurations/supervisord/
+-rw-r--r--   0 runner    (1001) docker     (118)      200 2024-05-16 06:02:17.000000 an-website-24.5/example-configurations/supervisord/an_website.ini
+-rw-r--r--   0 runner    (1001) docker     (118)     3034 2024-05-16 06:02:17.000000 an-website-24.5/pip-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (118)     1032 2024-05-16 06:02:17.000000 an-website-24.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (118)       38 2024-05-16 06:02:26.543903 an-website-24.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (118)     3602 2024-05-16 06:02:17.000000 an-website-24.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (118)        0 2024-05-16 06:02:26.541903 an-website-24.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (118)     8267 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_backdoor.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1226 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_christmas.py
+-rw-r--r--   0 runner    (1001) docker     (118)     4847 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_commitment.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3517 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_contact.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2402 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_currency_converter.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3476 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_hangman_solver.py
+-rw-r--r--   0 runner    (1001) docker     (118)     6783 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5772 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (118)    13039 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1666 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_random_text.py
+-rw-r--r--   0 runner    (1001) docker     (118)    18637 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_request_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5374 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (118)    11416 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_swapped_words.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2557 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (118)     3402 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_traversable_static_file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (118)     2769 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_troet.py
+-rw-r--r--   0 runner    (1001) docker     (118)     1956 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_uptime.py
+-rw-r--r--   0 runner    (1001) docker     (118)     5609 2024-05-16 06:02:17.000000 an-website-24.5/tests/test_utils.py
```

### Comparing `an-website-24.4/Containerfile` & `an-website-24.5/Containerfile`

 * *Files identical despite different names*

### Comparing `an-website-24.4/LICENSE.md` & `an-website-24.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `an-website-24.4/PKG-INFO` & `an-website-24.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: an-website
-Version: 24.4
+Version: 24.5
 Summary: #1 Website in the Worlds
 Home-page: https://github.com/asozialesnetzwerk/an-website
 Author: Das Asoziale Netzwerk
 Author-email: contact@asozial.org
 License: AGPL-3.0-or-later
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,70 +15,70 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: accept-types==0.4.1
 Requires-Dist: aiodns==3.2.0
-Requires-Dist: aiohttp[speedups]==3.9.3; python_version >= "3.8"
+Requires-Dist: aiohttp[speedups]==3.9.5; python_version >= "3.8"
 Requires-Dist: aiosignal==1.3.1; python_version >= "3.7"
 Requires-Dist: ansi2html==1.9.1; python_version >= "3.7"
 Requires-Dist: async-timeout==4.0.3; python_full_version < "3.11.3"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: beautifulsoup4==4.12.3; python_full_version >= "3.6.0"
 Requires-Dist: blake3==0.4.1
 Requires-Dist: brotli==1.1.0
 Requires-Dist: certifi==2023.11.17; python_version >= "3.6"
 Requires-Dist: cffi==1.16.0; python_version >= "3.8"
 Requires-Dist: defity==0.3.1; python_version >= "3.7"
 Requires-Dist: defusedxml==0.7.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
 Requires-Dist: dill==0.3.8; python_version >= "3.8"
-Requires-Dist: dunamai==1.19.2; python_version >= "3.5"
+Requires-Dist: dunamai==1.21.1; python_version >= "3.5"
 Requires-Dist: ecs-logging==2.1.0; python_version >= "3.6"
-Requires-Dist: elastic-apm==6.21.4.post8347027212; python_version >= "3.6" and python_version < "4"
+Requires-Dist: elastic-apm==6.22.0; python_version >= "3.6" and python_version < "4"
 Requires-Dist: elastic-enterprise-search==8.11.0; python_version >= "3.6"
 Requires-Dist: elastic-transport==8.13.0; python_version >= "3.7"
 Requires-Dist: elasticsearch[async]==8.12.1; python_version >= "3.7"
-Requires-Dist: emoji==2.11.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
+Requires-Dist: emoji==2.11.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: frozenlist==1.4.1; python_version >= "3.8"
 Requires-Dist: funcparserlib==1.0.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6" and python_version < "3.13"
 Requires-Dist: get-version==3.5.5; python_version >= "3.9"
 Requires-Dist: hangman-solver-rs==0.2.1; python_version >= "3.10"
 Requires-Dist: hiredis==2.3.2
 Requires-Dist: html2text==2020.1.16; python_version >= "3.5"
 Requires-Dist: hy==0.28.0; python_version < "3.13" and python_version >= "3.8"
 Requires-Dist: hyrule==0.5.0; python_version < "3.13"
-Requires-Dist: idna==3.6; python_version >= "3.5"
-Requires-Dist: jsonpickle==3.0.3; python_version >= "3.7"
-Requires-Dist: lxml==5.2.0; python_version >= "3.6"
+Requires-Dist: idna==3.7; python_version >= "3.5"
+Requires-Dist: jsonpickle==3.0.4; python_version >= "3.7"
+Requires-Dist: lxml==5.2.2; python_version >= "3.6"
 Requires-Dist: multidict==6.0.5; python_version >= "3.7"
 Requires-Dist: openmoji-dist==15.0.0.1
-Requires-Dist: orjson==3.10.0; python_version >= "3.8"
+Requires-Dist: orjson==3.10.3; python_version >= "3.8"
 Requires-Dist: packaging==23.2; python_version >= "3.7"
-Requires-Dist: pillow==10.2.0; python_version >= "3.8"
-Requires-Dist: pillow-jxl-plugin==1.2.2; python_version >= "3.8"
+Requires-Dist: pillow==10.3.0; python_version >= "3.8"
+Requires-Dist: pillow-jxl-plugin==1.2.4; python_version >= "3.8"
 Requires-Dist: pycares==4.4.0; python_version >= "3.8"
 Requires-Dist: pycparser==2.22; python_version >= "3.8"
 Requires-Dist: pycryptodome==3.20.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
 Requires-Dist: pycurl==7.45.2; python_version >= "3.5"
 Requires-Dist: pyjwt==2.8.0; python_version >= "3.7"
 Requires-Dist: pysocks==1.7.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-dateutil==2.9.0.post0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-geoip-geolite2-yplan==2019.1224
 Requires-Dist: python-geoip-yplan==1.2
 Requires-Dist: pytz==2023.4
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
-Requires-Dist: rapidfuzz==3.7.0; python_version >= "3.8"
-Requires-Dist: redis[hiredis]==5.0.3; python_version >= "3.7"
+Requires-Dist: rapidfuzz==3.9.0; python_version >= "3.8"
+Requires-Dist: redis[hiredis]==5.0.4; python_version >= "3.7"
 Requires-Dist: regex==2023.12.25; python_version >= "3.7"
 Requires-Dist: setproctitle==1.3.3; python_version >= "3.7"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: soupsieve==2.5; python_version >= "3.8"
 Requires-Dist: tornado==6.4; python_version >= "3.8"
-Requires-Dist: typed-stream==0.69.0; python_version >= "3.10"
+Requires-Dist: typed-stream==0.131.0; python_version >= "3.10"
 Requires-Dist: tzdata==2023.4; python_version >= "2"
 Requires-Dist: ultradict==0.0.6; python_version >= "3.8"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: uvloop==0.19.0; python_full_version >= "3.8.0"
 Requires-Dist: wrapt==1.14.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
 Requires-Dist: yarl==1.9.4; python_version >= "3.7"
```

### Comparing `an-website-24.4/README.md` & `an-website-24.5/README.md`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/__init__.py` & `an-website-24.5/an_website/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/__main__.py` & `an-website-24.5/an_website/__main__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/backdoor/__init__.py` & `an-website-24.5/an_website/backdoor/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/backdoor/backdoor.py` & `an-website-24.5/an_website/backdoor/backdoor.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/backdoor/client.py` & `an-website-24.5/an_website/backdoor/client.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/ca-bundle.crt` & `an-website-24.5/an_website/ca-bundle.crt`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/commitment/__init__.py` & `an-website-24.5/an_website/commitment/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/commitment/commitment.py` & `an-website-24.5/an_website/commitment/commitment.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/contact/__init__.py` & `an-website-24.5/an_website/contact/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/contact/contact.py` & `an-website-24.5/an_website/contact/contact.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/currency_converter/__init__.py` & `an-website-24.5/an_website/currency_converter/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/currency_converter/converter.py` & `an-website-24.5/an_website/currency_converter/converter.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/discord/__init__.py` & `an-website-24.5/an_website/discord/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/discord/discord.py` & `an-website-24.5/an_website/discord/discord.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/LICENSE.txt` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/NOTICE.txt` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/agent.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/agent.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/client.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/client.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/cloud.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/cloud.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/container.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/container.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/data_stream.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/data_stream.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/destination.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/destination.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/dll.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/dll.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/dns.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/dns.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/email.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/email.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/error.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/error.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/event.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/event.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/file.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/file.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/group.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/group.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/host.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/host.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/http.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/http.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/log.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/log.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/network.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/network.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/observer.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/observer.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/orchestrator.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/orchestrator.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/organization.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/organization.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/package.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/package.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/process.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/process.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/registry.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/registry.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/related.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/related.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/rule.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/rule.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/server.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/server.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/service.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/service.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/source.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/source.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/threat.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/threat.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/tls.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/tls.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/tracing.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/tracing.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/url.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/url.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/user.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/user.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/user_agent.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/user_agent.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/component_templates/ecs/vulnerability.json` & `an-website-24.5/an_website/elasticsearch/component_templates/ecs/vulnerability.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/elasticsearch/index_templates/reporting.json` & `an-website-24.5/an_website/elasticsearch/index_templates/reporting.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/element_web_link/__init__.py` & `an-website-24.5/an_website/element_web_link/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/element_web_link/element_web_link.py` & `an-website-24.5/an_website/element_web_link/element_web_link.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/emoji_chat/__init__.py` & `an-website-24.5/an_website/emoji_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/emoji_chat/chat.py` & `an-website-24.5/an_website/emoji_chat/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import random
 import sys
 import time
 from collections.abc import Awaitable, Iterable, Mapping
 from typing import Any, Final, Literal
 
 import orjson as json
-from emoji import (  # type: ignore[attr-defined]
+from emoji import (
     EMOJI_DATA,
     demojize,
     emoji_list,
     emojize,
     purely_emoji,
 )
 from redis.asyncio import Redis
```

### Comparing `an-website-24.4/an_website/endpoints/__init__.py` & `an-website-24.5/an_website/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/endpoints/endpoints.py` & `an-website-24.5/an_website/endpoints/endpoints.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/example/__init__.py` & `an-website-24.5/an_website/example/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/example/example.py` & `an-website-24.5/an_website/example/example.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/fake_orjson.py` & `an-website-24.5/an_website/fake_orjson.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/hangman_solver/__init__.py` & `an-website-24.5/an_website/hangman_solver/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/hangman_solver/hangman_solver.py` & `an-website-24.5/an_website/hangman_solver/hangman_solver.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/hangman_solver/wordgame_solver.py` & `an-website-24.5/an_website/hangman_solver/wordgame_solver.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/host_info/__init__.py` & `an-website-24.5/an_website/host_info/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/host_info/host_info.py` & `an-website-24.5/an_website/host_info/host_info.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/js_licenses/__init__.py` & `an-website-24.5/an_website/js_licenses/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/js_licenses/js_licenses.py` & `an-website-24.5/an_website/js_licenses/js_licenses.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/kangaroo_comics/__init__.py` & `an-website-24.5/an_website/kangaroo_comics/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/kangaroo_comics/comics.py` & `an-website-24.5/an_website/kangaroo_comics/comics.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/lolwut/__init__.py` & `an-website-24.5/an_website/lolwut/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/lolwut/lolwut.py` & `an-website-24.5/an_website/lolwut/lolwut.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/main.py` & `an-website-24.5/an_website/main.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/main_page/__init__.py` & `an-website-24.5/an_website/main_page/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/main_page/main_page.py` & `an-website-24.5/an_website/main_page/main_page.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/patches/__init__.py` & `an-website-24.5/an_website/patches/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,26 +255,26 @@
 def patch_tornado_gzip() -> None:
     """Use gzip for more content types."""
     GZipContentEncoding.CONTENT_TYPES = {
         type for type, data in MEDIA_TYPES.items() if data.get("compressible")
     }
 
 
-def patch_tornado_httpclient() -> None:
+def patch_tornado_httpclient() -> None:  # fmt: off
     """Make requests quick."""
     BACON = 0x75800  # noqa: N806  # pylint: disable=invalid-name
     EGGS = 1 << 25  # noqa: N806  # pylint: disable=invalid-name
 
     AsyncHTTPClient.configure("tornado.curl_httpclient.CurlAsyncHTTPClient")
 
     def prepare_curl_callback(self: HTTPRequest, curl: pycurl.Curl) -> None:
         # pylint: disable=c-extension-no-member, useless-suppression
         if urlsplit(self.url).scheme == "https":  # noqa: SIM102
             if (ver := pycurl.version_info())[2] >= BACON and ver[4] & EGGS:
-                curl.setopt(pycurl.HTTP_VERSION, pycurl.CURL_HTTP_VERSION_3)
+                curl.setopt(pycurl.HTTP_VERSION, pycurl.CURL_HTTP_VERSION_3)  # type: ignore[attr-defined]  # noqa: B950
 
     original_request_init = HTTPRequest.__init__
 
     def request_init(self: HTTPRequest, *args: Any, **kwargs: Any) -> None:
         if len(args) < 18:  # there are too many positional arguments here
             prepare_curl_method = MethodType(prepare_curl_callback, self)
             kwargs.setdefault("prepare_curl_callback", prepare_curl_method)
```

### Comparing `an-website-24.4/an_website/patches/braille.py` & `an-website-24.5/an_website/patches/braille.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/patches/json.py` & `an-website-24.5/an_website/patches/json.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/ping/__init__.py` & `an-website-24.5/an_website/ping/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/ping/ping.py` & `an-website-24.5/an_website/ping/ping.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/primes.bin` & `an-website-24.5/an_website/primes.bin`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/__init__.py` & `an-website-24.5/an_website/quotes/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/create.py` & `an-website-24.5/an_website/quotes/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,29 +48,33 @@
         await make_api_request(
             "quotes",
             method="POST",
             body={
                 "author": str(author.id),
                 "quote": quote_str,
             },
+            entity_should_exist=False,
         )
     )
 
 
 async def create_author(author_str: str) -> Author:
     """Create an author."""
     author_str = fix_author_name(author_str)
 
     author = get_author_by_name(author_str)
     if author is not None:
         return author
 
     return parse_author(
         await make_api_request(
-            "authors", method="POST", body={"author": author_str}
+            "authors",
+            method="POST",
+            body={"author": author_str},
+            entity_should_exist=False,
         )
     )
 
 
 async def create_wrong_quote(
     real_author_param: Author | str,
     fake_author_param: Author | str,
```

### Comparing `an-website-24.4/an_website/quotes/edit.sh` & `an-website-24.5/an_website/quotes/edit.sh`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/files/StempelNichtWitzig.png` & `an-website-24.5/an_website/quotes/files/StempelNichtWitzig.png`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/files/StempelWitzig.png` & `an-website-24.5/an_website/quotes/files/StempelWitzig.png`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/files/bg.png` & `an-website-24.5/an_website/quotes/files/bg.png`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/files/oswald.regular.ttf` & `an-website-24.5/an_website/quotes/files/oswald.regular.ttf`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/generator.py` & `an-website-24.5/an_website/quotes/generator.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/image.py` & `an-website-24.5/an_website/quotes/image.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/info.py` & `an-website-24.5/an_website/quotes/info.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/quote_of_the_day/__init__.py` & `an-website-24.5/an_website/quotes/quote_of_the_day/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/quote_of_the_day/data.py` & `an-website-24.5/an_website/quotes/quote_of_the_day/data.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/quote_of_the_day/store.py` & `an-website-24.5/an_website/quotes/quote_of_the_day/store.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/quotes.py` & `an-website-24.5/an_website/quotes/quotes.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/share.py` & `an-website-24.5/an_website/quotes/share.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/quotes/utils.py` & `an-website-24.5/an_website/quotes/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,15 +100,19 @@
             emojify(self.name.strip())
             if (now := datetime.now(timezone.utc)).day == 1 and now.month == 4
             else self.name.strip()
         )
 
     async def fetch_new_data(self) -> Author:
         """Fetch new data from the API."""
-        return parse_author(await make_api_request(f"authors/{self.id}"))
+        return parse_author(
+            await make_api_request(
+                f"authors/{self.id}", entity_should_exist=True
+            )
+        )
 
     def get_path(self) -> str:
         """Return the path to the author info."""
         return f"/zitate/info/a/{self.id}"
 
     def to_json(self) -> dict[str, Any]:
         """Get the author as JSON."""
@@ -149,15 +153,20 @@
             emojify(self.quote.strip())
             if (now := datetime.now(timezone.utc)).day == 1 and now.month == 4
             else self.quote.strip()
         )
 
     async def fetch_new_data(self) -> Quote:
         """Fetch new data from the API."""
-        return parse_quote(await make_api_request(f"quotes/{self.id}"), self)
+        return parse_quote(
+            await make_api_request(
+                f"quotes/{self.id}", entity_should_exist=True
+            ),
+            self,
+        )
 
     def get_path(self) -> str:
         """Return the path to the quote info."""
         return f"/zitate/info/z/{self.id}"
 
     def to_json(self) -> dict[str, Any]:
         """Get the quote as JSON."""
@@ -201,19 +210,22 @@
             api_data = await make_api_request(
                 "wrongquotes",
                 {
                     "quote": str(self.quote.id),
                     "simulate": "true",
                     "author": str(self.author.id),
                 },
+                entity_should_exist=True,
             )
             if api_data:
                 api_data = api_data[0]
         else:
-            api_data = await make_api_request(f"wrongquotes/{self.id}")
+            api_data = await make_api_request(
+                f"wrongquotes/{self.id}", entity_should_exist=True
+            )
         if not api_data:
             return self
         return parse_wrong_quote(api_data, self)
 
     def get_id(self) -> tuple[int, int]:
         """
         Get the id of the quote and the author in a tuple.
@@ -264,14 +276,15 @@
         #     return self
         # do the voting
         return parse_wrong_quote(
             await make_api_request(
                 f"wrongquotes/{self.id}",
                 method="POST",
                 body={"vote": str(vote)},
+                entity_should_exist=True,
             ),
             self,
         )
 
 
 def get_wrong_quotes(
     filter_fun: None | Callable[[WrongQuote], bool] = None,
@@ -326,14 +339,15 @@
     return list(authors)
 
 
 async def make_api_request(
     endpoint: str,
     args: Mapping[str, str] | None = None,
     *,
+    entity_should_exist: bool,
     method: Literal["GET", "POST"] = "GET",
     body: None | Mapping[str, str] = None,
 ) -> Any:  # TODO: list[dict[str, Any]] | dict[str, Any]:
     """Make API request and return the result as dict."""
     if pytest_is_running():
         return None
     query = f"?{urlencode(args)}" if args else ""
@@ -344,28 +358,30 @@
         method=method,
         headers={"Content-Type": "application/x-www-form-urlencoded"},
         body=body_str,
         raise_error=False,
         ca_certs=os.path.join(ROOT_DIR, "ca-bundle.crt"),
     )
     if response.code != 200:
-        LOGGER.warning(
+        normed_response_code = (
+            400
+            if not entity_should_exist and response.code == 500
+            else response.code
+        )
+        LOGGER.log(
+            logging.ERROR if normed_response_code >= 500 else logging.WARNING,
             "%s request to %r with body=%r failed with code=%d and reason=%r",
             method,
             url,
             body_str,
             response.code,
             response.reason,
         )
         raise HTTPError(
-            (
-                400
-                if response.code == 500
-                else (404 if response.code == 404 else 503)
-            ),
+            normed_response_code if normed_response_code in {400, 404} else 503,
             reason=(
                 f"{API_URL}/{endpoint} returned: "
                 f"{response.code} {response.reason}"
             ),
         )
     return json.loads(response.body)
 
@@ -384,16 +400,16 @@
     if not name:
         name = "None"
 
     author = AUTHORS_CACHE.get(author_id)
     if author is None:  # author not in cache, create new one
         # pylint: disable=too-many-function-args
         author = Author(author_id, name, None)
-        MAX_AUTHORS_ID.value = max(  # type: ignore[attr-defined]
-            MAX_AUTHORS_ID.value, author_id  # type: ignore[attr-defined]
+        MAX_AUTHORS_ID.value = max(
+            MAX_AUTHORS_ID.value, author_id
         )
     else:  # update to make sure cache is correct
         author.update_name(name)
 
     AUTHORS_CACHE[author.id] = author
 
     return author
@@ -426,16 +442,16 @@
     quote_str = fix_quote_str(json_data["quote"])
 
     if quote is None:  # no quote supplied, try getting it from cache
         quote = QUOTES_CACHE.get(quote_id)
     if quote is None:  # new quote
         # pylint: disable=too-many-function-args
         quote = Quote(quote_id, quote_str, author)
-        MAX_QUOTES_ID.value = max(  # type: ignore[attr-defined]
-            MAX_QUOTES_ID.value, quote.id  # type: ignore[attr-defined]
+        MAX_QUOTES_ID.value = max(
+            MAX_QUOTES_ID.value, quote.id
         )
     else:  # quote was already saved
         quote.update_quote(quote_str, author.id, author.name)
 
     QUOTES_CACHE[quote.id] = quote
 
     return quote
@@ -576,39 +592,45 @@
     LOGGER.info("Updating quotes cache")
     redis: Redis[str] = cast("Redis[str]", app.settings.get("REDIS"))
     prefix: str = app.settings.get("REDIS_PREFIX", NAME).removesuffix("-dev")
     redis_available = EVENT_REDIS.is_set()
 
     if update_wrong_quotes:
         await parse_list_of_quote_data(
-            wq_data := await make_api_request("wrongquotes"),
+            wq_data := await make_api_request(
+                "wrongquotes", entity_should_exist=True
+            ),
             parse_wrong_quote,
         )
         if wq_data and redis_available:
             await redis.setex(
                 f"{prefix}:cached-quote-data:wrongquotes",
                 60 * 60 * 24 * 30,
                 json.dumps(wq_data, option=ORJSON_OPTIONS),
             )
 
     if update_quotes:
         await parse_list_of_quote_data(
-            quotes_data := await make_api_request("quotes"),
+            quotes_data := await make_api_request(
+                "quotes", entity_should_exist=True
+            ),
             parse_quote,
         )
         if quotes_data and redis_available:
             await redis.setex(
                 f"{prefix}:cached-quote-data:quotes",
                 60 * 60 * 24 * 30,
                 json.dumps(quotes_data, option=ORJSON_OPTIONS),
             )
 
     if update_authors:
         await parse_list_of_quote_data(
-            authors_data := await make_api_request("authors"),
+            authors_data := await make_api_request(
+                "authors", entity_should_exist=True
+            ),
             parse_author,
         )
         if authors_data and redis_available:
             await redis.setex(
                 f"{prefix}:cached-quote-data:authors",
                 60 * 60 * 24 * 30,
                 json.dumps(authors_data, option=ORJSON_OPTIONS),
@@ -628,23 +650,29 @@
 
 
 async def get_author_by_id(author_id: int) -> Author:
     """Get an author by its id."""
     author = AUTHORS_CACHE.get(author_id)
     if author is not None:
         return author
-    return parse_author(await make_api_request(f"authors/{author_id}"))
+    return parse_author(
+        await make_api_request(
+            f"authors/{author_id}", entity_should_exist=False
+        )
+    )
 
 
 async def get_quote_by_id(quote_id: int) -> Quote:
     """Get a quote by its id."""
     quote = QUOTES_CACHE.get(quote_id)
     if quote is not None:
         return quote
-    return parse_quote(await make_api_request(f"quotes/{quote_id}"))
+    return parse_quote(
+        await make_api_request(f"quotes/{quote_id}", entity_should_exist=False)
+    )
 
 
 async def get_wrong_quote(
     quote_id: int, author_id: int, use_cache: bool = True
 ) -> WrongQuote:
     """Get a wrong quote with a quote id and an author id."""
     wrong_quote = WRONG_QUOTES_CACHE.get((quote_id, author_id))
@@ -667,14 +695,15 @@
     result = await make_api_request(
         "wrongquotes",
         {
             "quote": str(quote_id),
             "simulate": "true",
             "author": str(author_id),
         },
+        entity_should_exist=False,
     )
     if result:
         return parse_wrong_quote(result[0])
 
     raise HTTPError(404, reason="Falsches Zitat nicht gefunden")
 
 
@@ -682,22 +711,22 @@
     """Get the rating of a wrong quote."""
     return (await get_wrong_quote(quote_id, author_id)).rating
 
 
 def get_random_quote_id() -> int:
     """Get random quote id."""
     return random.randint(  # nosec: B311
-        1, MAX_QUOTES_ID.value  # type: ignore[attr-defined]
+        1, MAX_QUOTES_ID.value
     )
 
 
 def get_random_author_id() -> int:
     """Get random author id."""
     return random.randint(  # nosec: B311
-        1, MAX_AUTHORS_ID.value  # type: ignore[attr-defined]
+        1, MAX_AUTHORS_ID.value
     )
 
 
 def get_random_id() -> tuple[int, int]:
     """Get random wrong quote id."""
     return (
         get_random_quote_id(),
@@ -726,14 +755,15 @@
             "wrongquotes",
             method="POST",
             body={
                 "quote": str(quote_id),
                 "author": str(author_id),
                 "contributed_by": contributed_by,
             },
+            entity_should_exist=False,
         )
     )
     return await wrong_quote.vote(vote, lazy=True)
 
 
 class QuoteReadyCheckHandler(HTMLRequestHandler):
     """Class that checks if quotes have been loaded."""
```

### Comparing `an-website-24.4/an_website/random_text/__init__.py` & `an-website-24.5/an_website/random_text/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/random_text/random_text.py` & `an-website-24.5/an_website/random_text/random_text.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/random_text/words.txt` & `an-website-24.5/an_website/random_text/words.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/redirect/__init__.py` & `an-website-24.5/an_website/redirect/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/redirect/redirect.py` & `an-website-24.5/an_website/redirect/redirect.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/reporting/__init__.py` & `an-website-24.5/an_website/reporting/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/reporting/reporting.py` & `an-website-24.5/an_website/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/search/__init__.py` & `an-website-24.5/an_website/search/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/search/search.py` & `an-website-24.5/an_website/search/search.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/services/__init__.py` & `an-website-24.5/an_website/services/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/services/services.py` & `an-website-24.5/an_website/services/services.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/settings/__init__.py` & `an-website-24.5/an_website/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/settings/settings.py` & `an-website-24.5/an_website/settings/settings.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/snow/LICENSE` & `an-website-24.5/an_website/snow/LICENSE`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/__init__.py` & `an-website-24.5/an_website/soundboard/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/data.py` & `an-website-24.5/an_website/soundboard/data.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/dietmar-ich_hab_seine_hausaufgaben_aufgegessen.mp3` & `an-website-24.5/an_website/soundboard/files/dietmar-ich_hab_seine_hausaufgaben_aufgegessen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/fw-ihr_linken_intellektuellen_fuzzies.mp3` & `an-website-24.5/an_website/soundboard/files/fw-ihr_linken_intellektuellen_fuzzies.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/gott-das_ist_privat.mp3` & `an-website-24.5/an_website/soundboard/files/gott-das_ist_privat.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/gott-so_so_du_hast_also_keine_eier.mp3` & `an-website-24.5/an_website/soundboard/files/gott-so_so_du_hast_also_keine_eier.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/jesus-guck_mal_was_ich_kann.mp3` & `an-website-24.5/an_website/soundboard/files/jesus-guck_mal_was_ich_kann.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-aber_nicht_zu_lidl.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-aber_nicht_zu_lidl.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-alles_kapitalismus_alles_nestle_alles_haehnchen.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-alles_kapitalismus_alles_nestle_alles_haehnchen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-das_ist_freiwillig.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-das_ist_freiwillig.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-finsterstes_mittelalter_alter.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-finsterstes_mittelalter_alter.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-hallo.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-hallo.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-hier_sind_wir_jetzt_unterhalte_uns.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-hier_sind_wir_jetzt_unterhalte_uns.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-i_love_it.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-i_love_it.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-ich_bin_kommunist.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-ich_bin_kommunist.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-ich_darf_nich_und_ich_will_nich.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-ich_darf_nich_und_ich_will_nich.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-im_so_happy_for_no_reason_but_i_dont_care.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-im_so_happy_for_no_reason_but_i_dont_care.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-ja_ja.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-ja_ja.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-kein_problem_ich_hab_zeit.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-kein_problem_ich_hab_zeit.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-koestlich.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-koestlich.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-man_darf_nie_aufhoeren_alles_kritisch_zu_hinterfragen.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-man_darf_nie_aufhoeren_alles_kritisch_zu_hinterfragen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-ohh_hee.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-ohh_hee.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-this_kinda_feels_really_really_awesome.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-this_kinda_feels_really_really_awesome.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-wir_kaempfen_fuer_eine_gerechte_weltordnung_brot_fuer_alle_und_die_aechtung_von_sogennanntem_musikfernsehen.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-wir_kaempfen_fuer_eine_gerechte_weltordnung_brot_fuer_alle_und_die_aechtung_von_sogennanntem_musikfernsehen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-wir_sind_keine_intellektuellen.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-wir_sind_keine_intellektuellen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kaenguru-wolln_wir_uns_dutzen.mp3` & `an-website-24.5/an_website/soundboard/files/kaenguru-wolln_wir_uns_dutzen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/kuh-ahamumumu.mp3` & `an-website-24.5/an_website/soundboard/files/kuh-ahamumumu.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-du_bist_also_teil_der_juedisch-bolschewistischen_weltverschwoerung.mp3` & `an-website-24.5/an_website/soundboard/files/muk-du_bist_also_teil_der_juedisch-bolschewistischen_weltverschwoerung.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-fuer_nichts_und_wieder_nichts.mp3` & `an-website-24.5/an_website/soundboard/files/muk-fuer_nichts_und_wieder_nichts.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-i_am_bored.mp3` & `an-website-24.5/an_website/soundboard/files/muk-i_am_bored.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-i_am_bored_in_the_usa.mp3` & `an-website-24.5/an_website/soundboard/files/muk-i_am_bored_in_the_usa.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-im_just_here_for_the_famous_breakfast.mp3` & `an-website-24.5/an_website/soundboard/files/muk-im_just_here_for_the_famous_breakfast.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-ja_herzlich_willkommen.mp3` & `an-website-24.5/an_website/soundboard/files/muk-ja_herzlich_willkommen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-sprich_bitte_nur_fuer_dich.mp3` & `an-website-24.5/an_website/soundboard/files/muk-sprich_bitte_nur_fuer_dich.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-ueber_mich_hat_die_zeit_geschrieben_dass_ich_der_wahrscheinlich_einflussreichste_linke_interlektulelle_deutschlands_sei.mp3` & `an-website-24.5/an_website/soundboard/files/muk-ueber_mich_hat_die_zeit_geschrieben_dass_ich_der_wahrscheinlich_einflussreichste_linke_interlektulelle_deutschlands_sei.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-und_da_ist_mir_aufgefallen_dass_ich_keine_eier_hab.mp3` & `an-website-24.5/an_website/soundboard/files/muk-und_da_ist_mir_aufgefallen_dass_ich_keine_eier_hab.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-und_mich_dann_auch_noch_beschneiden_lassen.mp3` & `an-website-24.5/an_website/soundboard/files/muk-und_mich_dann_auch_noch_beschneiden_lassen.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-von_mir_aus.mp3` & `an-website-24.5/an_website/soundboard/files/muk-von_mir_aus.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/muk-yeah.mp3` & `an-website-24.5/an_website/soundboard/files/muk-yeah.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/psychiater-aha.mp3` & `an-website-24.5/an_website/soundboard/files/psychiater-aha.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/sarah-hey_thats_cool.mp3` & `an-website-24.5/an_website/soundboard/files/sarah-hey_thats_cool.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/sarah-i_love_life.mp3` & `an-website-24.5/an_website/soundboard/files/sarah-i_love_life.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/sarah-thats_amazing_its_like_you_know_i_dont_know_kind_of_like_whatever_and_stuff.mp3` & `an-website-24.5/an_website/soundboard/files/sarah-thats_amazing_its_like_you_know_i_dont_know_kind_of_like_whatever_and_stuff.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/sarah-the_world_is_so_beautiful.mp3` & `an-website-24.5/an_website/soundboard/files/sarah-the_world_is_so_beautiful.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/sarah-well_thats_just_like_you_know_amazing.mp3` & `an-website-24.5/an_website/soundboard/files/sarah-well_thats_just_like_you_know_amazing.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/files/sarah-yes_its_just_perfect.mp3` & `an-website-24.5/an_website/soundboard/files/sarah-yes_its_just_perfect.mp3`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/icon.svg` & `an-website-24.5/an_website/soundboard/icon.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/info.json` & `an-website-24.5/an_website/soundboard/info.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/soundboard/soundboard.py` & `an-website-24.5/an_website/soundboard/soundboard.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/base.css` & `an-website-24.5/an_website/static/css/base.css`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/base.css.map` & `an-website-24.5/an_website/static/css/base.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/comic.css.map` & `an-website-24.5/an_website/static/css/comic.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/emoji_chat.css.map` & `an-website-24.5/an_website/static/css/emoji_chat.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/form.css` & `an-website-24.5/an_website/static/css/form.css`

 * *Files 10% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-.form,form{width:min(50rem,calc(100% - 2rem))}textarea,select,input[type=email],input[type=range],input[type=search],input[type=text],input[type=number]{display:block;width:100%;box-sizing:border-box;padding:.75rem 1.25rem;border:.125rem solid var(--main-2);border-radius:.625rem;margin:.5rem 0;background:var(--bg)}input[type=submit],button[type=submit],.form-button{width:100%;padding:.875rem 1.25rem;border:none;border-radius:.25rem;margin:.5rem 0;background-color:var(--secondary-bg);cursor:pointer}input[type=submit]:hover,button[type=submit]:hover,.form-button:hover{background-color:var(--main)}.form-element{display:block;width:100%;margin-bottom:.625rem}
+.form,form{width:min(50rem,calc(100% - 2rem))}textarea,select,input[type=email],input[type=number],input[type=range],input[type=search],input[type=text]{display:block;width:100%;box-sizing:border-box;padding:.75rem 1.25rem;border:.125rem solid var(--main-2);border-radius:.625rem;margin:.5rem 0;background:var(--bg)}input[type=range]{padding:initial;border:initial}input[type=submit],button[type=submit],.form-button{width:100%;padding:.875rem 1.25rem;border:none;border-radius:.25rem;margin:.5rem 0;background-color:var(--secondary-bg);cursor:pointer}input[type=submit]:hover,button[type=submit]:hover,.form-button:hover{background-color:var(--main)}.form-element{display:block;width:100%;margin-bottom:.625rem}
 /*# sourceMappingURL=form.css.map */
```

### Comparing `an-website-24.4/an_website/static/css/form.css.map` & `an-website-24.5/an_website/static/css/form.css.map`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'mappings'": "'AAAA,CAAC,KACD,KACI,MAAO,IAAI,KAAK,CAAE,KAAK,KAAK,EAAE,MAClC,CAEA,SACA,OACA,KAAK,CAAC,YACN,KAAK,CAAC,aACN,KAAK,CAAC,YACN,KAAK,CAAC,aACN,KAAK,CAAC,WACF,QAAS,MACT,MAAO,KACP,WAAY,WAdhB,QAea,OAAQ,QACjB,OAAQ,QAAS,MAAM,IAAI,UAhB/B,cAiBmB,QAjBnB,OAkBY,MAAO,EACf,WAAY,IAAI,KACpB,CAEA,KAAK,CAAC,YACF,QAAS,QACT,OAAQ,OACZ,CAEA,KAAK,CAAC,aACN,MAAM,CAAC,aACP,CAAC,YACG,MAAO,KA9BX,QA+Ba,QAAS,QAClB,OAAQ,KAhCZ,cAiCmB,OAjCnB,OAkCY,MAAO,EACf,iBAAkB,IAAI,gBACtB,OAAQ,OACZ,CAEA,KAAK,CAAC,YAAc,OACpB,MAAM,CAAC,YAAc, […]*

```diff
@@ -1,11 +1,11 @@
 {
-    "mappings": "AAAA,CAAC,KACD,KACI,MAAO,IAAI,KAAK,CAAE,KAAK,KAAK,EAAE,MAClC,CAEA,SACA,OACA,KAAK,CAAC,YACN,KAAK,CAAC,YACN,KAAK,CAAC,aACN,KAAK,CAAC,WACN,KAAK,CAAC,aACF,QAAS,MACT,MAAO,KACP,WAAY,WAdhB,QAea,OAAQ,QACjB,OAAQ,QAAS,MAAM,IAAI,UAhB/B,cAiBmB,QAjBnB,OAkBY,MAAO,EACf,WAAY,IAAI,KACpB,CAEA,KAAK,CAAC,aACN,MAAM,CAAC,aACP,CAAC,YACG,MAAO,KAzBX,QA0Ba,QAAS,QAClB,OAAQ,KA3BZ,cA4BmB,OA5BnB,OA6BY,MAAO,EACf,iBAAkB,IAAI,gBACtB,OAAQ,OACZ,CAEA,KAAK,CAAC,YAAc,OACpB,MAAM,CAAC,YAAc,OACrB,CAZC,WAYW,OACR,iBAAkB,IAAI,OAC1B,CAEA,CAAC,aACG,QAAS,MACT,MAAO,KACP,cAAe,OACnB",
+    "mappings": "AAAA,CAAC,KACD,KACI,MAAO,IAAI,KAAK,CAAE,KAAK,KAAK,EAAE,MAClC,CAEA,SACA,OACA,KAAK,CAAC,YACN,KAAK,CAAC,aACN,KAAK,CAAC,YACN,KAAK,CAAC,aACN,KAAK,CAAC,WACF,QAAS,MACT,MAAO,KACP,WAAY,WAdhB,QAea,OAAQ,QACjB,OAAQ,QAAS,MAAM,IAAI,UAhB/B,cAiBmB,QAjBnB,OAkBY,MAAO,EACf,WAAY,IAAI,KACpB,CAEA,KAAK,CAAC,YACF,QAAS,QACT,OAAQ,OACZ,CAEA,KAAK,CAAC,aACN,MAAM,CAAC,aACP,CAAC,YACG,MAAO,KA9BX,QA+Ba,QAAS,QAClB,OAAQ,KAhCZ,cAiCmB,OAjCnB,OAkCY,MAAO,EACf,iBAAkB,IAAI,gBACtB,OAAQ,OACZ,CAEA,KAAK,CAAC,YAAc,OACpB,MAAM,CAAC,YAAc,OACrB,CAZC,WAYW,OACR,iBAAkB,IAAI,OAC1B,CAEA,CAAC,aACG,QAAS,MACT,MAAO,KACP,cAAe,OACnB",
     "names": [],
     "sources": [
         "../../../style/form.css"
     ],
     "sourcesContent": [
-        ".form,\nform {\n    width: min(50rem, calc(100% - 2rem));\n}\n\ntextarea,\nselect,\ninput[type=\"email\"],\ninput[type=\"range\"],\ninput[type=\"search\"],\ninput[type=\"text\"],\ninput[type=\"number\"] {\n    display: block;\n    width: 100%;\n    box-sizing: border-box;\n    padding: 0.75rem 1.25rem;\n    border: 0.125rem solid var(--main-2);\n    border-radius: 0.625rem;\n    margin: 0.5rem 0;\n    background: var(--bg);\n}\n\ninput[type=\"submit\"],\nbutton[type=\"submit\"],\n.form-button {\n    width: 100%;\n    padding: 0.875rem 1.25rem;\n    border: none;\n    border-radius: 0.25rem;\n    margin: 0.5rem 0;\n    background-color: var(--secondary-bg);\n    cursor: pointer;\n}\n\ninput[type=\"submit\"]:hover,\nbutton[type=\"submit\"]:hover,\n.form-button:hover {\n    background-color: var(--main);\n}\n\n.form-element {\n    display: block;\n    width: 100%;\n    margin-bottom: 0.625rem;\n}\n"
+        ".form,\nform {\n    width: min(50rem, calc(100% - 2rem));\n}\n\ntextarea,\nselect,\ninput[type=\"email\"],\ninput[type=\"number\"],\ninput[type=\"range\"],\ninput[type=\"search\"],\ninput[type=\"text\"] {\n    display: block;\n    width: 100%;\n    box-sizing: border-box;\n    padding: 0.75rem 1.25rem;\n    border: 0.125rem solid var(--main-2);\n    border-radius: 0.625rem;\n    margin: 0.5rem 0;\n    background: var(--bg);\n}\n\ninput[type=\"range\"] {\n    padding: initial;\n    border: initial;\n}\n\ninput[type=\"submit\"],\nbutton[type=\"submit\"],\n.form-button {\n    width: 100%;\n    padding: 0.875rem 1.25rem;\n    border: none;\n    border-radius: 0.25rem;\n    margin: 0.5rem 0;\n    background-color: var(--secondary-bg);\n    cursor: pointer;\n}\n\ninput[type=\"submit\"]:hover,\nbutton[type=\"submit\"]:hover,\n.form-button:hover {\n    background-color: var(--main);\n}\n\n.form-element {\n    display: block;\n    width: 100%;\n    margin-bottom: 0.625rem;\n}\n"
     ],
     "version": 3
 }
```

### Comparing `an-website-24.4/an_website/static/css/kangaroo_comics.css` & `an-website-24.5/an_website/static/css/kangaroo_comics.css`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/kangaroo_comics.css.map` & `an-website-24.5/an_website/static/css/kangaroo_comics.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/quotes/generator.css.map` & `an-website-24.5/an_website/static/css/quotes/generator.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/quotes/info.css` & `an-website-24.5/an_website/static/css/quotes/info.css`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/quotes/info.css.map` & `an-website-24.5/an_website/static/css/quotes/info.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/quotes/quotes.css` & `an-website-24.5/an_website/static/css/quotes/quotes.css`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/quotes/quotes.css.map` & `an-website-24.5/an_website/static/css/quotes/quotes.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/quotes/share.css` & `an-website-24.5/an_website/static/css/quotes/share.css`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/quotes/share.css.map` & `an-website-24.5/an_website/static/css/quotes/share.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/redirect.css.map` & `an-website-24.5/an_website/static/css/redirect.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/snow.css` & `an-website-24.5/an_website/static/css/snow.css`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/snow.css.map` & `an-website-24.5/an_website/static/css/snow.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/soundboard.css.map` & `an-website-24.5/an_website/static/css/soundboard.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/table.css.map` & `an-website-24.5/an_website/static/css/table.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/blue.css.map` & `an-website-24.5/an_website/static/css/themes/blue.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/christmas.css` & `an-website-24.5/an_website/static/css/themes/christmas.css`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/christmas.css.map` & `an-website-24.5/an_website/static/css/themes/christmas.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/default.css.map` & `an-website-24.5/an_website/static/css/themes/default.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/fun.css.map` & `an-website-24.5/an_website/static/css/themes/fun.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/green.css.map` & `an-website-24.5/an_website/static/css/themes/green.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/light.css.map` & `an-website-24.5/an_website/static/css/themes/light.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/light_blue.css.map` & `an-website-24.5/an_website/static/css/themes/light_blue.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/orange.css.map` & `an-website-24.5/an_website/static/css/themes/orange.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/pink.css.map` & `an-website-24.5/an_website/static/css/themes/pink.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/purple.css.map` & `an-website-24.5/an_website/static/css/themes/purple.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/themes/yellow.css.map` & `an-website-24.5/an_website/static/css/themes/yellow.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/css/uptime.css.map` & `an-website-24.5/an_website/static/css/uptime.css.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/favicon.jxl` & `an-website-24.5/an_website/static/favicon.jxl`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/favicon.png` & `an-website-24.5/an_website/static/favicon.png`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/fonts/NOTICE.txt` & `an-website-24.5/an_website/static/fonts/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/fonts/comic.woff2` & `an-website-24.5/an_website/static/fonts/comic.woff2`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/fonts/comicmono.woff2` & `an-website-24.5/an_website/static/fonts/comicmono.woff2`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/fonts/cursedtimerulil-aznm.woff2` & `an-website-24.5/an_website/static/fonts/cursedtimerulil-aznm.woff2`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/2020-11-03.jpg` & `an-website-24.5/an_website/static/img/2020-11-03.jpg`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/NOTICE.txt` & `an-website-24.5/an_website/static/img/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/kangarooface.svg` & `an-website-24.5/an_website/static/img/kangarooface.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/logo.svg` & `an-website-24.5/an_website/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/netcup-oekostrom2.jxl` & `an-website-24.5/an_website/static/img/netcup-oekostrom2.jxl`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/netcup-oekostrom2.png` & `an-website-24.5/an_website/static/img/netcup-oekostrom2.png`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/rss.svg` & `an-website-24.5/an_website/static/img/rss.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/save.svg` & `an-website-24.5/an_website/static/img/save.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/stamps/nichtwitzig.small.svg` & `an-website-24.5/an_website/static/img/stamps/nichtwitzig.small.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/img/stamps/witzig.small.svg` & `an-website-24.5/an_website/static/img/stamps/witzig.small.svg`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/currency_converter/converter.js` & `an-website-24.5/an_website/static/js/currency_converter/converter.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/currency_converter/converter.js.map` & `an-website-24.5/an_website/static/js/currency_converter/converter.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/emoji_chat/chat.js` & `an-website-24.5/an_website/static/js/emoji_chat/chat.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/emoji_chat/chat.js.map` & `an-website-24.5/an_website/static/js/emoji_chat/chat.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/hangman_solver/hangman_solver.js` & `an-website-24.5/an_website/static/js/hangman_solver/hangman_solver.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/hangman_solver/hangman_solver.js.map` & `an-website-24.5/an_website/static/js/hangman_solver/hangman_solver.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/kangaroo_comics/comics.js` & `an-website-24.5/an_website/static/js/kangaroo_comics/comics.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -137,15 +137,15 @@
             d()
         };
         const a = i.cloneNode(!0);
         a.classList.remove("normal-img"), a.classList.add("popup-img");
         const t = document.createElement("img");
         t.classList.add("close-button"), t.src = "/static/img/close.svg?v=0", n.appendChild(a), n.appendChild(t), i.parentNode.appendChild(n)
     };
-    o.concat(B.split("\n")), F();
+    o.push(...B.split("\n")), F();
     const v = u(y(), 1);
     b(v), k.onerror = () => {
         u(v, -1), b(v), g < E && g++
     }
 }
 const p = document.getElementById("start-button-no_3rd_party");
 if (p !== null) {
```

### Comparing `an-website-24.4/an_website/static/js/kangaroo_comics/comics.js.map` & `an-website-24.5/an_website/static/js/kangaroo_comics/comics.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'mappings'": "'AAAA;AACA,SAEA,SAASA,GAAqB,CAC1B,MAAMC,EAAY,CAACC,EAAcC,EAAeC,IAC5C,IAAI,KAAKF,EAAMC,EAAQ,EAAGC,EAAY,EAAG,EAAG,EAAG,CAAC,EAE9CC,EAA+B,CACjC,CACIJ,EAAU,KAAM,EAAG,EAAE,EACrB,8CACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,qDACJ,EACA,CACIA,EAAU,KAAM,GAAI,CAAC,EACrB,oDACJ,EACA,CACIA,EAAU,KAAM,GAAI,EAAE,EACtB,6CACJ,EACA,CACIA,EAAU,KAAM,GAAI,CAAC,EACrB,2DACJ,EACA,CACIA,EAAU,KAAM,GAAI,CAAC,EACrB,oDACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,uDACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,mDACJ,EACA,CACIA,EAAU, […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "mappings": "AAAA;AACA,SAEA,SAASA,GAAqB,CAC1B,MAAMC,EAAY,CAACC,EAAcC,EAAeC,IAC5C,IAAI,KAAKF,EAAMC,EAAQ,EAAGC,EAAY,EAAG,EAAG,EAAG,CAAC,EAE9CC,EAA+B,CACjC,CACIJ,EAAU,KAAM,EAAG,EAAE,EACrB,8CACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,qDACJ,EACA,CACIA,EAAU,KAAM,GAAI,CAAC,EACrB,oDACJ,EACA,CACIA,EAAU,KAAM,GAAI,EAAE,EACtB,6CACJ,EACA,CACIA,EAAU,KAAM,GAAI,CAAC,EACrB,2DACJ,EACA,CACIA,EAAU,KAAM,GAAI,CAAC,EACrB,oDACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,uDACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,mDACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,6CACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,6CACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,sEACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,oDACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,oDACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,6EACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,uDACJ,CACJ,EAEMK,EAAa,CACfC,EACAL,EACAC,EACAC,IAGAG,EAAK,YAAY,IAAML,GACvBK,EAAK,SAAS,IAAOJ,EAAQ,GAC7BI,EAAK,QAAQ,IAAMH,EAGjBI,EAAa,CAACC,EAAaC,IAC7BJ,EACIG,EACAC,EAAM,YAAY,EAClBA,EAAM,SAAS,EAAI,EACnBA,EAAM,QAAQ,CAClB,EAEEC,EAAYJ,GACdA,GACAA,EAAK,OAAO,IAAM,GAElB,CAACD,EAAWC,EAAM,KAAM,GAAI,EAAE,EAG5BK,EAAYL,GACdN,EAAUM,EAAK,YAAY,EAAGA,EAAK,SAAS,EAAI,EAAGA,EAAK,QAAQ,CAAC,EAG/DM,EAAW,IAAYD,EAAS,IAAI,IAAM,EAE1CE,EAAmB,CAAC,EAEpBC,EAAQ,+8EA+Cd,SAASC,GAAyB,CAC9B,MAAMC,EAAQJ,EAAS,EACjBN,EAAOK,EAASM,CAAoB,EAC1C,KAAOX,EAAK,QAAQ,GAAKU,EAAM,QAAQ,GACnCH,EAAO,KAAKK,EAAkBZ,CAAI,CAAC,EACnCa,EAAmBb,EAAM,CAAC,CAElC,CAEA,MAAMc,EAAiE,CACnE,UACA,SACA,WACA,WACA,aACA,UACA,SACJ,EAEMC,EAAcf,GAAuBc,EAAKd,EAAK,OAAO,CAAC,EACvDgB,EAaF,CACA,SACA,UACA,OACA,QACA,MACA,OACA,OACA,SACA,YACA,UACA,WACA,UACJ,EAEMC,EAAgBjB,GAAuBgB,EAAOhB,EAAK,SAAS,CAAC,EAE7DkB,EAAiBlB,GACnB,aAAa,OAAAe,EAAWf,CAAI,EAAC,UAAS,OAAAA,EAAK,QAAQ,EAAC,MAChD,OAAAiB,EAAajB,CAAI,EACrB,KAAI,OAAAA,EAAK,YAAY,GAGzB,SAASmB,GAAkB,CACvB,UAAWC,KAAQ,SAAS,uBAAuB,iBAAiB,EAChEA,EAAK,OAAO,CAEpB,CAEA,MAAMC,EAAmB,SAAS,eAC9B,sBACJ,EACMC,EAAa,SAAS,eACxB,aACJ,EACAA,EAAW,YAAcH,EAEzB,SAASI,EAAgBvB,EAAY,CACjC,IAAIwB,EAAOZ,EAAkBZ,CAAI,EACjCwB,EAAOA,EAAK,WAAW,GAAG,EAAIA,EAAO,uBAAyBA,EAC9DF,EAAW,IAAME,EAEjBH,EAAiB,UAAY,WAAaH,EAAclB,CAAI,EAAI,IAChEqB,EAAiB,KAAOG,CAC5B,CAEA,MAAMC,EAAuB/B,EAAU,KAAM,GAAI,CAAC,EAC5CgC,EACF,2EAEEf,EAAuBjB,EAAU,KAAM,EAAG,EAAE,EAC5CiC,EACF,0EAEEC,EAAoB,kDAE1B,SAASC,EAAgBL,EAA2B,CAChD,UAAWM,IAAO,CAACH,EAAcC,CAAiB,EAAG,CAEjD,MAAMG,EAAQP,EAAK,YAAY,EAAE,MAAMM,CAAG,EAC1C,GAAIC,GAASA,EAAM,OAAS,EACxB,OAAOrC,EAEH,SAASqC,EAAM,CAAC,CAAC,EAEjB,SAASA,EAAM,CAAC,CAAC,EAEjB,SAASA,EAAM,CAAC,CAAC,CACrB,CAER,CAEA,MAAMC,EAAMR,EAAK,YAAY,EAAE,MAAME,CAAY,EACjD,GAAIM,GAAOA,EAAI,OAAS,EAAG,CAEvB,MAAMC,EAAM,SAASD,EAAI,CAAC,CAAC,EAAI,EACzBhC,EAAO,IAAI,KAAKyB,EAAqB,QAAQ,CAAC,EACpD,QAASS,EAAI,EAAGA,EAAID,EAAKC,IACrBlC,EAAK,QACDa,EAAmBb,EAAMI,EAASJ,CAAI,EAAI,EAAI,CAAC,EAAE,QAAQ,CAC7D,EAEJ,OAAOI,EAASJ,CAAI,EAAIa,EAAmBb,EAAM,CAAC,EAAIA,CAC1D,CAEA,OADAwB,EAAOA,EAAK,YAAY,EAAE,KAAK,EACvBA,EAAM,CACV,IAAK,0DACD,OAAO9B,EAAU,KAAM,GAAI,EAAE,EACjC,IAAK,wDACD,OAAOA,EAAU,KAAM,GAAI,EAAE,EACjC,IAAK,4CACD,OAAOA,EAAU,KAAM,GAAI,EAAE,EACjC,IAAK,6DACD,OAAOA,EAAU,KAAM,GAAI,CAAC,EAChC,IAAK,4DACD,OAAOA,EAAU,KAAM,GAAI,CAAC,EAChC,IAAK,gEACD,OAAOA,EAAU,KAAM,GAAI,EAAE,CACrC,CACA,UAAWsC,KAAOlC,EACd,GAAI0B,IAASQ,EAAI,CAAC,EACd,OAAOA,EAAI,CAAC,EAGpB,OAAO,IACX,CAEA,MAAMG,EAAa,oDAEnB,SAASvB,EAAkBZ,EAAoB,CAC3C,UAAWgC,KAAOlC,EACd,GAAIG,EAAWD,EAAMgC,EAAI,CAAC,CAAC,EACvB,OAAOA,EAAI,CAAC,EAGpB,MAAMpC,GAASI,EAAK,SAAS,EAAI,GAAG,SAAS,EACvCoC,EAAMpC,EAAK,QAAQ,EAAE,SAAS,EACpC,OAAOmC,EACF,QAAQ,KAAMnC,EAAK,YAAY,EAAE,SAAS,CAAC,EAC3C,QAAQ,KAAMJ,EAAM,SAAW,EAAIA,EAAQ,IAAMA,CAAK,EACtD,QAAQ,KAAMwC,EAAI,SAAW,EAAIA,EAAM,IAAMA,CAAG,CACzD,CAEA,SAASvB,EAAmBb,EAAYc,EAAoB,CACxD,OAAAd,EAAK,QAEDA,EAAK,QAAQ,EAAKc,EAAO,IAAO,GAAK,GAAK,EAC9C,EACAd,EAAK,SAAS,CAAC,EACRA,CACX,CAEA,MAAMqC,EAA0B,EAC1BC,EAAa,SAAS,eAAe,aAAa,EAClDC,EAAO,SAAS,eAAe,iBAAiB,EACtD,IAAIC,EAAS,EAEb,MAAMC,EAAiB,IAAM,CACzB,QAAS,EAAI,EAAG,EAAIJ,EAAyB,IAAK,CAC9CG,IACA,MAAME,EAAInC,EAAO,OAASiC,EAC1B,GAAIE,EAAI,EACJ,MAGJ,IAAIlB,EAAOjB,EAAOmC,CAAC,EAEnB,MAAM1C,EAAO6B,EAAgBL,CAAI,EACjC,GAAIxB,IAAS,KAAM,CACf,QAAQ,MAAM,qBAAuBwB,CAAI,EACzC,QACJ,CAEAA,EAAOA,EAAK,WAAW,GAAG,EAAIA,EAAO,uBAAyBA,EAE9D,MAAMmB,EAAW,SAAS,cAAc,IAAI,EACtCC,EAAS,SAAS,cAAc,GAAG,EACzCA,EAAO,UAAU,IAAI,cAAc,EACnCA,EAAO,UAAY1B,EAAclB,CAAI,EAAI,IAEzC4C,EAAO,KAAOpB,EACdoB,EAAO,MAAM,SAAW,OACxBD,EAAS,YAAYC,CAAM,EAC3BD,EAAS,YAAY,SAAS,cAAc,IAAI,CAAC,EACjD,MAAME,EAAQ,SAAS,cAAc,KAAK,EAC1CA,EAAM,UAAU,IAAI,YAAY,EAGhCA,EAAM,IAAMrB,EACZqB,EAAM,IAAM3B,EAAclB,CAAI,EAC9B6C,EAAM,QAAU,IAAM,CAClBC,EAAeD,CAAK,CACxB,EACAA,EAAM,QAAU,IAAM,CACdzC,EAASJ,CAAI,EAGbuC,EAAK,YAAYI,CAAQ,EAGzBA,EAAS,OAAO,+BAA+B,CAEvD,EACAA,EAAS,YAAYE,CAAK,EAC1BN,EAAK,YAAYI,CAAQ,CAC7B,CAEIH,GAAUjC,EAAO,SACjB+B,EAAW,MAAM,QAAU,IAC3BA,EAAW,MAAM,WAAa,YAEtC,EACC,SAAS,eAAe,aAAa,EAAI,QAAUG,EAEpD,MAAMK,EAAkBD,GAA4B,CAChD1B,EAAgB,EAEhB,MAAM4B,EAAiB,SAAS,cAAc,KAAK,EACnDA,EAAe,UAAU,IAAI,iBAAiB,EAC9CA,EAAe,aAAe,IAAM,CAChCA,EAAe,OAAO,CAC1B,EACAA,EAAe,QAAU,IAAM,CAC3B5B,EAAgB,CACpB,EAEA,MAAM6B,EAAQH,EAAM,UAAU,EAAI,EAClCG,EAAM,UAAU,OAAO,YAAY,EACnCA,EAAM,UAAU,IAAI,WAAW,EAE/B,MAAMC,EAAc,SAAS,cAAc,KAAK,EAChDA,EAAY,UAAU,IAAI,cAAc,EACxCA,EAAY,IAAM,4BAElBF,EAAe,YAAYC,CAAK,EAChCD,EAAe,YAAYE,CAAW,EACtCJ,EAAM,WAAY,YAAYE,CAAc,CAChD,EAGAxC,EAAO,OAAOC,EAAM,MAAM,IAAI,CAAC,EAC/BC,EAAiB,EAEjB,MAAMC,EAAQG,EAAmBP,EAAS,EAAG,CAAC,EAC9CiB,EAAgBb,CAAK,EACrBY,EAAW,QAAU,IAAM,CACvBT,EAAmBH,EAAO,EAAE,EAC5Ba,EAAgBb,CAAK,EAEjB8B,EAASH,GACTG,GAER,CACJ,CAEA,MAAMU,EAAc,SAAS,eAAe,2BAA2B,EACvE,GAAIA,IAAgB,KAAM,CACtB,MAAMC,EAAmB,SAAS,eAC9B,yBACJ,EAEAD,EAAY,QAAU,IAAM,CACxBA,EAAY,OAAO,EACnBC,EAAiB,UAAU,OAAO,QAAQ,EAC1C1D,EAAmB,CACvB,EACA0D,EAAiB,UAAU,IAAI,QAAQ,CAC3C,MACI1D,EAAmB,EAEvB;",
+    "mappings": "AAAA;AACA,SAEA,SAASA,GAAqB,CAC1B,MAAMC,EAAY,CAACC,EAAcC,EAAeC,IAC5C,IAAI,KAAKF,EAAMC,EAAQ,EAAGC,EAAY,EAAG,EAAG,EAAG,CAAC,EAE9CC,EAA+B,CACjC,CACIJ,EAAU,KAAM,EAAG,EAAE,EACrB,8CACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,qDACJ,EACA,CACIA,EAAU,KAAM,GAAI,CAAC,EACrB,oDACJ,EACA,CACIA,EAAU,KAAM,GAAI,EAAE,EACtB,6CACJ,EACA,CACIA,EAAU,KAAM,GAAI,CAAC,EACrB,2DACJ,EACA,CACIA,EAAU,KAAM,GAAI,CAAC,EACrB,oDACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,uDACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,mDACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,6CACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,6CACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,sEACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,oDACJ,EACA,CACIA,EAAU,KAAM,EAAG,CAAC,EACpB,oDACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,6EACJ,EACA,CACIA,EAAU,KAAM,EAAG,EAAE,EACrB,uDACJ,CACJ,EAEMK,EAAa,CACfC,EACAL,EACAC,EACAC,IAGAG,EAAK,YAAY,IAAML,GACvBK,EAAK,SAAS,IAAOJ,EAAQ,GAC7BI,EAAK,QAAQ,IAAMH,EAGjBI,EAAa,CAACC,EAAaC,IAC7BJ,EACIG,EACAC,EAAM,YAAY,EAClBA,EAAM,SAAS,EAAI,EACnBA,EAAM,QAAQ,CAClB,EAEEC,EAAYJ,GACdA,GACAA,EAAK,OAAO,IAAM,GAElB,CAACD,EAAWC,EAAM,KAAM,GAAI,EAAE,EAG5BK,EAAYL,GACdN,EAAUM,EAAK,YAAY,EAAGA,EAAK,SAAS,EAAI,EAAGA,EAAK,QAAQ,CAAC,EAG/DM,EAAW,IAAYD,EAAS,IAAI,IAAM,EAE1CE,EAAmB,CAAC,EAEpBC,EAAQ,+8EA+Cd,SAASC,GAAyB,CAC9B,MAAMC,EAAQJ,EAAS,EACjBN,EAAOK,EAASM,CAAoB,EAC1C,KAAOX,EAAK,QAAQ,GAAKU,EAAM,QAAQ,GACnCH,EAAO,KAAKK,EAAkBZ,CAAI,CAAC,EACnCa,EAAmBb,EAAM,CAAC,CAElC,CAEA,MAAMc,EAAiE,CACnE,UACA,SACA,WACA,WACA,aACA,UACA,SACJ,EAEMC,EAAcf,GAAuBc,EAAKd,EAAK,OAAO,CAAC,EACvDgB,EAaF,CACA,SACA,UACA,OACA,QACA,MACA,OACA,OACA,SACA,YACA,UACA,WACA,UACJ,EAEMC,EAAgBjB,GAAuBgB,EAAOhB,EAAK,SAAS,CAAC,EAE7DkB,EAAiBlB,GACnB,aAAa,OAAAe,EAAWf,CAAI,EAAC,UAAS,OAAAA,EAAK,QAAQ,EAAC,MAChD,OAAAiB,EAAajB,CAAI,EACrB,KAAI,OAAAA,EAAK,YAAY,GAGzB,SAASmB,GAAkB,CACvB,UAAWC,KAAQ,SAAS,uBAAuB,iBAAiB,EAChEA,EAAK,OAAO,CAEpB,CAEA,MAAMC,EAAmB,SAAS,eAC9B,sBACJ,EACMC,EAAa,SAAS,eACxB,aACJ,EACAA,EAAW,YAAcH,EAEzB,SAASI,EAAgBvB,EAAY,CACjC,IAAIwB,EAAOZ,EAAkBZ,CAAI,EACjCwB,EAAOA,EAAK,WAAW,GAAG,EAAIA,EAAO,uBAAyBA,EAC9DF,EAAW,IAAME,EAEjBH,EAAiB,UAAY,WAAaH,EAAclB,CAAI,EAAI,IAChEqB,EAAiB,KAAOG,CAC5B,CAEA,MAAMC,EAAuB/B,EAAU,KAAM,GAAI,CAAC,EAC5CgC,EACF,2EAEEf,EAAuBjB,EAAU,KAAM,EAAG,EAAE,EAC5CiC,EACF,0EAEEC,EAAoB,kDAE1B,SAASC,EAAgBL,EAA2B,CAChD,UAAWM,IAAO,CAACH,EAAcC,CAAiB,EAAG,CAEjD,MAAMG,EAAQP,EAAK,YAAY,EAAE,MAAMM,CAAG,EAC1C,GAAIC,GAASA,EAAM,OAAS,EACxB,OAAOrC,EAEH,SAASqC,EAAM,CAAC,CAAC,EAEjB,SAASA,EAAM,CAAC,CAAC,EAEjB,SAASA,EAAM,CAAC,CAAC,CACrB,CAER,CAEA,MAAMC,EAAMR,EAAK,YAAY,EAAE,MAAME,CAAY,EACjD,GAAIM,GAAOA,EAAI,OAAS,EAAG,CAEvB,MAAMC,EAAM,SAASD,EAAI,CAAC,CAAC,EAAI,EACzBhC,EAAO,IAAI,KAAKyB,EAAqB,QAAQ,CAAC,EACpD,QAASS,EAAI,EAAGA,EAAID,EAAKC,IACrBlC,EAAK,QACDa,EAAmBb,EAAMI,EAASJ,CAAI,EAAI,EAAI,CAAC,EAAE,QAAQ,CAC7D,EAEJ,OAAOI,EAASJ,CAAI,EAAIa,EAAmBb,EAAM,CAAC,EAAIA,CAC1D,CAEA,OADAwB,EAAOA,EAAK,YAAY,EAAE,KAAK,EACvBA,EAAM,CACV,IAAK,0DACD,OAAO9B,EAAU,KAAM,GAAI,EAAE,EACjC,IAAK,wDACD,OAAOA,EAAU,KAAM,GAAI,EAAE,EACjC,IAAK,4CACD,OAAOA,EAAU,KAAM,GAAI,EAAE,EACjC,IAAK,6DACD,OAAOA,EAAU,KAAM,GAAI,CAAC,EAChC,IAAK,4DACD,OAAOA,EAAU,KAAM,GAAI,CAAC,EAChC,IAAK,gEACD,OAAOA,EAAU,KAAM,GAAI,EAAE,CACrC,CACA,UAAWsC,KAAOlC,EACd,GAAI0B,IAASQ,EAAI,CAAC,EACd,OAAOA,EAAI,CAAC,EAGpB,OAAO,IACX,CAEA,MAAMG,EAAa,oDAEnB,SAASvB,EAAkBZ,EAAoB,CAC3C,UAAWgC,KAAOlC,EACd,GAAIG,EAAWD,EAAMgC,EAAI,CAAC,CAAC,EACvB,OAAOA,EAAI,CAAC,EAGpB,MAAMpC,GAASI,EAAK,SAAS,EAAI,GAAG,SAAS,EACvCoC,EAAMpC,EAAK,QAAQ,EAAE,SAAS,EACpC,OAAOmC,EACF,QAAQ,KAAMnC,EAAK,YAAY,EAAE,SAAS,CAAC,EAC3C,QAAQ,KAAMJ,EAAM,SAAW,EAAIA,EAAQ,IAAMA,CAAK,EACtD,QAAQ,KAAMwC,EAAI,SAAW,EAAIA,EAAM,IAAMA,CAAG,CACzD,CAEA,SAASvB,EAAmBb,EAAYc,EAAoB,CACxD,OAAAd,EAAK,QAEDA,EAAK,QAAQ,EAAKc,EAAO,IAAO,GAAK,GAAK,EAC9C,EACAd,EAAK,SAAS,CAAC,EACRA,CACX,CAEA,MAAMqC,EAA0B,EAC1BC,EAAa,SAAS,eAAe,aAAa,EAClDC,EAAO,SAAS,eAAe,iBAAiB,EACtD,IAAIC,EAAS,EAEb,MAAMC,EAAiB,IAAM,CACzB,QAAS,EAAI,EAAG,EAAIJ,EAAyB,IAAK,CAC9CG,IACA,MAAME,EAAInC,EAAO,OAASiC,EAC1B,GAAIE,EAAI,EACJ,MAGJ,IAAIlB,EAAOjB,EAAOmC,CAAC,EAEnB,MAAM1C,EAAO6B,EAAgBL,CAAI,EACjC,GAAIxB,IAAS,KAAM,CACf,QAAQ,MAAM,qBAAuBwB,CAAI,EACzC,QACJ,CAEAA,EAAOA,EAAK,WAAW,GAAG,EAAIA,EAAO,uBAAyBA,EAE9D,MAAMmB,EAAW,SAAS,cAAc,IAAI,EACtCC,EAAS,SAAS,cAAc,GAAG,EACzCA,EAAO,UAAU,IAAI,cAAc,EACnCA,EAAO,UAAY1B,EAAclB,CAAI,EAAI,IAEzC4C,EAAO,KAAOpB,EACdoB,EAAO,MAAM,SAAW,OACxBD,EAAS,YAAYC,CAAM,EAC3BD,EAAS,YAAY,SAAS,cAAc,IAAI,CAAC,EACjD,MAAME,EAAQ,SAAS,cAAc,KAAK,EAC1CA,EAAM,UAAU,IAAI,YAAY,EAGhCA,EAAM,IAAMrB,EACZqB,EAAM,IAAM3B,EAAclB,CAAI,EAC9B6C,EAAM,QAAU,IAAM,CAClBC,EAAeD,CAAK,CACxB,EACAA,EAAM,QAAU,IAAM,CACdzC,EAASJ,CAAI,EAGbuC,EAAK,YAAYI,CAAQ,EAGzBA,EAAS,OAAO,+BAA+B,CAEvD,EACAA,EAAS,YAAYE,CAAK,EAC1BN,EAAK,YAAYI,CAAQ,CAC7B,CAEIH,GAAUjC,EAAO,SACjB+B,EAAW,MAAM,QAAU,IAC3BA,EAAW,MAAM,WAAa,YAEtC,EACC,SAAS,eAAe,aAAa,EAAI,QAAUG,EAEpD,MAAMK,EAAkBD,GAA4B,CAChD1B,EAAgB,EAEhB,MAAM4B,EAAiB,SAAS,cAAc,KAAK,EACnDA,EAAe,UAAU,IAAI,iBAAiB,EAC9CA,EAAe,aAAe,IAAM,CAChCA,EAAe,OAAO,CAC1B,EACAA,EAAe,QAAU,IAAM,CAC3B5B,EAAgB,CACpB,EAEA,MAAM6B,EAAQH,EAAM,UAAU,EAAI,EAClCG,EAAM,UAAU,OAAO,YAAY,EACnCA,EAAM,UAAU,IAAI,WAAW,EAE/B,MAAMC,EAAc,SAAS,cAAc,KAAK,EAChDA,EAAY,UAAU,IAAI,cAAc,EACxCA,EAAY,IAAM,4BAElBF,EAAe,YAAYC,CAAK,EAChCD,EAAe,YAAYE,CAAW,EACtCJ,EAAM,WAAY,YAAYE,CAAc,CAChD,EAGAxC,EAAO,KAAK,GAAGC,EAAM,MAAM,IAAI,CAAC,EAChCC,EAAiB,EAEjB,MAAMC,EAAQG,EAAmBP,EAAS,EAAG,CAAC,EAC9CiB,EAAgBb,CAAK,EACrBY,EAAW,QAAU,IAAM,CACvBT,EAAmBH,EAAO,EAAE,EAC5Ba,EAAgBb,CAAK,EAEjB8B,EAASH,GACTG,GAER,CACJ,CAEA,MAAMU,EAAc,SAAS,eAAe,2BAA2B,EACvE,GAAIA,IAAgB,KAAM,CACtB,MAAMC,EAAmB,SAAS,eAC9B,yBACJ,EAEAD,EAAY,QAAU,IAAM,CACxBA,EAAY,OAAO,EACnBC,EAAiB,UAAU,OAAO,QAAQ,EAC1C1D,EAAmB,CACvB,EACA0D,EAAiB,UAAU,IAAI,QAAQ,CAC3C,MACI1D,EAAmB,EAEvB;",
     "names": [
         "startLoadingComics",
         "getDateBy",
         "year",
         "month",
         "dayOfMonth",
         "wrongLinks",
@@ -61,11 +61,11 @@
         "startButton",
         "contentContainer"
     ],
     "sources": [
         "../../../kangaroo_comics/comics.ts"
     ],
     "sourcesContent": [
-        "// @license magnet:?xt=urn:btih:0b31508aeb0634b347b8270c7bee4d411b5d4109&dn=agpl-3.0.txt AGPL-3.0-or-later\nexport {};\n\nfunction startLoadingComics() {\n    const getDateBy = (year: number, month: number, dayOfMonth: number): Date =>\n        new Date(year, month - 1, dayOfMonth, 6, 0, 0, 0);\n    // date with special link format\n    const wrongLinks: [Date, string][] = [\n        [\n            getDateBy(2021, 5, 25),\n            \"administratives/kaenguru-comics/25/original/\",\n        ],\n        [\n            getDateBy(2021, 9, 6),\n            \"administratives/kaenguru-comics/2021-09/6/original/\",\n        ],\n        [\n            getDateBy(2021, 10, 4),\n            \"administratives/kaenguru-comics/2021-10/4/original\",\n        ],\n        [\n            getDateBy(2021, 10, 29),\n            \"administratives/kaenguru-comics/29/original\",\n        ],\n        [\n            getDateBy(2021, 11, 3),\n            \"administratives/kaenguru-comics/2021-11/03-11-21/original\",\n        ],\n        [\n            getDateBy(2021, 12, 6),\n            \"administratives/kaenguru-comics/2021-12/6/original\",\n        ],\n        [\n            getDateBy(2022, 1, 29),\n            \"administratives/kaenguru-comics/2022-01/29-3/original\",\n        ],\n        [\n            getDateBy(2022, 2, 7),\n            \"administratives/kaenguru-comics/08-02-22/original\",\n        ],\n        [\n            getDateBy(2022, 2, 12),\n            \"administratives/kaenguru-comics/12/original\",\n        ],\n        [\n            getDateBy(2022, 2, 14),\n            \"administratives/kaenguru-comics/14/original\",\n        ],\n        [\n            getDateBy(2022, 3, 28),\n            \"administratives/kaenguru-comics/2022-03/kaenguru-2022-03-28/original\",\n        ],\n        [\n            getDateBy(2022, 4, 4),\n            \"administratives/kaenguru-comics/2022-04/4/original\",\n        ],\n        [\n            getDateBy(2022, 5, 9),\n            \"administratives/kaenguru-comics/2022-05/9/original\",\n        ],\n        [\n            getDateBy(2022, 8, 15),\n            \"administratives/kaenguru-comics/2022-08/kaenguru-comics-2022-08-15/original\",\n        ],\n        [\n            getDateBy(2022, 8, 29),\n            \"administratives/kaenguru-comics/2022-08/29-3/original\",\n        ],\n    ];\n\n    const dateEquals = (\n        date: Date,\n        year: number,\n        month: number,\n        dayOfMonth: number,\n    ): boolean => (\n        // check if a date equals another based on year, month, and dayOfMonth\n        date.getFullYear() === year &&\n        date.getMonth() === (month - 1) && // JS is stupid\n        date.getDate() === dayOfMonth\n    );\n\n    const datesEqual = (date1: Date, date2: Date): boolean =>\n        dateEquals(\n            date1,\n            date2.getFullYear(),\n            date2.getMonth() + 1, // JS is stupid\n            date2.getDate(),\n        );\n\n    const isSunday = (date: Date | undefined) => (\n        date &&\n        date.getDay() === 0 &&\n        // exception for 2020-12-20 (sunday) because there was a comic\n        !dateEquals(date, 2020, 12, 20)\n    );\n\n    const copyDate = (date: Date): Date =>\n        getDateBy(date.getFullYear(), date.getMonth() + 1, date.getDate());\n\n    // get today without hours, minutes, seconds and ms\n    const getToday = (): Date => copyDate(new Date());\n\n    const comics: string[] = [];\n\n    const links = `/static/img/2020-11-03.jpg\nadministratives/kaenguru-comics/pilot-kaenguru/original\nadministratives/kaenguru-comics/pow-kaenguru/original\nstatic/img/kaenguru-announcement/original\nadministratives/kaenguru-comics/der-baum-kaenguru/original\nadministratives/kaenguru-comics/warnung-kaenguru/original\nadministratives/kaenguru-comics/kaenguru-005/original\nadministratives/kaenguru-comics/kaenguru-006/original\nadministratives/kaenguru-comics/kaenguru-007/original\nadministratives/kaenguru-comics/kaenguru-008/original\nadministratives/kaenguru-comics/kaenguru-009/original\nadministratives/kaenguru-comics/kaenguru-010/original\nadministratives/kaenguru-comics/kaenguru-011/original\nadministratives/kaenguru-comics/kaenguru-012/original\nadministratives/kaenguru-comics/kaenguru-013/original\nadministratives/kaenguru-comics/kaenguru-014/original\nadministratives/kaenguru-comics/kaenguru-015/original\nadministratives/kaenguru-comics/kaenguru-016/original\nadministratives/kaenguru-comics/kaenguru-017/original\nadministratives/kaenguru-comics/kaenguru-018/original\nadministratives/2020-12/kaenguru-comics-kaenguru-019/original\nadministratives/kaenguru-comics/kaenguru-020/original\nadministratives/kaenguru-comics/kaenguru-021/original\nadministratives/kaenguru-comics/kaenguru-023/original\nadministratives/kaenguru-comics/kaenguru-024/original\nadministratives/kaenguru-comics/kaenguru-025/original\nadministratives/kaenguru-comics/kaenguru-026/original\nadministratives/kaenguru-comics/kaenguru-027/original\nadministratives/kaenguru-comics/kaenguru-028/original\nadministratives/kaenguru-comics/kaenguru-029/original\nadministratives/kaenguru-comics/kaenguru-030/original\nadministratives/kaenguru-comics/kaenguru-031/original\nadministratives/kaenguru-comics/kaenguru-032/original\nadministratives/kaenguru-comics/kaenguru-033/original\nadministratives/kaenguru-comics/kaenguru-034/original\nadministratives/kaenguru-comics/kaenguru-035/original\nadministratives/kaenguru-comics/kaenguru-036/original\nadministratives/kaenguru-comics/kaenguru-037/original\nadministratives/kaenguru-comics/kaenguru-038-2/original\nadministratives/kaenguru-comics/kaenguru-039/original\nadministratives/kaenguru-comics/kaenguru-040/original\nadministratives/kaenguru-comics/kaenguru-41/original\nadministratives/kaenguru-comics/kaenguru-42/original\nadministratives/kaenguru-comics/kaenguru-43/original\nadministratives/kaenguru-comics/kaenguru-44/original\nadministratives/kaenguru-comics/kaenguru-045/original\n`;\n    function addLinksToComics(): void {\n        const today = getToday();\n        const date = copyDate(firstDateWithNewLink);\n        while (date.getTime() <= today.getTime()) {\n            comics.push(generateComicLink(date));\n            dateIncreaseByDays(date, 1);\n        }\n    }\n\n    const days: [string, string, string, string, string, string, string] = [\n        \"Sonntag\",\n        \"Montag\",\n        \"Dienstag\",\n        \"Mittwoch\",\n        \"Donnerstag\",\n        \"Freitag\",\n        \"Samstag\",\n    ];\n    // @ts-expect-error TS2322\n    const getDayName = (date: Date): string => days[date.getDay()];\n    const months: [\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n    ] = [\n        \"Januar\",\n        \"Februar\",\n        \"M\u00e4rz\",\n        \"April\",\n        \"Mai\",\n        \"Juni\",\n        \"Juli\",\n        \"August\",\n        \"September\",\n        \"Oktober\",\n        \"November\",\n        \"Dezember\",\n    ];\n    // @ts-expect-error TS2322\n    const getMonthName = (date: Date): string => months[date.getMonth()];\n\n    const getDateString = (date: Date): string => (\n        `Comic von ${getDayName(date)}, dem ${date.getDate()}. ${\n            getMonthName(date)\n        } ${date.getFullYear()}`\n    );\n\n    function removeAllPopups() {\n        for (const node of document.getElementsByClassName(\"popup-container\")) {\n            node.remove();\n        }\n    }\n\n    const currentImgHeader = document.getElementById(\n        \"current-comic-header\",\n    ) as HTMLAnchorElement;\n    const currentImg = document.getElementById(\n        \"current-img\",\n    ) as HTMLImageElement;\n    currentImg.onmouseover = removeAllPopups;\n    // const currentImgContainer = document.getElementById(\"current-img-container\");\n    function setCurrentComic(date: Date) {\n        let link = generateComicLink(date);\n        link = link.startsWith(\"/\") ? link : \"https://img.zeit.de/\" + link;\n        currentImg.src = link;\n        // currentImg.crossOrigin = \"\";\n        currentImgHeader.innerText = \"Neuster \" + getDateString(date) + \":\";\n        currentImgHeader.href = link;\n    }\n\n    const firstDateWithOldLink = getDateBy(2020, 12, 3);\n    const oldLinkRegex =\n        /administratives\\/kaenguru-comics\\/kaenguru-(\\d{2,3})(?:-2)?\\/original\\/?/;\n\n    const firstDateWithNewLink = getDateBy(2021, 1, 19);\n    const newLinkRegex =\n        /administratives\\/kaenguru-comics\\/(\\d{4})-(\\d{2})\\/(\\d{2})\\/original\\/?/;\n\n    const relativeLinkRegex = /\\/static\\/img\\/(\\d{4})-(\\d{1,2})-(\\d{1,2})\\.jpg/;\n\n    function getDateFromLink(link: string): Date | null {\n        for (const reg of [newLinkRegex, relativeLinkRegex]) {\n            // URLs with year, month, day in them as three groups\n            const match = link.toLowerCase().match(reg);\n            if (match && match.length > 3) {\n                return getDateBy(\n                    // @ts-expect-error TS2345\n                    parseInt(match[1]),\n                    // @ts-expect-error TS2345\n                    parseInt(match[2]),\n                    // @ts-expect-error TS2345\n                    parseInt(match[3]),\n                );\n            }\n        }\n        // URLs with incrementing number in them\n        const arr = link.toLowerCase().match(oldLinkRegex);\n        if (arr && arr.length > 1) {\n            // @ts-expect-error TS2345\n            const num = parseInt(arr[1]) - 5;\n            const date = new Date(firstDateWithOldLink.getTime());\n            for (let i = 0; i < num; i++) {\n                date.setTime(\n                    dateIncreaseByDays(date, isSunday(date) ? 2 : 1).getTime(),\n                );\n            }\n            return isSunday(date) ? dateIncreaseByDays(date, 1) : date;\n        }\n        link = link.toLowerCase().trim();\n        switch (link) { // first URLs with special format\n            case \"administratives/kaenguru-comics/pilot-kaenguru/original\":\n                return getDateBy(2020, 11, 29);\n            case \"administratives/kaenguru-comics/pow-kaenguru/original\":\n                return getDateBy(2020, 11, 30);\n            case \"static/img/kaenguru-announcement/original\":\n                return getDateBy(2020, 11, 30);\n            case \"administratives/kaenguru-comics/der-baum-kaenguru/original\":\n                return getDateBy(2020, 12, 1);\n            case \"administratives/kaenguru-comics/warnung-kaenguru/original\":\n                return getDateBy(2020, 12, 2);\n            case \"administratives/2020-12/kaenguru-comics-kaenguru-019/original\":\n                return getDateBy(2020, 12, 19);\n        }\n        for (const arr of wrongLinks) {\n            if (link === arr[1]) {\n                return arr[0];\n            }\n        }\n        return null;\n    }\n\n    const linkFormat = \"administratives/kaenguru-comics/%y-%m/%d/original\";\n\n    function generateComicLink(date: Date): string {\n        for (const arr of wrongLinks) {\n            if (datesEqual(date, arr[0])) {\n                return arr[1];\n            }\n        }\n        const month = (date.getMonth() + 1).toString();\n        const day = date.getDate().toString();\n        return linkFormat\n            .replace(\"%y\", date.getFullYear().toString())\n            .replace(\"%m\", month.length === 2 ? month : \"0\" + month)\n            .replace(\"%d\", day.length === 2 ? day : \"0\" + day);\n    }\n\n    function dateIncreaseByDays(date: Date, days: number): Date {\n        date.setTime(\n            // working in milliseconds\n            date.getTime() + (days * 1000 * 60 * 60 * 24),\n        );\n        date.setHours(6); // to compensate errors through daylight savings time\n        return date;\n    }\n\n    const comicCountToLoadOnCLick = 7;\n    const loadButton = document.getElementById(\"load-button\")!;\n    const list = document.getElementById(\"old-comics-list\")!;\n    let loaded = 0;\n\n    const loadMoreComics = () => {\n        for (let i = 0; i < comicCountToLoadOnCLick; i++) {\n            loaded++;\n            const c = comics.length - loaded;\n            if (c < 0) {\n                break;\n            }\n\n            let link = comics[c];\n            // @ts-expect-error TS2345\n            const date = getDateFromLink(link);\n            if (date === null) {\n                console.error(\"No date found for \" + link);\n                continue;\n            }\n            // @ts-expect-error TS2532\n            link = link.startsWith(\"/\") ? link : \"https://img.zeit.de/\" + link;\n\n            const listItem = document.createElement(\"li\");\n            const header = document.createElement(\"a\");\n            header.classList.add(\"comic-header\");\n            header.innerText = getDateString(date) + \":\";\n            // @ts-expect-error TS2322\n            header.href = link;\n            header.style.fontSize = \"25px\";\n            listItem.appendChild(header);\n            listItem.appendChild(document.createElement(\"br\"));\n            const image = document.createElement(\"img\");\n            image.classList.add(\"normal-img\");\n            // image.crossOrigin = \"\";\n            // @ts-expect-error TS2322\n            image.src = link;\n            image.alt = getDateString(date);\n            image.onclick = () => {\n                createImgPopup(image);\n            };\n            image.onerror = () => {\n                if (isSunday(date)) {\n                    // normally the image is not available on sundays\n                    // so we can remove the image if it is not available\n                    list.removeChild(listItem);\n                } else {\n                    // if the image is not available, display an error message\n                    listItem.append(\" konnte nicht geladen werden.\");\n                }\n            };\n            listItem.appendChild(image);\n            list.appendChild(listItem);\n        }\n\n        if (loaded >= comics.length) {\n            loadButton.style.opacity = \"0\";\n            loadButton.style.visibility = \"invisible\";\n        }\n    };\n    (document.getElementById(\"load-button\")!).onclick = loadMoreComics;\n\n    const createImgPopup = (image: HTMLImageElement) => {\n        removeAllPopups();\n\n        const popupContainer = document.createElement(\"div\");\n        popupContainer.classList.add(\"popup-container\");\n        popupContainer.onmouseleave = () => {\n            popupContainer.remove();\n        };\n        popupContainer.onclick = () => {\n            removeAllPopups();\n        };\n\n        const clone = image.cloneNode(true) as HTMLElement;\n        clone.classList.remove(\"normal-img\");\n        clone.classList.add(\"popup-img\");\n\n        const closeButton = document.createElement(\"img\");\n        closeButton.classList.add(\"close-button\");\n        closeButton.src = \"/static/img/close.svg?v=0\";\n\n        popupContainer.appendChild(clone);\n        popupContainer.appendChild(closeButton);\n        image.parentNode!.appendChild(popupContainer);\n    };\n\n    // add links to comics list\n    comics.concat(links.split(\"\\n\")); // first 50 comics 29.11.2020 - 17.01.21\n    addLinksToComics();\n\n    const today = dateIncreaseByDays(getToday(), 1);\n    setCurrentComic(today);\n    currentImg.onerror = () => {\n        dateIncreaseByDays(today, -1);\n        setCurrentComic(today);\n\n        if (loaded < comicCountToLoadOnCLick) {\n            loaded++;\n        }\n    };\n}\n\nconst startButton = document.getElementById(\"start-button-no_3rd_party\");\nif (startButton !== null) {\n    const contentContainer = document.getElementById(\n        \"comic-content-container\",\n    )!;\n    // no_3rd_party is activated\n    startButton.onclick = () => {\n        startButton.remove();\n        contentContainer.classList.remove(\"hidden\");\n        startLoadingComics();\n    };\n    contentContainer.classList.add(\"hidden\");\n} else {\n    startLoadingComics();\n}\n// @license-end\n"
+        "// @license magnet:?xt=urn:btih:0b31508aeb0634b347b8270c7bee4d411b5d4109&dn=agpl-3.0.txt AGPL-3.0-or-later\nexport {};\n\nfunction startLoadingComics() {\n    const getDateBy = (year: number, month: number, dayOfMonth: number): Date =>\n        new Date(year, month - 1, dayOfMonth, 6, 0, 0, 0);\n    // date with special link format\n    const wrongLinks: [Date, string][] = [\n        [\n            getDateBy(2021, 5, 25),\n            \"administratives/kaenguru-comics/25/original/\",\n        ],\n        [\n            getDateBy(2021, 9, 6),\n            \"administratives/kaenguru-comics/2021-09/6/original/\",\n        ],\n        [\n            getDateBy(2021, 10, 4),\n            \"administratives/kaenguru-comics/2021-10/4/original\",\n        ],\n        [\n            getDateBy(2021, 10, 29),\n            \"administratives/kaenguru-comics/29/original\",\n        ],\n        [\n            getDateBy(2021, 11, 3),\n            \"administratives/kaenguru-comics/2021-11/03-11-21/original\",\n        ],\n        [\n            getDateBy(2021, 12, 6),\n            \"administratives/kaenguru-comics/2021-12/6/original\",\n        ],\n        [\n            getDateBy(2022, 1, 29),\n            \"administratives/kaenguru-comics/2022-01/29-3/original\",\n        ],\n        [\n            getDateBy(2022, 2, 7),\n            \"administratives/kaenguru-comics/08-02-22/original\",\n        ],\n        [\n            getDateBy(2022, 2, 12),\n            \"administratives/kaenguru-comics/12/original\",\n        ],\n        [\n            getDateBy(2022, 2, 14),\n            \"administratives/kaenguru-comics/14/original\",\n        ],\n        [\n            getDateBy(2022, 3, 28),\n            \"administratives/kaenguru-comics/2022-03/kaenguru-2022-03-28/original\",\n        ],\n        [\n            getDateBy(2022, 4, 4),\n            \"administratives/kaenguru-comics/2022-04/4/original\",\n        ],\n        [\n            getDateBy(2022, 5, 9),\n            \"administratives/kaenguru-comics/2022-05/9/original\",\n        ],\n        [\n            getDateBy(2022, 8, 15),\n            \"administratives/kaenguru-comics/2022-08/kaenguru-comics-2022-08-15/original\",\n        ],\n        [\n            getDateBy(2022, 8, 29),\n            \"administratives/kaenguru-comics/2022-08/29-3/original\",\n        ],\n    ];\n\n    const dateEquals = (\n        date: Date,\n        year: number,\n        month: number,\n        dayOfMonth: number,\n    ): boolean => (\n        // check if a date equals another based on year, month, and dayOfMonth\n        date.getFullYear() === year &&\n        date.getMonth() === (month - 1) && // JS is stupid\n        date.getDate() === dayOfMonth\n    );\n\n    const datesEqual = (date1: Date, date2: Date): boolean =>\n        dateEquals(\n            date1,\n            date2.getFullYear(),\n            date2.getMonth() + 1, // JS is stupid\n            date2.getDate(),\n        );\n\n    const isSunday = (date: Date | undefined) => (\n        date &&\n        date.getDay() === 0 &&\n        // exception for 2020-12-20 (sunday) because there was a comic\n        !dateEquals(date, 2020, 12, 20)\n    );\n\n    const copyDate = (date: Date): Date =>\n        getDateBy(date.getFullYear(), date.getMonth() + 1, date.getDate());\n\n    // get today without hours, minutes, seconds and ms\n    const getToday = (): Date => copyDate(new Date());\n\n    const comics: string[] = [];\n\n    const links = `/static/img/2020-11-03.jpg\nadministratives/kaenguru-comics/pilot-kaenguru/original\nadministratives/kaenguru-comics/pow-kaenguru/original\nstatic/img/kaenguru-announcement/original\nadministratives/kaenguru-comics/der-baum-kaenguru/original\nadministratives/kaenguru-comics/warnung-kaenguru/original\nadministratives/kaenguru-comics/kaenguru-005/original\nadministratives/kaenguru-comics/kaenguru-006/original\nadministratives/kaenguru-comics/kaenguru-007/original\nadministratives/kaenguru-comics/kaenguru-008/original\nadministratives/kaenguru-comics/kaenguru-009/original\nadministratives/kaenguru-comics/kaenguru-010/original\nadministratives/kaenguru-comics/kaenguru-011/original\nadministratives/kaenguru-comics/kaenguru-012/original\nadministratives/kaenguru-comics/kaenguru-013/original\nadministratives/kaenguru-comics/kaenguru-014/original\nadministratives/kaenguru-comics/kaenguru-015/original\nadministratives/kaenguru-comics/kaenguru-016/original\nadministratives/kaenguru-comics/kaenguru-017/original\nadministratives/kaenguru-comics/kaenguru-018/original\nadministratives/2020-12/kaenguru-comics-kaenguru-019/original\nadministratives/kaenguru-comics/kaenguru-020/original\nadministratives/kaenguru-comics/kaenguru-021/original\nadministratives/kaenguru-comics/kaenguru-023/original\nadministratives/kaenguru-comics/kaenguru-024/original\nadministratives/kaenguru-comics/kaenguru-025/original\nadministratives/kaenguru-comics/kaenguru-026/original\nadministratives/kaenguru-comics/kaenguru-027/original\nadministratives/kaenguru-comics/kaenguru-028/original\nadministratives/kaenguru-comics/kaenguru-029/original\nadministratives/kaenguru-comics/kaenguru-030/original\nadministratives/kaenguru-comics/kaenguru-031/original\nadministratives/kaenguru-comics/kaenguru-032/original\nadministratives/kaenguru-comics/kaenguru-033/original\nadministratives/kaenguru-comics/kaenguru-034/original\nadministratives/kaenguru-comics/kaenguru-035/original\nadministratives/kaenguru-comics/kaenguru-036/original\nadministratives/kaenguru-comics/kaenguru-037/original\nadministratives/kaenguru-comics/kaenguru-038-2/original\nadministratives/kaenguru-comics/kaenguru-039/original\nadministratives/kaenguru-comics/kaenguru-040/original\nadministratives/kaenguru-comics/kaenguru-41/original\nadministratives/kaenguru-comics/kaenguru-42/original\nadministratives/kaenguru-comics/kaenguru-43/original\nadministratives/kaenguru-comics/kaenguru-44/original\nadministratives/kaenguru-comics/kaenguru-045/original\n`;\n    function addLinksToComics(): void {\n        const today = getToday();\n        const date = copyDate(firstDateWithNewLink);\n        while (date.getTime() <= today.getTime()) {\n            comics.push(generateComicLink(date));\n            dateIncreaseByDays(date, 1);\n        }\n    }\n\n    const days: [string, string, string, string, string, string, string] = [\n        \"Sonntag\",\n        \"Montag\",\n        \"Dienstag\",\n        \"Mittwoch\",\n        \"Donnerstag\",\n        \"Freitag\",\n        \"Samstag\",\n    ];\n    // @ts-expect-error TS2322\n    const getDayName = (date: Date): string => days[date.getDay()];\n    const months: [\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n        string,\n    ] = [\n        \"Januar\",\n        \"Februar\",\n        \"M\u00e4rz\",\n        \"April\",\n        \"Mai\",\n        \"Juni\",\n        \"Juli\",\n        \"August\",\n        \"September\",\n        \"Oktober\",\n        \"November\",\n        \"Dezember\",\n    ];\n    // @ts-expect-error TS2322\n    const getMonthName = (date: Date): string => months[date.getMonth()];\n\n    const getDateString = (date: Date): string => (\n        `Comic von ${getDayName(date)}, dem ${date.getDate()}. ${\n            getMonthName(date)\n        } ${date.getFullYear()}`\n    );\n\n    function removeAllPopups() {\n        for (const node of document.getElementsByClassName(\"popup-container\")) {\n            node.remove();\n        }\n    }\n\n    const currentImgHeader = document.getElementById(\n        \"current-comic-header\",\n    ) as HTMLAnchorElement;\n    const currentImg = document.getElementById(\n        \"current-img\",\n    ) as HTMLImageElement;\n    currentImg.onmouseover = removeAllPopups;\n    // const currentImgContainer = document.getElementById(\"current-img-container\");\n    function setCurrentComic(date: Date) {\n        let link = generateComicLink(date);\n        link = link.startsWith(\"/\") ? link : \"https://img.zeit.de/\" + link;\n        currentImg.src = link;\n        // currentImg.crossOrigin = \"\";\n        currentImgHeader.innerText = \"Neuster \" + getDateString(date) + \":\";\n        currentImgHeader.href = link;\n    }\n\n    const firstDateWithOldLink = getDateBy(2020, 12, 3);\n    const oldLinkRegex =\n        /administratives\\/kaenguru-comics\\/kaenguru-(\\d{2,3})(?:-2)?\\/original\\/?/;\n\n    const firstDateWithNewLink = getDateBy(2021, 1, 19);\n    const newLinkRegex =\n        /administratives\\/kaenguru-comics\\/(\\d{4})-(\\d{2})\\/(\\d{2})\\/original\\/?/;\n\n    const relativeLinkRegex = /\\/static\\/img\\/(\\d{4})-(\\d{1,2})-(\\d{1,2})\\.jpg/;\n\n    function getDateFromLink(link: string): Date | null {\n        for (const reg of [newLinkRegex, relativeLinkRegex]) {\n            // URLs with year, month, day in them as three groups\n            const match = link.toLowerCase().match(reg);\n            if (match && match.length > 3) {\n                return getDateBy(\n                    // @ts-expect-error TS2345\n                    parseInt(match[1]),\n                    // @ts-expect-error TS2345\n                    parseInt(match[2]),\n                    // @ts-expect-error TS2345\n                    parseInt(match[3]),\n                );\n            }\n        }\n        // URLs with incrementing number in them\n        const arr = link.toLowerCase().match(oldLinkRegex);\n        if (arr && arr.length > 1) {\n            // @ts-expect-error TS2345\n            const num = parseInt(arr[1]) - 5;\n            const date = new Date(firstDateWithOldLink.getTime());\n            for (let i = 0; i < num; i++) {\n                date.setTime(\n                    dateIncreaseByDays(date, isSunday(date) ? 2 : 1).getTime(),\n                );\n            }\n            return isSunday(date) ? dateIncreaseByDays(date, 1) : date;\n        }\n        link = link.toLowerCase().trim();\n        switch (link) { // first URLs with special format\n            case \"administratives/kaenguru-comics/pilot-kaenguru/original\":\n                return getDateBy(2020, 11, 29);\n            case \"administratives/kaenguru-comics/pow-kaenguru/original\":\n                return getDateBy(2020, 11, 30);\n            case \"static/img/kaenguru-announcement/original\":\n                return getDateBy(2020, 11, 30);\n            case \"administratives/kaenguru-comics/der-baum-kaenguru/original\":\n                return getDateBy(2020, 12, 1);\n            case \"administratives/kaenguru-comics/warnung-kaenguru/original\":\n                return getDateBy(2020, 12, 2);\n            case \"administratives/2020-12/kaenguru-comics-kaenguru-019/original\":\n                return getDateBy(2020, 12, 19);\n        }\n        for (const arr of wrongLinks) {\n            if (link === arr[1]) {\n                return arr[0];\n            }\n        }\n        return null;\n    }\n\n    const linkFormat = \"administratives/kaenguru-comics/%y-%m/%d/original\";\n\n    function generateComicLink(date: Date): string {\n        for (const arr of wrongLinks) {\n            if (datesEqual(date, arr[0])) {\n                return arr[1];\n            }\n        }\n        const month = (date.getMonth() + 1).toString();\n        const day = date.getDate().toString();\n        return linkFormat\n            .replace(\"%y\", date.getFullYear().toString())\n            .replace(\"%m\", month.length === 2 ? month : \"0\" + month)\n            .replace(\"%d\", day.length === 2 ? day : \"0\" + day);\n    }\n\n    function dateIncreaseByDays(date: Date, days: number): Date {\n        date.setTime(\n            // working in milliseconds\n            date.getTime() + (days * 1000 * 60 * 60 * 24),\n        );\n        date.setHours(6); // to compensate errors through daylight savings time\n        return date;\n    }\n\n    const comicCountToLoadOnCLick = 7;\n    const loadButton = document.getElementById(\"load-button\")!;\n    const list = document.getElementById(\"old-comics-list\")!;\n    let loaded = 0;\n\n    const loadMoreComics = () => {\n        for (let i = 0; i < comicCountToLoadOnCLick; i++) {\n            loaded++;\n            const c = comics.length - loaded;\n            if (c < 0) {\n                break;\n            }\n\n            let link = comics[c];\n            // @ts-expect-error TS2345\n            const date = getDateFromLink(link);\n            if (date === null) {\n                console.error(\"No date found for \" + link);\n                continue;\n            }\n            // @ts-expect-error TS2532\n            link = link.startsWith(\"/\") ? link : \"https://img.zeit.de/\" + link;\n\n            const listItem = document.createElement(\"li\");\n            const header = document.createElement(\"a\");\n            header.classList.add(\"comic-header\");\n            header.innerText = getDateString(date) + \":\";\n            // @ts-expect-error TS2322\n            header.href = link;\n            header.style.fontSize = \"25px\";\n            listItem.appendChild(header);\n            listItem.appendChild(document.createElement(\"br\"));\n            const image = document.createElement(\"img\");\n            image.classList.add(\"normal-img\");\n            // image.crossOrigin = \"\";\n            // @ts-expect-error TS2322\n            image.src = link;\n            image.alt = getDateString(date);\n            image.onclick = () => {\n                createImgPopup(image);\n            };\n            image.onerror = () => {\n                if (isSunday(date)) {\n                    // normally the image is not available on sundays\n                    // so we can remove the image if it is not available\n                    list.removeChild(listItem);\n                } else {\n                    // if the image is not available, display an error message\n                    listItem.append(\" konnte nicht geladen werden.\");\n                }\n            };\n            listItem.appendChild(image);\n            list.appendChild(listItem);\n        }\n\n        if (loaded >= comics.length) {\n            loadButton.style.opacity = \"0\";\n            loadButton.style.visibility = \"invisible\";\n        }\n    };\n    (document.getElementById(\"load-button\")!).onclick = loadMoreComics;\n\n    const createImgPopup = (image: HTMLImageElement) => {\n        removeAllPopups();\n\n        const popupContainer = document.createElement(\"div\");\n        popupContainer.classList.add(\"popup-container\");\n        popupContainer.onmouseleave = () => {\n            popupContainer.remove();\n        };\n        popupContainer.onclick = () => {\n            removeAllPopups();\n        };\n\n        const clone = image.cloneNode(true) as HTMLElement;\n        clone.classList.remove(\"normal-img\");\n        clone.classList.add(\"popup-img\");\n\n        const closeButton = document.createElement(\"img\");\n        closeButton.classList.add(\"close-button\");\n        closeButton.src = \"/static/img/close.svg?v=0\";\n\n        popupContainer.appendChild(clone);\n        popupContainer.appendChild(closeButton);\n        image.parentNode!.appendChild(popupContainer);\n    };\n\n    // add links to comics list\n    comics.push(...links.split(\"\\n\")); // first 50 comics 29.11.2020 - 17.01.21\n    addLinksToComics();\n\n    const today = dateIncreaseByDays(getToday(), 1);\n    setCurrentComic(today);\n    currentImg.onerror = () => {\n        dateIncreaseByDays(today, -1);\n        setCurrentComic(today);\n\n        if (loaded < comicCountToLoadOnCLick) {\n            loaded++;\n        }\n    };\n}\n\nconst startButton = document.getElementById(\"start-button-no_3rd_party\");\nif (startButton !== null) {\n    const contentContainer = document.getElementById(\n        \"comic-content-container\",\n    )!;\n    // no_3rd_party is activated\n    startButton.onclick = () => {\n        startButton.remove();\n        contentContainer.classList.remove(\"hidden\");\n        startLoadingComics();\n    };\n    contentContainer.classList.add(\"hidden\");\n} else {\n    startLoadingComics();\n}\n// @license-end\n"
     ],
     "version": 3
 }
```

### Comparing `an-website-24.4/an_website/static/js/quotes/create.js.map` & `an-website-24.5/an_website/static/js/quotes/create.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/quotes/quotes.js` & `an-website-24.5/an_website/static/js/quotes/quotes.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/quotes/quotes.js.map` & `an-website-24.5/an_website/static/js/quotes/quotes.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/search/search.js` & `an-website-24.5/an_website/static/js/search/search.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/search/search.js.map` & `an-website-24.5/an_website/static/js/search/search.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/settings/settings.js` & `an-website-24.5/an_website/static/js/settings/settings.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/settings/settings.js.map` & `an-website-24.5/an_website/static/js/settings/settings.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/snow/snow.js` & `an-website-24.5/an_website/static/js/snow/snow.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/snow/snow.js.map` & `an-website-24.5/an_website/static/js/snow/snow.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/swapped_words/swap.js` & `an-website-24.5/an_website/static/js/swapped_words/swap.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/swapped_words/swap.js.map` & `an-website-24.5/an_website/static/js/swapped_words/swap.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/uptime/uptime.js` & `an-website-24.5/an_website/static/js/uptime/uptime.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/uptime/uptime.js.map` & `an-website-24.5/an_website/static/js/uptime/uptime.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/utils/better_ui.js` & `an-website-24.5/an_website/static/js/utils/better_ui.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/utils/better_ui.js.map` & `an-website-24.5/an_website/static/js/utils/better_ui.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/utils/dynload.js` & `an-website-24.5/an_website/static/js/utils/dynload.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/utils/dynload.js.map` & `an-website-24.5/an_website/static/js/utils/dynload.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/utils/utils.js` & `an-website-24.5/an_website/static/js/utils/utils.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/utils/utils.js.map` & `an-website-24.5/an_website/static/js/utils/utils.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/vendored/vanilla.js` & `an-website-24.5/an_website/static/js/vendored/vanilla.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/static/js/vendored/vanilla.js.map` & `an-website-24.5/an_website/static/js/vendored/vanilla.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/swapped_words/__init__.py` & `an-website-24.5/an_website/swapped_words/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/swapped_words/config.sw` & `an-website-24.5/an_website/swapped_words/config.sw`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/swapped_words/config_file.py` & `an-website-24.5/an_website/swapped_words/config_file.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/swapped_words/swap.py` & `an-website-24.5/an_website/swapped_words/swap.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/ansi2html.html` & `an-website-24.5/an_website/templates/ansi2html.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/base.html` & `an-website-24.5/an_website/templates/base.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/error.html` & `an-website-24.5/an_website/templates/error.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/footer.html` & `an-website-24.5/an_website/templates/footer.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 <footer id="footer" data-elastic-exclude>Mit Liebe gebacken
     {% if globals()["🦘"] %}
-        {% raw emoji2html("🦘") %}
+        {% if now.isoweekday() == 3 %}
+            <span tooltip="What a week, huh?">{% raw emoji2html("🦘") %}</span>
+        {% else %}
+            {% raw emoji2html("🦘") %}
+        {% end %}
     {% elif now.microsecond % 4 == 3 and now.weekday() == 2 %}
         <span tooltip="ribbit">{% raw emoji2html("🐸") %}</span>
     {% elif globals()["🥚"] %}
         <a href="{{fix_url('https://bibliogram.froth.zone/p/BsOGulcndj-')}}"
            class="no-style-a-emoji">{% raw emoji2html("🥚") %}</a>
     {% elif now.month == now.day %}
         {% raw emoji2html(("🥇", "🥈", "🔱", "🍀", "🖐️", "🔯", "🎰", "✴️", "9⃣", "🔟", "🧝", "🕛️")[now.month - 1]) %}
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
-Mit Liebe gebacken {% if globals()["ð¦"] %} {% raw emoji2html("ð¦") %} {%
+Mit Liebe gebacken {% if globals()["ð¦"] %} {% if now.isoweekday() == 3 %} {%
+raw emoji2html("ð¦") %} {% else %} {% raw emoji2html("ð¦") %} {% end %} {%
 elif now.microsecond % 4 == 3 and now.weekday() == 2 %} {% raw emoji2html
 ("ð¸") %} {% elif globals()["ð¥"] %} _{_%_ _r_a_w_ _e_m_o_j_i_2_h_t_m_l_(_"_ð__¥__"_)_ _%_} {% elif
 now.month == now.day %} {% raw emoji2html(("ð¥", "ð¥", "ð±", "ð",
 "ðï¸", "ð¯", "ð°", "â´ï¸", "9â£", "ð", "ð§", "ðï¸")
 [now.month - 1]) %} {% elif now.month == 2 and now.day == 29 %} {% raw
 emoji2html("ð«") %} {% elif now.month == 3 and now.day == 8 %} {% raw
 emoji2html("âï¸") %} {% elif now.month == 3 and now.day == 14 %} {% raw
```

### Comparing `an-website-24.4/an_website/templates/header.html` & `an-website-24.5/an_website/templates/header.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/contact.html` & `an-website-24.5/an_website/templates/pages/contact.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/converter.html` & `an-website-24.5/an_website/templates/pages/converter.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/emoji_chat.html` & `an-website-24.5/an_website/templates/pages/emoji_chat.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/endpoints.html` & `an-website-24.5/an_website/templates/pages/endpoints.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/hangman_solver.html` & `an-website-24.5/an_website/templates/pages/hangman_solver.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/js_licenses.html` & `an-website-24.5/an_website/templates/pages/js_licenses.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/kangaroo_comics.html` & `an-website-24.5/an_website/templates/pages/kangaroo_comics.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/main_page.html` & `an-website-24.5/an_website/templates/pages/main_page.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/quotes/create1.html` & `an-website-24.5/an_website/templates/pages/quotes/create1.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/quotes/create2.html` & `an-website-24.5/an_website/templates/pages/quotes/create2.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/quotes/generator.html` & `an-website-24.5/an_website/templates/pages/quotes/generator.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/quotes/info.html` & `an-website-24.5/an_website/templates/pages/quotes/info.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/quotes/main_page.html` & `an-website-24.5/an_website/templates/pages/quotes/main_page.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/quotes/quotes.html` & `an-website-24.5/an_website/templates/pages/quotes/quotes.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/quotes/share.html` & `an-website-24.5/an_website/templates/pages/quotes/share.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/redirect.html` & `an-website-24.5/an_website/templates/pages/redirect.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/search.html` & `an-website-24.5/an_website/templates/pages/search.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/services.html` & `an-website-24.5/an_website/templates/pages/services.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/settings.html` & `an-website-24.5/an_website/templates/pages/settings.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/soundboard.html` & `an-website-24.5/an_website/templates/pages/soundboard.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/swapped_words.html` & `an-website-24.5/an_website/templates/pages/swapped_words.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/troet.html` & `an-website-24.5/an_website/templates/pages/troet.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/uptime.html` & `an-website-24.5/an_website/templates/pages/uptime.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/version.html` & `an-website-24.5/an_website/templates/pages/version.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/pages/wordgame_solver.html` & `an-website-24.5/an_website/templates/pages/wordgame_solver.html`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/templates/rss/quote_of_the_day.xml` & `an-website-24.5/an_website/templates/rss/quote_of_the_day.xml`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/troet/__init__.py` & `an-website-24.5/an_website/troet/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/troet/troet.py` & `an-website-24.5/an_website/troet/troet.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/update/__init__.py` & `an-website-24.5/an_website/update/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/update/update.py` & `an-website-24.5/an_website/update/update.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/uptime/__init__.py` & `an-website-24.5/an_website/uptime/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/uptime/uptime.py` & `an-website-24.5/an_website/uptime/uptime.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/__init__.py` & `an-website-24.5/an_website/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/base_request_handler.py` & `an-website-24.5/an_website/utils/base_request_handler.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/better_config_parser.py` & `an-website-24.5/an_website/utils/better_config_parser.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/data_parsing.py` & `an-website-24.5/an_website/utils/data_parsing.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/decorators.py` & `an-website-24.5/an_website/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/logging.py` & `an-website-24.5/an_website/utils/logging.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/options.py` & `an-website-24.5/an_website/utils/options.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/request_handler.py` & `an-website-24.5/an_website/utils/request_handler.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/search.py` & `an-website-24.5/an_website/utils/search.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/static_file_from_traversable.py` & `an-website-24.5/an_website/utils/static_file_from_traversable.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/static_file_handling.py` & `an-website-24.5/an_website/utils/static_file_handling.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/token.py` & `an-website-24.5/an_website/utils/token.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/utils/utils.py` & `an-website-24.5/an_website/utils/utils.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/vendored/apm-rum/elastic-apm-rum.umd.js` & `an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js` & `an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js.map` & `an-website-24.5/an_website/vendored/apm-rum/elastic-apm-rum.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/vendored/media-types.json` & `an-website-24.5/an_website/vendored/media-types.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/vendored/mime-db.json` & `an-website-24.5/an_website/vendored/mime-db.json`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/vendored/screenfetch` & `an-website-24.5/an_website/vendored/screenfetch`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/version/__init__.py` & `an-website-24.5/an_website/version/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/version/version.py` & `an-website-24.5/an_website/version/version.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/whats_my_ip/__init__.py` & `an-website-24.5/an_website/whats_my_ip/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/whats_my_ip/ip.py` & `an-website-24.5/an_website/whats_my_ip/ip.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/wiki/__init__.py` & `an-website-24.5/an_website/wiki/__init__.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website/wiki/wiki.py` & `an-website-24.5/an_website/wiki/wiki.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website.egg-info/PKG-INFO` & `an-website-24.5/an_website.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: an-website
-Version: 24.4
+Version: 24.5
 Summary: #1 Website in the Worlds
 Home-page: https://github.com/asozialesnetzwerk/an-website
 Author: Das Asoziale Netzwerk
 Author-email: contact@asozial.org
 License: AGPL-3.0-or-later
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,70 +15,70 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: accept-types==0.4.1
 Requires-Dist: aiodns==3.2.0
-Requires-Dist: aiohttp[speedups]==3.9.3; python_version >= "3.8"
+Requires-Dist: aiohttp[speedups]==3.9.5; python_version >= "3.8"
 Requires-Dist: aiosignal==1.3.1; python_version >= "3.7"
 Requires-Dist: ansi2html==1.9.1; python_version >= "3.7"
 Requires-Dist: async-timeout==4.0.3; python_full_version < "3.11.3"
 Requires-Dist: attrs==23.2.0; python_version >= "3.7"
 Requires-Dist: beautifulsoup4==4.12.3; python_full_version >= "3.6.0"
 Requires-Dist: blake3==0.4.1
 Requires-Dist: brotli==1.1.0
 Requires-Dist: certifi==2023.11.17; python_version >= "3.6"
 Requires-Dist: cffi==1.16.0; python_version >= "3.8"
 Requires-Dist: defity==0.3.1; python_version >= "3.7"
 Requires-Dist: defusedxml==0.7.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
 Requires-Dist: dill==0.3.8; python_version >= "3.8"
-Requires-Dist: dunamai==1.19.2; python_version >= "3.5"
+Requires-Dist: dunamai==1.21.1; python_version >= "3.5"
 Requires-Dist: ecs-logging==2.1.0; python_version >= "3.6"
-Requires-Dist: elastic-apm==6.21.4.post8347027212; python_version >= "3.6" and python_version < "4"
+Requires-Dist: elastic-apm==6.22.0; python_version >= "3.6" and python_version < "4"
 Requires-Dist: elastic-enterprise-search==8.11.0; python_version >= "3.6"
 Requires-Dist: elastic-transport==8.13.0; python_version >= "3.7"
 Requires-Dist: elasticsearch[async]==8.12.1; python_version >= "3.7"
-Requires-Dist: emoji==2.11.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
+Requires-Dist: emoji==2.11.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: frozenlist==1.4.1; python_version >= "3.8"
 Requires-Dist: funcparserlib==1.0.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6" and python_version < "3.13"
 Requires-Dist: get-version==3.5.5; python_version >= "3.9"
 Requires-Dist: hangman-solver-rs==0.2.1; python_version >= "3.10"
 Requires-Dist: hiredis==2.3.2
 Requires-Dist: html2text==2020.1.16; python_version >= "3.5"
 Requires-Dist: hy==0.28.0; python_version < "3.13" and python_version >= "3.8"
 Requires-Dist: hyrule==0.5.0; python_version < "3.13"
-Requires-Dist: idna==3.6; python_version >= "3.5"
-Requires-Dist: jsonpickle==3.0.3; python_version >= "3.7"
-Requires-Dist: lxml==5.2.0; python_version >= "3.6"
+Requires-Dist: idna==3.7; python_version >= "3.5"
+Requires-Dist: jsonpickle==3.0.4; python_version >= "3.7"
+Requires-Dist: lxml==5.2.2; python_version >= "3.6"
 Requires-Dist: multidict==6.0.5; python_version >= "3.7"
 Requires-Dist: openmoji-dist==15.0.0.1
-Requires-Dist: orjson==3.10.0; python_version >= "3.8"
+Requires-Dist: orjson==3.10.3; python_version >= "3.8"
 Requires-Dist: packaging==23.2; python_version >= "3.7"
-Requires-Dist: pillow==10.2.0; python_version >= "3.8"
-Requires-Dist: pillow-jxl-plugin==1.2.2; python_version >= "3.8"
+Requires-Dist: pillow==10.3.0; python_version >= "3.8"
+Requires-Dist: pillow-jxl-plugin==1.2.4; python_version >= "3.8"
 Requires-Dist: pycares==4.4.0; python_version >= "3.8"
 Requires-Dist: pycparser==2.22; python_version >= "3.8"
 Requires-Dist: pycryptodome==3.20.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
 Requires-Dist: pycurl==7.45.2; python_version >= "3.5"
 Requires-Dist: pyjwt==2.8.0; python_version >= "3.7"
 Requires-Dist: pysocks==1.7.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-dateutil==2.9.0.post0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: python-geoip-geolite2-yplan==2019.1224
 Requires-Dist: python-geoip-yplan==1.2
 Requires-Dist: pytz==2023.4
 Requires-Dist: pyyaml==6.0.1; python_version >= "3.6"
-Requires-Dist: rapidfuzz==3.7.0; python_version >= "3.8"
-Requires-Dist: redis[hiredis]==5.0.3; python_version >= "3.7"
+Requires-Dist: rapidfuzz==3.9.0; python_version >= "3.8"
+Requires-Dist: redis[hiredis]==5.0.4; python_version >= "3.7"
 Requires-Dist: regex==2023.12.25; python_version >= "3.7"
 Requires-Dist: setproctitle==1.3.3; python_version >= "3.7"
 Requires-Dist: six==1.16.0; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"
 Requires-Dist: soupsieve==2.5; python_version >= "3.8"
 Requires-Dist: tornado==6.4; python_version >= "3.8"
-Requires-Dist: typed-stream==0.69.0; python_version >= "3.10"
+Requires-Dist: typed-stream==0.131.0; python_version >= "3.10"
 Requires-Dist: tzdata==2023.4; python_version >= "2"
 Requires-Dist: ultradict==0.0.6; python_version >= "3.8"
 Requires-Dist: urllib3==2.2.1; python_version >= "3.8"
 Requires-Dist: uvloop==0.19.0; python_full_version >= "3.8.0"
 Requires-Dist: wrapt==1.14.1; python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"
 Requires-Dist: yarl==1.9.4; python_version >= "3.7"
```

### Comparing `an-website-24.4/an_website.egg-info/SOURCES.txt` & `an-website-24.5/an_website.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `an-website-24.4/an_website.egg-info/requires.txt` & `an-website-24.5/an_website.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,74 +23,74 @@
 [:python_version < "3.13" and python_version >= "3.8"]
 hy==0.28.0
 
 [:python_version >= "2"]
 tzdata==2023.4
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3"]
-emoji==2.11.0
+emoji==2.11.1
 pysocks==1.7.1
 python-dateutil==2.9.0.post0
 six==1.16.0
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4"]
 defusedxml==0.7.1
 pycryptodome==3.20.0
 wrapt==1.14.1
 
 [:python_version >= "2.7" and python_version not in "3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6" and python_version < "3.13"]
 funcparserlib==1.0.1
 
 [:python_version >= "3.10"]
 hangman-solver-rs==0.2.1
-typed-stream==0.69.0
+typed-stream==0.131.0
 
 [:python_version >= "3.5"]
-dunamai==1.19.2
+dunamai==1.21.1
 html2text==2020.1.16
-idna==3.6
+idna==3.7
 pycurl==7.45.2
 
 [:python_version >= "3.6"]
 certifi==2023.11.17
 ecs-logging==2.1.0
 elastic-enterprise-search==8.11.0
-lxml==5.2.0
+lxml==5.2.2
 pyyaml==6.0.1
 
 [:python_version >= "3.6" and python_version < "4"]
-elastic-apm==6.21.4.post8347027212
+elastic-apm==6.22.0
 
 [:python_version >= "3.7"]
 aiosignal==1.3.1
 ansi2html==1.9.1
 attrs==23.2.0
 defity==0.3.1
 elastic-transport==8.13.0
 elasticsearch[async]==8.12.1
-jsonpickle==3.0.3
+jsonpickle==3.0.4
 multidict==6.0.5
 packaging==23.2
 pyjwt==2.8.0
-redis[hiredis]==5.0.3
+redis[hiredis]==5.0.4
 regex==2023.12.25
 setproctitle==1.3.3
 yarl==1.9.4
 
 [:python_version >= "3.8"]
-aiohttp[speedups]==3.9.3
+aiohttp[speedups]==3.9.5
 cffi==1.16.0
 dill==0.3.8
 frozenlist==1.4.1
-orjson==3.10.0
-pillow==10.2.0
-pillow-jxl-plugin==1.2.2
+orjson==3.10.3
+pillow==10.3.0
+pillow-jxl-plugin==1.2.4
 pycares==4.4.0
 pycparser==2.22
-rapidfuzz==3.7.0
+rapidfuzz==3.9.0
 soupsieve==2.5
 tornado==6.4
 ultradict==0.0.6
 urllib3==2.2.1
 
 [:python_version >= "3.9"]
 get-version==3.5.5
```

### Comparing `an-website-24.4/build-oci-image.sh` & `an-website-24.5/build-oci-image.sh`

 * *Files identical despite different names*

### Comparing `an-website-24.4/example-configurations/config.ini.default` & `an-website-24.5/example-configurations/config.ini.default`

 * *Files identical despite different names*

### Comparing `an-website-24.4/example-configurations/config.ini.example` & `an-website-24.5/example-configurations/config.ini.example`

 * *Files identical despite different names*

### Comparing `an-website-24.4/example-configurations/nginx/an-website.conf` & `an-website-24.5/example-configurations/nginx/an-website.conf`

 * *Files identical despite different names*

### Comparing `an-website-24.4/pip-requirements.txt` & `an-website-24.5/pip-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 accept-types==0.4.1
 aiodns==3.2.0
-aiohttp[speedups]==3.9.3; python_version >= '3.8'
+aiohttp[speedups]==3.9.5; python_version >= '3.8'
 aiosignal==1.3.1; python_version >= '3.7'
 ansi2html==1.9.1; python_version >= '3.7'
 async-timeout==4.0.3; python_full_version < '3.11.3'
 attrs==23.2.0; python_version >= '3.7'
 beautifulsoup4==4.12.3; python_full_version >= '3.6.0'
 blake3==0.4.1
 brotli==1.1.0
 certifi==2023.11.17; python_version >= '3.6'
 cffi==1.16.0; python_version >= '3.8'
 defity==0.3.1; python_version >= '3.7'
 defusedxml==0.7.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
 dill==0.3.8; python_version >= '3.8'
-dunamai==1.19.2; python_version >= '3.5'
+dunamai==1.21.1; python_version >= '3.5'
 ecs-logging==2.1.0; python_version >= '3.6'
-elastic-apm==6.21.4.post8347027212; python_version >= '3.6' and python_version < '4'
+elastic-apm==6.22.0; python_version >= '3.6' and python_version < '4'
 elastic-enterprise-search==8.11.0; python_version >= '3.6'
 elastic-transport==8.13.0; python_version >= '3.7'
 elasticsearch[async]==8.12.1; python_version >= '3.7'
-emoji==2.11.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
+emoji==2.11.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 frozenlist==1.4.1; python_version >= '3.8'
 funcparserlib==1.0.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6' and python_version < '3.13'
 get-version==3.5.5; python_version >= '3.9'
 hangman-solver-rs==0.2.1; python_version >= '3.10'
 hiredis==2.3.2
 html2text==2020.1.16; python_version >= '3.5'
 hy==0.28.0; python_version < '3.13' and python_version >= '3.8'
 hyrule==0.5.0; python_version < '3.13'
-idna==3.6; python_version >= '3.5'
-jsonpickle==3.0.3; python_version >= '3.7'
-lxml==5.2.0; python_version >= '3.6'
+idna==3.7; python_version >= '3.5'
+jsonpickle==3.0.4; python_version >= '3.7'
+lxml==5.2.2; python_version >= '3.6'
 multidict==6.0.5; python_version >= '3.7'
 openmoji-dist==15.0.0.1
-orjson==3.10.0; python_version >= '3.8'
+orjson==3.10.3; python_version >= '3.8'
 packaging==23.2; python_version >= '3.7'
-pillow==10.2.0; python_version >= '3.8'
-pillow-jxl-plugin==1.2.2; python_version >= '3.8'
+pillow==10.3.0; python_version >= '3.8'
+pillow-jxl-plugin==1.2.4; python_version >= '3.8'
 pycares==4.4.0; python_version >= '3.8'
 pycparser==2.22; python_version >= '3.8'
 pycryptodome==3.20.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
 pycurl==7.45.2; python_version >= '3.5'
 pyjwt==2.8.0; python_version >= '3.7'
 pysocks==1.7.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 python-dateutil==2.9.0.post0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 python-geoip-geolite2-yplan==2019.1224
 python-geoip-yplan==1.2
 pytz==2023.4
 pyyaml==6.0.1; python_version >= '3.6'
-rapidfuzz==3.7.0; python_version >= '3.8'
-redis[hiredis]==5.0.3; python_version >= '3.7'
+rapidfuzz==3.9.0; python_version >= '3.8'
+redis[hiredis]==5.0.4; python_version >= '3.7'
 regex==2023.12.25; python_version >= '3.7'
 setproctitle==1.3.3; python_version >= '3.7'
 six==1.16.0; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 soupsieve==2.5; python_version >= '3.8'
 tornado==6.4; python_version >= '3.8'
-typed-stream==0.69.0; python_version >= '3.10'
+typed-stream==0.131.0; python_version >= '3.10'
 tzdata==2023.4; python_version >= '2'
 ultradict==0.0.6; python_version >= '3.8'
 urllib3==2.2.1; python_version >= '3.8'
 uvloop==0.19.0; python_full_version >= '3.8.0'
 wrapt==1.14.1; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
 yarl==1.9.4; python_version >= '3.7'
```

### Comparing `an-website-24.4/pyproject.toml` & `an-website-24.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -18,27 +18,28 @@
 add_imports = ["from __future__ import annotations"]
 
 [tool.mypy]
 strict = true
 sqlite_cache = true
 python_version = "3.12"
 warn_unreachable = true
-# disallow_any_decorated = true
-# disallow_any_explicit = true
 # disallow_any_expr = true
+# disallow_any_explicit = true
+# disallow_any_decorated = true
 disallow_any_unimported = true
 plugins = "numpy.typing.mypy_plugin"
 enable_error_code = [
   # "explicit-override",
   "ignore-without-code",
   "possibly-undefined",
   "redundant-expr",
   "redundant-self",
   "truthy-bool",
   "truthy-iterable",
   "unused-awaitable",
 ]
+local_partial_types = true
 disable_bytearray_promotion = true
 disable_memoryview_promotion = true
 enable_incomplete_feature = ["PreciseTupleTypes"]
 packages = ["an_website", "tests", "scripts"]
 modules = "setup"
```

### Comparing `an-website-24.4/setup.py` & `an-website-24.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,17 @@
 from pathlib import Path
 from warnings import filterwarnings
 
 from setuptools import setup
 from setuptools.build_meta import SetupRequirementsError
 
 BACKEND_REQUIRES = set()
-DULWICH = "dulwich==0.21.7"
+DULWICH = "dulwich==0.22.1"
 GET_VERSION = "get_version==3.5.5"
-TROVE_CLASSIFIERS = "trove-classifiers==2024.1.8"
+TROVE_CLASSIFIERS = "trove-classifiers"
 
 filterwarnings("ignore", "", UserWarning, "setuptools.dist")
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     (
         "License :: OSI Approved :: "
```

### Comparing `an-website-24.4/tests/test_backdoor.py` & `an-website-24.5/tests/test_backdoor.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_christmas.py` & `an-website-24.5/tests/test_christmas.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_commitment.py` & `an-website-24.5/tests/test_commitment.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_contact.py` & `an-website-24.5/tests/test_contact.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_currency_converter.py` & `an-website-24.5/tests/test_currency_converter.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_hangman_solver.py` & `an-website-24.5/tests/test_hangman_solver.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_main.py` & `an-website-24.5/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_permissions.py` & `an-website-24.5/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_quotes.py` & `an-website-24.5/tests/test_quotes.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,17 +70,17 @@
     assert quote == await quotes.get_quote_by_id(quote_id=quote.id)
     assert quote.id == 1
     assert quote.author.id == 1
 
     assert await quotes.get_rating_by_id(1, 2) == 4
 
     assert len(quotes.QUOTES_CACHE) == 1
-    assert quotes.MAX_QUOTES_ID.value == 1  # type: ignore[attr-defined]
+    assert quotes.MAX_QUOTES_ID.value == 1
     assert len(quotes.AUTHORS_CACHE) == 2
-    assert quotes.MAX_AUTHORS_ID.value == 2  # type: ignore[attr-defined]
+    assert quotes.MAX_AUTHORS_ID.value == 2
 
 
 def test_author_updating() -> None:
     """Test updating the author."""
     get_wrong_quote()
 
     assert (author := quotes.get_author_updated_with(1, "test")).name == "test"
@@ -137,15 +137,15 @@
 
 async def test_argument_checking_create_pages(
     fetch: FetchCallable,  # noqa: F811
 ) -> None:
     """Test whether the create handlers complain because of missing args."""
     wrong_quote = get_wrong_quote()
 
-    await quotes.make_api_request("/test")
+    await quotes.make_api_request("/test", entity_should_exist=False)
 
     for data in (
         "quote-1=&fake-author-1=",
         "quote-1=test&fake-author-1=",
         "quote-1=&fake-author-1=test",
         "x=y",
     ):
```

### Comparing `an-website-24.4/tests/test_random_text.py` & `an-website-24.5/tests/test_random_text.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_request_handlers.py` & `an-website-24.5/tests/test_request_handlers.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_settings.py` & `an-website-24.5/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_swapped_words.py` & `an-website-24.5/tests/test_swapped_words.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_token.py` & `an-website-24.5/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_traversable_static_file_handler.py` & `an-website-24.5/tests/test_traversable_static_file_handler.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_troet.py` & `an-website-24.5/tests/test_troet.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_uptime.py` & `an-website-24.5/tests/test_uptime.py`

 * *Files identical despite different names*

### Comparing `an-website-24.4/tests/test_utils.py` & `an-website-24.5/tests/test_utils.py`

 * *Files identical despite different names*

