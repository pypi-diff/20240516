# Comparing `tmp/grasp_planning-0.5.2.tar.gz` & `tmp/grasp_planning-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grasp_planning-0.5.2.tar", max compression
+gzip compressed data, was "grasp_planning-0.5.3.tar", max compression
```

## Comparing `grasp_planning-0.5.2.tar` & `grasp_planning-0.5.3.tar`

### file list

```diff
@@ -1,25 +1,18 @@
--rw-r--r--   0        0        0     1711 2024-05-14 12:21:39.645718 grasp_planning-0.5.2/README.md
--rw-r--r--   0        0        0      123 2024-05-07 16:34:01.834623 grasp_planning-0.5.2/grasp_planning/__init__.py
--rw-r--r--   0        0        0     1335 2024-05-13 14:27:59.161140 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/collision_constraint.cpython-38.pyc
--rw-r--r--   0        0        0      799 2024-05-13 12:55:10.134092 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/constraint_template.cpython-38.pyc
--rw-r--r--   0        0        0      411 2024-05-08 08:43:17.328729 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/constraints.cpython-38.pyc
--rw-r--r--   0        0        0     1331 2024-05-13 12:55:10.134092 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/grasp_pos_constraint.cpython-38.pyc
--rw-r--r--   0        0        0     1528 2024-05-13 13:10:01.879282 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/grasp_rot_constraint.cpython-38.pyc
--rw-r--r--   0        0        0     1557 2024-05-09 15:57:33.554280 grasp_planning-0.5.2/grasp_planning/constraints/__pycache__/manipulation_constraint.cpython-38.pyc
--rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884832 grasp_planning-0.5.2/grasp_planning/constraints/collision_constraint.py
--rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.2/grasp_planning/constraints/constraint_template.py
--rw-r--r--   0        0        0      252 2024-05-08 08:42:32.500427 grasp_planning-0.5.2/grasp_planning/constraints/constraints.py
--rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452309 grasp_planning-0.5.2/grasp_planning/constraints/grasp_pos_constraint.py
--rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.2/grasp_planning/constraints/grasp_rot_constraint.py
--rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.2/grasp_planning/constraints/manipulation_constraint.py
--rw-r--r--   0        0        0      219 2024-05-07 16:34:48.974947 grasp_planning-0.5.2/grasp_planning/cost/__pycache__/costs.cpython-38.pyc
--rw-r--r--   0        0        0     1344 2024-05-13 08:32:20.007123 grasp_planning-0.5.2/grasp_planning/cost/__pycache__/squared_acc_cost.cpython-38.pyc
--rw-r--r--   0        0        0       65 2024-05-07 16:34:01.834623 grasp_planning-0.5.2/grasp_planning/cost/costs.py
--rw-r--r--   0        0        0        0 2024-05-02 12:00:02.772313 grasp_planning-0.5.2/grasp_planning/cost/dist_to_home.py
--rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.2/grasp_planning/cost/squared_acc_cost.py
--rw-r--r--   0        0        0     5881 2024-05-14 14:48:45.786607 grasp_planning-0.5.2/grasp_planning/solver/__pycache__/gomp_planner.cpython-38.pyc
--rw-r--r--   0        0        0     2207 2024-05-14 14:05:14.682867 grasp_planning-0.5.2/grasp_planning/solver/__pycache__/robot_model.cpython-38.pyc
--rw-r--r--   0        0        0     7594 2024-05-14 14:48:28.822517 grasp_planning-0.5.2/grasp_planning/solver/gomp_planner.py
--rw-r--r--   0        0        0     1915 2024-05-14 14:04:42.954341 grasp_planning-0.5.2/grasp_planning/solver/robot_model.py
--rw-r--r--   0        0        0      450 2024-05-14 14:55:59.628741 grasp_planning-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     2353 1970-01-01 00:00:00.000000 grasp_planning-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1940 2024-05-15 08:31:46.546248 grasp_planning-0.5.3/README.md
+-rw-r--r--   0        0        0      175 2024-05-15 09:11:31.290902 grasp_planning-0.5.3/grasp_planning/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-13 14:27:19.884831 grasp_planning-0.5.3/grasp_planning/constraints/collision_constraint.py
+-rw-r--r--   0        0        0      226 2024-05-13 12:54:20.897417 grasp_planning-0.5.3/grasp_planning/constraints/constraint_template.py
+-rw-r--r--   0        0        0      375 2024-05-15 09:08:01.061356 grasp_planning-0.5.3/grasp_planning/constraints/constraints.py
+-rw-r--r--   0        0        0     1057 2024-05-13 12:38:19.452308 grasp_planning-0.5.3/grasp_planning/constraints/grasp_pos_constraint.py
+-rw-r--r--   0        0        0     1334 2024-05-13 13:10:00.135267 grasp_planning-0.5.3/grasp_planning/constraints/grasp_rot_constraint.py
+-rw-r--r--   0        0        0     1059 2024-05-09 15:55:53.313730 grasp_planning-0.5.3/grasp_planning/constraints/manipulation_constraint.py
+-rw-r--r--   0        0        0     1071 2024-05-15 09:07:33.253161 grasp_planning-0.5.3/grasp_planning/constraints/orientation_constraint.py
+-rw-r--r--   0        0        0     1023 2024-05-15 09:03:10.755469 grasp_planning-0.5.3/grasp_planning/constraints/position_constraint.py
+-rw-r--r--   0        0        0      120 2024-05-15 08:53:23.992220 grasp_planning-0.5.3/grasp_planning/cost/costs.py
+-rw-r--r--   0        0        0      424 2024-05-15 08:53:06.312040 grasp_planning-0.5.3/grasp_planning/cost/dist_to_home.py
+-rw-r--r--   0        0        0     1439 2024-05-13 08:29:45.664854 grasp_planning-0.5.3/grasp_planning/cost/squared_acc_cost.py
+-rw-r--r--   0        0        0     7603 2024-05-15 08:38:17.450744 grasp_planning-0.5.3/grasp_planning/solver/gomp_planner.py
+-rw-r--r--   0        0        0     5326 2024-05-15 09:24:17.669132 grasp_planning-0.5.3/grasp_planning/solver/ik_optim.py
+-rw-r--r--   0        0        0     1992 2024-05-15 08:35:25.352819 grasp_planning-0.5.3/grasp_planning/solver/robot_model.py
+-rw-r--r--   0        0        0      555 2024-05-15 09:29:35.627838 grasp_planning-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2696 1970-01-01 00:00:00.000000 grasp_planning-0.5.3/PKG-INFO
```

### Comparing `grasp_planning-0.5.2/README.md` & `grasp_planning-0.5.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -44,8 +44,14 @@
 x, solver_flag = planner.solve()
 end = time.time()
 print(f"Computational time: {end-start}" )
 print(f"Solver status: {solver_flag}" )
 ```
 
 ## ToDo
-- [ ] removing constraints
+- [ ] removing constraints
+- [ ] automatic constraints for collisions
+
+1. zacni riesit to ze nejde mi parametre
+
+- trebalo poriesit ze kazde zavolanie add collision vytvori premennu pre obstacle
+- idealne poriesit aby sa zadaval aj parent link pre koliziu
```

