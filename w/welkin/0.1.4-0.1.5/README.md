# Comparing `tmp/welkin-0.1.4.tar.gz` & `tmp/welkin-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "welkin-0.1.4.tar", max compression
+gzip compressed data, was "welkin-0.1.5.tar", max compression
```

## Comparing `welkin-0.1.4.tar` & `welkin-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0    35050 2024-05-10 23:09:46.295739 welkin-0.1.4/LICENSE.md
--rw-r--r--   0        0        0     2226 2024-05-10 23:09:46.295739 welkin-0.1.4/README.md
--rw-r--r--   0        0        0     2889 2024-05-10 23:09:46.295739 welkin-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2250 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/__init__.py
--rw-r--r--   0        0        0      660 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/__version__.py
--rw-r--r--   0        0        0     1897 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/authentication.py
--rw-r--r--   0        0        0    10160 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/client.py
--rw-r--r--   0        0        0      789 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/exceptions.py
--rw-r--r--   0        0        0     1644 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/__init__.py
--rw-r--r--   0        0        0     3185 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/assessment.py
--rw-r--r--   0        0        0     3651 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/base.py
--rw-r--r--   0        0        0     4049 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/calendar.py
--rw-r--r--   0        0        0      727 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/care_plan.py
--rw-r--r--   0        0        0     2159 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/cdt.py
--rw-r--r--   0        0        0     1556 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/chat.py
--rw-r--r--   0        0        0     2108 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/document.py
--rw-r--r--   0        0        0      845 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/email.py
--rw-r--r--   0        0        0     3312 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/encounter.py
--rw-r--r--   0        0        0     2637 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/formation.py
--rw-r--r--   0        0        0     2499 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/patient.py
--rw-r--r--   0        0        0     2321 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/program.py
--rw-r--r--   0        0        0      834 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/sms.py
--rw-r--r--   0        0        0     1617 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/models/user.py
--rw-r--r--   0        0        0     5300 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/pagination.py
--rw-r--r--   0        0        0     5447 2024-05-10 23:09:46.303739 welkin-0.1.4/welkin/util.py
--rw-r--r--   0        0        0     3415 1970-01-01 00:00:00.000000 welkin-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35050 2024-05-16 21:27:10.134789 welkin-0.1.5/LICENSE.md
+-rw-r--r--   0        0        0     2226 2024-05-16 21:27:10.134789 welkin-0.1.5/README.md
+-rw-r--r--   0        0        0     2889 2024-05-16 21:27:10.134789 welkin-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2250 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/__init__.py
+-rw-r--r--   0        0        0      660 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/__version__.py
+-rw-r--r--   0        0        0     1897 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/authentication.py
+-rw-r--r--   0        0        0    10207 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/client.py
+-rw-r--r--   0        0        0      789 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/exceptions.py
+-rw-r--r--   0        0        0     1718 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/__init__.py
+-rw-r--r--   0        0        0     3185 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/assessment.py
+-rw-r--r--   0        0        0     3651 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/base.py
+-rw-r--r--   0        0        0     4049 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/calendar.py
+-rw-r--r--   0        0        0      727 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/care_plan.py
+-rw-r--r--   0        0        0     2159 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/cdt.py
+-rw-r--r--   0        0        0     1556 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/chat.py
+-rw-r--r--   0        0        0     2108 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/document.py
+-rw-r--r--   0        0        0      845 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/email.py
+-rw-r--r--   0        0        0     3312 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/encounter.py
+-rw-r--r--   0        0        0      630 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/export.py
+-rw-r--r--   0        0        0     2637 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/formation.py
+-rw-r--r--   0        0        0     2499 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/patient.py
+-rw-r--r--   0        0        0     2321 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/program.py
+-rw-r--r--   0        0        0      834 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/sms.py
+-rw-r--r--   0        0        0     1617 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/models/user.py
+-rw-r--r--   0        0        0     5805 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/pagination.py
+-rw-r--r--   0        0        0     5447 2024-05-16 21:27:10.170789 welkin-0.1.5/welkin/util.py
+-rw-r--r--   0        0        0     3415 1970-01-01 00:00:00.000000 welkin-0.1.5/PKG-INFO
```

### Comparing `welkin-0.1.4/LICENSE.md` & `welkin-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/README.md` & `welkin-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/pyproject.toml` & `welkin-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "welkin"
-version = "0.1.4"
+version = "0.1.5"
 description = "Python Welkin Health API Wrapper."
 authors = ["Sam Morgan <sama4mail@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/lightmatter/welkin-health"
 documentation = "https://welkin.readthedocs.io"
 classifiers = [
```

### Comparing `welkin-0.1.4/welkin/__init__.py` & `welkin-0.1.5/welkin/__init__.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/__version__.py` & `welkin-0.1.5/welkin/__version__.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/authentication.py` & `welkin-0.1.5/welkin/authentication.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/client.py` & `welkin-0.1.5/welkin/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,33 +78,34 @@
     AssessmentRecords = models.AssessmentRecords
     Assessments = models.Assessments
     CalendarEvent = models.CalendarEvent
     CalendarEvents = models.CalendarEvents
     CarePlan = models.CarePlan
     CarePlanOverview = models.CarePlanOverview
     CDT = models.CDT
+    CDTRecordsExport = models.CDTRecordsExport
     CDTs = models.CDTs
     Chat = models.Chat
     Chats = models.Chats
     DocumentSummaries = models.DocumentSummaries
     DocumentSummary = models.DocumentSummary
     DocumentSummaryFile = models.DocumentSummaryFile
     DocumentSummaryFiles = models.DocumentSummaryFiles
     Email = models.Email
     Emails = models.Emails
     Encounter = models.Encounter
     EncounterDisposition = models.EncounterDisposition
     Encounters = models.Encounters
     Formation = models.Formation
     Patient = models.Patient
-    Patients = models.Patients
     PatientProgram = models.PatientProgram
+    PatientPrograms = models.PatientPrograms
+    Patients = models.Patients
     ProgramPhase = models.ProgramPhase
     ProgramPhases = models.ProgramPhases
-    PatientPrograms = models.PatientPrograms
     Schedules = models.Schedules
     SearchChats = models.SearchChats
     SMS = models.SMS
     SMSes = models.SMSes
     User = models.User
     Users = models.Users
     WorkHours = models.WorkHours
```

### Comparing `welkin-0.1.4/welkin/exceptions.py` & `welkin-0.1.5/welkin/exceptions.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/__init__.py` & `welkin-0.1.5/welkin/models/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     DocumentSummaries,
     DocumentSummary,
     DocumentSummaryFile,
     DocumentSummaryFiles,
 )
 from welkin.models.email import Email, Emails
 from welkin.models.encounter import Encounter, EncounterDisposition, Encounters
+from welkin.models.export import CDTRecordsExport
 from welkin.models.formation import Formation
 from welkin.models.patient import Patient, Patients
 from welkin.models.program import (
     PatientProgram,
     PatientPrograms,
     ProgramPhase,
     ProgramPhases,
@@ -35,33 +36,34 @@
     "AssessmentRecords",
     "Assessments",
     "CalendarEvent",
     "CalendarEvents",
     "CarePlan",
     "CarePlanOverview",
     "CDT",
+    "CDTRecordsExport",
     "CDTs",
     "Chat",
     "Chats",
     "DocumentSummaries",
     "DocumentSummary",
     "DocumentSummaryFile",
     "DocumentSummaryFiles",
     "Email",
     "Emails",
     "Encounter",
     "EncounterDisposition",
     "Encounters",
     "Formation",
     "Patient",
-    "Patients",
     "PatientProgram",
+    "PatientPrograms",
+    "Patients",
     "ProgramPhase",
     "ProgramPhases",
-    "PatientPrograms",
     "Schedules",
     "SearchChats",
     "SMS",
     "SMSes",
     "User",
     "Users",
     "WorkHours",
```

### Comparing `welkin-0.1.4/welkin/models/assessment.py` & `welkin-0.1.5/welkin/models/assessment.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/base.py` & `welkin-0.1.5/welkin/models/base.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/calendar.py` & `welkin-0.1.5/welkin/models/calendar.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/care_plan.py` & `welkin-0.1.5/welkin/models/care_plan.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/cdt.py` & `welkin-0.1.5/welkin/models/cdt.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/chat.py` & `welkin-0.1.5/welkin/models/chat.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/document.py` & `welkin-0.1.5/welkin/models/document.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/email.py` & `welkin-0.1.5/welkin/models/email.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/encounter.py` & `welkin-0.1.5/welkin/models/encounter.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/formation.py` & `welkin-0.1.5/welkin/models/formation.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/patient.py` & `welkin-0.1.5/welkin/models/patient.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/program.py` & `welkin-0.1.5/welkin/models/program.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/sms.py` & `welkin-0.1.5/welkin/models/sms.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/models/user.py` & `welkin-0.1.5/welkin/models/user.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/welkin/pagination.py` & `welkin-0.1.5/welkin/pagination.py`

 * *Files 12% similar despite different names*

```diff
@@ -190,7 +190,23 @@
     def _pre_request(self):
         if self.page_token:
             self.kwargs["params"] = {"pageToken": self.page_token}
 
     def _post_request(self, meta):
         self.page_token = meta["nextPageToken"]
         self.last = not meta.get("nextPageToken")
+
+
+class CursorIterator(PageIterator):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.meta_key = "cursor"
+        self.meta_dict = {
+            "start": None,
+            "end": None,
+            "pageSize": self.size,
+        }
+        self.kwargs.setdefault("params", {}).update(pageSize=self.size)
+
+    def _post_request(self, meta):
+        self.kwargs.setdefault("params", {}).update(start=meta.get("end"))
+        self.last = not meta.get("hasNext")
```

### Comparing `welkin-0.1.4/welkin/util.py` & `welkin-0.1.5/welkin/util.py`

 * *Files identical despite different names*

### Comparing `welkin-0.1.4/PKG-INFO` & `welkin-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: welkin
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python Welkin Health API Wrapper.
 Home-page: https://github.com/lightmatter/welkin-health
 License: GPL-3.0-or-later
 Author: Sam Morgan
 Author-email: sama4mail@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

