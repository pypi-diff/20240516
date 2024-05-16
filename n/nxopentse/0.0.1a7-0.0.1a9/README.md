# Comparing `tmp/nxopentse-0.0.1a7.tar.gz` & `tmp/nxopentse-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxopentse-0.0.1a7.tar", last modified: Thu Mar 21 09:27:01 2024, max compression
+gzip compressed data, was "nxopentse-0.0.1a9.tar", last modified: Thu Mar 28 10:52:33 2024, max compression
```

## Comparing `nxopentse-0.0.1a7.tar` & `nxopentse-0.0.1a9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:27:01.250104 nxopentse-0.0.1a7/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-21 09:27:01.246104 nxopentse-0.0.1a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 09:27:01.250104 nxopentse-0.0.1a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:27:01.242104 nxopentse-0.0.1a7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:27:01.246104 nxopentse-0.0.1a7/src/nxopentse/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:27:01.246104 nxopentse-0.0.1a7/src/nxopentse/cad/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/cad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/cad/code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:27:01.246104 nxopentse-0.0.1a7/src/nxopentse/cae/
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/cae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51174 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/cae/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    48524 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/cae/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/cae/solving.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:27:01.246104 nxopentse-0.0.1a7/src/nxopentse/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/tools/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-03-21 09:26:55.000000 nxopentse-0.0.1a7/src/nxopentse/tools/general.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 09:27:01.246104 nxopentse-0.0.1a7/src/nxopentse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-03-21 09:27:01.000000 nxopentse-0.0.1a7/src/nxopentse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-21 09:27:01.000000 nxopentse-0.0.1a7/src/nxopentse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 09:27:01.000000 nxopentse-0.0.1a7/src/nxopentse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-21 09:27:01.000000 nxopentse-0.0.1a7/src/nxopentse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:52:33.518894 nxopentse-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-28 10:52:33.518894 nxopentse-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 10:52:33.518894 nxopentse-0.0.1a9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:52:33.514894 nxopentse-0.0.1a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:52:33.514894 nxopentse-0.0.1a9/src/nxopentse/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:52:33.514894 nxopentse-0.0.1a9/src/nxopentse/cad/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/cad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13962 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/cad/code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:52:33.514894 nxopentse-0.0.1a9/src/nxopentse/cae/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/cae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58286 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/cae/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48524 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/cae/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/cae/solving.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:52:33.518894 nxopentse-0.0.1a9/src/nxopentse/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/tools/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-03-28 10:52:26.000000 nxopentse-0.0.1a9/src/nxopentse/tools/general.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 10:52:33.518894 nxopentse-0.0.1a9/src/nxopentse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-28 10:52:33.000000 nxopentse-0.0.1a9/src/nxopentse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-28 10:52:33.000000 nxopentse-0.0.1a9/src/nxopentse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 10:52:33.000000 nxopentse-0.0.1a9/src/nxopentse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-28 10:52:33.000000 nxopentse-0.0.1a9/src/nxopentse.egg-info/top_level.txt
```

### Comparing `nxopentse-0.0.1a7/LICENSE` & `nxopentse-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `nxopentse-0.0.1a7/pyproject.toml` & `nxopentse-0.0.1a9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # https://packaging.python.org/en/latest/guides/writing-pyproject-toml/
 
 [project]
 name = "nxopentse"
-version = "0.0.1a7"
+version = "0.0.1a9"
 authors = [
   { name="theScriptingEngineer", email="nxopen@theScriptingEngineer.com" },
 ]
 maintainers = [
   { name="theScriptingEngineer", email="nxopen@theScriptingEngineer.com" },
 ]
 description = "An NXOpen helper package to reuse code in scripts, in order to avoid having all the underlying code in the journals itself."
@@ -15,14 +15,14 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Documentation = "https://nxopentse.theScriptingEngineer.com"
+Documentation = "https://nxopentsedocumentation.theScriptingEngineer.com"
 Repository = "https://github.com/theScriptingEngineer/nxopentse"
 Issues = "https://github.com/theScriptingEngineer/nxopentse/issues"
 
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `nxopentse-0.0.1a7/src/nxopentse/cae/__init__.py` & `nxopentse-0.0.1a9/src/nxopentse/cae/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
                             combine_results, \
                             export_result, \
                             get_result_paramaters, \
                             envelope_results, \
                             envelope_solution, \
                             get_nodal_value, \
                             get_nodal_values, \
+                            get_element_nodal_value, \
                             add_companion_result, \
                             write_submodel_data_to_file
 
 from .preprocessing import hello, \
                             create_node, \
                             create_nodal_constraint, \
                             create_nodal_force_default_name, \
