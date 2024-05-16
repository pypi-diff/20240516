# Comparing `tmp/django-rest-models-2.1.2.tar.gz` & `tmp/django-rest-models-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-rest-models-2.1.2.tar", last modified: Mon Mar  6 14:30:07 2023, max compression
+gzip compressed data, was "dist/django-rest-models-2.1.3.tar", last modified: Thu May 16 15:52:13 2024, max compression
```

## Comparing `django-rest-models-2.1.2.tar` & `django-rest-models-2.1.3.tar`

### file list

```diff
@@ -1,41 +1,40 @@
-drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3191 2022-09-05 10:35:17.000000 django-rest-models-2.1.2/CONTRIBUTING.rst
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     1301 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/LICENSE.md
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)      149 2018-05-16 12:56:55.000000 django-rest-models-2.1.2/MANIFEST.in
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)    10256 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/PKG-INFO
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     9418 2023-02-01 13:42:28.000000 django-rest-models-2.1.2/README.rst
-drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/django_rest_models.egg-info/
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)    10256 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/django_rest_models.egg-info/PKG-INFO
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)      967 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/django_rest_models.egg-info/SOURCES.txt
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)        1 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/django_rest_models.egg-info/dependency_links.txt
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)        1 2019-03-05 08:23:37.000000 django-rest-models-2.1.2/django_rest_models.egg-info/not-zip-safe
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)       34 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/django_rest_models.egg-info/requires.txt
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)       12 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/django_rest_models.egg-info/top_level.txt
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)      159 2023-02-01 13:42:28.000000 django-rest-models-2.1.2/requirements.txt
-drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/rest_models/
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)      150 2023-03-06 14:26:11.000000 django-rest-models-2.1.2/rest_models/__init__.py
-drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/rest_models/backend/
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)        0 2018-05-16 12:56:55.000000 django-rest-models-2.1.2/rest_models/backend/__init__.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     4055 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/rest_models/backend/auth.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3419 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/rest_models/backend/base.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     2266 2023-02-01 13:42:28.000000 django-rest-models-2.1.2/rest_models/backend/client.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)    57952 2023-02-25 13:13:39.000000 django-rest-models-2.1.2/rest_models/backend/compiler.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)    16628 2023-02-01 13:42:28.000000 django-rest-models-2.1.2/rest_models/backend/connexion.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3430 2018-05-16 12:56:55.000000 django-rest-models-2.1.2/rest_models/backend/creation.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)      731 2018-05-16 12:56:55.000000 django-rest-models-2.1.2/rest_models/backend/exceptions.py
-drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/rest_models/backend/exec/
--rwxr-xr-x   0 vakarys   (1000) vakarys   (1000)     5851 2018-05-16 12:56:55.000000 django-rest-models-2.1.2/rest_models/backend/exec/resty
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     1416 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/rest_models/backend/features.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3587 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/rest_models/backend/introspection.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3110 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/rest_models/backend/middlewares.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)      524 2023-02-25 13:21:47.000000 django-rest-models-2.1.2/rest_models/backend/operations.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)      690 2018-05-16 12:56:55.000000 django-rest-models-2.1.2/rest_models/backend/schema.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)      739 2023-02-01 13:42:28.000000 django-rest-models-2.1.2/rest_models/backend/utils.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     5464 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/rest_models/checks.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3794 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/rest_models/router.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     4290 2022-09-05 10:35:17.000000 django-rest-models-2.1.2/rest_models/storage.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)    13847 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/rest_models/test.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     6606 2020-08-12 08:40:57.000000 django-rest-models-2.1.2/rest_models/utils.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)      284 2023-03-06 14:30:07.000000 django-rest-models-2.1.2/setup.cfg
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)     2180 2023-02-01 13:42:28.000000 django-rest-models-2.1.2/setup.py
--rw-r--r--   0 vakarys   (1000) vakarys   (1000)       28 2023-02-01 13:42:28.000000 django-rest-models-2.1.2/test_requirements.txt
+drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3191 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)      149 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/MANIFEST.in
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)    12718 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/PKG-INFO
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     9418 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/README.rst
+drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/django_rest_models.egg-info/
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)    12718 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/django_rest_models.egg-info/PKG-INFO
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)      956 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/django_rest_models.egg-info/SOURCES.txt
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)        1 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/django_rest_models.egg-info/dependency_links.txt
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)        1 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/django_rest_models.egg-info/not-zip-safe
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)       34 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/django_rest_models.egg-info/requires.txt
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)       12 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/django_rest_models.egg-info/top_level.txt
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)      159 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/requirements.txt
+drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/rest_models/
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)      150 2024-05-16 15:50:08.000000 django-rest-models-2.1.3/rest_models/__init__.py
+drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/rest_models/backend/
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)        0 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/__init__.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     4055 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/auth.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3419 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/base.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     2266 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/client.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)    57952 2024-05-16 15:45:29.000000 django-rest-models-2.1.3/rest_models/backend/compiler.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)    16628 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/connexion.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3430 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/creation.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)      731 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/exceptions.py
+drwxr-xr-x   0 vakarys   (1000) vakarys   (1000)        0 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/rest_models/backend/exec/
+-rwxr-xr-x   0 vakarys   (1000) vakarys   (1000)     5851 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/exec/resty
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     1416 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/features.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3587 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/introspection.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3110 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/middlewares.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)      524 2024-05-16 15:49:42.000000 django-rest-models-2.1.3/rest_models/backend/operations.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)      690 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/backend/schema.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)      957 2024-05-16 15:49:44.000000 django-rest-models-2.1.3/rest_models/backend/utils.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     5464 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/checks.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     3794 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/router.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     4290 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/storage.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)    13847 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/test.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     6606 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/rest_models/utils.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)      284 2024-05-16 15:52:13.000000 django-rest-models-2.1.3/setup.cfg
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)     2156 2024-05-16 15:49:44.000000 django-rest-models-2.1.3/setup.py
+-rw-r--r--   0 vakarys   (1000) vakarys   (1000)       28 2023-08-07 09:04:00.000000 django-rest-models-2.1.3/test_requirements.txt
```

### Comparing `django-rest-models-2.1.2/CONTRIBUTING.rst` & `django-rest-models-2.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/PKG-INFO` & `django-rest-models-2.1.3/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: django-rest-models
-Version: 2.1.2
-Summary: django Fake ORM model that query an RestAPI instead of a database — 
-Home-page: https://github.com/Yupeek/django-rest-models
-Author: Darius BERNARD
-Author-email: darius@yupeek.com
-License: BSD
-Keywords: django rest models API ORM
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Utilities
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Description-Content-Type: text/x-rst
-License-File: LICENSE.md
-
 ==================
 django-rest-models
 ==================
 
 Allow to query a **django** RestAPI with same interface as the django ORM. **(the targeted API must use django-rest-framework + dynamic-rest libraries)**
 In fact, it works like any other database engine. You add the rest_models engine in an alternate database and the rest_models databe router.
 Then add APIMeta class to the models querying the API, voilà !
