# Comparing `tmp/aa_timezones-2.0.0b1.tar.gz` & `tmp/aa_timezones-2.0.1.tar.gz`

## Comparing `aa_timezones-2.0.0b1.tar` & `aa_timezones-2.0.1.tar`

### file list

```diff
@@ -1,308 +1,316 @@
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/__init__.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/admin.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/app_settings.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/apps.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/auth_hooks.py
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/constants.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/models.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/urls.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/views.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/aadiscordbot/cogs/time.py
--rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/django.pot
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7129 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7046 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7087 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6047 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6793 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8949 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/management/commands/timezones_load_tz_data.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/migrations/0001_initial.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/migrations/0002_timezonedata_timezones.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/migrations/0003_auto_20201003_1748.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/migrations/0004_delete_aatimezones.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/migrations/0005_alter_timezonedata_options.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/migrations/__init__.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/css/timezones.css
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/css/timezones.min.css
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/css/timezones.min.css.map
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/js/timezones.js
--rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/js/timezones.min.js
--rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/js/timezones.min.js.map
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/jquery-timeago/1.6.7/jquery.timeago.js
--rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/jquery-timeago/1.6.7/jquery.timeago.min.js
--rw-r--r--   0        0        0   152829 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/moment-timezone/0.5.36/moment-timezone-with-data-1970-2030.js
--rw-r--r--   0        0        0   140183 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/moment-timezone/0.5.36/moment-timezone-with-data-1970-2030.min.js
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/bower.json
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/package.json
--rw-r--r--   0        0        0   145200 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons-wind.css
--rw-r--r--   0        0        0   126816 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons-wind.min.css
--rw-r--r--   0        0        0    30727 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons.css
--rw-r--r--   0        0        0    25853 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons.min.css
--rwxr-xr-x   0        0        0    99774 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.eot
--rwxr-xr-x   0        0        0    99564 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.ttf
--rwxr-xr-x   0        0        0    56468 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.woff
--rwxr-xr-x   0        0        0    44720 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.woff2
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons-classes.less
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons.less
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons.min.less
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/weather-icons-classes.scss
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/weather-icons-core.scss
--rw-r--r--   0        0        0    36110 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/icon-classes/classes-wind-degrees.scss
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-alien.svg
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-barometer.svg
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-celsius.svg
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-down.svg
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-refresh.svg
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-up.svg
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud.svg
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy-gusts.svg
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy-windy.svg
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy.svg
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-gusts.svg
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-high.svg
--rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-windy.svg
--rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy.svg
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-fog.svg
--rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-hail.svg
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-haze.svg
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-light-wind.svg
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-lightning.svg
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain-mix.svg
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain-wind.svg
--rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain.svg
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-showers.svg
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sleet-storm.svg
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sleet.svg
--rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow-thunderstorm.svg
--rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow-wind.svg
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow.svg
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sprinkle.svg
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-storm-showers.svg
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sunny-overcast.svg
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sunny.svg
--rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-thunderstorm.svg
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-windy.svg
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-degrees.svg
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down-left.svg
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down-right.svg
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down.svg
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-left.svg
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-right.svg
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up-left.svg
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up-right.svg
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up.svg
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-dust.svg
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-earthquake.svg
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fahrenheit.svg
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fire.svg
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-flood.svg
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fog.svg
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-gale-warning.svg
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hail.svg
--rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-horizon-alt.svg
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-horizon.svg
--rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hot.svg
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-humidity.svg
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hurricane-warning.svg
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hurricane.svg
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-lightning.svg
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-lunar-eclipse.svg
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-meteor.svg
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-first-quarter.svg
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-full.svg
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-new.svg
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-third-quarter.svg
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-1.svg
--rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-2.svg
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-3.svg
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-4.svg
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-5.svg
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-6.svg
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-1.svg
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-2.svg
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-3.svg
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-4.svg
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-5.svg
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-6.svg
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-1.svg
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-2.svg
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-3.svg
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-4.svg
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-5.svg
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-6.svg
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-1.svg
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-2.svg
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-3.svg
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-4.svg
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-5.svg
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-6.svg
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-first-quarter.svg
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-full.svg
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-new.svg
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-third-quarter.svg
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-1.svg
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-2.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-3.svg
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-4.svg
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-5.svg
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-6.svg
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-1.svg
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-2.svg
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-3.svg
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-4.svg
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-5.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-6.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-6.svg
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-1.svg
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-2.svg
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-3.svg
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-4.svg
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-5.svg
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-1.svg
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-2.svg
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-3.svg
--rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-4.svg
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-5.svg
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-6.svg
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moonrise.svg
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moonset.svg
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-na.svg
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-gusts.svg
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-high.svg
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-windy.svg
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy.svg
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-hail.svg
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-lightning.svg
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-partly-cloudy.svg
--rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain-mix.svg
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain-wind.svg
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain.svg
--rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-showers.svg
--rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sleet-storm.svg
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sleet.svg
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow-thunderstorm.svg
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow-wind.svg
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow.svg
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sprinkle.svg
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-storm-showers.svg
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-thunderstorm.svg
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-clear.svg
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-gusts.svg
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-high.svg
--rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-windy.svg
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy.svg
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-fog.svg
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-hail.svg
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-lightning.svg
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-partly-cloudy.svg
--rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain-mix.svg
--rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain-wind.svg
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain.svg
--rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-showers.svg
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sleet-storm.svg
--rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sleet.svg
--rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow-thunderstorm.svg
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow-wind.svg
--rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow.svg
--rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sprinkle.svg
--rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-storm-showers.svg
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-thunderstorm.svg
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain-mix.svg
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain-wind.svg
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain.svg
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-raindrop.svg
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-raindrops.svg
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-refresh-alt.svg
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-refresh.svg
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sandstorm.svg
--rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-showers.svg
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sleet.svg
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-small-craft-advisory.svg
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-smog.svg
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-smoke.svg
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snow-wind.svg
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snow.svg
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snowflake-cold.svg
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-solar-eclipse.svg
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sprinkle.svg
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-stars.svg
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-storm-showers.svg
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-storm-warning.svg
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-strong-wind.svg
--rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sunrise.svg
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sunset.svg
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer-exterior.svg
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer-internal.svg
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer.svg
--rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thunderstorm.svg
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-1.svg
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-10.svg
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-11.svg
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-12.svg
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-2.svg
--rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-3.svg
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-4.svg
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-5.svg
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-6.svg
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-7.svg
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-8.svg
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-9.svg
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-tornado.svg
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-train.svg
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-tsunami.svg
--rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-umbrella.svg
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-volcano.svg
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-0.svg
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-1.svg
--rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-10.svg
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-11.svg
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-12.svg
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-2.svg
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-3.svg
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-4.svg
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-5.svg
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-6.svg
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-7.svg
--rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-8.svg
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-9.svg
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-deg.svg
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-windy.svg
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/base.html
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/index.html
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/bundles/aa-timezones-css.html
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/bundles/aa-timezones-js.html
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/bundles/jquery-timeago-js.html
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/bundles/moment-timezone-js.html
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/bundles/weather-icons-css.html
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/partials/footer/app-translation-footer.html
--rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/partials/timezones/adjust-time.html
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/partials/timezones/time-until.html
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templates/timezones/partials/timezones/timezone-panel.html
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templatetags/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/templatetags/timezones.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/tests/__init__.py
--rw-r--r--   0        0        0     2260 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/tests/test_access.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/tests/test_admin.py
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/tests/test_auth_hooks.py
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/tests/test_models.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/tests/test_templatetags.py
--rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/tests/test_view.py
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/timezones/tests/utils.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/LICENSE
--rw-r--r--   0        0        0     8904 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/README.md
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/pyproject.toml
--rw-r--r--   0        0        0    51268 2020-02-02 00:00:00.000000 aa_timezones-2.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/__init__.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/admin.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/app_settings.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/apps.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/auth_hooks.py
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/constants.py
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/models.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/urls.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/views.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/aadiscordbot/cogs/time.py
+-rw-r--r--   0        0        0     5936 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/django.pot
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7202 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7124 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6120 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6397 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/pl_PL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     9045 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6204 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/sk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     8161 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/management/commands/timezones_load_tz_data.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/migrations/0002_timezonedata_timezones.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/migrations/0003_auto_20201003_1748.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/migrations/0004_delete_aatimezones.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/migrations/0005_alter_timezonedata_options.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/migrations/__init__.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/css/timezones.css
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/css/timezones.min.css
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/css/timezones.min.css.map
+-rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/js/timezones.js
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/js/timezones.min.js
+-rw-r--r--   0        0        0     4674 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/js/timezones.min.js.map
+-rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/jquery-timeago/1.6.7/jquery.timeago.js
+-rw-r--r--   0        0        0     4765 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/jquery-timeago/1.6.7/jquery.timeago.min.js
+-rw-r--r--   0        0        0   152829 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/moment-timezone/0.5.36/moment-timezone-with-data-1970-2030.js
+-rw-r--r--   0        0        0   140183 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/moment-timezone/0.5.36/moment-timezone-with-data-1970-2030.min.js
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/README.md
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/bower.json
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/package.json
+-rw-r--r--   0        0        0   145200 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons-wind.css
+-rw-r--r--   0        0        0   126816 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons-wind.min.css
+-rw-r--r--   0        0        0    30727 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons.css
+-rw-r--r--   0        0        0    25853 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons.min.css
+-rwxr-xr-x   0        0        0    99774 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.eot
+-rwxr-xr-x   0        0        0    99564 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.ttf
+-rwxr-xr-x   0        0        0    56468 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.woff
+-rwxr-xr-x   0        0        0    44720 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.woff2
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons-classes.less
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons.less
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons.min.less
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/weather-icons-classes.scss
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/weather-icons-core.scss
+-rw-r--r--   0        0        0    36110 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/icon-classes/classes-wind-degrees.scss
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-alien.svg
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-barometer.svg
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-celsius.svg
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-down.svg
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-refresh.svg
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-up.svg
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud.svg
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy-gusts.svg
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy-windy.svg
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy.svg
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-gusts.svg
+-rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-high.svg
+-rw-r--r--   0        0        0     3566 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-windy.svg
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy.svg
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-fog.svg
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-hail.svg
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-haze.svg
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-light-wind.svg
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-lightning.svg
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain-mix.svg
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain-wind.svg
+-rw-r--r--   0        0        0     3745 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain.svg
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-showers.svg
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sleet-storm.svg
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sleet.svg
+-rw-r--r--   0        0        0     4193 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow-thunderstorm.svg
+-rw-r--r--   0        0        0     4446 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow-wind.svg
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow.svg
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sprinkle.svg
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-storm-showers.svg
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sunny-overcast.svg
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sunny.svg
+-rw-r--r--   0        0        0     3688 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-thunderstorm.svg
+-rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-windy.svg
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-degrees.svg
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down-left.svg
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down-right.svg
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down.svg
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-left.svg
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-right.svg
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up-left.svg
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up-right.svg
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up.svg
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-dust.svg
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-earthquake.svg
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fahrenheit.svg
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fire.svg
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-flood.svg
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fog.svg
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-gale-warning.svg
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hail.svg
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-horizon-alt.svg
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-horizon.svg
+-rw-r--r--   0        0        0     6215 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hot.svg
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-humidity.svg
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hurricane-warning.svg
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hurricane.svg
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-lightning.svg
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-lunar-eclipse.svg
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-meteor.svg
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-first-quarter.svg
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-full.svg
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-new.svg
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-third-quarter.svg
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-1.svg
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-2.svg
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-3.svg
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-4.svg
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-5.svg
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-6.svg
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-1.svg
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-2.svg
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-3.svg
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-4.svg
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-5.svg
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-6.svg
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-1.svg
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-2.svg
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-3.svg
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-4.svg
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-5.svg
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-6.svg
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-1.svg
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-2.svg
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-3.svg
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-4.svg
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-5.svg
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-6.svg
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-first-quarter.svg
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-full.svg
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-new.svg
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-third-quarter.svg
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-1.svg
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-2.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-3.svg
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-4.svg
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-5.svg
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-6.svg
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-1.svg
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-2.svg
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-3.svg
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-4.svg
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-5.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-6.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-6.svg
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-1.svg
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-2.svg
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-3.svg
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-4.svg
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-5.svg
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-1.svg
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-2.svg
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-3.svg
+-rw-r--r--   0        0        0      662 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-4.svg
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-5.svg
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-6.svg
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moonrise.svg
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moonset.svg
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-na.svg
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-gusts.svg
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-high.svg
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-windy.svg
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy.svg
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-hail.svg
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-lightning.svg
+-rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-partly-cloudy.svg
+-rw-r--r--   0        0        0     4568 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain-mix.svg
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain-wind.svg
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain.svg
+-rw-r--r--   0        0        0     3638 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-showers.svg
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sleet-storm.svg
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sleet.svg
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow-thunderstorm.svg
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow-wind.svg
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow.svg
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sprinkle.svg
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-storm-showers.svg
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-thunderstorm.svg
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-clear.svg
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-gusts.svg
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-high.svg
+-rw-r--r--   0        0        0     2259 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-windy.svg
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy.svg
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-fog.svg
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-hail.svg
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-lightning.svg
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-partly-cloudy.svg
+-rw-r--r--   0        0        0     4302 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain-mix.svg
+-rw-r--r--   0        0        0     3048 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain-wind.svg
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain.svg
+-rw-r--r--   0        0        0     3389 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-showers.svg
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sleet-storm.svg
+-rw-r--r--   0        0        0     3731 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sleet.svg
+-rw-r--r--   0        0        0     2896 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow-thunderstorm.svg
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow-wind.svg
+-rw-r--r--   0        0        0     3154 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow.svg
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sprinkle.svg
+-rw-r--r--   0        0        0     3055 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-storm-showers.svg
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-thunderstorm.svg
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain-mix.svg
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain-wind.svg
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain.svg
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-raindrop.svg
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-raindrops.svg
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-refresh-alt.svg
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-refresh.svg
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sandstorm.svg
+-rw-r--r--   0        0        0     3385 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-showers.svg
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sleet.svg
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-small-craft-advisory.svg
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-smog.svg
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-smoke.svg
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snow-wind.svg
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snow.svg
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snowflake-cold.svg
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-solar-eclipse.svg
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sprinkle.svg
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-stars.svg
+-rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-storm-showers.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-storm-warning.svg
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-strong-wind.svg
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sunrise.svg
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sunset.svg
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer-exterior.svg
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer-internal.svg
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer.svg
+-rw-r--r--   0        0        0     2201 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thunderstorm.svg
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-1.svg
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-10.svg
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-11.svg
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-12.svg
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-2.svg
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-3.svg
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-4.svg
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-5.svg
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-6.svg
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-7.svg
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-8.svg
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-9.svg
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-tornado.svg
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-train.svg
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-tsunami.svg
+-rw-r--r--   0        0        0     2503 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-umbrella.svg
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-volcano.svg
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-0.svg
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-1.svg
+-rw-r--r--   0        0        0     2124 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-10.svg
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-11.svg
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-12.svg
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-2.svg
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-3.svg
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-4.svg
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-5.svg
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-6.svg
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-7.svg
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-8.svg
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-9.svg
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-deg.svg
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-windy.svg
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/base.html
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/index.html
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/bundles/aa-timezones-css.html
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/bundles/aa-timezones-js.html
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/bundles/jquery-timeago-js.html
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/bundles/moment-timezone-js.html
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/bundles/weather-icons-css.html
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/partials/footer/app-translation-footer.html
+-rw-r--r--   0        0        0    14571 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/partials/timezones/adjust-time.html
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/partials/timezones/time-until.html
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templates/timezones/partials/timezones/timezone-panel.html
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templatetags/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/templatetags/timezones.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/tests/__init__.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/tests/test_access.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/tests/test_admin.py
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/tests/test_auth_hooks.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/tests/test_models.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/tests/test_view.py
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/timezones/tests/utils.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/LICENSE
+-rw-r--r--   0        0        0     8993 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/README.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    51356 2020-02-02 00:00:00.000000 aa_timezones-2.0.1/PKG-INFO
```

