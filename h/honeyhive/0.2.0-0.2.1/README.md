# Comparing `tmp/honeyhive-0.2.0-py2.py3-none-any.whl.zip` & `tmp/honeyhive-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,326 +1,85 @@
-Zip file size: 464034 bytes, number of entries: 324
--rw-r--r--  2.0 unx      127 b- defN 24-Apr-30 21:50 honeyhive/__init__.py
--rw-r--r--  2.0 unx    12332 b- defN 24-May-09 19:07 honeyhive/configurations.py
--rw-r--r--  2.0 unx    16224 b- defN 24-May-09 19:07 honeyhive/datapoints.py
--rw-r--r--  2.0 unx    12379 b- defN 24-May-09 19:07 honeyhive/datasets.py
--rw-r--r--  2.0 unx    10110 b- defN 24-May-10 18:03 honeyhive/events.py
--rw-r--r--  2.0 unx    11824 b- defN 24-May-09 19:07 honeyhive/metrics.py
--rw-r--r--  2.0 unx    12244 b- defN 24-May-09 19:07 honeyhive/projects.py
--rw-r--r--  2.0 unx     3604 b- defN 24-May-09 19:07 honeyhive/sdk.py
--rw-r--r--  2.0 unx     1352 b- defN 24-May-10 18:03 honeyhive/sdkconfiguration.py
--rw-r--r--  2.0 unx     6872 b- defN 24-May-10 18:03 honeyhive/session.py
--rw-r--r--  2.0 unx    11992 b- defN 24-May-09 19:07 honeyhive/tools.py
--rw-r--r--  2.0 unx      272 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/__init__.cpython-312.pyc
--rw-r--r--  2.0 unx    15203 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/configurations.cpython-312.pyc
--rw-r--r--  2.0 unx    19510 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/datapoints.cpython-312.pyc
--rw-r--r--  2.0 unx    15380 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/datasets.cpython-312.pyc
--rw-r--r--  2.0 unx    11853 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/events.cpython-312.pyc
--rw-r--r--  2.0 unx    14666 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/metrics.cpython-312.pyc
--rw-r--r--  2.0 unx    15659 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/projects.cpython-312.pyc
--rw-r--r--  2.0 unx     4576 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/sdk.cpython-312.pyc
--rw-r--r--  2.0 unx     2229 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/sdkconfiguration.cpython-312.pyc
--rw-r--r--  2.0 unx    16042 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/session.cpython-312.pyc
--rw-r--r--  2.0 unx    13387 b- defN 24-Apr-30 21:51 honeyhive/__pycache__/tools.cpython-312.pyc
--rw-r--r--  2.0 unx      121 b- defN 24-Apr-30 21:50 honeyhive/_hooks/__init__.py
--rw-r--r--  2.0 unx     2393 b- defN 24-May-02 17:00 honeyhive/_hooks/sdkhooks.py
--rw-r--r--  2.0 unx     2468 b- defN 24-May-02 17:00 honeyhive/_hooks/types.py
--rw-r--r--  2.0 unx      273 b- defN 24-Apr-30 21:51 honeyhive/_hooks/__pycache__/__init__.cpython-312.pyc
--rw-r--r--  2.0 unx     4128 b- defN 24-Apr-30 21:51 honeyhive/_hooks/__pycache__/sdkhooks.cpython-312.pyc
--rw-r--r--  2.0 unx     4790 b- defN 24-Apr-30 21:51 honeyhive/_hooks/__pycache__/types.cpython-312.pyc
--rw-r--r--  2.0 unx       87 b- defN 24-Apr-30 21:50 honeyhive/models/__init__.py
--rw-r--r--  2.0 unx      220 b- defN 24-Apr-30 21:51 honeyhive/models/__pycache__/__init__.cpython-312.pyc
--rw-r--r--  2.0 unx     2166 b- defN 24-May-10 18:03 honeyhive/models/components/__init__.py
--rw-r--r--  2.0 unx     2285 b- defN 23-Nov-16 16:25 honeyhive/models/components/chatcompletionrequest.py
--rw-r--r--  2.0 unx     1769 b- defN 23-Nov-16 16:25 honeyhive/models/components/chatcompletionresponse.py
--rw-r--r--  2.0 unx     5776 b- defN 24-May-09 19:07 honeyhive/models/components/configuration.py
--rw-r--r--  2.0 unx     2383 b- defN 24-May-09 19:07 honeyhive/models/components/createdatapointrequest.py
--rw-r--r--  2.0 unx     2908 b- defN 24-May-09 19:07 honeyhive/models/components/createdatasetrequest.py
--rw-r--r--  2.0 unx     5463 b- defN 24-May-10 18:03 honeyhive/models/components/createeventrequest.py
--rw-r--r--  2.0 unx      643 b- defN 24-May-02 17:00 honeyhive/models/components/createprojectrequest.py
--rw-r--r--  2.0 unx     1265 b- defN 24-May-09 19:07 honeyhive/models/components/createtoolrequest.py
--rw-r--r--  2.0 unx     3789 b- defN 24-May-09 19:07 honeyhive/models/components/datapoint.py
--rw-r--r--  2.0 unx     3544 b- defN 24-May-09 19:07 honeyhive/models/components/dataset.py
--rw-r--r--  2.0 unx     3051 b- defN 23-Nov-16 16:25 honeyhive/models/components/datasetresponse.py
--rw-r--r--  2.0 unx     1782 b- defN 24-May-09 19:07 honeyhive/models/components/datasetupdate.py
--rw-r--r--  2.0 unx      653 b- defN 23-Nov-16 16:25 honeyhive/models/components/deleteresponse.py
--rw-r--r--  2.0 unx     4000 b- defN 23-Nov-16 16:25 honeyhive/models/components/evaluation.py
--rw-r--r--  2.0 unx     3785 b- defN 23-Nov-16 16:25 honeyhive/models/components/evaluationloggingquery.py
--rw-r--r--  2.0 unx     3492 b- defN 23-Nov-16 16:25 honeyhive/models/components/evaluationupdaterequest.py
--rw-r--r--  2.0 unx     5838 b- defN 24-May-09 19:07 honeyhive/models/components/event.py
--rw-r--r--  2.0 unx     1966 b- defN 24-May-10 18:03 honeyhive/models/components/eventfilter.py
--rw-r--r--  2.0 unx     1277 b- defN 23-Nov-16 16:25 honeyhive/models/components/feedbackquery.py
--rw-r--r--  2.0 unx     1750 b- defN 23-Nov-16 16:25 honeyhive/models/components/feedbackresponse.py
--rw-r--r--  2.0 unx     3390 b- defN 23-Nov-16 16:25 honeyhive/models/components/finetunedmodelresponse.py
--rw-r--r--  2.0 unx     3272 b- defN 23-Nov-16 16:25 honeyhive/models/components/generatequery.py
--rw-r--r--  2.0 unx     3185 b- defN 23-Nov-16 16:25 honeyhive/models/components/generation.py
--rw-r--r--  2.0 unx     3802 b- defN 23-Nov-16 16:25 honeyhive/models/components/generationloggingquery.py
--rw-r--r--  2.0 unx     1258 b- defN 23-Nov-16 16:25 honeyhive/models/components/generationresponse.py
--rw-r--r--  2.0 unx     4548 b- defN 24-May-10 18:03 honeyhive/models/components/metric.py
--rw-r--r--  2.0 unx      731 b- defN 23-Nov-16 16:25 honeyhive/models/components/metriccomputerequest.py
--rw-r--r--  2.0 unx      522 b- defN 23-Nov-16 16:25 honeyhive/models/components/metriccomputeresponse.py
--rw-r--r--  2.0 unx     2570 b- defN 23-Nov-16 16:25 honeyhive/models/components/metriccreaterequest.py
--rw-r--r--  2.0 unx      524 b- defN 23-Nov-16 16:25 honeyhive/models/components/metriccreateresponse.py
--rw-r--r--  2.0 unx      522 b- defN 23-Nov-16 16:25 honeyhive/models/components/metricdeleteresponse.py
--rw-r--r--  2.0 unx     4842 b- defN 24-May-09 19:07 honeyhive/models/components/metricedit.py
--rw-r--r--  2.0 unx     3290 b- defN 23-Nov-16 16:25 honeyhive/models/components/metricresponse.py
--rw-r--r--  2.0 unx     2448 b- defN 23-Nov-16 16:25 honeyhive/models/components/metricupdaterequest.py
--rw-r--r--  2.0 unx      522 b- defN 23-Nov-16 16:25 honeyhive/models/components/metricupdateresponse.py
--rw-r--r--  2.0 unx     5365 b- defN 24-May-09 19:07 honeyhive/models/components/postconfigurationrequest.py
--rw-r--r--  2.0 unx      740 b- defN 24-May-09 19:07 honeyhive/models/components/project.py
--rw-r--r--  2.0 unx     2442 b- defN 23-Nov-16 16:25 honeyhive/models/components/promptcreationquery.py
--rw-r--r--  2.0 unx     3146 b- defN 23-Nov-16 16:25 honeyhive/models/components/promptresponse.py
--rw-r--r--  2.0 unx     2042 b- defN 23-Nov-16 16:25 honeyhive/models/components/promptupdatequery.py
--rw-r--r--  2.0 unx     5815 b- defN 24-May-09 19:07 honeyhive/models/components/putconfigurationrequest.py
--rw-r--r--  2.0 unx      330 b- defN 24-Apr-30 21:50 honeyhive/models/components/security.py
--rw-r--r--  2.0 unx      834 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessionendresponse.py
--rw-r--r--  2.0 unx     4299 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessioneventquery.py
--rw-r--r--  2.0 unx      856 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessioneventresponse.py
--rw-r--r--  2.0 unx     2286 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessioneventupdate.py
--rw-r--r--  2.0 unx      889 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessionfeedback.py
--rw-r--r--  2.0 unx     1524 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessionstartquery.py
--rw-r--r--  2.0 unx     4099 b- defN 24-May-09 19:07 honeyhive/models/components/sessionstartrequest.py
--rw-r--r--  2.0 unx      853 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessionstartresponse.py
--rw-r--r--  2.0 unx      675 b- defN 23-Nov-16 16:25 honeyhive/models/components/sessiontrace.py
--rw-r--r--  2.0 unx      849 b- defN 23-Nov-16 16:25 honeyhive/models/components/successresponse.py
--rw-r--r--  2.0 unx      872 b- defN 23-Nov-16 16:25 honeyhive/models/components/successtraceresponse.py
--rw-r--r--  2.0 unx     2871 b- defN 23-Nov-16 16:25 honeyhive/models/components/taskcreationquery.py
--rw-r--r--  2.0 unx     3212 b- defN 23-Nov-16 16:25 honeyhive/models/components/taskresponse.py
--rw-r--r--  2.0 unx     2192 b- defN 23-Nov-16 16:25 honeyhive/models/components/taskupdatequery.py
--rw-r--r--  2.0 unx     1493 b- defN 23-Nov-16 16:25 honeyhive/models/components/taskupdateresponse.py
--rw-r--r--  2.0 unx     1403 b- defN 24-May-09 19:07 honeyhive/models/components/tool.py
--rw-r--r--  2.0 unx     1060 b- defN 24-Apr-30 21:05 honeyhive/models/components/toolupdate.py
--rw-r--r--  2.0 unx     1516 b- defN 23-Nov-16 16:25 honeyhive/models/components/traceevent.py
--rw-r--r--  2.0 unx     2426 b- defN 24-May-09 19:07 honeyhive/models/components/updatedatapointrequest.py
--rw-r--r--  2.0 unx      825 b- defN 24-May-09 19:07 honeyhive/models/components/updateprojectrequest.py
--rw-r--r--  2.0 unx      681 b- defN 23-Nov-16 16:25 honeyhive/models/components/updateresponse.py
--rw-r--r--  2.0 unx      898 b- defN 24-May-02 17:00 honeyhive/models/components/updatetoolrequest.py
--rw-r--r--  2.0 unx     1673 b- defN 23-Nov-16 16:25 honeyhive/models/components/uploaddataset.py
--rw-r--r--  2.0 unx     2060 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/__init__.cpython-312.pyc
--rw-r--r--  2.0 unx     4009 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/chatcompletionrequest.cpython-312.pyc
--rw-r--r--  2.0 unx     3729 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/chatcompletionresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     7768 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/configuration.cpython-312.pyc
--rw-r--r--  2.0 unx     4622 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/createdatapointrequest.cpython-312.pyc
--rw-r--r--  2.0 unx     4739 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/createdatasetrequest.cpython-312.pyc
--rw-r--r--  2.0 unx     8375 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/createeventrequest.cpython-312.pyc
--rw-r--r--  2.0 unx     2077 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/createprojectrequest.cpython-312.pyc
--rw-r--r--  2.0 unx     6415 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/datapoint.cpython-312.pyc
--rw-r--r--  2.0 unx     5341 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/dataset.cpython-312.pyc
--rw-r--r--  2.0 unx     5068 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/datasetresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     3777 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/datasetupdate.cpython-312.pyc
--rw-r--r--  2.0 unx     1496 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/deleteresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     6175 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/evaluation.cpython-312.pyc
--rw-r--r--  2.0 unx     5818 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/evaluationloggingquery.cpython-312.pyc
--rw-r--r--  2.0 unx     5410 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/evaluationupdaterequest.cpython-312.pyc
--rw-r--r--  2.0 unx     9401 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/event.cpython-312.pyc
--rw-r--r--  2.0 unx     2054 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/feedbackquery.cpython-312.pyc
--rw-r--r--  2.0 unx     3033 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/feedbackresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     5443 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/finetunedmodelresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     5020 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/generatequery.cpython-312.pyc
--rw-r--r--  2.0 unx     4974 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/generation.cpython-312.pyc
--rw-r--r--  2.0 unx     6038 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/generationloggingquery.cpython-312.pyc
--rw-r--r--  2.0 unx     2350 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/generationresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     6310 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/metric.cpython-312.pyc
--rw-r--r--  2.0 unx     1662 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/metriccomputerequest.cpython-312.pyc
--rw-r--r--  2.0 unx     1269 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/metriccomputeresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     5069 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/metriccreaterequest.cpython-312.pyc
--rw-r--r--  2.0 unx     1267 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/metriccreateresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     1266 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/metricdeleteresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     7330 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/metricedit.cpython-312.pyc
--rw-r--r--  2.0 unx     4554 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/metricresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     4884 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/metricupdaterequest.cpython-312.pyc
--rw-r--r--  2.0 unx     1266 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/metricupdateresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     1940 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/project.cpython-312.pyc
--rw-r--r--  2.0 unx     4083 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/promptcreationquery.cpython-312.pyc
--rw-r--r--  2.0 unx     5041 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/promptresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     3492 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/promptupdatequery.cpython-312.pyc
--rw-r--r--  2.0 unx      805 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/security.cpython-312.pyc
--rw-r--r--  2.0 unx     1651 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/sessionendresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     6788 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/sessioneventquery.cpython-312.pyc
--rw-r--r--  2.0 unx     1689 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/sessioneventresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     4238 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/sessioneventupdate.cpython-312.pyc
--rw-r--r--  2.0 unx     1717 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/sessionfeedback.cpython-312.pyc
--rw-r--r--  2.0 unx     2729 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/sessionstartquery.cpython-312.pyc
--rw-r--r--  2.0 unx     8053 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/sessionstartrequest.cpython-312.pyc
--rw-r--r--  2.0 unx     1643 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/sessionstartresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     1396 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/sessiontrace.cpython-312.pyc
--rw-r--r--  2.0 unx     1658 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/successresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     1707 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/successtraceresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     4813 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/taskcreationquery.cpython-312.pyc
--rw-r--r--  2.0 unx     5142 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/taskresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     3663 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/taskupdatequery.cpython-312.pyc
--rw-r--r--  2.0 unx     2543 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/taskupdateresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     2714 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/tool.cpython-312.pyc
--rw-r--r--  2.0 unx     2294 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/toolupdate.cpython-312.pyc
--rw-r--r--  2.0 unx     2390 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/traceevent.cpython-312.pyc
--rw-r--r--  2.0 unx     4701 b- defN 24-Apr-30 21:51 honeyhive/models/components/__pycache__/updatedatapointrequest.cpython-312.pyc
--rw-r--r--  2.0 unx     1528 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/updateresponse.cpython-312.pyc
--rw-r--r--  2.0 unx     2978 b- defN 24-Apr-30 20:12 honeyhive/models/components/__pycache__/uploaddataset.cpython-312.pyc
--rw-r--r--  2.0 unx      124 b- defN 24-Apr-30 21:50 honeyhive/models/errors/__init__.py
--rw-r--r--  2.0 unx      700 b- defN 24-Apr-30 21:50 honeyhive/models/errors/sdkerror.py
--rw-r--r--  2.0 unx      292 b- defN 24-Apr-30 21:51 honeyhive/models/errors/__pycache__/__init__.cpython-312.pyc
--rw-r--r--  2.0 unx     1368 b- defN 24-Apr-30 21:51 honeyhive/models/errors/__pycache__/sdkerror.cpython-312.pyc
--rw-r--r--  2.0 unx     2512 b- defN 24-May-10 18:03 honeyhive/models/operations/__init__.py
--rw-r--r--  2.0 unx      559 b- defN 24-Apr-30 21:50 honeyhive/models/operations/createconfiguration.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-09 19:07 honeyhive/models/operations/createdatapoint.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-09 19:07 honeyhive/models/operations/createdataset.py
--rw-r--r--  2.0 unx     1662 b- defN 24-May-02 17:00 honeyhive/models/operations/createevent.py
--rw-r--r--  2.0 unx      552 b- defN 24-May-02 17:00 honeyhive/models/operations/createmetric.py
--rw-r--r--  2.0 unx      759 b- defN 24-Apr-30 21:50 honeyhive/models/operations/createproject.py
--rw-r--r--  2.0 unx     1370 b- defN 24-May-09 19:07 honeyhive/models/operations/createtool.py
--rw-r--r--  2.0 unx      808 b- defN 24-Apr-30 21:05 honeyhive/models/operations/delete_datasets.py
--rw-r--r--  2.0 unx      969 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_datasets_name_.py
--rw-r--r--  2.0 unx      967 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_evaluations_id_.py
--rw-r--r--  2.0 unx      880 b- defN 24-Apr-30 21:05 honeyhive/models/operations/delete_events_event_id_.py
--rw-r--r--  2.0 unx      750 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_fine_tuned_models_id_.py
--rw-r--r--  2.0 unx      742 b- defN 24-Apr-30 21:05 honeyhive/models/operations/delete_metrics.py
--rw-r--r--  2.0 unx      959 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_prompts_id_.py
--rw-r--r--  2.0 unx      994 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_session_session_id_.py
--rw-r--r--  2.0 unx      953 b- defN 23-Nov-16 16:25 honeyhive/models/operations/delete_tasks.py
--rw-r--r--  2.0 unx      802 b- defN 24-May-09 19:07 honeyhive/models/operations/deleteconfiguration.py
--rw-r--r--  2.0 unx     1357 b- defN 24-May-09 19:07 honeyhive/models/operations/deletedatapoint.py
--rw-r--r--  2.0 unx      838 b- defN 24-May-09 19:07 honeyhive/models/operations/deletedataset.py
--rw-r--r--  2.0 unx      864 b- defN 24-May-02 17:00 honeyhive/models/operations/deleteevent.py
--rw-r--r--  2.0 unx      740 b- defN 24-May-02 17:00 honeyhive/models/operations/deletemetric.py
--rw-r--r--  2.0 unx      732 b- defN 24-Apr-30 21:50 honeyhive/models/operations/deleteproject.py
--rw-r--r--  2.0 unx      746 b- defN 24-Apr-30 21:50 honeyhive/models/operations/deletesession.py
--rw-r--r--  2.0 unx      740 b- defN 24-Apr-30 21:50 honeyhive/models/operations/deletetool.py
--rw-r--r--  2.0 unx     2076 b- defN 24-Apr-30 21:05 honeyhive/models/operations/get_datasets.py
--rw-r--r--  2.0 unx      767 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_evaluations.py
--rw-r--r--  2.0 unx      940 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_evaluations_id_.py
--rw-r--r--  2.0 unx     1179 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_fine_tuned_models.py
--rw-r--r--  2.0 unx     1011 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_fine_tuned_models_id_.py
--rw-r--r--  2.0 unx     1271 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_generations.py
--rw-r--r--  2.0 unx     1002 b- defN 24-Apr-30 21:05 honeyhive/models/operations/get_metrics.py
--rw-r--r--  2.0 unx     1123 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_prompts.py
--rw-r--r--  2.0 unx     1450 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_session.py
--rw-r--r--  2.0 unx      999 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_session_session_id_.py
--rw-r--r--  2.0 unx      993 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_session_session_id_export.py
--rw-r--r--  2.0 unx      967 b- defN 23-Nov-16 16:25 honeyhive/models/operations/get_tasks.py
--rw-r--r--  2.0 unx     2080 b- defN 24-May-09 19:07 honeyhive/models/operations/getconfigurations.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-09 19:07 honeyhive/models/operations/getdatapoint.py
--rw-r--r--  2.0 unx     1990 b- defN 24-May-09 19:07 honeyhive/models/operations/getdatapoints.py
--rw-r--r--  2.0 unx     2120 b- defN 24-May-09 19:07 honeyhive/models/operations/getdatasets.py
--rw-r--r--  2.0 unx     3208 b- defN 24-May-10 18:03 honeyhive/models/operations/getevents.py
--rw-r--r--  2.0 unx     1002 b- defN 24-May-02 17:00 honeyhive/models/operations/getmetrics.py
--rw-r--r--  2.0 unx      970 b- defN 24-Apr-30 21:50 honeyhive/models/operations/getprojects.py
--rw-r--r--  2.0 unx      932 b- defN 24-Apr-30 21:50 honeyhive/models/operations/getsession.py
--rw-r--r--  2.0 unx      773 b- defN 24-May-02 17:00 honeyhive/models/operations/gettools.py
--rw-r--r--  2.0 unx      814 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_chat.py
--rw-r--r--  2.0 unx     1567 b- defN 24-Apr-30 21:05 honeyhive/models/operations/post_datasets.py
--rw-r--r--  2.0 unx      785 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_evaluations.py
--rw-r--r--  2.0 unx     1658 b- defN 24-Apr-30 21:05 honeyhive/models/operations/post_events.py
--rw-r--r--  2.0 unx      787 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_feedback.py
--rw-r--r--  2.0 unx     1907 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_fine_tuned_models.py
--rw-r--r--  2.0 unx      800 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_generations.py
--rw-r--r--  2.0 unx      803 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_generations_log.py
--rw-r--r--  2.0 unx      551 b- defN 24-Apr-30 21:05 honeyhive/models/operations/post_metrics.py
--rw-r--r--  2.0 unx      819 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_metrics_compute.py
--rw-r--r--  2.0 unx      776 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_prompts.py
--rw-r--r--  2.0 unx     1012 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_session_id_end.py
--rw-r--r--  2.0 unx     1261 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_session_id_event.py
--rw-r--r--  2.0 unx     1230 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_session_id_feedback.py
--rw-r--r--  2.0 unx     1237 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_session_id_traces.py
--rw-r--r--  2.0 unx      812 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_session_start.py
--rw-r--r--  2.0 unx      764 b- defN 23-Nov-16 16:25 honeyhive/models/operations/post_tasks.py
--rw-r--r--  2.0 unx     1974 b- defN 24-May-07 15:08 honeyhive/models/operations/processeventtrace.py
--rw-r--r--  2.0 unx      551 b- defN 24-Apr-30 21:05 honeyhive/models/operations/put_datasets.py
--rw-r--r--  2.0 unx     1250 b- defN 23-Nov-16 16:25 honeyhive/models/operations/put_evaluations_id_.py
--rw-r--r--  2.0 unx     1810 b- defN 24-Apr-30 21:05 honeyhive/models/operations/put_events.py
--rw-r--r--  2.0 unx      550 b- defN 24-Apr-30 21:05 honeyhive/models/operations/put_metrics.py
--rw-r--r--  2.0 unx     1188 b- defN 23-Nov-16 16:25 honeyhive/models/operations/put_prompts_id_.py
--rw-r--r--  2.0 unx     1252 b- defN 23-Nov-16 16:25 honeyhive/models/operations/put_session_session_id_.py
--rw-r--r--  2.0 unx      794 b- defN 23-Nov-16 16:25 honeyhive/models/operations/put_tasks.py
--rw-r--r--  2.0 unx     1531 b- defN 24-Apr-30 21:50 honeyhive/models/operations/startsession.py
--rw-r--r--  2.0 unx     1067 b- defN 24-May-09 19:07 honeyhive/models/operations/updateconfiguration.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-09 19:07 honeyhive/models/operations/updatedatapoint.py
--rw-r--r--  2.0 unx      553 b- defN 24-May-02 17:00 honeyhive/models/operations/updatedataset.py
--rw-r--r--  2.0 unx     1653 b- defN 24-May-09 19:07 honeyhive/models/operations/updateevent.py
--rw-r--r--  2.0 unx      552 b- defN 24-May-02 17:00 honeyhive/models/operations/updatemetric.py
--rw-r--r--  2.0 unx      553 b- defN 24-May-02 17:00 honeyhive/models/operations/updateproject.py
--rw-r--r--  2.0 unx      550 b- defN 24-May-02 17:00 honeyhive/models/operations/updatetool.py
--rw-r--r--  2.0 unx     2784 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/__init__.cpython-312.pyc
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/createconfiguration.cpython-312.pyc
--rw-r--r--  2.0 unx     2685 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/createdatapoint.cpython-312.pyc
--rw-r--r--  2.0 unx     1174 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/createproject.cpython-312.pyc
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/createtool.cpython-312.pyc
--rw-r--r--  2.0 unx     1357 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/delete_datasets.cpython-312.pyc
--rw-r--r--  2.0 unx     1641 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/delete_datasets_name_.cpython-312.pyc
--rw-r--r--  2.0 unx     1642 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/delete_evaluations_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/delete_events_event_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     1364 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/delete_fine_tuned_models_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     1349 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/delete_metrics.cpython-312.pyc
--rw-r--r--  2.0 unx     1630 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/delete_prompts_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     1684 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/delete_session_session_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     1617 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/delete_tasks.cpython-312.pyc
--rw-r--r--  2.0 unx     1350 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/deleteconfiguration.cpython-312.pyc
--rw-r--r--  2.0 unx     1338 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/deletedatapoint.cpython-312.pyc
--rw-r--r--  2.0 unx     1333 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/deleteproject.cpython-312.pyc
--rw-r--r--  2.0 unx     1358 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/deletesession.cpython-312.pyc
--rw-r--r--  2.0 unx     1349 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/deletetool.cpython-312.pyc
--rw-r--r--  2.0 unx     3220 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/get_datasets.cpython-312.pyc
--rw-r--r--  2.0 unx     1215 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_evaluations.cpython-312.pyc
--rw-r--r--  2.0 unx     1605 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_evaluations_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     1863 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_fine_tuned_models.cpython-312.pyc
--rw-r--r--  2.0 unx     1702 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_fine_tuned_models_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     1933 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_generations.cpython-312.pyc
--rw-r--r--  2.0 unx     1621 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/get_metrics.cpython-312.pyc
--rw-r--r--  2.0 unx     1796 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_prompts.cpython-312.pyc
--rw-r--r--  2.0 unx     2037 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_session.cpython-312.pyc
--rw-r--r--  2.0 unx     1687 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_session_session_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     1695 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_session_session_id_export.cpython-312.pyc
--rw-r--r--  2.0 unx     1651 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/get_tasks.cpython-312.pyc
--rw-r--r--  2.0 unx     2097 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/getconfigurations.cpython-312.pyc
--rw-r--r--  2.0 unx     1586 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/getdatapoint.cpython-312.pyc
--rw-r--r--  2.0 unx     3209 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/getdatapoints.cpython-312.pyc
--rw-r--r--  2.0 unx     1640 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/getprojects.cpython-312.pyc
--rw-r--r--  2.0 unx     1589 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/getsession.cpython-312.pyc
--rw-r--r--  2.0 unx     1635 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/gettools.cpython-312.pyc
--rw-r--r--  2.0 unx     1260 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_chat.cpython-312.pyc
--rw-r--r--  2.0 unx     3053 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/post_datasets.cpython-312.pyc
--rw-r--r--  2.0 unx     1226 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_evaluations.cpython-312.pyc
--rw-r--r--  2.0 unx     3163 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/post_events.cpython-312.pyc
--rw-r--r--  2.0 unx     1226 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_feedback.cpython-312.pyc
--rw-r--r--  2.0 unx     3708 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_fine_tuned_models.cpython-312.pyc
--rw-r--r--  2.0 unx     1242 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_generations.cpython-312.pyc
--rw-r--r--  2.0 unx     1249 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_generations_log.cpython-312.pyc
--rw-r--r--  2.0 unx      923 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/post_metrics.cpython-312.pyc
--rw-r--r--  2.0 unx     1265 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_metrics_compute.cpython-312.pyc
--rw-r--r--  2.0 unx     1212 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_prompts.cpython-312.pyc
--rw-r--r--  2.0 unx     1704 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_session_session_id_end.cpython-312.pyc
--rw-r--r--  2.0 unx     2017 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_session_session_id_event.cpython-312.pyc
--rw-r--r--  2.0 unx     1988 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_session_session_id_feedback.cpython-312.pyc
--rw-r--r--  2.0 unx     1992 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_session_session_id_traces.cpython-312.pyc
--rw-r--r--  2.0 unx     1256 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_session_start.cpython-312.pyc
--rw-r--r--  2.0 unx     1198 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/post_tasks.cpython-312.pyc
--rw-r--r--  2.0 unx     3370 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/processeventtrace.cpython-312.pyc
--rw-r--r--  2.0 unx      923 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/put_datasets.cpython-312.pyc
--rw-r--r--  2.0 unx     2000 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/put_evaluations_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     3770 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/put_events.cpython-312.pyc
--rw-r--r--  2.0 unx      921 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/put_metrics.cpython-312.pyc
--rw-r--r--  2.0 unx     1918 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/put_prompts_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     2013 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/put_session_session_id_.cpython-312.pyc
--rw-r--r--  2.0 unx     1229 b- defN 24-Apr-30 20:12 honeyhive/models/operations/__pycache__/put_tasks.cpython-312.pyc
--rw-r--r--  2.0 unx     2845 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/startsession.cpython-312.pyc
--rw-r--r--  2.0 unx     1642 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/updateconfiguration.cpython-312.pyc
--rw-r--r--  2.0 unx     1721 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/updatedatapoint.cpython-312.pyc
--rw-r--r--  2.0 unx     1174 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/updateproject.cpython-312.pyc
--rw-r--r--  2.0 unx     1382 b- defN 24-Apr-30 21:51 honeyhive/models/operations/__pycache__/updatetool.cpython-312.pyc
--rw-r--r--  2.0 unx      120 b- defN 24-Apr-30 21:50 honeyhive/utils/__init__.py
--rw-r--r--  2.0 unx    37934 b- defN 24-May-09 19:07 honeyhive/utils/langchain_tracer.py
--rw-r--r--  2.0 unx    30426 b- defN 24-May-01 20:36 honeyhive/utils/llamaindex_tracer.py
--rw-r--r--  2.0 unx     3732 b- defN 24-May-02 17:00 honeyhive/utils/retries.py
--rw-r--r--  2.0 unx    25540 b- defN 24-Apr-22 20:04 honeyhive/utils/tracer.py
--rw-r--r--  2.0 unx    32651 b- defN 24-May-09 19:07 honeyhive/utils/utils.py
--rw-r--r--  2.0 unx      271 b- defN 24-Apr-30 21:51 honeyhive/utils/__pycache__/__init__.cpython-312.pyc
--rw-r--r--  2.0 unx    39632 b- defN 24-Apr-30 21:51 honeyhive/utils/__pycache__/langchain_tracer.cpython-312.pyc
--rw-r--r--  2.0 unx    32704 b- defN 24-Apr-30 21:51 honeyhive/utils/__pycache__/llamaindex_tracer.cpython-312.pyc
--rw-r--r--  2.0 unx     5750 b- defN 24-Apr-30 21:51 honeyhive/utils/__pycache__/retries.cpython-312.pyc
--rw-r--r--  2.0 unx    27841 b- defN 24-Apr-30 20:12 honeyhive/utils/__pycache__/tracer.cpython-312.pyc
--rw-r--r--  2.0 unx    36368 b- defN 24-Apr-30 21:51 honeyhive/utils/__pycache__/utils.cpython-312.pyc
--rw-r--r--  2.0 unx     1067 b- defN 24-May-10 18:04 honeyhive-0.2.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    13807 b- defN 24-May-10 18:04 honeyhive-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-May-10 18:04 honeyhive-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 24-May-10 18:04 honeyhive-0.2.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-May-10 18:04 honeyhive-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    36207 b- defN 24-May-10 18:04 honeyhive-0.2.0.dist-info/RECORD
-324 files, 1159532 bytes uncompressed, 403680 bytes compressed:  65.2%
+Zip file size: 91073 bytes, number of entries: 83
+-rw-r--r--  2.0 unx      127 b- defN 24-May-16 21:04 honeyhive/__init__.py
+-rw-r--r--  2.0 unx    11848 b- defN 24-May-16 21:53 honeyhive/configurations.py
+-rw-r--r--  2.0 unx    15611 b- defN 24-May-16 21:53 honeyhive/datapoints.py
+-rw-r--r--  2.0 unx    11862 b- defN 24-May-16 21:53 honeyhive/datasets.py
+-rw-r--r--  2.0 unx     9650 b- defN 24-May-16 21:53 honeyhive/events.py
+-rw-r--r--  2.0 unx    11379 b- defN 24-May-16 21:53 honeyhive/metrics.py
+-rw-r--r--  2.0 unx    11750 b- defN 24-May-16 21:53 honeyhive/projects.py
+-rw-r--r--  2.0 unx     3560 b- defN 24-May-16 21:53 honeyhive/sdk.py
+-rw-r--r--  2.0 unx     1239 b- defN 24-May-16 21:53 honeyhive/sdkconfiguration.py
+-rw-r--r--  2.0 unx     6540 b- defN 24-May-16 21:53 honeyhive/session.py
+-rw-r--r--  2.0 unx    11464 b- defN 24-May-16 21:53 honeyhive/tools.py
+-rw-r--r--  2.0 unx      121 b- defN 24-May-16 21:04 honeyhive/_hooks/__init__.py
+-rw-r--r--  2.0 unx     2392 b- defN 24-May-16 21:53 honeyhive/_hooks/sdkhooks.py
+-rw-r--r--  2.0 unx     2069 b- defN 24-May-16 21:53 honeyhive/_hooks/types.py
+-rw-r--r--  2.0 unx       87 b- defN 24-May-16 21:04 honeyhive/models/__init__.py
+-rw-r--r--  2.0 unx     2137 b- defN 24-May-16 21:53 honeyhive/models/components/__init__.py
+-rw-r--r--  2.0 unx     5776 b- defN 24-May-16 21:04 honeyhive/models/components/configuration.py
+-rw-r--r--  2.0 unx     2013 b- defN 24-May-16 21:53 honeyhive/models/components/createdatapointrequest.py
+-rw-r--r--  2.0 unx     2908 b- defN 24-May-16 21:04 honeyhive/models/components/createdatasetrequest.py
+-rw-r--r--  2.0 unx     5463 b- defN 24-May-16 21:04 honeyhive/models/components/createeventrequest.py
+-rw-r--r--  2.0 unx      643 b- defN 24-May-16 21:04 honeyhive/models/components/createprojectrequest.py
+-rw-r--r--  2.0 unx     1265 b- defN 24-May-16 21:04 honeyhive/models/components/createtoolrequest.py
+-rw-r--r--  2.0 unx     3789 b- defN 24-May-16 21:04 honeyhive/models/components/datapoint.py
+-rw-r--r--  2.0 unx     3544 b- defN 24-May-16 21:04 honeyhive/models/components/dataset.py
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-16 21:04 honeyhive/models/components/datasetupdate.py
+-rw-r--r--  2.0 unx     5838 b- defN 24-May-16 21:04 honeyhive/models/components/event.py
+-rw-r--r--  2.0 unx     1966 b- defN 24-May-16 21:04 honeyhive/models/components/eventfilter.py
+-rw-r--r--  2.0 unx     4548 b- defN 24-May-16 21:04 honeyhive/models/components/metric.py
+-rw-r--r--  2.0 unx     4842 b- defN 24-May-16 21:04 honeyhive/models/components/metricedit.py
+-rw-r--r--  2.0 unx     5365 b- defN 24-May-16 21:04 honeyhive/models/components/postconfigurationrequest.py
+-rw-r--r--  2.0 unx      740 b- defN 24-May-16 21:04 honeyhive/models/components/project.py
+-rw-r--r--  2.0 unx     5815 b- defN 24-May-16 21:04 honeyhive/models/components/putconfigurationrequest.py
+-rw-r--r--  2.0 unx      330 b- defN 24-May-16 21:04 honeyhive/models/components/security.py
+-rw-r--r--  2.0 unx     4099 b- defN 24-May-16 21:04 honeyhive/models/components/sessionstartrequest.py
+-rw-r--r--  2.0 unx     1403 b- defN 24-May-16 21:04 honeyhive/models/components/tool.py
+-rw-r--r--  2.0 unx     1969 b- defN 24-May-16 21:53 honeyhive/models/components/updatedatapointrequest.py
+-rw-r--r--  2.0 unx      825 b- defN 24-May-16 21:04 honeyhive/models/components/updateprojectrequest.py
+-rw-r--r--  2.0 unx      898 b- defN 24-May-16 21:04 honeyhive/models/components/updatetoolrequest.py
+-rw-r--r--  2.0 unx      124 b- defN 24-May-16 21:04 honeyhive/models/errors/__init__.py
+-rw-r--r--  2.0 unx      700 b- defN 24-May-16 21:04 honeyhive/models/errors/sdkerror.py
+-rw-r--r--  2.0 unx     2461 b- defN 24-May-16 21:53 honeyhive/models/operations/__init__.py
+-rw-r--r--  2.0 unx      559 b- defN 24-May-16 21:04 honeyhive/models/operations/createconfiguration.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-16 21:04 honeyhive/models/operations/createdatapoint.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-16 21:04 honeyhive/models/operations/createdataset.py
+-rw-r--r--  2.0 unx     1662 b- defN 24-May-16 21:04 honeyhive/models/operations/createevent.py
+-rw-r--r--  2.0 unx      552 b- defN 24-May-16 21:04 honeyhive/models/operations/createmetric.py
+-rw-r--r--  2.0 unx      759 b- defN 24-May-16 21:04 honeyhive/models/operations/createproject.py
+-rw-r--r--  2.0 unx     1370 b- defN 24-May-16 21:04 honeyhive/models/operations/createtool.py
+-rw-r--r--  2.0 unx      802 b- defN 24-May-16 21:04 honeyhive/models/operations/deleteconfiguration.py
+-rw-r--r--  2.0 unx     1357 b- defN 24-May-16 21:04 honeyhive/models/operations/deletedatapoint.py
+-rw-r--r--  2.0 unx      838 b- defN 24-May-16 21:04 honeyhive/models/operations/deletedataset.py
+-rw-r--r--  2.0 unx      740 b- defN 24-May-16 21:04 honeyhive/models/operations/deletemetric.py
+-rw-r--r--  2.0 unx      732 b- defN 24-May-16 21:04 honeyhive/models/operations/deleteproject.py
+-rw-r--r--  2.0 unx      740 b- defN 24-May-16 21:04 honeyhive/models/operations/deletetool.py
+-rw-r--r--  2.0 unx     1647 b- defN 24-May-16 21:53 honeyhive/models/operations/getconfigurations.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-16 21:04 honeyhive/models/operations/getdatapoint.py
+-rw-r--r--  2.0 unx     1857 b- defN 24-May-16 21:53 honeyhive/models/operations/getdatapoints.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-16 21:53 honeyhive/models/operations/getdatasets.py
+-rw-r--r--  2.0 unx     3208 b- defN 24-May-16 21:04 honeyhive/models/operations/getevents.py
+-rw-r--r--  2.0 unx     1002 b- defN 24-May-16 21:04 honeyhive/models/operations/getmetrics.py
+-rw-r--r--  2.0 unx      970 b- defN 24-May-16 21:04 honeyhive/models/operations/getprojects.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-16 21:04 honeyhive/models/operations/getsession.py
+-rw-r--r--  2.0 unx      773 b- defN 24-May-16 21:04 honeyhive/models/operations/gettools.py
+-rw-r--r--  2.0 unx     1531 b- defN 24-May-16 21:04 honeyhive/models/operations/startsession.py
+-rw-r--r--  2.0 unx     1067 b- defN 24-May-16 21:04 honeyhive/models/operations/updateconfiguration.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-16 21:04 honeyhive/models/operations/updatedatapoint.py
+-rw-r--r--  2.0 unx      553 b- defN 24-May-16 21:04 honeyhive/models/operations/updatedataset.py
+-rw-r--r--  2.0 unx     1653 b- defN 24-May-16 21:04 honeyhive/models/operations/updateevent.py
+-rw-r--r--  2.0 unx      552 b- defN 24-May-16 21:04 honeyhive/models/operations/updatemetric.py
+-rw-r--r--  2.0 unx      553 b- defN 24-May-16 21:04 honeyhive/models/operations/updateproject.py
+-rw-r--r--  2.0 unx      550 b- defN 24-May-16 21:04 honeyhive/models/operations/updatetool.py
+-rw-r--r--  2.0 unx      120 b- defN 24-May-16 21:04 honeyhive/utils/__init__.py
+-rw-r--r--  2.0 unx    38042 b- defN 24-May-15 18:02 honeyhive/utils/langchain_tracer.py
+-rw-r--r--  2.0 unx    30634 b- defN 24-May-15 18:02 honeyhive/utils/llamaindex_tracer.py
+-rw-r--r--  2.0 unx     3778 b- defN 24-May-16 21:53 honeyhive/utils/retries.py
+-rw-r--r--  2.0 unx    25642 b- defN 24-May-16 20:33 honeyhive/utils/tracer.py
+-rw-r--r--  2.0 unx    29904 b- defN 24-May-16 21:53 honeyhive/utils/utils.py
+-rw-r--r--  2.0 unx     1067 b- defN 24-May-16 21:55 honeyhive-0.2.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    13823 b- defN 24-May-16 21:55 honeyhive-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 21:55 honeyhive-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 24-May-16 21:55 honeyhive-0.2.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-May-16 21:55 honeyhive-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7842 b- defN 24-May-16 21:55 honeyhive-0.2.1.dist-info/RECORD
+83 files, 356509 bytes uncompressed, 78369 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -27,80 +27,29 @@
 
 Filename: honeyhive/session.py
 Comment: 
 
 Filename: honeyhive/tools.py
 Comment: 
 
