# Comparing `tmp/django_pint_field-0.3.4.tar.gz` & `tmp/django_pint_field-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pint_field-0.3.4.tar", max compression
+gzip compressed data, was "django_pint_field-0.3.5.tar", max compression
```

## Comparing `django_pint_field-0.3.4.tar` & `django_pint_field-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1067 2022-12-28 23:26:58.079295 django_pint_field-0.3.4/LICENSE
--rw-r--r--   0        0        0     8834 2023-01-13 02:55:24.916452 django_pint_field-0.3.4/README.md
--rw-r--r--   0        0        0       41 2023-01-13 02:48:29.461518 django_pint_field-0.3.4/django_pint_field/__init__.py
--rw-r--r--   0        0        0     2312 2023-01-03 21:02:41.490062 django_pint_field-0.3.4/django_pint_field/aggregates.py
--rw-r--r--   0        0        0     1335 2023-01-13 02:47:54.746470 django_pint_field-0.3.4/django_pint_field/apps.py
--rw-r--r--   0        0        0      167 2023-01-01 22:00:09.966661 django_pint_field-0.3.4/django_pint_field/exceptions.py
--rw-r--r--   0        0        0    12548 2023-01-18 03:47:38.051757 django_pint_field-0.3.4/django_pint_field/forms.py
--rw-r--r--   0        0        0     2415 2023-01-13 02:47:54.754469 django_pint_field-0.3.4/django_pint_field/helper.py
--rw-r--r--   0        0        0     8061 2023-01-09 04:00:18.586014 django_pint_field-0.3.4/django_pint_field/lookups.py
--rw-r--r--   0        0        0     2306 2023-01-03 21:03:05.537351 django_pint_field-0.3.4/django_pint_field/migrations/0001_create_composite_fields.py
--rw-r--r--   0        0        0        0 2022-12-29 00:16:43.308055 django_pint_field-0.3.4/django_pint_field/migrations/__init__.py
--rw-r--r--   0        0        0    27100 2023-01-18 03:44:54.764318 django_pint_field-0.3.4/django_pint_field/models.py
--rw-r--r--   0        0        0     2538 2023-01-18 02:03:04.240582 django_pint_field-0.3.4/django_pint_field/rest.py
--rw-r--r--   0        0        0      340 2023-01-13 02:42:17.255746 django_pint_field-0.3.4/django_pint_field/settings.py
--rw-r--r--   0        0        0      159 2023-01-02 17:56:02.700780 django_pint_field-0.3.4/django_pint_field/units.py
--rw-r--r--   0        0        0     1002 2023-01-18 03:46:56.535899 django_pint_field-0.3.4/django_pint_field/widgets.py
--rw-r--r--   0        0        0     1393 2023-01-18 03:48:06.691659 django_pint_field-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     9936 1970-01-01 00:00:00.000000 django_pint_field-0.3.4/setup.py
--rw-r--r--   0        0        0    10047 1970-01-01 00:00:00.000000 django_pint_field-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2022-12-28 23:26:58.079295 django_pint_field-0.3.5/LICENSE
+-rw-r--r--   0        0        0    10291 2023-01-28 21:11:00.622924 django_pint_field-0.3.5/README.md
+-rw-r--r--   0        0        0       41 2023-01-13 02:48:29.461518 django_pint_field-0.3.5/django_pint_field/__init__.py
+-rw-r--r--   0        0        0     2312 2023-01-03 21:02:41.490062 django_pint_field-0.3.5/django_pint_field/aggregates.py
+-rw-r--r--   0        0        0     1335 2023-01-13 02:47:54.746470 django_pint_field-0.3.5/django_pint_field/apps.py
+-rw-r--r--   0        0        0      167 2023-01-01 22:00:09.966661 django_pint_field-0.3.5/django_pint_field/exceptions.py
+-rw-r--r--   0        0        0    11488 2023-01-28 20:18:21.183658 django_pint_field-0.3.5/django_pint_field/forms.py
+-rw-r--r--   0        0        0     2415 2023-01-13 02:47:54.754469 django_pint_field-0.3.5/django_pint_field/helper.py
+-rw-r--r--   0        0        0     8061 2023-01-09 04:00:18.586014 django_pint_field-0.3.5/django_pint_field/lookups.py
+-rw-r--r--   0        0        0     2306 2023-01-03 21:03:05.537351 django_pint_field-0.3.5/django_pint_field/migrations/0001_create_composite_fields.py
+-rw-r--r--   0        0        0        0 2022-12-29 00:16:43.308055 django_pint_field-0.3.5/django_pint_field/migrations/__init__.py
+-rw-r--r--   0        0        0    27100 2023-01-28 20:45:04.353291 django_pint_field-0.3.5/django_pint_field/models.py
+-rw-r--r--   0        0        0     2538 2023-01-18 02:03:04.240582 django_pint_field-0.3.5/django_pint_field/rest.py
+-rw-r--r--   0        0        0      340 2023-01-13 02:42:17.255746 django_pint_field-0.3.5/django_pint_field/settings.py
+-rw-r--r--   0        0        0      574 2023-01-28 20:27:12.246678 django_pint_field-0.3.5/django_pint_field/templates/tabled_django_pint_field_widget.html
+-rw-r--r--   0        0        0      159 2023-01-02 17:56:02.700780 django_pint_field-0.3.5/django_pint_field/units.py
+-rw-r--r--   0        0        0     2490 2023-01-28 20:46:57.815414 django_pint_field-0.3.5/django_pint_field/widgets.py
+-rw-r--r--   0        0        0     1393 2023-01-28 21:13:25.471006 django_pint_field-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    11473 1970-01-01 00:00:00.000000 django_pint_field-0.3.5/setup.py
+-rw-r--r--   0        0        0    11504 1970-01-01 00:00:00.000000 django_pint_field-0.3.5/PKG-INFO
```

### Comparing `django_pint_field-0.3.4/LICENSE` & `django_pint_field-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pint_field-0.3.4/README.md` & `django_pint_field-0.3.5/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+
 # django-pint-field
 
 Use [pint](https://pint.readthedocs.io/en/stable/) with Django's ORM.
 
 If you want to store quantities (1 gram, 3 miles, 8.120391 angstroms, etc) in a model, edit them in forms, and have the ability to convert to other quantities in your django projects, this is the package for you!
 
 This package is modified from the fantastic [django-pint](https://github.com/CarliJoy/django-pint) with different goals. Unlike django-pint, in this project we use a composite Postgres field to store both the magnitude and the user's desired units, along with the equivalent value in base units. This third piece of date - the base units - makes it possible to conduct lookups comparing one instance that might be specified in "grams" with another that may be specified in "pounds", but display each instance in the units that the user desires. The units your users want to use are the units they see, while still allowing accurate comparisons of one quantity to another.
@@ -187,15 +188,56 @@
 - **IntegerPintFormField**: Used in forms with IntegerPintField and BigIntegerPintField.
 - **DecimalPintFormField**: Used in forms with DecimalPintField.
 
 
 ## Widgets
 
 - **PintFieldWidget**: Default widget for all django pint field types.
+- **TabledPintFieldWidget**: Provides a table showing conversion to each of the `unit_choices`.
+
+![TabledPintFieldWidget](https://raw.githubusercontent.com/jacklinke/django-pint-field/main/media/TabledPintFieldWidget.png)
+
+
+Example usage:
+
+```python
+class WeightModel(models.Model):
+    decimal_weight = DecimalPintField(
+        "gram",
+        blank=True,
+        null=True,
+        max_digits=10,
+        decimal_places=2,
+        unit_choices=[
+            "kilogram",
+            "milligram",
+            "pounds"
+        ],
+    )
+
+class TabledWeightForm(forms.ModelForm):
+    class Meta:
+        model = WeightModel
+        fields = "__all__"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # If we want to use the tabled widget, we need to pass the 
+        #   default_unit and unit_choices to the new widget
+        default_unit = self.fields["decimal_weight"].default_unit
+        unit_choices = self.fields["decimal_weight"].unit_choices
+        self.fields["decimal_weight"].widget = TabledPintFieldWidget(
+            default_unit=default_unit, unit_choices=unit_choices
+        )
+```
+
+The template for this widget is located at https://github.com/jacklinke/django-pint-field/blob/main/django_pint_field/templates/tabled_django_pint_field_widget.html
 
+If you want to override the template, add your own template in your project at: "templates/django_pint_field/tabled_django_pint_field_widget.html"
 
 ## DRF Serializer Fields
 
 - **IntegerPintRestField**: Used in DRF with IntegerPintField and BigIntegerPintField.
 - **DecimalPintRestField**: Used in DRF with DecimalPintField.
```

### Comparing `django_pint_field-0.3.4/django_pint_field/aggregates.py` & `django_pint_field-0.3.5/django_pint_field/aggregates.py`

 * *Files identical despite different names*

### Comparing `django_pint_field-0.3.4/django_pint_field/apps.py` & `django_pint_field-0.3.5/django_pint_field/apps.py`

 * *Files identical despite different names*

### Comparing `django_pint_field-0.3.4/django_pint_field/forms.py` & `django_pint_field-0.3.5/django_pint_field/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         if not isinstance(value, (list, tuple)):
             raise ValidationError(
                 _("Value type %(value)s is invalid"),
                 code="invalid_list",
                 params={"value": type(value)},
             )
 
-        if not self.required:
+        if not self.required and value[0] == "":
             return value
 
         if not value[0] or not value[1]:
             raise ValidationError(
                 _("Value (%(value)s) cannot be NoneType"),
                 code="value_is_nonetype",
                 params={"value": type(value)},
@@ -202,40 +202,16 @@
             raise ValueError("PintFormField requires a default_unit kwarg of a single unit type (eg: 'grams')")
         self.unit_choices = kwargs.pop("unit_choices", [self.default_unit])
         if self.default_unit not in self.unit_choices:
             self.unit_choices.append(self.default_unit)
 
         check_matching_unit_dimension(self.ureg, self.default_unit, self.unit_choices)
 
-        def is_special_admin_widget(widget) -> bool:
-            """
-            There are some special django admin widgets, defined
-            in django/contrib/admin/options.py in the variable
-            FORMFIELD_FOR_DBFIELD_DEFAULTS
-            The intention for Decimal and BigDecimalField is only to
-            define the width.
-
-            They are set through a complicated process of the
-            modelform_factory setting formfield_callback to
-            ModelForm.formfield_to_dbfield
-
-            As they will overwrite our Widget we check for them and
-            will ignore them, if they are set as attribute.
-
-            We still will allow subclasses, so the end user has still
-            the possibility to use this widget.
-            """
-            WIDGETS_TO_IGNORE = [
-                FORMFIELD_FOR_DBFIELD_DEFAULTS[models.DecimalField],
-            ]
-            classes_to_ignore = [ignored_widget["widget"].__name__ for ignored_widget in WIDGETS_TO_IGNORE]
-            return getattr(widget, "__name__") in classes_to_ignore
-
         widget = kwargs.get("widget", None)
-        if widget is None or is_special_admin_widget(widget):
+        if widget is None:
             widget = PintFieldWidget(default_unit=self.default_unit, unit_choices=self.unit_choices)
         kwargs["widget"] = widget
         super().__init__(*args, **kwargs)
 
     def prepare_value(self, value):
         if isinstance(value, Quantity):
             # quantize the decimal value so we can validate is is no longer than max_digits after quantization
@@ -259,15 +235,15 @@
         if not isinstance(value, (list, tuple)):
             raise ValidationError(
                 _("Value type %(value)s is invalid"),
                 code="invalid_list",
                 params={"value": type(value)},
             )
 
-        if not self.required:
+        if not self.required and value[0] == "":
             return value
 
         if not value[0] or not value[1]:
             raise ValidationError(
                 _("Value (%(value)s) cannot be NoneType"),
                 code="value_is_nonetype",
                 params={"value": type(value)},
```

### Comparing `django_pint_field-0.3.4/django_pint_field/helper.py` & `django_pint_field-0.3.5/django_pint_field/helper.py`

 * *Files identical despite different names*

### Comparing `django_pint_field-0.3.4/django_pint_field/lookups.py` & `django_pint_field-0.3.5/django_pint_field/lookups.py`

 * *Files identical despite different names*

### Comparing `django_pint_field-0.3.4/django_pint_field/migrations/0001_create_composite_fields.py` & `django_pint_field-0.3.5/django_pint_field/migrations/0001_create_composite_fields.py`

 * *Files identical despite different names*

### Comparing `django_pint_field-0.3.4/django_pint_field/models.py` & `django_pint_field-0.3.5/django_pint_field/models.py`

 * *Files identical despite different names*

### Comparing `django_pint_field-0.3.4/django_pint_field/rest.py` & `django_pint_field-0.3.5/django_pint_field/rest.py`

 * *Files identical despite different names*

### Comparing `django_pint_field-0.3.4/pyproject.toml` & `django_pint_field-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-pint-field"
-version = "0.3.4"
+version = "0.3.5"
 description = "Pint Fields for Django and Postgres"
 authors = ["Jack Linke <jack@watervize.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "django_pint_field"}]
 
 homepage = "https://github.com/jacklinke/django-pint-field"
```

### Comparing `django_pint_field-0.3.4/setup.py` & `django_pint_field-0.3.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['django_pint_field', 'django_pint_field.migrations']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'django_pint_field': ['templates/*']}
 
 install_requires = \
 ['django>=3.2', 'pint>=0.19', 'psycopg2-binary>=2.9,<3.0']
 
 setup_kwargs = {
     'name': 'django-pint-field',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'Pint Fields for Django and Postgres',
-    'long_description': '# django-pint-field\n\nUse [pint](https://pint.readthedocs.io/en/stable/) with Django\'s ORM.\n\nIf you want to store quantities (1 gram, 3 miles, 8.120391 angstroms, etc) in a model, edit them in forms, and have the ability to convert to other quantities in your django projects, this is the package for you!\n\nThis package is modified from the fantastic [django-pint](https://github.com/CarliJoy/django-pint) with different goals. Unlike django-pint, in this project we use a composite Postgres field to store both the magnitude and the user\'s desired units, along with the equivalent value in base units. This third piece of date - the base units - makes it possible to conduct lookups comparing one instance that might be specified in "grams" with another that may be specified in "pounds", but display each instance in the units that the user desires. The units your users want to use are the units they see, while still allowing accurate comparisons of one quantity to another.\n\nFor this reason, the project only works with Postgresql databases.\n\n\n## Install\n\n`pip install django_pint_field`\n\nAdd `"django_pint_field",` to your list of installed apps.\n\nRun `python manage.py migrate django_pint_field`\n\n\n## Usage\n\nAssuming we are starting with the following model:\n\n```python\nfrom decimal import Decimal\nfrom django.db import models\nfrom django.db.models import DecimalField\n\nfrom django_pint_field.models import IntegerPintField\n\n\nclass IntegerPintFieldSaveModel(models.Model):\n    name = models.CharField(max_length=20)\n    weight = IntegerPintField("gram")\n\n    def __str__(self):\n        return str(self.name)\n```\n\nWe can do the following:\n\n```python\nfrom decimal import Decimal\nfrom django_pint_field.units import ureg\n\nfrom .models import IntegerPintFieldSaveModel\n\nQuantity = ureg.Quantity\n\n# Start by creating a few Pint Quantity objects\nextra_small = Quantity(1 * ureg.gram)\nsmall = Quantity(10 * ureg.gram)\nmedium = Quantity(100 * ureg.gram)\nlarge = Quantity(1000 * ureg.gram)\nextra_large = Quantity(10000 * ureg.gram)\n\n# Create a couple objects\nIntegerPintFieldSaveModel.objects.create(name="small", weight=small)\nIntegerPintFieldSaveModel.objects.create(name="large", weight=large)\n\nIn [1]: IntegerPintFieldSaveModel.objects.first()\nOut[1]: <IntegerPintFieldSaveModel: small>\n\nIn [2]: IntegerPintFieldSaveModel.objects.first().weight\nOut[2]: 10 <Unit(\'gram\')>\n\nIn [3]: IntegerPintFieldSaveModel.objects.first().weight.magnitude\nOut[3]: 10\n\nIn [4]: IntegerPintFieldSaveModel.objects.first().weight.units\nOut[4]: <Unit(\'gram\')>\n```\n\n\n## Valid Lookups\n\nOther lookups will be added in the future. Currently available are:\n\n- exact\n- gt\n- gte\n- lt\n- lte\n- range\n- isnull\n\n```python\n# Perform some queries\nIntegerPintFieldSaveModel.objects.filter(weight__gt=medium)\n<QuerySet [<IntegerPintFieldSaveModel: large>]>\n\nIntegerPintFieldSaveModel.objects.filter(weight__gt=extra_small)\n<QuerySet [<IntegerPintFieldSaveModel: small>, <IntegerPintFieldSaveModel: large>]>\n\nIntegerPintFieldSaveModel.objects.filter(weight__gte=small)\n<QuerySet [<IntegerPintFieldSaveModel: small>, <IntegerPintFieldSaveModel: large>]>\n\nIntegerPintFieldSaveModel.objects.filter(weight__range=(small, medium))\n<QuerySet [<IntegerPintFieldSaveModel: small>]>\n```\n\n\n## Aggregates\n\nA number of aggregates have been implemented for the Django Pint Fields. Functionally they perform for Pint Fields the same way django\'s default aggregates work for other field types, and each is prepended with "Pint". The aggregates include:\n\n- PintAvg\n- PintCount\n- PintMax\n- PintMin\n- PintStdDev\n- PintSum\n- PintVariance\n\n```python\nfrom django_pint_field.aggregates import PintAvg, PintCount, PintMax, PintMin, PintStdDev, PintSum, PintVariance\n\n# Perform some queries\nIntegerPintFieldSaveModel.objects.aggregate(PintAvg(\'weight\'))\n{\'weight__pintavg\': Decimal(\'0.50500000000000000000\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintCount(\'weight\'))\n{\'weight__pintcount\': 2}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintMax(\'weight\'))\n{\'weight__pintmax\': Decimal(\'1.0\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintMin(\'weight\'))\n{\'weight__pintmin\': Decimal(\'0.01\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintStdDev(\'weight\'))\n{\'weight__pintstddev\': Decimal(\'0.49500000000000000000\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintSum(\'weight\'))\n{\'weight__pintsum\': Decimal(\'1.01\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintVariance(\'weight\'))\n{\'weight__pintvariance\': Decimal(\'0.24502500000000000000\') <Unit(\'kilogram\')>}\n```\n\n\n## Use with Django Rest Framework\n\n\n```python\nfrom django_pint_field.rest import IntegerPintRestField\n\nclass DjangoPintFieldSerializer(serializers.ModelSerializer):\n    # Let DRF know which type of serializer field to use\n    weight = IntegerPintRestField()\n\n    class Meta:\n        model = IntegerPintFieldSaveModel\n        fields = ["name", "weight"]\n```\n\n\n## Creating your own units\n\nYou can [create your own pint units](https://pint.readthedocs.io/en/stable/advanced/defining.html) if the [default units](https://github.com/hgrecco/pint/blob/master/pint/default_en.txt) in pint are not sufficient.\n\nAnywhere within your project (ideally in settings or a file adjacent to settings), define the custom unit registry by importing Pint\'s default UnitRegistry and extending it:\n\n```python\nfrom pint import UnitRegistry\n\ncustom_ureg = UnitRegistry()\ncustom_ureg.define("custom = [custom]")\ncustom_ureg.define("kilocustom = 1000 * custom")\n```\n\nThen add the custom registry to your app\'s settings.py:\n\n`DJANGO_PINT_FIELD_UNIT_REGISTER = custom_ureg`\n\n\n## Model Fields\n\n- **IntegerPintField**: Stores a pint measurement as an integer (-2147483648 to 2147483647).\n- **BigIntegerPintField**: Stores a pint measurement as a big integer (-9223372036854775808 to 9223372036854775807).\n- **DecimalPintField**: Stores a pint measurement as a decimal. Like Django\'s DecimalField, DecimalPintField takes required `max_digits` and `decimal_places` parameters.\n\n\n## Form Fields\n\n- **IntegerPintFormField**: Used in forms with IntegerPintField and BigIntegerPintField.\n- **DecimalPintFormField**: Used in forms with DecimalPintField.\n\n\n## Widgets\n\n- **PintFieldWidget**: Default widget for all django pint field types.\n\n\n## DRF Serializer Fields\n\n- **IntegerPintRestField**: Used in DRF with IntegerPintField and BigIntegerPintField.\n- **DecimalPintRestField**: Used in DRF with DecimalPintField.\n\n\n## Settings\n\n<dl>\n  <dt><code>DJANGO_PINT_FIELD_DECIMAL_PRECISION</code></dt>\n  <dd>\n    Determines whether django_pint_field should automatically set the python decimal precision for the project. If an integer greater than 0 is provided, the decimal context precision for the entire project will be set to that value. Otherwise, the precision remains at the default (usually 28).<br>\n    <em>* Type: int</em>\n    <em>* Default: 0</em>\n  </dd>\n\n  <dt><code>DJANGO_PINT_FIELD_UNIT_REGISTER</code></dt>\n  <dd>\n    The Unit Registry to use in the project. Defaults to pint.UnitRegistry.<br>\n    <em>* Type: int</em>\n    <em>* Default: 0</em>\n  </dd>\n</dl>\n\n\n## Rounding modes (upcoming feature)\n\n**decimal.ROUND_CEILING**\nRound towards Infinity.\n\n**decimal.ROUND_DOWN**\nRound towards zero.\n\n**decimal.ROUND_FLOOR**\nRound towards -Infinity.\n\n**decimal.ROUND_HALF_DOWN**\nRound to nearest with ties going towards zero.\n\n**decimal.ROUND_HALF_EVEN**\nRound to nearest with ties going to nearest even integer.\n\n**decimal.ROUND_HALF_UP**\nRound to nearest with ties going away from zero.\n\n**decimal.ROUND_UP**\nRound away from zero.\n\n**decimal.ROUND_05UP**\nRound away from zero if last digit after rounding towards zero would have been 0 or 5; otherwise round towards zero.\n\nRead more about rounding modes for decimals at the [decimal docs](https://docs.python.org/3/library/decimal.html#rounding-modes)\n\n\n## Use the test app with docker compose\n\n### Set up a virtual environment (recommended)\n\nMake a virtual environment named `.venv`:\n\n`python3 -m venv .venv`\n    \nActivate the new environment:\n\n`source .venv/bin/activate`\n\n\n### Install dependencies\n\n*Requires [poetry](https://python-poetry.org/). If you do not yet have it installed, run `pip install poetry`.*\n\n`poetry install --with dev`\n\n### Build and bring up\n\n```\ndocker compose build\ndocker compose run django python manage.py migrate\ndocker compose run django python manage.py createsuperuser\ndocker compose up -d\n```\n\nNavigate to `127.0.0.1:8000`\n\n### Test (assuming you have already performed `build`)\n\n`docker compose run django python manage.py test`\n\n\n## Run psql on the Postgres database\n\n`docker compose exec postgres psql -U postgres`\n\n\n## ToDos:\n- Implement rounding modes\n- Think through what it would take to build range types for these fields\n- Add extensible widget template\n',
+    'long_description': '\n# django-pint-field\n\nUse [pint](https://pint.readthedocs.io/en/stable/) with Django\'s ORM.\n\nIf you want to store quantities (1 gram, 3 miles, 8.120391 angstroms, etc) in a model, edit them in forms, and have the ability to convert to other quantities in your django projects, this is the package for you!\n\nThis package is modified from the fantastic [django-pint](https://github.com/CarliJoy/django-pint) with different goals. Unlike django-pint, in this project we use a composite Postgres field to store both the magnitude and the user\'s desired units, along with the equivalent value in base units. This third piece of date - the base units - makes it possible to conduct lookups comparing one instance that might be specified in "grams" with another that may be specified in "pounds", but display each instance in the units that the user desires. The units your users want to use are the units they see, while still allowing accurate comparisons of one quantity to another.\n\nFor this reason, the project only works with Postgresql databases.\n\n\n## Install\n\n`pip install django_pint_field`\n\nAdd `"django_pint_field",` to your list of installed apps.\n\nRun `python manage.py migrate django_pint_field`\n\n\n## Usage\n\nAssuming we are starting with the following model:\n\n```python\nfrom decimal import Decimal\nfrom django.db import models\nfrom django.db.models import DecimalField\n\nfrom django_pint_field.models import IntegerPintField\n\n\nclass IntegerPintFieldSaveModel(models.Model):\n    name = models.CharField(max_length=20)\n    weight = IntegerPintField("gram")\n\n    def __str__(self):\n        return str(self.name)\n```\n\nWe can do the following:\n\n```python\nfrom decimal import Decimal\nfrom django_pint_field.units import ureg\n\nfrom .models import IntegerPintFieldSaveModel\n\nQuantity = ureg.Quantity\n\n# Start by creating a few Pint Quantity objects\nextra_small = Quantity(1 * ureg.gram)\nsmall = Quantity(10 * ureg.gram)\nmedium = Quantity(100 * ureg.gram)\nlarge = Quantity(1000 * ureg.gram)\nextra_large = Quantity(10000 * ureg.gram)\n\n# Create a couple objects\nIntegerPintFieldSaveModel.objects.create(name="small", weight=small)\nIntegerPintFieldSaveModel.objects.create(name="large", weight=large)\n\nIn [1]: IntegerPintFieldSaveModel.objects.first()\nOut[1]: <IntegerPintFieldSaveModel: small>\n\nIn [2]: IntegerPintFieldSaveModel.objects.first().weight\nOut[2]: 10 <Unit(\'gram\')>\n\nIn [3]: IntegerPintFieldSaveModel.objects.first().weight.magnitude\nOut[3]: 10\n\nIn [4]: IntegerPintFieldSaveModel.objects.first().weight.units\nOut[4]: <Unit(\'gram\')>\n```\n\n\n## Valid Lookups\n\nOther lookups will be added in the future. Currently available are:\n\n- exact\n- gt\n- gte\n- lt\n- lte\n- range\n- isnull\n\n```python\n# Perform some queries\nIntegerPintFieldSaveModel.objects.filter(weight__gt=medium)\n<QuerySet [<IntegerPintFieldSaveModel: large>]>\n\nIntegerPintFieldSaveModel.objects.filter(weight__gt=extra_small)\n<QuerySet [<IntegerPintFieldSaveModel: small>, <IntegerPintFieldSaveModel: large>]>\n\nIntegerPintFieldSaveModel.objects.filter(weight__gte=small)\n<QuerySet [<IntegerPintFieldSaveModel: small>, <IntegerPintFieldSaveModel: large>]>\n\nIntegerPintFieldSaveModel.objects.filter(weight__range=(small, medium))\n<QuerySet [<IntegerPintFieldSaveModel: small>]>\n```\n\n\n## Aggregates\n\nA number of aggregates have been implemented for the Django Pint Fields. Functionally they perform for Pint Fields the same way django\'s default aggregates work for other field types, and each is prepended with "Pint". The aggregates include:\n\n- PintAvg\n- PintCount\n- PintMax\n- PintMin\n- PintStdDev\n- PintSum\n- PintVariance\n\n```python\nfrom django_pint_field.aggregates import PintAvg, PintCount, PintMax, PintMin, PintStdDev, PintSum, PintVariance\n\n# Perform some queries\nIntegerPintFieldSaveModel.objects.aggregate(PintAvg(\'weight\'))\n{\'weight__pintavg\': Decimal(\'0.50500000000000000000\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintCount(\'weight\'))\n{\'weight__pintcount\': 2}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintMax(\'weight\'))\n{\'weight__pintmax\': Decimal(\'1.0\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintMin(\'weight\'))\n{\'weight__pintmin\': Decimal(\'0.01\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintStdDev(\'weight\'))\n{\'weight__pintstddev\': Decimal(\'0.49500000000000000000\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintSum(\'weight\'))\n{\'weight__pintsum\': Decimal(\'1.01\') <Unit(\'kilogram\')>}\n\nIntegerPintFieldSaveModel.objects.aggregate(PintVariance(\'weight\'))\n{\'weight__pintvariance\': Decimal(\'0.24502500000000000000\') <Unit(\'kilogram\')>}\n```\n\n\n## Use with Django Rest Framework\n\n\n```python\nfrom django_pint_field.rest import IntegerPintRestField\n\nclass DjangoPintFieldSerializer(serializers.ModelSerializer):\n    # Let DRF know which type of serializer field to use\n    weight = IntegerPintRestField()\n\n    class Meta:\n        model = IntegerPintFieldSaveModel\n        fields = ["name", "weight"]\n```\n\n\n## Creating your own units\n\nYou can [create your own pint units](https://pint.readthedocs.io/en/stable/advanced/defining.html) if the [default units](https://github.com/hgrecco/pint/blob/master/pint/default_en.txt) in pint are not sufficient.\n\nAnywhere within your project (ideally in settings or a file adjacent to settings), define the custom unit registry by importing Pint\'s default UnitRegistry and extending it:\n\n```python\nfrom pint import UnitRegistry\n\ncustom_ureg = UnitRegistry()\ncustom_ureg.define("custom = [custom]")\ncustom_ureg.define("kilocustom = 1000 * custom")\n```\n\nThen add the custom registry to your app\'s settings.py:\n\n`DJANGO_PINT_FIELD_UNIT_REGISTER = custom_ureg`\n\n\n## Model Fields\n\n- **IntegerPintField**: Stores a pint measurement as an integer (-2147483648 to 2147483647).\n- **BigIntegerPintField**: Stores a pint measurement as a big integer (-9223372036854775808 to 9223372036854775807).\n- **DecimalPintField**: Stores a pint measurement as a decimal. Like Django\'s DecimalField, DecimalPintField takes required `max_digits` and `decimal_places` parameters.\n\n\n## Form Fields\n\n- **IntegerPintFormField**: Used in forms with IntegerPintField and BigIntegerPintField.\n- **DecimalPintFormField**: Used in forms with DecimalPintField.\n\n\n## Widgets\n\n- **PintFieldWidget**: Default widget for all django pint field types.\n- **TabledPintFieldWidget**: Provides a table showing conversion to each of the `unit_choices`.\n\n![TabledPintFieldWidget](https://raw.githubusercontent.com/jacklinke/django-pint-field/main/media/TabledPintFieldWidget.png)\n\n\nExample usage:\n\n```python\nclass WeightModel(models.Model):\n    decimal_weight = DecimalPintField(\n        "gram",\n        blank=True,\n        null=True,\n        max_digits=10,\n        decimal_places=2,\n        unit_choices=[\n            "kilogram",\n            "milligram",\n            "pounds"\n        ],\n    )\n\nclass TabledWeightForm(forms.ModelForm):\n    class Meta:\n        model = WeightModel\n        fields = "__all__"\n\n    def __init__(self, *args, **kwargs):\n        super().__init__(*args, **kwargs)\n\n        # If we want to use the tabled widget, we need to pass the \n        #   default_unit and unit_choices to the new widget\n        default_unit = self.fields["decimal_weight"].default_unit\n        unit_choices = self.fields["decimal_weight"].unit_choices\n        self.fields["decimal_weight"].widget = TabledPintFieldWidget(\n            default_unit=default_unit, unit_choices=unit_choices\n        )\n```\n\nThe template for this widget is located at https://github.com/jacklinke/django-pint-field/blob/main/django_pint_field/templates/tabled_django_pint_field_widget.html\n\nIf you want to override the template, add your own template in your project at: "templates/django_pint_field/tabled_django_pint_field_widget.html"\n\n## DRF Serializer Fields\n\n- **IntegerPintRestField**: Used in DRF with IntegerPintField and BigIntegerPintField.\n- **DecimalPintRestField**: Used in DRF with DecimalPintField.\n\n\n## Settings\n\n<dl>\n  <dt><code>DJANGO_PINT_FIELD_DECIMAL_PRECISION</code></dt>\n  <dd>\n    Determines whether django_pint_field should automatically set the python decimal precision for the project. If an integer greater than 0 is provided, the decimal context precision for the entire project will be set to that value. Otherwise, the precision remains at the default (usually 28).<br>\n    <em>* Type: int</em>\n    <em>* Default: 0</em>\n  </dd>\n\n  <dt><code>DJANGO_PINT_FIELD_UNIT_REGISTER</code></dt>\n  <dd>\n    The Unit Registry to use in the project. Defaults to pint.UnitRegistry.<br>\n    <em>* Type: int</em>\n    <em>* Default: 0</em>\n  </dd>\n</dl>\n\n\n## Rounding modes (upcoming feature)\n\n**decimal.ROUND_CEILING**\nRound towards Infinity.\n\n**decimal.ROUND_DOWN**\nRound towards zero.\n\n**decimal.ROUND_FLOOR**\nRound towards -Infinity.\n\n**decimal.ROUND_HALF_DOWN**\nRound to nearest with ties going towards zero.\n\n**decimal.ROUND_HALF_EVEN**\nRound to nearest with ties going to nearest even integer.\n\n**decimal.ROUND_HALF_UP**\nRound to nearest with ties going away from zero.\n\n**decimal.ROUND_UP**\nRound away from zero.\n\n**decimal.ROUND_05UP**\nRound away from zero if last digit after rounding towards zero would have been 0 or 5; otherwise round towards zero.\n\nRead more about rounding modes for decimals at the [decimal docs](https://docs.python.org/3/library/decimal.html#rounding-modes)\n\n\n## Use the test app with docker compose\n\n### Set up a virtual environment (recommended)\n\nMake a virtual environment named `.venv`:\n\n`python3 -m venv .venv`\n    \nActivate the new environment:\n\n`source .venv/bin/activate`\n\n\n### Install dependencies\n\n*Requires [poetry](https://python-poetry.org/). If you do not yet have it installed, run `pip install poetry`.*\n\n`poetry install --with dev`\n\n### Build and bring up\n\n```\ndocker compose build\ndocker compose run django python manage.py migrate\ndocker compose run django python manage.py createsuperuser\ndocker compose up -d\n```\n\nNavigate to `127.0.0.1:8000`\n\n### Test (assuming you have already performed `build`)\n\n`docker compose run django python manage.py test`\n\n\n## Run psql on the Postgres database\n\n`docker compose exec postgres psql -U postgres`\n\n\n## ToDos:\n- Implement rounding modes\n- Think through what it would take to build range types for these fields\n- Add extensible widget template\n',
     'author': 'Jack Linke',
     'author_email': 'jack@watervize.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/jacklinke/django-pint-field',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `django_pint_field-0.3.4/PKG-INFO` & `django_pint_field-0.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pint-field
-Version: 0.3.4
+Version: 0.3.5
 Summary: Pint Fields for Django and Postgres
 Home-page: https://github.com/jacklinke/django-pint-field
 License: MIT
 Keywords: django
 Author: Jack Linke
 Author-email: jack@watervize.com
 Requires-Python: >=3.8,<4.0
@@ -26,14 +26,15 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: django (>=3.2)
 Requires-Dist: pint (>=0.19)
 Requires-Dist: psycopg2-binary (>=2.9,<3.0)
 Project-URL: Repository, https://github.com/jacklinke/django-pint-field
 Description-Content-Type: text/markdown
 
+
 # django-pint-field
 
 Use [pint](https://pint.readthedocs.io/en/stable/) with Django's ORM.
 
 If you want to store quantities (1 gram, 3 miles, 8.120391 angstroms, etc) in a model, edit them in forms, and have the ability to convert to other quantities in your django projects, this is the package for you!
 
 This package is modified from the fantastic [django-pint](https://github.com/CarliJoy/django-pint) with different goals. Unlike django-pint, in this project we use a composite Postgres field to store both the magnitude and the user's desired units, along with the equivalent value in base units. This third piece of date - the base units - makes it possible to conduct lookups comparing one instance that might be specified in "grams" with another that may be specified in "pounds", but display each instance in the units that the user desires. The units your users want to use are the units they see, while still allowing accurate comparisons of one quantity to another.
@@ -219,15 +220,56 @@
 - **IntegerPintFormField**: Used in forms with IntegerPintField and BigIntegerPintField.
 - **DecimalPintFormField**: Used in forms with DecimalPintField.
 
 
 ## Widgets
 
 - **PintFieldWidget**: Default widget for all django pint field types.
+- **TabledPintFieldWidget**: Provides a table showing conversion to each of the `unit_choices`.
+
+![TabledPintFieldWidget](https://raw.githubusercontent.com/jacklinke/django-pint-field/main/media/TabledPintFieldWidget.png)
+
+
+Example usage:
+
+```python
+class WeightModel(models.Model):
+    decimal_weight = DecimalPintField(
+        "gram",
+        blank=True,
+        null=True,
+        max_digits=10,
+        decimal_places=2,
+        unit_choices=[
+            "kilogram",
+            "milligram",
+            "pounds"
+        ],
+    )
+
+class TabledWeightForm(forms.ModelForm):
+    class Meta:
+        model = WeightModel
+        fields = "__all__"
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        # If we want to use the tabled widget, we need to pass the 
+        #   default_unit and unit_choices to the new widget
+        default_unit = self.fields["decimal_weight"].default_unit
+        unit_choices = self.fields["decimal_weight"].unit_choices
+        self.fields["decimal_weight"].widget = TabledPintFieldWidget(
+            default_unit=default_unit, unit_choices=unit_choices
+        )
+```
+
+The template for this widget is located at https://github.com/jacklinke/django-pint-field/blob/main/django_pint_field/templates/tabled_django_pint_field_widget.html
 
+If you want to override the template, add your own template in your project at: "templates/django_pint_field/tabled_django_pint_field_widget.html"
 
 ## DRF Serializer Fields
 
 - **IntegerPintRestField**: Used in DRF with IntegerPintField and BigIntegerPintField.
 - **DecimalPintRestField**: Used in DRF with DecimalPintField.
```