### Comparing `aa_timezones-2.0.0b1/timezones/admin.py` & `aa_timezones-2.0.1/timezones/admin.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/app_settings.py` & `aa_timezones-2.0.1/timezones/app_settings.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/auth_hooks.py` & `aa_timezones-2.0.1/timezones/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/constants.py` & `aa_timezones-2.0.1/timezones/constants.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/models.py` & `aa_timezones-2.0.1/timezones/models.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/views.py` & `aa_timezones-2.0.1/timezones/views.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/aadiscordbot/cogs/time.py` & `aa_timezones-2.0.1/timezones/aadiscordbot/cogs/time.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/locale/django.pot` & `aa_timezones-2.0.1/timezones/locale/django.pot`

 * *Files 2% similar despite different names*

```diff
@@ -4,67 +4,68 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
+"POT-Creation-Date: 2024-03-20 17:01+0100\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=INTEGER; plural=EXPRESSION;\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
 msgstr ""
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
 msgstr ""
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 msgid "Time zone"
 msgstr ""
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 msgid "Activate selected timezones"
 msgstr ""
 
-#: timezones/admin.py:59
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
+msgid "Activated {notifications_count} timezone"
+msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] ""
 msgstr[1] ""
 
-#: timezones/admin.py:69
+#: timezones/admin.py:70
 #, python-brace-format
-msgid "Activated {notifications_count} timezone"
-msgid_plural "Activated {notifications_count} timezones"
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
 msgstr[0] ""
 msgstr[1] ""
 
-#: timezones/admin.py:75
+#: timezones/admin.py:86
 msgid "Deactivate selected timezones"
 msgstr ""
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
 msgstr[0] ""
 msgstr[1] ""
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
 msgstr[0] ""
 msgstr[1] ""
 
 #: timezones/apps.py:20
@@ -105,129 +106,129 @@
 msgstr ""
 
 #: timezones/models.py:79
 msgid "Timezones"
 msgstr ""
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 msgid "Local time"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
 msgstr ""
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 msgid "Adjust time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
 msgid "Set time to be in"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 msgid "Set time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
 msgstr ""
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr ""
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/de/LC_MESSAGES/django.mo` & `aa_timezones-2.0.1/timezones/locale/de/LC_MESSAGES/django.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,18 +7,15 @@
 "Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-timezones/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
-
-msgid "Activate selected timezone(s)"
-msgstr "Ausgewählte Zeitzonen aktivieren"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Activate selected timezones"
 msgstr "Ausgewählte Zeitzonen aktivieren"
 
 msgid "Activated {notifications_count} timezone"
 msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] "{notifications_count} Zeitzone aktiviert"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/de/LC_MESSAGES/django.po` & `aa_timezones-2.0.1/timezones/locale/de/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Peter Pfeufer <rounon.dax@terra-nanotech.de>, 2020
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 #
 # Translators:
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
-"PO-Revision-Date: 2023-09-27 17:06+0000\n"
+"POT-Creation-Date: 2024-03-16 02:05+0100\n"
+"PO-Revision-Date: 2024-05-10 14:13+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: German <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-timezones/de/>\n"
+"Language-Team: German <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-timezones/de/>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
 msgstr "Zeitzonen"
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
 msgstr "Panel Name"
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 msgid "Time zone"
 msgstr "Zeitzone"
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 msgid "Activate selected timezones"
 msgstr "Ausgewählte Zeitzonen aktivieren"
 
-#: timezones/admin.py:59
-#, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
-msgstr[0] "Aktivieren von {failed} Zeitzone ist fehlgeschlagen"
-msgstr[1] "Aktivieren von {failed} Zeitzonen ist fehlgeschlagen"
-
-#: timezones/admin.py:69
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
 msgid "Activated {notifications_count} timezone"
 msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] "{notifications_count} Zeitzone aktiviert"
 msgstr[1] "{notifications_count} Zeitzonen aktiviert"
 
-#: timezones/admin.py:75
+#: timezones/admin.py:70
+#, python-brace-format
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
+msgstr[0] "Aktivieren von {failed} Zeitzone ist fehlgeschlagen"
+msgstr[1] "Aktivieren von {failed} Zeitzonen ist fehlgeschlagen"
+
+#: timezones/admin.py:86
 msgid "Deactivate selected timezones"
 msgstr "Ausgewählte Zeitzonen deaktivieren"
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
 msgstr[0] "Deaktivieren von {failed} Zeitzone ist fehlgeschlagen"
 msgstr[1] "Deaktivieren von {failed} Zeitzonen ist fehlgeschlagen"
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
 msgstr[0] "{notifications_count} Zeitzone deaktiviert"
 msgstr[1] "{notifications_count} Zeitzonen deaktiviert"
 
 #: timezones/apps.py:20
@@ -109,35 +110,35 @@
 msgstr "Zeitzone"
 
 #: timezones/models.py:79
 msgid "Timezones"
 msgstr "Zeitzonen"
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 msgid "Local time"
 msgstr "Ortszeit"
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
 msgstr "lade"
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
 msgstr "Eve Zeit"
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
 msgstr "Tage"
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
 msgstr "Schon vorbei, Du hast alles verpasst!"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -145,95 +146,95 @@
 "Du möchtest helfen diese App in Deine Sprache zu übersetzen oder die "
 "bestehende Übersetzung verbessern?"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Tritt unserm Team von Übersetzern bei!"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 msgid "Adjust time"
 msgstr "Zeit anpassen"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
 msgstr "Entfernen"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
 msgstr "Zur aktuellen Zeit wechseln"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
 msgstr "Zur angepassten Zeit wechseln"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
 msgid "Set time to be in"
 msgstr "Setze Zeit in"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
 msgstr "Stunden"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
 msgstr "Minuten"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 msgid "Set time"
 msgstr "Zeit setzen"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
 msgstr "Setze Zeit und Datum"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
 msgstr "Januar"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
 msgstr "Februar"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
 msgstr "März"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
 msgstr "April"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
 msgstr "Mai"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
 msgstr "Juni"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
 msgstr "Juli"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
 msgstr "August"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
 msgstr "September"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
 msgstr "Oktober"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
 msgstr "November"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
 msgstr "Dezember"
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr "Verbleibend"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/es/LC_MESSAGES/django.mo` & `aa_timezones-2.0.1/timezones/locale/es/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-timezones/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Already over, you missed it!"
 msgstr "Ya terminó, te lo perdiste!"
 
 msgid "April"
 msgstr "Abril"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/es/LC_MESSAGES/django.po` & `aa_timezones-2.0.1/timezones/locale/es/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,77 +1,78 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
-# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023.
+# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
+# Zigor Fernandez Moreno <sietehierros@gmail.com>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-timezones/es/>\n"
+"POT-Creation-Date: 2024-03-16 02:05+0100\n"
+"PO-Revision-Date: 2024-05-10 14:13+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Spanish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-timezones/es/>\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
 msgstr "Zonas horarias"
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
 msgstr ""
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 #, fuzzy
 #| msgid "Timezone"
 msgid "Time zone"
 msgstr "Zona horaria"
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 #, fuzzy
 #| msgid "Selected timezone"
 msgid "Activate selected timezones"
 msgstr "Zona horaria seleccionada"
 
-#: timezones/admin.py:59
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
+msgid "Activated {notifications_count} timezone"
+msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] ""
 msgstr[1] ""
 
-#: timezones/admin.py:69
+#: timezones/admin.py:70
 #, python-brace-format
-msgid "Activated {notifications_count} timezone"
-msgid_plural "Activated {notifications_count} timezones"
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
 msgstr[0] ""
 msgstr[1] ""
 
-#: timezones/admin.py:75
+#: timezones/admin.py:86
 #, fuzzy
 #| msgid "Selected timezone"
 msgid "Deactivate selected timezones"
 msgstr "Zona horaria seleccionada"
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
 msgstr[0] ""
 msgstr[1] ""
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
 msgstr[0] ""
 msgstr[1] ""
 
 #: timezones/apps.py:20
@@ -114,37 +115,37 @@
 msgstr "Zona horaria"
 
 #: timezones/models.py:79
 msgid "Timezones"
 msgstr "Zonas horarias"
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 #, fuzzy
 #| msgid "Local Time"
 msgid "Local time"
 msgstr "Hora local"
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
 msgstr "cargando"
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
 msgstr "Días"
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
 msgstr "Ya terminó, te lo perdiste!"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -152,99 +153,99 @@
 "¿Quieres ayudar a traducir esta aplicación a tu idioma o mejorar la "
 "traducción existente?"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "¡Únete a nuestro equipo de traductores!"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 #, fuzzy
 #| msgid "Adjust Time"
 msgid "Adjust time"
 msgstr "Ajustar hora"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
 msgstr "Eliminar"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
 msgstr "Cambiar a la hora actual"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
 msgstr "Cambiar al tiempo ajustado"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
 msgid "Set time to be in"
 msgstr "Establecer tiempo para estar en"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
 msgstr "Horas"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
 msgstr "Minutos"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 #, fuzzy
 #| msgid "Set Time"
 msgid "Set time"
 msgstr "Fijar tiempo"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
 msgstr "Establecer la hora para estar en una fecha y hora específicas"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
 msgstr "Enero"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
 msgstr "Febrero"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
 msgstr "Marzo"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
 msgstr "Abril"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
 msgstr "Mayo"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
 msgstr "Junio"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
 msgstr "Julio"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
 msgstr "Agosto"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
 msgstr "Septiembre"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
 msgstr "Octubre"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
 msgstr "Noviembre"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
 msgstr "Diciembre"
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr "Tiempo restante"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/fr_FR/LC_MESSAGES/django.po` & `aa_timezones-2.0.1/timezones/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,73 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # "H. Peter Pfeufer" <info@ppfeufer.de>, 2023, 2024.
 # erka Ekanon <M6musicT@hotmail.fr>, 2024.
+# Matthias P <randomusernetcom@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
-"PO-Revision-Date: 2024-02-03 19:02+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"POT-Creation-Date: 2024-03-16 02:05+0100\n"
+"PO-Revision-Date: 2024-05-10 14:13+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
 "Language-Team: French <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-timezones/fr/>\n"
 "Language: fr_FR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n > 1;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
 msgstr "Fuseaux horaires"
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
 msgstr "Nom du panneau"
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 msgid "Time zone"
 msgstr "Fuseau horaire"
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 msgid "Activate selected timezones"
 msgstr "Activer les fuseaux horaires sélectionnés"
 
-#: timezones/admin.py:59
-#, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
-msgstr[0] "Échec de l'activation du fuseau horaire {failed}"
-msgstr[1] "Échec de l'activation des fuseaux horaires {failed}"
-
-#: timezones/admin.py:69
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
 msgid "Activated {notifications_count} timezone"
 msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] "{notifications_count} fuseau horaire activé"
 msgstr[1] "{notifications_count} fuseaux horaires activés"
 
-#: timezones/admin.py:75
+#: timezones/admin.py:70
+#, python-brace-format
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
+msgstr[0] "Échec de l'activation du fuseau horaire {failed}"
+msgstr[1] "Échec de l'activation des fuseaux horaires {failed}"
+
+#: timezones/admin.py:86
 msgid "Deactivate selected timezones"
 msgstr "Désactiver les fuseaux horaires sélectionnés"
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
 msgstr[0] "Échec de la désactivation du fuseau horaire {failed}"
 msgstr[1] "Échec de la désactivation des fuseaux horaires {failed}"
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
 msgstr[0] "{notifications_count} fuseau horaire désactivé"
 msgstr[1] "{notifications_count} fuseaux horaires désactivés"
 
 #: timezones/apps.py:20
@@ -106,131 +108,132 @@
 msgstr "Fuseau horaire"
 
 #: timezones/models.py:79
 msgid "Timezones"
 msgstr "Fuseaux horaires"
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 msgid "Local time"
 msgstr "Heure locale"
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
 msgstr "chargement"
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
-msgstr ""
+msgstr "Heure d'Eve"
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
-msgstr ""
+msgstr "Jours"
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
-msgstr ""
+msgstr "Déjà fini, vous l'avez manqué !"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 "Voulez-vous aider à traduire cette application dans votre langue ou "
 "améliorer la traduction existante ?"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Rejoignez notre équipe de traducteurs !"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 msgid "Adjust time"
-msgstr ""
+msgstr "Ajuster le temps"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
-msgstr ""
+msgstr "Supprimer"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
-msgstr ""
+msgstr "Basculer sur le temps actuel"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
-msgstr ""
+msgstr "Basculer sur le temps ajusté"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#, fuzzy
 msgid "Set time to be in"
-msgstr ""
+msgstr "Paramétrez le temps pour qu'il soit dans"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
-msgstr ""
+msgstr "Heures"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
-msgstr ""
+msgstr "Minutes"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 msgid "Set time"
-msgstr ""
+msgstr "Régler l'heure"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
-msgstr ""
+msgstr "Régler l'heure pour qu'il soit a une date et heure précise"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
 msgstr "Janvier"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
 msgstr "Février"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
 msgstr "Mars"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
 msgstr "Avril"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
 msgstr "Mai"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
 msgstr "Juin"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
 msgstr "Juillet"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
 msgstr "Août"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
 msgstr "Septembre"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
 msgstr "Octobre"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
 msgstr "Novembre"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
 msgstr "Décembre"
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr ""
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/it_IT/LC_MESSAGES/django.mo` & `aa_timezones-2.0.1/timezones/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files 12% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-timezones/it/>\n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "April"
 msgstr "Aprile"
 
 msgid "August"
 msgstr "Agosto"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/it_IT/LC_MESSAGES/django.po` & `aa_timezones-2.0.1/timezones/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# "H. Peter Pfeufer" <info@ppfeufer.de>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
-"Language-Team: Italian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-timezones/it/>\n"
-"Language: it_IT\n"
+"POT-Creation-Date: 2024-03-20 17:01+0100\n"
+"PO-Revision-Date: 2024-05-10 14:13+0000\n"
+"Last-Translator: Anonymous <noreply@weblate.org>\n"
+"Language-Team: Polish <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-timezones/pl/>\n"
+"Language: pl_PL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n != 1;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=3; plural=n==1 ? 0 : n%10>=2 && n%10<=4 && (n%100<10 "
+"|| n%100>=20) ? 1 : 2;\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
 msgstr ""
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
 msgstr ""
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 msgid "Time zone"
 msgstr ""
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 msgid "Activate selected timezones"
 msgstr ""
 
-#: timezones/admin.py:59
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
+msgid "Activated {notifications_count} timezone"
+msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: timezones/admin.py:69
+#: timezones/admin.py:70
 #, python-brace-format
-msgid "Activated {notifications_count} timezone"
-msgid_plural "Activated {notifications_count} timezones"
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: timezones/admin.py:75
+#: timezones/admin.py:86
 msgid "Deactivate selected timezones"
 msgstr ""
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
 
 #: timezones/apps.py:20
 #, python-brace-format
 msgid "Time Zones v{__version__}"
 msgstr ""
 
 #: timezones/models.py:16
@@ -105,129 +111,131 @@
 msgstr ""
 
 #: timezones/models.py:79
 msgid "Timezones"
 msgstr ""
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 msgid "Local time"
-msgstr ""
+msgstr "Czas lokalny"
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
-msgstr ""
+msgstr "Czas Gry"
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
 msgstr ""
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
+"Chciałbyś pomóc w tłumaczeniu tej apki na Twój język bądź poprawić aktualne "
+"tłumaczenia?"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
-msgstr ""
+msgstr "Dołącz do naszego zespołu tłumaczy!"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 msgid "Adjust time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
-msgstr ""
+msgstr "Usuń"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
 msgid "Set time to be in"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 msgid "Set time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
-msgstr "Gennaio"
+msgstr "Styczeń"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
-msgstr "Febbraio"
+msgstr "Luty"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
-msgstr "Marzo"
+msgstr "Marzec"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
-msgstr "Aprile"
+msgstr "Kwiecień"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
-msgstr "Maggio"
+msgstr "Maj"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
-msgstr "Giugno"
+msgstr "Czerwiec"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
-msgstr "Luglio"
+msgstr "Lipiec"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
-msgstr "Agosto"
+msgstr "Sierpień"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
-msgstr "Settembre"
+msgstr "Wrzesień"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
-msgstr "Ottobre"
+msgstr "Pażdziernik"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
-msgstr "Novembre"
+msgstr "Listopad"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
-msgstr "Dicembre"
+msgstr "Grudzień"
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/ja/LC_MESSAGES/django.mo` & `aa_timezones-2.0.1/timezones/locale/ja/LC_MESSAGES/django.mo`

 * *Files 15% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,15 +7,15 @@
 "Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-timezones/ja/>\n"
 "Language: ja\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "April"
 msgstr "4月"
 
 msgid "August"
 msgstr "8月"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/ja/LC_MESSAGES/django.po` & `aa_timezones-2.0.1/timezones/locale/sk/LC_MESSAGES/django.po`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,86 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
+#
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
-"PO-Revision-Date: 2023-09-24 13:13+0000\n"
+"POT-Creation-Date: 2024-03-20 17:01+0100\n"
+"PO-Revision-Date: 2024-05-10 14:13+0000\n"
 "Last-Translator: Anonymous <noreply@weblate.org>\n"
-"Language-Team: Japanese <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-timezones/ja/>\n"
-"Language: ja\n"
+"Language-Team: Slovak <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-timezones/sk/>\n"
+"Language: sk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.0.2\n"
+"Plural-Forms: nplurals=4; plural=(n % 1 == 0 && n == 1 ? 0 : n % 1 == 0 && n "
+">= 2 && n <= 4 ? 1 : n % 1 != 0 ? 2: 3);\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
 msgstr ""
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
 msgstr ""
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 msgid "Time zone"
 msgstr ""
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 msgid "Activate selected timezones"
 msgstr ""
 
-#: timezones/admin.py:59
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
+msgid "Activated {notifications_count} timezone"
+msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
-#: timezones/admin.py:69
+#: timezones/admin.py:70
 #, python-brace-format
-msgid "Activated {notifications_count} timezone"
-msgid_plural "Activated {notifications_count} timezones"
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
-#: timezones/admin.py:75
+#: timezones/admin.py:86
 msgid "Deactivate selected timezones"
 msgstr ""
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
 msgstr[0] ""
+msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #: timezones/apps.py:20
 #, python-brace-format
 msgid "Time Zones v{__version__}"
 msgstr ""
 
 #: timezones/models.py:16
@@ -101,129 +116,129 @@
 msgstr ""
 
 #: timezones/models.py:79
 msgid "Timezones"
 msgstr ""
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 msgid "Local time"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
 msgstr ""
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 msgid "Adjust time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
 msgid "Set time to be in"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 msgid "Set time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
-msgstr "1月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
-msgstr "2月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
-msgstr "3月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
-msgstr "4月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
-msgstr "5月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
-msgstr "6月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
-msgstr "7月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
-msgstr "8月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
-msgstr "9月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
-msgstr "10月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
-msgstr "11月"
+msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
-msgstr "12月"
+msgstr ""
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr ""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/ko_KR/LC_MESSAGES/django.mo` & `aa_timezones-2.0.1/timezones/locale/ko_KR/LC_MESSAGES/django.mo`

 * *Files 25% similar despite different names*