-Filename: honeyhive/__pycache__/__init__.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/configurations.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/datapoints.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/datasets.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/events.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/metrics.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/projects.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/sdk.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/sdkconfiguration.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/session.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/__pycache__/tools.cpython-312.pyc
-Comment: 
-
 Filename: honeyhive/_hooks/__init__.py
 Comment: 
 
 Filename: honeyhive/_hooks/sdkhooks.py
 Comment: 
 
 Filename: honeyhive/_hooks/types.py
 Comment: 
 
-Filename: honeyhive/_hooks/__pycache__/__init__.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/_hooks/__pycache__/sdkhooks.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/_hooks/__pycache__/types.cpython-312.pyc
-Comment: 
-
 Filename: honeyhive/models/__init__.py
 Comment: 
 
-Filename: honeyhive/models/__pycache__/__init__.cpython-312.pyc
-Comment: 
-
 Filename: honeyhive/models/components/__init__.py
 Comment: 
 
-Filename: honeyhive/models/components/chatcompletionrequest.py
-Comment: 
-
-Filename: honeyhive/models/components/chatcompletionresponse.py
-Comment: 
-
 Filename: honeyhive/models/components/configuration.py
 Comment: 
 
 Filename: honeyhive/models/components/createdatapointrequest.py
 Comment: 
 
 Filename: honeyhive/models/components/createdatasetrequest.py
