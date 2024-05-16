# Comparing `tmp/bbot-1.1.7.7rc0.tar.gz` & `tmp/bbot-1.1.8.3321rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.1.7.7rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.8.3321rc0.tar", max compression
```

## Comparing `bbot-1.1.7.7rc0.tar` & `bbot-1.1.8.3321rc0.tar`

### file list

```diff
@@ -1,339 +1,346 @@
--rw-r--r--   0        0        0    32473 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/LICENSE
--rw-r--r--   0        0        0    37988 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/README.md
--rw-r--r--   0        0        0      208 2024-03-22 20:11:21.669284 bbot-1.1.7.7rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7898 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    17601 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/cli.py
--rw-r--r--   0        0        0       59 2024-03-22 20:11:00.297268 bbot-1.1.7.7rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3588 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     9843 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5182 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1341 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      617 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/errors.py
--rw-r--r--   0        0        0       91 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    45979 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1656 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0     1183 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/flags.py
--rw-r--r--   0        0        0       86 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3583 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     1537 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     4341 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/cloud.py
--rw-r--r--   0        0        0    10930 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14117 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9199 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    47786 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     5639 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     6354 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0    12632 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    82517 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    22071 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0    10041 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0     1990 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     3463 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     5947 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     8781 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    31592 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    19801 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0      191 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8118 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     4148 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     2328 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/ajaxpro.py
--rw-r--r--   0        0        0     1824 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     1372 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/azure_realm.py
--rw-r--r--   0        0        0     4691 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     4150 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/baddns.py
--rw-r--r--   0        0        0     1245 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/baddns_zone.py
--rw-r--r--   0        0        0     3549 2024-03-22 20:11:00.301268 bbot-1.1.7.7rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    59062 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2352 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1299 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0      655 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_amazon.py
--rw-r--r--   0        0        0     1020 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      775 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1915 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_file_enum.py
--rw-r--r--   0        0        0     1352 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2540 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bucket_google.py
--rw-r--r--   0        0        0     4911 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     6553 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1188 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3371 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      798 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     1522 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/chaos.py
--rw-r--r--   0        0        0      735 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     3297 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/credshed.py
--rw-r--r--   0        0        0      376 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1230 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0     5220 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/deadly/dastardly.py
--rw-r--r--   0        0        0    14079 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    17188 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5239 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     3928 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dehashed.py
--rw-r--r--   0        0        0      930 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/digitorus.py
--rw-r--r--   0        0        0     5324 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     3186 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     3247 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dockerhub.py
--rw-r--r--   0        0        0     9245 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/dotnetnuke.py
--rw-r--r--   0        0        0      791 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11758 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     7502 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/filedownload.py
--rw-r--r--   0        0        0     2184 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1195 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7794 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1319 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2073 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/git_clone.py
--rw-r--r--   0        0        0     3135 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/github_codesearch.py
--rw-r--r--   0        0        0     8664 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/github_org.py
--rw-r--r--   0        0        0    11415 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      890 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7172 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     6758 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5990 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2098 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0    13124 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    18687 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     7448 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     4384 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/internetdb.py
--rw-r--r--   0        0        0     2123 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/ip2location.py
--rw-r--r--   0        0        0     1539 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     1767 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1541 2024-03-22 20:11:00.305269 bbot-1.1.7.7rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    10816 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    21031 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      857 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     2281 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/newsletters.py
--rw-r--r--   0        0        0     5506 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     4731 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0     5852 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/oauth.py
--rw-r--r--   0        0        0      774 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    14731 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     3268 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2604 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0      531 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/discord.py
--rw-r--r--   0        0        0      985 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/emails.py
--rw-r--r--   0        0        0     2182 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1907 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1375 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1482 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     1117 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/slack.py
--rw-r--r--   0        0        0     1886 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/splunk.py
--rw-r--r--   0        0        0     1430 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/subdomains.py
--rw-r--r--   0        0        0      723 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/teams.py
--rw-r--r--   0        0        0     3627 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2218 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1689 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     9461 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1619 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1420 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0     5479 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/postman.py
--rw-r--r--   0        0        0      832 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8456 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      828 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2025 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2898 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1201 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0      792 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1993 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/sitedossier.py
--rw-r--r--   0        0        0     1478 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1408 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1769 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7822 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     1327 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/subdomaincenter.py
--rw-r--r--   0        0        0      553 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    17041 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0     5642 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/bucket.py
--rw-r--r--   0        0        0     1308 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/github.py
--rw-r--r--   0        0        0     2436 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/portscanner.py
--rw-r--r--   0        0        0     1182 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/shodan.py
--rw-r--r--   0        0        0     6100 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/subdomain_enum.py
--rw-r--r--   0        0        0     3789 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/templates/webhook.py
--rw-r--r--   0        0        0      678 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     4348 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/trufflehog.py
--rw-r--r--   0        0        0     4102 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2992 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2325 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1591 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     2010 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1272 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2871 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2337 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    29339 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    41838 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3049 2024-03-22 20:11:00.309269 bbot-1.1.7.7rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0    11073 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/scanner/target.py
--rwxr-xr-x   0        0        0     5889 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/scripts/docs.py
--rw-r--r--   0        0        0        0 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    12418 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     4870 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0       31 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/coverage.cfg
--rwxr-xr-x   0        0        0      652 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1091 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      323 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_output.ndjson
--rw-r--r--   0        0        0        0 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5523 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6544 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0     3808 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     5853 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     7572 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0       79 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_docs.py
--rw-r--r--   0        0        0    22219 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    31826 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0    16305 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_manager_deduplication.py
--rw-r--r--   0        0        0    77598 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
--rw-r--r--   0        0        0    16717 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     2657 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     7144 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_regexes.py
--rw-r--r--   0        0        0     2884 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2148 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0    13141 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     5344 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      664 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      473 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0     2789 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
--rw-r--r--   0        0        0      546 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     3098 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1207 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
--rw-r--r--   0        0        0     4805 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     2795 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
--rw-r--r--   0        0        0     2397 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
--rw-r--r--   0        0        0     5599 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3984 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
--rw-r--r--   0        0        0      552 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      907 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0     2282 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
--rw-r--r--   0        0        0      506 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1312 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
--rw-r--r--   0        0        0     5051 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     3551 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      956 2024-03-22 20:11:00.313269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
--rw-r--r--   0        0        0      564 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0     3362 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
--rw-r--r--   0        0        0      762 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0     2321 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
--rw-r--r--   0        0        0     3432 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
--rw-r--r--   0        0        0     1613 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
--rw-r--r--   0        0        0     1863 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
--rw-r--r--   0        0        0      952 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0     3907 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
--rw-r--r--   0        0        0     8232 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
--rw-r--r--   0        0        0      461 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0      944 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
--rw-r--r--   0        0        0    14423 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     2955 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0     2389 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
--rw-r--r--   0        0        0      445 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0    12266 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
--rw-r--r--   0        0        0     3682 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
--rw-r--r--   0        0        0    22783 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
--rw-r--r--   0        0        0     3487 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0     2155 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     3663 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2879 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     2231 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
--rw-r--r--   0        0        0     1123 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
--rw-r--r--   0        0        0      604 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2767 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0     1006 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0     1641 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1711 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      428 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0      659 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0     2305 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
--rw-r--r--   0        0        0     3618 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1116 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     5609 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     9402 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
--rw-r--r--   0        0        0     1160 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2142 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10680 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2190 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0    14768 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
--rw-r--r--   0        0        0      184 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      537 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      713 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     6220 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
--rw-r--r--   0        0        0     2321 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0      415 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
--rw-r--r--   0        0        0     2426 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0     1218 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     3121 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0     1866 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
--rw-r--r--   0        0        0      706 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0      610 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
--rw-r--r--   0        0        0     1116 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
--rw-r--r--   0        0        0      611 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     1222 2024-03-22 20:11:00.317268 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
--rw-r--r--   0        0        0     7751 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0    13270 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
--rw-r--r--   0        0        0     1144 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0     1304 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2026 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1984 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1103 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     1704 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2024-03-22 20:11:00.321269 bbot-1.1.7.7rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0      764 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/ms_on_prem_subdomains.txt
--rw-r--r--   0        0        0    32226 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2024-03-22 20:11:00.325269 bbot-1.1.7.7rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     2627 2024-03-22 20:11:21.665284 bbot-1.1.7.7rc0/pyproject.toml
--rw-r--r--   0        0        0    40032 1970-01-01 00:00:00.000000 bbot-1.1.7.7rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/LICENSE
+-rw-r--r--   0        0        0    40272 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/README.md
+-rw-r--r--   0        0        0      211 2024-05-15 21:42:22.242473 bbot-1.1.8.3321rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7898 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    17601 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/cli.py
+-rw-r--r--   0        0        0       59 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3588 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9843 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5182 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1341 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      617 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0       91 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    46323 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1656 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1232 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       86 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     1537 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     4341 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/cloud.py
+-rw-r--r--   0        0        0    10976 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14117 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9199 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    47786 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     5639 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     6354 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0    12632 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    82906 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    22071 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0    10041 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0     1990 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     3463 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     5947 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     8781 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    31838 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    19801 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0      191 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8118 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     4158 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     2328 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/ajaxpro.py
+-rw-r--r--   0        0        0     1824 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     1372 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/azure_realm.py
+-rw-r--r--   0        0        0     4691 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     4150 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/baddns.py
+-rw-r--r--   0        0        0     1245 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/baddns_zone.py
+-rw-r--r--   0        0        0     3549 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    59062 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2352 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1299 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0      655 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bucket_amazon.py
+-rw-r--r--   0        0        0     1020 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      775 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1915 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bucket_file_enum.py
+-rw-r--r--   0        0        0     1352 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2540 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/bucket_google.py
+-rw-r--r--   0        0        0     4911 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     6553 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1188 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3371 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      798 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     1522 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/chaos.py
+-rw-r--r--   0        0        0     1810 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/code_repository.py
+-rw-r--r--   0        0        0      735 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     3297 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/credshed.py
+-rw-r--r--   0        0        0      376 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1230 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0     5316 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/deadly/dastardly.py
+-rw-r--r--   0        0        0    14079 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    17260 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5239 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     3928 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dehashed.py
+-rw-r--r--   0        0        0      930 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/digitorus.py
+-rw-r--r--   0        0        0     5324 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     3186 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     8781 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/docker_pull.py
+-rw-r--r--   0        0        0     3271 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dockerhub.py
+-rw-r--r--   0        0        0     9245 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dotnetnuke.py
+-rw-r--r--   0        0        0      791 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11758 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     7540 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/filedownload.py
+-rw-r--r--   0        0        0     2184 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1195 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7794 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1329 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2073 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/git_clone.py
+-rw-r--r--   0        0        0     3147 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/github_codesearch.py
+-rw-r--r--   0        0        0     8735 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/github_org.py
+-rw-r--r--   0        0        0     6070 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/github_workflows.py
+-rw-r--r--   0        0        0     5655 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/gitlab.py
+-rw-r--r--   0        0        0    11415 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      890 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7172 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     6758 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5990 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2098 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0    13124 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    18695 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     8286 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     4384 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internetdb.py
+-rw-r--r--   0        0        0     2123 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ip2location.py
+-rw-r--r--   0        0        0     1539 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     1767 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1541 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    10816 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    21031 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      857 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     2281 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/newsletters.py
+-rw-r--r--   0        0        0     5506 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     4731 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0     5852 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/oauth.py
+-rw-r--r--   0        0        0      774 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    14731 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     3215 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2604 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0      531 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/discord.py
+-rw-r--r--   0        0        0      985 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/emails.py
+-rw-r--r--   0        0        0     2182 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1907 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1375 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     2746 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     1117 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/slack.py
+-rw-r--r--   0        0        0     1886 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/splunk.py
+-rw-r--r--   0        0        0     1430 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/subdomains.py
+-rw-r--r--   0        0        0      723 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/teams.py
+-rw-r--r--   0        0        0     3627 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2218 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1689 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     9552 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1619 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1420 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0     5479 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/postman.py
+-rw-r--r--   0        0        0      832 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8456 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      828 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2025 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2898 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1201 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0      792 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1993 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/sitedossier.py
+-rw-r--r--   0        0        0     1478 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1408 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     2000 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7822 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     1327 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/subdomaincenter.py
+-rw-r--r--   0        0        0      553 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    17041 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0     5744 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/bucket.py
+-rw-r--r--   0        0        0     1308 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/github.py
+-rw-r--r--   0        0        0     2436 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/portscanner.py
+-rw-r--r--   0        0        0     1182 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/shodan.py
+-rw-r--r--   0        0        0     6100 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/subdomain_enum.py
+-rw-r--r--   0        0        0     3789 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/webhook.py
+-rw-r--r--   0        0        0      678 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     4527 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/trufflehog.py
+-rw-r--r--   0        0        0     4102 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2992 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2325 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1591 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     2010 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1272 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2871 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2336 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    29339 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    42299 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     2702 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0    11540 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     5889 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    12010 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     4870 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/conftest.py
+-rw-r--r--   0        0        0       31 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/coverage.cfg
+-rwxr-xr-x   0        0        0      652 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1091 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_output.ndjson
+-rw-r--r--   0        0        0        0 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5523 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6544 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0     3808 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     5853 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     7572 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    23553 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    31826 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0    16305 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_manager_deduplication.py
+-rw-r--r--   0        0        0    79706 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
+-rw-r--r--   0        0        0    16943 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     2657 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     7144 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_regexes.py
+-rw-r--r--   0        0        0     2870 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2175 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0    13141 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     5344 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      664 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      473 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0     2789 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
+-rw-r--r--   0        0        0      546 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     3098 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1207 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
+-rw-r--r--   0        0        0     4805 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     2795 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
+-rw-r--r--   0        0        0     2397 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
+-rw-r--r--   0        0        0     5599 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3984 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
+-rw-r--r--   0        0        0      552 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      907 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0     2282 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
+-rw-r--r--   0        0        0      506 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1312 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
+-rw-r--r--   0        0        0     5051 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     3551 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      956 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
+-rw-r--r--   0        0        0     2047 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py
+-rw-r--r--   0        0        0      564 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0     3362 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
+-rw-r--r--   0        0        0      762 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0     2321 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
+-rw-r--r--   0        0        0     3615 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
+-rw-r--r--   0        0        0     1613 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
+-rw-r--r--   0        0        0     1863 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
+-rw-r--r--   0        0        0      952 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0    27988 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py
+-rw-r--r--   0        0        0     3907 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
+-rw-r--r--   0        0        0     8232 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
+-rw-r--r--   0        0        0      461 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0      944 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
+-rw-r--r--   0        0        0    14708 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     2955 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0     2389 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
+-rw-r--r--   0        0        0      445 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0    12266 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
+-rw-r--r--   0        0        0     3718 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
+-rw-r--r--   0        0        0    24606 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
+-rw-r--r--   0        0        0    35521 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py
+-rw-r--r--   0        0        0    11579 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py
+-rw-r--r--   0        0        0     3433 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0     2155 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     4939 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2879 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     2231 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
+-rw-r--r--   0        0        0     1123 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
+-rw-r--r--   0        0        0      604 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2767 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0     1006 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0     1641 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1711 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      428 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0     1030 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0     2305 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
+-rw-r--r--   0        0        0     3618 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1116 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     5609 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     9402 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
+-rw-r--r--   0        0        0     1160 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2142 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10680 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2190 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0    14768 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
+-rw-r--r--   0        0        0      184 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      537 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      713 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     6220 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
+-rw-r--r--   0        0        0     2321 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0      415 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
+-rw-r--r--   0        0        0     2426 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0     1700 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     3121 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0     1866 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
+-rw-r--r--   0        0        0      706 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0      610 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
+-rw-r--r--   0        0        0     1116 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
+-rw-r--r--   0        0        0      611 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     1222 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
+-rw-r--r--   0        0        0     7751 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0    62527 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
+-rw-r--r--   0        0        0     1144 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0     1304 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2026 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1979 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1103 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     1704 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0      764 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/ms_on_prem_subdomains.txt
+-rw-r--r--   0        0        0    32226 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     2663 2024-05-15 21:42:22.238473 bbot-1.1.8.3321rc0/pyproject.toml
+-rw-r--r--   0        0        0    42361 1970-01-01 00:00:00.000000 bbot-1.1.8.3321rc0/PKG-INFO
```

### Comparing `bbot-1.1.7.7rc0/LICENSE` & `bbot-1.1.8.3321rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/README.md` & `bbot-1.1.8.3321rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -260,37 +260,38 @@
 
 ![subdomain-stats-ebay](https://github.com/blacklanternsecurity/bbot/assets/20261699/53e07e9f-50b6-4b70-9e83-297dbfbcb436)
 
 ## BBOT Modules By Flag
 For a full list of modules, including the data types consumed and emitted by each one, see [List of Modules](https://www.blacklanternsecurity.com/bbot/modules/list_of_modules/).
 
 <!-- BBOT MODULE FLAGS -->
-| Flag             | # Modules   | Description                                        | Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-|------------------|-------------|----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| safe             | 78          | Non-intrusive, safe to run                         | affiliates, aggregate, ajaxpro, anubisdb, asn, azure_realm, azure_tenant, baddns, baddns_zone, badsecrets, bevigil, binaryedge, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, dockerhub, emailformat, filedownload, fingerprintx, fullhunt, git, git_clone, github_codesearch, github_org, gowitness, hackertarget, httpx, hunt, hunterio, iis_shortnames, internetdb, ip2location, ipstack, leakix, myssl, newsletters, ntlm, oauth, otx, passivetotal, pgp, postman, rapiddns, riddler, robots, secretsdb, securitytrails, shodan_dns, sitedossier, skymem, social, sslcert, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wappalyzer, wayback, zoomeye |
-| passive          | 58          | Never connects to target systems                   | affiliates, aggregate, anubisdb, asn, azure_realm, azure_tenant, bevigil, binaryedge, bucket_file_enum, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, emailformat, excavate, fullhunt, git_clone, github_codesearch, github_org, hackertarget, hunterio, internetdb, ip2location, ipneighbor, ipstack, leakix, massdns, myssl, otx, passivetotal, pgp, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, skymem, social, speculate, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wayback, zoomeye                                                                                                                                                                                                                                         |
-| subdomain-enum   | 45          | Enumerates subdomains                              | anubisdb, asn, azure_realm, azure_tenant, baddns_zone, bevigil, binaryedge, builtwith, c99, censys, certspotter, chaos, columbus, crt, digitorus, dnscommonsrv, dnsdumpster, fullhunt, github_codesearch, github_org, hackertarget, httpx, hunterio, internetdb, ipneighbor, leakix, massdns, myssl, oauth, otx, passivetotal, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, sslcert, subdomaincenter, subdomains, threatminer, urlscan, virustotal, wayback, zoomeye                                                                                                                                                                                                                                                                                                                                                                                      |
-| active           | 42          | Makes active connections to target systems         | ajaxpro, baddns, baddns_zone, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dockerhub, dotnetnuke, ffuf, ffuf_shortnames, filedownload, fingerprintx, generic_ssrf, git, gowitness, host_header, httpx, hunt, iis_shortnames, masscan, newsletters, nmap, ntlm, nuclei, oauth, paramminer_cookies, paramminer_getparams, paramminer_headers, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, vhost, wafw00f, wappalyzer                                                                                                                                                                                                                                                                                                                                                                    |
-| web-thorough     | 29          | More advanced web scanning functionality           | ajaxpro, azure_realm, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf_shortnames, filedownload, generic_ssrf, git, host_header, httpx, hunt, iis_shortnames, nmap, ntlm, oauth, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-| aggressive       | 20          | Generates a large amount of network traffic        | bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, generic_ssrf, host_header, ipneighbor, masscan, massdns, nmap, nuclei, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, telerik, url_manipulation, vhost, wafw00f                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
-| web-basic        | 17          | Basic, non-intrusive web scan functionality        | azure_realm, baddns, badsecrets, bucket_amazon, bucket_azure, bucket_firebase, bucket_google, filedownload, git, httpx, iis_shortnames, ntlm, oauth, robots, secretsdb, sslcert, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| cloud-enum       | 12          | Enumerates cloud resources                         | azure_realm, azure_tenant, baddns, baddns_zone, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, httpx, oauth                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-| slow             | 9           | May take a long time to complete                   | bucket_digitalocean, dastardly, fingerprintx, git_clone, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
-| affiliates       | 8           | Discovers affiliated hostnames/domains             | affiliates, azure_realm, azure_tenant, builtwith, oauth, sslcert, viewdns, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
-| email-enum       | 7           | Enumerates email addresses                         | dehashed, emailformat, emails, hunterio, pgp, skymem, sslcert                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| deadly           | 4           | Highly aggressive                                  | dastardly, ffuf, nuclei, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-| portscan         | 3           | Discovers open ports                               | internetdb, masscan, nmap                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| web-paramminer   | 3           | Discovers HTTP parameters through brute-force      | paramminer_cookies, paramminer_getparams, paramminer_headers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| baddns           | 2           | Runs all modules from the DNS auditing tool BadDNS | baddns, baddns_zone                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
-| iis-shortnames   | 2           | Scans for IIS Shortname vulnerability              | ffuf_shortnames, iis_shortnames                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
-| report           | 2           | Generates a report at the end of the scan          | affiliates, asn                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
-| social-enum      | 2           | Enumerates social media                            | httpx, social                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| service-enum     | 1           | Identifies protocols running on open ports         | fingerprintx                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| subdomain-hijack | 1           | Detects hijackable subdomains                      | baddns                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
-| web-screenshots  | 1           | Takes screenshots of web pages                     | gowitness                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| Flag             | # Modules   | Description                                        | Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+|------------------|-------------|----------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| safe             | 82          | Non-intrusive, safe to run                         | affiliates, aggregate, ajaxpro, anubisdb, asn, azure_realm, azure_tenant, baddns, baddns_zone, badsecrets, bevigil, binaryedge, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, builtwith, c99, censys, certspotter, chaos, code_repository, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, docker_pull, dockerhub, emailformat, filedownload, fingerprintx, fullhunt, git, git_clone, github_codesearch, github_org, github_workflows, gitlab, gowitness, hackertarget, httpx, hunt, hunterio, iis_shortnames, internetdb, ip2location, ipstack, leakix, myssl, newsletters, ntlm, oauth, otx, passivetotal, pgp, postman, rapiddns, riddler, robots, secretsdb, securitytrails, shodan_dns, sitedossier, skymem, social, sslcert, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wappalyzer, wayback, zoomeye |
+| passive          | 62          | Never connects to target systems                   | affiliates, aggregate, anubisdb, asn, azure_realm, azure_tenant, bevigil, binaryedge, bucket_file_enum, builtwith, c99, censys, certspotter, chaos, code_repository, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, docker_pull, dockerhub, emailformat, excavate, fullhunt, git_clone, github_codesearch, github_org, github_workflows, hackertarget, hunterio, internetdb, ip2location, ipneighbor, ipstack, leakix, massdns, myssl, otx, passivetotal, pgp, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, skymem, social, speculate, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wayback, zoomeye                                                                                                                                                                                                                                      |
+| subdomain-enum   | 45          | Enumerates subdomains                              | anubisdb, asn, azure_realm, azure_tenant, baddns_zone, bevigil, binaryedge, builtwith, c99, censys, certspotter, chaos, columbus, crt, digitorus, dnscommonsrv, dnsdumpster, fullhunt, github_codesearch, github_org, hackertarget, httpx, hunterio, internetdb, ipneighbor, leakix, massdns, myssl, oauth, otx, passivetotal, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, sslcert, subdomaincenter, subdomains, threatminer, urlscan, virustotal, wayback, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| active           | 42          | Makes active connections to target systems         | ajaxpro, baddns, baddns_zone, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, filedownload, fingerprintx, generic_ssrf, git, gitlab, gowitness, host_header, httpx, hunt, iis_shortnames, masscan, newsletters, nmap, ntlm, nuclei, oauth, paramminer_cookies, paramminer_getparams, paramminer_headers, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, vhost, wafw00f, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| web-thorough     | 29          | More advanced web scanning functionality           | ajaxpro, azure_realm, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf_shortnames, filedownload, generic_ssrf, git, host_header, httpx, hunt, iis_shortnames, nmap, ntlm, oauth, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+| aggressive       | 20          | Generates a large amount of network traffic        | bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, generic_ssrf, host_header, ipneighbor, masscan, massdns, nmap, nuclei, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, telerik, url_manipulation, vhost, wafw00f                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| web-basic        | 17          | Basic, non-intrusive web scan functionality        | azure_realm, baddns, badsecrets, bucket_amazon, bucket_azure, bucket_firebase, bucket_google, filedownload, git, httpx, iis_shortnames, ntlm, oauth, robots, secretsdb, sslcert, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| cloud-enum       | 12          | Enumerates cloud resources                         | azure_realm, azure_tenant, baddns, baddns_zone, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, httpx, oauth                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+| slow             | 10          | May take a long time to complete                   | bucket_digitalocean, dastardly, docker_pull, fingerprintx, git_clone, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| affiliates       | 8           | Discovers affiliated hostnames/domains             | affiliates, azure_realm, azure_tenant, builtwith, oauth, sslcert, viewdns, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
+| email-enum       | 7           | Enumerates email addresses                         | dehashed, emailformat, emails, hunterio, pgp, skymem, sslcert                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| deadly           | 4           | Highly aggressive                                  | dastardly, ffuf, nuclei, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| portscan         | 3           | Discovers open ports                               | internetdb, masscan, nmap                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| web-paramminer   | 3           | Discovers HTTP parameters through brute-force      | paramminer_cookies, paramminer_getparams, paramminer_headers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| baddns           | 2           | Runs all modules from the DNS auditing tool BadDNS | baddns, baddns_zone                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| iis-shortnames   | 2           | Scans for IIS Shortname vulnerability              | ffuf_shortnames, iis_shortnames                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| report           | 2           | Generates a report at the end of the scan          | affiliates, asn                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| social-enum      | 2           | Enumerates social media                            | httpx, social                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| repo-enum        | 1           | Enumerates code repositories                       | code_repository                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| service-enum     | 1           | Identifies protocols running on open ports         | fingerprintx                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| subdomain-hijack | 1           | Detects hijackable subdomains                      | baddns                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| web-screenshots  | 1           | Takes screenshots of web pages                     | gowitness                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 <!-- END BBOT MODULE FLAGS -->
 
 ## BBOT Output Modules
 BBOT can save its data to TXT, CSV, JSON, and tons of other destinations including [Neo4j](https://www.blacklanternsecurity.com/bbot/scanning/output/#neo4j), [Splunk](https://www.blacklanternsecurity.com/bbot/scanning/output/#splunk), and [Discord](https://www.blacklanternsecurity.com/bbot/scanning/output/#discord-slack-teams). For instructions on how to use these, see [Output Modules](https://www.blacklanternsecurity.com/bbot/scanning/output). 
 
 <!-- BBOT OUTPUT MODULES -->
 | Module          | Type   | Needs API Key   | Description                                                                             | Flags          | Consumed Events                                                                                  | Produced Events           |
```

### Comparing `bbot-1.1.7.7rc0/bbot/agent/agent.py` & `bbot-1.1.8.3321rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/cli.py` & `bbot-1.1.8.3321rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.8.3321rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/configurator/args.py` & `bbot-1.1.8.3321rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/configurator/environ.py` & `bbot-1.1.8.3321rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/configurator/files.py` & `bbot-1.1.8.3321rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/errors.py` & `bbot-1.1.8.3321rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/event/base.py` & `bbot-1.1.8.3321rc0/bbot/core/event/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import json
 import asyncio
 import logging
 import ipaddress
 import traceback
+from copy import copy
 from typing import Optional
 from datetime import datetime
 from contextlib import suppress
 from urllib.parse import urljoin
 from pydantic import BaseModel, field_validator
 
 from .helpers import *
@@ -208,14 +209,17 @@
             # removed this second part because it was making certain sslcert events internal
             if _internal:  # or source._internal:
                 self.internal = True
 
         # an event indicating whether the event has undergone DNS resolution
         self._resolved = asyncio.Event()
 
+        # inherit web spider distance from parent
+        self.web_spider_distance = getattr(self.source, "web_spider_distance", 0)
+
     @property
     def data(self):
         return self._data
 
     @property
     def resolved_hosts(self):
         if is_ip(self.host):
@@ -874,15 +878,14 @@
 
 
 class URL_UNVERIFIED(BaseEvent):
     _status_code_regex = re.compile(r"^status-(\d{1,3})$")
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.web_spider_distance = getattr(self.source, "web_spider_distance", 0)
         # increment the web spider distance
         if self.type == "URL_UNVERIFIED" and getattr(self.module, "name", "") != "TARGET":
             self.web_spider_distance += 1
         self.num_redirects = getattr(self.source, "num_redirects", 0)
 
     def sanitize_data(self, data):
         self.parsed = validators.validate_url_parsed(data)
@@ -961,14 +964,19 @@
     _always_emit = True
 
     class _data_validator(BaseModel):
         name: str
         url: str
         _validate_url = field_validator("url")(validators.validate_url)
 
+    def sanitize_data(self, data):
+        data = super().sanitize_data(data)
+        data["name"] = data["name"].lower()
+        return data
+
     def _words(self):
         return self.data["name"]
 
 
 class URL_HINT(URL_UNVERIFIED):
     pass
 
@@ -993,14 +1001,15 @@
         self.num_redirects = getattr(self.source, "num_redirects", 0)
         if str(self.http_status).startswith("3"):
             self.num_redirects += 1
 
     def sanitize_data(self, data):
         url = data.get("url", "")
         self.parsed = validators.validate_url_parsed(url)
+        data["url"] = self.parsed.geturl()
 
         header_dict = {}
         for i in data.get("raw_header", "").splitlines():
             if len(i) > 0 and ":" in i:
                 k, v = i.split(":", 1)
                 k = k.strip().lower()
                 v = v.lstrip()
@@ -1181,21 +1190,21 @@
 class WAF(DictHostEvent):
     _always_emit = True
     _quick_emit = True
 
     class _data_validator(BaseModel):
         url: str
         host: str
-        WAF: str
+        waf: str
         info: Optional[str] = None
         _validate_url = field_validator("url")(validators.validate_url)
         _validate_host = field_validator("host")(validators.validate_host)
 
     def _pretty_string(self):
-        return self.data["WAF"]
+        return self.data["waf"]
 
 
 def make_event(
     data,
     event_type=None,
     source=None,
     module=None,
@@ -1251,27 +1260,30 @@
     """
 
     # allow tags to be either a string or an array
     if not tags:
         tags = []
     elif isinstance(tags, str):
         tags = [tags]
-    tags = list(tags)
+    tags = set(tags)
 
     if is_event(data):
+        data = copy(data)
         if scan is not None and not data.scan:
             data.scan = scan
         if scans is not None and not data.scans:
             data.scans = scans
         if module is not None:
             data.module = module
         if source is not None:
             data.source = source
         if internal == True:
             data.internal = True
+        if tags:
+            data.tags = tags.union(data.tags)
         event_type = data.type
         return data
     else:
         if event_type is None:
             event_type, data = get_event_type(data)
             if not dummy:
                 log.debug(f'Autodetected event type "{event_type}" based on data: "{data}"')
@@ -1294,15 +1306,15 @@
                 if event_type == "DNS_NAME" and data_is_ip:
                     event_type = "IP_ADDRESS"
                 elif event_type == "IP_ADDRESS" and not data_is_ip:
                     event_type = "DNS_NAME"
         # USERNAME <--> EMAIL_ADDRESS confusion
         if event_type == "USERNAME" and validators.soft_validate(data, "email"):
             event_type = "EMAIL_ADDRESS"
-            tags.append("affiliate")
+            tags.add("affiliate")
 
         event_class = globals().get(event_type, DefaultEvent)
 
         return event_class(
             data,
             event_type=event_type,
             source=source,
```

### Comparing `bbot-1.1.7.7rc0/bbot/core/event/helpers.py` & `bbot-1.1.8.3321rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/flags.py` & `bbot-1.1.8.3321rc0/bbot/core/flags.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     "passive": "Never connects to target systems",
     "portscan": "Discovers open ports",
     "report": "Generates a report at the end of the scan",
     "safe": "Non-intrusive, safe to run",
     "service-enum": "Identifies protocols running on open ports",
     "slow": "May take a long time to complete",
     "social-enum": "Enumerates social media",
+    "repo-enum": "Enumerates code repositories",
     "subdomain-enum": "Enumerates subdomains",
     "subdomain-hijack": "Detects hijackable subdomains",
     "web-basic": "Basic, non-intrusive web scan functionality",
     "web-paramminer": "Discovers HTTP parameters through brute-force",
     "web-screenshots": "Takes screenshots of web pages",
     "web-thorough": "More advanced web scanning functionality",
 }
```

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/cache.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/cloud.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/cloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/command.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,16 @@
 
 
 async def _write_proc_line(proc, chunk):
     try:
         proc.stdin.write(smart_encode(chunk) + b"\n")
         await proc.stdin.drain()
     except Exception as e:
-        command = " ".join([str(s) for s in proc.args])
+        proc_args = [str(s) for s in getattr(proc, "args", [])]
+        command = " ".join(proc_args)
         log.warning(f"Error writing line to stdin for command: {command}: {e}")
         log.trace(traceback.format_exc())
 
 
 async def _write_stdin(proc, _input):
     """
     Asynchronously writes input to an active subprocess's stdin.
```

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/diff.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/dns.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/files.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/helper.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/logger.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/misc.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,21 +21,22 @@
 import subprocess as sp
 from pathlib import Path
 from itertools import islice
 from datetime import datetime
 from tabulate import tabulate
 import wordninja as _wordninja
 from contextlib import suppress
+from unidecode import unidecode  # noqa F401
 import cloudcheck as _cloudcheck
 import tldextract as _tldextract
 import xml.etree.ElementTree as ET
 from collections.abc import Mapping
 from hashlib import sha1 as hashlib_sha1
 from asyncio import create_task, gather, sleep, wait_for  # noqa
-from urllib.parse import urlparse, quote, unquote, urlunparse  # noqa F401
+from urllib.parse import urlparse, quote, unquote, urlunparse, urljoin  # noqa F401
 
 from .url import *  # noqa F401
 from .. import errors
 from .logger import log_to_stderr
 from . import regexes as bbot_regexes
 from .names_generator import random_name, names, adjectives  # noqa F401
 
@@ -1140,25 +1141,27 @@
     """
     Forgive me father for I have sinned
     """
     try:
         parent = psutil.Process(parent_pid)
     except psutil.NoSuchProcess:
         log.debug(f"No such PID: {parent_pid}")
+        return
     log.debug(f"Killing children of process ID {parent.pid}")
     children = parent.children(recursive=True)
     for child in children:
         log.debug(f"Killing child with PID {child.pid}")
         if child.name != "python":
             try:
                 child.send_signal(sig)
             except psutil.NoSuchProcess:
                 log.debug(f"No such PID: {child.pid}")
             except psutil.AccessDenied:
                 log.debug(f"Error killing PID: {child.pid} - access denied")
+    log.debug(f"Finished killing children of process ID {parent.pid}")
 
 
 def str_or_file(s):
     """Reads a string or file and yields its content line-by-line.
 
     This function tries to open the given string `s` as a file and yields its lines.
     If it fails to open `s` as a file, it treats `s` as a regular string and yields it as is.
@@ -1963,15 +1966,15 @@
             check=True,
         )
     except sp.CalledProcessError:
         return False
     return True
 
 
-def make_table(*args, **kwargs):
+def make_table(rows, header, **kwargs):
     """Generate a formatted table from the given rows and headers.
 
     This function uses the `tabulate` package to generate a table with formatting options.
     It can accept various input formats and table styles, which can be customized using optional arguments.
 
     Args:
         *args: Positional arguments to be passed to `tabulate.tabulate`.
@@ -1990,29 +1993,36 @@
         +===========+===========+
         | row1      | row1      |
         +-----------+-----------+
         | row2      | row2      |
         +-----------+-----------+
     """
     # fix IndexError: list index out of range
-    if args and not args[0]:
-        args = ([[]],) + args[1:]
+    if not rows:
+        rows = [[]]
     tablefmt = os.environ.get("BBOT_TABLE_FORMAT", None)
     defaults = {"tablefmt": "grid", "disable_numparse": True, "maxcolwidths": None}
     if tablefmt is None:
         defaults.update({"maxcolwidths": 40})
     else:
         defaults.update({"tablefmt": tablefmt})
     for k, v in defaults.items():
         if k not in kwargs:
             kwargs[k] = v
     # don't wrap columns in markdown
     if tablefmt in ("github", "markdown"):
         kwargs.pop("maxcolwidths")
-    return tabulate(*args, **kwargs)
+        # escape problematic markdown characters in rows
+
+        def markdown_escape(s):
+            return str(s).replace("|", "&#124;")
+
+        rows = [[markdown_escape(f) for f in row] for row in rows]
+        header = [markdown_escape(h) for h in header]
+    return tabulate(rows, header, **kwargs)
 
 
 def human_timedelta(d):
     """Convert a TimeDelta object into a human-readable string.
 
     This function takes a datetime.timedelta object and converts it into a string format that
     is easier to read and understand.
```

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/modules.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/url.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/validators.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/web.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/web.py`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,17 @@
         else:
             # kwargs["raise_error"] = True
             # kwargs["stream"] = True
             kwargs["follow_redirects"] = follow_redirects
             if not "method" in kwargs:
                 kwargs["method"] = "GET"
             try:
-                async with self._acatch(url, raise_error), self.AsyncClient().stream(url=url, **kwargs) as response:
+                async with self._acatch(url, raise_error=True), self.AsyncClient().stream(
+                    url=url, **kwargs
+                ) as response:
                     status_code = getattr(response, "status_code", 0)
                     log.debug(f"Download result: HTTP {status_code}")
                     if status_code != 0:
                         response.raise_for_status()
                         with open(filename, "wb") as f:
                             agen = response.aiter_bytes(chunk_size=chunk_size)
                             async for chunk in agen:
@@ -296,14 +298,16 @@
                                 f.write(chunk)
                         success = True
             except httpx.HTTPError as e:
                 log_fn = log.verbose
                 if warn:
                     log_fn = log.warning
                 log_fn(f"Failed to download {url}: {e}")
+                if raise_error:
+                    raise
                 return
 
         if success:
             return filename.resolve()
 
     async def wordlist(self, path, lines=None, **kwargs):
         """
@@ -647,44 +651,50 @@
         Note:
             This function is internal and should generally not be used directly.
             `url`, `args`, `kwargs`, and `raise_error` should be in the same context as this function.
         """
         try:
             yield
         except httpx.TimeoutException:
-            log.verbose(f"HTTP timeout to URL: {url}")
             if raise_error:
                 raise
+            else:
+                log.verbose(f"HTTP timeout to URL: {url}")
         except httpx.ConnectError:
-            log.debug(f"HTTP connect failed to URL: {url}")
             if raise_error:
                 raise
-        except httpx.RequestError as e:
-            log.trace(f"Error with request to URL: {url}: {e}")
-            log.trace(traceback.format_exc())
+            else:
+                log.debug(f"HTTP connect failed to URL: {url}")
+        except httpx.HTTPError as e:
             if raise_error:
                 raise
+            else:
+                log.trace(f"Error with request to URL: {url}: {e}")
+                log.trace(traceback.format_exc())
         except ssl.SSLError as e:
             msg = f"SSL error with request to URL: {url}: {e}"
-            log.trace(msg)
-            log.trace(traceback.format_exc())
             if raise_error:
                 raise httpx.RequestError(msg)
+            else:
+                log.trace(msg)
+                log.trace(traceback.format_exc())
         except anyio.EndOfStream as e:
             msg = f"AnyIO error with request to URL: {url}: {e}"
-            log.trace(msg)
-            log.trace(traceback.format_exc())
             if raise_error:
                 raise httpx.RequestError(msg)
+            else:
+                log.trace(msg)
+                log.trace(traceback.format_exc())
         except SOCKSError as e:
             msg = f"SOCKS error with request to URL: {url}: {e}"
-            log.trace(msg)
-            log.trace(traceback.format_exc())
             if raise_error:
                 raise httpx.RequestError(msg)
+            else:
+                log.trace(msg)
+                log.trace(traceback.format_exc())
         except BaseException as e:
             # don't log if the error is the result of an intentional cancellation
             if not any(
                 isinstance(_e, asyncio.exceptions.CancelledError) for _e in self.parent_helper.get_exception_chain(e)
             ):
                 log.trace(f"Unhandled exception with request to URL: {url}: {e}")
                 log.trace(traceback.format_exc())
```

### Comparing `bbot-1.1.7.7rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.8.3321rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/core/logger/logger.py` & `bbot-1.1.8.3321rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/defaults.yml` & `bbot-1.1.8.3321rc0/bbot/defaults.yml`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,15 @@
     - svg
     - webp
     # web/fonts
     - css
     - woff
     - woff2
     - ttf
+    - eot
     - sass
     - scss
     # audio
     - mp3
     - m4a
     - wav
     - flac
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/ajaxpro.py` & `bbot-1.1.8.3321rc0/bbot/modules/ajaxpro.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/anubisdb.py` & `bbot-1.1.8.3321rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/azure_realm.py` & `bbot-1.1.8.3321rc0/bbot/modules/azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.8.3321rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/baddns.py` & `bbot-1.1.8.3321rc0/bbot/modules/baddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/baddns_zone.py` & `bbot-1.1.8.3321rc0/bbot/modules/baddns_zone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/badsecrets.py` & `bbot-1.1.8.3321rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/base.py` & `bbot-1.1.8.3321rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/bevigil.py` & `bbot-1.1.8.3321rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/binaryedge.py` & `bbot-1.1.8.3321rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/bucket_amazon.py` & `bbot-1.1.8.3321rc0/bbot/modules/bucket_amazon.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.8.3321rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.8.3321rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/bucket_file_enum.py` & `bbot-1.1.8.3321rc0/bbot/modules/bucket_file_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.8.3321rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/bucket_google.py` & `bbot-1.1.8.3321rc0/bbot/modules/bucket_google.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/builtwith.py` & `bbot-1.1.8.3321rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/bypass403.py` & `bbot-1.1.8.3321rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/c99.py` & `bbot-1.1.8.3321rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/censys.py` & `bbot-1.1.8.3321rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/certspotter.py` & `bbot-1.1.8.3321rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/chaos.py` & `bbot-1.1.8.3321rc0/bbot/modules/chaos.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/columbus.py` & `bbot-1.1.8.3321rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/credshed.py` & `bbot-1.1.8.3321rc0/bbot/modules/credshed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/crt.py` & `bbot-1.1.8.3321rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/deadly/dastardly.py` & `bbot-1.1.8.3321rc0/bbot/modules/deadly/dastardly.py`

 * *Files 3% similar despite different names*

```diff
@@ -100,18 +100,20 @@
             "public.ecr.aws/portswigger/dastardly:latest",
         ]
         return command, temp_path
 
     def parse_dastardly_xml(self, xml_file):
         try:
             with open(xml_file, "rb") as f:
-                et = etree.parse(f)
+                et = etree.parse(f, parser=etree.XMLParser(recover=True))
                 for testsuite in et.iter("testsuite"):
                     yield TestSuite(testsuite)
-        except Exception as e:
+        except FileNotFoundError:
+            pass
+        except etree.ParseError as e:
             self.warning(f"Error parsing Dastardly XML at {xml_file}: {e}")
 
 
 class Failure:
     def __init__(self, xml):
         self.etree = xml
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.8.3321rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.8.3321rc0/bbot/modules/deadly/nuclei.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,21 +334,23 @@
     def get_yaml_request_attr(self, yf, attr):
         p = self.parse_yaml(yf)
         requests = p.get("http", [])
         for r in requests:
             raw = r.get("raw")
             if not raw:
                 res = r.get(attr)
-                yield res
+                if res is not None:
+                    yield res
 
     def get_yaml_info_attr(self, yf, attr):
         p = self.parse_yaml(yf)
         info = p.get("info", [])
         res = info.get(attr)
-        yield res
+        if res is not None:
+            yield res
 
     # Parse through all templates and locate those which match the conditions necessary to collapse down to the budget setting
     def find_collapsible_templates(self):
         collapsible_templates = []
         severity_dict = {}
         for yf in self.yaml_list:
             valid = True
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.8.3321rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/dehashed.py` & `bbot-1.1.8.3321rc0/bbot/modules/dehashed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/digitorus.py` & `bbot-1.1.8.3321rc0/bbot/modules/digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.8.3321rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.8.3321rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/dockerhub.py` & `bbot-1.1.8.3321rc0/bbot/modules/dockerhub.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from bbot.modules.base import BaseModule
 
 
 class dockerhub(BaseModule):
     watched_events = ["SOCIAL", "ORG_STUB"]
     produced_events = ["SOCIAL", "CODE_REPOSITORY", "URL_UNVERIFIED"]
-    flags = ["active", "safe"]
+    flags = ["passive", "safe"]
     meta = {"description": "Search for docker repositories of discovered orgs/usernames"}
 
     site_url = "https://hub.docker.com"
     api_url = f"{site_url}/v2"
 
     scope_distance_modifier = 2
 
@@ -26,15 +26,15 @@
 
     async def handle_org_stub(self, event):
         profile_name = event.data
         # docker usernames are case sensitive, so if there are capitalizations we also try a lowercase variation
         profiles_to_check = set([profile_name, profile_name.lower()])
         for p in profiles_to_check:
             api_url = f"{self.api_url}/users/{p}"
-            api_result = await self.helpers.request(api_url)
+            api_result = await self.helpers.request(api_url, follow_redirects=True)
             status_code = getattr(api_result, "status_code", 0)
             if status_code == 200:
                 site_url = f"{self.site_url}/u/{p}"
                 # emit social event
                 await self.emit_event(
                     {"platform": "docker", "url": site_url, "profile_name": p}, "SOCIAL", source=event
                 )
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/dotnetnuke.py` & `bbot-1.1.8.3321rc0/bbot/modules/dotnetnuke.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/emailformat.py` & `bbot-1.1.8.3321rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.8.3321rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/filedownload.py` & `bbot-1.1.8.3321rc0/bbot/modules/filedownload.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,16 @@
         if event.type == "URL_UNVERIFIED":
             url_lower = event.data.lower()
             extension_matches = any(url_lower.endswith(f".{e}") for e in self.extensions)
             filedownload_requested = "filedownload" in event.tags
             if extension_matches or filedownload_requested:
                 await self.download_file(event.data)
         elif event.type == "HTTP_RESPONSE":
-            content_type = event.data["header"].get("content_type", "")
+            headers = event.data.get("header", {})
+            content_type = headers.get("content_type", "")
             if content_type:
                 url = event.data["url"]
                 await self.download_file(url, content_type=content_type)
 
     async def download_file(self, url, content_type=None):
         orig_filename, file_destination, base_url = self.make_filename(url, content_type=content_type)
         if orig_filename is None:
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.8.3321rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/fullhunt.py` & `bbot-1.1.8.3321rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.8.3321rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/git.py` & `bbot-1.1.8.3321rc0/bbot/modules/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import re
-from urllib.parse import urljoin
 
 from bbot.modules.base import BaseModule
 
 
 class git(BaseModule):
     watched_events = ["URL"]
     produced_events = ["FINDING"]
@@ -13,17 +12,17 @@
     in_scope_only = True
 
     fp_regex = re.compile(r"<html|<body", re.I)
 
     async def handle_event(self, event):
         base_url = event.data.rstrip("/")
         urls = {
-            # git config
-            urljoin(base_url, ".git/config"),
-            urljoin(f"{base_url}/", ".git/config"),
+            # look for git config in both
+            self.helpers.urljoin(base_url, ".git/config"),
+            self.helpers.urljoin(f"{base_url}/", ".git/config"),
         }
         tasks = [self.get_url(u) for u in urls]
         async for task in self.helpers.as_completed(tasks):
             result, url = await task
             text = getattr(result, "text", "")
             if not text:
                 text = ""
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/git_clone.py` & `bbot-1.1.8.3321rc0/bbot/modules/git_clone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/github_codesearch.py` & `bbot-1.1.8.3321rc0/bbot/modules/github_codesearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     async def setup(self):
         self.limit = self.config.get("limit", 100)
         return await super().setup()
 
     async def handle_event(self, event):
         query = self.make_query(event)
         for repo_url, raw_urls in (await self.query(query)).items():
-            repo_event = self.make_event({"url": repo_url}, "CODE_REPOSITORY", source=event)
+            repo_event = self.make_event({"url": repo_url}, "CODE_REPOSITORY", tags="git", source=event)
             if repo_event is None:
                 continue
             await self.emit_event(repo_event)
             for raw_url in raw_urls:
                 url_event = self.make_event(raw_url, "URL_UNVERIFIED", source=repo_event, tags=["httpx-safe"])
                 if not url_event:
                     continue
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/github_org.py` & `bbot-1.1.8.3321rc0/bbot/modules/github_org.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,16 @@
                         await self.emit_event(member_event)
 
         # find valid orgs from stub (ORG_STUB --> SOCIAL)
         elif event.type == "ORG_STUB":
             user = event.data
             self.verbose(f"Validating whether the organization {user} is within our scope...")
             is_org, in_scope = await self.validate_org(user)
+            if "target" in event.tags:
+                in_scope = True
             if not is_org or not in_scope:
                 self.verbose(f"Unable to validate that {user} is in-scope, skipping...")
                 return
 
             event_data = {"platform": "github", "profile_name": user, "url": f"https://github.com/{user}"}
             github_org_event = self.make_event(event_data, "SOCIAL", tags="github-org", source=event)
             if github_org_event:
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/gowitness.py` & `bbot-1.1.8.3321rc0/bbot/modules/gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/hackertarget.py` & `bbot-1.1.8.3321rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/host_header.py` & `bbot-1.1.8.3321rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/httpx.py` & `bbot-1.1.8.3321rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/hunt.py` & `bbot-1.1.8.3321rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/hunterio.py` & `bbot-1.1.8.3321rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.8.3321rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/internal/base.py` & `bbot-1.1.8.3321rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.8.3321rc0/bbot/modules/internal/excavate.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         super().__init__(excavate)
 
     async def report(self, result, name, event, **kwargs):
         await self.excavate.emit_event(result, "DNS_NAME", source=event)
 
 
 class URLExtractor(BaseExtractor):
-    url_path_regex = r"((?:\w|\d)(?:[\d\w-]+\.?)+(?::\d{1,5})?(?:/[-\w\.\(\)]+)*/?)"
+    url_path_regex = r"((?:\w|\d)(?:[\d\w-]+\.?)+(?::\d{1,5})?(?:/[-\w\.\(\)]*[-\w\.]+)*/?)"
     regexes = {
         "fulluri": r"(?i)" + r"([a-z]\w{1,15})://" + url_path_regex,
         "fullurl": r"(?i)" + r"(https?)://" + url_path_regex,
         "a-tag": r"<a\s+(?:[^>]*?\s+)?href=([\"'])(.*?)\1",
         "link-tag": r"<link\s+(?:[^>]*?\s+)?href=([\"'])(.*?)\1",
         "script-tag": r"<script\s+(?:[^>]*?\s+)?src=([\"'])(.*?)\1",
     }
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.8.3321rc0/bbot/modules/internal/speculate.py`

 * *Files 15% similar despite different names*

```diff
@@ -79,43 +79,55 @@
 
         # parent domains
         if event.type == "DNS_NAME":
             parent = self.helpers.parent_domain(event.data)
             if parent != event.data:
                 await self.emit_event(parent, "DNS_NAME", source=event, internal=True)
 
-        # generate open ports
-
         # we speculate on distance-1 stuff too, because distance-1 open ports are needed by certain modules like sslcert
         event_in_scope_distance = event.scope_distance <= (self.scan.scope_search_distance + 1)
         speculate_open_ports = self.emit_open_ports and event_in_scope_distance
 
-        # from URLs
+        # URL --> OPEN_TCP_PORT
         if event.type == "URL" or (event.type == "URL_UNVERIFIED" and self.open_port_consumers):
             # only speculate port from a URL if it wouldn't be speculated naturally from the host
             if event.host and (event.port not in self.ports or not speculate_open_ports):
                 await self.emit_event(
                     self.helpers.make_netloc(event.host, event.port),
                     "OPEN_TCP_PORT",
                     source=event,
                     internal=True,
                     quick=(event.type == "URL"),
                 )
 
-        # generate sub-directory URLS from URLS
+        # speculate sub-directory URLS from URLS
         if event.type == "URL":
             url_parents = self.helpers.url_parents(event.data)
             for up in url_parents:
                 url_event = self.make_event(f"{up}/", "URL_UNVERIFIED", source=event)
                 if url_event is not None:
                     # inherit web spider distance from parent (don't increment)
                     source_web_spider_distance = getattr(event, "web_spider_distance", 0)
                     url_event.web_spider_distance = source_web_spider_distance
                     await self.emit_event(url_event)
 
+        # speculate URL_UNVERIFIED from URL or any event with "url" attribute
+        event_is_url = event.type == "URL"
+        event_has_url = isinstance(event.data, dict) and "url" in event.data
+        if event_is_url or event_has_url:
+            if event_is_url:
+                url = event.data
+            else:
+                url = event.data["url"]
+            if not any(e.type == "URL_UNVERIFIED" and e.data == url for e in event.get_sources()):
+                tags = None
+                if self.helpers.is_spider_danger(event.source, url):
+                    tags = ["spider-danger"]
+                await self.emit_event(url, "URL_UNVERIFIED", tags=tags, source=event)
+
         # from hosts
         if speculate_open_ports:
             # don't act on unresolved DNS_NAMEs
             usable_dns = False
             if event.type == "DNS_NAME":
                 if (not self.dns_resolution) or ("a-record" in event.tags or "aaaa-record" in event.tags):
                     usable_dns = True
@@ -137,15 +149,17 @@
         org_stubs = set()
         if event.type == "DNS_NAME" and event.scope_distance == 0:
             tldextracted = self.helpers.tldextract(event.data)
             registered_domain = getattr(tldextracted, "registered_domain", "")
             if registered_domain:
                 tld_stub = getattr(tldextracted, "domain", "")
                 if tld_stub:
-                    org_stubs.add(tld_stub)
+                    decoded_tld_stub = self.helpers.smart_decode_punycode(tld_stub)
+                    org_stubs.add(decoded_tld_stub)
+                    org_stubs.add(self.helpers.unidecode(decoded_tld_stub))
         elif event.type == "SOCIAL":
             stub = event.data.get("stub", "")
             if stub:
                 org_stubs.add(stub.lower())
         elif event.type == "AZURE_TENANT":
             tenant_names = event.data.get("tenant-names", [])
             org_stubs.update(set(tenant_names))
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/internetdb.py` & `bbot-1.1.8.3321rc0/bbot/modules/internetdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/ip2location.py` & `bbot-1.1.8.3321rc0/bbot/modules/ip2location.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.8.3321rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/ipstack.py` & `bbot-1.1.8.3321rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/leakix.py` & `bbot-1.1.8.3321rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/masscan.py` & `bbot-1.1.8.3321rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/massdns.py` & `bbot-1.1.8.3321rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/myssl.py` & `bbot-1.1.8.3321rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/newsletters.py` & `bbot-1.1.8.3321rc0/bbot/modules/newsletters.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/nmap.py` & `bbot-1.1.8.3321rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/ntlm.py` & `bbot-1.1.8.3321rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/oauth.py` & `bbot-1.1.8.3321rc0/bbot/modules/oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/otx.py` & `bbot-1.1.8.3321rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/asset_inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -312,15 +312,15 @@
                 if severity_int > self.risk_rating:
                     self.risk_rating = severity_int
 
         if event.type == "TECHNOLOGY":
             self.technologies.add(event.data["technology"])
 
         if event.type == "WAF":
-            if waf := event.data.get("WAF", ""):
+            if waf := event.data.get("waf", ""):
                 if update_http_status or not self.waf:
                     self.waf = waf
 
         if event.type == "HTTP_RESPONSE":
             if title := event.data.get("title", ""):
                 if update_http_status or not self.http_title:
                     self.http_title = title
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/base.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
         return True, "precheck succeeded"
 
     async def _event_postcheck(self, event):
         acceptable, reason = await super()._event_postcheck(event)
         if acceptable and not event._stats_recorded and event.type not in ("FINISHED",):
             event._stats_recorded = True
-            self.scan.stats.event_distributed(event)
             self.scan.stats.event_produced(event)
         return acceptable, reason
 
     def is_incoming_duplicate(self, event, add=False):
         is_incoming_duplicate, reason = super().is_incoming_duplicate(event, add=add)
         # make exception for graph-important events
         if self._is_graph_important(event):
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/csv.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/discord.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/discord.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/emails.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/emails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/http.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/human.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/json.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/slack.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/slack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/splunk.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/splunk.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/subdomains.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/teams.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/teams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/web_report.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/output/websocket.py` & `bbot-1.1.8.3321rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.8.3321rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.8.3321rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.8.3321rc0/bbot/modules/paramminer_headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,17 @@
         elif len(group) > 1 or (len(group) == 1 and len(reasons) == 0):
             for group_slice in self.helpers.split_list(group):
                 match, reasons, reflection, subject_response = await self.check_batch(compare_helper, url, group_slice)
                 if match == False:
                     async for r in self.binary_search(compare_helper, url, group_slice, reasons, reflection):
                         yield r
         else:
-            self.warning(f"Submitted group of size 0 to binary_search()")
+            self.debug(
+                f"binary_search() failed to start with group of size {str(len(group))} and {str(len(reasons))} length reasons"
+            )
 
     async def check_batch(self, compare_helper, url, header_list):
         rand = self.rand_string()
         test_headers = {}
         for header in header_list:
             test_headers[header] = rand
         return await compare_helper.compare(url, headers=test_headers, check_reflection=(len(header_list) == 1))
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/passivetotal.py` & `bbot-1.1.8.3321rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/pgp.py` & `bbot-1.1.8.3321rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/postman.py` & `bbot-1.1.8.3321rc0/bbot/modules/postman.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/rapiddns.py` & `bbot-1.1.8.3321rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.8.3321rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/report/asn.py` & `bbot-1.1.8.3321rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/riddler.py` & `bbot-1.1.8.3321rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/robots.py` & `bbot-1.1.8.3321rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/secretsdb.py` & `bbot-1.1.8.3321rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/securitytrails.py` & `bbot-1.1.8.3321rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.8.3321rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/sitedossier.py` & `bbot-1.1.8.3321rc0/bbot/modules/sitedossier.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/skymem.py` & `bbot-1.1.8.3321rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/smuggler.py` & `bbot-1.1.8.3321rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/sslcert.py` & `bbot-1.1.8.3321rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/subdomaincenter.py` & `bbot-1.1.8.3321rc0/bbot/modules/subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/sublist3r.py` & `bbot-1.1.8.3321rc0/bbot/modules/sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/telerik.py` & `bbot-1.1.8.3321rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/templates/bucket.py` & `bbot-1.1.8.3321rc0/bbot/modules/templates/bucket.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,20 +41,21 @@
         if event.type == "DNS_NAME":
             await self.handle_dns_name(event)
         elif event.type == "STORAGE_BUCKET":
             await self.handle_storage_bucket(event)
 
     async def handle_dns_name(self, event):
         buckets = set()
-        base = event.data
+        base = self.helpers.unidecode(self.helpers.smart_decode_punycode(event.data))
         stem = self.helpers.domain_stem(base)
         for b in [base, stem]:
             split = b.split(".")
             for d in self.delimiters:
-                buckets.add(d.join(split))
+                bucket_name = d.join(split)
+                buckets.add(bucket_name)
         async for bucket_name, url, tags in self.brute_buckets(buckets, permutations=self.permutations):
             await self.emit_event({"name": bucket_name, "url": url}, "STORAGE_BUCKET", source=event, tags=tags)
 
     async def handle_storage_bucket(self, event):
         url = event.data["url"]
         bucket_name = event.data["name"]
         if self.supports_open_check:
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/templates/github.py` & `bbot-1.1.8.3321rc0/bbot/modules/templates/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/templates/portscanner.py` & `bbot-1.1.8.3321rc0/bbot/modules/templates/portscanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/templates/shodan.py` & `bbot-1.1.8.3321rc0/bbot/modules/templates/shodan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/templates/subdomain_enum.py` & `bbot-1.1.8.3321rc0/bbot/modules/templates/subdomain_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/templates/webhook.py` & `bbot-1.1.8.3321rc0/bbot/modules/templates/webhook.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/threatminer.py` & `bbot-1.1.8.3321rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/trufflehog.py` & `bbot-1.1.8.3321rc0/bbot/modules/trufflehog.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 class trufflehog(BaseModule):
     watched_events = ["FILESYSTEM"]
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["passive", "safe"]
     meta = {"description": "TruffleHog is a tool for finding credentials"}
 
     options = {
-        "version": "3.69.0",
+        "version": "3.75.1",
         "only_verified": True,
         "concurrency": 8,
     }
     options_desc = {
         "version": "trufflehog version",
         "only_verified": "Only report credentials that have been verified",
         "concurrency": "Number of concurrent workers",
@@ -33,41 +33,42 @@
     scope_distance_modifier = 2
 
     async def setup(self):
         self.verified = self.config.get("only_verified", True)
         self.concurrency = int(self.config.get("concurrency", 8))
         return True
 
-    async def filter_event(self, event):
-        if event.type == "FILESYSTEM":
-            if "git" not in event.tags and "docker" not in event.tags:
-                return False, "event is not a git repository or a docker image"
-        return True
-
     async def handle_event(self, event):
         path = event.data["path"]
+        description = event.data.get("description", "")
         if "git" in event.tags:
             module = "git"
         elif "docker" in event.tags:
             module = "docker"
+        else:
+            module = "filesystem"
         async for decoder_name, detector_name, raw_result, verified, source_metadata in self.execute_trufflehog(
             module, path
         ):
             if verified:
                 data = {
                     "severity": "High",
                     "description": f"Verified Secret Found. Detector Type: [{detector_name}] Decoder Type: [{decoder_name}] Secret: [{raw_result}] Details: [{source_metadata}]",
                     "host": str(event.source.host),
                 }
+                if description:
+                    data["description"] += f" Description: [{description}]"
                 await self.emit_event(data, "VULNERABILITY", event)
             else:
                 data = {
                     "description": f"Potential Secret Found. Detector Type: [{detector_name}] Decoder Type: [{decoder_name}] Secret: [{raw_result}] Details: [{source_metadata}]",
                     "host": str(event.source.host),
                 }
+                if description:
+                    data["description"] += f" Description: [{description}]"
                 await self.emit_event(data, "FINDING", event)
 
     async def execute_trufflehog(self, module, path):
         command = [
             "trufflehog",
             "--json",
         ]
@@ -76,14 +77,17 @@
         command.append("--concurrency=" + str(self.concurrency))
         if module == "git":
             command.append("git")
             command.append("file://" + path)
         elif module == "docker":
             command.append("docker")
             command.append("--image=file://" + path)
+        elif module == "filesystem":
+            command.append("filesystem")
+            command.append(path)
 
         stats_file = self.helpers.tempfile_tail(callback=self.log_trufflehog_status)
         try:
             with open(stats_file, "w") as stats_fh:
                 async for line in self.helpers.run_live(command, stderr=stats_fh):
                     try:
                         j = json.loads(line)
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.8.3321rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/urlscan.py` & `bbot-1.1.8.3321rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/viewdns.py` & `bbot-1.1.8.3321rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/virustotal.py` & `bbot-1.1.8.3321rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/wafw00f.py` & `bbot-1.1.8.3321rc0/bbot/modules/wafw00f.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,22 +34,22 @@
 
     async def handle_event(self, event):
         url = f"{event.parsed.scheme}://{event.parsed.netloc}/"
         WW = await self.scan.run_in_executor(wafw00f_main.WAFW00F, url, followredirect=False)
         waf_detections = await self.scan.run_in_executor(WW.identwaf)
         if waf_detections:
             for waf in waf_detections:
-                await self.emit_event({"host": str(event.host), "url": url, "WAF": waf}, "WAF", source=event)
+                await self.emit_event({"host": str(event.host), "url": url, "waf": waf}, "WAF", source=event)
         else:
             if self.config.get("generic_detect") == True:
                 generic = await self.scan.run_in_executor(WW.genericdetect)
                 if generic:
                     await self.emit_event(
                         {
                             "host": str(event.host),
                             "url": url,
-                            "WAF": "generic detection",
+                            "waf": "generic detection",
                             "info": WW.knowledge["generic"]["reason"],
                         },
                         "WAF",
                         source=event,
                     )
```

### Comparing `bbot-1.1.7.7rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.8.3321rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/wayback.py` & `bbot-1.1.8.3321rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/modules/zoomeye.py` & `bbot-1.1.8.3321rc0/bbot/modules/zoomeye.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     options = {"api_key": "", "max_pages": 20, "include_related": False}
     options_desc = {
         "api_key": "ZoomEye API key",
         "max_pages": "How many pages of results to fetch",
         "include_related": "Include domains which may be related to the target",
     }
 
-    base_url = "https://api.zoomeye.org"
+    base_url = "https://api.zoomeye.hk"
 
     async def setup(self):
         self.max_pages = self.config.get("max_pages", 20)
         self.headers = {"API-KEY": self.config.get("api_key", "")}
         self.include_related = self.config.get("include_related", False)
         return await super().setup()
```

### Comparing `bbot-1.1.7.7rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.8.3321rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/scanner/manager.py` & `bbot-1.1.8.3321rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/scanner/scanner.py` & `bbot-1.1.8.3321rc0/bbot/scanner/scanner.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,15 +395,21 @@
                 except BBOTError as e:
                     self.critical(f"Error during scan: {e}")
 
                 except Exception:
                     self.critical(f"Unexpected error during scan:\n{traceback.format_exc()}")
 
         finally:
-            self._cancel_tasks()
+            tasks = self._cancel_tasks()
+            self.debug(f"Awaiting {len(tasks):,} tasks")
+            for task in tasks:
+                self.debug(f"Awaiting {task}")
+                with contextlib.suppress(BaseException):
+                    await task
+            self.debug(f"Awaited {len(tasks):,} tasks")
             await self._report()
             await self._cleanup()
 
             log_fn = self.hugesuccess
             if self.status == "ABORTING":
                 self.status = "ABORTED"
                 log_fn = self.hugewarning
@@ -561,21 +567,22 @@
 
         Returns:
             None
         """
         if not self._stopping:
             self._stopping = True
             self.status = "ABORTING"
-            self.hugewarning(f"Aborting scan")
+            self.hugewarning("Aborting scan")
             self.trace()
             self._cancel_tasks()
             self._drain_queues()
             self.helpers.kill_children()
             self._drain_queues()
             self.helpers.kill_children()
+            self.debug("Finished aborting scan")
 
     async def finish(self):
         """Finalizes the scan by invoking the `finished()` method on all active modules if new activity is detected.
 
         The method is idempotent and will return False if no new activity has been recorded since the last invocation.
 
         Returns:
@@ -630,14 +637,15 @@
         and the scan manager. After collecting these tasks, it cancels them synchronously
         using a helper function. Finally, it shuts down the process pool, canceling any
         pending futures.
 
         Returns:
             None
         """
+        self.debug("Cancelling all scan tasks")
         tasks = []
         # module workers
         for m in self.modules.values():
             tasks += getattr(m, "_tasks", [])
         # init events
         if self.init_events_task:
             tasks.append(self.init_events_task)
@@ -647,14 +655,16 @@
         # dispatcher
         tasks += self.dispatcher_tasks
         # manager worker loops
         tasks += self._manager_worker_loop_tasks
         self.helpers.cancel_tasks_sync(tasks)
         # process pool
         self.process_pool.shutdown(cancel_futures=True)
+        self.debug("Finished cancelling all scan tasks")
+        return tasks
 
     async def _report(self):
         """Asynchronously executes the `report()` method for each module in the scan.
 
         This method is called once at the end of each scan and is responsible for
         triggering the `report()` function for each module. It executes irrespective
         of whether the scan was aborted or completed successfully. The method makes
```

### Comparing `bbot-1.1.7.7rc0/bbot/scanner/stats.py` & `bbot-1.1.8.3321rc0/bbot/scanner/stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,21 +12,16 @@
 
 class ScanStats:
     def __init__(self, scan):
         self.scan = scan
         self.module_stats = {}
         self.events_emitted_by_type = {}
 
-    def event_distributed(self, event):
-        _increment(self.events_emitted_by_type, event.type)
-        module_stat = self.get(event.module)
-        if module_stat is not None:
-            module_stat.increment_emitted(event)
-
     def event_produced(self, event):
+        _increment(self.events_emitted_by_type, event.type)
         module_stat = self.get(event.module)
         if module_stat is not None:
             module_stat.increment_produced(event)
 
     def event_consumed(self, event, module):
         module_stat = self.get(module)
         if module_stat is not None:
@@ -70,26 +65,19 @@
             table += [["None", "None", "None"]]
         return table[1:], table[0]
 
 
 class ModuleStat:
     def __init__(self, module):
         self.module = module
-
-        self.emitted = {}
-        self.emitted_total = 0
         self.produced = {}
         self.produced_total = 0
         self.consumed = {}
         self.consumed_total = 0
 
-    def increment_emitted(self, event):
-        self.emitted_total += 1
-        _increment(self.emitted, event.type)
-
     def increment_produced(self, event):
         self.produced_total += 1
         _increment(self.produced, event.type)
 
     def increment_consumed(self, event):
         if event.type not in ("FINISHED",):
             self.consumed_total += 1
```

### Comparing `bbot-1.1.7.7rc0/bbot/scanner/target.py` & `bbot-1.1.8.3321rc0/bbot/scanner/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import logging
 import ipaddress
 from contextlib import suppress
 
 from bbot.core.errors import *
 from bbot.modules.base import BaseModule
 from bbot.core.event import make_event, is_event
@@ -82,14 +83,18 @@
             - If you are instantiating a target from within a BBOT module, use `self.helpers.make_target()` instead. (this removes the need to pass in a scan object.)
             - The strict_scope flag can be set to restrict scope calculation to only exactly-matching hosts and not their child subdomains.
             - Each target is processed and stored as an `Event` in the '_events' dictionary.
         """
         self.scan = scan
         self.strict_scope = strict_scope
         self.make_in_scope = make_in_scope
+        self.special_event_types = {
+            "ORG_STUB": re.compile(r"^ORG:(.*)", re.IGNORECASE),
+            "ASN": re.compile(r"^ASN:(.*)", re.IGNORECASE),
+        }
 
         self._dummy_module = TargetDummyModule(scan)
         self._events = dict()
         if len(targets) > 0:
             log.verbose(f"Creating events from {len(targets):,} targets")
         for t in targets:
             self.add_target(t)
@@ -120,27 +125,33 @@
                     self._events[k].update(v)
                 except KeyError:
                     self._events[k] = set(t._events[k])
         else:
             if is_event(t):
                 event = t
             else:
+                for eventtype, regex in self.special_event_types.items():
+                    match = regex.match(t)
+                    if match:
+                        t = match.groups()[0]
+                        event_type = eventtype
+                        break
                 try:
                     event = self.scan.make_event(
                         t,
                         event_type=event_type,
                         source=self.scan.root_event,
                         module=self._dummy_module,
                         tags=["target"],
                     )
                 except ValidationError as e:
                     # allow commented lines
                     if not str(t).startswith("#"):
                         raise ValidationError(f'Could not add target "{t}": {e}')
-            if self.make_in_scope:
+            if self.make_in_scope and event.host:
                 event.scope_distance = 0
             try:
                 self._events[event.host].add(event)
             except KeyError:
                 self._events[event.host] = {
                     event,
                 }
```

### Comparing `bbot-1.1.7.7rc0/bbot/scripts/docs.py` & `bbot-1.1.8.3321rc0/bbot/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.8.3321rc0/bbot/test/bbot_fixtures.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,33 +49,14 @@
 def bbot_scanner():
     from bbot.scanner import Scanner
 
     return Scanner
 
 
 @pytest.fixture
-def neograph(monkeypatch, helpers):
-    helpers.depsinstaller.pip_install(["py2neo"])
-
-    class NeoGraph:
-        def __init__(self, *args, **kwargs):
-            pass
-
-        def merge(self, *args, **kwargs):
-            return True
-
-    import py2neo
-
-    monkeypatch.setattr(py2neo, "Graph", NeoGraph)
-    from bbot.db.neo4j import Neo4j
-
-    return Neo4j(uri="bolt://127.0.0.1:1111")
-
-
-@pytest.fixture
 def scan(monkeypatch, bbot_config):
     from bbot.scanner import Scanner
 
     bbot_scan = Scanner("127.0.0.1", modules=["ipneighbor"], config=bbot_config)
 
     fallback_nameservers_file = bbot_scan.helpers.bbot_home / "fallback_nameservers.txt"
     with open(fallback_nameservers_file, "w") as f:
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/conftest.py` & `bbot-1.1.8.3321rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/run_tests.sh` & `bbot-1.1.8.3321rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test.conf` & `bbot-1.1.8.3321rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,14 +115,20 @@
         "HTTP_RESPONSE",
         dummy=True,
     )
     assert http_response.http_status == 301
     assert http_response.http_title == "HTTP RESPONSE"
     assert http_response.redirect_location == "http://www.evilcorp.com/asdf"
 
+    # http response url validation
+    http_response_2 = scan.make_event(
+        {"port": "80", "url": "http://evilcorp.com:80/asdf"}, "HTTP_RESPONSE", dummy=True
+    )
+    assert http_response_2.data["url"] == "http://evilcorp.com/asdf"
+
     # open port tests
     assert events.open_port in events.domain
     assert "api.publicapis.org:443" in events.open_port
     assert "bad.publicapis.org:443" not in events.open_port
     assert "publicapis.org:443" not in events.open_port
     assert events.ipv4_open_port in events.ipv4
     assert events.ipv4_open_port in events.netv4
@@ -194,14 +200,31 @@
         affiliate_event = scan.make_event("1.2.3.4", source=root_event, tags=tag)
         assert tag in affiliate_event.tags
         affiliate_event2 = scan.make_event("1.2.3.4:88", source=affiliate_event)
         affiliate_event3 = scan.make_event("4.3.2.1:88", source=affiliate_event)
         assert tag in affiliate_event2.tags
         assert tag not in affiliate_event3.tags
 
+    # updating an already-created event with make_event()
+    # updating tags
+    event1 = scan.make_event("127.0.0.1", source=scan.root_event)
+    updated_event = scan.make_event(event1, tags="asdf")
+    assert "asdf" not in event1.tags
+    assert "asdf" in updated_event.tags
+    # updating source
+    event2 = scan.make_event("127.0.0.1", source=scan.root_event)
+    updated_event = scan.make_event(event2, source=event1)
+    assert event2.source == scan.root_event
+    assert updated_event.source == event1
+    # updating module
+    event3 = scan.make_event("127.0.0.1", source=scan.root_event)
+    updated_event = scan.make_event(event3, internal=True)
+    assert event3.internal == False
+    assert updated_event.internal == True
+
     # event sorting
     parent1 = scan.make_event("127.0.0.1", source=scan.root_event)
     parent2 = scan.make_event("127.0.0.1", source=scan.root_event)
     parent2_child1 = scan.make_event("127.0.0.1", source=parent2)
     parent1_child1 = scan.make_event("127.0.0.1", source=parent1)
     parent1_child2 = scan.make_event("127.0.0.1", source=parent1)
     parent1_child2_child1 = scan.make_event("127.0.0.1", source=parent1_child2)
@@ -417,7 +440,16 @@
     event_2 = scan.make_event("127.0.0.2", source=event_1)
     event_3 = scan.make_event("127.0.0.3", source=event_2)
     event_3._omit = True
     event_4 = scan.make_event("127.0.0.4", source=event_3)
     event_5 = scan.make_event("127.0.0.5", source=event_4)
     assert event_5.get_sources() == [event_4, event_3, event_2, event_1, scan.root_event]
     assert event_5.get_sources(omit=True) == [event_4, event_2, event_1, scan.root_event]
+
+    # test storage bucket validation
+    bucket_event = scan.make_event(
+        {"name": "ASDF.s3.amazonaws.com", "url": "https://ASDF.s3.amazonaws.com"},
+        "STORAGE_BUCKET",
+        source=scan.root_event,
+    )
+    assert bucket_event.data["name"] == "asdf.s3.amazonaws.com"
+    assert bucket_event.data["url"] == "https://asdf.s3.amazonaws.com/"
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_manager_deduplication.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_manager_deduplication.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""
+The tests in this file are a bit unique because they're not intended to test any specific functionality
+
+They are meant to be a thorough baseline of how different modules and BBOT systems interact
+Basically, if there is a small change in how scope works, dns resolution, etc., these tests are designed to catch it.
+They will show you how your change affects bbot's behavior across a wide range of scans and configurations.
+
+I know they suck but they exist for a reason. If one of these tests is failing for you, it's important to take the time and
+understand exactly what changed and why (and whether it's okay) before changing the test to match your results.
+"""
+
 from ..bbot_fixtures import *  # noqa: F401
 
 from pytest_httpserver import HTTPServer
 
 
 @pytest.fixture
 def bbot_other_httpservers():
@@ -320,51 +331,55 @@
     assert 1 == len([e for e in events if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
     assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.0"])
     assert 1 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
     assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888"])
     assert 1 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in events if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
     assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888"])
+    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/"])
     assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/"])
     assert 1 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
     assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888"])
 
-    assert len(all_events) == 13
+    assert len(all_events) == 14
     assert 1 == len([e for e in all_events if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.0" and e.internal == True and e.scope_distance == 0])
     assert 2 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888" and e.internal == True and e.scope_distance == 0])
     assert 2 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
+    assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0 and "spider-danger" in e.tags])
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == True and e.scope_distance == 1])
 
-    assert len(all_events_nodups) == 11
+    assert len(all_events_nodups) == 12
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.0" and e.internal == True and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888" and e.internal == True and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
+    assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0 and "spider-danger" in e.tags])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == True and e.scope_distance == 1])
 
     for _graph_output_events in (graph_output_events, graph_output_batch_events):
         assert len(_graph_output_events) == 6
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.0"])
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888"])
         assert 1 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
         assert 1 == len([e for e in _graph_output_events if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888"])
+        assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/"])
         assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/"])
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
         assert 0 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888"])
 
     # httpx/speculate IP_RANGE --> IP_ADDRESS --> OPEN_TCP_PORT --> URL, search distance = 0, in_scope_only = False
     events, all_events, all_events_nodups, graph_output_events, graph_output_batch_events = await do_scan(
         "127.0.0.1/31",
@@ -384,46 +399,49 @@
     assert 1 == len([e for e in events if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
     assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.0"])
     assert 1 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
     assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888"])
     assert 1 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in events if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
     assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888"])
+    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/"])
     assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/"])
     assert 1 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in events if e.type == "URL" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.77:8888"])
     assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.88"])
     assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/"])
 
-    assert len(all_events) == 18
+    assert len(all_events) == 19
     assert 1 == len([e for e in all_events if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.0" and e.internal == True and e.scope_distance == 0])
     assert 2 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888" and e.internal == True and e.scope_distance == 0])
     assert 2 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
+    assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0 and "spider-danger" in e.tags])
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
     assert 2 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "URL" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.88" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.88:8888/" and e.internal == True and e.scope_distance == 2])
 
-    assert len(all_events_nodups) == 15
+    assert len(all_events_nodups) == 16
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.0" and e.internal == True and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888" and e.internal == True and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
+    assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0 and "spider-danger" in e.tags])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.88" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.88:8888/" and e.internal == True and e.scope_distance == 2])
@@ -433,14 +451,15 @@
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.0"])
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888"])
         assert 1 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
         assert 1 == len([e for e in _graph_output_events if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888"])
+        assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/"])
         assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/"])
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
         assert 1 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
         assert 1 == len([e for e in _graph_output_events if e.type == "URL" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
         assert 0 == len([e for e in _graph_output_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.77:8888"])
         assert 0 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.88"])
         assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.88:8888/"])
@@ -464,60 +483,61 @@
     assert 1 == len([e for e in events if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
     assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.0"])
     assert 1 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
     assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888"])
     assert 1 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in events if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
     assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888"])
+    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/"])
     assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/"])
     assert 1 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in events if e.type == "URL" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.77:8888"])
     assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.88"])
     assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/"])
 
-    assert len(all_events) == 23
+    assert len(all_events) == 24
     assert 1 == len([e for e in all_events if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.0" and e.internal == True and e.scope_distance == 0])
     assert 2 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888" and e.internal == True and e.scope_distance == 0])
     assert 2 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
+    assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0 and "spider-danger" in e.tags])
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
     assert 2 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "URL" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.88:8888/" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.88" and e.internal == True and e.scope_distance == 2])
-    assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.88" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.88:8888" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events if e.type == "URL" and e.data == "http://127.0.0.88:8888/" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.88:8888" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.99:8888/" and e.internal == True and e.scope_distance == 3])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.99" and e.internal == True and e.scope_distance == 3])
 
-    assert len(all_events_nodups) == 20
+    assert len(all_events_nodups) == 21
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.0" and e.internal == True and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888" and e.internal == True and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
+    assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0 and "spider-danger" in e.tags])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.88:8888/" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.88" and e.internal == True and e.scope_distance == 2])
-    assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.88" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.88:8888" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL" and e.data == "http://127.0.0.88:8888/" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events_nodups if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.88:8888" and e.internal == True and e.scope_distance == 2])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.99:8888/" and e.internal == True and e.scope_distance == 3])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.99" and e.internal == True and e.scope_distance == 3])
 
     for _graph_output_events in (graph_output_events, graph_output_batch_events):
