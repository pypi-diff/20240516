# Comparing `tmp/argus_htmx_frontend-0.1.tar.gz` & `tmp/argus_htmx_frontend-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argus_htmx_frontend-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "argus_htmx_frontend-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `argus_htmx_frontend-0.1.tar` & `argus_htmx_frontend-0.2.tar`

### file list

```diff
@@ -1,26 +1,68 @@
--rw-r--r--   0        0        0     1910 2024-05-03 11:15:45.167836 argus_htmx_frontend-0.1/README.rst
--rw-r--r--   0        0        0      766 2024-05-03 11:35:19.185202 argus_htmx_frontend-0.1/pyproject.toml
--rw-r--r--   0        0        0       20 2024-05-03 11:00:23.122887 argus_htmx_frontend-0.1/src/argus_htmx/__init__.py
--rw-r--r--   0        0        0       63 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.1/src/argus_htmx/admin.py
--rw-r--r--   0        0        0      179 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.1/src/argus_htmx/apps.py
--rw-r--r--   0        0        0      143 2024-05-03 11:00:23.126887 argus_htmx_frontend-0.1/src/argus_htmx/forms.py
--rw-r--r--   0        0        0        0 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.1/src/argus_htmx/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.1/src/argus_htmx/models.py
--rw-r--r--   0        0        0      842 2024-05-03 11:25:57.357257 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/base.html
--rw-r--r--   0        0        0      128 2024-05-03 11:00:23.126887 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/_incident_ack.html
--rw-r--r--   0        0        0       27 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/_incident_description.html
--rw-r--r--   0        0        0       85 2024-05-03 11:00:23.122887 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/_incident_pk.html
--rw-r--r--   0        0        0      642 2024-05-03 11:06:02.287268 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/_incident_row.html
--rw-r--r--   0        0        0       26 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/_incident_start_time.html
--rw-r--r--   0        0        0       54 2024-05-03 11:00:23.126887 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/_incident_status.html
--rw-r--r--   0        0        0       57 2024-05-03 11:06:02.287268 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/_incident_tag.html
--rw-r--r--   0        0        0      803 2024-05-03 11:00:23.126887 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/incident_add_ack.html
--rw-r--r--   0        0        0      862 2024-05-03 11:16:31.860608 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/incident_detail.html
--rw-r--r--   0        0        0      321 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/list.html
--rw-r--r--   0        0        0      359 2024-05-03 11:06:41.243772 argus_htmx_frontend-0.1/src/argus_htmx/templates/registration/login.html
--rw-r--r--   0        0        0        0 2024-05-03 11:06:02.287268 argus_htmx_frontend-0.1/src/argus_htmx/templatetags/__init__.py
--rw-r--r--   0        0        0      319 2024-05-03 11:16:31.860608 argus_htmx_frontend-0.1/src/argus_htmx/templatetags/argus_htmx.py
--rw-r--r--   0        0        0       60 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.1/src/argus_htmx/tests.py
--rw-r--r--   0        0        0      798 2024-05-03 11:25:33.256906 argus_htmx_frontend-0.1/src/argus_htmx/urls.py
--rw-r--r--   0        0        0     2142 2024-05-03 11:25:57.357257 argus_htmx_frontend-0.1/src/argus_htmx/views.py
--rw-r--r--   0        0        0     2546 1970-01-01 00:00:00.000000 argus_htmx_frontend-0.1/PKG-INFO
+-rw-r--r--   0        0        0     3030 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/README.rst
+-rw-r--r--   0        0        0      885 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-05-16 06:36:16.232378 argus_htmx_frontend-0.2/src/argus_htmx/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.2/src/argus_htmx/admin.py
+-rw-r--r--   0        0        0      179 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.2/src/argus_htmx/apps.py
+-rw-r--r--   0        0        0      468 2024-05-15 08:27:00.819713 argus_htmx_frontend-0.2/src/argus_htmx/context_processors.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/destinations/__init__.py
+-rw-r--r--   0        0        0      511 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/destinations/urls.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/incidents/__init__.py
+-rw-r--r--   0        0        0      143 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/incidents/forms.py
+-rw-r--r--   0        0        0      359 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/incidents/urls.py
+-rw-r--r--   0        0        0     3630 2024-05-16 06:50:33.906254 argus_htmx_frontend-0.2/src/argus_htmx/incidents/views.py
+-rw-r--r--   0        0        0        0 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.2/src/argus_htmx/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.2/src/argus_htmx/models.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/notificationprofiles/__init__.py
+-rw-r--r--   0        0        0      529 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/notificationprofiles/urls.py
+-rw-r--r--   0        0        0      148 2024-05-15 08:27:00.819713 argus_htmx_frontend-0.2/src/argus_htmx/static/color-schemes/blue.css
+-rw-r--r--   0        0        0      142 2024-05-15 08:27:00.819713 argus_htmx_frontend-0.2/src/argus_htmx/static/color-schemes/dark.css
+-rw-r--r--   0        0        0      143 2024-05-15 08:27:00.819713 argus_htmx_frontend-0.2/src/argus_htmx/static/color-schemes/light.css
+-rw-r--r--   0        0        0    14007 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/Chocolate.css
+-rw-r--r--   0        0        0    14863 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/Traditional.css
+-rw-r--r--   0        0        0    10674 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/bahunya.min.css
+-rw-r--r--   0        0        0     5280 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/bamboo.css
+-rw-r--r--   0        0        0       73 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/default.css
+-rw-r--r--   0        0        0     1270 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/default/background.svg
+-rw-r--r--   0        0        0      402 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/ebmf.css
+-rw-r--r--   0        0        0     5761 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/kacit.min.css
+-rw-r--r--   0        0        0    46887 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/mini-default.min.css
+-rw-r--r--   0        0        0     6953 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/no-class.min.css
+-rw-r--r--   0        0        0    70167 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/pico.classless.min.css
+-rw-r--r--   0        0        0        0 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/purehtml.css
+-rw-r--r--   0        0        0     1093 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/reset.css
+-rw-r--r--   0        0        0    12746 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/simple.css
+-rw-r--r--   0        0        0     5207 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/stylize.css
+-rw-r--r--   0        0        0     6624 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/tacit-css-1.5.0.min.css
+-rw-r--r--   0        0        0    11212 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/tufte.css
+-rw-r--r--   0        0        0     4851 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/vanilla.css
+-rw-r--r--   0        0        0     3400 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/water-dark.css
+-rw-r--r--   0        0        0     3401 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/water-light.css
+-rw-r--r--   0        0        0     2228 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/writ.min.css
+-rw-r--r--   0        0        0    12670 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/static/themes/yorha.min.css
+-rw-r--r--   0        0        0     1630 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/base.html
+-rw-r--r--   0        0        0       54 2024-05-15 08:27:00.819713 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_base.html
+-rw-r--r--   0        0        0      123 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incident_ack.html
+-rw-r--r--   0        0        0       27 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incident_description.html
+-rw-r--r--   0        0        0       80 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incident_pk.html
+-rw-r--r--   0        0        0      642 2024-05-03 11:06:02.287268 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incident_row.html
+-rw-r--r--   0        0        0       26 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incident_start_time.html
+-rw-r--r--   0        0        0       54 2024-05-03 11:00:23.126887 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incident_status.html
+-rw-r--r--   0        0        0     1073 2024-05-15 08:27:00.819713 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incident_table_row.html
+-rw-r--r--   0        0        0       57 2024-05-03 11:06:02.287268 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incident_tag.html
+-rw-r--r--   0        0        0     3669 2024-05-15 08:27:00.819713 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incidents_table.html
+-rw-r--r--   0        0        0      803 2024-05-03 11:00:23.126887 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/incident_add_ack.html
+-rw-r--r--   0        0        0      862 2024-05-03 11:16:31.860608 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/incident_detail.html
+-rw-r--r--   0        0        0      410 2024-05-15 08:27:00.819713 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/incidents_list.html
+-rw-r--r--   0        0        0      309 2024-05-16 06:50:33.906254 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/list.html
+-rw-r--r--   0        0        0      445 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/themes/themes_list.html
+-rw-r--r--   0        0        0      359 2024-05-03 11:06:41.243772 argus_htmx_frontend-0.2/src/argus_htmx/templates/registration/login.html
+-rw-r--r--   0        0        0        0 2024-05-03 11:06:02.287268 argus_htmx_frontend-0.2/src/argus_htmx/templatetags/__init__.py
+-rw-r--r--   0        0        0      319 2024-05-03 11:16:31.860608 argus_htmx_frontend-0.2/src/argus_htmx/templatetags/argus_htmx.py
+-rw-r--r--   0        0        0       60 2024-05-03 10:56:35.355953 argus_htmx_frontend-0.2/src/argus_htmx/tests.py
+-rw-r--r--   0        0        0        0 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/themes/__init__.py
+-rw-r--r--   0        0        0      152 2024-05-16 06:36:03.820467 argus_htmx_frontend-0.2/src/argus_htmx/themes/urls.py
+-rw-r--r--   0        0        0     1714 2024-05-16 06:36:03.824467 argus_htmx_frontend-0.2/src/argus_htmx/themes/views.py
+-rw-r--r--   0        0        0        0 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/timeslots/__init__.py
+-rw-r--r--   0        0        0      505 2024-05-15 11:44:23.929081 argus_htmx_frontend-0.2/src/argus_htmx/timeslots/urls.py
+-rw-r--r--   0        0        0     1106 2024-05-16 06:36:03.824467 argus_htmx_frontend-0.2/src/argus_htmx/urls.py
+-rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 argus_htmx_frontend-0.2/PKG-INFO
```