@@ -117,371 +66,62 @@
 
 Filename: honeyhive/models/components/datapoint.py
 Comment: 
 
 Filename: honeyhive/models/components/dataset.py
 Comment: 
 
-Filename: honeyhive/models/components/datasetresponse.py
-Comment: 
-
 Filename: honeyhive/models/components/datasetupdate.py
 Comment: 
 
-Filename: honeyhive/models/components/deleteresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/evaluation.py
-Comment: 
-
-Filename: honeyhive/models/components/evaluationloggingquery.py
-Comment: 
-
-Filename: honeyhive/models/components/evaluationupdaterequest.py
-Comment: 
-
 Filename: honeyhive/models/components/event.py
 Comment: 
 
 Filename: honeyhive/models/components/eventfilter.py
 Comment: 
 
-Filename: honeyhive/models/components/feedbackquery.py
-Comment: 
-
-Filename: honeyhive/models/components/feedbackresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/finetunedmodelresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/generatequery.py
-Comment: 
-
-Filename: honeyhive/models/components/generation.py
-Comment: 
-
-Filename: honeyhive/models/components/generationloggingquery.py
-Comment: 
-
-Filename: honeyhive/models/components/generationresponse.py
-Comment: 
-
 Filename: honeyhive/models/components/metric.py
 Comment: 
 