```

### Comparing `nxopentse-0.0.1a7/src/nxopentse/cae/postprocessing.py` & `nxopentse-0.0.1a9/src/nxopentse/cae/postprocessing.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,15 @@
         sim_solution: NXOpen.CAE.SimSolution = get_solution(post_inputs[i]._solution)
         sim_result_reference: NXOpen.CAE.SimResultReference = cast(NXOpen.CAE.SimResultReference, sim_solution.Find(reference_type))
 
         try:
             # SolutionResult[filename_solutionname]
             solution_results[i] = cast(NXOpen.CAE.SolutionResult, the_session.ResultManager.FindObject("SolutionResult[" + sys.Path.GetFileName(simPart.FullPath) + "_" + sim_solution.Name + "]"))
         except:
+            the_uf_session.Ui.DisplayMessage("Loading results for " + post_inputs[i]._solution + " SubCase " + str(post_inputs[i]._subcase) + " Iteration " + str(post_inputs[i]._iteration) + " ResultType " + post_inputs[i]._resultType)
             solution_results[i] = the_session.ResultManager.CreateReferenceResult(sim_result_reference)
 
     return solution_results
 
 
 def get_results_units(base_result_types: List[NXOpen.CAE.BaseResultType]) -> List[NXOpen.Unit]:
     """This funciton returns the unit of the first component in each resulttype.
@@ -871,14 +872,170 @@
     nodal_data: Dict[int, List[float]] = {}
     for node_label in node_labels:
         nodal_data[node_label] = result_access.AskNodalResultAllComponents(solution_results[0].AskNodeIndex(node_label))
 
     return dict(sorted(nodal_data.items()))
 
 
+def get_element_nodal_value(solution_name: str, subcase: int, iteration: int, result_type: str, element_label: int, result_parameters: NXOpen.CAE.ResultParameters = None) -> tuple:
+    """
+    Retrieve element-nodal values for a specific element in a given solution.
+    Note that the element-nodal values are hard coded to be stress and the maximum of the section for shell elements
+
+    Parameters
+    ----------
+    solution_name : str
+        The name of the solution containing the results.
+
+    subcase : int
+        The subcase number within the solution.
+
+    iteration : int
+        The iteration number within the subcase.
+
+    result_type : str
+        The type of result to retrieve (e.g. 'Displacement - Nodal', 'Reaction Force - Nodal', 'Reaction Moment - Nodal').
+
+    element_label : int
+        The label of the element for which element-nodal values are to be retrieved.
+
+    result_parameters : NXOpen.CAE.ResultParameters, optional
+        The result parameters to use for the elemental values. Default is ShellSection.Maximum and stress components.
+
+    Returns
+    -------
+    tuple
+        A tuple with 3 objects: 
+        a list with the node numbers
+        an int which is the number of results per node (numComponents)
+        and a list which containst the element-nodal values: node_index*numComponents + component_index
+
+        
+    Raises
+    ------
+    IndexError
+        If the solution_results list is empty.
+    IndexError
+        If the result_types list is empty.
+    IndexError
+        If the result_parameters list is empty.
+    IndexError
+        If element_nodal_data list does not contain expected element-nodal values:
+            XX YY ZZ XY YZ ZX Determinant Mean MaxShear MinPrincipal MidPrincipal MaxPrincipal WorstPrincipal Octahedral Von-Mises
+
+    Notes
+    -----
+    Tested in SC2212
+
+    """
+    post_input: PostInput = PostInput(solution_name, subcase, iteration, result_type)
+    # check input and catch errors so that the user doesn't get a error pop-up in SC
+    try:
+        check_post_input([post_input])
+    
+    except ValueError as e:
+        # internal raised exceptions are raised as valueError
+        the_lw.WriteFullline("Did not execute ExportResult due to input error. Please check the previous messages.")
+        # we still return the tehcnical message as an additional log
+        the_lw.WriteFullline(str(e))
+        return
+    except Exception as e:
+        the_lw.WriteFullline("Did not execute ExportResult due to general error. Please check the previous messages.")
+        # we still return the tehcnical message as an additional log
+        the_lw.WriteFullline(str(e))
+        return
+    solution_results: List[NXOpen.CAE.SolutionResult] = load_results([post_input])
+    result: NXOpen.CAE.Result = cast(NXOpen.CAE.Result, solution_results[0])
+    result_types: List[NXOpen.CAE.ResultType] = get_result_types([post_input], solution_results)
+    if result_parameters is None:
+        result_parameters: List[NXOpen.CAE.ResultParameters] = get_result_paramaters(result_types, NXOpen.CAE.Result.ShellSection.Maximum, NXOpen.CAE.Result.Component.Xx, False)
+    result_access: NXOpen.CAE.ResultAccess = the_session.ResultManager.CreateResultAccess(result, result_parameters[0])
+    element_nodal_data: tuple = result_access.AskElementNodalResultAllComponents(solution_results[0].AskElementIndex(element_label)) #.AskNodalResultAllComponents(solution_results[0].AskNodeIndex(element_label))
+    
+
+    # the_lw.WriteFullline("Fx:\t" + str(nodal_data[0]) + "\tFy:\t" + str(nodal_data[1]) + "\tFz:\t" + str(nodal_data[2]) + "\tMagnitude:\t" + str(nodal_data[3]))
+
+    return element_nodal_data
+
+
+def get_elemental_value(solution_name: str, subcase: int, iteration: int, result_type: str, element_label: int, result_parameters: NXOpen.CAE.ResultParameters = None) -> tuple:
+    """
+    Retrieve elemental values for a specific element in a given solution.
+    Note that the elemental values are hard coded to be stress and the maximum of the section for shell elements
+
+    Parameters
+    ----------
+    solution_name : str
+        The name of the solution containing the results.
+
+    subcase : int
+        The subcase number within the solution.
+
+    iteration : int
+        The iteration number within the subcase.
+
+    result_type : str
+        The type of result to retrieve (e.g. 'Displacement - Nodal', 'Reaction Force - Nodal', 'Reaction Moment - Nodal').
+
+    element_label : int
+        The label of the element for which elemental values are to be retrieved.
+    
+    result_parameters : NXOpen.CAE.ResultParameters, optional
+        The result parameters to use for the elemental values. Default is ShellSection.Maximum and stress components.
+
+    Returns
+    -------
+    List[float]
+        A list with the requested elemental values.
+
+        
+    Raises
+    ------
+    IndexError
+        If the solution_results list is empty.
+    IndexError
+        If the result_types list is empty.
+    IndexError
+        If the result_parameters list is empty.
+    IndexError
+        If elemental_data list does not contain expected element-nodal values:
+            XX YY ZZ XY YZ ZX Determinant Mean MaxShear MinPrincipal MidPrincipal MaxPrincipal WorstPrincipal Octahedral Von-Mises
+
+    Notes
+    -----
+    Tested in SC2212
+
+    """
+    post_input: PostInput = PostInput(solution_name, subcase, iteration, result_type)
+    # check input and catch errors so that the user doesn't get a error pop-up in SC
+    try:
+        check_post_input([post_input])
+    
+    except ValueError as e:
+        # internal raised exceptions are raised as valueError
+        the_lw.WriteFullline("Did not execute ExportResult due to input error. Please check the previous messages.")
+        # we still return the tehcnical message as an additional log
+        the_lw.WriteFullline(str(e))
+        return
+    except Exception as e:
+        the_lw.WriteFullline("Did not execute ExportResult due to general error. Please check the previous messages.")
+        # we still return the tehcnical message as an additional log
+        the_lw.WriteFullline(str(e))
+        return
+    solution_results: List[NXOpen.CAE.SolutionResult] = load_results([post_input])
+    result: NXOpen.CAE.Result = cast(NXOpen.CAE.Result, solution_results[0])
+    result_types: List[NXOpen.CAE.ResultType] = get_result_types([post_input], solution_results)
+    if result_parameters is None:
+        result_parameters: List[NXOpen.CAE.ResultParameters] = get_result_paramaters(result_types, NXOpen.CAE.Result.ShellSection.Maximum, NXOpen.CAE.Result.Component.Xx, False)
+    result_access: NXOpen.CAE.ResultAccess = the_session.ResultManager.CreateResultAccess(result, result_parameters[0])
+    elemental_data: List[float] = result_access.AskElementResultAllComponents(solution_results[0].AskElementIndex(element_label))
+
+    return elemental_data
+
+
 def add_companion_result(solution_name: str, companion_result_file_name: str, reference_type: str = "Structural"):
     """
     Add a companion result to a given solution, by file name
 
     Parameters
     ----------
     solution_name : str
```

### Comparing `nxopentse-0.0.1a7/src/nxopentse/cae/preprocessing.py` & `nxopentse-0.0.1a9/src/nxopentse/cae/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nxopentse-0.0.1a7/src/nxopentse/cae/solving.py` & `nxopentse-0.0.1a9/src/nxopentse/cae/solving.py`

 * *Files identical despite different names*

### Comparing `nxopentse-0.0.1a7/src/nxopentse/tools/general.py` & `nxopentse-0.0.1a9/src/nxopentse/tools/general.py`

 * *Files identical despite different names*