#### msgunfmt {}

```diff
@@ -7,39 +7,58 @@
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/alliance-auth-"
 "apps/aa-timezones/ko/>\n"
 "Language: ko\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
+
+msgid "Activated {notifications_count} timezone"
+msgid_plural "Activated {notifications_count} timezones"
+msgstr[0] "{notifications_count} 개의 시간대가 활성화됨"
 
 msgid "Already over, you missed it!"
 msgstr "이미 지났습니다, 놓치셨군요!"
 
 msgid "April"
 msgstr "4월"
 
 msgid "August"
 msgstr "8월"
 
 msgid "Days"
 msgstr "일"
 
+msgid "Deactivate selected timezones"
+msgstr "선택한 타임존 비활성화"
+
+msgid "Deactivated {notifications_count} timezone"
+msgid_plural "Deactivated {notifications_count} timezones"
+msgstr[0] "{notifications_count} 개의 시간대 비활성화됨"
+
 msgid "December"
 msgstr "12월"
 
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 msgid "Eve time"
 msgstr "이브 표준시간"
 
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
+msgstr[0] "{failed} 개의 시간대 활성화에 실패했습니다"
+
+msgid "Failed to deactivate {failed} timezone"
+msgid_plural "Failed to deactivate {failed} timezones"
+msgstr[0] "{failed} 개의 시간대 비활성화에 실패 했습니다"
+
 msgid "February"
 msgstr "2월"
 
 msgid "Hours"
 msgstr "시간"
 
 msgid "ID of the timezone panel in frontend"
@@ -113,14 +132,17 @@
 
 msgid "Time zone"
 msgstr "시간대"
 
 msgid "Timezone"
 msgstr "시간대"
 
+msgid "Timezone data"
+msgstr "시간대 데이터"
+
 msgid "Timezones"
 msgstr "시간대"
 
 msgid "UTC offset of the timezone"
 msgstr "UTC 오프셋 타임존"
 
 msgid "Whether this timezone is enabled or not"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/ko_KR/LC_MESSAGES/django.po` & `aa_timezones-2.0.1/timezones/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
-# Author50CO <tkddlschry@gmail.com>, 2023.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Author50CO <tkddlschry@gmail.com>, 2023, 2024.
+# Rodpold Shard <rodpold@gmail.com>, 2024.
+# Mind of the Raven <okanieva@gmail.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
-"PO-Revision-Date: 2023-12-29 10:04+0000\n"
-"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"POT-Creation-Date: 2024-03-16 02:05+0100\n"
+"PO-Revision-Date: 2024-05-10 14:13+0000\n"
+"Last-Translator: Mind of the Raven <okanieva@gmail.com>\n"
 "Language-Team: Korean <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-timezones/ko/>\n"
 "Language: ko_KR\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
 msgstr "시간대"
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
 msgstr "패널 이름"
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 msgid "Time zone"
 msgstr "시간대"
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 #, fuzzy
 #| msgid "Selected timezone"
 msgid "Activate selected timezones"
 msgstr "선택된 시간대"
 
-#: timezones/admin.py:59
-#, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
-msgstr[0] ""
-
-#: timezones/admin.py:69
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
 msgid "Activated {notifications_count} timezone"
 msgid_plural "Activated {notifications_count} timezones"
-msgstr[0] ""
+msgstr[0] "{notifications_count} 개의 시간대가 활성화됨"
 
-#: timezones/admin.py:75
-#, fuzzy
-#| msgid "Selected timezone"
+#: timezones/admin.py:70
+#, python-brace-format
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
+msgstr[0] "{failed} 개의 시간대 활성화에 실패했습니다"
+
+#: timezones/admin.py:86
 msgid "Deactivate selected timezones"
-msgstr "선택된 시간대"
+msgstr "선택한 타임존 비활성화"
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
-msgstr[0] ""
+msgstr[0] "{failed} 개의 시간대 비활성화에 실패 했습니다"
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
-msgstr[0] ""
+msgstr[0] "{notifications_count} 개의 시간대 비활성화됨"
 
 #: timezones/apps.py:20
 #, python-brace-format
 msgid "Time Zones v{__version__}"
 msgstr ""
 
 #: timezones/models.py:16
@@ -82,16 +83,14 @@
 msgstr "UTC 오프셋 타임존"
 
 #: timezones/models.py:30
 msgid "ID of the timezone panel in frontend"
 msgstr "프론트엔드의 타임존 패널 ID"
 
 #: timezones/models.py:41 timezones/models.py:42
-#, fuzzy
-#| msgid "Timezone Data"
 msgid "Timezone data"
 msgstr "시간대 데이터"
 
 #: timezones/models.py:55
 msgid "Name of the timezone panel"
 msgstr "시간대 패널 이름"
 
@@ -108,133 +107,133 @@
 msgstr "시간대"
 
 #: timezones/models.py:79
 msgid "Timezones"
 msgstr "시간대"
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 msgid "Local time"
 msgstr "현지 시간"
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
 msgstr "로딩 중"
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
 msgstr "이브 표준시간"
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
 msgstr "일"
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
 msgstr "이미 지났습니다, 놓치셨군요!"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "이 앱을 번역하거나 기존 번역을 개선하고 싶으신가요?"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "번역가 팀에 참여하세요!"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 #, fuzzy
 #| msgid "Adjust Time"
 msgid "Adjust time"
 msgstr "시간 조정"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
 msgstr "제거"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
 msgstr "현재 시간으로 변경"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
 msgstr "조정된 시간으로 변경"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
 msgid "Set time to be in"
 msgstr "현재 시간 기준 시간 설정"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
 msgstr "시간"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
 msgstr "분"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 #, fuzzy
 #| msgid "Set Time"
 msgid "Set time"
 msgstr "시간 설정"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
 msgstr "특정 시각 기준 시각 설정"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
 msgstr "1월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
 msgstr "2월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
 msgstr "3월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
 msgstr "4월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
 msgstr "5월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
 msgstr "6월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
 msgstr "7월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
 msgstr "8월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
 msgstr "9월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
 msgstr "10월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
 msgstr "11월"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
 msgstr "12월"
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr "남은 시간"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/ru/LC_MESSAGES/django.mo` & `aa_timezones-2.0.1/timezones/locale/ru/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-timezones/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Activate selected timezones"
 msgstr "Активация выбранного часового пояса"
 
 msgid "Activated {notifications_count} timezone"
 msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] "Активированный часовой пояс {notifications_count}"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/ru/LC_MESSAGES/django.po` & `aa_timezones-2.0.1/timezones/locale/ru/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,83 +1,84 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Nikolay <nick.postnikov@gmail.com>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
-# Max <mark25@inbox.ru>, 2023.
+# Nikolay <nick.postnikov@gmail.com>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Max <mark25@inbox.ru>, 2023, 2024.
 #
 # Translators:
 # Николай Постников, 2021
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
-"PO-Revision-Date: 2023-10-03 15:43+0000\n"
-"Last-Translator: Max <mark25@inbox.ru>\n"
+"POT-Creation-Date: 2024-03-16 02:05+0100\n"
+"PO-Revision-Date: 2024-05-10 14:13+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: Russian <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-timezones/ru/>\n"
 "Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
 msgstr "Часовые пояса"
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
 msgstr "Название панели"
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 msgid "Time zone"
 msgstr "Часовой пояс"
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 msgid "Activate selected timezones"
 msgstr "Активация выбранного часового пояса"
 
-#: timezones/admin.py:59
-#, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
-msgstr[0] "Не удалось активировать {failed} часовой пояс"
-msgstr[1] "Не удалось активировать {failed} часовые пояса"
-msgstr[2] "Не удалось активировать {failed} часовые пояса"
-msgstr[3] "Не удалось активировать {failed} часовые пояса"
-
-#: timezones/admin.py:69
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
 msgid "Activated {notifications_count} timezone"
 msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] "Активированный часовой пояс {notifications_count}"
 msgstr[1] "Активированные часовые пояса {notifications_count}"
 msgstr[2] "Активированные часовые пояса {notifications_count}"
 msgstr[3] "Активированные часовые пояса {notifications_count}"
 
-#: timezones/admin.py:75
+#: timezones/admin.py:70
+#, python-brace-format
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
+msgstr[0] "Не удалось активировать {failed} часовой пояс"
+msgstr[1] "Не удалось активировать {failed} часовые пояса"
+msgstr[2] "Не удалось активировать {failed} часовые пояса"
+msgstr[3] "Не удалось активировать {failed} часовые пояса"
+
+#: timezones/admin.py:86
 msgid "Deactivate selected timezones"
 msgstr "Деактивировать выбранный часовой пояс"
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
 msgstr[0] "Не удалось отключить {failed} часовой пояс"
 msgstr[1] "Не удалось отключить {failed} часовые пояса"
 msgstr[2] "Не удалось отключить {failed} часовые пояса"
 msgstr[3] "Не удалось отключить {failed} часовые пояса"
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
 msgstr[0] "Отключенный часовой пояс {notifications_count}"
 msgstr[1] "Отключенные часовые пояса {notifications_count}"
 msgstr[2] "Отключенные часовые пояса {notifications_count}"
 msgstr[3] "Отключенные часовые пояса {notifications_count}"
@@ -120,35 +121,35 @@
 msgstr "Часовой пояс"
 
 #: timezones/models.py:79
 msgid "Timezones"
 msgstr "Часовые пояса"
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 msgid "Local time"
 msgstr "Местное время"
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
 msgstr "загрузка"
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
 msgstr "Время Eve"
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
 msgstr "дней"
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
 msgstr "Поздно, установленное время уже в прошлом!"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
@@ -156,95 +157,95 @@
 "Вы хотите помочь перевести это приложение на ваш язык или улучшить текущий "
 "перевод?"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "Присоединяйтесь к нашей команде переводчиков!"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 msgid "Adjust time"
 msgstr "Задать время"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
 msgstr "Удалить"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
 msgstr "Показать текущее время"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
 msgstr "Показать заданное время"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
 msgid "Set time to be in"
 msgstr "Задать время через"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
 msgstr "часов"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
 msgstr "минут"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 msgid "Set time"
 msgstr "Установить время"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
 msgstr "Установите время на определенное время и дату"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
 msgstr "Январь"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
 msgstr "Февраль"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
 msgstr "Март"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
 msgstr "Апрель"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
 msgstr "Май"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
 msgstr "Июнь"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
 msgstr "Июль"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
 msgstr "Август"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
 msgstr "Сентябрь"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
 msgstr "Октябрь"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
 msgstr "Ноябрь"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
 msgstr "Декабрь"
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr "Осталось времени"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/uk/LC_MESSAGES/django.mo` & `aa_timezones-2.0.1/timezones/locale/uk/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -8,15 +8,15 @@
 "apps/aa-timezones/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
 msgid "Activate selected timezones"
 msgstr "Активувати обрані часові пояси"
 
 msgid "Activated {notifications_count} timezone"
 msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] "Активований {notifications_count} часовий пояс"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/uk/LC_MESSAGES/django.po` & `aa_timezones-2.0.1/timezones/locale/uk/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# Kristof <kristof@teh.ninja>, 2023.
-# Peter Pfeufer <info@ppfeufer.de>, 2023.
+# Kristof <kristof@teh.ninja>, 2023, 2024.
+# Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
-"PO-Revision-Date: 2023-10-01 10:43+0000\n"
-"Last-Translator: Kristof <kristof@teh.ninja>\n"
-"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/alliance-auth-"
-"apps/aa-timezones/uk/>\n"
+"POT-Creation-Date: 2024-03-16 02:05+0100\n"
+"PO-Revision-Date: 2024-05-10 14:13+0000\n"
+"Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
+"Language-Team: Ukrainian <https://weblate.ppfeufer.de/projects/"
+"alliance-auth-apps/aa-timezones/uk/>\n"
 "Language: uk\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=4; plural=n==1 ? 3 : (n%10==1 && n%100!=11 ? 0 : "
 "n%10>=2 && n%10<=4 && (n%100<10 || n%100>=20) ? 1 : 2);\n"
-"X-Generator: Weblate 5.0.2\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
 msgstr "Часові пояси"
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
 msgstr "Назва панелі"
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 #, fuzzy
 #| msgid "Timezone"
 msgid "Time zone"
 msgstr "Часовий пояс"
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 msgid "Activate selected timezones"
 msgstr "Активувати обрані часові пояси"
 
-#: timezones/admin.py:59
-#, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
-msgstr[0] "Не вийшло активувати {failed} часовий пояс"
-msgstr[1] "Не вийшло активувати {failed} пояси"
-msgstr[2] "Не вийшло активувати {failed} часові пояси"
-msgstr[3] "Не вийшло активувати {failed} часові пояси"
-
-#: timezones/admin.py:69
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
 msgid "Activated {notifications_count} timezone"
 msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] "Активований {notifications_count} часовий пояс"
 msgstr[1] "Активовані {notifications_count}часові пояси"
 msgstr[2] "Активовані {notifications_count}часові пояси"
 msgstr[3] "Активовані {notifications_count}часові пояси"
 
-#: timezones/admin.py:75
+#: timezones/admin.py:70
+#, python-brace-format
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
+msgstr[0] "Не вийшло активувати {failed} часовий пояс"
+msgstr[1] "Не вийшло активувати {failed} пояси"
+msgstr[2] "Не вийшло активувати {failed} часові пояси"
+msgstr[3] "Не вийшло активувати {failed} часові пояси"
+
+#: timezones/admin.py:86
 msgid "Deactivate selected timezones"
 msgstr "Деактивувати обрані часові пояси"
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
 msgstr[0] ""
 msgstr[1] ""
 msgstr[2] ""
 msgstr[3] ""
@@ -119,135 +120,135 @@
 msgstr "Часовий пояс"
 
 #: timezones/models.py:79
 msgid "Timezones"
 msgstr "Часові пояси"
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 #, fuzzy
 #| msgid "Local Time"
 msgid "Local time"
 msgstr "Місцевий час"
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
 msgstr "завантаження"
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
 msgstr "Днів"
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
 msgstr "Вже закінчилося, ви все пропустили!"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr ""
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 #, fuzzy
 #| msgid "Adjust Time"
 msgid "Adjust time"
 msgstr "Налаштувати час"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
 msgstr "Видалити"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
 msgstr "Перейти на поточний час"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
 msgstr "Перейти до налаштованого часу"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
 msgid "Set time to be in"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
 msgstr "Годин"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
 msgstr "Мінут"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 #, fuzzy
 #| msgid "Set Time"
 msgid "Set time"
 msgstr "Встановити час"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
 msgstr "Встановіть час на певний час і дату"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
 msgstr "Січень"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
 msgstr "Лютий"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
 msgstr "Березень"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
 msgstr "Квітень"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
 msgstr "Травень"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
 msgstr "Червень"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
 msgstr "Липень"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
 msgstr "Серпень"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
 msgstr "Вересень"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
 msgstr "Жовтень"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
 msgstr "Листопад"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
 msgstr "Грудень"
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr "Час, що залишився"
```