```

### Comparing `django-rest-models-2.1.2/README.rst` & `django-rest-models-2.1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,307 +1,329 @@
-==================
-django-rest-models
-==================
-
-Allow to query a **django** RestAPI with same interface as the django ORM. **(the targeted API must use django-rest-framework + dynamic-rest libraries)**
-In fact, it works like any other database engine. You add the rest_models engine in an alternate database and the rest_models databe router.
-Then add APIMeta class to the models querying the API, voilà !
-
-Stable branch
-
-.. image:: https://img.shields.io/travis/Yupeek/django-rest-models/master.svg
-    :target: https://travis-ci.org/Yupeek/django-rest-models
-
-.. image:: https://readthedocs.org/projects/django-rest-models/badge/?version=latest
-    :target: http://django-rest-models.readthedocs.org/en/latest/
-
-.. image:: https://coveralls.io/repos/github/Yupeek/django-rest-models/badge.svg?branch=master
-    :target: https://coveralls.io/github/Yupeek/django-rest-models?branch=master
-
-.. image:: https://img.shields.io/pypi/v/django-rest-models.svg
-    :target: https://pypi.python.org/pypi/django-rest-models
-    :alt: Latest PyPI version
-
-.. image:: https://requires.io/github/Yupeek/django-rest-models/requirements.svg?branch=master
-     :target: https://requires.io/github/Yupeek/django-rest-models/requirements/?branch=master
-     :alt: Requirements Status
-
-Development status
-
-.. image:: https://img.shields.io/travis/Yupeek/django-rest-models/develop.svg
-    :target: https://travis-ci.org/Yupeek/django-rest-models
-
-.. image:: https://coveralls.io/repos/github/Yupeek/django-rest-models/badge.svg?branch=develop
-    :target: https://coveralls.io/github/Yupeek/django-rest-models?branch=develop
-
-.. image:: https://requires.io/github/Yupeek/django-rest-models/requirements.svg?branch=develop
-     :target: https://requires.io/github/Yupeek/django-rest-models/requirements/?branch=develop
-     :alt: Requirements Status
-
-
-Installation
-------------
-
-1. Install using pip:
-
-   ``pip install django-rest-models``
-
-2. Alternatively, you can download or clone this repo and install with :
-
-    ``pip install -e .``.
-
-Requirements
-------------
-
-This database wrapper work with
-
-- python 3.6, 3.7
-- django 2.0, 2.1, 2.2, 3.0, 3.1, 3.2
-
-On the api, this is tested against
-
-- django-rest-framework 3.11, 3.12, 3.13
-- dynamic-rest 2.1
-
-
-Examples
---------
-
-settings.py:
-
-.. code-block:: python
-
-    DATABASES = {
-        'default': {
-            ...
-        },
-        'api': {
-            'ENGINE': 'rest_models.backend',
-            'NAME': 'https://requestb.in/',
-            'USER': 'userapi',
-            'PASSWORD': 'passwordapi',
-            'AUTH': 'rest_models.backend.auth.BasicAuth',
-        },
-    }
-
-    DATABASE_ROUTERS = [
-        'rest_models.router.RestModelRouter',
-    ]
-
-
-models.py:
-
-.. code-block:: python
-
-    class MyModel(models.Model):
-        field = models.IntegerField()
-        ...
-
-        class Meta:
-            # basic django meta Stuff
-            verbose_name = 'my model'
-
-        # the only customisation that make this model special
-        class APIMeta:
-            pass
-
-
-    class MyOtherModel(models.Model):
-        other_field = models.IntegerField()
-        first_model = models.ForeignKey(MyModel, db_column='mymodel')
-        ...
-
-        class Meta:
-            # basic django meta Stuff
-            verbose_name = 'my other model'
-
-        # the only customisation that make this model special
-        class APIMeta:
-            pass
-
-
-
-Targeted API requirements
--------------------------
-
-To allow this database adapter to work like a relational one, the targeted API must respect some requirements :
-
-- dynamic-rest installed and all serializers/views must respectively inherit from Dynamic* (DynamicModelSerializer, etc...)
-
-Each API serializer must :
-
-- Provide the id field
-- Provide the related field (ManyToMany and ForeignKey on Models) as DynamicRelationField
-- Provide the reverse related field. We must, for each ForeignKey and ManyToMany, add a field on the related model's
-  serializer.
-
-.. code-block:: python
-
-    class MenuSerializer(DynamicModelSerializer):
-        pizzas = DynamicRelationField('PizzaSerializer', many=True)     # Menu.pizza = ManyToMany
-
-        class Meta:
-            model = Menu
-            name = 'menu'
-            fields = ('id', 'code', 'name', 'pizzas')
-            deferred_fields = ('pizza_set', )
-
-
-    class PizzaSerializer(DynamicModelSerializer):
-
-        toppings = DynamicRelationField(ToppingSerializer, many=True)
-        menu = DynamicRelationField(MenuSerializer)                     # Add this because Menu.pizza = ManyToMany
-
-        class Meta:
-            model = Pizza
-            name = 'pizza'
-            fields = ('id', 'name', 'price', 'from_date', 'to_date', 'toppings', 'menu')
-
-django-rest-models provide a way to check the consistency of the api with the local models via the django check framework.
-At each startup, it will query the api with OPTIONS to check if the local models match the remote serializers.
-
-
-Caveats
--------
-
-Since this is not a real relational database, all feature cannot be implemented. Some limitations are inherited by
-dynamic-rest filtering system too.
-
-- Aggregations : is not implemented on the api endpoint, maybe in future releases
-- Complex filtering using OR : all filter passed to dynamic-rest is ANDed together, so no OR is possible
-- Negated AND in filtering: a negated AND give a OR, so previous limitation apply
-- Negated OR in filtering: since the compitation of nested filter is complexe and error prone, we disable all OR. in
-  fact, only some nested of AND is accepted. only the final value of the Q() object can be negated
-
-    for short, you **CANNOT** :
-
-.. code-block:: python
-
-
-        Pizza.objects.aggregate()
-        Pizza.objects.annotate()
-        Pizza.objects.filter(Q(..) | Q(..))
-        Pizza.objects.exclude(Q(..) & Q(..))
-        Pizza.objects.exclude(Q(..) | Q(..))
-
-    but you can :
-
-.. code-block:: python
-
-        Pizza.objects.create
-        Pizza.objects.bulk_create
-        Pizza.objects.update
-        Pizza.objects.bulk_update
-        Pizza.objects.select_related
-        Pizza.objects.prefetch_related
-        Pizza.objects.values
-        Pizza.objects.values_list
-        Pizza.objects.delete
-        Pizza.objects.count()
-        Pizza.objects.filter(..., ..., ...)
-        Pizza.objects.filter(...).filter(...).exclude(...)
-        Pizza.objects.exclude(..., ...).exclude(...)
-        Pizza.objects.filter(Q(..) & Q(..))
-        Pizza.objects.none()
-        pizza.toppings.add(...)
-        pizza.toppings.remove(...)
-        pizza.toppings.set(...)
-        pizza.toppings.clear(...)
-
-.. note::
-
-    prefetch_related work as expected, but the performance is readly bad. As a matter of fact, a ``Pizza.objects.prefetch_related('toppings')``
-    will query the toppings for all pizzas as expected, but the query to recover the pizza will contains the linked pizza in the response.
-    If the database contains a great number of pizzas for the given toppings, the response will contains them all, even if it's
-    useless at first glance, the linked pizza for each topping is mandotary to django to glue topping <=> pizza relationships.
-
-    So, be careful when using prefetch_related.
-
-
-
-Specific behaviour
----------------------
-
-Some specific behaviour has been implemented to use the extra feature of a Rest API :
-
-- When inserting, the resulting model is returned by the API. the inserted model is updated with the resulting values.
-  This imply 2 things:
-
-  * If you provided default values for fields in the api, these data will be populated into your created instance if it was ommited.
-  * If the serializer have some computed data, its data will always be used as a replacement of the one you gave to your
-    models. (cf example: Pizza.cost which is the sum of the cost of the toppling. after each save, its value will be updated)
-
-
-Support
--------
-
-This database api support :
-
-- select_related
-- order_by
-- only
-- defer
-- filter
-- exclude
-- delete
-- update
-- create
-- bulk create (with retrive of pk)
-- ManyToManyField
-- ForeignKey*
-
-.. note::
-
-    ForeignKey must have db_column fixed to the name of the reflected field in the api. or all update/create won't use
-    the value if this field
-
-.. note::
-
-		Support for ForeignKey is only available with models on the same database (api<->api) or (default<->default).
-		It's not possible to add a ForeignKey/ManyToMany field on a local model related to a remote model (with ApiMeta)
-
-Documentation
--------------
-
-The full documentation is at http://django-rest-models.readthedocs.org/en/latest/.
-
-
-Requirements
-------------
-
-- Python 2.7, 3.5
-- Django >= 1.8
-
-Contributions and pull requests are welcome.
-
-
-Bugs and requests
------------------
-
-If you found a bug or if you have a request for additional feature, please use the issue tracker on GitHub.
-
-https://github.com/Yupeek/django-rest-models/issues
-
-known limitations
------------------
-
-JSONField from postgresql and mysql is supported by django-rest-models, but not by the current dynamic-rest (1.8.1)
-so you can do `MyModel.objects.filter(myjson__mydata__contains='aaa')` but it will work if drest support it
-
-same for DateField's year,month,day lookup.
-
-License
--------
-
-You can use this under GPLv3.
-
-Author
-------
-
-Original author: `Darius BERNARD <https://github.com/ornoone>`_.
-Contributor: `PaulWay <https://github.com/PaulWay>`_.
-
-
-Thanks
-------
-
-Thanks to django for this amazing framework.
+Metadata-Version: 2.1
+Name: django-rest-models
+Version: 2.1.3
+Summary: django Fake ORM model that query an RestAPI instead of a database — 
+Home-page: https://github.com/Yupeek/django-rest-models
+Author: Darius BERNARD
+Author-email: darius@yupeek.com
+License: BSD
+Description: ==================
+        django-rest-models
+        ==================
+        
+        Allow to query a **django** RestAPI with same interface as the django ORM. **(the targeted API must use django-rest-framework + dynamic-rest libraries)**
+        In fact, it works like any other database engine. You add the rest_models engine in an alternate database and the rest_models databe router.
+        Then add APIMeta class to the models querying the API, voilà !
+        
+        Stable branch
+        
+        .. image:: https://img.shields.io/travis/Yupeek/django-rest-models/master.svg
+            :target: https://travis-ci.org/Yupeek/django-rest-models
+        
+        .. image:: https://readthedocs.org/projects/django-rest-models/badge/?version=latest
+            :target: http://django-rest-models.readthedocs.org/en/latest/
+        
+        .. image:: https://coveralls.io/repos/github/Yupeek/django-rest-models/badge.svg?branch=master
+            :target: https://coveralls.io/github/Yupeek/django-rest-models?branch=master
+        
+        .. image:: https://img.shields.io/pypi/v/django-rest-models.svg
+            :target: https://pypi.python.org/pypi/django-rest-models
+            :alt: Latest PyPI version
+        
+        .. image:: https://requires.io/github/Yupeek/django-rest-models/requirements.svg?branch=master
+             :target: https://requires.io/github/Yupeek/django-rest-models/requirements/?branch=master
+             :alt: Requirements Status
+        
+        Development status
+        
+        .. image:: https://img.shields.io/travis/Yupeek/django-rest-models/develop.svg
+            :target: https://travis-ci.org/Yupeek/django-rest-models
+        
+        .. image:: https://coveralls.io/repos/github/Yupeek/django-rest-models/badge.svg?branch=develop
+            :target: https://coveralls.io/github/Yupeek/django-rest-models?branch=develop
+        
+        .. image:: https://requires.io/github/Yupeek/django-rest-models/requirements.svg?branch=develop
+             :target: https://requires.io/github/Yupeek/django-rest-models/requirements/?branch=develop
+             :alt: Requirements Status
+        
+        
+        Installation
+        ------------
+        
+        1. Install using pip:
+        
+           ``pip install django-rest-models``
+        
+        2. Alternatively, you can download or clone this repo and install with :
+        
+            ``pip install -e .``.
+        
+        Requirements
+        ------------
+        
+        This database wrapper work with
+        
+        - python 3.6, 3.7
+        - django 2.0, 2.1, 2.2, 3.0, 3.1, 3.2
+        
+        On the api, this is tested against
+        
+        - django-rest-framework 3.11, 3.12, 3.13
+        - dynamic-rest 2.1
+        
+        
+        Examples
+        --------
+        
+        settings.py:
+        
+        .. code-block:: python
+        
+            DATABASES = {
+                'default': {
+                    ...
+                },
+                'api': {
+                    'ENGINE': 'rest_models.backend',
+                    'NAME': 'https://requestb.in/',
+                    'USER': 'userapi',
+                    'PASSWORD': 'passwordapi',
+                    'AUTH': 'rest_models.backend.auth.BasicAuth',
+                },
+            }
+        
+            DATABASE_ROUTERS = [
+                'rest_models.router.RestModelRouter',
+            ]
+        
+        
+        models.py:
+        
+        .. code-block:: python
+        
+            class MyModel(models.Model):
+                field = models.IntegerField()
+                ...
+        
+                class Meta:
+                    # basic django meta Stuff
+                    verbose_name = 'my model'
+        
+                # the only customisation that make this model special
+                class APIMeta:
+                    pass
+        
+        
+            class MyOtherModel(models.Model):
+                other_field = models.IntegerField()
+                first_model = models.ForeignKey(MyModel, db_column='mymodel')
+                ...
+        
+                class Meta:
+                    # basic django meta Stuff
+                    verbose_name = 'my other model'
+        
+                # the only customisation that make this model special
+                class APIMeta:
+                    pass
+        
+        
+        
+        Targeted API requirements
+        -------------------------
+        
+        To allow this database adapter to work like a relational one, the targeted API must respect some requirements :
+        
+        - dynamic-rest installed and all serializers/views must respectively inherit from Dynamic* (DynamicModelSerializer, etc...)
+        
+        Each API serializer must :
+        
+        - Provide the id field
+        - Provide the related field (ManyToMany and ForeignKey on Models) as DynamicRelationField
+        - Provide the reverse related field. We must, for each ForeignKey and ManyToMany, add a field on the related model's
+          serializer.
+        
+        .. code-block:: python
+        
+            class MenuSerializer(DynamicModelSerializer):
+                pizzas = DynamicRelationField('PizzaSerializer', many=True)     # Menu.pizza = ManyToMany
+        
+                class Meta:
+                    model = Menu
+                    name = 'menu'
+                    fields = ('id', 'code', 'name', 'pizzas')
+                    deferred_fields = ('pizza_set', )
+        
+        
+            class PizzaSerializer(DynamicModelSerializer):
+        
+                toppings = DynamicRelationField(ToppingSerializer, many=True)
+                menu = DynamicRelationField(MenuSerializer)                     # Add this because Menu.pizza = ManyToMany
+        
+                class Meta:
+                    model = Pizza
+                    name = 'pizza'
+                    fields = ('id', 'name', 'price', 'from_date', 'to_date', 'toppings', 'menu')
+        
+        django-rest-models provide a way to check the consistency of the api with the local models via the django check framework.
+        At each startup, it will query the api with OPTIONS to check if the local models match the remote serializers.
+        
+        
+        Caveats
+        -------
+        
+        Since this is not a real relational database, all feature cannot be implemented. Some limitations are inherited by
+        dynamic-rest filtering system too.
+        
+        - Aggregations : is not implemented on the api endpoint, maybe in future releases
+        - Complex filtering using OR : all filter passed to dynamic-rest is ANDed together, so no OR is possible
+        - Negated AND in filtering: a negated AND give a OR, so previous limitation apply
+        - Negated OR in filtering: since the compitation of nested filter is complexe and error prone, we disable all OR. in
+          fact, only some nested of AND is accepted. only the final value of the Q() object can be negated
+        
+            for short, you **CANNOT** :
+        
+        .. code-block:: python
+        
+        
+                Pizza.objects.aggregate()
+                Pizza.objects.annotate()
+                Pizza.objects.filter(Q(..) | Q(..))
+                Pizza.objects.exclude(Q(..) & Q(..))
+                Pizza.objects.exclude(Q(..) | Q(..))
+        
+            but you can :
+        
+        .. code-block:: python
+        
+                Pizza.objects.create
+                Pizza.objects.bulk_create
+                Pizza.objects.update
+                Pizza.objects.bulk_update
+                Pizza.objects.select_related
+                Pizza.objects.prefetch_related
+                Pizza.objects.values
+                Pizza.objects.values_list
+                Pizza.objects.delete
+                Pizza.objects.count()
+                Pizza.objects.filter(..., ..., ...)
+                Pizza.objects.filter(...).filter(...).exclude(...)
+                Pizza.objects.exclude(..., ...).exclude(...)
+                Pizza.objects.filter(Q(..) & Q(..))
+                Pizza.objects.none()
+                pizza.toppings.add(...)
+                pizza.toppings.remove(...)
+                pizza.toppings.set(...)
+                pizza.toppings.clear(...)
+        
+        .. note::
+        
+            prefetch_related work as expected, but the performance is readly bad. As a matter of fact, a ``Pizza.objects.prefetch_related('toppings')``
+            will query the toppings for all pizzas as expected, but the query to recover the pizza will contains the linked pizza in the response.
+            If the database contains a great number of pizzas for the given toppings, the response will contains them all, even if it's
+            useless at first glance, the linked pizza for each topping is mandotary to django to glue topping <=> pizza relationships.
+        
+            So, be careful when using prefetch_related.
+        
+        
+        
+        Specific behaviour
+        ---------------------
+        
+        Some specific behaviour has been implemented to use the extra feature of a Rest API :
+        
+        - When inserting, the resulting model is returned by the API. the inserted model is updated with the resulting values.
+          This imply 2 things:
+        
+          * If you provided default values for fields in the api, these data will be populated into your created instance if it was ommited.
+          * If the serializer have some computed data, its data will always be used as a replacement of the one you gave to your
+            models. (cf example: Pizza.cost which is the sum of the cost of the toppling. after each save, its value will be updated)
+        
+        
+        Support
+        -------
+        
+        This database api support :
+        
+        - select_related
+        - order_by
+        - only
+        - defer
+        - filter
+        - exclude
+        - delete
+        - update
+        - create
+        - bulk create (with retrive of pk)
+        - ManyToManyField
+        - ForeignKey*
+        
+        .. note::
+        
+            ForeignKey must have db_column fixed to the name of the reflected field in the api. or all update/create won't use
+            the value if this field
+        
+        .. note::
+        
+        		Support for ForeignKey is only available with models on the same database (api<->api) or (default<->default).
+        		It's not possible to add a ForeignKey/ManyToMany field on a local model related to a remote model (with ApiMeta)
+        
+        Documentation
+        -------------
+        
+        The full documentation is at http://django-rest-models.readthedocs.org/en/latest/.
+        
+        
+        Requirements
+        ------------
+        
+        - Python 2.7, 3.5
+        - Django >= 1.8
+        
+        Contributions and pull requests are welcome.
+        
+        
+        Bugs and requests
+        -----------------
+        
+        If you found a bug or if you have a request for additional feature, please use the issue tracker on GitHub.
+        
+        https://github.com/Yupeek/django-rest-models/issues
+        
+        known limitations
+        -----------------
+        
+        JSONField from postgresql and mysql is supported by django-rest-models, but not by the current dynamic-rest (1.8.1)
+        so you can do `MyModel.objects.filter(myjson__mydata__contains='aaa')` but it will work if drest support it
+        
+        same for DateField's year,month,day lookup.
+        
+        License
+        -------
+        
+        You can use this under GPLv3.
+        
+        Author
+        ------
+        
+        Original author: `Darius BERNARD <https://github.com/ornoone>`_.
+        Contributor: `PaulWay <https://github.com/PaulWay>`_.
+        
+        
+        Thanks
+        ------
+        
+        Thanks to django for this amazing framework.
+        
+Keywords: django rest models API ORM
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Utilities
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Description-Content-Type: text/x-rst
```

### Comparing `django-rest-models-2.1.2/django_rest_models.egg-info/PKG-INFO` & `django-rest-models-2.1.3/django_rest_models.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,329 +1,329 @@
 Metadata-Version: 2.1
 Name: django-rest-models