@@ -525,14 +545,15 @@
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_RANGE" and e.data == "127.0.0.0/31" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.0"])
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.1" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.0:8888"])
         assert 1 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.1:8888" and e.internal == False and e.scope_distance == 0])
         assert 1 == len([e for e in _graph_output_events if e.type == "URL" and e.data == "http://127.0.0.1:8888/" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.1:8888"])
+        assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.1:8888/"])
         assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.77:8888/"])
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.77" and e.internal == False and e.scope_distance == 1])
         assert 1 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.77:8888" and e.internal == False and e.scope_distance == 1])
         assert 1 == len([e for e in _graph_output_events if e.type == "URL" and e.data == "http://127.0.0.77:8888/" and e.internal == False and e.scope_distance == 1])
         assert 0 == len([e for e in _graph_output_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.77:8888"])
         assert 0 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.88"])
         assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.88:8888/"])
@@ -551,47 +572,49 @@
             "internal_modules": {"speculate": {"ports": "8888"}},
             "omit_event_types": ["HTTP_RESPONSE", "URL_UNVERIFIED"],
         },
     )
 
     assert len(events) == 11
     assert 1 == len([e for e in events if e.type == "IP_RANGE" and e.data == "127.0.0.110/31" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.110" and e.internal == True and e.scope_distance == 0])
+    assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.110"])
     assert 1 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.111" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.110:8888" and e.internal == True and e.scope_distance == 0])
+    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.110:8888"])
     assert 1 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.111:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in events if e.type == "URL" and e.data == "http://127.0.0.111:8888/" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.111:8888" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.222:8889/" and e.internal == False and e.scope_distance == 0])
