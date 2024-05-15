# Comparing `tmp/deeprecsys-0.2.5.tar.gz` & `tmp/deeprecsys-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeprecsys-0.2.5.tar", max compression
+gzip compressed data, was "deeprecsys-0.2.6.tar", max compression
```

## Comparing `deeprecsys-0.2.5.tar` & `deeprecsys-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    35149 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/LICENSE
--rw-r--r--   0        0        0     2079 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/README.md
--rw-r--r--   0        0        0        0 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/deeprecsys/__init__.py
--rw-r--r--   0        0        0     2950 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/deeprecsys/neural_networks/base_network.py
--rw-r--r--   0        0        0     1204 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/deeprecsys/neural_networks/binary_classifier.py
--rw-r--r--   0        0        0     3564 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/deeprecsys/neural_networks/deep_q_network.py
--rw-r--r--   0        0        0     6820 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/dueling.py
--rw-r--r--   0        0        0     3781 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/gaussian_actor.py
--rw-r--r--   0        0        0     1726 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/noisy_layer.py
--rw-r--r--   0        0        0     2960 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/policy_estimator.py
--rw-r--r--   0        0        0     3195 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/q_value_estimator.py
--rw-r--r--   0        0        0     1607 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/value_estimator.py
--rw-r--r--   0        0        0      800 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/__init__.py
--rw-r--r--   0        0        0     3723 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/actor_critic.py
--rw-r--r--   0        0        0     1683 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/agent.py
--rw-r--r--   0        0        0     3322 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/dqn.py
--rw-r--r--   0        0        0     1719 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/epsilon_greedy.py
--rw-r--r--   0        0        0     4344 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/rainbow.py
--rw-r--r--   0        0        0     3806 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/agents/reinforce.py
--rw-r--r--   0        0        0     6452 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/agents/soft_actor_critic.py
--rw-r--r--   0        0        0     1340 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/experience_replay/buffer_parameters.py
--rw-r--r--   0        0        0     2829 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/experience_replay/experience_buffer.py
--rw-r--r--   0        0        0     4982 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/experience_replay/priority_replay_buffer.py
--rw-r--r--   0        0        0     3157 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/learning_statistics.py
--rw-r--r--   0        0        0     9864 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/manager.py
--rw-r--r--   0        0        0     2048 2024-05-15 21:58:38.818828 deeprecsys-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 deeprecsys-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/LICENSE
+-rw-r--r--   0        0        0     2079 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/deeprecsys/__init__.py
+-rw-r--r--   0        0        0     2950 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/deeprecsys/neural_networks/base_network.py
+-rw-r--r--   0        0        0     1204 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/deeprecsys/neural_networks/binary_classifier.py
+-rw-r--r--   0        0        0     3564 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/deeprecsys/neural_networks/deep_q_network.py
+-rw-r--r--   0        0        0     6820 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/deeprecsys/neural_networks/dueling.py
+-rw-r--r--   0        0        0     3781 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/deeprecsys/neural_networks/gaussian_actor.py
+-rw-r--r--   0        0        0     1726 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/deeprecsys/neural_networks/noisy_layer.py
+-rw-r--r--   0        0        0     2960 2024-05-15 22:11:10.831702 deeprecsys-0.2.6/deeprecsys/neural_networks/policy_estimator.py
+-rw-r--r--   0        0        0     3195 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/neural_networks/q_value_estimator.py
+-rw-r--r--   0        0        0     1607 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/neural_networks/value_estimator.py
+-rw-r--r--   0        0        0      800 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/__init__.py
+-rw-r--r--   0        0        0     3723 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/agents/actor_critic.py
+-rw-r--r--   0        0        0     1683 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/agents/agent.py
+-rw-r--r--   0        0        0     3322 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/agents/dqn.py
+-rw-r--r--   0        0        0     1719 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/agents/epsilon_greedy.py
+-rw-r--r--   0        0        0     4344 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/agents/rainbow.py
+-rw-r--r--   0        0        0     3806 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/agents/reinforce.py
+-rw-r--r--   0        0        0     6452 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/agents/soft_actor_critic.py
+-rw-r--r--   0        0        0     1340 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/experience_replay/buffer_parameters.py
+-rw-r--r--   0        0        0     2829 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/experience_replay/experience_buffer.py
+-rw-r--r--   0        0        0     4982 2024-05-15 22:11:10.832702 deeprecsys-0.2.6/deeprecsys/rl/experience_replay/priority_replay_buffer.py
+-rw-r--r--   0        0        0     3157 2024-05-15 22:11:10.833701 deeprecsys-0.2.6/deeprecsys/rl/learning_statistics.py
+-rw-r--r--   0        0        0     9864 2024-05-15 22:11:10.833701 deeprecsys-0.2.6/deeprecsys/rl/manager.py
+-rw-r--r--   0        0        0     2048 2024-05-15 22:13:41.547655 deeprecsys-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 deeprecsys-0.2.6/PKG-INFO
```

### Comparing `deeprecsys-0.2.5/LICENSE` & `deeprecsys-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/README.md` & `deeprecsys-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/neural_networks/base_network.py` & `deeprecsys-0.2.6/deeprecsys/neural_networks/base_network.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/neural_networks/binary_classifier.py` & `deeprecsys-0.2.6/deeprecsys/neural_networks/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/neural_networks/deep_q_network.py` & `deeprecsys-0.2.6/deeprecsys/neural_networks/deep_q_network.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/neural_networks/dueling.py` & `deeprecsys-0.2.6/deeprecsys/neural_networks/dueling.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/neural_networks/gaussian_actor.py` & `deeprecsys-0.2.6/deeprecsys/neural_networks/gaussian_actor.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/neural_networks/noisy_layer.py` & `deeprecsys-0.2.6/deeprecsys/neural_networks/noisy_layer.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/neural_networks/policy_estimator.py` & `deeprecsys-0.2.6/deeprecsys/neural_networks/policy_estimator.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/neural_networks/q_value_estimator.py` & `deeprecsys-0.2.6/deeprecsys/neural_networks/q_value_estimator.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/neural_networks/value_estimator.py` & `deeprecsys-0.2.6/deeprecsys/neural_networks/value_estimator.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/__init__.py` & `deeprecsys-0.2.6/deeprecsys/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/agents/actor_critic.py` & `deeprecsys-0.2.6/deeprecsys/rl/agents/actor_critic.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/agents/agent.py` & `deeprecsys-0.2.6/deeprecsys/rl/agents/agent.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/agents/dqn.py` & `deeprecsys-0.2.6/deeprecsys/rl/agents/dqn.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/agents/epsilon_greedy.py` & `deeprecsys-0.2.6/deeprecsys/rl/agents/epsilon_greedy.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/agents/rainbow.py` & `deeprecsys-0.2.6/deeprecsys/rl/agents/rainbow.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/agents/reinforce.py` & `deeprecsys-0.2.6/deeprecsys/rl/agents/reinforce.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/agents/soft_actor_critic.py` & `deeprecsys-0.2.6/deeprecsys/rl/agents/soft_actor_critic.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/experience_replay/buffer_parameters.py` & `deeprecsys-0.2.6/deeprecsys/rl/experience_replay/buffer_parameters.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/experience_replay/experience_buffer.py` & `deeprecsys-0.2.6/deeprecsys/rl/experience_replay/experience_buffer.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/experience_replay/priority_replay_buffer.py` & `deeprecsys-0.2.6/deeprecsys/rl/experience_replay/priority_replay_buffer.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/learning_statistics.py` & `deeprecsys-0.2.6/deeprecsys/rl/learning_statistics.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/deeprecsys/rl/manager.py` & `deeprecsys-0.2.6/deeprecsys/rl/manager.py`

 * *Files identical despite different names*

### Comparing `deeprecsys-0.2.5/pyproject.toml` & `deeprecsys-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deeprecsys"
-version = "0.2.5"
+version = "0.2.6"
 description = "deeprecsys is an open tool belt to speed up the development of modern data science projects at an enterprise level"
 authors = ["Lucas Farris <lucas@farris.com.br>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://deeprecsys.com"
 repository = "https://github.com/luksfarris/deeprecsys"
 documentation = "https://deeprecsys.com"
```

### Comparing `deeprecsys-0.2.5/PKG-INFO` & `deeprecsys-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeprecsys
-Version: 0.2.5
+Version: 0.2.6
 Summary: deeprecsys is an open tool belt to speed up the development of modern data science projects at an enterprise level
 Home-page: https://deeprecsys.com
 License: GPL-3.0-or-later
 Keywords: machinelearning,reinforcementlearning,recommmendersystems,deeplearning,datascience
 Author: Lucas Farris
 Author-email: lucas@farris.com.br
 Requires-Python: >=3.9,<4
```