-Version: 2.1.2
+Version: 2.1.3
 Summary: django Fake ORM model that query an RestAPI instead of a database — 
 Home-page: https://github.com/Yupeek/django-rest-models
 Author: Darius BERNARD
 Author-email: darius@yupeek.com
 License: BSD
+Description: ==================
+        django-rest-models
+        ==================
+        
+        Allow to query a **django** RestAPI with same interface as the django ORM. **(the targeted API must use django-rest-framework + dynamic-rest libraries)**
+        In fact, it works like any other database engine. You add the rest_models engine in an alternate database and the rest_models databe router.
+        Then add APIMeta class to the models querying the API, voilà !
+        
+        Stable branch
+        
+        .. image:: https://img.shields.io/travis/Yupeek/django-rest-models/master.svg
+            :target: https://travis-ci.org/Yupeek/django-rest-models
+        
+        .. image:: https://readthedocs.org/projects/django-rest-models/badge/?version=latest
+            :target: http://django-rest-models.readthedocs.org/en/latest/
+        
+        .. image:: https://coveralls.io/repos/github/Yupeek/django-rest-models/badge.svg?branch=master
+            :target: https://coveralls.io/github/Yupeek/django-rest-models?branch=master
+        
+        .. image:: https://img.shields.io/pypi/v/django-rest-models.svg
+            :target: https://pypi.python.org/pypi/django-rest-models
+            :alt: Latest PyPI version
+        
+        .. image:: https://requires.io/github/Yupeek/django-rest-models/requirements.svg?branch=master
+             :target: https://requires.io/github/Yupeek/django-rest-models/requirements/?branch=master
+             :alt: Requirements Status
+        
+        Development status
+        
+        .. image:: https://img.shields.io/travis/Yupeek/django-rest-models/develop.svg
+            :target: https://travis-ci.org/Yupeek/django-rest-models
+        
+        .. image:: https://coveralls.io/repos/github/Yupeek/django-rest-models/badge.svg?branch=develop
+            :target: https://coveralls.io/github/Yupeek/django-rest-models?branch=develop
+        
+        .. image:: https://requires.io/github/Yupeek/django-rest-models/requirements.svg?branch=develop
+             :target: https://requires.io/github/Yupeek/django-rest-models/requirements/?branch=develop
+             :alt: Requirements Status
+        
+        
+        Installation
+        ------------
+        
+        1. Install using pip:
+        
+           ``pip install django-rest-models``
+        
+        2. Alternatively, you can download or clone this repo and install with :
+        
+            ``pip install -e .``.
+        
+        Requirements
+        ------------
+        
+        This database wrapper work with
+        
+        - python 3.6, 3.7
+        - django 2.0, 2.1, 2.2, 3.0, 3.1, 3.2
+        
+        On the api, this is tested against
+        
+        - django-rest-framework 3.11, 3.12, 3.13
+        - dynamic-rest 2.1
+        
+        
+        Examples
+        --------
+        
+        settings.py:
+        
+        .. code-block:: python
+        
+            DATABASES = {
+                'default': {
+                    ...
+                },
+                'api': {
+                    'ENGINE': 'rest_models.backend',
+                    'NAME': 'https://requestb.in/',
+                    'USER': 'userapi',
+                    'PASSWORD': 'passwordapi',
+                    'AUTH': 'rest_models.backend.auth.BasicAuth',
+                },
+            }
+        
+            DATABASE_ROUTERS = [
+                'rest_models.router.RestModelRouter',
+            ]
+        
+        
+        models.py:
+        
+        .. code-block:: python
+        
+            class MyModel(models.Model):
+                field = models.IntegerField()
+                ...
+        
+                class Meta:
+                    # basic django meta Stuff
+                    verbose_name = 'my model'
+        
+                # the only customisation that make this model special
+                class APIMeta:
+                    pass
+        
+        
+            class MyOtherModel(models.Model):
+                other_field = models.IntegerField()
+                first_model = models.ForeignKey(MyModel, db_column='mymodel')
+                ...
+        
+                class Meta:
+                    # basic django meta Stuff
+                    verbose_name = 'my other model'
+        
+                # the only customisation that make this model special
+                class APIMeta:
+                    pass
+        
+        
+        
+        Targeted API requirements
+        -------------------------
+        
+        To allow this database adapter to work like a relational one, the targeted API must respect some requirements :
+        
+        - dynamic-rest installed and all serializers/views must respectively inherit from Dynamic* (DynamicModelSerializer, etc...)
+        
+        Each API serializer must :
+        
+        - Provide the id field
+        - Provide the related field (ManyToMany and ForeignKey on Models) as DynamicRelationField
+        - Provide the reverse related field. We must, for each ForeignKey and ManyToMany, add a field on the related model's
+          serializer.
+        
+        .. code-block:: python
+        
+            class MenuSerializer(DynamicModelSerializer):
+                pizzas = DynamicRelationField('PizzaSerializer', many=True)     # Menu.pizza = ManyToMany
+        
+                class Meta:
+                    model = Menu
+                    name = 'menu'
+                    fields = ('id', 'code', 'name', 'pizzas')
+                    deferred_fields = ('pizza_set', )
+        
+        
+            class PizzaSerializer(DynamicModelSerializer):
+        
+                toppings = DynamicRelationField(ToppingSerializer, many=True)
+                menu = DynamicRelationField(MenuSerializer)                     # Add this because Menu.pizza = ManyToMany
+        
+                class Meta:
+                    model = Pizza
+                    name = 'pizza'
+                    fields = ('id', 'name', 'price', 'from_date', 'to_date', 'toppings', 'menu')
+        
+        django-rest-models provide a way to check the consistency of the api with the local models via the django check framework.
+        At each startup, it will query the api with OPTIONS to check if the local models match the remote serializers.
+        
+        
+        Caveats
+        -------
+        
+        Since this is not a real relational database, all feature cannot be implemented. Some limitations are inherited by
+        dynamic-rest filtering system too.
+        
+        - Aggregations : is not implemented on the api endpoint, maybe in future releases
+        - Complex filtering using OR : all filter passed to dynamic-rest is ANDed together, so no OR is possible
+        - Negated AND in filtering: a negated AND give a OR, so previous limitation apply
+        - Negated OR in filtering: since the compitation of nested filter is complexe and error prone, we disable all OR. in
+          fact, only some nested of AND is accepted. only the final value of the Q() object can be negated
+        
+            for short, you **CANNOT** :
+        
+        .. code-block:: python
+        
+        
+                Pizza.objects.aggregate()
+                Pizza.objects.annotate()
+                Pizza.objects.filter(Q(..) | Q(..))
+                Pizza.objects.exclude(Q(..) & Q(..))
+                Pizza.objects.exclude(Q(..) | Q(..))
+        
+            but you can :
+        
+        .. code-block:: python
+        
+                Pizza.objects.create
+                Pizza.objects.bulk_create
+                Pizza.objects.update
+                Pizza.objects.bulk_update
+                Pizza.objects.select_related
+                Pizza.objects.prefetch_related
+                Pizza.objects.values
+                Pizza.objects.values_list
+                Pizza.objects.delete
+                Pizza.objects.count()
+                Pizza.objects.filter(..., ..., ...)
+                Pizza.objects.filter(...).filter(...).exclude(...)
+                Pizza.objects.exclude(..., ...).exclude(...)
+                Pizza.objects.filter(Q(..) & Q(..))
+                Pizza.objects.none()
+                pizza.toppings.add(...)
+                pizza.toppings.remove(...)
+                pizza.toppings.set(...)
+                pizza.toppings.clear(...)
+        
+        .. note::
+        
+            prefetch_related work as expected, but the performance is readly bad. As a matter of fact, a ``Pizza.objects.prefetch_related('toppings')``
+            will query the toppings for all pizzas as expected, but the query to recover the pizza will contains the linked pizza in the response.
+            If the database contains a great number of pizzas for the given toppings, the response will contains them all, even if it's
+            useless at first glance, the linked pizza for each topping is mandotary to django to glue topping <=> pizza relationships.
+        
+            So, be careful when using prefetch_related.
+        
+        
+        
+        Specific behaviour
+        ---------------------
+        
+        Some specific behaviour has been implemented to use the extra feature of a Rest API :
+        
+        - When inserting, the resulting model is returned by the API. the inserted model is updated with the resulting values.
+          This imply 2 things:
+        
+          * If you provided default values for fields in the api, these data will be populated into your created instance if it was ommited.
+          * If the serializer have some computed data, its data will always be used as a replacement of the one you gave to your
+            models. (cf example: Pizza.cost which is the sum of the cost of the toppling. after each save, its value will be updated)
+        
+        
+        Support
+        -------
+        
+        This database api support :
+        
+        - select_related
+        - order_by
+        - only
+        - defer
+        - filter
+        - exclude
+        - delete
+        - update
+        - create
+        - bulk create (with retrive of pk)
+        - ManyToManyField
+        - ForeignKey*
+        
+        .. note::
+        
+            ForeignKey must have db_column fixed to the name of the reflected field in the api. or all update/create won't use
+            the value if this field
+        
+        .. note::
+        
+        		Support for ForeignKey is only available with models on the same database (api<->api) or (default<->default).
+        		It's not possible to add a ForeignKey/ManyToMany field on a local model related to a remote model (with ApiMeta)
+        
+        Documentation
+        -------------
+        
+        The full documentation is at http://django-rest-models.readthedocs.org/en/latest/.
+        
+        
+        Requirements
+        ------------
+        
+        - Python 2.7, 3.5
+        - Django >= 1.8
+        
+        Contributions and pull requests are welcome.
+        
+        
+        Bugs and requests
+        -----------------
+        
+        If you found a bug or if you have a request for additional feature, please use the issue tracker on GitHub.
+        
+        https://github.com/Yupeek/django-rest-models/issues
+        
+        known limitations
+        -----------------
+        
+        JSONField from postgresql and mysql is supported by django-rest-models, but not by the current dynamic-rest (1.8.1)
+        so you can do `MyModel.objects.filter(myjson__mydata__contains='aaa')` but it will work if drest support it
+        
+        same for DateField's year,month,day lookup.
+        
+        License
+        -------
+        
+        You can use this under GPLv3.
+        
+        Author
+        ------
+        
+        Original author: `Darius BERNARD <https://github.com/ornoone>`_.
+        Contributor: `PaulWay <https://github.com/PaulWay>`_.
+        
+        
+        Thanks
+        ------
+        
+        Thanks to django for this amazing framework.
+        
 Keywords: django rest models API ORM
+Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Description-Content-Type: text/x-rst
-License-File: LICENSE.md
-
-==================
-django-rest-models
-==================
-
-Allow to query a **django** RestAPI with same interface as the django ORM. **(the targeted API must use django-rest-framework + dynamic-rest libraries)**
-In fact, it works like any other database engine. You add the rest_models engine in an alternate database and the rest_models databe router.
-Then add APIMeta class to the models querying the API, voilà !
-
-Stable branch
-
-.. image:: https://img.shields.io/travis/Yupeek/django-rest-models/master.svg
-    :target: https://travis-ci.org/Yupeek/django-rest-models
-
-.. image:: https://readthedocs.org/projects/django-rest-models/badge/?version=latest
-    :target: http://django-rest-models.readthedocs.org/en/latest/
-
-.. image:: https://coveralls.io/repos/github/Yupeek/django-rest-models/badge.svg?branch=master
-    :target: https://coveralls.io/github/Yupeek/django-rest-models?branch=master
-
-.. image:: https://img.shields.io/pypi/v/django-rest-models.svg
-    :target: https://pypi.python.org/pypi/django-rest-models
-    :alt: Latest PyPI version
-
-.. image:: https://requires.io/github/Yupeek/django-rest-models/requirements.svg?branch=master
-     :target: https://requires.io/github/Yupeek/django-rest-models/requirements/?branch=master
-     :alt: Requirements Status
-
-Development status
-
-.. image:: https://img.shields.io/travis/Yupeek/django-rest-models/develop.svg
-    :target: https://travis-ci.org/Yupeek/django-rest-models
-
-.. image:: https://coveralls.io/repos/github/Yupeek/django-rest-models/badge.svg?branch=develop
-    :target: https://coveralls.io/github/Yupeek/django-rest-models?branch=develop
-
-.. image:: https://requires.io/github/Yupeek/django-rest-models/requirements.svg?branch=develop
-     :target: https://requires.io/github/Yupeek/django-rest-models/requirements/?branch=develop
-     :alt: Requirements Status
-
-
-Installation
-------------
-
-1. Install using pip:
-
-   ``pip install django-rest-models``
-
-2. Alternatively, you can download or clone this repo and install with :
-
-    ``pip install -e .``.
-
-Requirements
-------------
-
-This database wrapper work with
-
-- python 3.6, 3.7
-- django 2.0, 2.1, 2.2, 3.0, 3.1, 3.2
-
-On the api, this is tested against
-
-- django-rest-framework 3.11, 3.12, 3.13
-- dynamic-rest 2.1
-
-
-Examples
---------
-
-settings.py:
-
-.. code-block:: python
-
-    DATABASES = {
-        'default': {
-            ...
-        },
-        'api': {
-            'ENGINE': 'rest_models.backend',
-            'NAME': 'https://requestb.in/',
-            'USER': 'userapi',
-            'PASSWORD': 'passwordapi',
-            'AUTH': 'rest_models.backend.auth.BasicAuth',
-        },
-    }
-
-    DATABASE_ROUTERS = [
-        'rest_models.router.RestModelRouter',
-    ]
-
-
-models.py:
-
-.. code-block:: python
-
-    class MyModel(models.Model):
-        field = models.IntegerField()
-        ...
-
-        class Meta:
-            # basic django meta Stuff
-            verbose_name = 'my model'
-
-        # the only customisation that make this model special
-        class APIMeta:
-            pass
-
-
-    class MyOtherModel(models.Model):
-        other_field = models.IntegerField()
-        first_model = models.ForeignKey(MyModel, db_column='mymodel')
-        ...
-
-        class Meta:
-            # basic django meta Stuff
-            verbose_name = 'my other model'
-
-        # the only customisation that make this model special
-        class APIMeta:
-            pass
-
-
-
-Targeted API requirements
--------------------------
-
-To allow this database adapter to work like a relational one, the targeted API must respect some requirements :
-
-- dynamic-rest installed and all serializers/views must respectively inherit from Dynamic* (DynamicModelSerializer, etc...)
-
-Each API serializer must :
-
-- Provide the id field
-- Provide the related field (ManyToMany and ForeignKey on Models) as DynamicRelationField
-- Provide the reverse related field. We must, for each ForeignKey and ManyToMany, add a field on the related model's
-  serializer.
-
-.. code-block:: python
-
-    class MenuSerializer(DynamicModelSerializer):
-        pizzas = DynamicRelationField('PizzaSerializer', many=True)     # Menu.pizza = ManyToMany
-
-        class Meta:
-            model = Menu
-            name = 'menu'
-            fields = ('id', 'code', 'name', 'pizzas')
-            deferred_fields = ('pizza_set', )
-
-
-    class PizzaSerializer(DynamicModelSerializer):
-
-        toppings = DynamicRelationField(ToppingSerializer, many=True)
-        menu = DynamicRelationField(MenuSerializer)                     # Add this because Menu.pizza = ManyToMany
-
-        class Meta:
-            model = Pizza
-            name = 'pizza'
-            fields = ('id', 'name', 'price', 'from_date', 'to_date', 'toppings', 'menu')
-
-django-rest-models provide a way to check the consistency of the api with the local models via the django check framework.
-At each startup, it will query the api with OPTIONS to check if the local models match the remote serializers.
-
-
-Caveats
--------
-
-Since this is not a real relational database, all feature cannot be implemented. Some limitations are inherited by
-dynamic-rest filtering system too.
-
-- Aggregations : is not implemented on the api endpoint, maybe in future releases
-- Complex filtering using OR : all filter passed to dynamic-rest is ANDed together, so no OR is possible
-- Negated AND in filtering: a negated AND give a OR, so previous limitation apply
-- Negated OR in filtering: since the compitation of nested filter is complexe and error prone, we disable all OR. in
-  fact, only some nested of AND is accepted. only the final value of the Q() object can be negated
-
-    for short, you **CANNOT** :
-
-.. code-block:: python
-
-
-        Pizza.objects.aggregate()
-        Pizza.objects.annotate()
-        Pizza.objects.filter(Q(..) | Q(..))
-        Pizza.objects.exclude(Q(..) & Q(..))
-        Pizza.objects.exclude(Q(..) | Q(..))
-
-    but you can :
-
-.. code-block:: python
-
-        Pizza.objects.create
-        Pizza.objects.bulk_create
-        Pizza.objects.update
-        Pizza.objects.bulk_update
-        Pizza.objects.select_related
-        Pizza.objects.prefetch_related
-        Pizza.objects.values
-        Pizza.objects.values_list
-        Pizza.objects.delete
-        Pizza.objects.count()
-        Pizza.objects.filter(..., ..., ...)
-        Pizza.objects.filter(...).filter(...).exclude(...)
-        Pizza.objects.exclude(..., ...).exclude(...)
-        Pizza.objects.filter(Q(..) & Q(..))
-        Pizza.objects.none()
-        pizza.toppings.add(...)
-        pizza.toppings.remove(...)
-        pizza.toppings.set(...)
-        pizza.toppings.clear(...)
-
-.. note::
-
-    prefetch_related work as expected, but the performance is readly bad. As a matter of fact, a ``Pizza.objects.prefetch_related('toppings')``
-    will query the toppings for all pizzas as expected, but the query to recover the pizza will contains the linked pizza in the response.
-    If the database contains a great number of pizzas for the given toppings, the response will contains them all, even if it's
-    useless at first glance, the linked pizza for each topping is mandotary to django to glue topping <=> pizza relationships.
-
-    So, be careful when using prefetch_related.
-
-
-
-Specific behaviour
----------------------
-
-Some specific behaviour has been implemented to use the extra feature of a Rest API :
-
-- When inserting, the resulting model is returned by the API. the inserted model is updated with the resulting values.
-  This imply 2 things:
-
-  * If you provided default values for fields in the api, these data will be populated into your created instance if it was ommited.
-  * If the serializer have some computed data, its data will always be used as a replacement of the one you gave to your
-    models. (cf example: Pizza.cost which is the sum of the cost of the toppling. after each save, its value will be updated)
-
-
-Support
--------
-
-This database api support :
-
-- select_related
-- order_by
-- only
-- defer
-- filter
-- exclude
-- delete
-- update
-- create
-- bulk create (with retrive of pk)
-- ManyToManyField
-- ForeignKey*
-
-.. note::
-
-    ForeignKey must have db_column fixed to the name of the reflected field in the api. or all update/create won't use
-    the value if this field
-
-.. note::
-
-		Support for ForeignKey is only available with models on the same database (api<->api) or (default<->default).
-		It's not possible to add a ForeignKey/ManyToMany field on a local model related to a remote model (with ApiMeta)
-
-Documentation
--------------
-
-The full documentation is at http://django-rest-models.readthedocs.org/en/latest/.
-
-
-Requirements
-------------
-
-- Python 2.7, 3.5
-- Django >= 1.8
-
-Contributions and pull requests are welcome.
-
-
-Bugs and requests
------------------
-
-If you found a bug or if you have a request for additional feature, please use the issue tracker on GitHub.
-
-https://github.com/Yupeek/django-rest-models/issues
-
-known limitations
------------------
-
-JSONField from postgresql and mysql is supported by django-rest-models, but not by the current dynamic-rest (1.8.1)
-so you can do `MyModel.objects.filter(myjson__mydata__contains='aaa')` but it will work if drest support it
-
-same for DateField's year,month,day lookup.
-
-License
--------
-
-You can use this under GPLv3.
-
-Author
-------
-
-Original author: `Darius BERNARD <https://github.com/ornoone>`_.
-Contributor: `PaulWay <https://github.com/PaulWay>`_.
-
-
-Thanks
-------
-
-Thanks to django for this amazing framework.
```

### Comparing `django-rest-models-2.1.2/django_rest_models.egg-info/SOURCES.txt` & `django-rest-models-2.1.3/django_rest_models.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 CONTRIBUTING.rst
-LICENSE.md
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 test_requirements.txt
 django_rest_models.egg-info/PKG-INFO