+    assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.111:8888"])
+    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.111:8888/"])
+    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.222:8889/"])
     assert 1 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.222" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.33:8889/" and e.internal == False and e.scope_distance == 0])
+    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.33:8889/"])
     assert 1 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.33" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.222:8888" and e.internal == True and e.scope_distance == 0])
+    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.222:8888"])
     assert 1 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.222:8889" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.33:8888" and e.internal == True and e.scope_distance == 0])
+    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.33:8888"])
     assert 1 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.33:8889" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in events if e.type == "URL" and e.data == "http://127.0.0.222:8889/" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.222:8889" and e.internal == False and e.scope_distance == 0])
+    assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.222:8889"])
     assert 1 == len([e for e in events if e.type == "URL" and e.data == "http://127.0.0.33:8889/" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.33:8889" and e.internal == False and e.scope_distance == 0])
-    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.44:8888/" and e.internal == True and e.scope_distance == 1])
-    assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.44" and e.internal == True and e.scope_distance == 1])
-    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.55:8888/" and e.internal == True and e.scope_distance == 1])
-    assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.55" and e.internal == True and e.scope_distance == 1])
-    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.44:8888" and e.internal == True and e.scope_distance == 1])
-    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.55:8888" and e.internal == True and e.scope_distance == 1])
+    assert 0 == len([e for e in events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.33:8889"])
+    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.44:8888/"])
+    assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.44"])
+    assert 0 == len([e for e in events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.55:8888/"])
+    assert 0 == len([e for e in events if e.type == "IP_ADDRESS" and e.data == "127.0.0.55"])
+    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.44:8888"])
+    assert 0 == len([e for e in events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.55:8888"])
 
-    assert len(all_events) == 30
+    assert len(all_events) == 31
     assert 1 == len([e for e in all_events if e.type == "IP_RANGE" and e.data == "127.0.0.110/31" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.110" and e.internal == True and e.scope_distance == 0])
     assert 2 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.111" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.110:8888" and e.internal == True and e.scope_distance == 0])
     assert 2 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.111:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "URL" and e.data == "http://127.0.0.111:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.111:8888" and e.internal == False and e.scope_distance == 0])
+    assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.111:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.222:8889/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.222" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.33:8889/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.33" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.222:8888" and e.internal == True and e.scope_distance == 0])
     assert 2 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.222:8889" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.33:8888" and e.internal == True and e.scope_distance == 0])
@@ -603,22 +626,23 @@
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.44:8888/" and e.internal == True and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.44" and e.internal == True and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.55:8888/" and e.internal == True and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.55" and e.internal == True and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.44:8888" and e.internal == True and e.scope_distance == 1])
     assert 1 == len([e for e in all_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.55:8888" and e.internal == True and e.scope_distance == 1])
 
-    assert len(all_events_nodups) == 26
+    assert len(all_events_nodups) == 27
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_RANGE" and e.data == "127.0.0.110/31" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.110" and e.internal == True and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.111" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.110:8888" and e.internal == True and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.111:8888" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL" and e.data == "http://127.0.0.111:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.111:8888" and e.internal == False and e.scope_distance == 0])
+    assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.111:8888/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.222:8889/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.222" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.33:8889/" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "IP_ADDRESS" and e.data == "127.0.0.33" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.222:8888" and e.internal == True and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.222:8889" and e.internal == False and e.scope_distance == 0])
     assert 1 == len([e for e in all_events_nodups if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.33:8888" and e.internal == True and e.scope_distance == 0])
@@ -639,14 +663,15 @@
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_RANGE" and e.data == "127.0.0.110/31" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.110"])
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.111" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.110:8888"])
         assert 1 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.111:8888" and e.internal == False and e.scope_distance == 0])
         assert 1 == len([e for e in _graph_output_events if e.type == "URL" and e.data == "http://127.0.0.111:8888/" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "HTTP_RESPONSE" and e.data["input"] == "127.0.0.111:8888"])