-Filename: honeyhive/models/components/metriccomputerequest.py
-Comment: 
-
-Filename: honeyhive/models/components/metriccomputeresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/metriccreaterequest.py
-Comment: 
-
-Filename: honeyhive/models/components/metriccreateresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/metricdeleteresponse.py
-Comment: 
-
 Filename: honeyhive/models/components/metricedit.py
 Comment: 
 
-Filename: honeyhive/models/components/metricresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/metricupdaterequest.py
-Comment: 
-
-Filename: honeyhive/models/components/metricupdateresponse.py
-Comment: 
-
 Filename: honeyhive/models/components/postconfigurationrequest.py
 Comment: 
 
 Filename: honeyhive/models/components/project.py
 Comment: 
 
-Filename: honeyhive/models/components/promptcreationquery.py
-Comment: 
-
-Filename: honeyhive/models/components/promptresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/promptupdatequery.py
-Comment: 
-
 Filename: honeyhive/models/components/putconfigurationrequest.py
 Comment: 
 
 Filename: honeyhive/models/components/security.py
 Comment: 
 
-Filename: honeyhive/models/components/sessionendresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/sessioneventquery.py
-Comment: 
-
-Filename: honeyhive/models/components/sessioneventresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/sessioneventupdate.py
-Comment: 
-
-Filename: honeyhive/models/components/sessionfeedback.py
-Comment: 
-
-Filename: honeyhive/models/components/sessionstartquery.py
-Comment: 
-
 Filename: honeyhive/models/components/sessionstartrequest.py
 Comment: 
 
-Filename: honeyhive/models/components/sessionstartresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/sessiontrace.py
-Comment: 
-
-Filename: honeyhive/models/components/successresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/successtraceresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/taskcreationquery.py
-Comment: 
-
-Filename: honeyhive/models/components/taskresponse.py
-Comment: 
-
-Filename: honeyhive/models/components/taskupdatequery.py
-Comment: 
-
-Filename: honeyhive/models/components/taskupdateresponse.py
-Comment: 
-
 Filename: honeyhive/models/components/tool.py
 Comment: 
 
-Filename: honeyhive/models/components/toolupdate.py
-Comment: 
-
-Filename: honeyhive/models/components/traceevent.py
-Comment: 
-
 Filename: honeyhive/models/components/updatedatapointrequest.py
 Comment: 
 
 Filename: honeyhive/models/components/updateprojectrequest.py
 Comment: 
 
-Filename: honeyhive/models/components/updateresponse.py
-Comment: 
-
 Filename: honeyhive/models/components/updatetoolrequest.py
 Comment: 
 
-Filename: honeyhive/models/components/uploaddataset.py
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/__init__.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/chatcompletionrequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/chatcompletionresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/configuration.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/createdatapointrequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/createdatasetrequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/createeventrequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/createprojectrequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/datapoint.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/dataset.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/datasetresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/datasetupdate.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/deleteresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/evaluation.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/evaluationloggingquery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/evaluationupdaterequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/event.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/feedbackquery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/feedbackresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/finetunedmodelresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/generatequery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/generation.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/generationloggingquery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/generationresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metric.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metriccomputerequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metriccomputeresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metriccreaterequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metriccreateresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metricdeleteresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metricedit.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metricresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metricupdaterequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/metricupdateresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/project.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/promptcreationquery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/promptresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/promptupdatequery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/security.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/sessionendresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/sessioneventquery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/sessioneventresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/sessioneventupdate.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/sessionfeedback.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/sessionstartquery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/sessionstartrequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/sessionstartresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/sessiontrace.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/successresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/successtraceresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/taskcreationquery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/taskresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/taskupdatequery.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/taskupdateresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/tool.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/toolupdate.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/traceevent.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/updatedatapointrequest.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/updateresponse.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/components/__pycache__/uploaddataset.cpython-312.pyc
-Comment: 
-
 Filename: honeyhive/models/errors/__init__.py
 Comment: 
 
 Filename: honeyhive/models/errors/sdkerror.py
 Comment: 
 
-Filename: honeyhive/models/errors/__pycache__/__init__.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/errors/__pycache__/sdkerror.cpython-312.pyc
-Comment: 
-
 Filename: honeyhive/models/operations/__init__.py
 Comment: 
 
 Filename: honeyhive/models/operations/createconfiguration.py
 Comment: 
 
 Filename: honeyhive/models/operations/createdatapoint.py
@@ -498,101 +138,32 @@
 
 Filename: honeyhive/models/operations/createproject.py
 Comment: 
 
 Filename: honeyhive/models/operations/createtool.py
 Comment: 
 
-Filename: honeyhive/models/operations/delete_datasets.py
-Comment: 
-
-Filename: honeyhive/models/operations/delete_datasets_name_.py
-Comment: 
-
-Filename: honeyhive/models/operations/delete_evaluations_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/delete_events_event_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/delete_fine_tuned_models_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/delete_metrics.py
-Comment: 
-
-Filename: honeyhive/models/operations/delete_prompts_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/delete_session_session_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/delete_tasks.py
-Comment: 
-
 Filename: honeyhive/models/operations/deleteconfiguration.py
 Comment: 
 
 Filename: honeyhive/models/operations/deletedatapoint.py
 Comment: 
 
 Filename: honeyhive/models/operations/deletedataset.py
 Comment: 
 
-Filename: honeyhive/models/operations/deleteevent.py
-Comment: 
-
 Filename: honeyhive/models/operations/deletemetric.py
 Comment: 
 
 Filename: honeyhive/models/operations/deleteproject.py
 Comment: 
 
-Filename: honeyhive/models/operations/deletesession.py
-Comment: 
-
 Filename: honeyhive/models/operations/deletetool.py
 Comment: 
 
-Filename: honeyhive/models/operations/get_datasets.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_evaluations.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_evaluations_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_fine_tuned_models.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_fine_tuned_models_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_generations.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_metrics.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_prompts.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_session.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_session_session_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_session_session_id_export.py
-Comment: 
-
-Filename: honeyhive/models/operations/get_tasks.py
-Comment: 
-
 Filename: honeyhive/models/operations/getconfigurations.py
 Comment: 
 
 Filename: honeyhive/models/operations/getdatapoint.py
 Comment: 
 
 Filename: honeyhive/models/operations/getdatapoints.py
@@ -612,89 +183,14 @@
 
 Filename: honeyhive/models/operations/getsession.py
 Comment: 
 
 Filename: honeyhive/models/operations/gettools.py
 Comment: 
 
-Filename: honeyhive/models/operations/post_chat.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_datasets.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_evaluations.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_events.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_feedback.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_fine_tuned_models.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_generations.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_generations_log.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_metrics.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_metrics_compute.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_prompts.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_session_session_id_end.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_session_session_id_event.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_session_session_id_feedback.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_session_session_id_traces.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_session_start.py
-Comment: 
-
-Filename: honeyhive/models/operations/post_tasks.py
-Comment: 
-
-Filename: honeyhive/models/operations/processeventtrace.py
-Comment: 
-
-Filename: honeyhive/models/operations/put_datasets.py
-Comment: 
-
-Filename: honeyhive/models/operations/put_evaluations_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/put_events.py
-Comment: 
-
-Filename: honeyhive/models/operations/put_metrics.py
-Comment: 
-
-Filename: honeyhive/models/operations/put_prompts_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/put_session_session_id_.py
-Comment: 
-
-Filename: honeyhive/models/operations/put_tasks.py
-Comment: 
-
 Filename: honeyhive/models/operations/startsession.py
 Comment: 
 
 Filename: honeyhive/models/operations/updateconfiguration.py
 Comment: 
 
 Filename: honeyhive/models/operations/updatedatapoint.py
@@ -711,215 +207,14 @@
 
 Filename: honeyhive/models/operations/updateproject.py
 Comment: 
 
 Filename: honeyhive/models/operations/updatetool.py
 Comment: 
 
-Filename: honeyhive/models/operations/__pycache__/__init__.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/createconfiguration.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/createdatapoint.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/createproject.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/createtool.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/delete_datasets.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/delete_datasets_name_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/delete_evaluations_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/delete_events_event_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/delete_fine_tuned_models_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/delete_metrics.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/delete_prompts_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/delete_session_session_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/delete_tasks.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/deleteconfiguration.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/deletedatapoint.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/deleteproject.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/deletesession.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/deletetool.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_datasets.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_evaluations.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_evaluations_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_fine_tuned_models.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_fine_tuned_models_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_generations.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_metrics.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_prompts.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_session.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_session_session_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_session_session_id_export.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/get_tasks.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/getconfigurations.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/getdatapoint.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/getdatapoints.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/getprojects.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/getsession.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/gettools.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_chat.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_datasets.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_evaluations.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_events.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_feedback.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_fine_tuned_models.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_generations.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_generations_log.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_metrics.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_metrics_compute.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_prompts.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_session_session_id_end.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_session_session_id_event.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_session_session_id_feedback.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_session_session_id_traces.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_session_start.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/post_tasks.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/processeventtrace.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/put_datasets.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/put_evaluations_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/put_events.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/put_metrics.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/put_prompts_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/put_session_session_id_.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/put_tasks.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/startsession.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/updateconfiguration.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/updatedatapoint.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/updateproject.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/models/operations/__pycache__/updatetool.cpython-312.pyc
-Comment: 
-
 Filename: honeyhive/utils/__init__.py
 Comment: 
 
 Filename: honeyhive/utils/langchain_tracer.py
 Comment: 
 
 Filename: honeyhive/utils/llamaindex_tracer.py
@@ -930,44 +225,26 @@
 
 Filename: honeyhive/utils/tracer.py
 Comment: 
 
 Filename: honeyhive/utils/utils.py
 Comment: 
 
-Filename: honeyhive/utils/__pycache__/__init__.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/utils/__pycache__/langchain_tracer.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/utils/__pycache__/llamaindex_tracer.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/utils/__pycache__/retries.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/utils/__pycache__/tracer.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive/utils/__pycache__/utils.cpython-312.pyc
-Comment: 
-
-Filename: honeyhive-0.2.0.dist-info/LICENSE.md
+Filename: honeyhive-0.2.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: honeyhive-0.2.0.dist-info/METADATA
+Filename: honeyhive-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: honeyhive-0.2.0.dist-info/WHEEL
+Filename: honeyhive-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: honeyhive-0.2.0.dist-info/entry_points.txt
+Filename: honeyhive-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: honeyhive-0.2.0.dist-info/top_level.txt
+Filename: honeyhive-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: honeyhive-0.2.0.dist-info/RECORD
+Filename: honeyhive-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## honeyhive/configurations.py

```diff
@@ -1,73 +1,72 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from honeyhive import utils
-from honeyhive._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
+from honeyhive._hooks import HookContext
 from honeyhive.models import components, errors, operations
 from typing import List, Optional
 
 class Configurations:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def get_configurations(self, project_name: str, type_: Optional[operations.GetConfigurationsQueryParamType] = None, env: Optional[operations.Env] = None, name: Optional[str] = None) -> operations.GetConfigurationsResponse:
+    def get_configurations(self, project_name: str, env: Optional[operations.Env] = None, name: Optional[str] = None) -> operations.GetConfigurationsResponse:
         r"""Retrieve a list of configurations"""
         hook_ctx = HookContext(operation_id='getConfigurations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetConfigurationsRequest(
             project_name=project_name,
-            type=type_,
             env=env,
             name=name,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/configurations'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetConfigurationsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.GetConfigurationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetConfigurationsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.Configuration]])
                 res.configurations = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -96,34 +95,35 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.CreateConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
@@ -138,15 +138,15 @@
         request = operations.UpdateConfigurationRequest(
             id=id,
             put_configuration_request=put_configuration_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/configurations/{id}', request)
+        url = utils.generate_url(operations.UpdateConfigurationRequest, base_url, '/configurations/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateConfigurationRequest, "put_configuration_request", False, False, 'json')
@@ -155,34 +155,35 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.UpdateConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
@@ -196,51 +197,51 @@
         hook_ctx = HookContext(operation_id='deleteConfiguration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeleteConfigurationRequest(
             id=id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/configurations/{id}', request)
+        url = utils.generate_url(operations.DeleteConfigurationRequest, base_url, '/configurations/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.DeleteConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DeleteConfigurationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
-
+
```

## honeyhive/datapoints.py

```diff
@@ -1,72 +1,72 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from honeyhive import utils
-from honeyhive._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
+from honeyhive._hooks import HookContext
 from honeyhive.models import components, errors, operations
 from typing import List, Optional
 
 class Datapoints:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def get_datapoints(self, project: str, type_: Optional[operations.Type] = None, datapoint_ids: Optional[List[str]] = None) -> operations.GetDatapointsResponse:
+    def get_datapoints(self, project: str, datapoint_ids: Optional[List[str]] = None, dataset_name: Optional[str] = None) -> operations.GetDatapointsResponse:
         r"""Retrieve a list of datapoints"""
         hook_ctx = HookContext(operation_id='getDatapoints', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetDatapointsRequest(
             project=project,
-            type=type_,
             datapoint_ids=datapoint_ids,
+            dataset_name=dataset_name,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/datapoints'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetDatapointsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.GetDatapointsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetDatapointsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDatapointsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -95,38 +95,38 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.CreateDatapointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateDatapointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateDatapointResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -142,50 +142,50 @@
         hook_ctx = HookContext(operation_id='getDatapoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetDatapointRequest(
             id=id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/datapoints/{id}', request)
+        url = utils.generate_url(operations.GetDatapointRequest, base_url, '/datapoints/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.GetDatapointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetDatapointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDatapointResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -202,15 +202,15 @@
         request = operations.UpdateDatapointRequest(
             id=id,
             update_datapoint_request=update_datapoint_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/datapoints/{id}', request)
+        url = utils.generate_url(operations.UpdateDatapointRequest, base_url, '/datapoints/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateDatapointRequest, "update_datapoint_request", False, False, 'json')
@@ -219,34 +219,35 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.UpdateDatapointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateDatapointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
@@ -260,57 +261,56 @@
         hook_ctx = HookContext(operation_id='deleteDatapoint', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeleteDatapointRequest(
             id=id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/datapoints/{id}', request)
+        url = utils.generate_url(operations.DeleteDatapointRequest, base_url, '/datapoints/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.DeleteDatapointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DeleteDatapointResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteDatapointResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
-
+
```