### Comparing `grasp_planning-0.5.2/grasp_planning/constraints/collision_constraint.py` & `grasp_planning-0.5.3/grasp_planning/constraints/collision_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.2/grasp_planning/constraints/grasp_pos_constraint.py` & `grasp_planning-0.5.3/grasp_planning/constraints/grasp_pos_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.2/grasp_planning/constraints/grasp_rot_constraint.py` & `grasp_planning-0.5.3/grasp_planning/constraints/grasp_rot_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.2/grasp_planning/constraints/manipulation_constraint.py` & `grasp_planning-0.5.3/grasp_planning/constraints/manipulation_constraint.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.2/grasp_planning/cost/squared_acc_cost.py` & `grasp_planning-0.5.3/grasp_planning/cost/squared_acc_cost.py`

 * *Files identical despite different names*

### Comparing `grasp_planning-0.5.2/grasp_planning/solver/gomp_planner.py` & `grasp_planning-0.5.3/grasp_planning/solver/gomp_planner.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         
     def solve(self):
         result = self.solver(x0=self.x_init,
                              lbg=self.g_lb,
                              ubg=self.g_ub,
                              lbx=self.l_joint_limits.reshape((-1,1), order='F'),
                              ubx=self.u_joint_limits.reshape((-1,1), order='F'),
-                             p=self.T_W_Grasp)
+                             p=self.params_optim_num)
 
         success_flag = self.solver.stats()["success"]
         success_msg = self.solver.stats()["return_status"]
         return  result['x'].reshape((self.n_dofs, self.n_waypoints)), success_flag
 
     def _add_grasp_pos_constraint(self, waypoint_ID, tolerance=0.0):
         self.g_list.append(GraspPosConstraint(self._robot_model, 
@@ -177,8 +177,9 @@
     def update_constraints_params(self, T_W_Obj, T_W_Obst=None):
         self.update_object_pose(T_W_Obj)
         self.update_grasp_DOF(theta=self.theta, degrees=False)
 
         if self._collision_flag:
             self.params_optim_num = ca.vertcat(self.T_W_Grasp, T_W_Obst)
         else:
-            self.params_optim_num = self.T_W_Grasp
+            self.params_optim_num = self.T_W_Grasp
+
```

### Comparing `grasp_planning-0.5.2/grasp_planning/solver/robot_model.py` & `grasp_planning-0.5.3/grasp_planning/solver/robot_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,8 +46,9 @@
                 self.joint_pos_limits[i] = [joint.limit.lower, joint.limit.upper]
                 i += 1
 
 
     def get_joint_pos_limits(self):
         return self.joint_pos_limits
 
-
+    def get_link_names(self):
+        return self.robot_fk.robot.link_names()
```

### Comparing `grasp_planning-0.5.2/PKG-INFO` & `grasp_planning-0.5.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: grasp_planning
-Version: 0.5.2
+Version: 0.5.3
 Summary: "Grasp and Motion Planning Python Package."
+Home-page: https://github.com/TomasMerva/gomp.git
 License: MIT
 Author: Tomas Merva
 Author-email: tmerva7@gmail.com
 Requires-Python: >=3.8,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: casadi (>=3.6,<4.0)
 Requires-Dist: forwardkinematics (>=1.1.3)
 Requires-Dist: numpy (>=1.15.3,<2.0.0)
 Requires-Dist: scipy (<=1.10.1)
 Requires-Dist: spatial-casadi (>=1.1.0,<2.0.0)
+Project-URL: Repository, https://github.com/TomasMerva/gomp.git
 Description-Content-Type: text/markdown
 
 This package provides grasp and motion planning using CasADi and IPOPT. 
 
 
 ## Usage
 ```python
@@ -64,7 +66,13 @@
 end = time.time()
 print(f"Computational time: {end-start}" )
 print(f"Solver status: {solver_flag}" )
 ```
 
 ## ToDo
 - [ ] removing constraints
+- [ ] automatic constraints for collisions
+
+1. zacni riesit to ze nejde mi parametre
+
+- trebalo poriesit ze kazde zavolanie add collision vytvori premennu pre obstacle
+- idealne poriesit aby sa zadaval aj parent link pre koliziu
```