+        assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.111:8888/"])
         assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.222:8889/"])
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.222"])
         assert 0 == len([e for e in _graph_output_events if e.type == "URL_UNVERIFIED" and e.data == "http://127.0.0.33:8889/"])
         assert 1 == len([e for e in _graph_output_events if e.type == "IP_ADDRESS" and e.data == "127.0.0.33"])
         assert 0 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.222:8888"])
         assert 1 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.222:8889" and e.internal == False and e.scope_distance == 0])
         assert 0 == len([e for e in _graph_output_events if e.type == "OPEN_TCP_PORT" and e.data == "127.0.0.33:8888"])
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -332,50 +332,59 @@
             "asdf.evilcorp.com": {"A": ["127.0.254.3"]},
         },
     )
 
     scan.modules["dummy"] = dummy(scan)
     events = [e async for e in scan.async_start()]
 
-    assert len(events) == 6
+    assert len(events) == 7
     assert 1 == len([e for e in events if e.type == "SCAN"])
     assert 2 == len([e for e in events if e.type == "DNS_NAME"])
     assert 1 == len([e for e in events if e.type == "DNS_NAME" and e.data == "evilcorp.com"])
     # the reason we don't have a DNS_NAME for www.evilcorp.com is because FINDING.quick_emit = True
     assert 0 == len([e for e in events if e.type == "DNS_NAME" and e.data == "www.evilcorp.com"])
     assert 1 == len([e for e in events if e.type == "DNS_NAME" and e.data == "asdf.evilcorp.com"])
     assert 1 == len([e for e in events if e.type == "ORG_STUB" and e.data == "evilcorp"])
     assert 1 == len([e for e in events if e.type == "FINDING"])