## honeyhive/datasets.py

```diff
@@ -1,25 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from honeyhive import utils
-from honeyhive._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
+from honeyhive._hooks import HookContext
 from honeyhive.models import components, errors, operations
 from typing import Optional
 
 class Datasets:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
-        
-    
     
-    def get_datasets(self, project: str, type_: Optional[operations.QueryParamType] = None, dataset_id: Optional[str] = None) -> operations.GetDatasetsResponse:
+    def get_datasets(self, project: str, type_: Optional[operations.Type] = None, dataset_id: Optional[str] = None) -> operations.GetDatasetsResponse:
         r"""Get datasets"""
         hook_ctx = HookContext(operation_id='getDatasets', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetDatasetsRequest(
             project=project,
             type=type_,
             dataset_id=dataset_id,
         )
@@ -29,44 +27,44 @@
         url = base_url + '/datasets'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetDatasetsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.GetDatasetsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetDatasetsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDatasetsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -95,38 +93,38 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.CreateDatasetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateDatasetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateDatasetResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -155,34 +153,35 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.UpdateDatasetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateDatasetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
@@ -203,45 +202,45 @@
         url = base_url + '/datasets'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
+        query_params = { **utils.get_query_params(operations.DeleteDatasetRequest, request), **query_params }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.DeleteDatasetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DeleteDatasetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
     
-
```

## honeyhive/events.py

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from honeyhive import utils
-from honeyhive._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
+from honeyhive._hooks import HookContext
 from honeyhive.models import errors, operations
 from typing import Optional
 
 class Events:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -35,38 +35,38 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.CreateEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateEventResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -95,34 +95,35 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.UpdateEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateEventResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code == 400 or http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
@@ -149,45 +150,44 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.GetEventsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetEventsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetEventsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
-
+
```

## honeyhive/metrics.py

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from honeyhive import utils
-from honeyhive._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
+from honeyhive._hooks import HookContext
 from honeyhive.models import components, errors, operations
 from typing import List, Optional
 
 class Metrics:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -29,44 +29,44 @@
         url = base_url + '/metrics'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetMetricsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.GetMetricsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetMetricsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.Metric]])
                 res.metrics = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -97,34 +97,35 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.CreateMetricResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateMetricResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
@@ -153,34 +154,35 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.UpdateMetricResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateMetricResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
@@ -203,45 +205,45 @@
         url = base_url + '/metrics'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
+        query_params = { **utils.get_query_params(operations.DeleteMetricRequest, request), **query_params }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.DeleteMetricResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DeleteMetricResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
-
+
```

## honeyhive/projects.py

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from honeyhive import utils
-from honeyhive._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
+from honeyhive._hooks import HookContext
 from honeyhive.models import components, errors, operations
 from typing import List, Optional
 
 class Projects:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -27,44 +27,44 @@
         url = base_url + '/projects'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetProjectsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.GetProjectsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetProjectsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.Project]])
                 res.projects = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -93,38 +93,38 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.CreateProjectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateProjectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Project])
                 res.project = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -153,34 +153,35 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.UpdateProjectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateProjectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
@@ -201,45 +202,45 @@
         url = base_url + '/projects'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
+        query_params = { **utils.get_query_params(operations.DeleteProjectRequest, request), **query_params }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.DeleteProjectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DeleteProjectResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
-
+
```

## honeyhive/sdk.py

```diff
@@ -6,15 +6,14 @@
 from .datasets import Datasets
 from .events import Events
 from .metrics import Metrics
 from .projects import Projects
 from .sdkconfiguration import SDKConfiguration
 from .session import Session
 from .tools import Tools
-from .utils.retries import RetryConfig
 from honeyhive import utils
 from honeyhive._hooks import SDKHooks
 from honeyhive.models import components
 from typing import Callable, Dict, Optional, Union
 
 class HoneyHive:
     session: Session
@@ -30,44 +29,43 @@
 
     def __init__(self,
                  bearer_auth: Union[str, Callable[[], str]],
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
-                 retry_config: Optional[RetryConfig] = None
+                 retry_config: Optional[utils.RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param bearer_auth: The bearer_auth required for authentication
         :type bearer_auth: Union[str, Callable[[], str]]
         :param server_idx: The index of the server to use for all operations
         :type server_idx: int
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session
         :param retry_config: The utils.RetryConfig to use globally
-        :type retry_config: RetryConfig
+        :type retry_config: utils.RetryConfig
         """
         if client is None:
             client = requests_http.Session()
 
         if callable(bearer_auth):
             def security():
                 return components.Security(bearer_auth = bearer_auth())
         else:
             security = components.Security(bearer_auth = bearer_auth)
 
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
-    
 
         self.sdk_configuration = SDKConfiguration(
             client,
             security,
             server_url,
             server_idx,
             retry_config=retry_config
@@ -77,15 +75,15 @@
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
         if current_server_url != server_url:
             self.sdk_configuration.server_url = server_url
 
         # pylint: disable=protected-access
-        self.sdk_configuration.__dict__['_hooks'] = hooks
+        self.sdk_configuration._hooks = hooks
 
         self._init_sdks()
 
 
     def _init_sdks(self):
         self.session = Session(self.sdk_configuration)
         self.events = Events(self.sdk_configuration)
```

## honeyhive/sdkconfiguration.py

```diff
@@ -3,40 +3,38 @@
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from dataclasses import dataclass
 from honeyhive.models import components
-from typing import Callable, Dict, Optional, Tuple, Union
+from typing import Callable, Dict, Tuple, Union
 
 
 SERVERS = [
     'https://api.honeyhive.ai',
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
-    server_url: Optional[str] = ''
-    server_idx: Optional[int] = 0
+    server_url: str = ''
+    server_idx: int = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0.1'
-    sdk_version: str = '0.7.5'
-    gen_version: str = '2.326.3'
-    user_agent: str = 'speakeasy-sdk/python 0.7.5 2.326.3 1.0.1 HoneyHive'
-    retry_config: Optional[RetryConfig] = None
-
-    def __post_init__(self):
-        self._hooks = SDKHooks()
+    sdk_version: str = '0.9.0'
+    gen_version: str = '2.281.2'
+    user_agent: str = 'speakeasy-sdk/python 0.9.0 2.281.2 1.0.1 HoneyHive'
+    retry_config: RetryConfig = None
+    _hooks: SDKHooks = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url is not None and self.server_url != '':
+        if self.server_url:
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], {}
```

## honeyhive/session.py

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from honeyhive import utils
-from honeyhive._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
+from honeyhive._hooks import HookContext
 from honeyhive.models import components, errors, operations
 from typing import Optional
 
 class Session:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -33,38 +33,38 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.StartSessionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.StartSessionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.StartSessionResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -80,57 +80,56 @@
         hook_ctx = HookContext(operation_id='getSession', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetSessionRequest(
             session_id=session_id,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(base_url, '/session/{session_id}', request)
+        url = utils.generate_url(operations.GetSessionRequest, base_url, '/session/{session_id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.GetSessionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetSessionResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Event])
                 res.event = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
-
+
```

## honeyhive/tools.py

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from honeyhive import utils
-from honeyhive._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
+from honeyhive._hooks import HookContext
 from honeyhive.models import components, errors, operations
 from typing import List, Optional
 
 class Tools:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -28,38 +28,38 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.GetToolsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.GetToolsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.Tool]])
                 res.tools = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -88,38 +88,38 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.CreateToolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.CreateToolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
-            # pylint: disable=no-else-return
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateToolResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -148,34 +148,35 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.UpdateToolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.UpdateToolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
@@ -196,45 +197,45 @@
         url = base_url + '/tools'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(request), **query_params }
+        query_params = { **utils.get_query_params(operations.DeleteToolRequest, request), **query_params }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            req = self.sdk_configuration.get_hooks().before_request(
+                hook_ctx, 
+                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
+            )
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
+            raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
+            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
+            if e:
                 raise e
-            if result is not None:
-                http_res = result
         else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
+            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
+            if isinstance(result, Exception):
+                raise result
+            http_res = result
         
         
-        res = operations.DeleteToolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
+        res = operations.DeleteToolResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
         
         if http_res.status_code == 200:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
-
+
```

## honeyhive/_hooks/sdkhooks.py

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Union
 
 
 class SDKHooks(Hooks):
     def __init__(self):
         self.sdk_init_hooks: List[SDKInitHook] = []
         self.before_request_hooks: List[BeforeRequestHook] = []
         self.after_success_hooks: List[AfterSuccessHook] = []
@@ -25,29 +25,27 @@
         self.after_error_hooks.append(hook)
 
     def sdk_init(self, base_url: str, client: requests.Session) -> Tuple[str, requests.Session]:
         for hook in self.sdk_init_hooks:
             base_url, client = hook.sdk_init(base_url, client)
         return base_url, client
 
-    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> requests.PreparedRequest:
+    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> Union[requests.PreparedRequest, Exception]:
         for hook in self.before_request_hooks:
-            out = hook.before_request(hook_ctx, request)
-            if isinstance(out, Exception):
-                raise out
-            request = out
+            request = hook.before_request(hook_ctx, request)
+            if isinstance(request, Exception):
+                raise request
 
         return request
 
     def after_success(self, hook_ctx: AfterSuccessContext, response: requests.Response) -> requests.Response:
         for hook in self.after_success_hooks:
-            out = hook.after_success(hook_ctx, response)
-            if isinstance(out, Exception):
-                raise out
-            response = out
+            response = hook.after_success(hook_ctx, response)
+            if isinstance(response, Exception):
+                raise response
         return response
 
     def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests.Response], error: Optional[Exception]) -> Tuple[Optional[requests.Response], Optional[Exception]]:
         for hook in self.after_error_hooks:
             result = hook.after_error(hook_ctx, response, error)
             if isinstance(result, Exception):
                 raise result
```

## honeyhive/_hooks/types.py

```diff
@@ -13,27 +13,23 @@
     def __init__(self, operation_id: str, oauth2_scopes: Optional[List[str]], security_source: Optional[Union[Any, Callable[[], Any]]]):
         self.operation_id = operation_id
         self.oauth2_scopes = oauth2_scopes
         self.security_source = security_source
 
 
 class BeforeRequestContext(HookContext):
-    def __init__(self, hook_ctx: HookContext):
-        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    pass
 
 
 class AfterSuccessContext(HookContext):
-    def __init__(self, hook_ctx: HookContext):
-        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
-    
+    pass
 
 
 class AfterErrorContext(HookContext):
-    def __init__(self, hook_ctx: HookContext):
-        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    pass
 
 
 class SDKInitHook(ABC):
     @abstractmethod
     def sdk_init(self, base_url: str, client: requests_http.Session) -> Tuple[str, requests_http.Session]:
         pass
 
@@ -42,21 +38,21 @@
     @abstractmethod
     def before_request(self, hook_ctx: BeforeRequestContext, request: requests_http.PreparedRequest) -> Union[requests_http.PreparedRequest, Exception]:
         pass
 
 
 class AfterSuccessHook(ABC):
     @abstractmethod
-    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.Response, Exception]:
+    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.PreparedRequest, Exception]:
         pass
 
 
 class AfterErrorHook(ABC):
     @abstractmethod
-    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.Response], Optional[Exception]], Exception]:
+    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.PreparedRequest], Optional[Exception]], Exception]:
         pass
 
 
 class Hooks(ABC):
     @abstractmethod
     def register_sdk_init_hook(self, hook: SDKInitHook):
         pass
```

## honeyhive/models/components/__init__.py

```diff
@@ -19,8 +19,8 @@
 from .security import *
 from .sessionstartrequest import *
 from .tool import *
 from .updatedatapointrequest import *
 from .updateprojectrequest import *
 from .updatetoolrequest import *
 
-__all__ = ["CallType","Configuration","ConfigurationType","CreateDatapointRequest","CreateDatapointRequestType","CreateDatasetRequest","CreateDatasetRequestPipelineType","CreateDatasetRequestType","CreateEventRequest","CreateEventRequestEventType","CreateEventRequestInputs","CreateProjectRequest","CreateToolRequest","CreateToolRequestType","Datapoint","DatapointInputs","Dataset","DatasetType","DatasetUpdate","Env","Event","EventFilter","EventType","FunctionCallParams","History","Inputs","Metric","MetricEdit","MetricEditEventType","MetricEditReturnType","MetricEditThreshold","MetricEditType","MetricType","Operator","Parameters","PipelineType","PostConfigurationRequest","PostConfigurationRequestCallType","PostConfigurationRequestEnv","PostConfigurationRequestFunctionCallParams","PostConfigurationRequestParameters","PostConfigurationRequestResponseFormat","PostConfigurationRequestSelectedFunctions","Project","PutConfigurationRequest","PutConfigurationRequestCallType","PutConfigurationRequestEnv","PutConfigurationRequestFunctionCallParams","PutConfigurationRequestParameters","PutConfigurationRequestResponseFormat","PutConfigurationRequestSelectedFunctions","PutConfigurationRequestType","ResponseFormat","ReturnType","Security","SelectedFunctions","SessionStartRequest","Threshold","Tool","ToolType","Type","UpdateDatapointRequest","UpdateDatapointRequestHistory","UpdateProjectRequest","UpdateToolRequest"]
+__all__ = ["CallType","Configuration","ConfigurationType","CreateDatapointRequest","CreateDatasetRequest","CreateDatasetRequestPipelineType","CreateDatasetRequestType","CreateEventRequest","CreateEventRequestEventType","CreateEventRequestInputs","CreateProjectRequest","CreateToolRequest","CreateToolRequestType","Datapoint","DatapointInputs","Dataset","DatasetType","DatasetUpdate","Env","Event","EventFilter","EventType","FunctionCallParams","History","Inputs","Metric","MetricEdit","MetricEditEventType","MetricEditReturnType","MetricEditThreshold","MetricEditType","MetricType","Operator","Parameters","PipelineType","PostConfigurationRequest","PostConfigurationRequestCallType","PostConfigurationRequestEnv","PostConfigurationRequestFunctionCallParams","PostConfigurationRequestParameters","PostConfigurationRequestResponseFormat","PostConfigurationRequestSelectedFunctions","Project","PutConfigurationRequest","PutConfigurationRequestCallType","PutConfigurationRequestEnv","PutConfigurationRequestFunctionCallParams","PutConfigurationRequestParameters","PutConfigurationRequestResponseFormat","PutConfigurationRequestSelectedFunctions","PutConfigurationRequestType","ResponseFormat","ReturnType","Security","SelectedFunctions","SessionStartRequest","Threshold","Tool","ToolType","Type","UpdateDatapointRequest","UpdateDatapointRequestHistory","UpdateProjectRequest","UpdateToolRequest"]
```

## honeyhive/models/components/createdatapointrequest.py

```diff
@@ -1,36 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from honeyhive import utils
 from typing import Any, Dict, List, Optional
 
-class CreateDatapointRequestType(str, Enum):
-    r"""Type of datapoint - \\"event\\" or \\"session\\" """
-    EVENT = 'event'
-    SESSION = 'session'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateDatapointRequest:
     project: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('project') }})
     r"""UUID for the project to which the datapoint belongs"""
     inputs: Dict[str, Any] = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('inputs') }})
     r"""Arbitrary JSON object containing the inputs for the datapoint"""
-    type: CreateDatapointRequestType = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type') }})
-    r"""Type of datapoint - \\"event\\" or \\"session\\" """
+    history: Optional[List[Dict[str, Any]]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('history'), 'exclude': lambda f: f is None }})
+    r"""Conversation history associated with the datapoint"""
     ground_truth: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ground_truth'), 'exclude': lambda f: f is None }})
     r"""Expected output JSON object for the datapoint"""
     linked_event: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linked_event'), 'exclude': lambda f: f is None }})
     r"""Event id for the event from which the datapoint was created"""
-    linked_evals: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linked_evals'), 'exclude': lambda f: f is None }})
-    r"""Ids of evaluations where the datapoint is included"""
     linked_datasets: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linked_datasets'), 'exclude': lambda f: f is None }})
     r"""Ids of all datasets that include the datapoint"""
     metadata: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""Any additional metadata for the datapoint"""
```

## honeyhive/models/components/updatedatapointrequest.py

```diff
@@ -21,15 +21,11 @@
     r"""Conversation history associated with the datapoint"""
     ground_truth: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('ground_truth'), 'exclude': lambda f: f is None }})
     r"""Expected output JSON object for the datapoint"""
     linked_evals: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linked_evals'), 'exclude': lambda f: f is None }})
     r"""Ids of evaluations where the datapoint is included"""
     linked_datasets: Optional[List[str]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('linked_datasets'), 'exclude': lambda f: f is None }})
     r"""Ids of all datasets that include the datapoint"""
