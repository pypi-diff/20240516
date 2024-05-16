# Comparing `tmp/aa_gdpr-0.4.2.tar.gz` & `tmp/aa_gdpr-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_gdpr-0.4.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_gdpr-0.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_gdpr-0.4.2.tar` & `aa_gdpr-0.4.3.tar`

### file list

```diff
@@ -1,367 +1,367 @@
--rw-r--r--   0        0        0     1069 2024-05-12 06:52:37.979464 aa_gdpr-0.4.2/LICENSE
--rw-r--r--   0        0        0     3068 2024-05-12 06:52:37.979464 aa_gdpr-0.4.2/README.md
--rw-r--r--   0        0        0       97 2024-05-12 06:52:37.979464 aa_gdpr-0.4.2/aagdpr/__init__.py
--rw-r--r--   0        0        0      238 2024-05-12 06:52:37.979464 aa_gdpr-0.4.2/aagdpr/app_settings.py
--rw-r--r--   0        0        0      180 2024-05-12 06:52:37.979464 aa_gdpr-0.4.2/aagdpr/apps.py
--rw-r--r--   0        0        0   232803 2024-05-12 06:52:37.980465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css
--rw-r--r--   0        0        0    60635 2024-05-12 06:52:37.981464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootstrap/5.3.3/js/bootstrap.min.js
--rw-r--r--   0        0        0     1297 2024-05-12 06:52:37.981464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/_bootswatch.scss
--rw-r--r--   0        0        0     5804 2024-05-12 06:52:37.981464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/_variables.scss
--rw-r--r--   0        0        0   281028 2024-05-12 06:52:37.982464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.css
--rw-r--r--   0        0        0   230846 2024-05-12 06:52:37.983464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.min.css
--rw-r--r--   0        0        0    87361 2024-05-12 06:52:37.984465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.min.css.map
--rw-r--r--   0        0        0   280238 2024-05-12 06:52:37.985464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.rtl.css
--rw-r--r--   0        0        0   230950 2024-05-12 06:52:37.986464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.rtl.min.css
--rw-r--r--   0        0        0     2343 2024-05-12 06:52:37.986464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/fonts-lato.css
--rw-r--r--   0        0        0      986 2024-05-12 06:52:37.986464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/fonts-lato.min.css
--rw-r--r--   0        0        0     1153 2024-05-12 06:52:37.986464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/_bootswatch.scss
--rw-r--r--   0        0        0     3731 2024-05-12 06:52:37.986464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/_variables.scss
--rw-r--r--   0        0        0   281687 2024-05-12 06:52:37.987465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.css
--rw-r--r--   0        0        0   231635 2024-05-12 06:52:37.987465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.min.css
--rw-r--r--   0        0        0   280897 2024-05-12 06:52:37.988464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.rtl.css
--rw-r--r--   0        0        0   231739 2024-05-12 06:52:37.988464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.rtl.min.css
--rw-r--r--   0        0        0     2343 2024-05-12 06:52:37.988464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/fonts-lato.css
--rw-r--r--   0        0        0      986 2024-05-12 06:52:37.988464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/fonts-lato.min.css
--rw-r--r--   0        0        0    11938 2024-05-12 06:52:37.988464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/_bootswatch.scss
--rw-r--r--   0        0        0     3053 2024-05-12 06:52:37.989464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/_variables.scss
--rw-r--r--   0        0        0   308306 2024-05-12 06:52:37.989464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.css
--rw-r--r--   0        0        0   254640 2024-05-12 06:52:37.989464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.min.css
--rw-r--r--   0        0        0   307572 2024-05-12 06:52:37.990465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.rtl.css
--rw-r--r--   0        0        0   254797 2024-05-12 06:52:37.991464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.rtl.min.css
--rw-r--r--   0        0        0    11103 2024-05-12 06:52:37.991464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/fonts-roboto.css
--rw-r--r--   0        0        0     4740 2024-05-12 06:52:37.991464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/fonts-roboto.min.css
--rw-r--r--   0        0        0     9160 2024-05-12 06:52:37.991464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/clipboard.js/2.0.11/clipboard.min.js
--rw-r--r--   0        0        0    12123 2024-05-12 06:52:37.991464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/css/dataTables.bootstrap5.min.css
--rw-r--r--   0        0        0     2358 2024-05-12 06:52:37.991464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/js/dataTables.bootstrap5.min.js
--rw-r--r--   0        0        0    87238 2024-05-12 06:52:37.992464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/js/jquery.dataTables.min.js
--rw-r--r--   0        0        0     6402 2024-05-12 06:52:37.992464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/css/dataTables.bootstrap.min.css
--rw-r--r--   0        0        0     4401 2024-05-12 06:52:37.992464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/js/dataTables.bootstrap.min.js
--rw-r--r--   0        0        0    87897 2024-05-12 06:52:37.993465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/js/jquery.dataTables.min.js
--rw-r--r--   0        0        0    11174 2024-05-12 06:52:37.993465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/css/dataTables.bootstrap.min.css
--rw-r--r--   0        0        0    12123 2024-05-12 06:52:37.993465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/css/dataTables.bootstrap5.min.css
--rw-r--r--   0        0        0     2223 2024-05-12 06:52:37.993465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/dataTables.bootstrap.min.js
--rw-r--r--   0        0        0     2358 2024-05-12 06:52:37.993465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/dataTables.bootstrap5.min.js
--rw-r--r--   0        0        0    87238 2024-05-12 06:52:37.994464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/jquery.dataTables.min.js
--rw-r--r--   0        0        0     1548 2024-05-12 06:52:37.994464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/LICENSE.txt
--rw-r--r--   0        0        0    73577 2024-05-12 06:52:37.994464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/all.css
--rw-r--r--   0        0        0    59305 2024-05-12 06:52:37.995464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/all.min.css
--rw-r--r--   0        0        0      732 2024-05-12 06:52:37.995464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/brands.css
--rw-r--r--   0        0        0      675 2024-05-12 06:52:37.995464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/brands.min.css
--rw-r--r--   0        0        0    71942 2024-05-12 06:52:37.995464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/fontawesome.css
--rw-r--r--   0        0        0    57873 2024-05-12 06:52:37.996464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/fontawesome.min.css
--rw-r--r--   0        0        0      734 2024-05-12 06:52:37.996464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/regular.css
--rw-r--r--   0        0        0      677 2024-05-12 06:52:37.996464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/regular.min.css
--rw-r--r--   0        0        0      727 2024-05-12 06:52:37.996464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/solid.css
--rw-r--r--   0        0        0      669 2024-05-12 06:52:37.996464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/solid.min.css
--rw-r--r--   0        0        0     8077 2024-05-12 06:52:37.996464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/svg-with-js.css
--rw-r--r--   0        0        0     6359 2024-05-12 06:52:37.996464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/svg-with-js.min.css
--rw-r--r--   0        0        0    41312 2024-05-12 06:52:37.997465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/v4-shims.css
--rw-r--r--   0        0        0    26702 2024-05-12 06:52:37.997465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/v4-shims.min.css
--rw-r--r--   0        0        0   134294 2024-05-12 06:52:37.998464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.eot
--rw-r--r--   0        0        0   747470 2024-05-12 06:52:38.004464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.svg
--rw-r--r--   0        0        0   133988 2024-05-12 06:52:38.005464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    89988 2024-05-12 06:52:38.005464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.woff
--rw-r--r--   0        0        0    76736 2024-05-12 06:52:38.005464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    34034 2024-05-12 06:52:38.006464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.eot
--rw-r--r--   0        0        0   144562 2024-05-12 06:52:38.007465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.svg
--rw-r--r--   0        0        0    33736 2024-05-12 06:52:38.007465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    16276 2024-05-12 06:52:38.007465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.woff
--rw-r--r--   0        0        0    13224 2024-05-12 06:52:38.008464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   203030 2024-05-12 06:52:38.009464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.eot
--rw-r--r--   0        0        0   917989 2024-05-12 06:52:38.015464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.svg
--rw-r--r--   0        0        0   202744 2024-05-12 06:52:38.017464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   101648 2024-05-12 06:52:38.017464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.woff
--rw-r--r--   0        0        0    78268 2024-05-12 06:52:38.017464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     7427 2024-05-12 06:52:38.017464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/LICENSE.txt
--rw-r--r--   0        0        0   140292 2024-05-12 06:52:38.018464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/all.css
--rw-r--r--   0        0        0   102217 2024-05-12 06:52:38.018464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/all.min.css
--rw-r--r--   0        0        0    24006 2024-05-12 06:52:38.019464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/brands.css
--rw-r--r--   0        0        0    18855 2024-05-12 06:52:38.019464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/brands.min.css
--rw-r--r--   0        0        0   113421 2024-05-12 06:52:38.019464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/fontawesome.css
--rw-r--r--   0        0        0    80823 2024-05-12 06:52:38.019464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/fontawesome.min.css
--rw-r--r--   0        0        0      633 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/regular.css
--rw-r--r--   0        0        0      580 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/regular.min.css
--rw-r--r--   0        0        0      625 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/solid.css
--rw-r--r--   0        0        0      572 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/solid.min.css
--rw-r--r--   0        0        0    21637 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/svg-with-js.css
--rw-r--r--   0        0        0    16956 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/svg-with-js.min.css
--rw-r--r--   0        0        0     1831 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-font-face.css
--rw-r--r--   0        0        0     1736 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-font-face.min.css
--rw-r--r--   0        0        0    41574 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-shims.css
--rw-r--r--   0        0        0    27593 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-shims.min.css
--rw-r--r--   0        0        0      871 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v5-font-face.css
--rw-r--r--   0        0        0      794 2024-05-12 06:52:38.020465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v5-font-face.min.css
--rw-r--r--   0        0        0   189684 2024-05-12 06:52:38.022464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   109808 2024-05-12 06:52:38.022464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    63348 2024-05-12 06:52:38.022464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    24488 2024-05-12 06:52:38.023465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   394668 2024-05-12 06:52:38.025464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150020 2024-05-12 06:52:38.025464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10172 2024-05-12 06:52:38.025464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4568 2024-05-12 06:52:38.025464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0    60579 2024-05-12 06:52:38.026465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.full.min.js
--rw-r--r--   0        0        0    16503 2024-05-12 06:52:38.026465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.min.css
--rw-r--r--   0        0        0    51705 2024-05-12 06:52:38.026465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.min.js
--rw-r--r--   0        0        0     7142 2024-05-12 06:52:38.027464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0        0        0     7126 2024-05-12 06:52:38.027464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0        0        0     4670 2024-05-12 06:52:38.027464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png
--rw-r--r--   0        0        0     7163 2024-05-12 06:52:38.027464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png
--rw-r--r--   0        0        0     4670 2024-05-12 06:52:38.027464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0        0        0     6539 2024-05-12 06:52:38.027464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0        0        0    32131 2024-05-12 06:52:38.027464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/jquery-ui.min.css
--rw-r--r--   0        0        0   255083 2024-05-12 06:52:38.028464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/js/jquery-ui.min.js
--rw-r--r--   0        0        0      854 2024-05-12 06:52:38.029464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-visibility/1.0.11/jquery-visibility.min.js
--rw-r--r--   0        0        0    85578 2024-05-12 06:52:38.029464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery/2.2.4/jquery.min.js
--rw-r--r--   0        0        0    87533 2024-05-12 06:52:38.030465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery/3.7.1/jquery.min.js
--rw-r--r--   0        0        0    70264 2024-05-12 06:52:38.030465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery/3.7.1/jquery.slim.min.js
--rw-r--r--   0        0        0   149321 2024-05-12 06:52:38.031464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/less.js/4.2.0/less.min.js
--rw-r--r--   0        0        0     2149 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/af.js
--rw-r--r--   0        0        0     4449 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-dz.js
--rw-r--r--   0        0        0     1934 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-kw.js
--rw-r--r--   0        0        0     4648 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-ly.js
--rw-r--r--   0        0        0     1989 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-ma.js
--rw-r--r--   0        0        0     3042 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-sa.js
--rw-r--r--   0        0        0     1936 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-tn.js
--rw-r--r--   0        0        0     5072 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar.js
--rw-r--r--   0        0        0     2846 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/az.js
--rw-r--r--   0        0        0     5154 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/be.js
--rw-r--r--   0        0        0     2955 2024-05-12 06:52:38.032464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bg.js
--rw-r--r--   0        0        0     1784 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bm.js
--rw-r--r--   0        0        0     4349 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bn-bd.js
--rw-r--r--   0        0        0     3898 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bn.js
--rw-r--r--   0        0        0     4399 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bo.js
--rw-r--r--   0        0        0     4544 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/br.js
--rw-r--r--   0        0        0     4475 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bs.js
--rw-r--r--   0        0        0     3031 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ca.js
--rw-r--r--   0        0        0     6718 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cs.js
--rw-r--r--   0        0        0     2341 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cv.js
--rw-r--r--   0        0        0     2834 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cy.js
--rw-r--r--   0        0        0     1629 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/da.js
--rw-r--r--   0        0        0     2635 2024-05-12 06:52:38.033465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de-at.js
--rw-r--r--   0        0        0     2563 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de-ch.js
--rw-r--r--   0        0        0     2562 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de.js
--rw-r--r--   0        0        0     2464 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/dv.js
--rw-r--r--   0        0        0     3877 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/el.js
--rw-r--r--   0        0        0     2029 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-au.js
--rw-r--r--   0        0        0     1878 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-ca.js
--rw-r--r--   0        0        0     2035 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-gb.js
--rw-r--r--   0        0        0     2033 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-ie.js
--rw-r--r--   0        0        0     1871 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-il.js
--rw-r--r--   0        0        0     2029 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-in.js
--rw-r--r--   0        0        0     2038 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-nz.js
--rw-r--r--   0        0        0     2047 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-sg.js
--rw-r--r--   0        0        0     2338 2024-05-12 06:52:38.034464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/eo.js
--rw-r--r--   0        0        0     3441 2024-05-12 06:52:38.035464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-do.js
--rw-r--r--   0        0        0     3510 2024-05-12 06:52:38.035464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-mx.js
--rw-r--r--   0        0        0     3538 2024-05-12 06:52:38.035464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-us.js
--rw-r--r--   0        0        0     3498 2024-05-12 06:52:38.035464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es.js
--rw-r--r--   0        0        0     2631 2024-05-12 06:52:38.035464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/et.js
--rw-r--r--   0        0        0     1964 2024-05-12 06:52:38.035464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/eu.js
--rw-r--r--   0        0        0     3230 2024-05-12 06:52:38.035464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fa.js
--rw-r--r--   0        0        0     3632 2024-05-12 06:52:38.035464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fi.js
--rw-r--r--   0        0        0     1776 2024-05-12 06:52:38.035464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fil.js
--rw-r--r--   0        0        0     1772 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fo.js
--rw-r--r--   0        0        0     2104 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr-ca.js
--rw-r--r--   0        0        0     2263 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr-ch.js
--rw-r--r--   0        0        0     3471 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr.js
--rw-r--r--   0        0        0     2275 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fy.js
--rw-r--r--   0        0        0     2360 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ga.js
--rw-r--r--   0        0        0     2380 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gd.js
--rw-r--r--   0        0        0     2347 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gl.js
--rw-r--r--   0        0        0     5506 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gom-deva.js
--rw-r--r--   0        0        0     4130 2024-05-12 06:52:38.036465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gom-latn.js
--rw-r--r--   0        0        0     4132 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gu.js
--rw-r--r--   0        0        0     3211 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/he.js
--rw-r--r--   0        0        0     6421 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hi.js
--rw-r--r--   0        0        0     4718 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hr.js
--rw-r--r--   0        0        0     3815 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hu.js
--rw-r--r--   0        0        0     3236 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hy-am.js
--rw-r--r--   0        0        0     2375 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/id.js
--rw-r--r--   0        0        0     4458 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/is.js
--rw-r--r--   0        0        0     1941 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/it-ch.js
--rw-r--r--   0        0        0     3251 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/it.js
--rw-r--r--   0        0        0     3955 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ja.js
--rw-r--r--   0        0        0     2384 2024-05-12 06:52:38.037464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/jv.js
--rw-r--r--   0        0        0     3504 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ka.js
--rw-r--r--   0        0        0     2495 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/kk.js
--rw-r--r--   0        0        0     3362 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/km.js
--rw-r--r--   0        0        0     4252 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/kn.js
--rw-r--r--   0        0        0     2223 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ko.js
--rw-r--r--   0        0        0     3330 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ku.js
--rw-r--r--   0        0        0     2521 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ky.js
--rw-r--r--   0        0        0     4269 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lb.js
--rw-r--r--   0        0        0     2585 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lo.js
--rw-r--r--   0        0        0     4005 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lt.js
--rw-r--r--   0        0        0     3449 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lv.js
--rw-r--r--   0        0        0     3661 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/me.js
--rw-r--r--   0        0        0     2023 2024-05-12 06:52:38.038464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mi.js
--rw-r--r--   0        0        0     3021 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mk.js
--rw-r--r--   0        0        0     3287 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ml.js
--rw-r--r--   0        0        0     3414 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mn.js
--rw-r--r--   0        0        0     6574 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mr.js
--rw-r--r--   0        0        0     2330 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ms-my.js
--rw-r--r--   0        0        0     2277 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ms.js
--rw-r--r--   0        0        0     1684 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mt.js
--rw-r--r--   0        0        0     3094 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/my.js
--rw-r--r--   0        0        0     1899 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nb.js
--rw-r--r--   0        0        0     4031 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ne.js
--rw-r--r--   0        0        0     3169 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nl-be.js
--rw-r--r--   0        0        0     3202 2024-05-12 06:52:38.039464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nl.js
--rw-r--r--   0        0        0     1828 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nn.js
--rw-r--r--   0        0        0     2472 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/oc-lnc.js
--rw-r--r--   0        0        0     4198 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pa-in.js
--rw-r--r--   0        0        0     4166 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pl.js
--rw-r--r--   0        0        0     1854 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pt-br.js
--rw-r--r--   0        0        0     1968 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pt.js
--rw-r--r--   0        0        0     2319 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ro.js
--rw-r--r--   0        0        0     8418 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ru.js
--rw-r--r--   0        0        0     2153 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sd.js
--rw-r--r--   0        0        0     1849 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/se.js
--rw-r--r--   0        0        0     2681 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/si.js
--rw-r--r--   0        0        0     5173 2024-05-12 06:52:38.040464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sk.js
--rw-r--r--   0        0        0     6115 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sl.js
--rw-r--r--   0        0        0     1987 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sq.js
--rw-r--r--   0        0        0     4762 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sr-cyrl.js
--rw-r--r--   0        0        0     4209 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sr.js
--rw-r--r--   0        0        0     2572 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ss.js
--rw-r--r--   0        0        0     2066 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sv.js
--rw-r--r--   0        0        0     1651 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sw.js
--rw-r--r--   0        0        0     4800 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ta.js
--rw-r--r--   0        0        0     3392 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/te.js
--rw-r--r--   0        0        0     2155 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tet.js
--rw-r--r--   0        0        0     3604 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tg.js
--rw-r--r--   0        0        0     2736 2024-05-12 06:52:38.041464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/th.js
--rw-r--r--   0        0        0     2488 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tk.js
--rw-r--r--   0        0        0     1735 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tl-ph.js
--rw-r--r--   0        0        0     3755 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tlh.js
--rw-r--r--   0        0        0     2927 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tr.js
--rw-r--r--   0        0        0     3109 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzl.js
--rw-r--r--   0        0        0     1691 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzm-latn.js
--rw-r--r--   0        0        0     2322 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzm.js
--rw-r--r--   0        0        0     3880 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ug-cn.js
--rw-r--r--   0        0        0     5955 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uk.js
--rw-r--r--   0        0        0     2200 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ur.js
--rw-r--r--   0        0        0     1639 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uz-latn.js
--rw-r--r--   0        0        0     1885 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uz.js
--rw-r--r--   0        0        0     2430 2024-05-12 06:52:38.042464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/vi.js
--rw-r--r--   0        0        0     2348 2024-05-12 06:52:38.043465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/x-pseudo.js
--rw-r--r--   0        0        0     1887 2024-05-12 06:52:38.043465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/yo.js
--rw-r--r--   0        0        0     3711 2024-05-12 06:52:38.043465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-cn.js
--rw-r--r--   0        0        0     3116 2024-05-12 06:52:38.043465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-hk.js
--rw-r--r--   0        0        0     3066 2024-05-12 06:52:38.043465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-mo.js
--rw-r--r--   0        0        0     3013 2024-05-12 06:52:38.043465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-tw.js
--rw-r--r--   0        0        0   369019 2024-05-12 06:52:38.045464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/moment-with-locales.min.js
--rw-r--r--   0        0        0    58024 2024-05-12 06:52:38.045464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/moment.min.js
--rw-r--r--   0        0        0    20122 2024-05-12 06:52:38.046465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/popper.js/2.11.8/umd/popper.min.js
--rw-r--r--   0        0        0    39680 2024-05-12 06:52:38.046465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/3.4.1/js/bootstrap.min.js
--rw-r--r--   0        0        0   162017 2024-05-12 06:52:38.047464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/css/bootstrap.min.css
--rw-r--r--   0        0        0   653535 2024-05-12 06:52:38.050464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/css/bootstrap.min.css.map
--rw-r--r--   0        0        0    62440 2024-05-12 06:52:38.051464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/js/bootstrap.min.js
--rw-r--r--   0        0        0   187646 2024-05-12 06:52:38.052464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/js/bootstrap.min.js.map
--rw-r--r--   0        0        0    21137 2024-05-12 06:52:38.053465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/css/bootstrap-editable.css
--rw-r--r--   0        0        0      244 2024-05-12 06:52:38.053465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/img/clear.png
--rw-r--r--   0        0        0     1849 2024-05-12 06:52:38.053465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/img/loading.gif
--rw-r--r--   0        0        0    75909 2024-05-12 06:52:38.053465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/js/bootstrap-editable.min.js
--rw-r--r--   0        0        0      709 2024-05-12 06:52:38.053465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/bootstrap-locals.less
--rw-r--r--   0        0        0     1078 2024-05-12 06:52:38.054464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/darkly/LICENSE
--rw-r--r--   0        0        0     5407 2024-05-12 06:52:38.054464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/darkly/bootswatch.less
--rw-r--r--   0        0        0      520 2024-05-12 06:52:38.054464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/darkly/darkly.less
--rw-r--r--   0        0        0   122733 2024-05-12 06:52:38.054464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/darkly/darkly.min.css
--rw-r--r--   0        0        0      979 2024-05-12 06:52:38.054464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly-shared.less
--rw-r--r--   0        0        0     1078 2024-05-12 06:52:38.055464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly/LICENSE
--rw-r--r--   0        0        0     5104 2024-05-12 06:52:38.055464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly/bootswatch.less
--rw-r--r--   0        0        0      881 2024-05-12 06:52:38.055464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly/flatly.less
--rw-r--r--   0        0        0   123149 2024-05-12 06:52:38.055464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly/flatly.min.css
--rw-r--r--   0        0        0     4229 2024-05-12 06:52:38.055464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/fonts-lato.css
--rw-r--r--   0        0        0    20127 2024-05-12 06:52:38.055464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0   108738 2024-05-12 06:52:38.056465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    45404 2024-05-12 06:52:38.056465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23424 2024-05-12 06:52:38.056465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0    18028 2024-05-12 06:52:38.056465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.woff2
--rw-r--r--   0        0        0     4406 2024-05-12 06:52:38.057464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/OFL.txt
--rw-r--r--   0        0        0    29264 2024-05-12 06:52:38.057464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100.woff
--rw-r--r--   0        0        0    23300 2024-05-12 06:52:38.057464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100.woff2
--rw-r--r--   0        0        0    23416 2024-05-12 06:52:38.057464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100italic.woff
--rw-r--r--   0        0        0    18228 2024-05-12 06:52:38.057464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100italic.woff2
--rw-r--r--   0        0        0    32196 2024-05-12 06:52:38.057464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300.woff
--rw-r--r--   0        0        0    24836 2024-05-12 06:52:38.058464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300.woff2
--rw-r--r--   0        0        0    24056 2024-05-12 06:52:38.058464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300italic.woff
--rw-r--r--   0        0        0    18868 2024-05-12 06:52:38.058464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300italic.woff2
--rw-r--r--   0        0        0    30356 2024-05-12 06:52:38.058464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700.woff
--rw-r--r--   0        0        0    24712 2024-05-12 06:52:38.058464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700.woff2
--rw-r--r--   0        0        0    32564 2024-05-12 06:52:38.059465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700italic.woff
--rw-r--r--   0        0        0    26344 2024-05-12 06:52:38.059465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700italic.woff2
--rw-r--r--   0        0        0    29700 2024-05-12 06:52:38.059465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900.woff
--rw-r--r--   0        0        0    24344 2024-05-12 06:52:38.059465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900.woff2
--rw-r--r--   0        0        0    31260 2024-05-12 06:52:38.059465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900italic.woff
--rw-r--r--   0        0        0    25636 2024-05-12 06:52:38.059465 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900italic.woff2
--rw-r--r--   0        0        0    32220 2024-05-12 06:52:38.060464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-italic.woff
--rw-r--r--   0        0        0    26312 2024-05-12 06:52:38.060464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-italic.woff2
--rw-r--r--   0        0        0    30924 2024-05-12 06:52:38.060464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-regular.woff
--rw-r--r--   0        0        0    25320 2024-05-12 06:52:38.060464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-regular.woff2
--rw-r--r--   0        0        0    23040 2024-05-12 06:52:38.060464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-700.woff2
--rw-r--r--   0        0        0    24780 2024-05-12 06:52:38.060464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-700.woff2
--rw-r--r--   0        0        0    26328 2024-05-12 06:52:38.061464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-italic.woff2
--rw-r--r--   0        0        0    25284 2024-05-12 06:52:38.061464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-regular.woff2
--rw-r--r--   0        0        0    24408 2024-05-12 06:52:38.061464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-italic.woff2
--rw-r--r--   0        0        0    23580 2024-05-12 06:52:38.061464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-regular.woff2
--rw-r--r--   0        0        0    22160 2024-05-12 06:52:38.061464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-300.woff2
--rw-r--r--   0        0        0    22632 2024-05-12 06:52:38.061464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-500.woff2
--rw-r--r--   0        0        0    22404 2024-05-12 06:52:38.062464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-700.woff2
--rw-r--r--   0        0        0    22360 2024-05-12 06:52:38.062464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-900.woff2
--rw-r--r--   0        0        0    32976 2024-05-12 06:52:38.062464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-300.woff2
--rw-r--r--   0        0        0    33680 2024-05-12 06:52:38.062464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-500.woff2
--rw-r--r--   0        0        0    33412 2024-05-12 06:52:38.062464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-700.woff2
--rw-r--r--   0        0        0    33328 2024-05-12 06:52:38.062464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-900.woff2
--rw-r--r--   0        0        0    20556 2024-05-12 06:52:38.062464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-300.woff2
--rw-r--r--   0        0        0    20484 2024-05-12 06:52:38.062464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-500.woff2
--rw-r--r--   0        0        0    20444 2024-05-12 06:52:38.062464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-700.woff2
--rw-r--r--   0        0        0    20344 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-900.woff2
--rw-r--r--   0        0        0    20660 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-300.woff2
--rw-r--r--   0        0        0    20588 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-500.woff2
--rw-r--r--   0        0        0    20424 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-700.woff2
--rw-r--r--   0        0        0    20416 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-900.woff2
--rw-r--r--   0        0        0    15740 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-300.woff2
--rw-r--r--   0        0        0    15920 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-500.woff2
--rw-r--r--   0        0        0    15860 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-700.woff2
--rw-r--r--   0        0        0    15752 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-900.woff2
--rw-r--r--   0        0        0    22448 2024-05-12 06:52:38.063464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-300.woff2
--rw-r--r--   0        0        0    22648 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-500.woff2
--rw-r--r--   0        0        0    22580 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-700.woff2
--rw-r--r--   0        0        0    22400 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-900.woff2
--rw-r--r--   0        0        0    18472 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-300.woff2
--rw-r--r--   0        0        0    18636 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-500.woff2
--rw-r--r--   0        0        0    18616 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-700.woff2
--rw-r--r--   0        0        0    18412 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-900.woff2
--rw-r--r--   0        0        0      782 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/templates/bundles/bootstrap-css.html
--rw-r--r--   0        0        0      621 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/templates/bundles/bootstrap-js.html
--rw-r--r--   0        0        0      382 2024-05-12 06:52:38.064464 aa_gdpr-0.4.2/aagdpr/templates/bundles/clipboard-js.html
--rw-r--r--   0        0        0      329 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/datatables-css-bs5.html
--rw-r--r--   0        0        0      328 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/datatables-css.html
--rw-r--r--   0        0        0      686 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/datatables-js-bs5.html
--rw-r--r--   0        0        0      685 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/datatables-js.html
--rw-r--r--   0        0        0      310 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/fontawesome.html
--rw-r--r--   0        0        0      354 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/jquery-datetimepicker-css.html
--rw-r--r--   0        0        0      349 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/jquery-datetimepicker-js.html
--rw-r--r--   0        0        0      336 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/jquery-js.html
--rw-r--r--   0        0        0      352 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/jquery-ui-js.html
--rw-r--r--   0        0        0      328 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/jquery-visibility-js.html
--rw-r--r--   0        0        0      500 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/moment-js.html
--rw-r--r--   0        0        0      310 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/x-editable-js.html
--rw-r--r--   0        0        0      317 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/bundles/x-editable.css.html
--rw-r--r--   0        0        0     6661 2024-05-12 06:52:38.065464 aa_gdpr-0.4.2/aagdpr/templates/esi/select_token.html
--rw-r--r--   0        0        0        0 2024-05-12 06:52:38.108464 aa_gdpr-0.4.2/aagdpr/theme/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 06:52:38.108464 aa_gdpr-0.4.2/aagdpr/theme/bootstrap/__init__.py
--rw-r--r--   0        0        0      235 2024-05-12 06:52:38.066465 aa_gdpr-0.4.2/aagdpr/theme/bootstrap/apps.py
--rw-r--r--   0        0        0     2006 2024-05-12 06:52:38.066465 aa_gdpr-0.4.2/aagdpr/theme/bootstrap/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 06:52:38.109465 aa_gdpr-0.4.2/aagdpr/theme/darkly/__init__.py
--rw-r--r--   0        0        0      234 2024-05-12 06:52:38.066465 aa_gdpr-0.4.2/aagdpr/theme/darkly/apps.py
--rw-r--r--   0        0        0     1664 2024-05-12 06:52:38.066465 aa_gdpr-0.4.2/aagdpr/theme/darkly/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 06:52:38.109465 aa_gdpr-0.4.2/aagdpr/theme/flatly/__init__.py
--rw-r--r--   0        0        0      234 2024-05-12 06:52:38.066465 aa_gdpr-0.4.2/aagdpr/theme/flatly/apps.py
--rw-r--r--   0        0        0     1659 2024-05-12 06:52:38.066465 aa_gdpr-0.4.2/aagdpr/theme/flatly/auth_hooks.py
--rw-r--r--   0        0        0        0 2024-05-12 06:52:38.109465 aa_gdpr-0.4.2/aagdpr/theme/materia/__init__.py
--rw-r--r--   0        0        0      238 2024-05-12 06:52:38.066465 aa_gdpr-0.4.2/aagdpr/theme/materia/apps.py
--rw-r--r--   0        0        0     1675 2024-05-12 06:52:38.066465 aa_gdpr-0.4.2/aagdpr/theme/materia/auth_hooks.py
--rw-r--r--   0        0        0     2042 2024-05-12 06:52:38.066465 aa_gdpr-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     4536 1970-01-01 00:00:00.000000 aa_gdpr-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-16 16:26:25.734388 aa_gdpr-0.4.3/LICENSE
+-rw-r--r--   0        0        0     3068 2024-05-16 16:26:25.734388 aa_gdpr-0.4.3/README.md
+-rw-r--r--   0        0        0       97 2024-05-16 16:26:25.734388 aa_gdpr-0.4.3/aagdpr/__init__.py
+-rw-r--r--   0        0        0      238 2024-05-16 16:26:25.734388 aa_gdpr-0.4.3/aagdpr/app_settings.py
+-rw-r--r--   0        0        0      180 2024-05-16 16:26:25.734388 aa_gdpr-0.4.3/aagdpr/apps.py
+-rw-r--r--   0        0        0   232803 2024-05-16 16:26:25.736388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css
+-rw-r--r--   0        0        0    60635 2024-05-16 16:26:25.736388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootstrap/5.3.3/js/bootstrap.min.js
+-rw-r--r--   0        0        0     1297 2024-05-16 16:26:25.736388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/_bootswatch.scss
+-rw-r--r--   0        0        0     5804 2024-05-16 16:26:25.736388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/_variables.scss
+-rw-r--r--   0        0        0   281028 2024-05-16 16:26:25.737388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.css
+-rw-r--r--   0        0        0   230846 2024-05-16 16:26:25.738388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.min.css
+-rw-r--r--   0        0        0    87361 2024-05-16 16:26:25.739388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280238 2024-05-16 16:26:25.740388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.rtl.css
+-rw-r--r--   0        0        0   230950 2024-05-16 16:26:25.741388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0     2343 2024-05-16 16:26:25.741388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/fonts-lato.css
+-rw-r--r--   0        0        0      986 2024-05-16 16:26:25.741388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/fonts-lato.min.css
+-rw-r--r--   0        0        0     1153 2024-05-16 16:26:25.741388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/_bootswatch.scss
+-rw-r--r--   0        0        0     3731 2024-05-16 16:26:25.742388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/_variables.scss
+-rw-r--r--   0        0        0   281687 2024-05-16 16:26:25.742388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.css
+-rw-r--r--   0        0        0   231635 2024-05-16 16:26:25.742388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.min.css
+-rw-r--r--   0        0        0   280897 2024-05-16 16:26:25.743388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.rtl.css
+-rw-r--r--   0        0        0   231739 2024-05-16 16:26:25.743388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0     2343 2024-05-16 16:26:25.743388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/fonts-lato.css
+-rw-r--r--   0        0        0      986 2024-05-16 16:26:25.743388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/fonts-lato.min.css
+-rw-r--r--   0        0        0    11938 2024-05-16 16:26:25.744388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/_bootswatch.scss
+-rw-r--r--   0        0        0     3053 2024-05-16 16:26:25.744388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/_variables.scss
+-rw-r--r--   0        0        0   308306 2024-05-16 16:26:25.744388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.css
+-rw-r--r--   0        0        0   254640 2024-05-16 16:26:25.745388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.min.css
+-rw-r--r--   0        0        0   307572 2024-05-16 16:26:25.745388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.rtl.css
+-rw-r--r--   0        0        0   254797 2024-05-16 16:26:25.746388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0    11103 2024-05-16 16:26:25.746388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/fonts-roboto.css
+-rw-r--r--   0        0        0     4740 2024-05-16 16:26:25.746388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/fonts-roboto.min.css
+-rw-r--r--   0        0        0     9160 2024-05-16 16:26:25.746388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/clipboard.js/2.0.11/clipboard.min.js
+-rw-r--r--   0        0        0    12123 2024-05-16 16:26:25.746388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/css/dataTables.bootstrap5.min.css
+-rw-r--r--   0        0        0     2358 2024-05-16 16:26:25.747388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/js/dataTables.bootstrap5.min.js
+-rw-r--r--   0        0        0    87238 2024-05-16 16:26:25.747388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/js/jquery.dataTables.min.js
+-rw-r--r--   0        0        0     6402 2024-05-16 16:26:25.747388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/css/dataTables.bootstrap.min.css
+-rw-r--r--   0        0        0     4401 2024-05-16 16:26:25.747388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/js/dataTables.bootstrap.min.js
+-rw-r--r--   0        0        0    87897 2024-05-16 16:26:25.748388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/js/jquery.dataTables.min.js
+-rw-r--r--   0        0        0    11174 2024-05-16 16:26:25.748388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/css/dataTables.bootstrap.min.css
+-rw-r--r--   0        0        0    12123 2024-05-16 16:26:25.748388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/css/dataTables.bootstrap5.min.css
+-rw-r--r--   0        0        0     2223 2024-05-16 16:26:25.748388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/dataTables.bootstrap.min.js
+-rw-r--r--   0        0        0     2358 2024-05-16 16:26:25.748388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/dataTables.bootstrap5.min.js
+-rw-r--r--   0        0        0    87238 2024-05-16 16:26:25.749388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/jquery.dataTables.min.js
+-rw-r--r--   0        0        0     1548 2024-05-16 16:26:25.749388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/LICENSE.txt
+-rw-r--r--   0        0        0    73577 2024-05-16 16:26:25.749388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/all.css
+-rw-r--r--   0        0        0    59305 2024-05-16 16:26:25.750388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/all.min.css
+-rw-r--r--   0        0        0      732 2024-05-16 16:26:25.750388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/brands.css
+-rw-r--r--   0        0        0      675 2024-05-16 16:26:25.750388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/brands.min.css
+-rw-r--r--   0        0        0    71942 2024-05-16 16:26:25.750388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/fontawesome.css
+-rw-r--r--   0        0        0    57873 2024-05-16 16:26:25.751388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/fontawesome.min.css
+-rw-r--r--   0        0        0      734 2024-05-16 16:26:25.751388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/regular.css
+-rw-r--r--   0        0        0      677 2024-05-16 16:26:25.751388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/regular.min.css
+-rw-r--r--   0        0        0      727 2024-05-16 16:26:25.751388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/solid.css
+-rw-r--r--   0        0        0      669 2024-05-16 16:26:25.751388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/solid.min.css
+-rw-r--r--   0        0        0     8077 2024-05-16 16:26:25.751388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/svg-with-js.css
+-rw-r--r--   0        0        0     6359 2024-05-16 16:26:25.751388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/svg-with-js.min.css
+-rw-r--r--   0        0        0    41312 2024-05-16 16:26:25.752388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/v4-shims.css
+-rw-r--r--   0        0        0    26702 2024-05-16 16:26:25.752388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/v4-shims.min.css
+-rw-r--r--   0        0        0   134294 2024-05-16 16:26:25.753388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   747470 2024-05-16 16:26:25.759388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   133988 2024-05-16 16:26:25.760388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    89988 2024-05-16 16:26:25.760388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    76736 2024-05-16 16:26:25.760388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    34034 2024-05-16 16:26:25.761388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   144562 2024-05-16 16:26:25.762388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    33736 2024-05-16 16:26:25.762388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    16276 2024-05-16 16:26:25.762388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    13224 2024-05-16 16:26:25.762388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   203030 2024-05-16 16:26:25.764388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   917989 2024-05-16 16:26:25.770388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   202744 2024-05-16 16:26:25.771388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   101648 2024-05-16 16:26:25.772388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    78268 2024-05-16 16:26:25.772388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     7427 2024-05-16 16:26:25.772388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/LICENSE.txt
+-rw-r--r--   0        0        0   140292 2024-05-16 16:26:25.773388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/all.css
+-rw-r--r--   0        0        0   102217 2024-05-16 16:26:25.773388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/all.min.css
+-rw-r--r--   0        0        0    24006 2024-05-16 16:26:25.773388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/brands.css
+-rw-r--r--   0        0        0    18855 2024-05-16 16:26:25.773388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/brands.min.css
+-rw-r--r--   0        0        0   113421 2024-05-16 16:26:25.774387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/fontawesome.css
+-rw-r--r--   0        0        0    80823 2024-05-16 16:26:25.774387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/fontawesome.min.css
+-rw-r--r--   0        0        0      633 2024-05-16 16:26:25.774387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/regular.css
+-rw-r--r--   0        0        0      580 2024-05-16 16:26:25.774387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/regular.min.css
+-rw-r--r--   0        0        0      625 2024-05-16 16:26:25.774387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/solid.css
+-rw-r--r--   0        0        0      572 2024-05-16 16:26:25.774387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/solid.min.css
+-rw-r--r--   0        0        0    21637 2024-05-16 16:26:25.775388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/svg-with-js.css
+-rw-r--r--   0        0        0    16956 2024-05-16 16:26:25.775388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/svg-with-js.min.css
+-rw-r--r--   0        0        0     1831 2024-05-16 16:26:25.775388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-font-face.css
+-rw-r--r--   0        0        0     1736 2024-05-16 16:26:25.775388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-font-face.min.css
+-rw-r--r--   0        0        0    41574 2024-05-16 16:26:25.775388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-shims.css
+-rw-r--r--   0        0        0    27593 2024-05-16 16:26:25.775388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-shims.min.css
+-rw-r--r--   0        0        0      871 2024-05-16 16:26:25.775388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v5-font-face.css
+-rw-r--r--   0        0        0      794 2024-05-16 16:26:25.775388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v5-font-face.min.css
+-rw-r--r--   0        0        0   189684 2024-05-16 16:26:25.776388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   109808 2024-05-16 16:26:25.777387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    63348 2024-05-16 16:26:25.777387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    24488 2024-05-16 16:26:25.777387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   394668 2024-05-16 16:26:25.779388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150020 2024-05-16 16:26:25.780387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10172 2024-05-16 16:26:25.780387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4568 2024-05-16 16:26:25.780387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0    60579 2024-05-16 16:26:25.780387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.full.min.js
+-rw-r--r--   0        0        0    16503 2024-05-16 16:26:25.781388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.min.css
+-rw-r--r--   0        0        0    51705 2024-05-16 16:26:25.781388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.min.js
+-rw-r--r--   0        0        0     7142 2024-05-16 16:26:25.781388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0        0        0     7126 2024-05-16 16:26:25.781388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0        0        0     4670 2024-05-16 16:26:25.781388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png
+-rw-r--r--   0        0        0     7163 2024-05-16 16:26:25.781388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png
+-rw-r--r--   0        0        0     4670 2024-05-16 16:26:25.782388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0        0        0     6539 2024-05-16 16:26:25.782388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0        0        0    32131 2024-05-16 16:26:25.782388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/jquery-ui.min.css
+-rw-r--r--   0        0        0   255083 2024-05-16 16:26:25.783388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/js/jquery-ui.min.js
+-rw-r--r--   0        0        0      854 2024-05-16 16:26:25.783388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-visibility/1.0.11/jquery-visibility.min.js
+-rw-r--r--   0        0        0    85578 2024-05-16 16:26:25.784387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery/2.2.4/jquery.min.js
+-rw-r--r--   0        0        0    87533 2024-05-16 16:26:25.785388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery/3.7.1/jquery.min.js
+-rw-r--r--   0        0        0    70264 2024-05-16 16:26:25.785388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery/3.7.1/jquery.slim.min.js
+-rw-r--r--   0        0        0   149321 2024-05-16 16:26:25.786388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/less.js/4.2.0/less.min.js
+-rw-r--r--   0        0        0     2149 2024-05-16 16:26:25.786388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/af.js
+-rw-r--r--   0        0        0     4449 2024-05-16 16:26:25.786388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-dz.js
+-rw-r--r--   0        0        0     1934 2024-05-16 16:26:25.786388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-kw.js
+-rw-r--r--   0        0        0     4648 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-ly.js
+-rw-r--r--   0        0        0     1989 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-ma.js
+-rw-r--r--   0        0        0     3042 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-sa.js
+-rw-r--r--   0        0        0     1936 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-tn.js
+-rw-r--r--   0        0        0     5072 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar.js
+-rw-r--r--   0        0        0     2846 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/az.js
+-rw-r--r--   0        0        0     5154 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/be.js
+-rw-r--r--   0        0        0     2955 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bg.js
+-rw-r--r--   0        0        0     1784 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bm.js
+-rw-r--r--   0        0        0     4349 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bn-bd.js
+-rw-r--r--   0        0        0     3898 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bn.js
+-rw-r--r--   0        0        0     4399 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bo.js
+-rw-r--r--   0        0        0     4544 2024-05-16 16:26:25.787387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/br.js
+-rw-r--r--   0        0        0     4475 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bs.js
+-rw-r--r--   0        0        0     3031 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ca.js
+-rw-r--r--   0        0        0     6718 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cs.js
+-rw-r--r--   0        0        0     2341 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cv.js
+-rw-r--r--   0        0        0     2834 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cy.js
+-rw-r--r--   0        0        0     1629 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/da.js
+-rw-r--r--   0        0        0     2635 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de-at.js
+-rw-r--r--   0        0        0     2563 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de-ch.js
+-rw-r--r--   0        0        0     2562 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de.js
+-rw-r--r--   0        0        0     2464 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/dv.js
+-rw-r--r--   0        0        0     3877 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/el.js
+-rw-r--r--   0        0        0     2029 2024-05-16 16:26:25.788388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-au.js
+-rw-r--r--   0        0        0     1878 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-ca.js
+-rw-r--r--   0        0        0     2035 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-gb.js
+-rw-r--r--   0        0        0     2033 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-ie.js
+-rw-r--r--   0        0        0     1871 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-il.js
+-rw-r--r--   0        0        0     2029 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-in.js
+-rw-r--r--   0        0        0     2038 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-nz.js
+-rw-r--r--   0        0        0     2047 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-sg.js
+-rw-r--r--   0        0        0     2338 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/eo.js
+-rw-r--r--   0        0        0     3441 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-do.js
+-rw-r--r--   0        0        0     3510 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-mx.js
+-rw-r--r--   0        0        0     3538 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-us.js
+-rw-r--r--   0        0        0     3498 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es.js
+-rw-r--r--   0        0        0     2631 2024-05-16 16:26:25.789388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/et.js
+-rw-r--r--   0        0        0     1964 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/eu.js
+-rw-r--r--   0        0        0     3230 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fa.js
+-rw-r--r--   0        0        0     3632 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fi.js
+-rw-r--r--   0        0        0     1776 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fil.js
+-rw-r--r--   0        0        0     1772 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fo.js
+-rw-r--r--   0        0        0     2104 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr-ca.js
+-rw-r--r--   0        0        0     2263 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr-ch.js
+-rw-r--r--   0        0        0     3471 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr.js
+-rw-r--r--   0        0        0     2275 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fy.js
+-rw-r--r--   0        0        0     2360 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ga.js
+-rw-r--r--   0        0        0     2380 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gd.js
+-rw-r--r--   0        0        0     2347 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gl.js
+-rw-r--r--   0        0        0     5506 2024-05-16 16:26:25.790387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gom-deva.js
+-rw-r--r--   0        0        0     4130 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gom-latn.js
+-rw-r--r--   0        0        0     4132 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gu.js
+-rw-r--r--   0        0        0     3211 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/he.js
+-rw-r--r--   0        0        0     6421 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hi.js
+-rw-r--r--   0        0        0     4718 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hr.js
+-rw-r--r--   0        0        0     3815 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hu.js
+-rw-r--r--   0        0        0     3236 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hy-am.js
+-rw-r--r--   0        0        0     2375 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/id.js
+-rw-r--r--   0        0        0     4458 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/is.js
+-rw-r--r--   0        0        0     1941 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/it-ch.js
+-rw-r--r--   0        0        0     3251 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/it.js
+-rw-r--r--   0        0        0     3955 2024-05-16 16:26:25.791387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ja.js
+-rw-r--r--   0        0        0     2384 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/jv.js
+-rw-r--r--   0        0        0     3504 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ka.js
+-rw-r--r--   0        0        0     2495 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/kk.js
+-rw-r--r--   0        0        0     3362 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/km.js
+-rw-r--r--   0        0        0     4252 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/kn.js
+-rw-r--r--   0        0        0     2223 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ko.js
+-rw-r--r--   0        0        0     3330 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ku.js
+-rw-r--r--   0        0        0     2521 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ky.js
+-rw-r--r--   0        0        0     4269 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lb.js
+-rw-r--r--   0        0        0     2585 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lo.js
+-rw-r--r--   0        0        0     4005 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lt.js
+-rw-r--r--   0        0        0     3449 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lv.js
+-rw-r--r--   0        0        0     3661 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/me.js
+-rw-r--r--   0        0        0     2023 2024-05-16 16:26:25.792388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mi.js
+-rw-r--r--   0        0        0     3021 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mk.js
+-rw-r--r--   0        0        0     3287 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ml.js
+-rw-r--r--   0        0        0     3414 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mn.js
+-rw-r--r--   0        0        0     6574 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mr.js
+-rw-r--r--   0        0        0     2330 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ms-my.js
+-rw-r--r--   0        0        0     2277 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ms.js
+-rw-r--r--   0        0        0     1684 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mt.js
+-rw-r--r--   0        0        0     3094 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/my.js
+-rw-r--r--   0        0        0     1899 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nb.js
+-rw-r--r--   0        0        0     4031 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ne.js
+-rw-r--r--   0        0        0     3169 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nl-be.js
+-rw-r--r--   0        0        0     3202 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nl.js
+-rw-r--r--   0        0        0     1828 2024-05-16 16:26:25.793388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nn.js
+-rw-r--r--   0        0        0     2472 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/oc-lnc.js
+-rw-r--r--   0        0        0     4198 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pa-in.js
+-rw-r--r--   0        0        0     4166 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pl.js
+-rw-r--r--   0        0        0     1854 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pt-br.js
+-rw-r--r--   0        0        0     1968 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pt.js
+-rw-r--r--   0        0        0     2319 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ro.js
+-rw-r--r--   0        0        0     8418 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ru.js
+-rw-r--r--   0        0        0     2153 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sd.js
+-rw-r--r--   0        0        0     1849 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/se.js
+-rw-r--r--   0        0        0     2681 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/si.js
+-rw-r--r--   0        0        0     5173 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sk.js
+-rw-r--r--   0        0        0     6115 2024-05-16 16:26:25.794387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sl.js
+-rw-r--r--   0        0        0     1987 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sq.js
+-rw-r--r--   0        0        0     4762 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sr-cyrl.js
+-rw-r--r--   0        0        0     4209 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sr.js
+-rw-r--r--   0        0        0     2572 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ss.js
+-rw-r--r--   0        0        0     2066 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sv.js
+-rw-r--r--   0        0        0     1651 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sw.js
+-rw-r--r--   0        0        0     4800 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ta.js
+-rw-r--r--   0        0        0     3392 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/te.js
+-rw-r--r--   0        0        0     2155 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tet.js
+-rw-r--r--   0        0        0     3604 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tg.js
+-rw-r--r--   0        0        0     2736 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/th.js
+-rw-r--r--   0        0        0     2488 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tk.js
+-rw-r--r--   0        0        0     1735 2024-05-16 16:26:25.795388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tl-ph.js
+-rw-r--r--   0        0        0     3755 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tlh.js
+-rw-r--r--   0        0        0     2927 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tr.js
+-rw-r--r--   0        0        0     3109 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzl.js
+-rw-r--r--   0        0        0     1691 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzm-latn.js
+-rw-r--r--   0        0        0     2322 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzm.js
+-rw-r--r--   0        0        0     3880 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ug-cn.js
+-rw-r--r--   0        0        0     5955 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uk.js
+-rw-r--r--   0        0        0     2200 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ur.js
+-rw-r--r--   0        0        0     1639 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uz-latn.js
+-rw-r--r--   0        0        0     1885 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uz.js
+-rw-r--r--   0        0        0     2430 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/vi.js
+-rw-r--r--   0        0        0     2348 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/x-pseudo.js
+-rw-r--r--   0        0        0     1887 2024-05-16 16:26:25.796388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/yo.js
+-rw-r--r--   0        0        0     3711 2024-05-16 16:26:25.797387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-cn.js
+-rw-r--r--   0        0        0     3116 2024-05-16 16:26:25.797387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-hk.js
+-rw-r--r--   0        0        0     3066 2024-05-16 16:26:25.797387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-mo.js
+-rw-r--r--   0        0        0     3013 2024-05-16 16:26:25.797387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-tw.js
+-rw-r--r--   0        0        0   369019 2024-05-16 16:26:25.799388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/moment-with-locales.min.js
+-rw-r--r--   0        0        0    58024 2024-05-16 16:26:25.799388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/moment.min.js
+-rw-r--r--   0        0        0    20122 2024-05-16 16:26:25.799388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/popper.js/2.11.8/umd/popper.min.js
+-rw-r--r--   0        0        0    39680 2024-05-16 16:26:25.800387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/3.4.1/js/bootstrap.min.js
+-rw-r--r--   0        0        0   162017 2024-05-16 16:26:25.800387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/css/bootstrap.min.css
+-rw-r--r--   0        0        0   653535 2024-05-16 16:26:25.804387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0    62440 2024-05-16 16:26:25.804387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/js/bootstrap.min.js
+-rw-r--r--   0        0        0   187646 2024-05-16 16:26:25.806388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0    21137 2024-05-16 16:26:25.806388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/css/bootstrap-editable.css
+-rw-r--r--   0        0        0      244 2024-05-16 16:26:25.806388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/img/clear.png
+-rw-r--r--   0        0        0     1849 2024-05-16 16:26:25.806388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/img/loading.gif
+-rw-r--r--   0        0        0    75909 2024-05-16 16:26:25.807387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/js/bootstrap-editable.min.js
+-rw-r--r--   0        0        0      709 2024-05-16 16:26:25.807387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/bootstrap-locals.less
+-rw-r--r--   0        0        0     1078 2024-05-16 16:26:25.807387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/darkly/LICENSE
+-rw-r--r--   0        0        0     5407 2024-05-16 16:26:25.807387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/darkly/bootswatch.less
+-rw-r--r--   0        0        0      520 2024-05-16 16:26:25.807387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/darkly/darkly.less
+-rw-r--r--   0        0        0   122733 2024-05-16 16:26:25.808387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/darkly/darkly.min.css
+-rw-r--r--   0        0        0      979 2024-05-16 16:26:25.808387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly-shared.less
+-rw-r--r--   0        0        0     1078 2024-05-16 16:26:25.808387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly/LICENSE
+-rw-r--r--   0        0        0     5104 2024-05-16 16:26:25.808387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly/bootswatch.less
+-rw-r--r--   0        0        0      881 2024-05-16 16:26:25.808387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly/flatly.less
+-rw-r--r--   0        0        0   123149 2024-05-16 16:26:25.808387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly/flatly.min.css
+-rw-r--r--   0        0        0     4229 2024-05-16 16:26:25.808387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/fonts-lato.css
+-rw-r--r--   0        0        0    20127 2024-05-16 16:26:25.809388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0   108738 2024-05-16 16:26:25.809388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    45404 2024-05-16 16:26:25.809388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23424 2024-05-16 16:26:25.810387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    18028 2024-05-16 16:26:25.810387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.woff2
+-rw-r--r--   0        0        0     4406 2024-05-16 16:26:25.810387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/OFL.txt
+-rw-r--r--   0        0        0    29264 2024-05-16 16:26:25.810387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100.woff
+-rw-r--r--   0        0        0    23300 2024-05-16 16:26:25.810387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100.woff2
+-rw-r--r--   0        0        0    23416 2024-05-16 16:26:25.810387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100italic.woff
+-rw-r--r--   0        0        0    18228 2024-05-16 16:26:25.811387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100italic.woff2
+-rw-r--r--   0        0        0    32196 2024-05-16 16:26:25.811387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300.woff
+-rw-r--r--   0        0        0    24836 2024-05-16 16:26:25.811387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300.woff2
+-rw-r--r--   0        0        0    24056 2024-05-16 16:26:25.811387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300italic.woff
+-rw-r--r--   0        0        0    18868 2024-05-16 16:26:25.811387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300italic.woff2
+-rw-r--r--   0        0        0    30356 2024-05-16 16:26:25.811387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700.woff
+-rw-r--r--   0        0        0    24712 2024-05-16 16:26:25.812388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700.woff2
+-rw-r--r--   0        0        0    32564 2024-05-16 16:26:25.812388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700italic.woff
+-rw-r--r--   0        0        0    26344 2024-05-16 16:26:25.812388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700italic.woff2
+-rw-r--r--   0        0        0    29700 2024-05-16 16:26:25.812388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900.woff
+-rw-r--r--   0        0        0    24344 2024-05-16 16:26:25.812388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900.woff2
+-rw-r--r--   0        0        0    31260 2024-05-16 16:26:25.812388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900italic.woff
+-rw-r--r--   0        0        0    25636 2024-05-16 16:26:25.813387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900italic.woff2
+-rw-r--r--   0        0        0    32220 2024-05-16 16:26:25.813387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-italic.woff
+-rw-r--r--   0        0        0    26312 2024-05-16 16:26:25.813387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-italic.woff2
+-rw-r--r--   0        0        0    30924 2024-05-16 16:26:25.813387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-regular.woff
+-rw-r--r--   0        0        0    25320 2024-05-16 16:26:25.813387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-regular.woff2
+-rw-r--r--   0        0        0    23040 2024-05-16 16:26:25.814387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-700.woff2
+-rw-r--r--   0        0        0    24780 2024-05-16 16:26:25.814387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-700.woff2
+-rw-r--r--   0        0        0    26328 2024-05-16 16:26:25.814387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-italic.woff2
+-rw-r--r--   0        0        0    25284 2024-05-16 16:26:25.814387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-regular.woff2
+-rw-r--r--   0        0        0    24408 2024-05-16 16:26:25.814387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-italic.woff2
+-rw-r--r--   0        0        0    23580 2024-05-16 16:26:25.814387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-regular.woff2
+-rw-r--r--   0        0        0    22160 2024-05-16 16:26:25.814387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-300.woff2
+-rw-r--r--   0        0        0    22632 2024-05-16 16:26:25.815388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-500.woff2
+-rw-r--r--   0        0        0    22404 2024-05-16 16:26:25.815388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-700.woff2
+-rw-r--r--   0        0        0    22360 2024-05-16 16:26:25.815388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-900.woff2
+-rw-r--r--   0        0        0    32976 2024-05-16 16:26:25.815388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-300.woff2
+-rw-r--r--   0        0        0    33680 2024-05-16 16:26:25.815388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-500.woff2
+-rw-r--r--   0        0        0    33412 2024-05-16 16:26:25.815388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-700.woff2
+-rw-r--r--   0        0        0    33328 2024-05-16 16:26:25.815388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-900.woff2
+-rw-r--r--   0        0        0    20556 2024-05-16 16:26:25.815388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-300.woff2
+-rw-r--r--   0        0        0    20484 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-500.woff2
+-rw-r--r--   0        0        0    20444 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-700.woff2
+-rw-r--r--   0        0        0    20344 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-900.woff2
+-rw-r--r--   0        0        0    20660 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-300.woff2
+-rw-r--r--   0        0        0    20588 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-500.woff2
+-rw-r--r--   0        0        0    20424 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-700.woff2
+-rw-r--r--   0        0        0    20416 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-900.woff2
+-rw-r--r--   0        0        0    15740 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-300.woff2
+-rw-r--r--   0        0        0    15920 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-500.woff2
+-rw-r--r--   0        0        0    15860 2024-05-16 16:26:25.816388 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-700.woff2
+-rw-r--r--   0        0        0    15752 2024-05-16 16:26:25.817387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-900.woff2
+-rw-r--r--   0        0        0    22448 2024-05-16 16:26:25.817387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-300.woff2
+-rw-r--r--   0        0        0    22648 2024-05-16 16:26:25.817387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-500.woff2
+-rw-r--r--   0        0        0    22580 2024-05-16 16:26:25.817387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-700.woff2
+-rw-r--r--   0        0        0    22400 2024-05-16 16:26:25.817387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-900.woff2
+-rw-r--r--   0        0        0    18472 2024-05-16 16:26:25.817387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-300.woff2
+-rw-r--r--   0        0        0    18636 2024-05-16 16:26:25.817387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-500.woff2
+-rw-r--r--   0        0        0    18616 2024-05-16 16:26:25.817387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-700.woff2
+-rw-r--r--   0        0        0    18412 2024-05-16 16:26:25.817387 aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-900.woff2
+-rw-r--r--   0        0        0      782 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/bootstrap-css.html
+-rw-r--r--   0        0        0      621 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/bootstrap-js.html
+-rw-r--r--   0        0        0      382 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/clipboard-js.html
+-rw-r--r--   0        0        0      329 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/datatables-css-bs5.html
+-rw-r--r--   0        0        0      328 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/datatables-css.html
+-rw-r--r--   0        0        0      686 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/datatables-js-bs5.html
+-rw-r--r--   0        0        0      685 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/datatables-js.html
+-rw-r--r--   0        0        0      310 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/fontawesome.html
+-rw-r--r--   0        0        0      354 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/jquery-datetimepicker-css.html
+-rw-r--r--   0        0        0      349 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/jquery-datetimepicker-js.html
+-rw-r--r--   0        0        0      336 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/jquery-js.html
+-rw-r--r--   0        0        0      352 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/jquery-ui-js.html
+-rw-r--r--   0        0        0      328 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/jquery-visibility-js.html
+-rw-r--r--   0        0        0      499 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/moment-js.html
+-rw-r--r--   0        0        0      310 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/x-editable-js.html
+-rw-r--r--   0        0        0      317 2024-05-16 16:26:25.818387 aa_gdpr-0.4.3/aagdpr/templates/bundles/x-editable.css.html
+-rw-r--r--   0        0        0     6661 2024-05-16 16:26:25.819388 aa_gdpr-0.4.3/aagdpr/templates/esi/select_token.html
+-rw-r--r--   0        0        0        0 2024-05-16 16:26:25.861387 aa_gdpr-0.4.3/aagdpr/theme/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 16:26:25.861387 aa_gdpr-0.4.3/aagdpr/theme/bootstrap/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-16 16:26:25.819388 aa_gdpr-0.4.3/aagdpr/theme/bootstrap/apps.py
+-rw-r--r--   0        0        0     2006 2024-05-16 16:26:25.819388 aa_gdpr-0.4.3/aagdpr/theme/bootstrap/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-16 16:26:25.861387 aa_gdpr-0.4.3/aagdpr/theme/darkly/__init__.py
+-rw-r--r--   0        0        0      234 2024-05-16 16:26:25.819388 aa_gdpr-0.4.3/aagdpr/theme/darkly/apps.py
+-rw-r--r--   0        0        0     1664 2024-05-16 16:26:25.819388 aa_gdpr-0.4.3/aagdpr/theme/darkly/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-16 16:26:25.861387 aa_gdpr-0.4.3/aagdpr/theme/flatly/__init__.py
+-rw-r--r--   0        0        0      234 2024-05-16 16:26:25.819388 aa_gdpr-0.4.3/aagdpr/theme/flatly/apps.py
+-rw-r--r--   0        0        0     1659 2024-05-16 16:26:25.819388 aa_gdpr-0.4.3/aagdpr/theme/flatly/auth_hooks.py
+-rw-r--r--   0        0        0        0 2024-05-16 16:26:25.861387 aa_gdpr-0.4.3/aagdpr/theme/materia/__init__.py
+-rw-r--r--   0        0        0      238 2024-05-16 16:26:25.819388 aa_gdpr-0.4.3/aagdpr/theme/materia/apps.py
+-rw-r--r--   0        0        0     1675 2024-05-16 16:26:25.819388 aa_gdpr-0.4.3/aagdpr/theme/materia/auth_hooks.py
+-rw-r--r--   0        0        0     2042 2024-05-16 16:26:25.820387 aa_gdpr-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     4536 1970-01-01 00:00:00.000000 aa_gdpr-0.4.3/PKG-INFO
```