### Comparing `argus_htmx_frontend-0.1/pyproject.toml` & `argus_htmx_frontend-0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     "Programming Language :: Python :: 3 :: Only",
     "Environment :: Web Environment",
 ]
 dynamic = ["version"]
 dependencies = [
     "argus-server",
     "django-htmx",
+    # The next is for python_version < 3.12 but we simplify code by always needing it
+    "importlib_resources>=5.12",
 ]
 
 [project.urls]
 Github = "https://github.com/Uninett/argus-htmx-frontend"
 
 [project.optional-dependencies]
 docs = ["sphinx"]
```

### Comparing `argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/_incident_row.html` & `argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/_incident_row.html`

 * *Files identical despite different names*

### Comparing `argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/incident_add_ack.html` & `argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/incident_add_ack.html`

 * *Files identical despite different names*

### Comparing `argus_htmx_frontend-0.1/src/argus_htmx/templates/htmx/incidents/incident_detail.html` & `argus_htmx_frontend-0.2/src/argus_htmx/templates/htmx/incidents/incident_detail.html`

 * *Files identical despite different names*

### Comparing `argus_htmx_frontend-0.1/src/argus_htmx/urls.py` & `argus_htmx_frontend-0.2/src/argus_htmx/urls.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from django.urls import path, include
 from django.contrib.auth import views as auth_views
 
 from argus.auth.utils import get_psa_authentication_names
 from argus.auth.views import LogoutView
 