+    assert 1 == len([e for e in events if e.type == "URL_UNVERIFIED"])
 
     assert scan.stats.events_emitted_by_type == {
         "SCAN": 1,
         "DNS_NAME": 2,
         "URL": 1,
+        "URL_UNVERIFIED": 1,
         "FINDING": 1,
         "ORG_STUB": 1,
     }
 
     assert set(scan.stats.module_stats) == {"host", "speculate", "python", "dummy", "TARGET"}
 
     target_stats = scan.stats.module_stats["TARGET"]
-    assert target_stats.emitted == {"SCAN": 1, "DNS_NAME": 1}
-    assert target_stats.emitted_total == 2
     assert target_stats.produced == {"SCAN": 1, "DNS_NAME": 1}
     assert target_stats.produced_total == 2
     assert target_stats.consumed == {}
     assert target_stats.consumed_total == 0
 
     dummy_stats = scan.stats.module_stats["dummy"]
-    assert dummy_stats.emitted == {"FINDING": 1, "URL": 1}
-    assert dummy_stats.emitted_total == 2
     assert dummy_stats.produced == {"FINDING": 1, "URL": 1}
     assert dummy_stats.produced_total == 2
-    assert dummy_stats.consumed == {"DNS_NAME": 2, "OPEN_TCP_PORT": 1, "SCAN": 1, "URL": 1}
-    assert dummy_stats.consumed_total == 5
+    assert dummy_stats.consumed == {"DNS_NAME": 2, "OPEN_TCP_PORT": 1, "SCAN": 1, "URL": 1, "URL_UNVERIFIED": 1}
+    assert dummy_stats.consumed_total == 6
 
     python_stats = scan.stats.module_stats["python"]