### Comparing `aa_gdpr-0.4.2/LICENSE` & `aa_gdpr-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/README.md` & `aa_gdpr-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootstrap/5.3.3/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootstrap/5.3.3/js/bootstrap.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootstrap/5.3.3/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/_bootswatch.scss` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/_variables.scss` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/_variables.scss`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.min.css.map` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.rtl.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.rtl.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/fonts-lato.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/fonts-lato.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/fonts-lato.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/darkly/fonts-lato.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/_bootswatch.scss` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/_variables.scss` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/_variables.scss`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.rtl.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.rtl.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/fonts-lato.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/fonts-lato.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/fonts-lato.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/flatly/fonts-lato.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/_bootswatch.scss` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/_bootswatch.scss`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/_variables.scss` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/_variables.scss`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.rtl.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.rtl.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/fonts-roboto.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/fonts-roboto.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/fonts-roboto.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/bootswatch/5.3.3/materia/fonts-roboto.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/clipboard.js/2.0.11/clipboard.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/clipboard.js/2.0.11/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/css/dataTables.bootstrap5.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/css/dataTables.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/js/dataTables.bootstrap5.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/js/dataTables.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/js/jquery.dataTables.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net-bs5/1.13.7/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/css/dataTables.bootstrap.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/js/dataTables.bootstrap.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/js/jquery.dataTables.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.11.3/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/css/dataTables.bootstrap.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/css/dataTables.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/css/dataTables.bootstrap5.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/css/dataTables.bootstrap5.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/dataTables.bootstrap.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/dataTables.bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/dataTables.bootstrap5.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/dataTables.bootstrap5.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/jquery.dataTables.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/datatables.net/1.13.7/js/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/LICENSE.txt` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/all.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/all.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/all.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/all.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/brands.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/brands.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/brands.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/fontawesome.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/fontawesome.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/regular.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/regular.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/regular.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/solid.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/solid.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/solid.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/svg-with-js.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/svg-with-js.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/v4-shims.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/v4-shims.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.eot` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.svg` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.ttf` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.eot` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.svg` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.ttf` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.eot` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.svg` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.ttf` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/5.15.4/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/LICENSE.txt` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/all.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/all.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/all.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/all.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/brands.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/brands.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/brands.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/fontawesome.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/fontawesome.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/regular.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/regular.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/regular.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/solid.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/solid.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/solid.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/svg-with-js.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/svg-with-js.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-font-face.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-font-face.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-font-face.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-shims.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-shims.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v5-font-face.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v5-font-face.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v5-font-face.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/css/v5-font-face.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-brands-400.ttf` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-brands-400.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-regular-400.ttf` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-regular-400.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-solid-900.ttf` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-solid-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-v4compatibility.ttf` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-v4compatibility.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/font-awesome/6.4.2/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.full.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.full.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-datetimepicker/2.5.20/jquery.datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/jquery-ui.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/css/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/js/jquery-ui.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-ui/1.13.2/js/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery-visibility/1.0.11/jquery-visibility.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery-visibility/1.0.11/jquery-visibility.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery/2.2.4/jquery.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery/2.2.4/jquery.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery/3.7.1/jquery.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery/3.7.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/jquery/3.7.1/jquery.slim.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/jquery/3.7.1/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/less.js/4.2.0/less.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/less.js/4.2.0/less.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/af.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/af.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-dz.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-dz.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-kw.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-kw.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-ly.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-ly.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-ma.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-ma.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-sa.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-sa.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-tn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar-tn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ar.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/az.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/az.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/be.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/be.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bg.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bg.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bm.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bm.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bn-bd.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bn-bd.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bo.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bo.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/br.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/br.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bs.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/bs.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ca.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ca.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cs.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cs.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cv.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cv.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cy.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/cy.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/da.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/da.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de-at.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de-at.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de-ch.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de-ch.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/de.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/dv.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/dv.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/el.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/el.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-au.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-au.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-ca.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-ca.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-gb.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-gb.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-ie.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-ie.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-il.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-il.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-in.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-in.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-nz.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-nz.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-sg.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/en-sg.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/eo.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/eo.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-do.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-do.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-mx.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-mx.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-us.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es-us.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/es.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/et.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/et.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/eu.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/eu.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fa.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fa.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fi.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fi.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fil.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fil.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fo.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fo.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr-ca.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr-ca.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr-ch.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr-ch.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fr.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fy.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/fy.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ga.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ga.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gd.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gd.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gl.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gl.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gom-deva.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gom-deva.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gom-latn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gom-latn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gu.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/gu.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/he.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/he.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hi.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hi.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hr.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hr.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hu.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hu.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hy-am.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/hy-am.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/id.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/id.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/is.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/is.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/it-ch.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/it-ch.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/it.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/it.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ja.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ja.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/jv.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/jv.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ka.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ka.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/kk.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/kk.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/km.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/km.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/kn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/kn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ko.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ko.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ku.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ku.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ky.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ky.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lb.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lb.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lo.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lo.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lt.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lt.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lv.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/lv.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/me.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/me.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mi.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mi.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mk.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mk.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ml.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ml.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mr.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mr.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ms-my.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ms-my.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ms.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ms.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mt.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/mt.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/my.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/my.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nb.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nb.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ne.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ne.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nl-be.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nl-be.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nl.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nl.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/nn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/oc-lnc.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/oc-lnc.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pa-in.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pa-in.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pl.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pl.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pt-br.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pt-br.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pt.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/pt.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ro.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ro.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ru.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ru.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sd.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sd.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/se.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/se.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/si.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/si.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sk.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sk.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sl.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sl.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sq.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sq.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sr-cyrl.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sr-cyrl.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sr.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sr.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ss.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ss.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sv.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sv.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sw.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/sw.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ta.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ta.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/te.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/te.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tet.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tet.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tg.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tg.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/th.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/th.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tk.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tk.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tl-ph.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tl-ph.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tlh.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tlh.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tr.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tr.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzl.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzl.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzm-latn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzm-latn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzm.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/tzm.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ug-cn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ug-cn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uk.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uk.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ur.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/ur.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uz-latn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uz-latn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uz.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/uz.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/vi.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/vi.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/x-pseudo.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/x-pseudo.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/yo.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/yo.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-cn.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-cn.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-hk.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-hk.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-mo.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-mo.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-tw.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/locale/zh-tw.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/moment-with-locales.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/moment.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/moment.js/2.29.4/moment.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/popper.js/2.11.8/umd/popper.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/popper.js/2.11.8/umd/popper.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/3.4.1/js/bootstrap.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/3.4.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/css/bootstrap.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/css/bootstrap.min.css.map` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/js/bootstrap.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/js/bootstrap.min.js.map` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/twitter-bootstrap/4.6.1/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/css/bootstrap-editable.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/css/bootstrap-editable.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/img/loading.gif` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/img/loading.gif`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/js/bootstrap-editable.min.js` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/ajax/libs/x-editable/1.5.1/js/bootstrap-editable.min.js`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/bootstrap-locals.less` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/bootstrap-locals.less`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/darkly/LICENSE` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/darkly/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/darkly/bootswatch.less` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/darkly/bootswatch.less`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/darkly/darkly.less` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/darkly/darkly.less`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/darkly/darkly.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/darkly/darkly.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly-shared.less` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly-shared.less`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly/LICENSE` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly/bootswatch.less` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly/bootswatch.less`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly/flatly.less` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly/flatly.less`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/flatly/flatly.min.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/flatly/flatly.min.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/css/themes/fonts-lato.css` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/css/themes/fonts-lato.css`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.eot` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.svg` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.ttf` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/glyphicons-halflings/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/OFL.txt` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/OFL.txt`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100italic.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100italic.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100italic.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-100italic.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300italic.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300italic.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300italic.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-300italic.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700italic.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700italic.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700italic.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-700italic.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900italic.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900italic.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900italic.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-900italic.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-italic.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-italic.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-italic.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-regular.woff` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-regular.woff`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-regular.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v16/lato-v16-latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-italic.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-italic.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-regular.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-ext-regular.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-italic.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-regular.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/lato/v24/lato-v24-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-300.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-300.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-500.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-500.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-300.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-500.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-cyrillic-ext-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-300.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-300.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-500.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-500.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-300.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-500.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-greek-ext-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-300.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-500.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-500.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-300.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-300.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-500.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-500.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-latin-ext-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-300.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-300.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-500.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-500.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-700.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-700.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-900.woff2` & `aa_gdpr-0.4.3/aagdpr/static/aagdpr/fonts/roboto/v30/roboto-v30-vietnamese-900.woff2`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/templates/bundles/bootstrap-css.html` & `aa_gdpr-0.4.3/aagdpr/templates/bundles/bootstrap-css.html`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/templates/bundles/bootstrap-js.html` & `aa_gdpr-0.4.3/aagdpr/templates/bundles/bootstrap-js.html`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/templates/bundles/datatables-js-bs5.html` & `aa_gdpr-0.4.3/aagdpr/templates/bundles/datatables-js-bs5.html`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/templates/bundles/datatables-js.html` & `aa_gdpr-0.4.3/aagdpr/templates/bundles/datatables-js.html`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/templates/esi/select_token.html` & `aa_gdpr-0.4.3/aagdpr/templates/esi/select_token.html`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/theme/bootstrap/auth_hooks.py` & `aa_gdpr-0.4.3/aagdpr/theme/bootstrap/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/theme/darkly/auth_hooks.py` & `aa_gdpr-0.4.3/aagdpr/theme/darkly/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/theme/flatly/auth_hooks.py` & `aa_gdpr-0.4.3/aagdpr/theme/flatly/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/aagdpr/theme/materia/auth_hooks.py` & `aa_gdpr-0.4.3/aagdpr/theme/materia/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/pyproject.toml` & `aa_gdpr-0.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_gdpr-0.4.2/PKG-INFO` & `aa_gdpr-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-gdpr
-Version: 0.4.2
+Version: 0.4.3
 Summary: A Collection of GDPR Tools for Alliance Auth
 Keywords: allianceauth,eveonline
 Author-email: Joel Falknau <joel.falknau@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Celery
```

