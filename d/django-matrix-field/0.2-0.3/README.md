# Comparing `tmp/django-matrix-field-0.2.tar.gz` & `tmp/django_matrix_field-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-matrix-field-0.2.tar", last modified: Fri Dec 28 02:11:16 2012, max compression
+gzip compressed data, was "django_matrix_field-0.3.tar", last modified: Wed May 15 23:37:43 2024, max compression
```

## Comparing `django-matrix-field-0.2.tar` & `django_matrix_field-0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mfogel     (501) staff       (20)        0 2012-12-28 02:11:16.000000 django-matrix-field-0.2/
-drwxr-xr-x   0 mfogel     (501) staff       (20)        0 2012-12-28 02:11:16.000000 django-matrix-field-0.2/django_matrix_field.egg-info/
--rw-r--r--   0 mfogel     (501) staff       (20)        1 2012-12-28 02:11:16.000000 django-matrix-field-0.2/django_matrix_field.egg-info/dependency_links.txt
--rw-r--r--   0 mfogel     (501) staff       (20)     3465 2012-12-28 02:11:16.000000 django-matrix-field-0.2/django_matrix_field.egg-info/PKG-INFO
--rw-r--r--   0 mfogel     (501) staff       (20)        6 2012-12-28 02:11:16.000000 django-matrix-field-0.2/django_matrix_field.egg-info/requires.txt
--rw-r--r--   0 mfogel     (501) staff       (20)      405 2012-12-28 02:11:16.000000 django-matrix-field-0.2/django_matrix_field.egg-info/SOURCES.txt
--rw-r--r--   0 mfogel     (501) staff       (20)       13 2012-12-28 02:11:16.000000 django-matrix-field-0.2/django_matrix_field.egg-info/top_level.txt
-drwxr-xr-x   0 mfogel     (501) staff       (20)        0 2012-12-28 02:11:16.000000 django-matrix-field-0.2/matrix_field/
--rw-r--r--   0 mfogel     (501) staff       (20)       78 2012-12-28 02:00:06.000000 django-matrix-field-0.2/matrix_field/__init__.py
--rw-r--r--   0 mfogel     (501) staff       (20)     2641 2012-12-28 02:00:06.000000 django-matrix-field-0.2/matrix_field/fields.py
--rw-r--r--   0 mfogel     (501) staff       (20)      558 2012-12-28 00:17:22.000000 django-matrix-field-0.2/matrix_field/forms.py
--rw-r--r--   0 mfogel     (501) staff       (20)       27 2012-12-28 00:17:22.000000 django-matrix-field-0.2/matrix_field/models.py
--rw-r--r--   0 mfogel     (501) staff       (20)     5093 2012-12-28 00:17:22.000000 django-matrix-field-0.2/matrix_field/test_settings.py
--rw-r--r--   0 mfogel     (501) staff       (20)     5316 2012-12-28 02:00:06.000000 django-matrix-field-0.2/matrix_field/tests.py
--rw-r--r--   0 mfogel     (501) staff       (20)     1648 2012-12-28 02:00:06.000000 django-matrix-field-0.2/matrix_field/validators.py
--rw-r--r--   0 mfogel     (501) staff       (20)     3465 2012-12-28 02:11:16.000000 django-matrix-field-0.2/PKG-INFO
--rw-r--r--   0 mfogel     (501) staff       (20)     2135 2012-12-28 02:07:56.000000 django-matrix-field-0.2/README.rst
--rw-r--r--   0 mfogel     (501) staff       (20)       59 2012-12-28 02:11:16.000000 django-matrix-field-0.2/setup.cfg
--rw-r--r--   0 mfogel     (501) staff       (20)     1419 2012-12-28 02:00:06.000000 django-matrix-field-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 23:37:43.171526 django_matrix_field-0.3/
+-rw-rw-rw-   0        0        0     2218 2024-05-15 23:37:43.170526 django_matrix_field-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1575 2024-05-15 23:35:50.000000 django_matrix_field-0.3/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-15 23:37:43.169525 django_matrix_field-0.3/django_matrix_field.egg-info/
+-rw-rw-rw-   0        0        0     2218 2024-05-15 23:37:43.000000 django_matrix_field-0.3/django_matrix_field.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2024-05-15 23:37:43.000000 django_matrix_field-0.3/django_matrix_field.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 23:37:43.000000 django_matrix_field-0.3/django_matrix_field.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 23:37:43.000000 django_matrix_field-0.3/django_matrix_field.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-15 23:37:43.000000 django_matrix_field-0.3/django_matrix_field.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-15 23:37:43.168526 django_matrix_field-0.3/matrix_field/
+-rw-rw-rw-   0        0        0       81 2024-05-15 23:35:50.000000 django_matrix_field-0.3/matrix_field/__init__.py
+-rw-rw-rw-   0        0        0     2871 2024-05-15 23:35:50.000000 django_matrix_field-0.3/matrix_field/fields.py
+-rw-rw-rw-   0        0        0      574 2024-05-15 23:35:50.000000 django_matrix_field-0.3/matrix_field/forms.py
+-rw-rw-rw-   0        0        0       28 2024-05-15 23:35:50.000000 django_matrix_field-0.3/matrix_field/models.py
+-rw-rw-rw-   0        0        0     5254 2024-05-15 23:35:50.000000 django_matrix_field-0.3/matrix_field/test_settings.py
+-rw-rw-rw-   0        0        0     5473 2024-05-15 23:35:50.000000 django_matrix_field-0.3/matrix_field/tests.py
+-rw-rw-rw-   0        0        0     1694 2024-05-15 23:35:50.000000 django_matrix_field-0.3/matrix_field/validators.py
+-rw-rw-rw-   0        0        0       42 2024-05-15 23:37:43.171526 django_matrix_field-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1468 2024-05-15 23:35:50.000000 django_matrix_field-0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-matrix-field-0.2/matrix_field/fields.py` & `django_matrix_field-0.3/matrix_field/fields.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,85 @@
-import json
-
-from django.core.exceptions import ImproperlyConfigured, ValidationError
-from django.db import models
-from django.db.models.fields import NOT_PROVIDED
-
-from .forms import MatrixFormField
-from .validators import DataTypeValidator, DimensionsValidator
-
-
-class MatrixField(models.Field):
-    """
-    Provides database store for matrices.
-    """
-
-    description = "A matrix"
-    __metaclass__ = models.SubfieldBase
-
-    MAX_LENGTH = 255
-
-    def __init__(self, datatype=None, dimensions=None, **kwargs):
-        if not datatype or not dimensions:
-            raise ImproperlyConfigured("Required kwarg 'datatype' or "
-                                       "'dimensions' missing")
-        self.datatype, self.dimensions = datatype, dimensions
-        defaults = {
-            'max_length': self.MAX_LENGTH,
-            'default': None,
-        }
-        defaults.update(kwargs)
-        super(MatrixField, self).__init__(**defaults)
-        self.validators.append(DataTypeValidator(self.datatype))
-        self.validators.append(DimensionsValidator(self.dimensions))
-
-    def get_internal_type(self):
-        # TODO: take advantage of postgres matrix type
-        #       kinda the whole reason this django app even exists...
-        return 'CharField'
-
-    def to_python(self, value):
-        "Convert to python matrix (arrays of arrays)"
-        if isinstance(value, (list, tuple)) or value is None:
-            return value
-        try:
-            return json.loads(value)
-        except:
-            raise ValidationError("Unable to convert value to matrix")
-
-    def get_prep_value(self, value):
-        "Convert to string"
-        return json.dumps(value)
-
-    def formfield(self, **kwargs):
-        defaults = {
-            'datatype': self.datatype,
-            'dimensions': self.dimensions,
-            'form_class': MatrixFormField,
-        }
-        defaults.update(kwargs)
-        return super(MatrixField, self).formfield(**defaults)
-
-
-# South support
-try:
-    from south.modelsinspector import add_introspection_rules
-except ImportError:
-    pass
-else:
-    add_introspection_rules(
-        rules=[(
-            (MatrixField, ),    # Class(es) these apply to
-            [],                 # Positional arguments (not used)
-            {                   # Keyword argument
-                'max_length': [
-                    'max_length', {'default': MatrixField.MAX_LENGTH}
-                ],
-                'datatype': ['datatype', {'default': NOT_PROVIDED}],
-                'dimensions': ['dimensions', {'default': NOT_PROVIDED}],
-            },
-        )],
-        patterns=['matrix_field\.fields\.']
-    )
+import json
+
+from django.core.exceptions import ImproperlyConfigured, ValidationError
+from django.db import models
+from django.db.models.fields import NOT_PROVIDED
+
+from .forms import MatrixFormField
+from .validators import DataTypeValidator, DimensionsValidator
+
+
+class MatrixField(models.Field):
+    """
+    Provides database store for matrices.
+    """
+
+    description = "A matrix"
+    #_metaclass__ = models.SubfieldBase
+
+    MAX_LENGTH = 255
+
+    def __init__(self, datatype='int', dimensions=(3,3), **kwargs):
+        if not datatype or not dimensions:
+            print('a', self)
+            # raise ImproperlyConfigured("Required kwarg 'datatype' or "
+            #                            "'dimensions' missing")
+        else:
+            self.datatype, self.dimensions = datatype, dimensions
+            defaults = {
+                'max_length': self.MAX_LENGTH,
+                'default': None,
+            }
+            defaults.update(kwargs)
+            super(MatrixField, self).__init__(**defaults)
+            self.validators.append(DataTypeValidator(self.datatype))
+            self.validators.append(DimensionsValidator(self.dimensions))
+
+    def get_internal_type(self):
+        # TODO: take advantage of postgres matrix type
+        #       kinda the whole reason this django app even exists...
+        return 'CharField'
+
+    def to_python(self, value):
+        "Convert to python matrix (arrays of arrays)"
+        if isinstance(value, (list, tuple)) or value is None:
+            return value
+        try:
+            return json.loads(value)
+        except:
+            raise ValidationError("Unable to convert value to matrix")
+
+    def get_prep_value(self, value):
+        "Convert to string"
+        return json.dumps(value)
+
+    def formfield(self, **kwargs):
+        defaults = {
+            'datatype': self.datatype,
+            'dimensions': self.dimensions,
+            'form_class': MatrixFormField,
+        }
+        defaults.update(kwargs)
+        #return super(MatrixField, self).formfield(**defaults)
+        return super().formfield(**{**defaults, **kwargs})
+
+
+# South support
+try:
+    from south.modelsinspector import add_introspection_rules
+except ImportError:
+    pass
+else:
+    add_introspection_rules(
+        rules=[(
+            (MatrixField, ),    # Class(es) these apply to
+            [],                 # Positional arguments (not used)
+            {                   # Keyword argument
+                'max_length': [
+                    'max_length', {'default': MatrixField.MAX_LENGTH}
+                ],
+                'datatype': ['datatype', {'default': NOT_PROVIDED}],
+                'dimensions': ['dimensions', {'default': NOT_PROVIDED}],
+            },
+        )],
+        patterns=['matrix_field\.fields\.']
+    )
```

### Comparing `django-matrix-field-0.2/matrix_field/tests.py` & `django_matrix_field-0.3/matrix_field/tests.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import json
-
-from django import forms
-from django.core.exceptions import ValidationError
-from django.db import models
-from django.test import TestCase
-
-from . import MatrixField, MatrixFormField
-
-
-M1 = [[3, 4], [4, 5], [6, 7]]
-M2 = [[[2.0]]]
-M3a = ['a', 'b']
-M3b = ['c', 'd']
-
-M1_str = json.dumps(M1)
-M2_str = json.dumps(M2)
-M3a_str = json.dumps(M3a)
-M3b_str = json.dumps(M3b)
-
-
-class TestModel(models.Model):
-    f1 = MatrixField(datatype='int', dimensions=(3, 2))
-    f2 = MatrixField(datatype='float', dimensions=(1, 1, 1), blank=True)
-    f3 = MatrixField(datatype='str', dimensions=(2,), blank=True,
-                     default=M3a_str)
-
-
-class TestForm(forms.Form):
-    f1 = MatrixFormField(datatype='int', dimensions=(3, 2))
-    f2 = MatrixFormField(datatype='float', dimensions=(1, 1, 1),
-                         required=False)
-
-
-class TestModelForm(forms.ModelForm):
-    class Meta:
-        model = TestModel
-
-
-class MatrixFormFieldTestCase(TestCase):
-
-    def test_valid_specify_all(self):
-        form = TestForm({'f1': M1_str, 'f2': M2_str})
-        self.assertTrue(form.is_valid())
-        self.assertEqual(form.cleaned_data['f1'], M1)
-        self.assertEqual(form.cleaned_data['f2'], M2)
-
-    def test_valid_with_defaults(self):
-        form = TestForm({'f1': M1_str})
-        self.assertTrue(form.is_valid())
-        self.assertEqual(form.cleaned_data['f1'], M1)
-        self.assertEqual(form.cleaned_data['f2'], None)
-
-    def test_invalid_blank(self):
-        form = TestForm({})
-        self.assertFalse(form.is_valid())
-        self.assertTrue(any('required' in e for e in form.errors['f1']))
-
-    def test_invalid_datatype(self):
-        value = [[1.0, 1.0], [1.0, 1.0], [1.0, 1.0]]
-        form = TestForm({'f1': json.dumps(value)})
-        self.assertFalse(form.is_valid())
-        self.assertTrue(any('datatype' in e for e in form.errors['f1']))
-
-    def test_invalid_dimesion(self):
-        form = TestForm({'f1': json.dumps([1])})
-        self.assertFalse(form.is_valid())
-        self.assertTrue(any('dimension' in e for e in form.errors['f1']))
-
-
-class MatrixFieldModelFormTestCase(TestCase):
-
-    def test_valid_specify_all(self):
-        form = TestModelForm({'f1': M1_str, 'f2': M2_str, 'f3': M3b_str})
-        self.assertTrue(form.is_valid())
-        form.save()
-        self.assertEqual(TestModel.objects.count(), 1)
-
-        m = TestModel.objects.get()
-        self.assertEqual(m.f1, M1)
-        self.assertEqual(m.f2, M2)
-        self.assertEqual(m.f3, M3b)
-
-    def test_valid_with_defaults(self):
-        # seems there should be a better way to get a form's default values...?
-        # http://stackoverflow.com/questions/7399490/
-        data = dict(
-            (field_name, field.initial)
-            for field_name, field in TestModelForm().fields.iteritems()
-        )
-        data.update({'f1': M1})
-        form = TestModelForm(data=data)
-        self.assertTrue(form.is_valid())
-        form.save()
-        self.assertEqual(TestModel.objects.count(), 1)
-
-        m = TestModel.objects.get()
-        self.assertEqual(m.f2, None)
-        self.assertEqual(m.f3, M3a)
-
-    def test_invalid_required(self):
-        form = TestModelForm({})
-        self.assertFalse(form.is_valid())
-        self.assertTrue(any('required' in e for e in form.errors['f1']))
-
-    def test_invalid_datatype(self):
-        value = [[1.0, 1.0], [1.0, 1.0], [1.0, 1.0]]
-        form = TestModelForm({'f1': json.dumps(value)})
-        self.assertFalse(form.is_valid())
-        self.assertTrue(any('datatype' in e for e in form.errors['f1']))
-
-    def test_invalid_dims1(self):
-        form = TestModelForm({'f1': M1_str, 'f2': json.dumps([[1]])})
-        self.assertFalse(form.is_valid())
-        self.assertTrue(any('dimension' in e for e in form.errors['f2']))
-
-    def test_invalid_dims2(self):
-        value = ['a', 'b', 'c']
-        form = TestModelForm({'f1': M1_str, 'f3': json.dumps(value)})
-        self.assertFalse(form.is_valid())
-        self.assertTrue(any('dimension' in e for e in form.errors['f3']))
-
-
-class MatrixFieldTestCase(TestCase):
-
-    def test_valid(self):
-        m = TestModel.objects.create(f1=M1, f2=M2, f3=M3b)
-        m = TestModel.objects.get(pk=m.pk)
-        self.assertEqual(m.f1, M1)
-        self.assertEqual(m.f2, M2)
-        self.assertEqual(m.f3, M3b)
-
-    def test_valid_blank(self):
-        m = TestModel.objects.create(f1=M1)
-        m = TestModel.objects.get(pk=m.pk)
-        self.assertEqual(m.f2, None)
-        self.assertEqual(m.f3, M3a)
-
-    def test_invalid_type(self):
-        with self.assertRaises(ValidationError):
-            TestModel(f1=M1, f3=[2.0, 3.0]).full_clean()
-        with self.assertRaises(ValidationError):
-            TestModel(f1=M1, f2=[[[2]]]).full_clean()
-
-    def test_invalid_dims(self):
-        with self.assertRaises(ValidationError):
-            TestModel(f1=M1, f2=['a']).full_clean()
-        with self.assertRaises(ValidationError):
-            TestModel(f1=M1, f3=[['a'], ['b']]).full_clean()
-
-    def test_invalid_altogether(self):
-        with self.assertRaises(ValidationError):
-            TestModel(f1={'a': 2}).full_clean()
-        with self.assertRaises(ValidationError):
-            TestModel(f1=4).full_clean()
-        with self.assertRaises(ValidationError):
-            TestModel(f1='blah blah').full_clean()
+import json
+
+from django import forms
+from django.core.exceptions import ValidationError
+from django.db import models
+from django.test import TestCase
+
+from . import MatrixField, MatrixFormField
+
+
+M1 = [[3, 4], [4, 5], [6, 7]]
+M2 = [[[2.0]]]
+M3a = ['a', 'b']
+M3b = ['c', 'd']
+
+M1_str = json.dumps(M1)
+M2_str = json.dumps(M2)
+M3a_str = json.dumps(M3a)
+M3b_str = json.dumps(M3b)
+
+
+class TestModel(models.Model):
+    f1 = MatrixField(datatype='int', dimensions=(3, 2))
+    f2 = MatrixField(datatype='float', dimensions=(1, 1, 1), blank=True)
+    f3 = MatrixField(datatype='str', dimensions=(2,), blank=True,
+                     default=M3a_str)
+
+
+class TestForm(forms.Form):
+    f1 = MatrixFormField(datatype='int', dimensions=(3, 2))
+    f2 = MatrixFormField(datatype='float', dimensions=(1, 1, 1),
+                         required=False)
+
+
+class TestModelForm(forms.ModelForm):
+    class Meta:
+        model = TestModel
+
+
+class MatrixFormFieldTestCase(TestCase):
+
+    def test_valid_specify_all(self):
+        form = TestForm({'f1': M1_str, 'f2': M2_str})
+        self.assertTrue(form.is_valid())
+        self.assertEqual(form.cleaned_data['f1'], M1)
+        self.assertEqual(form.cleaned_data['f2'], M2)
+
+    def test_valid_with_defaults(self):
+        form = TestForm({'f1': M1_str})
+        self.assertTrue(form.is_valid())
+        self.assertEqual(form.cleaned_data['f1'], M1)
+        self.assertEqual(form.cleaned_data['f2'], None)
+
+    def test_invalid_blank(self):
+        form = TestForm({})
+        self.assertFalse(form.is_valid())
+        self.assertTrue(any('required' in e for e in form.errors['f1']))
+
+    def test_invalid_datatype(self):
+        value = [[1.0, 1.0], [1.0, 1.0], [1.0, 1.0]]
+        form = TestForm({'f1': json.dumps(value)})
+        self.assertFalse(form.is_valid())
+        self.assertTrue(any('datatype' in e for e in form.errors['f1']))
+
+    def test_invalid_dimesion(self):
+        form = TestForm({'f1': json.dumps([1])})
+        self.assertFalse(form.is_valid())
+        self.assertTrue(any('dimension' in e for e in form.errors['f1']))
+
+
+class MatrixFieldModelFormTestCase(TestCase):
+
+    def test_valid_specify_all(self):
+        form = TestModelForm({'f1': M1_str, 'f2': M2_str, 'f3': M3b_str})
+        self.assertTrue(form.is_valid())
+        form.save()
+        self.assertEqual(TestModel.objects.count(), 1)
+
+        m = TestModel.objects.get()
+        self.assertEqual(m.f1, M1)
+        self.assertEqual(m.f2, M2)
+        self.assertEqual(m.f3, M3b)
+
+    def test_valid_with_defaults(self):
+        # seems there should be a better way to get a form's default values...?
+        # http://stackoverflow.com/questions/7399490/
+        data = dict(
+            (field_name, field.initial)
+            for field_name, field in TestModelForm().fields.iteritems()
+        )
+        data.update({'f1': M1})
+        form = TestModelForm(data=data)
+        self.assertTrue(form.is_valid())
+        form.save()
+        self.assertEqual(TestModel.objects.count(), 1)
+
+        m = TestModel.objects.get()
+        self.assertEqual(m.f2, None)
+        self.assertEqual(m.f3, M3a)
+
+    def test_invalid_required(self):
+        form = TestModelForm({})
+        self.assertFalse(form.is_valid())
+        self.assertTrue(any('required' in e for e in form.errors['f1']))
+
+    def test_invalid_datatype(self):
+        value = [[1.0, 1.0], [1.0, 1.0], [1.0, 1.0]]
+        form = TestModelForm({'f1': json.dumps(value)})
+        self.assertFalse(form.is_valid())
+        self.assertTrue(any('datatype' in e for e in form.errors['f1']))
+
+    def test_invalid_dims1(self):
+        form = TestModelForm({'f1': M1_str, 'f2': json.dumps([[1]])})
+        self.assertFalse(form.is_valid())
+        self.assertTrue(any('dimension' in e for e in form.errors['f2']))
+
+    def test_invalid_dims2(self):
+        value = ['a', 'b', 'c']
+        form = TestModelForm({'f1': M1_str, 'f3': json.dumps(value)})
+        self.assertFalse(form.is_valid())
+        self.assertTrue(any('dimension' in e for e in form.errors['f3']))
+
+
+class MatrixFieldTestCase(TestCase):
+
+    def test_valid(self):
+        m = TestModel.objects.create(f1=M1, f2=M2, f3=M3b)
+        m = TestModel.objects.get(pk=m.pk)
+        self.assertEqual(m.f1, M1)
+        self.assertEqual(m.f2, M2)
+        self.assertEqual(m.f3, M3b)
+
+    def test_valid_blank(self):
+        m = TestModel.objects.create(f1=M1)
+        m = TestModel.objects.get(pk=m.pk)
+        self.assertEqual(m.f2, None)
+        self.assertEqual(m.f3, M3a)
+
+    def test_invalid_type(self):
+        with self.assertRaises(ValidationError):
+            TestModel(f1=M1, f3=[2.0, 3.0]).full_clean()
+        with self.assertRaises(ValidationError):
+            TestModel(f1=M1, f2=[[[2]]]).full_clean()
+
+    def test_invalid_dims(self):
+        with self.assertRaises(ValidationError):
+            TestModel(f1=M1, f2=['a']).full_clean()
+        with self.assertRaises(ValidationError):
+            TestModel(f1=M1, f3=[['a'], ['b']]).full_clean()
+
+    def test_invalid_altogether(self):
+        with self.assertRaises(ValidationError):
+            TestModel(f1={'a': 2}).full_clean()
+        with self.assertRaises(ValidationError):
+            TestModel(f1=4).full_clean()
+        with self.assertRaises(ValidationError):
+            TestModel(f1='blah blah').full_clean()
```

### Comparing `django-matrix-field-0.2/README.rst` & `django_matrix_field-0.3/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,87 +1,59 @@
-django-matrix-field
-===================
-
-.. image:: https://api.travis-ci.org/mfogel/django-matrix-field.png?branch=develop
-   :alt: Build Status
-   :target: https://travis-ci.org/mfogel/django-matrix-field
-
-A Django app providing database and form fields for matrices (arrays of arrays).
-
-Examples
---------
-
-Database Field
-~~~~~~~~~~~~~~
-
-.. code:: python
-
-    from django.db import models
-    from matrix_field import MatrixField
-
-    class MyModel(models.Model):
-        matrix1 = MatrixField(datatype='float', dimensions=(3, 2))
-        matrix2 = MatrixField(datatype='str', dimensions=(2,))
-
-    my_inst = MyModel(
-        matrix1=[[5.1, -1.2], [4.2, 0.0], [3.14, 2.71]],
-        matrix2=['a list', 'of strings'],
-    )
-    my_inst.full_clean()  # validates datatype, dimensions
-    my_inst.save()        # values stored in DB as json
-
-    m1 = my_inst.matrix1  # values retrieved as matrices
-    repr(m1)              # '[[5.1, -1.2], [4.2, 0.0], [3.14, 2.71]]'
-
-
-Form Field
-~~~~~~~~~~
-
-.. code:: python
-
-    import json
-    from django import forms
-    from matrix_field import MatrixFormField
-
-    class MyForm(forms.Form):
-        matrix = MatrixFormField(datatype='int', dimensions=(2, 1))
-
-    my_form = MyForm({
-        'matrix': json.dumps([[2], [1]]),  # assignment of json representation
-    })
-    my_form.full_clean()                   # validates datatype, dimensions
-
-    m = my_form.cleaned_data['matrix']  # values retrieved as matrices
-    repr(m)                             # '[[2], [1]]'
-
-
-Installation
-------------
-
-Now on `pypi`__!
-
-.. code:: sh
-
-    pip install django-matrix-field
-
-Running the Tests
------------------
-
-Using `Doug Hellman's virtualenvwrapper`__:
-
-.. code:: sh
-
-    mktmpenv
-    pip install django-matrix-field
-    export DJANGO_SETTINGS_MODULE=matrix_field.test_settings
-    django-admin.py test matrix_field
-
-
-Found a Bug?
-------------
-
-To file a bug or submit a patch, please head over to `django-matrix-field on github`__.
-
-
-__ http://pypi.python.org/pypi/django-matrix-field/
-__ http://www.doughellmann.com/projects/virtualenvwrapper/
-__ https://github.com/mfogel/django-matrix-field/
+django-matrix-field
+===================
+
+A Django app providing database and form fields for matrices (arrays of arrays).
+
+Examples
+--------
+
+Database Field
+~~~~~~~~~~~~~~
+
+.. code:: python
+
+    from django.db import models
+    from matrix_field import MatrixField
+
+    class MyModel(models.Model):
+        matrix1 = MatrixField(datatype='float', dimensions=(3, 2))
+        matrix2 = MatrixField(datatype='str', dimensions=(2,))
+
+    my_inst = MyModel(
+        matrix1=[[5.1, -1.2], [4.2, 0.0], [3.14, 2.71]],
+        matrix2=['a list', 'of strings'],
+    )
+    my_inst.full_clean()  # validates datatype, dimensions
+    my_inst.save()        # values stored in DB as json
+
+    m1 = my_inst.matrix1  # values retrieved as matrices
+    repr(m1)              # '[[5.1, -1.2], [4.2, 0.0], [3.14, 2.71]]'
+
+
+Form Field
+~~~~~~~~~~
+
+.. code:: python
+
+    import json
+    from django import forms
+    from matrix_field import MatrixFormField
+
+    class MyForm(forms.Form):
+        matrix = MatrixFormField(datatype='int', dimensions=(2, 1))
+
+    my_form = MyForm({
+        'matrix': json.dumps([[2], [1]]),  # assignment of json representation
+    })
+    my_form.full_clean()                   # validates datatype, dimensions
+
+    m = my_form.cleaned_data['matrix']  # values retrieved as matrices
+    repr(m)                             # '[[2], [1]]'
+
+
+Found a Bug?
+------------
+
+To file a bug or submit a patch, please head over to `django-matrix-field on github`__.
+
+
+__ https://github.com/Sharmaxz/django-matrix-field
```