-    assert python_stats.emitted == {}
-    assert python_stats.emitted_total == 0
     assert python_stats.produced == {}
     assert python_stats.produced_total == 0
-    assert python_stats.consumed == {"DNS_NAME": 2, "FINDING": 1, "ORG_STUB": 1, "SCAN": 1, "URL": 1}
-    assert python_stats.consumed_total == 6
+    assert python_stats.consumed == {
+        "DNS_NAME": 2,
+        "FINDING": 1,
+        "ORG_STUB": 1,
+        "SCAN": 1,
+        "URL": 1,
+        "URL_UNVERIFIED": 1,
+    }
+    assert python_stats.consumed_total == 7
+
+    speculate_stats = scan.stats.module_stats["speculate"]
+    assert speculate_stats.produced == {"URL_UNVERIFIED": 1, "ORG_STUB": 1}
+    assert speculate_stats.produced_total == 2
+    assert speculate_stats.consumed == {"URL": 1, "DNS_NAME": 2, "URL_UNVERIFIED": 1}
+    assert speculate_stats.consumed_total == 4
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_regexes.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 
 @pytest.mark.asyncio
 async def test_scan(
     events,
     bbot_config,
     helpers,
-    neograph,
     monkeypatch,
     bbot_scanner,
     mock_dns,
 ):
     scan0 = bbot_scanner(
         "1.1.1.1/31",
         "evilcorp.com",
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from ..bbot_fixtures import *  # noqa: F401
 
 
-def test_target(bbot_config, bbot_scanner):
+@pytest.mark.asyncio
+async def test_target(bbot_config, bbot_scanner):
     scan1 = bbot_scanner("api.publicapis.org", "8.8.8.8/30", "2001:4860:4860::8888/126", config=bbot_config)
     scan2 = bbot_scanner("8.8.8.8/29", "publicapis.org", "2001:4860:4860::8888/125", config=bbot_config)
     scan3 = bbot_scanner("8.8.8.8/29", "publicapis.org", "2001:4860:4860::8888/125", config=bbot_config)
     scan4 = bbot_scanner("8.8.8.8/29", config=bbot_config)
     scan5 = bbot_scanner(config=bbot_config)
     assert not scan5.target
     assert len(scan1.target) == 9
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,20 @@
     }
 
     async def setup_before_prep(self, module_test):
         module_test.httpx_mock.add_response(
             url=f"https://api.dehashed.com/search?query=domain:blacklanternsecurity.com&size=10000&page=1",
             json=dehashed_domain_response,
         )