```

### Comparing `django-rest-models-2.1.2/rest_models/backend/auth.py` & `django-rest-models-2.1.3/rest_models/backend/auth.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/base.py` & `django-rest-models-2.1.3/rest_models/backend/base.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/client.py` & `django-rest-models-2.1.3/rest_models/backend/client.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/compiler.py` & `django-rest-models-2.1.3/rest_models/backend/compiler.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/connexion.py` & `django-rest-models-2.1.3/rest_models/backend/connexion.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/creation.py` & `django-rest-models-2.1.3/rest_models/backend/creation.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/exceptions.py` & `django-rest-models-2.1.3/rest_models/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/exec/resty` & `django-rest-models-2.1.3/rest_models/backend/exec/resty`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/features.py` & `django-rest-models-2.1.3/rest_models/backend/features.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/introspection.py` & `django-rest-models-2.1.3/rest_models/backend/introspection.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/middlewares.py` & `django-rest-models-2.1.3/rest_models/backend/middlewares.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/operations.py` & `django-rest-models-2.1.3/rest_models/backend/operations.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/schema.py` & `django-rest-models-2.1.3/rest_models/backend/schema.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/backend/utils.py` & `django-rest-models-2.1.3/rest_models/backend/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,10 +21,17 @@
     except ImportError:
         pass
 
 try:
     class JSONField(JSONFieldLegacy):
         def get_prep_value(self, value):
             return value
+
+        def from_db_value(self, value, expression, connection):
+            try:
+                return super().from_db_value(value, expression, connection)
+            except TypeError:
+                return value
+
 except NameError:
     def JSONField(*args, **kwargs):
         return None
```

### Comparing `django-rest-models-2.1.2/rest_models/checks.py` & `django-rest-models-2.1.3/rest_models/checks.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/router.py` & `django-rest-models-2.1.3/rest_models/router.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/storage.py` & `django-rest-models-2.1.3/rest_models/storage.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/test.py` & `django-rest-models-2.1.3/rest_models/test.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/rest_models/utils.py` & `django-rest-models-2.1.3/rest_models/utils.py`

 * *Files identical despite different names*

### Comparing `django-rest-models-2.1.2/setup.py` & `django-rest-models-2.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import os
 import sys
 
 import rest_models
 
 try:
```