### Comparing `aa_timezones-2.0.0b1/timezones/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_timezones-2.0.1/timezones/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files 8% similar despite different names*

```diff
@@ -1,229 +1,231 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # Peter Pfeufer <info@ppfeufer.de>, 2023, 2024.
+# Zeratu <1097222620@qq.com>, 2024.
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-01 13:30+0200\n"
-"PO-Revision-Date: 2024-02-03 19:02+0000\n"
+"POT-Creation-Date: 2024-03-16 02:05+0100\n"
+"PO-Revision-Date: 2024-05-10 14:13+0000\n"
 "Last-Translator: Peter Pfeufer <info@ppfeufer.de>\n"
 "Language-Team: Chinese (Simplified) <https://weblate.ppfeufer.de/projects/"
 "alliance-auth-apps/aa-timezones/zh_Hans/>\n"
 "Language: zh_Hans\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
-"X-Generator: Weblate 5.3.1\n"
+"X-Generator: Weblate 5.5.3\n"
 
-#: timezones/__init__.py:12 timezones/templates/timezones/base.html:5
+#: timezones/__init__.py:9 timezones/templates/timezones/base.html:6
 #: timezones/templates/timezones/base.html:10
+#: timezones/templates/timezones/base.html:17
 msgid "Time Zones"
-msgstr ""
+msgstr "时区"
 
-#: timezones/admin.py:25
+#: timezones/admin.py:26
 msgid "Panel name"
-msgstr ""
+msgstr "面板名称"
 
-#: timezones/admin.py:29
+#: timezones/admin.py:30
 msgid "Time zone"
-msgstr ""
+msgstr "时区"
 
-#: timezones/admin.py:35
+#: timezones/admin.py:36
 msgid "Activate selected timezones"
-msgstr ""
-
-#: timezones/admin.py:59
-#, python-brace-format
-msgid "Failed to activate {failed} timezone"
-msgid_plural "Failed to activate {failed} timezones"
-msgstr[0] ""
+msgstr "激活所选时区"
 
-#: timezones/admin.py:69
+#: timezones/admin.py:60 timezones/admin.py:80
 #, python-brace-format
 msgid "Activated {notifications_count} timezone"
 msgid_plural "Activated {notifications_count} timezones"
 msgstr[0] ""
 
-#: timezones/admin.py:75
+#: timezones/admin.py:70
+#, python-brace-format
+msgid "Failed to activate {failed} timezone"
+msgid_plural "Failed to activate {failed} timezones"
+msgstr[0] "激活 {failed} 时区失败"
+
+#: timezones/admin.py:86
 msgid "Deactivate selected timezones"
-msgstr ""
+msgstr "停用所选时区"
 
-#: timezones/admin.py:99
+#: timezones/admin.py:111
 #, python-brace-format
 msgid "Failed to deactivate {failed} timezone"
 msgid_plural "Failed to deactivate {failed} timezones"
-msgstr[0] ""
+msgstr[0] "停用 {failed} 时区失败"
 
-#: timezones/admin.py:109
+#: timezones/admin.py:121
 #, python-brace-format
 msgid "Deactivated {notifications_count} timezone"
 msgid_plural "Deactivated {notifications_count} timezones"
 msgstr[0] ""
 
 #: timezones/apps.py:20
 #, python-brace-format
 msgid "Time Zones v{__version__}"
-msgstr ""
+msgstr "时区 v{__version__}"
 
 #: timezones/models.py:16
 msgid "Name of the timezone"
-msgstr ""
+msgstr "时区的名称"
 
 #: timezones/models.py:23
 msgid "UTC offset of the timezone"
 msgstr ""
 
 #: timezones/models.py:30
 msgid "ID of the timezone panel in frontend"
 msgstr ""
 
 #: timezones/models.py:41 timezones/models.py:42
 msgid "Timezone data"
-msgstr ""
+msgstr "时区数据"
 
 #: timezones/models.py:55
 msgid "Name of the timezone panel"
-msgstr ""
+msgstr "时区面板的名称"
 
 #: timezones/models.py:62
 msgid "Selected timezone"
-msgstr ""
+msgstr "已选择的时区"
 
 #: timezones/models.py:67
 msgid "Whether this timezone is enabled or not"
 msgstr ""
 
 #: timezones/models.py:78
 msgid "Timezone"
-msgstr ""
+msgstr "时区"
 
 #: timezones/models.py:79
 msgid "Timezones"
-msgstr ""
+msgstr "时区"
 
 #: timezones/templates/timezones/index.html:12
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:263
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:249
 msgid "Local time"
-msgstr ""
+msgstr "当地时间"
 
-#: timezones/templates/timezones/index.html:17
-#: timezones/templates/timezones/index.html:34
-#: timezones/templates/timezones/partials/timezones/timezone-panel.html:12
+#: timezones/templates/timezones/index.html:20
+#: timezones/templates/timezones/index.html:40
+#: timezones/templates/timezones/partials/timezones/timezone-panel.html:15
 msgid "loading"
-msgstr ""
+msgstr "加载中"
 
-#: timezones/templates/timezones/index.html:29
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:265
+#: timezones/templates/timezones/index.html:32
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:251
 msgid "Eve time"
-msgstr ""
+msgstr "EVE 时间"
 
-#: timezones/templates/timezones/index.html:67
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:57
+#: timezones/templates/timezones/index.html:73
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:41
 msgid "Days"
 msgstr ""
 
-#: timezones/templates/timezones/index.html:68
+#: timezones/templates/timezones/index.html:74
 msgid "Already over, you missed it!"
 msgstr ""
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:5
 msgid ""
 "Do you want to help translate this app into your language or improve the "
 "existing translation?"
 msgstr "您想帮助将此应用程序翻译成您的母语或改进现有的翻译吗?"
 
 #: timezones/templates/timezones/partials/footer/app-translation-footer.html:8
 msgid "Join our team of translators!"
 msgstr "加入我们的翻译团队吧！"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:6
 msgid "Adjust time"
-msgstr ""
+msgstr "调整时间"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:10
 msgid "Remove"
-msgstr ""
+msgstr "移除"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:14
 msgid "Switch to current time"
-msgstr ""
+msgstr "切换至当前时间"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:34
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:18
 msgid "Switch to adjusted time"
-msgstr ""
+msgstr "切换至调整后的时间"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:43
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:26
 msgid "Set time to be in"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:87
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:71
 msgid "Hours"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:153
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:137
 msgid "Minutes"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:157
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:338
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:141
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:324
 msgid "Set time"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:164
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:150
 msgid "Set time to be at a specific time and date"
 msgstr ""
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:283
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:269
 msgid "January"
 msgstr "一月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:284
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:270
 msgid "February"
 msgstr "二月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:285
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:271
 msgid "March"
 msgstr "三月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:286
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:272
 msgid "April"
 msgstr "四月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:287
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:273
 msgid "May"
 msgstr "五月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:288
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:274
 msgid "June"
 msgstr "六月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:289
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:275
 msgid "July"
 msgstr "七月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:290
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:276
 msgid "August"
 msgstr "八月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:291
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:277
 msgid "September"
 msgstr "九月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:292
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:278
 msgid "October"
 msgstr "十月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:293
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:279
 msgid "November"
 msgstr "十一月"
 
-#: timezones/templates/timezones/partials/timezones/adjust-time.html:294
+#: timezones/templates/timezones/partials/timezones/adjust-time.html:280
 msgid "December"
 msgstr "十二月"
 
 #: timezones/templates/timezones/partials/timezones/time-until.html:5
 msgid "Time left"
 msgstr ""
```