-from . import views
-
+from .incidents.urls import urlpatterns as incident_urls
+from .timeslots.urls import urlpatterns as timeslot_urls
+from .notificationprofiles.urls import urlpatterns as notificationprofile_urls
+from .destinations.urls import urlpatterns as destination_urls
+from .themes.urls import urlpatterns as theme_urls
 
 app_name = "htmx"
 urlpatterns = [
     path(
         "accounts/login/",
         auth_views.LoginView.as_view(extra_context={"oauth2_backends": get_psa_authentication_names()}),
         name="login",
     ),
     path("accounts/logout/", auth_views.LogoutView.as_view(), name="logout"),
     #path("accounts/", include("django.contrib.auth.urls")),
-    path("incidents/", views.incidents, name="htmx_incidents"),
-    path("incidents/<int:pk>/", views.incident_detail, name="htmx_incident_detail"),
-    path("incidents/<int:pk>/ack/", views.incident_add_ack, name="htmx-incident-add-ack"),
+    path("incidents/", include(incident_urls)),
+    path("timeslots/", include(timeslot_urls)),
+    path("notificationprofiles/", include(notificationprofile_urls)),
+    path("destinations/", include(destination_urls)),
+    path("themes/", include(theme_urls)),
 ]
```

### Comparing `argus_htmx_frontend-0.1/PKG-INFO` & `argus_htmx_frontend-0.2/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,17 @@
-Metadata-Version: 2.1
-Name: argus-htmx-frontend
-Version: 0.1
-Summary: HTTP Frontend as a django app for argus-server using HTMx
-Author-email: Hanne Moa <hanne.moa@sikt.no>
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Environment :: Web Environment
-Requires-Dist: argus-server
-Requires-Dist: django-htmx
-Requires-Dist: sphinx ; extra == "docs"
-Project-URL: Github, https://github.com/Uninett/argus-htmx-frontend
-Provides-Extra: docs
-
 ===================
 argus-HTMx-frontend
 ===================
 
 Experimental frontend for `argus-server`_ as a django app.
 
 Will possibly cease to exist as a separate app if the experiment is deemed
 successful.
 