-    saved: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('saved'), 'exclude': lambda f: f is None }})
-    r"""Whether the datapoint is saved or detected"""
-    type: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('type'), 'exclude': lambda f: f is None }})
-    r"""session or event - specify the type of datapoint"""
     metadata: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
     r"""Any additional metadata for the datapoint"""
```

## honeyhive/models/operations/__init__.py

```diff
@@ -27,8 +27,8 @@
 from .updatedatapoint import *
 from .updatedataset import *
 from .updateevent import *
 from .updatemetric import *
 from .updateproject import *
 from .updatetool import *
 
-__all__ = ["CreateConfigurationResponse","CreateDatapointResponse","CreateDatapointResponseBody","CreateDatapointResult","CreateDatasetResponse","CreateDatasetResponseBody","CreateDatasetResult","CreateEventRequestBody","CreateEventResponse","CreateEventResponseBody","CreateMetricResponse","CreateProjectResponse","CreateToolResponse","CreateToolResponseBody","DateRange","DeleteConfigurationRequest","DeleteConfigurationResponse","DeleteDatapointRequest","DeleteDatapointResponse","DeleteDatapointResponseBody","DeleteDatasetRequest","DeleteDatasetResponse","DeleteMetricRequest","DeleteMetricResponse","DeleteProjectRequest","DeleteProjectResponse","DeleteToolRequest","DeleteToolResponse","Env","GetConfigurationsQueryParamType","GetConfigurationsRequest","GetConfigurationsResponse","GetDatapointRequest","GetDatapointResponse","GetDatapointResponseBody","GetDatapointsRequest","GetDatapointsResponse","GetDatapointsResponseBody","GetDatasetsRequest","GetDatasetsResponse","GetDatasetsResponseBody","GetEventsRequestBody","GetEventsResponse","GetEventsResponseBody","GetMetricsRequest","GetMetricsResponse","GetProjectsRequest","GetProjectsResponse","GetSessionRequest","GetSessionResponse","GetToolsResponse","QueryParamType","Result","StartSessionRequestBody","StartSessionResponse","StartSessionResponseBody","Type","UpdateConfigurationRequest","UpdateConfigurationResponse","UpdateDatapointRequest","UpdateDatapointResponse","UpdateDatasetResponse","UpdateEventRequestBody","UpdateEventResponse","UpdateMetricResponse","UpdateProjectResponse","UpdateToolResponse"]
+__all__ = ["CreateConfigurationResponse","CreateDatapointResponse","CreateDatapointResponseBody","CreateDatapointResult","CreateDatasetResponse","CreateDatasetResponseBody","CreateDatasetResult","CreateEventRequestBody","CreateEventResponse","CreateEventResponseBody","CreateMetricResponse","CreateProjectResponse","CreateToolResponse","CreateToolResponseBody","DateRange","DeleteConfigurationRequest","DeleteConfigurationResponse","DeleteDatapointRequest","DeleteDatapointResponse","DeleteDatapointResponseBody","DeleteDatasetRequest","DeleteDatasetResponse","DeleteMetricRequest","DeleteMetricResponse","DeleteProjectRequest","DeleteProjectResponse","DeleteToolRequest","DeleteToolResponse","Env","GetConfigurationsRequest","GetConfigurationsResponse","GetDatapointRequest","GetDatapointResponse","GetDatapointResponseBody","GetDatapointsRequest","GetDatapointsResponse","GetDatapointsResponseBody","GetDatasetsRequest","GetDatasetsResponse","GetDatasetsResponseBody","GetEventsRequestBody","GetEventsResponse","GetEventsResponseBody","GetMetricsRequest","GetMetricsResponse","GetProjectsRequest","GetProjectsResponse","GetSessionRequest","GetSessionResponse","GetToolsResponse","Result","StartSessionRequestBody","StartSessionResponse","StartSessionResponseBody","Type","UpdateConfigurationRequest","UpdateConfigurationResponse","UpdateDatapointRequest","UpdateDatapointResponse","UpdateDatasetResponse","UpdateEventRequestBody","UpdateEventResponse","UpdateMetricResponse","UpdateProjectResponse","UpdateToolResponse"]
```

## honeyhive/models/operations/getconfigurations.py

```diff
@@ -3,32 +3,25 @@
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ...models.components import configuration as components_configuration
 from enum import Enum
 from typing import List, Optional
 
-class GetConfigurationsQueryParamType(str, Enum):
-    r"""Configuration type - \\"LLM\\" or \\"pipeline\\" - default is \\"LLM\\" """
-    LLM = 'LLM'
-    PIPELINE = 'pipeline'
-
 class Env(str, Enum):
     r"""Environment - \\"dev\\", \\"staging\\" or \\"prod\\" """
     DEV = 'dev'
     STAGING = 'staging'
     PROD = 'prod'
 
 
 @dataclasses.dataclass
 class GetConfigurationsRequest:
     project_name: str = dataclasses.field(metadata={'query_param': { 'field_name': 'project_name', 'style': 'form', 'explode': True }})
     r"""Project name for configuration like `Example Project`"""
-    type: Optional[GetConfigurationsQueryParamType] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})
-    r"""Configuration type - \\"LLM\\" or \\"pipeline\\" - default is \\"LLM\\" """
     env: Optional[Env] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'env', 'style': 'form', 'explode': True }})
     r"""Environment - \\"dev\\", \\"staging\\" or \\"prod\\" """
     name: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'name', 'style': 'form', 'explode': True }})
     r"""The name of the configuration like `v0`"""
```

## honeyhive/models/operations/getdatapoints.py

```diff
@@ -1,32 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import requests as requests_http
 from ...models.components import datapoint as components_datapoint
 from dataclasses_json import Undefined, dataclass_json
-from enum import Enum
 from honeyhive import utils
 from typing import List, Optional
 
-class Type(str, Enum):
-    r"""Type of data - \\"session\\" or \\"event\\" """
-    SESSION = 'session'
-    EVENT = 'event'
-
 
 @dataclasses.dataclass
 class GetDatapointsRequest:
     project: str = dataclasses.field(metadata={'query_param': { 'field_name': 'project', 'style': 'form', 'explode': True }})
     r"""Project ID to filter datapoints"""
-    type: Optional[Type] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})
-    r"""Type of data - \\"session\\" or \\"event\\" """
     datapoint_ids: Optional[List[str]] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'datapoint_ids', 'style': 'form', 'explode': True }})
     r"""List of datapoint ids to fetch"""
+    dataset_name: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'dataset_name', 'style': 'form', 'explode': True }})
+    r"""Name of the dataset to get datapoints from"""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class GetDatapointsResponseBody:
```

## honeyhive/models/operations/getdatasets.py

```diff
@@ -5,25 +5,25 @@
 import requests as requests_http
 from ...models.components import dataset as components_dataset
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from honeyhive import utils
 from typing import List, Optional
 
-class QueryParamType(str, Enum):
+class Type(str, Enum):
     r"""Type of the dataset - \\"evaluation\\" or \\"fine-tuning\\" """
     EVALUATION = 'evaluation'
     FINE_TUNING = 'fine-tuning'
 
 
 @dataclasses.dataclass
 class GetDatasetsRequest:
     project: str = dataclasses.field(metadata={'query_param': { 'field_name': 'project', 'style': 'form', 'explode': True }})
     r"""Project ID associated with the datasets like `65e0fc2d6a2eb95f55a92cbc`"""
-    type: Optional[QueryParamType] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})
+    type: Optional[Type] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'type', 'style': 'form', 'explode': True }})
     r"""Type of the dataset - \\"evaluation\\" or \\"fine-tuning\\" """
     dataset_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'dataset_id', 'style': 'form', 'explode': True }})
     r"""Unique dataset ID for filtering specific dataset like `663876ec4611c47f4970f0c3`"""
```

## honeyhive/utils/langchain_tracer.py

```diff
@@ -46,26 +46,30 @@
         self,
         project: str,
         name: Optional[str] = None,
         source: Optional[str] = None,
         user_properties: Optional[Dict[str, Any]] = None,
         api_key: Optional[str] = None,
         metadata: Optional[Dict[str, Any]] = None,
-        verbose = False,
+        verbose: bool = False,
+        base_url: Optional[str] = None,
     ):
         """Initialize the HoneyHive tracer."""
         super().__init__()
         self.verbose = verbose
         if self._env_api_key:
             api_key = self._env_api_key
         elif not api_key:
             raise ValueError(
                 "HoneyHive API key is not set! Please set the HONEYHIVE_API_KEY environment variable or pass in the api_key value."
             )
 
+        if base_url:
+            self._base_url = base_url
+
         if api_key:
             self._headers["Authorization"] = f"Bearer {api_key}"
 
         self.project = project
         self.source = source if source is not None else "langchain"
         self.name = name
         self.user_properties = user_properties
@@ -165,15 +169,15 @@
             logs = self._convert_run_to_logs(run=run)
             if self.project is not None:
                 logs[0].project = self.project
             self._post_trace(logs=logs)
         except Exception as error:
             logging.warning(f"Failed to persist run: {error}")
             if self.verbose:
-              traceback.print_exc()
+                traceback.print_exc()
 
     def _convert_run_to_logs(
         self, run: Run, parent_log: Optional[Log] = None
     ) -> List[Log]:
         logs: List[Log] = []
         duration = (run.end_time - run.start_time) / timedelta(milliseconds=1)
         metadata = {"langchain_trace_id": str(run.id), **run.extra}
```

## honeyhive/utils/llamaindex_tracer.py

```diff
@@ -25,14 +25,15 @@
     Log,
     log_to_dict,
     requests_retry_session,
 )
 
 import traceback
 
+
 class HHEventType(str, Enum):
     MODEL = "model"
     CHAIN = "chain"
     TOOL = "tool"
 
 
 class HoneyHiveLlamaIndexTracer(BaseCallbackHandler):
@@ -47,27 +48,31 @@
         name: Optional[str] = None,
         source: Optional[str] = None,
         user_properties: Optional[Dict[str, Any]] = None,
         tokenizer: Optional[TokenCounter] = None,
         event_types_to_ignore: Optional[List[CBEventType]] = None,
         api_key: Optional[str] = None,
         metadata: Optional[Dict[str, Any]] = None,
-        verbose = False,
+        verbose: bool = False,
+        base_url: Optional[str] = None,
     ) -> None:
         self.verbose = verbose
         if self._env_api_key:
             api_key = self._env_api_key
         elif not api_key:
             raise ValueError(
                 "HoneyHive API key is not set! Please set the HONEYHIVE_API_KEY environment variable or pass in the api_key value."
             )
 
         if api_key:
             self._headers["Authorization"] = f"Bearer {api_key}"
 