+        module_test.mock_dns(
+            {
+                "bob.com": {"A": ["127.0.0.1"]},
+                "blacklanternsecurity.com": {"A": ["127.0.0.1"]},
+            }
+        )
 
     def check(self, module_test, events):
         assert len(events) == 11
         assert 1 == len([e for e in events if e.type == "DNS_NAME" and e.data == "blacklanternsecurity.com"])
         assert 1 == len([e for e in events if e.type == "ORG_STUB" and e.data == "blacklanternsecurity"])
         assert 1 == len(
             [
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_discord.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_discord.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_emails.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_emails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         )
         module_test.httpserver.expect_request("/nonhttpredirect/").respond_with_data(
             "", status=302, headers={"Location": "awb://127.0.0.1:7777"}
         )
         module_test.httpserver.no_handler_status_code = 404
 
     def check(self, module_test, events):
-        assert 1 == len(
+        assert 2 == len(
             [
                 e
                 for e in events
                 if e.type == "URL_UNVERIFIED" and e.data == "https://www.test.notreal/yep" and e.scope_distance == 1
             ]
         )
         assert 1 == len([e for e in events if e.type == "URL" and e.data == "http://127.0.0.1:8888/relative/owa/"])
@@ -256,19 +256,23 @@
     <a href="http://127.0.0.1:8888/25"/>
     """
 
     async def setup_before_prep(self, module_test):
         module_test.httpserver.expect_request("/").respond_with_data(self.lots_of_links)
 
     def check(self, module_test, events):
-        url_events = [e for e in events if e.type == "URL_UNVERIFIED"]
-        assert len(url_events) == 26
-        url_data = [e.data for e in url_events if "spider-danger" not in e.tags]
+        url_unverified_events = [e for e in events if e.type == "URL_UNVERIFIED"]
+        # base URL + 25 links (10 w/o spider-danger) + 10 links (extracted from HTTP_RESPONSES, w/ spider-danger) == 36
+        assert len(url_unverified_events) == 36
+        url_data = [e.data for e in url_unverified_events if "spider-danger" not in e.tags]
+        assert len(url_data) == 11
         assert "http://127.0.0.1:8888/10" in url_data
         assert "http://127.0.0.1:8888/11" not in url_data
+        url_events = [e for e in events if e.type == "URL"]
+        assert len(url_events) == 11
 
 
 class TestExcavateCSP(TestExcavate):
     csp_test_header = "default-src 'self'; script-src test.asdf.fakedomain; object-src 'none';"
 
     async def setup_before_prep(self, module_test):
         expect_args = {"method": "GET", "uri": "/"}
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
             ]
         ), "Failed to emit URL_UNVERIFIED"
         assert 1 == len(
             [
                 e
                 for e in events
                 if e.type == "CODE_REPOSITORY"
+                and "git" in e.tags
                 and e.data["url"] == "https://github.com/projectdiscovery/nuclei"
                 and e.scope_distance == 1
             ]
         ), "Failed to emit CODE_REPOSITORY"
         assert 1 == len(
             [e for e in events if e.type == "URL" and e.data == self.github_file_url and e.scope_distance == 1]
         ), "Failed to visit URL"
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py`

 * *Files 6% similar despite different names*

```diff
@@ -314,14 +314,15 @@
             ]
         ), "Failed to find TheTechromancer github"
         assert 1 == len(
             [
                 e
                 for e in events
                 if e.type == "CODE_REPOSITORY"
+                and "git" in e.tags
                 and e.data["url"] == "https://github.com/blacklanternsecurity/test_keys"
                 and e.scope_distance == 1
             ]
         ), "Failed to find blacklanternsecurity github repo"
 
 
 class TestGithub_Org_No_Members(TestGithub_Org):
@@ -357,11 +358,64 @@
     def check(self, module_test, events):
         assert len(events) == 7
         assert 1 == len(
             [
                 e
                 for e in events
                 if e.type == "CODE_REPOSITORY"
+                and "git" in e.tags
                 and e.data["url"] == "https://github.com/TheTechromancer/websitedemo"
                 and e.scope_distance == 2
             ]
         ), "Found to find TheTechromancer github repo"
+
+
+class TestGithub_Org_Custom_Target(TestGithub_Org):
+    targets = ["ORG:blacklanternsecurity"]
+    config_overrides = {"scope_report_distance": 10, "omit_event_types": [], "speculate": True}
+
+    def check(self, module_test, events):
+        assert len(events) == 7
+        assert 1 == len(
+            [e for e in events if e.type == "ORG_STUB" and e.data == "blacklanternsecurity" and e.scope_distance == 1]
+        )
+        assert 1 == len(
+            [
+                e
+                for e in events
+                if e.type == "SOCIAL"
+                and e.data["platform"] == "github"
+                and e.data["profile_name"] == "blacklanternsecurity"
+                and e.scope_distance == 1
+            ]
+        )
+        assert 1 == len(
+            [e for e in events if e.type == "DNS_NAME" and e.data == "github.com" and e.scope_distance == 1]
+        )
+        assert 1 == len(
+            [
+                e
+                for e in events
+                if e.type == "URL_UNVERIFIED"
+                and e.data == "https://github.com/blacklanternsecurity"
+                and e.scope_distance == 1
+            ]
+        )
+        assert 1 == len(
+            [
+                e
+                for e in events
+                if e.type == "CODE_REPOSITORY"
+                and e.data["url"] == "https://github.com/blacklanternsecurity/test_keys"
+                and e.scope_distance == 1
+            ]
+        )
+        assert 1 == len(
+            [
+                e
+                for e in events
+                if e.type == "SOCIAL"
+                and e.data["platform"] == "github"
+                and e.data["profile_name"] == "TheTechromancer"
+                and e.scope_distance == 2
+            ]
+        )
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,18 +25,18 @@
         request_args = dict(uri="/blacklanternsecurity")
         respond_args = dict(response_data="""blacklanternsecurity github <a data-bem""")
         module_test.set_expect_requests(request_args, respond_args)
 
         # monkeypatch social
         old_emit_event = module_test.scan.modules["social"].emit_event
 
-        async def new_emit_event(event_data, event_type, **kwargs):
-            if event_data["url"] == "https://github.com/blacklanternsecurity":
-                event_data["url"] = event_data["url"].replace("https://github.com", "http://127.0.0.1:8888")
-            await old_emit_event(event_data, event_type, **kwargs)
+        async def new_emit_event(event):
+            if event.data["url"] == "https://github.com/blacklanternsecurity":
+                event.data["url"] = event.data["url"].replace("https://github.com", "http://127.0.0.1:8888")
+            await old_emit_event(event)
 
         module_test.monkeypatch.setattr(module_test.scan.modules["social"], "emit_event", new_emit_event)
 
     def check(self, module_test, events):
         screenshots_path = self.home_dir / "scans" / module_test.scan.name / "gowitness" / "screenshots"
         screenshots = list(screenshots_path.glob("*.png"))
         assert (
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_json.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,37 @@
 from .base import ModuleTestBase
 
 
 class TestNeo4j(ModuleTestBase):
     async def setup_before_prep(self, module_test):
-        # install py2neo
+        # install neo4j
         deps_pip = module_test.preloaded["neo4j"]["deps"]["pip"]
         await module_test.scan.helpers.depsinstaller.pip_install(deps_pip)
 
-        class MockGraph:
+        self.neo4j_used = False
+
+        class MockResult:
+            async def single(s):
+                self.neo4j_used = True
+                return {"id(_)": 1}
+
+        class MockSession:
+            async def run(s, *args, **kwargs):
+                return MockResult()
+
+            async def close(self):
+                pass
+
+        class MockDriver:
             def __init__(self, *args, **kwargs):
-                self.used = False
+                pass
+
+            def session(self, *args, **kwargs):
+                return MockSession()
 
-            def merge(self, *args, **kwargs):
-                self.used = True
+            async def close(self):
+                pass
 
-        module_test.monkeypatch.setattr("py2neo.Graph", MockGraph)
+        module_test.monkeypatch.setattr("neo4j.AsyncGraphDatabase.driver", MockDriver)
 
     def check(self, module_test, events):
-        assert module_test.scan.modules["neo4j"].neo4j.graph.used == True
+        assert self.neo4j_used == True
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_postman.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_postman.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,25 +7,42 @@
 
     async def setup_after_prep(self, module_test):
         expect_args = {"method": "GET", "uri": "/"}
         respond_args = {
             "response_data": """
             <html>
                 <a href="https://discord.gg/asdf"/><a href="https://github.com/blacklanternsecurity/bbot"/>
+                <a href="https://hub.docker.com/r/blacklanternsecurity"/>
                 <a href="https://hub.docker.com/r/blacklanternsecurity/bbot"/>
+                <a href="https://hub.docker.com/r/blacklanternSECURITY/bbot"/>
             </html>
             """
         }
         module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
 
     def check(self, module_test, events):
-        assert any(
-            e.type == "SOCIAL" and e.data["platform"] == "discord" and e.data["profile_name"] == "asdf" for e in events
+        assert 3 == len([e for e in events if e.type == "SOCIAL"])
+        assert 1 == len(
+            [
+                e
+                for e in events
+                if e.type == "SOCIAL" and e.data["platform"] == "discord" and e.data["profile_name"] == "asdf"
+            ]
         )
-        assert any(
-            e.type == "SOCIAL" and e.data["platform"] == "docker" and e.data["profile_name"] == "blacklanternsecurity"
-            for e in events
+        assert 1 == len(
+            [
+                e
+                for e in events
+                if e.type == "SOCIAL"
+                and e.data["platform"] == "docker"
+                and e.data["profile_name"] == "blacklanternsecurity"
+            ]
         )
-        assert any(
-            e.type == "SOCIAL" and e.data["platform"] == "github" and e.data["profile_name"] == "blacklanternsecurity"
-            for e in events
+        assert 1 == len(
+            [
+                e
+                for e in events
+                if e.type == "SOCIAL"
+                and e.data["platform"] == "github"
+                and e.data["profile_name"] == "blacklanternsecurity"
+            ]
         )
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_teams.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_teams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     async def setup_after_prep(self, module_test):
         expect_args = {"method": "GET", "uri": "/"}
         respond_args = {"response_data": "Proudly powered by litespeed web server"}
         module_test.set_expect_requests(expect_args=expect_args, respond_args=respond_args)
 
     def check(self, module_test, events):
-        assert any(e.type == "WAF" and "LiteSpeed" in e.data["WAF"] for e in events)
+        assert any(e.type == "WAF" and "LiteSpeed" in e.data["waf"] for e in events)
 
 
 class TestWafw00f_noredirect(ModuleTestBase):
     targets = ["http://127.0.0.1:8888"]
     modules_overrides = ["httpx", "wafw00f"]
 
     async def setup_after_prep(self, module_test):
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 
 
 class TestZoomEye(ModuleTestBase):
     config_overrides = {"modules": {"zoomeye": {"api_key": "asdf", "include_related": True, "max_pages": 3}}}
 
     async def setup_before_prep(self, module_test):
         module_test.httpx_mock.add_response(
-            url="https://api.zoomeye.org/resources-info",
+            url="https://api.zoomeye.hk/resources-info",
             match_headers={"API-KEY": "asdf"},
             json={"quota_info": {"remain_total_quota": 5}},
         )
         module_test.httpx_mock.add_response(
-            url="https://api.zoomeye.org/domain/search?q=blacklanternsecurity.com&type=0&page=1",
+            url="https://api.zoomeye.hk/domain/search?q=blacklanternsecurity.com&type=0&page=1",
             json={"list": [{"name": "asdf.blacklanternsecurity.com"}]},
         )
         module_test.httpx_mock.add_response(
-            url="https://api.zoomeye.org/domain/search?q=blacklanternsecurity.com&type=0&page=2",
+            url="https://api.zoomeye.hk/domain/search?q=blacklanternsecurity.com&type=0&page=2",
             json={"list": [{"name": "zzzz.blacklanternsecurity.com"}]},
         )
         module_test.httpx_mock.add_response(
-            url="https://api.zoomeye.org/domain/search?q=blacklanternsecurity.com&type=0&page=3",
+            url="https://api.zoomeye.hk/domain/search?q=blacklanternsecurity.com&type=0&page=3",
             json={"list": [{"name": "ffff.blacklanternsecurity.com"}, {"name": "affiliate.bls"}]},
         )
         module_test.httpx_mock.add_response(
-            url="https://api.zoomeye.org/domain/search?q=blacklanternsecurity.com&type=0&page=4",
+            url="https://api.zoomeye.hk/domain/search?q=blacklanternsecurity.com&type=0&page=4",
             json={"list": [{"name": "nope.blacklanternsecurity.com"}]},
         )
 
     def check(self, module_test, events):
         assert any(e.data == "asdf.blacklanternsecurity.com" for e in events), "Failed to detect subdomain #1"
         assert any(e.data == "zzzz.blacklanternsecurity.com" for e in events), "Failed to detect subdomain #2"
         assert any(e.data == "ffff.blacklanternsecurity.com" for e in events), "Failed to detect subdomain #3"
```

### Comparing `bbot-1.1.7.7rc0/bbot/test/testsslcert.pem` & `bbot-1.1.8.3321rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/test/testsslkey.pem` & `bbot-1.1.8.3321rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.8.3321rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/wordlists/ms_on_prem_subdomains.txt` & `bbot-1.1.8.3321rc0/bbot/wordlists/ms_on_prem_subdomains.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.8.3321rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.8.3321rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.8.3321rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.8.3321rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.8.3321rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.1.7.7rc0/pyproject.toml` & `bbot-1.1.8.3321rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.1.7.7rc"
+version = "v1.1.8.3321rc"
 description = "OSINT automation for hackers."
 authors = [
     "TheTechromancer",
     "Paul Mueller",
 ]
 license = "GPL-3.0"
 readme = "README.md"
@@ -26,15 +26,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 omegaconf = "^2.3.0"
 psutil = "^5.9.4"
 wordninja = "^2.0.0"
 ansible-runner = "^2.3.2"
-deepdiff = "^6.2.3"
+deepdiff = ">=6.2.3,<8.0.0"
 xmltojson = "^2.0.2"
 pycryptodome = "^3.17"
 idna = "^3.4"
 ansible = ">=7.3,<9.0"
 tabulate = "0.8.10"
 websockets = ">=11.0.2,<13.0.0"
 pyjwt = "^2.7.0"
@@ -43,27 +43,28 @@
 dnspython = "^2.4.2"
 pydantic = "^2.4.2"
 httpx = "^0.26.0"
 cloudcheck = ">=2.1.0.181,<4.0.0.0"
 tldextract = "^5.1.1"
 cachetools = "^5.3.2"
 socksio = "^1.0.0"
+unidecode = "^1.3.8"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = ">=6,<8"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 poetry-dynamic-versioning = ">=0.21.4,<1.3.0"
 pytest-rerunfailures = ">=11.1.2,<15.0.0"
 pytest-asyncio = ">=0.21,<0.24"
 urllib3 = "^2.0.2"
 werkzeug = ">=2.3.4,<4.0.0"
 pytest-httpserver = "^1.0.8"
 pytest-env = ">=0.8.2,<1.2.0"
 pytest-timeout = "^2.1.0"
-pytest = "^7.4.0"
+pytest = ">=7.4,<9.0"
 pre-commit = "^3.4.0"
 black = "^24.1.1"
 pytest-httpx = "^0.29.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.2"
 mkdocs-extra-sass-plugin = "^0.1.0"
@@ -86,11 +87,11 @@
 [tool.black]
 line-length = 119
 extend-exclude = "(test_step_1/test_manager_*)"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 metadata = false
-format-jinja = 'v1.1.7{% if branch == "dev" %}.{{ distance }}rc{% endif %}'
+format-jinja = 'v1.1.8{% if branch == "dev" %}.{{ distance }}rc{% endif %}'
 
 [tool.poetry-dynamic-versioning.substitution]
 files = ["*/__init__.py"]
```

### Comparing `bbot-1.1.7.7rc0/PKG-INFO` & `bbot-1.1.8.3321rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.1.7.7rc0
+Version: 1.1.8.3321rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Keywords: python,cli,automation,osint,neo4j,scanner,python-library,hacking,recursion,pentesting,recon,command-line-tool,bugbounty,subdomains,security-tools,subdomain-scanner,osint-framework,attack-surface,subdomain-enumeration,osint-tool
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,27 +16,28 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Requires-Dist: ansible (>=7.3,<9.0)
 Requires-Dist: ansible-runner (>=2.3.2,<3.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: cachetools (>=5.3.2,<6.0.0)
 Requires-Dist: cloudcheck (>=2.1.0.181,<4.0.0.0)
-Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
+Requires-Dist: deepdiff (>=6.2.3,<8.0.0)
 Requires-Dist: dnspython (>=2.4.2,<3.0.0)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: idna (>=3.4,<4.0)
 Requires-Dist: lxml (>=4.9.2,<6.0.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
 Requires-Dist: psutil (>=5.9.4,<6.0.0)
 Requires-Dist: pycryptodome (>=3.17,<4.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pyjwt (>=2.7.0,<3.0.0)
 Requires-Dist: socksio (>=1.0.0,<2.0.0)
 Requires-Dist: tabulate (==0.8.10)
 Requires-Dist: tldextract (>=5.1.1,<6.0.0)
+Requires-Dist: unidecode (>=1.3.8,<2.0.0)
 Requires-Dist: websockets (>=11.0.2,<13.0.0)
 Requires-Dist: wordninja (>=2.0.0,<3.0.0)
 Requires-Dist: xmltojson (>=2.0.2,<3.0.0)
 Project-URL: Documentation, https://www.blacklanternsecurity.com/bbot/
 Project-URL: Discord, https://discord.com/invite/PZqkgxu5SA
 Project-URL: Docker Hub, https://hub.docker.com/r/blacklanternsecurity/bbot
 Project-URL: Repository, https://github.com/blacklanternsecurity/bbot
@@ -304,37 +305,38 @@
 
 ![subdomain-stats-ebay](https://github.com/blacklanternsecurity/bbot/assets/20261699/53e07e9f-50b6-4b70-9e83-297dbfbcb436)
 
 ## BBOT Modules By Flag
 For a full list of modules, including the data types consumed and emitted by each one, see [List of Modules](https://www.blacklanternsecurity.com/bbot/modules/list_of_modules/).
 
 <!-- BBOT MODULE FLAGS -->
-| Flag             | # Modules   | Description                                        | Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
-|------------------|-------------|----------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| safe             | 78          | Non-intrusive, safe to run                         | affiliates, aggregate, ajaxpro, anubisdb, asn, azure_realm, azure_tenant, baddns, baddns_zone, badsecrets, bevigil, binaryedge, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, dockerhub, emailformat, filedownload, fingerprintx, fullhunt, git, git_clone, github_codesearch, github_org, gowitness, hackertarget, httpx, hunt, hunterio, iis_shortnames, internetdb, ip2location, ipstack, leakix, myssl, newsletters, ntlm, oauth, otx, passivetotal, pgp, postman, rapiddns, riddler, robots, secretsdb, securitytrails, shodan_dns, sitedossier, skymem, social, sslcert, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wappalyzer, wayback, zoomeye |
-| passive          | 58          | Never connects to target systems                   | affiliates, aggregate, anubisdb, asn, azure_realm, azure_tenant, bevigil, binaryedge, bucket_file_enum, builtwith, c99, censys, certspotter, chaos, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, emailformat, excavate, fullhunt, git_clone, github_codesearch, github_org, hackertarget, hunterio, internetdb, ip2location, ipneighbor, ipstack, leakix, massdns, myssl, otx, passivetotal, pgp, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, skymem, social, speculate, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wayback, zoomeye                                                                                                                                                                                                                                         |
-| subdomain-enum   | 45          | Enumerates subdomains                              | anubisdb, asn, azure_realm, azure_tenant, baddns_zone, bevigil, binaryedge, builtwith, c99, censys, certspotter, chaos, columbus, crt, digitorus, dnscommonsrv, dnsdumpster, fullhunt, github_codesearch, github_org, hackertarget, httpx, hunterio, internetdb, ipneighbor, leakix, massdns, myssl, oauth, otx, passivetotal, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, sslcert, subdomaincenter, subdomains, threatminer, urlscan, virustotal, wayback, zoomeye                                                                                                                                                                                                                                                                                                                                                                                      |
-| active           | 42          | Makes active connections to target systems         | ajaxpro, baddns, baddns_zone, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dockerhub, dotnetnuke, ffuf, ffuf_shortnames, filedownload, fingerprintx, generic_ssrf, git, gowitness, host_header, httpx, hunt, iis_shortnames, masscan, newsletters, nmap, ntlm, nuclei, oauth, paramminer_cookies, paramminer_getparams, paramminer_headers, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, vhost, wafw00f, wappalyzer                                                                                                                                                                                                                                                                                                                                                                    |
-| web-thorough     | 29          | More advanced web scanning functionality           | ajaxpro, azure_realm, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf_shortnames, filedownload, generic_ssrf, git, host_header, httpx, hunt, iis_shortnames, nmap, ntlm, oauth, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-| aggressive       | 20          | Generates a large amount of network traffic        | bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, generic_ssrf, host_header, ipneighbor, masscan, massdns, nmap, nuclei, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, telerik, url_manipulation, vhost, wafw00f                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
-| web-basic        | 17          | Basic, non-intrusive web scan functionality        | azure_realm, baddns, badsecrets, bucket_amazon, bucket_azure, bucket_firebase, bucket_google, filedownload, git, httpx, iis_shortnames, ntlm, oauth, robots, secretsdb, sslcert, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
-| cloud-enum       | 12          | Enumerates cloud resources                         | azure_realm, azure_tenant, baddns, baddns_zone, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, httpx, oauth                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
-| slow             | 9           | May take a long time to complete                   | bucket_digitalocean, dastardly, fingerprintx, git_clone, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
-| affiliates       | 8           | Discovers affiliated hostnames/domains             | affiliates, azure_realm, azure_tenant, builtwith, oauth, sslcert, viewdns, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
-| email-enum       | 7           | Enumerates email addresses                         | dehashed, emailformat, emails, hunterio, pgp, skymem, sslcert                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| deadly           | 4           | Highly aggressive                                  | dastardly, ffuf, nuclei, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
-| portscan         | 3           | Discovers open ports                               | internetdb, masscan, nmap                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
-| web-paramminer   | 3           | Discovers HTTP parameters through brute-force      | paramminer_cookies, paramminer_getparams, paramminer_headers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| baddns           | 2           | Runs all modules from the DNS auditing tool BadDNS | baddns, baddns_zone                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
-| iis-shortnames   | 2           | Scans for IIS Shortname vulnerability              | ffuf_shortnames, iis_shortnames                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
-| report           | 2           | Generates a report at the end of the scan          | affiliates, asn                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
-| social-enum      | 2           | Enumerates social media                            | httpx, social                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
-| service-enum     | 1           | Identifies protocols running on open ports         | fingerprintx                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
-| subdomain-hijack | 1           | Detects hijackable subdomains                      | baddns                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
-| web-screenshots  | 1           | Takes screenshots of web pages                     | gowitness                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| Flag             | # Modules   | Description                                        | Modules                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
+|------------------|-------------|----------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
+| safe             | 82          | Non-intrusive, safe to run                         | affiliates, aggregate, ajaxpro, anubisdb, asn, azure_realm, azure_tenant, baddns, baddns_zone, badsecrets, bevigil, binaryedge, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, builtwith, c99, censys, certspotter, chaos, code_repository, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, docker_pull, dockerhub, emailformat, filedownload, fingerprintx, fullhunt, git, git_clone, github_codesearch, github_org, github_workflows, gitlab, gowitness, hackertarget, httpx, hunt, hunterio, iis_shortnames, internetdb, ip2location, ipstack, leakix, myssl, newsletters, ntlm, oauth, otx, passivetotal, pgp, postman, rapiddns, riddler, robots, secretsdb, securitytrails, shodan_dns, sitedossier, skymem, social, sslcert, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wappalyzer, wayback, zoomeye |
+| passive          | 62          | Never connects to target systems                   | affiliates, aggregate, anubisdb, asn, azure_realm, azure_tenant, bevigil, binaryedge, bucket_file_enum, builtwith, c99, censys, certspotter, chaos, code_repository, columbus, credshed, crobat, crt, dehashed, digitorus, dnscommonsrv, dnsdumpster, docker_pull, dockerhub, emailformat, excavate, fullhunt, git_clone, github_codesearch, github_org, github_workflows, hackertarget, hunterio, internetdb, ip2location, ipneighbor, ipstack, leakix, massdns, myssl, otx, passivetotal, pgp, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, skymem, social, speculate, subdomaincenter, sublist3r, threatminer, trufflehog, urlscan, viewdns, virustotal, wayback, zoomeye                                                                                                                                                                                                                                      |
+| subdomain-enum   | 45          | Enumerates subdomains                              | anubisdb, asn, azure_realm, azure_tenant, baddns_zone, bevigil, binaryedge, builtwith, c99, censys, certspotter, chaos, columbus, crt, digitorus, dnscommonsrv, dnsdumpster, fullhunt, github_codesearch, github_org, hackertarget, httpx, hunterio, internetdb, ipneighbor, leakix, massdns, myssl, oauth, otx, passivetotal, postman, rapiddns, riddler, securitytrails, shodan_dns, sitedossier, sslcert, subdomaincenter, subdomains, threatminer, urlscan, virustotal, wayback, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| active           | 42          | Makes active connections to target systems         | ajaxpro, baddns, baddns_zone, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, filedownload, fingerprintx, generic_ssrf, git, gitlab, gowitness, host_header, httpx, hunt, iis_shortnames, masscan, newsletters, nmap, ntlm, nuclei, oauth, paramminer_cookies, paramminer_getparams, paramminer_headers, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, vhost, wafw00f, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| web-thorough     | 29          | More advanced web scanning functionality           | ajaxpro, azure_realm, badsecrets, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_firebase, bucket_google, bypass403, dastardly, dotnetnuke, ffuf_shortnames, filedownload, generic_ssrf, git, host_header, httpx, hunt, iis_shortnames, nmap, ntlm, oauth, robots, secretsdb, smuggler, sslcert, telerik, url_manipulation, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+| aggressive       | 20          | Generates a large amount of network traffic        | bypass403, dastardly, dotnetnuke, ffuf, ffuf_shortnames, generic_ssrf, host_header, ipneighbor, masscan, massdns, nmap, nuclei, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, telerik, url_manipulation, vhost, wafw00f                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
+| web-basic        | 17          | Basic, non-intrusive web scan functionality        | azure_realm, baddns, badsecrets, bucket_amazon, bucket_azure, bucket_firebase, bucket_google, filedownload, git, httpx, iis_shortnames, ntlm, oauth, robots, secretsdb, sslcert, wappalyzer                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
+| cloud-enum       | 12          | Enumerates cloud resources                         | azure_realm, azure_tenant, baddns, baddns_zone, bucket_amazon, bucket_azure, bucket_digitalocean, bucket_file_enum, bucket_firebase, bucket_google, httpx, oauth                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
+| slow             | 10          | May take a long time to complete                   | bucket_digitalocean, dastardly, docker_pull, fingerprintx, git_clone, paramminer_cookies, paramminer_getparams, paramminer_headers, smuggler, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| affiliates       | 8           | Discovers affiliated hostnames/domains             | affiliates, azure_realm, azure_tenant, builtwith, oauth, sslcert, viewdns, zoomeye                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
+| email-enum       | 7           | Enumerates email addresses                         | dehashed, emailformat, emails, hunterio, pgp, skymem, sslcert                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| deadly           | 4           | Highly aggressive                                  | dastardly, ffuf, nuclei, vhost                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
+| portscan         | 3           | Discovers open ports                               | internetdb, masscan, nmap                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
+| web-paramminer   | 3           | Discovers HTTP parameters through brute-force      | paramminer_cookies, paramminer_getparams, paramminer_headers                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| baddns           | 2           | Runs all modules from the DNS auditing tool BadDNS | baddns, baddns_zone                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
+| iis-shortnames   | 2           | Scans for IIS Shortname vulnerability              | ffuf_shortnames, iis_shortnames                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| report           | 2           | Generates a report at the end of the scan          | affiliates, asn                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| social-enum      | 2           | Enumerates social media                            | httpx, social                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
+| repo-enum        | 1           | Enumerates code repositories                       | code_repository                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
+| service-enum     | 1           | Identifies protocols running on open ports         | fingerprintx                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
+| subdomain-hijack | 1           | Detects hijackable subdomains                      | baddns                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
+| web-screenshots  | 1           | Takes screenshots of web pages                     | gowitness                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
 <!-- END BBOT MODULE FLAGS -->
 
 ## BBOT Output Modules
 BBOT can save its data to TXT, CSV, JSON, and tons of other destinations including [Neo4j](https://www.blacklanternsecurity.com/bbot/scanning/output/#neo4j), [Splunk](https://www.blacklanternsecurity.com/bbot/scanning/output/#splunk), and [Discord](https://www.blacklanternsecurity.com/bbot/scanning/output/#discord-slack-teams). For instructions on how to use these, see [Output Modules](https://www.blacklanternsecurity.com/bbot/scanning/output). 
 
 <!-- BBOT OUTPUT MODULES -->
 | Module          | Type   | Needs API Key   | Description                                                                             | Flags          | Consumed Events                                                                                  | Produced Events           |
```