-See `argus-server`_ for more abour argus.
+See `argus-server`_ for more about argus.
 
 Imports `django-htmx`_. See the `documentation for django-htmx`_
 for details.
 
 How to play
 ===========
 
@@ -59,30 +41,53 @@
     INSTALLED_APPS += [
         "django_htmx",
         "argus_htmx",
     ]
     ROOT_URLCONF = "urls.py"
     MIDDLEWARE += ["django_htmx.middleware.HtmxMiddleware"]
 
+In the same file, add a copy of the entirety of ``TEMPLATES``. Choose one of
+the functions in ``argus_htmx.context_processors``. In the entry for
+``django.template.backends.django.DjangoTemplates``, append the full dotted
+path to the end of the ``context_processors`` list.
+
 Next to ``localsettings.py`` create an ``urls.py`` containing::
 
    from argus.site.urls import urlpatterns
 
    urlpatterns += [
        path("", include("argus_htmx.urls")
    ]
 
 With EXTRA_APPS
 ~~~~~~~~~~~~~~~
 
+Choose one of the functions in ``argus_htmx.context_processors``, exemplified
+by "theme_via_GET" below.
+
 In your environment variables::
 
-    ARGUS_EXTRA_APPS = '[{"app_name": "django_htmx"},{"app_name": "argus_htmx","urls": {"path": "", "urlpatterns_module": "argus_htmx.urls"}}]'
+    ARGUS_EXTRA_APPS = '[{"app_name": "django_htmx"}, {"app_name": "argus_htmx", "urls": {"path": "", "urlpatterns_module": "argus_htmx.urls"}, "context_processors": ["argus_htmx.context_processor.theme_via_GET"]}]'
 
 In your local settings that star-imports from an `argus-server`_ settings file::
 
     MIDDLEWARE += ["django_htmx.middleware.HtmxMiddleware"]
 
+Themes
+------
+
+To try out class-less themes use the context processor
+``argus_htmx.context_processor.theme_via_session`` instead of
+``argus_htmx.context_processor.theme_via_GET``.
+
+There are plenty of themes copied from `CSS Bed`_ to play with. Your own themes
+can be added by copying one css-file per theme to the static path ``themes/``,
+either in an app or in a directory mentioned in ``STATICFILES_DIRS``.
+
+Icons, pictures, etc. used by the theme MUST be in a subdirectory named the
+same as the theme (minus the ".css") in the same directory as the theme so
+update the paths accordingly. See the included theme "default.css".
+
+.. _CSS Bed: https://www.cssbed.com/
 .. _django-htmx: https://github.com/adamchainz/django-htmx
 .. _argus-server: https://github.com/Uninett/Argus
 .. _documentation for django-htmx: https://django-htmx.readthedocs.io/en/latest/
-
```