+        if base_url:
+            self._base_url = base_url
+
         self.event_starts_to_ignore = event_types_to_ignore or []
         self.event_ends_to_ignore = event_types_to_ignore or []
         self._event_pairs_by_id: Dict[str, List[CBEvent]] = defaultdict(list)
         self._cur_trace_id: Optional[str] = None
         self._trace_map: Dict[str, List[str]] = defaultdict(list)
         self.tokenizer = (
             TokenCounter(tokenizer=tokenizer) if tokenizer else TokenCounter()
@@ -231,36 +236,37 @@
 
         # Helper function to find the nearest non-blacklisted ancestor
         def find_valid_parent(event_id):
             while event_id in parent_map:
                 if event_map.get(parent_map[event_id]) is not None:
                     return parent_map[event_id]
                 event_id = parent_map[event_id]
-            return 'root'  # Default to root if no valid parents found
+            return "root"  # Default to root if no valid parents found
 
         # Recursively handle all children of each node
         def handle_children(event_id, valid_parent):
             for child in trace_map[event_id]:
                 if event_map.get(child) is not None:  # If child is not blacklisted
                     new_trace_map[valid_parent].append(child)
                     handle_children(child, child)  # Child becomes a new valid parent
                 else:
-                    handle_children(child, valid_parent)  # Continue with the current valid parent
+                    handle_children(
+                        child, valid_parent
+                    )  # Continue with the current valid parent
 
         # Start processing from root
-        for child in trace_map['root']:
+        for child in trace_map["root"]:
             if event_map.get(child) is None:  # Root's direct child is blacklisted
-                handle_children(child, 'root')  # Handle all descendants under root
+                handle_children(child, "root")  # Handle all descendants under root
             else:
-                new_trace_map['root'].append(child)
+                new_trace_map["root"].append(child)
                 handle_children(child, child)
 
         return new_trace_map
 
-
     def log_trace(self) -> None:
         try:
             events = []
             for event_list in self._trace_map.values():
                 events.extend(event_list)
             events = set(events)
             event_map = {}
@@ -272,15 +278,17 @@
             for event_id, child_event_ids in self._trace_map.items():
                 if event_id == "root":
                     continue
                 parent_log = event_map.get(event_id)
                 for child_event_id in child_event_ids:
                     child_log = event_map.get(child_event_id)
                     if child_log:
-                        child_log.parent_id = None if parent_log is None else parent_log.event_id
+                        child_log.parent_id = (
+                            None if parent_log is None else parent_log.event_id
+                        )
                         if parent_log:
                             if parent_log.children is None:
                                 parent_log.children = [child_log]
                             else:
                                 parent_log.children += [child_log]
             root_events = []
             for event_id in self._trace_map["root"]:
```

## honeyhive/utils/retries.py

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if retries.config.retry_connection_errors:
+                if retries.config.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if retries.config.retry_connection_errors:
+                if retries.config.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
@@ -110,10 +110,11 @@
             if now - start > max_elapsed_time:
                 if isinstance(exception, TemporaryError):
                     return exception.response
 
                 raise
             sleep = ((initial_interval/1000) *
                      exponent**retries + random.uniform(0, 1))
-            sleep = min(sleep, max_interval / 1000)
+            if sleep > max_interval/1000:
+                sleep = max_interval/1000
             time.sleep(sleep)
             retries += 1
```

## honeyhive/utils/tracer.py

```diff
@@ -133,17 +133,24 @@
 
     def get_output(self):
         return self.event_data["output"]
 
 
 class HoneyHiveTracer:
     def __init__(
-        self, project, name, source, api_key, user_properties={}, show_trace=False
+        self,
+        project,
+        name,
+        source,
+        api_key,
+        user_properties={},
+        show_trace=False,
+        base_url=None,
     ):
-        self._base_url = "https://api.honeyhive.ai"
+        self._base_url = "https://api.honeyhive.ai" if not base_url else base_url
         self._headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {api_key}",
         }
         body = {
             "session": {
                 "project": project,
```

## honeyhive/utils/utils.py

```diff
@@ -5,25 +5,16 @@
 import re
 import sys
 from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    List,
-    Optional,
-    Tuple,
-    Union,
-    get_args,
-    get_origin,
-)
+from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
+                    get_args, get_origin)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
 from dataclasses_json import DataClassJsonMixin
 
 
 def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
@@ -35,600 +26,470 @@
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get("security")
+        metadata = sec_field.metadata.get('security')
         if metadata is None:
             continue
-        if metadata.get("option"):
+        if metadata.get('option'):
             _parse_security_option(headers, query_params, value)
             return headers, query_params
-        if metadata.get("scheme"):
+        if metadata.get('scheme'):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
                 _parse_security_scheme(headers, query_params, metadata, security)
             else:
                 _parse_security_scheme(headers, query_params, metadata, value)
 
     return headers, query_params
 
 
-def _parse_security_option(
-    headers: Dict[str, str], query_params: Dict[str, str], option: Any
-):
+def _parse_security_option(headers: Dict[str, str], query_params: Dict[str, str], option: Any):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get("security")
-        if metadata is None or metadata.get("scheme") is None:
+        metadata = opt_field.metadata.get('security')
+        if metadata is None or metadata.get('scheme') is None:
             continue
         _parse_security_scheme(
-            headers, query_params, metadata, getattr(option, opt_field.name)
-        )
+            headers, query_params, metadata, getattr(option, opt_field.name))
 
 
-def _parse_security_scheme(
-    headers: Dict[str, str],
-    query_params: Dict[str, str],
-    scheme_metadata: Dict,
-    scheme: Any,
-):
-    scheme_type = scheme_metadata.get("type")
-    sub_type = scheme_metadata.get("sub_type")
+def _parse_security_scheme(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, scheme: Any):
+    scheme_type = scheme_metadata.get('type')
+    sub_type = scheme_metadata.get('sub_type')
 
     if is_dataclass(scheme):
-        if scheme_type == "http" and sub_type == "basic":
+        if scheme_type == 'http' and sub_type == 'basic':
             _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get("security")
-            if metadata is None or metadata.get("field_name") is None:
+            metadata = scheme_field.metadata.get('security')
+            if metadata is None or metadata.get('field_name') is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                headers, query_params, scheme_metadata, metadata, value
-            )
+                headers, query_params, scheme_metadata, metadata, value)
     else:
         _parse_security_scheme_value(
-            headers, query_params, scheme_metadata, scheme_metadata, scheme
-        )
+            headers, query_params, scheme_metadata, scheme_metadata, scheme)
 
 
-def _parse_security_scheme_value(
-    headers: Dict[str, str],
-    query_params: Dict[str, str],
-    scheme_metadata: Dict,
-    security_metadata: Dict,
-    value: Any,
-):
-    scheme_type = scheme_metadata.get("type")
-    sub_type = scheme_metadata.get("sub_type")
+def _parse_security_scheme_value(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, security_metadata: Dict, value: Any):
+    scheme_type = scheme_metadata.get('type')
+    sub_type = scheme_metadata.get('sub_type')
 
-    header_name = str(security_metadata.get("field_name"))
+    header_name = str(security_metadata.get('field_name'))
 
     if scheme_type == "apiKey":
-        if sub_type == "header":
+        if sub_type == 'header':
             headers[header_name] = value
-        elif sub_type == "query":
+        elif sub_type == 'query':
             query_params[header_name] = value
         else:
-            raise Exception("not supported")
+            raise Exception('not supported')
     elif scheme_type == "openIdConnect":
         headers[header_name] = _apply_bearer(value)
-    elif scheme_type == "oauth2":
-        if sub_type != "client_credentials":
+    elif scheme_type == 'oauth2':
+        if sub_type != 'client_credentials':
             headers[header_name] = _apply_bearer(value)
-    elif scheme_type == "http":
-        if sub_type == "bearer":
+    elif scheme_type == 'http':
+        if sub_type == 'bearer':
             headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception("not supported")
+            raise Exception('not supported')
     else:
-        raise Exception("not supported")
+        raise Exception('not supported')
 
 
 def _apply_bearer(token: str) -> str:
-    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
+    return token.lower().startswith('bearer ') and token or f'Bearer {token}'
 
 
 def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get("security")
-        if metadata is None or metadata.get("field_name") is None:
+        metadata = scheme_field.metadata.get('security')
+        if metadata is None or metadata.get('field_name') is None:
             continue
 
-        field_name = metadata.get("field_name")
+        field_name = metadata.get('field_name')
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == "username":
+        if field_name == 'username':
             username = value
-        if field_name == "password":
+        if field_name == 'password':
             password = value
 
-    data = f"{username}:{password}".encode()
-    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
+    data = f'{username}:{password}'.encode()
+    headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
 
 
-def generate_url(
-    server_url: str,
-    path: str,
-    path_params: Any,
-    gbls: Optional[Any] = None,
-) -> str:
-    path_param_values: Dict[str, str] = {}
-
-    globals_already_populated = _populate_path_params(
-        path_params, gbls, path_param_values, []
-    )
-    if gbls is not None:
-        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
-
-    for key, value in path_param_values.items():
-        path = path.replace("{" + key + "}", value, 1)
-
-    return remove_suffix(server_url, "/") + path
-
-
-def _populate_path_params(
-    path_params: Any,
-    gbls: Any,
-    path_param_values: Dict[str, str],
-    skip_fields: List[str],
-) -> List[str]:
-    globals_already_populated: List[str] = []
-
-    path_param_fields: Tuple[Field, ...] = fields(path_params)
+def generate_url(clazz: type, server_url: str, path: str, path_params: Any,
+                 gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> str:
+    path_param_fields: Tuple[Field, ...] = fields(clazz)
     for field in path_param_fields:
-        if field.name in skip_fields:
+        request_metadata = field.metadata.get('request')
+        if request_metadata is not None:
             continue
 
-        param_metadata = field.metadata.get("path_param")
+        param_metadata = field.metadata.get('path_param')
         if param_metadata is None:
             continue
 
-        param = getattr(path_params, field.name) if path_params is not None else None
-        param, global_found = _populate_from_globals(
-            field.name, param, "path_param", gbls
-        )
-        if global_found:
-            globals_already_populated.append(field.name)
+        param = getattr(
+            path_params, field.name) if path_params is not None else None
+        param = _populate_from_globals(
+            field.name, param, 'pathParam', gbls)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get("serialization", "")
-        if serialization != "":
+        serialization = param_metadata.get('serialization', '')
+        if serialization != '':
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param
-            )
+                param_metadata, field.type, f_name, param)
             for key, value in serialized_params.items():
-                path_param_values[key] = value
+                path = path.replace(
+                    '{' + key + '}', value, 1)
         else:
-            if param_metadata.get("style", "simple") == "simple":
+            if param_metadata.get('style', 'simple') == 'simple':
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path_param_values[param_metadata.get("field_name", field.name)] = (
-                        ",".join(pp_vals)
-                    )
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get("explode"):
-                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get('explode'):
+                            pp_vals.append(
+                                f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path_param_values[param_metadata.get("field_name", field.name)] = (
-                        ",".join(pp_vals)
-                    )
+                            pp_vals.append(
+                                f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get("path_param")
+                        param_value_metadata = param_field.metadata.get(
+                            'path_param')
                         if not param_value_metadata:
                             continue
 
-                        param_name = param_value_metadata.get("field_name", field.name)
+                        parm_name = param_value_metadata.get(
+                            'field_name', field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get("explode"):
+                        if param_metadata.get('explode'):
                             pp_vals.append(
-                                f"{param_name}={_val_to_string(param_field_val)}"
-                            )
+                                f"{parm_name}={_val_to_string(param_field_val)}")
                         else:
                             pp_vals.append(
-                                f"{param_name},{_val_to_string(param_field_val)}"
-                            )
-                    path_param_values[param_metadata.get("field_name", field.name)] = (
-                        ",".join(pp_vals)
-                    )
+                                f"{parm_name},{_val_to_string(param_field_val)}")
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
                 else:
-                    path_param_values[param_metadata.get("field_name", field.name)] = (
-                        _val_to_string(param)
-                    )
+                    path = path.replace(
+                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
 
-    return globals_already_populated
+    return remove_suffix(server_url, '/') + path
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace("{" + key + "}", value)
+        url_with_params = url_with_params.replace(
+            '{' + key + '}', value)
 
     return url_with_params
 
 
-def get_query_params(
-    query_params: Any,
-    gbls: Optional[Any] = None,
-) -> Dict[str, List[str]]:
+def get_query_params(clazz: type, query_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[
+        str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
-    if gbls is not None:
-        _populate_query_params(gbls, None, params, globals_already_populated)
-
-    return params
-
-
-def _populate_query_params(
-    query_params: Any,
-    gbls: Any,
-    query_param_values: Dict[str, List[str]],
-    skip_fields: List[str],
-) -> List[str]:
-    globals_already_populated: List[str] = []
-
-    param_fields: Tuple[Field, ...] = fields(query_params)
+    param_fields: Tuple[Field, ...] = fields(clazz)
     for field in param_fields:
-        if field.name in skip_fields:
+        request_metadata = field.metadata.get('request')
+        if request_metadata is not None:
             continue
 
-        metadata = field.metadata.get("query_param")
+        metadata = field.metadata.get('query_param')
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(query_params, param_name) if query_params is not None else None
+        value = getattr(
+            query_params, param_name) if query_params is not None else None
 
-        value, global_found = _populate_from_globals(
-            param_name, value, "query_param", gbls
-        )
-        if global_found:
-            globals_already_populated.append(param_name)
+        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get("serialization", "")
-        if serialization != "":
+        serialization = metadata.get('serialization', '')
+        if serialization != '':
             serialized_parms = _get_serialized_params(
-                metadata, field.type, f_name, value
-            )
+                metadata, field.type, f_name, value)
             for key, value in serialized_parms.items():
-                if key in query_param_values:
-                    query_param_values[key].extend(value)
+                if key in params:
+                    params[key].extend(value)
                 else:
-                    query_param_values[key] = [value]
+                    params[key] = [value]
         else:
-            style = metadata.get("style", "form")
-            if style == "deepObject":
-                _populate_deep_object_query_params(
-                    metadata, f_name, value, query_param_values
-                )
-            elif style == "form":
-                _populate_delimited_query_params(
-                    metadata, f_name, value, ",", query_param_values
-                )
-            elif style == "pipeDelimited":
-                _populate_delimited_query_params(
-                    metadata, f_name, value, "|", query_param_values
-                )
+            style = metadata.get('style', 'form')
+            if style == 'deepObject':
+                params = {**params, **_get_deep_object_query_params(
+                    metadata, f_name, value)}
+            elif style == 'form':
+                params = {**params, **_get_delimited_query_params(
+                    metadata, f_name, value, ",")}
+            elif style == 'pipeDelimited':
+                params = {**params, **_get_delimited_query_params(
+                    metadata, f_name, value, "|")}
             else:
-                raise Exception("not yet implemented")
+                raise Exception('not yet implemented')
+    return params
 
-    return globals_already_populated
 
+def get_headers(headers_params: Any) -> Dict[str, str]:
+    if headers_params is None:
+        return {}
 
-def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    globals_already_populated = []
-    if headers_params is not None:
-        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
-    if gbls is not None:
-        _populate_headers(gbls, None, headers, globals_already_populated)
-
-    return headers
-
-
-def _populate_headers(
-    headers_params: Any,
-    gbls: Any,
-    header_values: Dict[str, str],
-    skip_fields: List[str],
-) -> List[str]:
-    globals_already_populated: List[str] = []
-
     param_fields: Tuple[Field, ...] = fields(headers_params)
     for field in param_fields:
-        if field.name in skip_fields:
-            continue
-
-        metadata = field.metadata.get("header")
+        metadata = field.metadata.get('header')
         if not metadata:
             continue
 
-        value, global_found = _populate_from_globals(
-            field.name, getattr(headers_params, field.name), "header", gbls
-        )
-        if global_found:
-            globals_already_populated.append(field.name)
-        value = _serialize_header(metadata.get("explode", False), value)
-
-        if value != "":
-            header_values[metadata.get("field_name", field.name)] = value
-
-    return globals_already_populated
-
-
-def _get_serialized_params(
-    metadata: Dict, field_type: type, field_name: str, obj: Any
-) -> Dict[str, str]:
+        value = _serialize_header(metadata.get(
+            'explode', False), getattr(headers_params, field.name))
+
+        if value != '':
+            headers[metadata.get('field_name', field.name)] = value
+
+    return headers
+
+
+def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: Any) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get("serialization", "")
-    if serialization == "json":
-        params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
+    serialization = metadata.get('serialization', '')
+    if serialization == 'json':
+        params[metadata.get("field_name", field_name)
+               ] = marshal_json(obj, field_type)
 
     return params
 
 
-def _populate_deep_object_query_params(
-    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
-):
+def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: Any) -> Dict[str, List[str]]:
+    params: Dict[str, List[str]] = {}
+
     if obj is None:
-        return
+        return params
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get("query_param")
+            obj_param_metadata = obj_field.metadata.get('query_param')
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if (
-                        params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
-                        )
-                        is None
-                    ):
+                    if params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
-                        ] = []
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                        ]
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
-                    ].append(_val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
+                        _val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
-                ] = [_val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
+                    _val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if (
-                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
-                        is None
-                    ):
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
-
-                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
-                        _val_to_string(val)
-                    )
+                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
+                        ]
+
+                    params[
+                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)
-                ]
+                    _val_to_string(value)]
+    return params
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get("query_param")
+    obj_param_metadata = obj_field.metadata.get('query_param')
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_delimited_query_params(
-    metadata: Dict,
-    field_name: str,
-    obj: Any,
-    delimiter: str,
-    query_param_values: Dict[str, List[str]],
-):
-    _populate_form(
-        field_name,
-        metadata.get("explode", True),
-        obj,
-        _get_query_param_field_name,
-        delimiter,
-        query_param_values,
-    )
+def _get_delimited_query_params(metadata: Dict, field_name: str, obj: Any, delimiter: str) -> Dict[
+        str, List[str]]:
+    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    "json": "application/json",
-    "form": "application/x-www-form-urlencoded",
-    "multipart": "multipart/form-data",
-    "raw": "application/octet-stream",
-    "string": "text/plain",
+    'json': 'application/json',
+    'form': 'application/x-www-form-urlencoded',
+    'multipart': 'multipart/form-data',
+    'raw': 'application/octet-stream',
+    'string': 'text/plain',
 }
 
 
-def serialize_request_body(
-    request: Any,
-    request_type: type,
-    request_field_name: str,
-    nullable: bool,
-    optional: bool,
-    serialization_method: str,
-    encoder=None,
-) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
+def serialize_request_body(request: Any, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
+        Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(
-            request_field_name,
-            request_type,
-            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-            request,
-            encoder,
-        )
+        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+                                      request, encoder)
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get("request")
+            request_metadata = field.metadata.get('request')
             break
 
     if request_metadata is None:
-        raise Exception("invalid request type")
+        raise Exception('invalid request type')
 
-    return serialize_content_type(
-        request_field_name,
-        request_type,
-        request_metadata.get("media_type", "application/octet-stream"),
-        request_val,
-    )
+    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
+                                  request_val)
 
 
-def serialize_content_type(
-    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
-) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
-    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
+def serialize_content_type(field_name: str, request_type: Any, media_type: str, request: Any, encoder=None) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r"multipart\/.*", media_type) is not None:
+    if re.match(r'multipart\/.*', media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
+    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}"
-    )
+        f"invalid request body type {type(request)} for mediaType {media_type}")
 
 
-def serialize_multipart_form(
-    media_type: str, request: Any
-) -> Tuple[str, Any, List[List[Any]]]:
+def serialize_multipart_form(media_type: str, request: Any) -> Tuple[str, Any, List[List[Any]]]:
     form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get("multipart_form")
+        field_metadata = field.metadata.get('multipart_form')
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get("multipart_form")
+                file_metadata = file_field.metadata.get('multipart_form')
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get("field_name", file_field.name)
+                    field_name = file_metadata.get(
+                        "field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception("invalid multipart/form-data file")
+                raise Exception('invalid multipart/form-data file')
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [
-                field_metadata.get("field_name", field.name),
-                [None, marshal_json(val, field.type), "application/json"],
-            ]
+            to_append = [field_metadata.get("field_name", field.name), [
+                None, marshal_json(val, field.type), "application/json"]]
             form.append(to_append)
         else:
-            field_name = field_metadata.get("field_name", field.name)
+            field_name = field_metadata.get(
+                "field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append([field_name + "[]", [None, _val_to_string(value)]])
+                    form.append(
+                        [field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(
-    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
-) -> Dict[str, List[str]]:
+def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
+        str, List[str]]:
     if existing is None:
         existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -649,218 +510,215 @@
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get("form")
+            metadata = field.metadata.get('form')
             if metadata is None:
                 continue
 
-            field_name = metadata.get("field_name", field.name)
+            field_name = metadata.get('field_name', field.name)
 
-            if metadata.get("json"):
+            if metadata.get('json'):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get("style", "form") == "form":
-                    _populate_form(
-                        field_name,
-                        metadata.get("explode", True),
-                        val,
-                        _get_form_field_name,
-                        ",",
-                        form,
-                    )
+                if metadata.get('style', 'form') == 'form':
+                    form = {**form, **_populate_form(
+                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
                 else:
-                    raise Exception(f"Invalid form style for field {field.name}")
+                    raise Exception(
+                        f'Invalid form style for field {field.name}')
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f"Invalid request body type for field {field_name}")
+        raise Exception(f'Invalid request body type for field {field_name}')
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get("form")
+    obj_param_metadata = obj_field.metadata.get('form')
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(
-    field_name: str,
-    explode: boolean,
-    obj: Any,
-    get_field_name_func: Callable,
-    delimiter: str,
-    form: Dict[str, List[str]],
-):
+def _populate_form(field_name: str, explode: boolean, obj: Any, get_field_name_func: Callable, delimiter: str) -> \
+        Dict[str, List[str]]:
+    params: Dict[str, List[str]] = {}
+
     if obj is None:
-        return form
+        return params
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == "":
+            if obj_field_name == '':
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                form[obj_field_name] = [_val_to_string(val)]
+                params[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
+                items.append(
+                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
 
         if len(items) > 0:
-            form[field_name] = [delimiter.join(items)]
+            params[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                form[key] = [_val_to_string(value)]
+                params[key] = [_val_to_string(value)]
             else:
-                items.append(f"{key}{delimiter}{_val_to_string(value)}")
+                items.append(f'{key}{delimiter}{_val_to_string(value)}')
 
         if len(items) > 0:
-            form[field_name] = [delimiter.join(items)]
+            params[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in form:
-                    form[field_name] = []
-                form[field_name].append(_val_to_string(value))
+                if not field_name in params:
+                    params[field_name] = []
+                params[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            form[field_name] = [delimiter.join([str(item) for item in items])]
+            params[field_name] = [delimiter.join(
+                [str(item) for item in items])]
     else:
-        form[field_name] = [_val_to_string(obj)]
+        params[field_name] = [_val_to_string(obj)]
 
-    return form
+    return params
 
 
 def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ""
+        return ''
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get("header")
+            obj_param_metadata = obj_field.metadata.get('header')
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
-            if obj_field_name == "":
+            obj_field_name = obj_param_metadata.get(
+                'field_name', obj_field.name)
+            if obj_field_name == '':
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(f"{obj_field_name}={_val_to_string(val)}")
+                items.append(
+                    f'{obj_field_name}={_val_to_string(val)}')
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ",".join(items)
+            return ','.join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f"{key}={_val_to_string(value)}")
+                items.append(f'{key}={_val_to_string(value)}')
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ",".join([str(item) for item in items])
+            return ','.join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ",".join(items)
+            return ','.join(items)
     else:
-        return f"{_val_to_string(obj)}"
+        return f'{_val_to_string(obj)}'
 
-    return ""
+    return ''
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
+                               bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f"unable to unmarshal {data} as {typ} - {attr_err}"
-        ) from attr_err
+            f'unable to unmarshal {data} as {typ} - {attr_err}') from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
-        raise ValueError(f"Could not marshal None into non-optional type: {typ}")
+        raise ValueError(
+            f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
+    marshal = make_dataclass('Marshal', [('res', typ)],
+                             bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(",", ":"), sort_keys=True)
+    return json.dumps(val, separators=(',', ':'), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg["content-type"] = content_type
+    msg['content-type'] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
+        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
             return True
 
     return False
 
 
 def match_status_codes(status_codes: List[str], status_code: int) -> bool:
     for code in status_codes:
@@ -904,41 +762,14 @@
 
 
 def bigintdecoder(val):
     if isinstance(val, float):
         raise ValueError(f"{val} is a float")
     return int(val)
 
-def integerstrencoder(optional: bool):
-    def integerstrencode(val: int):
-        if optional and val is None:
-            return None
-        return str(val)
-
-    return integerstrencode
-
-
-def integerstrdecoder(val):
-    if isinstance(val, float):
-        raise ValueError(f"{val} is a float")
-    return int(val)
-
-
-def numberstrencoder(optional: bool):
-    def numberstrencode(val: float):
-        if optional and val is None:
-            return None
-        return str(val)
-
-    return numberstrencode
-
-
-def numberstrdecoder(val):
-    return float(val)
-
 
 def decimalencoder(optional: bool, as_str: bool):
     def decimalencode(val: Decimal):
         if optional and val is None:
             return None
 
         if as_str:
@@ -1004,84 +835,64 @@
 
 
 def union_encoder(all_encoders: Dict[str, Callable]):
     def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
-
     return selective_encoder
 
 
 def union_decoder(all_decoders: List[Callable]):
     def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
-
     return selective_decoder
 
 
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
 def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return str(val.isoformat().replace("+00:00", "Z"))
+        return str(val.isoformat().replace('+00:00', 'Z'))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(
-    param_name: str, value: Any, param_type: str, gbls: Any
-) -> Tuple[Any, bool]:
-    if gbls is None:
-        return value, False
-
-    global_fields = fields(gbls)
-
-    found = False
-    for field in global_fields:
-        if field.name is not param_name:
-            continue
-
-        found = True
-
-        if value is not None:
-            return value, True
+def _populate_from_globals(param_name: str, value: Any, param_type: str, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]]):
+    if value is None and gbls is not None:
+        if 'parameters' in gbls:
+            if param_type in gbls['parameters']:
+                if param_name in gbls['parameters'][param_type]:
+                    global_value = gbls['parameters'][param_type][param_name]
+                    if global_value is not None:
+                        value = global_value
 
-        global_value = getattr(gbls, field.name)
-
-        param_metadata = field.metadata.get(param_type)
-        if param_metadata is None:
-            return value, True
-
-        return global_value, True
-
-    return value, found
+    return value
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules["sdk.models.components"], obj[field_name])
+        kls = getattr(sys.modules['sdk.models.components'], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
-
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[: -len(suffix)]
+        return input_string[:-len(suffix)]
     return input_string
```

## Comparing `honeyhive-0.2.0.dist-info/LICENSE.md` & `honeyhive-0.2.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `honeyhive-0.2.0.dist-info/METADATA` & `honeyhive-0.2.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeyhive
-Version: 0.2.0
+Version: 0.2.1
 Summary: The HoneyHive SDK for Python
 Author: HoneyHive
 Author-email: support@honeyhive.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.honeyhive.ai/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -48,15 +48,15 @@
 import honeyhive
 from honeyhive.models import components, operations
 
 s = honeyhive.HoneyHive(
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-res = s.session.start_session(request=operations.StartSessionRequestBody(
+req = operations.StartSessionRequestBody(
     session=components.SessionStartRequest(
         project='Simple RAG Project',
         session_name='Playground Session',
         source='playground',
         session_id='caf77ace-3417-4da4-944d-f4a0688f3c23',
         children_ids=[
             '7f22137a-6911-4ed3-bc36-110f1dde6b66',
@@ -83,15 +83,17 @@
         },
         metadata={
 
         },
         start_time=1712025501605,
         end_time=1712025499832,
     ),
-))
+)
+
+res = s.session.start_session(req)
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End SDK Example Usage [usage] -->
@@ -157,29 +159,27 @@
 <!-- Start Error Handling [errors] -->
 ## Error Handling
 
 Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 
 | Error Object    | Status Code     | Content Type    |
 | --------------- | --------------- | --------------- |
-| errors.SDKError | 4xx-5xx         | */*             |
+| errors.SDKError | 4x-5xx          | */*             |
 
 ### Example
 
 ```python
 import honeyhive
 from honeyhive.models import components, errors, operations
 
 s = honeyhive.HoneyHive(
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-res = None
-try:
-    res = s.session.start_session(request=operations.StartSessionRequestBody(
+req = operations.StartSessionRequestBody(
     session=components.SessionStartRequest(
         project='Simple RAG Project',
         session_name='Playground Session',
         source='playground',
         session_id='caf77ace-3417-4da4-944d-f4a0688f3c23',
         children_ids=[
             '7f22137a-6911-4ed3-bc36-110f1dde6b66',
@@ -206,15 +206,19 @@
         },
         metadata={
 
         },
         start_time=1712025501605,
         end_time=1712025499832,
     ),
-))
+)
+
+res = None
+try:
+    res = s.session.start_session(req)
 except errors.SDKError as e:
     # handle exception
     raise(e)
 
 if res.object is not None:
     # handle response
     pass
@@ -240,15 +244,15 @@
 from honeyhive.models import components, operations
 
 s = honeyhive.HoneyHive(
     server_idx=0,
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-res = s.session.start_session(request=operations.StartSessionRequestBody(
+req = operations.StartSessionRequestBody(
     session=components.SessionStartRequest(
         project='Simple RAG Project',
         session_name='Playground Session',
         source='playground',
         session_id='caf77ace-3417-4da4-944d-f4a0688f3c23',
         children_ids=[
             '7f22137a-6911-4ed3-bc36-110f1dde6b66',
@@ -275,15 +279,17 @@
         },
         metadata={
 
         },
         start_time=1712025501605,
         end_time=1712025499832,
     ),
-))
+)
+
+res = s.session.start_session(req)
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 
@@ -296,15 +302,15 @@
 from honeyhive.models import components, operations
 
 s = honeyhive.HoneyHive(
     server_url="https://api.honeyhive.ai",
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-res = s.session.start_session(request=operations.StartSessionRequestBody(
+req = operations.StartSessionRequestBody(
     session=components.SessionStartRequest(
         project='Simple RAG Project',
         session_name='Playground Session',
         source='playground',
         session_id='caf77ace-3417-4da4-944d-f4a0688f3c23',
         children_ids=[
             '7f22137a-6911-4ed3-bc36-110f1dde6b66',
@@ -331,15 +337,17 @@
         },
         metadata={
 
         },
         start_time=1712025501605,
         end_time=1712025499832,
     ),
-))
+)
+
+res = s.session.start_session(req)
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End Server Selection [server] -->
@@ -352,15 +360,15 @@
 For example, you could specify a header for every request that this sdk makes as follows:
 ```python
 import honeyhive
 import requests
 
 http_client = requests.Session()
 http_client.headers.update({'x-custom-header': 'someValue'})
-s = honeyhive.HoneyHive(client=http_client)
+s = honeyhive.HoneyHive(client: http_client)
 ```
 <!-- End Custom HTTP Client [http-client] -->
 
 <!-- Start Authentication [security] -->
 ## Authentication
 
 ### Per-Client Security Schemes
@@ -376,15 +384,15 @@
 import honeyhive
 from honeyhive.models import components, operations
 
 s = honeyhive.HoneyHive(
     bearer_auth="<YOUR_BEARER_TOKEN_HERE>",
 )
 
-res = s.session.start_session(request=operations.StartSessionRequestBody(
+req = operations.StartSessionRequestBody(
     session=components.SessionStartRequest(
         project='Simple RAG Project',
         session_name='Playground Session',
         source='playground',
         session_id='caf77ace-3417-4da4-944d-f4a0688f3c23',
         children_ids=[
             '7f22137a-6911-4ed3-bc36-110f1dde6b66',
@@ -411,15 +419,17 @@
         },
         metadata={
 
         },
         start_time=1712025501605,
         end_time=1712025499832,
     ),
-))
+)
+
+res = s.session.start_session(req)
 
 if res.object is not None:
     # handle response
     pass
 
 ```
 <!-- End Authentication [security] -->
```