### Comparing `aa_timezones-2.0.0b1/timezones/management/commands/timezones_load_tz_data.py` & `aa_timezones-2.0.1/timezones/management/commands/timezones_load_tz_data.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/migrations/0001_initial.py` & `aa_timezones-2.0.1/timezones/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/migrations/0002_timezonedata_timezones.py` & `aa_timezones-2.0.1/timezones/migrations/0002_timezonedata_timezones.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/css/timezones.min.css.map` & `aa_timezones-2.0.1/timezones/static/timezones/css/timezones.min.css.map`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/js/timezones.js` & `aa_timezones-2.0.1/timezones/static/timezones/js/timezones.js`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/js/timezones.min.js` & `aa_timezones-2.0.1/timezones/static/timezones/js/timezones.min.js`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/js/timezones.min.js.map` & `aa_timezones-2.0.1/timezones/static/timezones/js/timezones.min.js.map`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/jquery-timeago/1.6.7/jquery.timeago.js` & `aa_timezones-2.0.1/timezones/static/timezones/libs/jquery-timeago/1.6.7/jquery.timeago.js`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/jquery-timeago/1.6.7/jquery.timeago.min.js` & `aa_timezones-2.0.1/timezones/static/timezones/libs/jquery-timeago/1.6.7/jquery.timeago.min.js`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/moment-timezone/0.5.36/moment-timezone-with-data-1970-2030.js` & `aa_timezones-2.0.1/timezones/static/timezones/libs/moment-timezone/0.5.36/moment-timezone-with-data-1970-2030.js`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/moment-timezone/0.5.36/moment-timezone-with-data-1970-2030.min.js` & `aa_timezones-2.0.1/timezones/static/timezones/libs/moment-timezone/0.5.36/moment-timezone-with-data-1970-2030.min.js`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/README.md` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/README.md`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/bower.json` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/bower.json`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons-wind.css` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons-wind.css`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons-wind.min.css` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons-wind.min.css`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons.css` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons.css`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons.min.css` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/css/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.eot` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.ttf` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.woff` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.woff2` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/font/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons.less` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons.less`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons.min.less` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/less/weather-icons.min.less`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/weather-icons-core.scss` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/weather-icons-core.scss`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/icon-classes/classes-wind-degrees.scss` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/sass/icon-classes/classes-wind-degrees.scss`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-alien.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-alien.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-barometer.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-barometer.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-celsius.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-celsius.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-down.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-down.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-refresh.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-refresh.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-up.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud-up.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloud.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy-gusts.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy-gusts.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy-windy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy-windy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-cloudy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-gusts.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-gusts.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-high.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-high.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-windy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy-windy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-cloudy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-fog.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-fog.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-hail.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-hail.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-haze.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-haze.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-light-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-light-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-lightning.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-lightning.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain-mix.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain-mix.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-rain.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-showers.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-showers.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sleet-storm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sleet-storm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sleet.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sleet.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow-thunderstorm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow-thunderstorm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-snow.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sprinkle.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sprinkle.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-storm-showers.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-storm-showers.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sunny-overcast.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sunny-overcast.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sunny.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-sunny.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-thunderstorm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-thunderstorm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-windy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-day-windy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-degrees.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-degrees.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down-left.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down-left.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down-right.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down-right.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-down.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-left.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-left.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-right.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-right.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up-left.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up-left.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up-right.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up-right.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-direction-up.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-dust.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-dust.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-earthquake.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-earthquake.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fahrenheit.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fahrenheit.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fire.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fire.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-flood.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-flood.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fog.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-fog.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hail.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hail.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-horizon-alt.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-horizon-alt.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-horizon.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-horizon.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hot.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hot.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-humidity.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-humidity.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hurricane-warning.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hurricane-warning.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hurricane.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-hurricane.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-lightning.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-lightning.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-lunar-eclipse.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-lunar-eclipse.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-meteor.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-meteor.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-first-quarter.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-first-quarter.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-full.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-full.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-new.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-new.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-third-quarter.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-third-quarter.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-crescent-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waning-gibbous-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-crescent-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-alt-waxing-gibbous-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-first-quarter.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-first-quarter.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-full.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-full.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-new.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-new.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-third-quarter.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-third-quarter.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-crescent-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waning-gibbous-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-crescent-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moon-waxing-gibbous-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moonrise.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moonrise.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moonset.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-moonset.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-na.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-na.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-gusts.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-gusts.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-high.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-high.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-windy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy-windy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-cloudy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-hail.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-hail.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-lightning.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-lightning.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-partly-cloudy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-partly-cloudy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain-mix.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain-mix.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-rain.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-showers.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-showers.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sleet-storm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sleet-storm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sleet.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sleet.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow-thunderstorm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow-thunderstorm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-snow.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sprinkle.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-sprinkle.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-storm-showers.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-storm-showers.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-thunderstorm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-alt-thunderstorm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-clear.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-clear.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-gusts.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-gusts.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-high.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-high.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-windy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy-windy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-cloudy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-fog.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-fog.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-hail.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-hail.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-lightning.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-lightning.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-partly-cloudy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-partly-cloudy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain-mix.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain-mix.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-rain.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-showers.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-showers.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sleet-storm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sleet-storm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sleet.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sleet.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow-thunderstorm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow-thunderstorm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-snow.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sprinkle.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-sprinkle.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-storm-showers.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-storm-showers.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-thunderstorm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-night-thunderstorm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain-mix.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain-mix.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-rain.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-raindrop.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-raindrop.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-raindrops.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-raindrops.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-refresh-alt.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-refresh-alt.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-refresh.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-refresh.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sandstorm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sandstorm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-showers.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-showers.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sleet.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sleet.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-smog.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-smog.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-smoke.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-smoke.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snow-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snow-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snow.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snow.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snowflake-cold.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-snowflake-cold.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-solar-eclipse.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-solar-eclipse.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sprinkle.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sprinkle.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-stars.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-stars.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-storm-showers.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-storm-showers.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-strong-wind.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-strong-wind.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sunrise.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sunrise.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sunset.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-sunset.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer-exterior.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer-exterior.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer-internal.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer-internal.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thermometer.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thunderstorm.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-thunderstorm.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-10.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-10.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-11.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-11.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-12.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-12.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-7.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-7.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-8.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-8.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-9.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-time-9.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-tornado.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-tornado.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-train.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-train.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-tsunami.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-tsunami.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-umbrella.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-umbrella.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-volcano.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-volcano.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-0.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-0.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-1.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-1.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-10.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-10.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-11.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-11.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-12.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-12.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-2.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-2.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-3.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-3.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-4.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-4.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-5.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-5.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-6.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-6.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-7.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-7.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-8.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-8.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-9.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-beaufort-9.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-deg.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-wind-deg.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-windy.svg` & `aa_timezones-2.0.1/timezones/static/timezones/libs/weather-icons/2.0.10/svg/wi-windy.svg`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/templates/timezones/base.html` & `aa_timezones-2.0.1/timezones/templates/timezones/base.html`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/templates/timezones/index.html` & `aa_timezones-2.0.1/timezones/templates/timezones/index.html`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/templates/timezones/partials/timezones/adjust-time.html` & `aa_timezones-2.0.1/timezones/templates/timezones/partials/timezones/adjust-time.html`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/templates/timezones/partials/timezones/timezone-panel.html` & `aa_timezones-2.0.1/timezones/templates/timezones/partials/timezones/timezone-panel.html`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/templatetags/timezones.py` & `aa_timezones-2.0.1/timezones/templatetags/timezones.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/tests/test_access.py` & `aa_timezones-2.0.1/timezones/tests/test_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         cls.user_1001 = create_fake_user(
             character_id=1001, character_name="Peter Parker"
         )
 
         cls.html_menu = f"""
             <li class="d-flex flex-wrap m-2 p-2 pt-0 pb-0 mt-0 mb-0 me-0 pe-0">
                 <i class="nav-link fa-regular fa-clock fa-fw fa-fw align-self-center me-3 active"></i>
-                <a class="nav-link flex-fill align-self-center me-auto" href="{reverse('timezones:index')}">
+                <a class="nav-link flex-fill align-self-center me-auto active" href="{reverse('timezones:index')}">
                     Time Zones
                 </a>
             </li>
         """
 
         cls.header = """
             <div class="aa-timezones-header">
```

### Comparing `aa_timezones-2.0.0b1/timezones/tests/test_admin.py` & `aa_timezones-2.0.1/timezones/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/tests/test_auth_hooks.py` & `aa_timezones-2.0.1/timezones/tests/test_auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/tests/test_models.py` & `aa_timezones-2.0.1/timezones/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/tests/test_templatetags.py` & `aa_timezones-2.0.1/timezones/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/tests/test_view.py` & `aa_timezones-2.0.1/timezones/tests/test_view.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/timezones/tests/utils.py` & `aa_timezones-2.0.1/timezones/tests/utils.py`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/LICENSE` & `aa_timezones-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_timezones-2.0.0b1/README.md` & `aa_timezones-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -41,19 +41,21 @@
 
 ![Time Zones](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/docs/images/presentation/aa-timezones.jpg)
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Time Zones needs at least Alliance Auth v4.0.0!**
+> **AA Time Zones >= 2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.16.2`.
 
 ### Step 1: Install the App<a name="step-1-install-the-app"></a>
 
 Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
 
 ```bash
@@ -140,15 +142,15 @@
 
 ## Adjusting Time<a name="adjusting-time"></a>
 
 You can easily adjust the time that is displayed for all timezones. This is useful
 for reinforcement timers or pre-planned fleets. To do so, click on the "Adjust Time"
 button below the time zone panels, and you will see 2 different ways to set a new time.
 
-![Adjusting Time](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/docs/images/weblate/adjust-time-settings.jpg)
+![Adjusting Time](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/docs/images/weblate/aa-timezones_adjust-time-settings.jpg)
 
 The first one is meant for timers, like reinforcement timers, anchoring timers or
 the like. Its maximum is 7 days, 59 minutes and 59 seconds into the future. That
 should cover pretty much all timers you can find in Eve Online.
 
 The second one is best suited for pre-planned fleets. Here you can set a fixed date
 and time based on the selected time zone. The default selected time zone is "EVE
```

### Comparing `aa_timezones-2.0.0b1/pyproject.toml` & `aa_timezones-2.0.1/pyproject.toml`

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
     "allianceauth-app-utils>=1.25",
     "pytz>=2023.3.post1",
 ]
 [project.optional-dependencies]
 tests-allianceauth-latest = [
     "allianceauth-discordbot",
     "coverage",
```

### Comparing `aa_timezones-2.0.0b1/PKG-INFO` & `aa_timezones-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: aa-timezones
-Version: 2.0.0b1
+Version: 2.0.1
 Summary: Time Zones Overview for Alliance Auth
 Project-URL: Changelog, https://github.com/ppfeufer/aa-timezones/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://github.com/ppfeufer/aa-timezones/blob/master/README.md
 Project-URL: Donations, https://ko-fi.com/ppfeufer
 Project-URL: Homepage, https://github.com/ppfeufer/aa-timezones
 Project-URL: Source, https://github.com/ppfeufer/aa-timezones.git
 Project-URL: Tracker, https://github.com/ppfeufer/aa-timezones/issues
@@ -698,15 +698,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Requires-Dist: allianceauth-app-utils>=1.25
-Requires-Dist: allianceauth>=4.0.0b1
+Requires-Dist: allianceauth<5.0.0,>=4
 Requires-Dist: pytz>=2023.3.post1
 Provides-Extra: tests-allianceauth-latest
 Requires-Dist: allianceauth-discordbot; extra == 'tests-allianceauth-latest'
 Requires-Dist: coverage; extra == 'tests-allianceauth-latest'
 Requires-Dist: django-webtest; extra == 'tests-allianceauth-latest'
 Description-Content-Type: text/markdown
 
@@ -753,19 +753,21 @@
 
 ![Time Zones](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/docs/images/presentation/aa-timezones.jpg)
 
 ## Installation<a name="installation"></a>
 
 > \[!NOTE\]
 >
-> **AA Time Zones needs at least Alliance Auth v4.0.0!**
+> **AA Time Zones >= 2.0.0 needs at least Alliance Auth v4.0.0!**
 >
 > Please make sure to update your Alliance Auth instance _before_ you install this
 > module or update to the latest version, otherwise an update to Alliance Auth will
 > be pulled in unsupervised.
+>
+> The last version compatible with Alliance Auth v3 is `1.16.2`.
 
 ### Step 1: Install the App<a name="step-1-install-the-app"></a>
 
 Make sure you're in the virtual environment (venv) of your Alliance Auth installation.
 Then install the latest version:
 
 ```bash
@@ -852,15 +854,15 @@
 
 ## Adjusting Time<a name="adjusting-time"></a>
 
 You can easily adjust the time that is displayed for all timezones. This is useful
 for reinforcement timers or pre-planned fleets. To do so, click on the "Adjust Time"
 button below the time zone panels, and you will see 2 different ways to set a new time.
 
-![Adjusting Time](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/docs/images/weblate/adjust-time-settings.jpg)
+![Adjusting Time](https://raw.githubusercontent.com/ppfeufer/aa-timezones/master/docs/images/weblate/aa-timezones_adjust-time-settings.jpg)
 
 The first one is meant for timers, like reinforcement timers, anchoring timers or
 the like. Its maximum is 7 days, 59 minutes and 59 seconds into the future. That
 should cover pretty much all timers you can find in Eve Online.
 
 The second one is best suited for pre-planned fleets. Here you can set a fixed date
 and time based on the selected time zone. The default selected time zone is "EVE
```

