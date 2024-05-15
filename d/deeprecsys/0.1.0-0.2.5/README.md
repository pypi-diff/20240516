# Comparing `tmp/deeprecsys-0.1.0.tar.gz` & `tmp/deeprecsys-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeprecsys-0.1.0.tar", max compression
+gzip compressed data, was "deeprecsys-0.2.5.tar", max compression
```

## Comparing `deeprecsys-0.1.0.tar` & `deeprecsys-0.2.5.tar`

### file list

```diff
@@ -1,41 +1,27 @@
--rw-r--r--   0        0        0     1069 2022-07-11 19:30:05.031179 deeprecsys-0.1.0/LICENSE
--rw-r--r--   0        0        0        0 2022-07-11 19:30:05.036179 deeprecsys-0.1.0/deeprecsys/__init__.py
--rw-r--r--   0        0        0     7557 2022-07-11 20:04:31.178612 deeprecsys-0.1.0/deeprecsys/movielens_fairness_env.py
--rw-r--r--   0        0        0        0 2022-07-11 19:30:05.036179 deeprecsys-0.1.0/deeprecsys/rl/__init__.py
--rw-r--r--   0        0        0     3362 2022-07-11 20:03:27.886893 deeprecsys-0.1.0/deeprecsys/rl/agents/actor_critic.py
--rw-r--r--   0        0        0     1155 2022-07-11 19:30:05.036179 deeprecsys-0.1.0/deeprecsys/rl/agents/agent.py
--rw-r--r--   0        0        0     3139 2022-07-11 20:03:27.897888 deeprecsys-0.1.0/deeprecsys/rl/agents/dqn.py
--rw-r--r--   0        0        0     1476 2022-07-11 19:30:05.036179 deeprecsys-0.1.0/deeprecsys/rl/agents/epsilon_greedy.py
--rw-r--r--   0        0        0     4027 2022-07-11 20:03:27.972859 deeprecsys-0.1.0/deeprecsys/rl/agents/rainbow.py
--rw-r--r--   0        0        0     3210 2022-07-11 20:03:27.756944 deeprecsys-0.1.0/deeprecsys/rl/agents/reinforce.py
--rw-r--r--   0        0        0     5867 2022-07-11 20:03:27.956865 deeprecsys-0.1.0/deeprecsys/rl/agents/soft_actor_critic.py
--rw-r--r--   0        0        0     1177 2022-07-11 19:30:05.036179 deeprecsys-0.1.0/deeprecsys/rl/experience_replay/buffer_parameters.py
--rw-r--r--   0        0        0     2274 2022-07-11 20:03:27.930875 deeprecsys-0.1.0/deeprecsys/rl/experience_replay/experience_buffer.py
--rw-r--r--   0        0        0     4438 2022-07-11 20:03:27.991851 deeprecsys-0.1.0/deeprecsys/rl/experience_replay/priority_replay_buffer.py
--rw-r--r--   0        0        0     2479 2022-07-11 19:30:05.036179 deeprecsys-0.1.0/deeprecsys/rl/learning_statistics.py
--rw-r--r--   0        0        0     8790 2022-07-11 20:03:27.862902 deeprecsys-0.1.0/deeprecsys/rl/manager.py
--rw-r--r--   0        0        0     2434 2022-07-11 19:30:05.036179 deeprecsys-0.1.0/deeprecsys/rl/neural_networks/base_network.py
--rw-r--r--   0        0        0     3378 2022-07-11 20:03:28.008844 deeprecsys-0.1.0/deeprecsys/rl/neural_networks/deep_q_network.py
--rw-r--r--   0        0        0     6685 2022-07-11 20:03:27.979856 deeprecsys-0.1.0/deeprecsys/rl/neural_networks/dueling.py
--rw-r--r--   0        0        0     3422 2022-07-11 20:03:27.941871 deeprecsys-0.1.0/deeprecsys/rl/neural_networks/gaussian_actor.py
--rw-r--r--   0        0        0     1252 2022-07-11 19:30:05.037179 deeprecsys-0.1.0/deeprecsys/rl/neural_networks/noisy_layer.py
--rw-r--r--   0        0        0     2457 2022-07-11 20:03:27.946869 deeprecsys-0.1.0/deeprecsys/rl/neural_networks/policy_estimator.py
--rw-r--r--   0        0        0     2669 2022-07-11 20:03:28.015842 deeprecsys-0.1.0/deeprecsys/rl/neural_networks/q_value_estimator.py
--rw-r--r--   0        0        0     1381 2022-07-11 20:03:27.915881 deeprecsys-0.1.0/deeprecsys/rl/neural_networks/value_estimator.py
--rw-r--r--   0        0        0        0 2022-07-11 19:30:05.037179 deeprecsys-0.1.0/deeprecsys/tests/__init__.py
--rw-r--r--   0        0        0      579 2022-07-11 19:30:05.037179 deeprecsys-0.1.0/deeprecsys/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-07-11 19:30:05.037179 deeprecsys-0.1.0/deeprecsys/tests/unit/__init__.py
--rw-r--r--   0        0        0      783 2022-07-11 20:03:27.905885 deeprecsys-0.1.0/deeprecsys/tests/unit/test_actor_critic.py
--rw-r--r--   0        0        0     1698 2022-07-11 20:03:28.021839 deeprecsys-0.1.0/deeprecsys/tests/unit/test_base_networks.py
--rw-r--r--   0        0        0      620 2022-07-11 20:03:27.937873 deeprecsys-0.1.0/deeprecsys/tests/unit/test_epsilon_greedy.py
--rw-r--r--   0        0        0     1079 2022-07-11 20:03:27.997849 deeprecsys-0.1.0/deeprecsys/tests/unit/test_manager.py
--rw-r--r--   0        0        0     1256 2022-07-11 20:03:27.952866 deeprecsys-0.1.0/deeprecsys/tests/unit/test_movielens_fairness_env.py
--rw-r--r--   0        0        0     1044 2022-07-11 20:03:27.923878 deeprecsys-0.1.0/deeprecsys/tests/unit/test_rainbow_agent.py
--rw-r--r--   0        0        0     1155 2022-07-11 20:03:27.987853 deeprecsys-0.1.0/deeprecsys/tests/unit/test_random_agent.py
--rw-r--r--   0        0        0      707 2022-07-11 20:03:28.001847 deeprecsys-0.1.0/deeprecsys/tests/unit/test_reinforce_agent.py
--rw-r--r--   0        0        0     2463 2022-07-11 20:03:27.967861 deeprecsys-0.1.0/deeprecsys/tests/unit/test_reproducibility.py
--rw-r--r--   0        0        0     1776 2022-07-11 20:03:27.963862 deeprecsys-0.1.0/deeprecsys/tests/unit/test_sac_agent.py
--rw-r--r--   0        0        0     1209 2022-07-11 20:03:28.004846 deeprecsys-0.1.0/deeprecsys/tests/unit/test_slate_training.py
--rw-r--r--   0        0        0     1191 2022-07-11 20:02:56.922243 deeprecsys-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1010 2022-07-11 20:04:49.249047 deeprecsys-0.1.0/setup.py
--rw-r--r--   0        0        0      721 2022-07-11 20:04:49.249566 deeprecsys-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2079 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/deeprecsys/__init__.py
+-rw-r--r--   0        0        0     2950 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/deeprecsys/neural_networks/base_network.py
+-rw-r--r--   0        0        0     1204 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/deeprecsys/neural_networks/binary_classifier.py
+-rw-r--r--   0        0        0     3564 2024-05-15 21:56:21.104316 deeprecsys-0.2.5/deeprecsys/neural_networks/deep_q_network.py
+-rw-r--r--   0        0        0     6820 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/dueling.py
+-rw-r--r--   0        0        0     3781 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/gaussian_actor.py
+-rw-r--r--   0        0        0     1726 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/noisy_layer.py
+-rw-r--r--   0        0        0     2960 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/policy_estimator.py
+-rw-r--r--   0        0        0     3195 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/q_value_estimator.py
+-rw-r--r--   0        0        0     1607 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/neural_networks/value_estimator.py
+-rw-r--r--   0        0        0      800 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/__init__.py
+-rw-r--r--   0        0        0     3723 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/actor_critic.py
+-rw-r--r--   0        0        0     1683 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/agent.py
+-rw-r--r--   0        0        0     3322 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/dqn.py
+-rw-r--r--   0        0        0     1719 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/epsilon_greedy.py
+-rw-r--r--   0        0        0     4344 2024-05-15 21:56:21.105316 deeprecsys-0.2.5/deeprecsys/rl/agents/rainbow.py
+-rw-r--r--   0        0        0     3806 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/agents/reinforce.py
+-rw-r--r--   0        0        0     6452 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/agents/soft_actor_critic.py
+-rw-r--r--   0        0        0     1340 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/experience_replay/buffer_parameters.py
+-rw-r--r--   0        0        0     2829 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/experience_replay/experience_buffer.py
+-rw-r--r--   0        0        0     4982 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/experience_replay/priority_replay_buffer.py
+-rw-r--r--   0        0        0     3157 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/learning_statistics.py
+-rw-r--r--   0        0        0     9864 2024-05-15 21:56:21.106316 deeprecsys-0.2.5/deeprecsys/rl/manager.py
+-rw-r--r--   0        0        0     2048 2024-05-15 21:58:38.818828 deeprecsys-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 deeprecsys-0.2.5/PKG-INFO
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/agents/actor_critic.py` & `deeprecsys-0.2.5/deeprecsys/rl/agents/reinforce.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,91 @@
-from deeprecsys.rl.agents.agent import ReinforcementLearning
 from typing import Any, List, Optional
-from deeprecsys.rl.experience_replay.experience_buffer import ExperienceReplayBuffer
+
+import numpy as np
+from torch import FloatTensor
+
+from deeprecsys.neural_networks.policy_estimator import PolicyEstimator
+from deeprecsys.rl.agents.agent import ReinforcementLearning
 from deeprecsys.rl.experience_replay.buffer_parameters import (
     ExperienceReplayBufferParameters,
 )
-from deeprecsys.rl.neural_networks.policy_estimator import PolicyEstimator
-from deeprecsys.rl.neural_networks.value_estimator import ValueEstimator
+from deeprecsys.rl.experience_replay.experience_buffer import ExperienceReplayBuffer
 
 
-class ActorCriticAgent(ReinforcementLearning):
-    """Policy estimator using a value estimator as a baseline.
+class ReinforceAgent(ReinforcementLearning):
+    """REINFORCE: Policy estimator using a value estimator as a baseline.
     It's on-policy, for discrete action spaces, and episodic environments.
-    This implementation uses stochastic policies.
-    TODO: could be a sub class of reinforce"""
+    """
+
+    buffer: ExperienceReplayBuffer
 
     def __init__(
         self,
         n_actions: int,
         state_size: int,
-        discount_factor: int = 0.99,
-        actor_hidden_layers: Optional[List[int]] = None,
-        critic_hidden_layers: Optional[List[int]] = None,
-        actor_learning_rate=1e-3,
-        critic_learning_rate=1e-3,
+        hidden_layers: Optional[List[int]] = None,
+        discount_factor: float = 0.99,
+        learning_rate: float = 1e-3,
     ):
-        if not actor_hidden_layers:
-            actor_hidden_layers = [state_size * 2, state_size * 2]
-        if not critic_hidden_layers:
-            critic_hidden_layers = [state_size * 2, int(state_size / 2)]
+        """Start the network with the parameters provided.
+        The discount factor is commonly known as gamma.
+        """
         self.episode_count = 0
-        self.value_estimator = ValueEstimator(
-            state_size,
-            critic_hidden_layers,
-            1,
-            learning_rate=critic_learning_rate,
-        )
+        if not hidden_layers:
+            hidden_layers = [state_size * 2, state_size * 2]
         self.policy_estimator = PolicyEstimator(
             state_size,
-            actor_hidden_layers,
+            hidden_layers,
             n_actions,
-            learning_rate=actor_learning_rate,
+            learning_rate=learning_rate,
         )
         self.discount_factor = discount_factor
         # starts the buffer
         self.reset_buffer()
 
-    def reset_buffer(self):
-        self.buffer = ExperienceReplayBuffer(
-            ExperienceReplayBufferParameters(10000, 1, 1)
-        )
+    def reset_buffer(self) -> None:
+        """Recreate the experience buffer, effectively forgetting all the experiences
+        collected so far.
+        """
+        self.buffer = ExperienceReplayBuffer(ExperienceReplayBufferParameters(10000, 1, 1))
 
     def top_k_actions_for_state(self, state: Any, k: int = 1) -> List[int]:
+        """Return the k next best actions for the given state."""
         return self.policy_estimator.predict(state, k=k)
 
     def action_for_state(self, state: Any) -> int:
+        """Return the best action for the given state."""
         return self.top_k_actions_for_state(state)[0]
 
-    def store_experience(
-        self, state: Any, action: Any, reward: float, done: bool, new_state: Any
-    ):
+    def store_experience(self, state: Any, action: Any, reward: float, done: bool, new_state: Any) -> None:
+        """Store the experience in the buffer and run the backpropagation if the buffer is ready."""
         state_flat = state.flatten()
         new_state_flat = new_state.flatten()
         self.buffer.store_experience(state_flat, action, reward, done, new_state_flat)
         # FIXME: should learn after every episode, or after every N experiences?
         if done:  # and self.buffer.ready_to_predict():
             self.learn_from_experiences()
             self.reset_buffer()
 
-    def learn_from_experiences(self):
+    def discounted_rewards(self, rewards: np.array) -> np.array:
+        """From a list of rewards obtained in an episode, we calculate
+        the return minus the baseline. The baseline is the list of discounted
+        rewards minus the mean, divided by the standard deviation.
+        """
+        discount_r = np.zeros_like(rewards)
+        timesteps = range(len(rewards))
+        reward_sum = 0
+        for i in reversed(timesteps):
+            reward_sum = rewards[i] + self.discount_factor * reward_sum
+            discount_r[i] = reward_sum
+        return_mean = discount_r.mean()
+        return_std = discount_r.std()
+        baseline = (discount_r - return_mean) / return_std
+        return baseline
+
+    def learn_from_experiences(self) -> None:
+        """Train the policy estimator with all the experiences collected so far."""
         experiences = list(self.buffer.experience_queue)
-        for timestep, experience in enumerate(experiences):
-            total_return = 0
-            for i, t in enumerate(experiences[timestep:]):
-                total_return += (self.discount_factor ** i) * t.reward
-
-            # Calculate baseline/advantage
-            baseline_value = self.value_estimator.predict(experience.state).detach()
-            advantage = total_return - baseline_value
-            # Update our value estimator
-            self.value_estimator.update(experience.state, total_return)
-            # Update our policy estimator
-            self.policy_estimator.update(experience.state, advantage, experience.action)
+        states, actions, rewards, dones, next_states = zip(*experiences, strict=False)
+        advantages = self.discounted_rewards(rewards)
+        advantages_tensor = FloatTensor(advantages).to(device=self.policy_estimator.device)
+        self.policy_estimator.update(states, advantages_tensor, actions)
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/agents/agent.py` & `deeprecsys-0.2.5/deeprecsys/rl/agents/agent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 from abc import ABC, abstractmethod
-from gym import Space
 from typing import Any
 
+from gymnasium import Space
+
 
 class ReinforcementLearning(ABC):
+    """Abstract class that encapsulates the behavior of RL models."""
+
     @abstractmethod
     def action_for_state(self, state: Any) -> Any:
-        pass
+        """Given a state, return the next predicted action."""
 
     @abstractmethod
     def top_k_actions_for_state(self, state: Any, k: int = 1) -> Any:
-        pass
+        """Retrieve the next K best actions for this state."""
 
     @abstractmethod
-    def store_experience(
-        self, state: Any, action: Any, reward: float, done: bool, new_state: Any
-    ):
-        pass
+    def store_experience(self, state: Any, action: Any, reward: float, done: bool, new_state: Any) -> None:
+        """Store an experience (used in case of experience replay buffers)"""
 
 
 class RandomAgent(ReinforcementLearning):
     """An agent that randomly samples actions, regardless of the
-    environment's state."""
+    environment's state.
+    """
 
     action_space: Space
 
-    def __init__(self, action_space: Space, random_state=42):
+    def __init__(self, action_space: Space, random_state: Any = 42):
+        """Start the agent with the provided action space and seed."""
         self.action_space = action_space
         # we seed the state so actions are reproducible
         self.action_space.seed(random_state)
 
     def action_for_state(self, state: Any) -> Any:
+        """Sample a random action from the action space."""
         return self.action_space.sample()
 
     def top_k_actions_for_state(self, state: Any, k: int = 1) -> Any:
+        """Randomly sample K actions from the action space."""
         return self.action_space.sample()
 
-    def store_experience(
-        self, state: Any, action: Any, reward: float, done: bool, new_state: Any
-    ):
+    def store_experience(self, state: Any, action: Any, reward: float, done: bool, new_state: Any) -> None:
+        """Ignore the experience because this agent doesn't have any experience replay."""
         pass
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/agents/dqn.py` & `deeprecsys-0.2.5/deeprecsys/rl/agents/dqn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,91 +1,95 @@
-from numpy.random import RandomState
-from typing import List, Any
+from typing import Any, List, Optional
+
 from numpy import arange
-from deeprecsys.rl.experience_replay.experience_buffer import ExperienceReplayBuffer
-from deeprecsys.rl.experience_replay.buffer_parameters import (
-    ExperienceReplayBufferParameters,
-)
-from deeprecsys.rl.agents.epsilon_greedy import DecayingEpsilonGreedy
-from deeprecsys.rl.neural_networks.deep_q_network import (
+from numpy.random import RandomState
+
+from deeprecsys.neural_networks.deep_q_network import (
     DeepQNetwork,
     sequential_architecture,
 )
+from deeprecsys.rl.agents.epsilon_greedy import DecayingEpsilonGreedy
+from deeprecsys.rl.experience_replay.buffer_parameters import (
+    ExperienceReplayBufferParameters,
+)
+from deeprecsys.rl.experience_replay.experience_buffer import ExperienceReplayBuffer
 
 
 class DQNAgent(DecayingEpsilonGreedy):
-    """ TODO: This agent needs to be fixed"""
+    """TODO: This agent needs to be fixed"""
 
     def __init__(
         self,
         input_size: int,
         output_size: int,
         hidden_layers: List,
         network_update_frequency: int = 3,
         initial_exploration_probability: float = 1.0,
         decay_rate: float = 0.99,
-        minimum_exploration_probability=0.05,
+        minimum_exploration_probability: float = 0.05,
         buffer_size: int = 10000,
         buffer_burn_in: int = 1000,
         batch_size: int = 32,
         discount_factor: float = 0.99,
         learning_rate: float = 0.99,
-        random_state: RandomState = RandomState(),
-    ):
+        random_state: Optional[RandomState] = None,
+    ) -> None:
+        """TODO"""
+        if random_state is None:
+            random_state = RandomState()
         super().__init__(
             initial_exploration_probability,
             decay_rate,
             minimum_exploration_probability,
             random_state,
         )
 
-        architecture = sequential_architecture(
-            [input_size] + hidden_layers + [output_size]
-        )
+        architecture = sequential_architecture([input_size] + hidden_layers + [output_size])
         self.network = DeepQNetwork(learning_rate, architecture, discount_factor)
         self.buffer = ExperienceReplayBuffer(
             ExperienceReplayBufferParameters(
                 max_experiences=buffer_size,
                 minimum_experiences_to_start_predicting=buffer_burn_in,
                 batch_size=batch_size,
                 random_state=random_state,
             )
         )
         self.step_count = 0
         self.network_update_frequency = network_update_frequency
         self.actions = arange(output_size)
 
-    def _check_update_network(self):
+    def _check_update_network(self) -> None:
         if self.buffer.ready_to_predict():
             self.step_count += 1
             if self.step_count == self.network_update_frequency:
                 self.step_count = 0
                 batch = self.buffer.sample_batch()
                 self.network.learn_from(batch)
 
     def action_for_state(self, state: Any) -> Any:
+        """TODO"""
         state_flat = state.flatten()
         if self.buffer.ready_to_predict():
             action = super().action_for_state(state_flat)
         else:
             action = self.explore()
         self._check_update_network()
         return action
 
     def top_k_actions_for_state(self, state: Any, k: int = 1) -> Any:
-        # TODO:
-        pass
+        """TODO"""
 
-    def explore(self):
+    def explore(self) -> float:
+        """TODO"""
         return self.random_state.choice(self.actions)
 
-    def exploit(self, state: Any):
+    def exploit(self, state: Any) -> float:
+        """TODO"""
         return self.network.best_action_for_state(state)
 
-    def store_experience(
-        self, state: Any, action: Any, reward: float, done: bool, new_state: Any
-    ):
+    def store_experience(self, state: Any, action: Any, reward: float, done: bool, new_state: Any) -> None:
+        """TODO"""
         if done and self.buffer.ready_to_predict():
             self._decay()
         state_flat = state.flatten()
         new_state_flat = new_state.flatten()
         self.buffer.store_experience(state_flat, action, reward, done, new_state_flat)
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/agents/epsilon_greedy.py` & `deeprecsys-0.2.5/deeprecsys/rl/agents/epsilon_greedy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-from .agent import ReinforcementLearning
 from abc import ABC, abstractmethod
-from numpy.random import RandomState
 from typing import Any
 
+from numpy.random import RandomState
+
+from deeprecsys.rl.agents.agent import ReinforcementLearning
+
 
 class DecayingEpsilonGreedy(ReinforcementLearning, ABC):
+    """A reinforcement learning model that reduces exploration over time."""
+
     def __init__(
         self,
         initial_exploration_probability: float = 0.2,
         decay_rate: float = 1,
-        minimum_exploration_probability=0.01,
-        random_state: RandomState = RandomState(),
+        minimum_exploration_probability: float = 0.01,
+        random_state: RandomState = None,
     ):
+        """To set up a classic e-greedy model, the decay rate needs to be 1."""
+        if random_state is None:
+            random_state = RandomState()
         self.random_state = random_state
         self.epsilon = initial_exploration_probability
         self.minimum_exploration_probability = minimum_exploration_probability
         self.decay_rate = decay_rate
 
     def action_for_state(self, state: Any) -> Any:
         """With probability epsilon, we explore by sampling one of the random available actions.
-        Otherwise we exploit by chosing the action with the highest Q value."""
+        Otherwise we exploit by chosing the action with the highest Q value.
+        """
         if self.random_state.random() < self.epsilon:
             action = self.explore()
         else:
             action = self.exploit(state)
         return action
 
-    def _decay(self):
-        """ Slowly decrease the exploration probability. """
-        self.epsilon = max(
-            self.epsilon * self.decay_rate, self.minimum_exploration_probability
-        )
+    def _decay(self) -> None:
+        """Slowly decrease the exploration probability."""
+        self.epsilon = max(self.epsilon * self.decay_rate, self.minimum_exploration_probability)
 
     @abstractmethod
     def explore(self) -> Any:
-        """ Randomly selects an action"""
+        """Randomly selects an action"""
         pass
 
     @abstractmethod
     def exploit(self, state: Any) -> Any:
-        """ Selects the best action known for the given state """
+        """Select the best action known for the given state"""
         pass
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/agents/rainbow.py` & `deeprecsys-0.2.5/deeprecsys/rl/agents/rainbow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from numpy.random import RandomState
-from typing import Any, Optional, List
-from numpy import arange
 from copy import deepcopy
-from deeprecsys.rl.neural_networks.dueling import DuelingDDQN
-from deeprecsys.rl.experience_replay.priority_replay_buffer import (
-    PrioritizedExperienceReplayBuffer,
-)
+from typing import Any, List, Optional
+
+from numpy import arange
+from numpy.random import RandomState
+
+from deeprecsys.neural_networks.dueling import DuelingDDQN
+from deeprecsys.rl.agents.agent import ReinforcementLearning
 from deeprecsys.rl.experience_replay.buffer_parameters import (
-    PERBufferParameters,
     ExperienceReplayBufferParameters,
+    PERBufferParameters,
+)
+from deeprecsys.rl.experience_replay.priority_replay_buffer import (
+    PrioritizedExperienceReplayBuffer,
 )
-from deeprecsys.rl.agents.agent import ReinforcementLearning
 from deeprecsys.rl.learning_statistics import LearningStatistics
 
 
 class RainbowDQNAgent(ReinforcementLearning):
-
     """Instead of sampling randomly from the buffer we prioritize experiences with PER
     Instead of epsilon-greedy we use gaussian noisy layers for exploration
     Instead of the Q value we calculate Value and Advantage (Dueling DQN).
-    This implementation does not include the Categorical DQN part (yet)."""
+    This implementation does not include the Categorical DQN part (yet).
+    """
 
     def __init__(
         self,
         input_size: int,
         output_size: int,
         network_update_frequency: int = 5,
         network_sync_frequency: int = 200,
@@ -32,18 +34,20 @@
         buffer_size: int = 10000,
         buffer_burn_in: int = 1000,
         batch_size: int = 32,
         noise_sigma: float = 0.017,
         discount_factor: float = 0.99,
         learning_rate: float = 0.0001,
         hidden_layers: List[int] = None,
-        random_state: RandomState = RandomState(),
+        random_state: RandomState = None,
         statistics: Optional[LearningStatistics] = None,
     ):
-
+        """Start the network and the buffer with the provided parameters."""
+        if random_state is None:
+            random_state = RandomState()
         self.network = DuelingDDQN(
             n_input=input_size,
             n_output=output_size,
             learning_rate=learning_rate,
             noise_sigma=noise_sigma,
             discount_factor=discount_factor,
             statistics=statistics,
@@ -65,37 +69,38 @@
         )
         self.step_count = 0
         self.network_update_frequency = network_update_frequency
         self.network_sync_frequency = network_sync_frequency
         self.actions = arange(output_size)
         self.random_state = random_state
 
-    def _check_update_network(self):
+    def _check_update_network(self) -> None:
         # we only start training the network once the buffer is ready
         # (the burn in is filled)
         if self.buffer.ready_to_predict():
             self.step_count += 1
             if self.step_count % self.network_update_frequency == 0:
                 # we train at every K steps
                 self.network.learn_with(self.buffer, self.target_network)
             if self.step_count % self.network_sync_frequency == 0:
                 # at every N steps replaces the target network with the main network
                 self.target_network.load_state_dict(self.network.state_dict())
 
     def top_k_actions_for_state(self, state: Any, k: int = 1) -> Any:
+        """Get the next k best actions for the given state"""
         state_flat = state.flatten()
         if self.buffer.ready_to_predict():
             actions = self.target_network.top_k_actions_for_state(state_flat, k=k)
         else:
             actions = self.random_state.choice(self.actions, size=k)
         self._check_update_network()
         return actions
 
     def action_for_state(self, state: Any) -> Any:
+        """Get the next best action for the given state."""
         return self.top_k_actions_for_state(state, k=1)[0]
 
-    def store_experience(
-        self, state: Any, action: Any, reward: float, done: bool, new_state: Any
-    ):
+    def store_experience(self, state: Any, action: Any, reward: float, done: bool, new_state: Any) -> None:
+        """Store the experience in the buffer"""
         state_flat = state.flatten()
         new_state_flat = new_state.flatten()
         self.buffer.store_experience(state_flat, action, reward, done, new_state_flat)
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/agents/soft_actor_critic.py` & `deeprecsys-0.2.5/deeprecsys/rl/agents/soft_actor_critic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,130 +1,133 @@
 from copy import deepcopy
+from typing import Any, Optional
+
 import torch
-from torch import FloatTensor, BoolTensor
-from typing import Any
-from gym.spaces import Space
-from deeprecsys.rl.neural_networks.gaussian_actor import GaussianActor
-from deeprecsys.rl.neural_networks.q_value_estimator import TwinnedQValueEstimator
+from gymnasium.spaces import Discrete
+from torch import BoolTensor, FloatTensor
+
+from deeprecsys.neural_networks.gaussian_actor import GaussianActor
+from deeprecsys.neural_networks.q_value_estimator import TwinnedQValueEstimator
 from deeprecsys.rl.agents.agent import ReinforcementLearning
-from deeprecsys.rl.experience_replay.priority_replay_buffer import (
-    PrioritizedExperienceReplayBuffer,
-)
 from deeprecsys.rl.experience_replay.buffer_parameters import (
     ExperienceReplayBufferParameters,
     PERBufferParameters,
 )
+from deeprecsys.rl.experience_replay.priority_replay_buffer import (
+    PrioritizedExperienceReplayBuffer,
+)
 
 
 class SoftActorCritic(ReinforcementLearning):
     """TODO: there's things to fix in this agent. It needs temperature
     optimization, and replace the current q-value estimator with the
     Q-value + value + value_target estimators, like described here
-    https://lilianweng.github.io/lil-log/2018/04/08/policy-gradient-algorithms.html"""
+    https://lilianweng.github.io/lil-log/2018/04/08/policy-gradient-algorithms.html
+    """
 
     def __init__(
         self,
-        action_space: Space,
+        action_space: Discrete,
         state_size: int,
         timesteps_to_start_predicting: int = 256,
         learning_rate: float = 0.0001,
         soft_target_update_rate: float = 0.005,
         entropy_coefficient: float = 0.2,
         target_update_interval: int = 2,
         discount_factor: float = 0.99,
-        buffer_parameters=ExperienceReplayBufferParameters(),
-        per_parameters=PERBufferParameters(),
+        buffer_parameters: Optional[ExperienceReplayBufferParameters] = None,
+        per_parameters: Optional[PERBufferParameters] = None,
     ):
-
+        """Initialize the agent and the buffer with the given parameters."""
+        if buffer_parameters is None:
+            buffer_parameters = ExperienceReplayBufferParameters()
+        if per_parameters is None:
+            per_parameters = PERBufferParameters()
         self.action_space = action_space
         n_actions = 1  # TODO: slate size
         self.actor = GaussianActor(
             inputs=state_size,
             outputs=n_actions,
             learning_rate=learning_rate,
             entropy_coefficient=entropy_coefficient,
             discount_factor=discount_factor,
         )
-        self.critic = TwinnedQValueEstimator(
-            inputs=state_size + 1, learning_rate=learning_rate
-        )
+        self.critic = TwinnedQValueEstimator(inputs=state_size + 1, learning_rate=learning_rate)
         self.target_critic = deepcopy(self.critic)
         self.buffer = PrioritizedExperienceReplayBuffer(
-            buffer_parameters=ExperienceReplayBufferParameters(),
-            per_parameters=PERBufferParameters(),
+            buffer_parameters=buffer_parameters,
+            per_parameters=per_parameters,
         )
 
         # disable gradient calculations of the target network
         self.target_critic.disable_learning()
 
         self.timesteps_to_start_predicting = timesteps_to_start_predicting
         self.timesteps = 0
         self.learning_steps = 0  # times the network was trained
         self.tau = soft_target_update_rate
         self.target_update_interval = target_update_interval
         self.gamma = discount_factor
 
-    def should_update_network(self):
+    def should_update_network(self) -> bool:
+        """Check if the buffer is ready to predict and if enough timesteps have passed."""
         return (
-            self.timesteps >= self.timesteps_to_start_predicting
-            and self.buffer.ready_to_predict()  # noqa
+            self.timesteps >= self.timesteps_to_start_predicting and self.buffer.ready_to_predict()  # noqa
         )
 
     def action_for_state(self, state: Any) -> Any:
+        """Before we're ready to start predicting, we return random actions (explore)."""
         if self.timesteps < self.timesteps_to_start_predicting:
             action = self.action_space.sample()
         else:
             action = self.explore(state)
         return int(action)
 
-    def top_k_actions_for_state(self, state, k):
-        # TODO:
+    def top_k_actions_for_state(self, state: Any, k: int = 1) -> Any:
+        """TODO"""
         pass
 
-    def store_experience(
-        self, state: Any, action: Any, reward: float, done: bool, new_state: Any
-    ):
+    def store_experience(self, state: Any, action: Any, reward: float, done: bool, new_state: Any) -> None:
+        """Store the experience in the buffer."""
         self.timesteps += 1
         state_flat = state.flatten()
         new_state_flat = new_state.flatten()
         self.buffer.store_experience(state_flat, action, reward, done, new_state_flat)
         if self.should_update_network():
             self.learn()
 
     def explore(self, state: Any) -> Any:
-        # act with gaussian randomness
+        """Act with gaussian randomness"""
         with torch.no_grad():
             action, _, _ = self.actor.predict(state.reshape(1, -1))
         action_array = action.cpu().numpy().reshape(-1)
         n_actions = self.action_space.n
         return action_array[0].clip(0, n_actions - 1).round()
 
     def exploit(self, state: Any) -> Any:
-        # act without randomness
+        """Act without randomness"""
         with torch.no_grad():
             _, _, action = self.actor.predict(state.reshape(1, -1))
         action_array = action.cpu().numpy().reshape(-1)
         n_actions = self.action_space.n
         return action_array[0].clip(0, n_actions - 1).round()
 
-    def learn(self):
+    def learn(self) -> None:
+        """Run the backpropagation and update the buffer priorities"""
         self.learning_steps += 1
-
         if self.learning_steps % self.target_update_interval == 0:
             # instead of updating the target network "the hard way", we use a Tau
             # parameter as a weighting factor to update the weights as an
             # exponential moving average. This is analogous to the target net update
             # in the DQN algorithm.
             self.target_critic.soft_parameter_update(self.critic, update_rate=self.tau)
 
         # batch with indices and priority weights
         batch = self.buffer.sample_batch()
-        states, actions, rewards, dones, next_states, weights, samples = [
-            i for i in batch
-        ]
+        states, actions, rewards, dones, next_states, weights, samples = [i for i in batch]
         # convert to tensors
         device = self.critic.device
         state_tensors = FloatTensor(states).to(device=device)
         next_state_tensors = FloatTensor(next_states).to(device=device)
         reward_tensors = FloatTensor(rewards).to(device=device).reshape(-1, 1)
         action_tensors = FloatTensor(actions).reshape(-1, 1).to(device=device)
         done_tensors = BoolTensor(dones).to(device=device)
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/experience_replay/buffer_parameters.py` & `deeprecsys-0.2.5/deeprecsys/rl/experience_replay/buffer_parameters.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 from numpy.random import RandomState
 
 
 class ExperienceReplayBufferParameters:
-    """ Parameters to configure an experience replay buffer. """
+    """Parameters to configure an experience replay buffer."""
 
     def __init__(
         self,
         max_experiences: int = 50,
         minimum_experiences_to_start_predicting: int = 32,
         batch_size: int = 32,
-        random_state: RandomState = RandomState(),
+        random_state: RandomState = None,
     ):
+        """Initialize the buffer parameters."""
+        if random_state is None:
+            random_state = RandomState()
         if minimum_experiences_to_start_predicting < batch_size:
             raise ValueError("The batch size mus the larger than the burn in")
         self.max_experiences = max_experiences
-        self.minimum_experiences_to_start_predicting = (
-            minimum_experiences_to_start_predicting
-        )
+        self.minimum_experiences_to_start_predicting = minimum_experiences_to_start_predicting
         self.batch_size = batch_size
         self.random_state = random_state
 
 
 class PERBufferParameters:
-    """Parameters to configure the priorititization of experiences in a
-    Prioritized-Experience Replay Buffer"""
+    """Parameters to configure the prioritization of experiences in a
+    Prioritized-Experience Replay Buffer
+    """
 
     def __init__(
         self,
         beta: float = 0.01,
         beta_growth: float = 0.001,
         alpha: float = 0.6,
         epsilon: float = 0.01,
     ):
+        """Store the parameters referring to the importance sampling."""
         self.beta = beta
         self.beta_growth = beta_growth
         self.alpha = alpha
         self.epsilon = epsilon
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/experience_replay/experience_buffer.py` & `deeprecsys-0.2.5/deeprecsys/rl/experience_replay/experience_buffer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,66 +1,67 @@
 from abc import ABC, abstractmethod
-from collections import namedtuple, deque
-from typing import List, Tuple, Any
+from collections import deque, namedtuple
+from typing import Any, List, Tuple
+
 from deeprecsys.rl.experience_replay.buffer_parameters import (
     ExperienceReplayBufferParameters,
 )
 
-Experience = namedtuple(
+Experience = namedtuple(  # type: ignore
     "Experience", field_names=["state", "action", "reward", "done", "next_state"]
 )
 
 
 class ExperienceBuffer(ABC):
+    """Abstract class encapsulating common aspects of an experience replay buffer."""
+
     @abstractmethod
     def ready_to_predict(self) -> bool:
-        pass
+        """Whether enough experiences were collected"""
 
     @abstractmethod
     def sample_batch(self) -> List[Tuple]:
-        pass
+        """Sample a batch of experiences from the buffer."""
 
     @abstractmethod
-    def store_experience(
-        self, state: Any, action: Any, reward: float, done: bool, next_state: Any
-    ):
-        pass
+    def store_experience(self, state: Any, action: Any, reward: float, done: bool, next_state: Any) -> None:
+        """Store an experience in the buffer."""
 
 
 class ExperienceReplayBuffer(ExperienceBuffer):
+    """Traditional experience replay buffer. Experiences are sampled randomly without
+    replacements within batches. Different batches may contain the same experience.
+    """
+
     def __init__(
         self,
-        parameters=ExperienceReplayBufferParameters(),
+        parameters: ExperienceReplayBufferParameters = None,
     ):
-        self.minimum_experiences_to_start_predicting = (
-            parameters.minimum_experiences_to_start_predicting
-        )
+        """Initialize the buffer with the provided parameters."""
+        if not parameters:
+            parameters = ExperienceReplayBufferParameters()
+        self.minimum_experiences_to_start_predicting = parameters.minimum_experiences_to_start_predicting
         self.random_state = parameters.random_state
         # create double ended queue to store the experiences
-        self.experience_queue = deque(maxlen=parameters.max_experiences)
+        self.experience_queue: List = list(deque(maxlen=parameters.max_experiences))
         self.batch_size = parameters.batch_size
 
     def sample_batch(self) -> List[Tuple]:
-        """ Samples a given number of experiences from the queue """
+        """Sample a given number of experiences from the queue"""
         # samples the index of `batch_size` different experiences from the replay memory
-        samples = self.random_state.choice(
-            len(self.experience_queue), self.batch_size, replace=False
-        )
+        samples = self.random_state.choice(len(self.experience_queue), self.batch_size, replace=False)
         # get the experiences
         experiences = [self.experience_queue[i] for i in samples]
         # returns a flattened list of the samples
-        return zip(*experiences)
+        return zip(*experiences, strict=False)  # type: ignore
 
-    def store_experience(
-        self, state: Any, action: Any, reward: float, done: bool, next_state: Any
-    ):
-        """ Stores a new experience in the queue """
-        experience = Experience(state, action, reward, done, next_state)
+    def store_experience(self, state: Any, action: Any, reward: float, done: bool, next_state: Any) -> None:
+        """Store a new experience in the queue"""
+        experience = Experience(state, action, reward, done, next_state)  # type: ignore
         # append to the right (end) of the queue
         self.experience_queue.append(experience)
 
-    def ready_to_predict(self):
-        """Returns true only if we had enough experiences to start predicting
-        (measured by the burn in)"""
-        return (
-            len(self.experience_queue) >= self.minimum_experiences_to_start_predicting
-        )
+    def ready_to_predict(self) -> bool:
+        """Return true only if we had enough experiences to start predicting
+        (measured by the burn in)
+        """
+        return len(self.experience_queue) >= self.minimum_experiences_to_start_predicting
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/experience_replay/priority_replay_buffer.py` & `deeprecsys-0.2.5/deeprecsys/rl/experience_replay/priority_replay_buffer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,97 +1,106 @@
 from collections import namedtuple
 from typing import Any, List, Tuple
+
 import numpy
+import numpy as np
+
+from deeprecsys.rl.experience_replay.buffer_parameters import (
+    ExperienceReplayBufferParameters,
+    PERBufferParameters,
+)
 from deeprecsys.rl.experience_replay.experience_buffer import (
     Experience,
     ExperienceReplayBuffer,
 )
-from deeprecsys.rl.experience_replay.buffer_parameters import (
-    PERBufferParameters,
-    ExperienceReplayBufferParameters,
-)
-import numpy as np
 
-PriorityExperience = namedtuple(
+PriorityExperience = namedtuple(  # type: ignore
     "PriorityExperience", field_names=["experience", "priority"]
 )
 
 
 class PrioritizedExperienceReplayBuffer(ExperienceReplayBuffer):
+    """Experience Replay Buffer that gives priority to experiences that the network learns more from. We can tell this
+    using the loss. We use importance sampling to avoid bias towards those experiences.
+    """
+
     def __init__(
         self,
-        buffer_parameters=ExperienceReplayBufferParameters(),
-        per_parameters=PERBufferParameters(),
+        buffer_parameters: ExperienceReplayBufferParameters = None,
+        per_parameters: PERBufferParameters = None,
     ):
+        """Start the buffer with the provided parameters."""
+        if not buffer_parameters:
+            buffer_parameters = ExperienceReplayBufferParameters()
+        if not per_parameters:
+            per_parameters = PERBufferParameters()
         super().__init__(buffer_parameters)
         # beta controls the effect of the weights (how much to learn from each
         # experience in the batch)
         self.beta = per_parameters.beta
         self.beta_growth = per_parameters.beta_growth
         # alpha controls the effect of the priority (how much priority is affected
         # by the loss)
         self.alpha = per_parameters.alpha
         # epsilon guarantees no experience has priority zero
         self.epsilon = per_parameters.epsilon
 
     def priorities(self) -> numpy.array:
-        """ Gets the priority for each experience in the queue """
-        return numpy.array(
-            [e.priority for e in self.experience_queue], dtype=numpy.float32
-        )
+        """Get the priority of each experience in the queue"""
+        return numpy.array([e.priority for e in self.experience_queue], dtype=numpy.float32)
 
-    def store_experience(
-        self, state: Any, action: Any, reward: float, done: bool, next_state: Any
-    ):
+    def store_experience(self, state: Any, action: Any, reward: float, done: bool, next_state: Any) -> None:
         """We include a priority to the experience. if the queue is empty, priority is 1 (max),
-        otherwise we check the maximum priority in the queue"""
+        otherwise we check the maximum priority in the queue
+        """
         priorities = self.priorities()
         priority = priorities.max() if len(priorities) > 0 else 1.0
         if not np.isnan(priority):
             experience = Experience(state, action, reward, done, next_state)
-            priority_experience = PriorityExperience(experience, priority)
+            priority_experience = PriorityExperience(experience, priority)  # type: ignore
             # append to the right (end) of the queue
             self.experience_queue.append(priority_experience)
 
-    def update_beta(self):
+    def update_beta(self) -> None:
         """We want to grow the beta value slowly and linearly, starting at a value
-        close to zero, and stopping at 1.0. This is for the Importance Sampling"""
+        close to zero, and stopping at 1.0. This is for the Importance Sampling
+        """
         if self.beta < 1.0:
             self.beta += self.beta_growth
 
-    def update_priorities(self, batch: List[Tuple], errors_from_batch: List[float]):
+    def update_priorities(self, batch: List[Tuple], errors_from_batch: List[float]) -> None:
         """We want the priority of elements to be the TD error of plus an epsilon
         constant. The epsilon constant makes sure that no experience ever gets a
         priority zero. This prioritization strategy gives more importance to
-        elements that bring more learning to the network."""
-        experience_indexes = [b[-1] for b in numpy.array(batch, dtype=numpy.object).T]
+        elements that bring more learning to the network.
+        """
+        experience_indexes = [b[-1] for b in numpy.array(batch, dtype="object").T]
         for i in range(len(experience_indexes)):
             error = abs(errors_from_batch[i]) + self.epsilon
             if not np.isnan(error):
-                self.experience_queue[experience_indexes[i]] = self.experience_queue[
-                    experience_indexes[i]
-                ]._replace(priority=error)
+                experience = self.experience_queue[experience_indexes[i]]
+                experience._replace(priority=error)
+                self.experience_queue[experience_indexes[i]] = experience
 
     def sample_batch(self) -> List[Tuple]:
         """We sample experiences using their priorities as weights for sampling. The
         effect of the priorities is controlled by the alpha parameter. This is
-        already an advantage but it can introduce bias in a network by always
+        already an advantage, but it can introduce bias in a network by always
         choosing the same type of experiences for training. In order to fight this, we
         compute the weight of the experience (this is called Importance Sampling,
         or IP). We want the weights to decrease over time, this is controlled by
-        the beta parameter."""
+        the beta parameter.
+        """
         # calculate probabilities (alpha)
         probabilities = self.priorities() ** self.alpha
         p = probabilities / probabilities.sum()
         # sample experiences
         buffer_size = len(self.experience_queue)
-        samples = numpy.random.choice(
-            a=buffer_size, size=self.batch_size, p=p, replace=False
-        )
+        samples = numpy.random.choice(a=buffer_size, size=self.batch_size, p=p, replace=False)
         experiences = [self.experience_queue[i].experience for i in samples]
         # importance Sampling
         # w_i = (1/N * 1/P_i) ^ beta
         weights = ((1 / buffer_size) * (1 / p[samples])) ** self.beta
         weights = weights / weights.max()
         self.update_beta()
         # return experiences with weights
-        return list(zip(*experiences)) + [tuple(weights)] + [tuple(samples)]
+        return list(zip(*experiences, strict=False)) + [tuple(weights)] + [tuple(samples)]
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/learning_statistics.py` & `deeprecsys-0.2.5/deeprecsys/rl/learning_statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,82 @@
+from typing import Any, Dict, List, Optional
+
 import matplotlib.pyplot as plt
 import pandas
 import seaborn as sns
-from typing import Any, List, Dict, Optional
 
 sns.set_theme()
 sns.set_context("paper")
 
 
 class LearningStatistics:
-    def __init__(
-        self, model_name: Optional[str] = None, env_name: Optional[str] = None
-    ):
+    """Special class to store and aggregate learning parameters."""
+
+    def __init__(self, model_name: Optional[str] = None, env_name: Optional[str] = None):
+        """Start the collector for the given model and environment name."""
         self.collected_metrics: List[Dict] = []
         self.model_name = model_name
         self.env_name = env_name
         self.timestep = 0
         self.episode = 0
 
-    def append_metric(self, metric_name: str, metric_value: Any):
+    def append_metric(self, metric_name: str, metric_value: Any) -> None:
+        """Store the metric with the given name and value."""
         self.collected_metrics.append(
             {
                 "metric": metric_name,
                 "measurement": metric_value,
                 "timestep": self.timestep,
                 "episode": self.episode,
                 "model": self.model_name,
                 "env": self.env_name,
             }
         )
 
     def get_metrics(
         self, metric_name: str, model: Optional[str] = None, env: Optional[str] = None
     ) -> Optional[pandas.Series]:
+        """Get all the collected metrics for the given name, model, and environment."""
         measurements = [
             v["measurement"]
             for v in self.collected_metrics
             if (v["metric"] == metric_name and v["model"] == model and v["env"] == env)
         ]
         if measurements:
             return pandas.Series(measurements)
+        else:
+            return None
 
     @property
     def moving_rewards(self) -> Optional[pandas.Series]:
+        """Get the moving average of the rewards observed so far."""
         return self.get_metrics("moving_rewards")
 
     @property
     def episode_rewards(self) -> Optional[pandas.Series]:
+        """Get the reward values stored so far."""
         return self.get_metrics("episode_rewards")
 
     @property
     def epsilon_values(self) -> Optional[pandas.Series]:
+        """Get the epsilon values stored so far."""
         return self.get_metrics("epsilon_values")
 
     @property
     def loss_values(self) -> Optional[pandas.Series]:
+        """Get the loss values stored so far."""
         return self.get_metrics("loss")
 
-    def plot_rewards(self):
+    def plot_rewards(self) -> None:
+        """Plot the rewards obtaining so far."""
         self.episode_rewards.plot()
         self.moving_rewards.plot()
 
-    def plot_learning_stats(self):
+    def plot_learning_stats(self) -> None:
+        """Plot the relevant reinforcement learning metrics."""
         # generate subplots
         fig, axs = plt.subplots(2, 2)
         fig.suptitle("Agent learning metrics")
         fig.set_figheight(6)
         fig.set_figwidth(12)
         fig.subplots_adjust(hspace=0.3)
         # add data to plots
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/manager.py` & `deeprecsys-0.2.5/deeprecsys/rl/manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,223 +1,252 @@
-from gym import make, spec, Env
-from collections import namedtuple, defaultdict
-from typing import Any, List, Optional
 import math
-from numpy.random import RandomState
+from collections import defaultdict, namedtuple
+from typing import Any, Generator, List, Optional
+
 import numpy as np
-import highway_env  # noqa: F401
-import deeprecsys.movielens_fairness_env  # noqa: F401
-from deeprecsys.rl.agents.agent import ReinforcementLearning
-from deeprecsys.rl.learning_statistics import LearningStatistics
 import torch
+from gymnasium import Env, make, spec
+from numpy.core.multiarray import ndarray
+from numpy.random import RandomState
 
+from deeprecsys.rl import Logger
+from deeprecsys.rl.agents.agent import ReinforcementLearning
+from deeprecsys.rl.learning_statistics import LearningStatistics
 
 # An episode output is a data model to represent 3 things: how many timesteps the
 # episode took to finish, the total sum of rewards, and the average reward sum of the
 # last 100 episodes.
 EpisodeOutput = namedtuple("EpisodeOutput", "timesteps,reward_sum")
 
+logger = Logger.create()
+
 
-class Manager(object):
-    """ Class for learning from gym environments with some convenience methods. """
+class Manager:
+    """Class for learning from gym environments with some convenience methods."""
 
     env_name: str
     env: Any
+    seed: int | None = None
+    random_state: RandomState | None = None
 
     def __init__(
         self,
         env_name: Optional[str] = None,
         seed: Optional[int] = None,
         env: Optional[Env] = None,
-        max_episode_steps: int = math.inf,
+        max_episode_steps: float = math.inf,
         reward_threshold: float = math.inf,
-        **kwargs,
-    ):
-        if any(
-            [env_name is None and env is None, env_name is not None and env is not None]
-        ):
+        **kwargs: Any,
+    ) -> None:
+        """Start the manager"""
+        if any([env_name is None and env is None, env_name is not None and env is not None]):
             raise ValueError("Must specify exactly one of [env_name, env]")
         if env_name is not None:
             self.env_name = env_name
             # extract some parameters from the environment
-            self.max_episode_steps = (
-                spec(self.env_name).max_episode_steps or max_episode_steps
-            )
-            self.reward_threshold = (
-                spec(self.env_name).reward_threshold or reward_threshold
-            )
+            self.max_episode_steps = spec(self.env_name).max_episode_steps or max_episode_steps
+            self.reward_threshold = spec(self.env_name).reward_threshold or reward_threshold
             # create the environment
             self.env = make(env_name, **kwargs)
             # we seed the environment so that results are reproducible
         else:
             self.env = env
             self.max_episode_steps = max_episode_steps
             self.reward_threshold = reward_threshold
 
         self.setup_reproducibility(seed)
         self.slate_size: int = kwargs["slate_size"] if "slate_size" in kwargs else 1
 
-    def print_overview(self):
-        """ Prints the most important variables of the environment. """
-        print("Reward threshold: {} ".format(self.reward_threshold))
-        print("Reward signal range: {} ".format(self.env.reward_range))
-        print("Maximum episode steps: {} ".format(self.max_episode_steps))
-        print("Action apace size: {}".format(self.env.action_space))
-        print("Observation space size {} ".format(self.env.observation_space))
+    def print_overview(self) -> None:
+        """Print the most important variables of the environment."""
+        logger.info("Reward threshold: {} ".format(self.reward_threshold))
+        logger.info("Reward signal range: {} ".format(self.env.reward_range))
+        logger.info("Maximum episode steps: {} ".format(self.max_episode_steps))
+        logger.info("Action apace size: {}".format(self.env.action_space))
+        logger.info("Observation space size {} ".format(self.env.observation_space))
 
     def execute_episodes(
         self,
         rl: ReinforcementLearning,
         n_episodes: int = 1,
         should_render: bool = False,
-        should_print: bool = False,
     ) -> List[EpisodeOutput]:
         """Execute any number of episodes with the given agent.
-        Returns the number of timesteps and sum of rewards per episode."""
+        Returns the number of timesteps and sum of rewards per episode.
+        """
         episode_outputs = []
         for episode in range(n_episodes):
-            t, reward_sum, done, state = 0, 0, False, self.env.reset()
-            if should_print:
-                print(f"Running episode {episode}, starting at state {state}")
+            t, reward_sum, done, (state, _) = 0, 0, False, self.env.reset(seed=self.seed)
+            logger.info(f"Running episode {episode}, starting at state {state}")
             while not done and t < self.max_episode_steps:
                 if should_render:
                     self.env.render()
                 action = rl.action_for_state(state)
                 state, reward, done, _ = self.env.step(action)
-                if should_print:
-                    print(f"t={t} a={action} r={reward} s={state}")
+                logger.info(f"t={t} a={action} r={reward} s={state}")
                 reward_sum += reward
                 t += 1
             episode_outputs.append(EpisodeOutput(t, reward_sum))
             self.env.close()
         return episode_outputs
 
+    @staticmethod
+    def _train_start_new_episode(statistics: LearningStatistics, episode: int) -> None:
+        if statistics:
+            statistics.episode = episode
+            statistics.timestep = 0
+
+    @staticmethod
+    def _train_update_timestep(statistics: LearningStatistics) -> None:
+        if statistics:
+            statistics.timestep += 1
+
+    @staticmethod
+    def _train_add_statistics(statistics: LearningStatistics, rewards: List, moving_average: ndarray) -> None:
+        if statistics:
+            statistics.append_metric("episode_rewards", sum(rewards))
+            statistics.append_metric("timestep_rewards", rewards)
+            statistics.append_metric("moving_rewards", moving_average)
+
+    def _train_get_step_action(self, rl: ReinforcementLearning, state: Any) -> Any:
+        if self.slate_size == 1:
+            return rl.action_for_state(state)
+        else:
+            return rl.top_k_actions_for_state(state, k=self.slate_size)
+
     def train(
         self,
         rl: ReinforcementLearning,
         statistics: Optional[LearningStatistics] = None,
-        max_episodes=50,
-        should_print: bool = True,
-    ):
-        if should_print is True:
-            print("Training...")
+        max_episodes: int = 50,
+    ) -> None:
+        """Train the agent for the given amount of episodes."""
+        logger.info("Training...")
         episode_rewards = []
         for episode in range(max_episodes):
-            state = self.env.reset()
+            state, info = self.env.reset(seed=self.seed)
             rewards = []
-            if statistics:
-                statistics.episode = episode
-                statistics.timestep = 0
+            self._train_start_new_episode(statistics, episode)
             done = False
             while done is False:
-                if self.slate_size == 1:
-                    action = rl.action_for_state(state)
-                else:
-                    action = rl.top_k_actions_for_state(state, k=self.slate_size)
-                new_state, reward, done, info = self.env.step(action)
+                action = self._train_get_step_action(rl, state)
+                new_state, reward, done, _, info = self.env.step(action)
                 if "chosen_action" in info:
                     action = action[info["chosen_action"]]
-                rl.store_experience(
-                    state, action, reward, done, new_state
-                )  # guardar experiencia en el buffer
+                rl.store_experience(state, action, reward, done, new_state)
                 rewards.append(reward)
                 state = new_state.copy()
-                if statistics:
-                    statistics.timestep += 1
+                self._train_update_timestep(statistics)
             episode_rewards.append(sum(rewards))
             moving_average = np.mean(episode_rewards[-100:])
-            if statistics:
-                statistics.append_metric("episode_rewards", sum(rewards))
-                statistics.append_metric("timestep_rewards", rewards)
-                statistics.append_metric("moving_rewards", moving_average)
-            if should_print is True:
-                print(
-                    "\rEpisode {:d} Mean Rewards {:.2f} Last Reward {:.2f}\t\t".format(
-                        episode, moving_average, sum(rewards)
-                    ),
-                    end="",
-                )
+            self._train_add_statistics(statistics, rewards, moving_average)
+
+            logger.print(
+                f"\rEpisode {episode:d} Mean Rewards {moving_average:.2f} Last Reward {rewards[-1]:.2f}\t\t",
+                end="",
+            )
             if moving_average >= self.reward_threshold:
-                if should_print is True:
-                    print("Reward threshold reached")
+                logger.info("Reward threshold reached")
                 break
 
+    def _hyperparameter_search_run_combinations(
+        self,
+        runs_per_combination: int,
+        rl: ReinforcementLearning,
+        episodes: int,
+        learning_statistics: LearningStatistics,
+        parameter_name: str,
+        parameter_value: Any,
+    ) -> Generator:
+        for run in range(runs_per_combination):
+            self.train(
+                rl=rl,
+                max_episodes=episodes,
+                statistics=learning_statistics,
+            )
+            yield learning_statistics.moving_rewards.iloc[-1]
+            logger.print(
+                f"\rTested combination {parameter_name}={parameter_value} round {run} result was {learning_statistics.moving_rewards.iloc[-1]} \t\t",  # noqa: E501
+                end="",
+            )
+
     def hyperparameter_search(
         self,
         agent: type,
         params: dict,
         default_params: dict,
         episodes: int = 100,
         runs_per_combination: int = 3,
-        verbose: bool = True,
     ) -> dict:
         """Given an agent class, and a dictionary of hyperparameter names and values,
-        will try all combinations, and return the mean reward of each combinatio
-        for the given number of episods, and will run the determined number of times."""
+        will try all combinations, and return the mean reward of each combination
+        for the given number of episodes, and will run the determined number of times.
+        """
         combination_results = defaultdict(lambda: [])
-        for (p_name, p_value) in params.items():
+        for p_name, p_value in params.items():
             if len(p_value) < 2:
                 continue
             for value in p_value:
                 rl = agent(**{**default_params, p_name: value})
                 learning_statistics = LearningStatistics()
                 combination_key = f"{p_name}={value}"
-                for run in range(runs_per_combination):
-                    self.train(
-                        rl=rl,
-                        max_episodes=episodes,
-                        should_print=False,
-                        statistics=learning_statistics,
-                    )
-                    combination_results[combination_key].append(
-                        learning_statistics.moving_rewards.iloc[-1]
-                    )
-                    if verbose:
-                        print(
-                            f"\rTested combination {p_name}={value} round {run} "
-                            f"result was {learning_statistics.moving_rewards.iloc[-1]}"
-                            "\t\t",
-                            end="",
-                        )
+                for result in self._hyperparameter_search_run_combinations(
+                    runs_per_combination,
+                    rl,
+                    episodes,
+                    learning_statistics,
+                    p_name,
+                    value,
+                ):
+                    combination_results[combination_key].append(result)
 
         return combination_results
 
-    def setup_reproducibility(
-        self, seed: Optional[int] = None
-    ) -> Optional[RandomState]:
-        """ Seeds the project's libraries: numpy, torch, gym """
+    def setup_reproducibility(self, seed: Optional[int] = None) -> Optional[RandomState]:
+        """Seeds the project's libraries: numpy, torch, gym"""
         if seed:
             # seed pytorch
             torch.manual_seed(seed)
             torch.backends.cudnn.deterministic = True
             torch.backends.cudnn.benchmark = False
             # seed numpy
             np.random.seed(seed)
             # seed gym
-            self.env.seed(seed)
+            self.seed = seed
             self.random_state = RandomState(seed)
             return self.random_state
+        return None
 
 
 class HighwayManager(Manager):
+    """Manager for the highway environment"""
+
     def __init__(self, seed: Optional[int] = None, vehicles: int = 50):
+        """Start the manager"""
         super().__init__(env_name="highway-v0", seed=seed)
         self.env.configure({"vehicles_count": vehicles})
         self.max_episode_steps = self.env.config["duration"]
 
 
 class CartpoleManager(Manager):
+    """Manager for the cart pole environment"""
+
     def __init__(self, seed: Optional[int] = None):
-        super().__init__(env_name="CartPole-v0", seed=seed)
+        """Start the manager"""
+        super().__init__(env_name="CartPole-v1", seed=seed)
         self.reward_threshold = 50
 
 
 class LunarLanderManager(Manager):
+    """Manager for the lunar lander environment"""
+
     def __init__(self, seed: Optional[int] = None):
+        """Start the manager"""
         super().__init__(env_name="LunarLander-v2", seed=seed)
 
 
 class MovieLensFairnessManager(Manager):
+    """Manager for the movie lens environment"""
+
     def __init__(self, seed: Optional[int] = None, slate_size: int = 1):
-        super().__init__(
-            env_name="MovieLensFairness-v0", seed=seed, slate_size=slate_size
-        )
+        """Start the manager"""
+        super().__init__(env_name="MovieLensFairness-v0", seed=seed, slate_size=slate_size)
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/neural_networks/base_network.py` & `deeprecsys-0.2.5/deeprecsys/neural_networks/base_network.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,66 @@
-from torch.nn import Module
-from torch import save, load
+import numpy as np
 import torch
+from torch import Tensor, device, load, save
+from torch.nn import Module
 from torch.utils.tensorboard import SummaryWriter
-import numpy as np
 from torchviz import make_dot
 
 
 class BaseNetwork(Module):
-    def __init__(self):
+    """Base class representing a neural network, contains utility and common methods"""
+
+    def __init__(self) -> None:
+        """Automatically detects if the device is CUDA or CPU"""
         super().__init__()
         self.device = self._auto_detect_device()
 
     @staticmethod
-    def _auto_detect_device():
+    def _auto_detect_device() -> device:
         has_cuda = torch.cuda.is_available() and torch.cuda.is_initialized()
         return torch.device("cuda" if has_cuda else "cpu")
 
-    def save(self, path: str):
-        """ Writes the model's parameters to the given path. """
+    def save(self, path: str) -> None:
+        """Write the model's parameters to the given path."""
         save(self.state_dict(), path)
 
-    def load(self, path: str):
-        """ Reads the model's parameters from the given path. """
+    def load(self, path: str) -> None:
+        """Read the model's parameters from the given path."""
         self.load_state_dict(load(path))
 
-    def soft_parameter_update(self, source_network: Module, update_rate: float = 0.0):
+    def soft_parameter_update(self, source_network: Module, update_rate: float = 0.0) -> None:
         """When using target networks, this method updates the parameters of the current network
         using the parameters of the given source network. The update_rate is a float in
         range (0,1) and controls how the update affects the target (self). update_rate=0
         means a full deep copy, and update_rate=1 means the target does not update
         at all. This parameter is usually called Tau. This method is usually called
-        an exponential moving average update."""
-        for t, s in zip(self.parameters(), source_network.parameters()):
+        an exponential moving average update.
+        """
+        for t, s in zip(self.parameters(), source_network.parameters(), strict=False):
             t.data.copy_(t.data * (1.0 - update_rate) + s.data * update_rate)
 
-    def run_backpropagation(self, loss):
-        """Requires an optimizer property. Runs backward on the given loss, and
-        steps the optimizer."""
+    def run_backpropagation(self, loss: Tensor) -> None:
+        """Run backward on the given loss, and step the optimizer.
+        Requires an optimizer property.
+        """
         self.optimizer.zero_grad()
         loss.backward()
         self.optimizer.step()
 
-    def disable_learning(self):
+    def disable_learning(self) -> None:
+        """Turn off the `requires_grad` parameter to stop the learning."""
         for param in self.parameters():
             param.requires_grad = False
 
-    def forward(self, *input):
+    def forward(self, *input: Tensor) -> Module:
+        """Return the output of the network for the provided input"""
         return self.model(*input)
 
-    def add_to_tensorboard(self, input_example: np.array):
+    def add_to_tensorboard(self, input_example: np.array) -> None:
+        """Add the input to the tensor board and renders the network graph to pdf"""
         writer = SummaryWriter(f"output/writer/{type(self).__name__}")
         tensor = torch.FloatTensor(input_example)
         writer.add_graph(self, tensor, verbose=True)
         writer.close()
         graph = make_dot(
             self.forward(tensor),
             params=dict(self.named_parameters()),
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/neural_networks/deep_q_network.py` & `deeprecsys-0.2.5/deeprecsys/neural_networks/deep_q_network.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,60 @@
-from torch import FloatTensor, max, LongTensor, BoolTensor, gather, Tensor
+from typing import Any, List, Optional, Tuple
+
 from numpy import array, ravel
-from torch.nn import Sequential, Linear, ReLU, MSELoss, Module
+from torch import BoolTensor, FloatTensor, LongTensor, Tensor, gather, max
+from torch.nn import Linear, Module, MSELoss, ReLU, Sequential
 from torch.optim import Adam
-from typing import List, Any, Tuple, Optional
+
+from deeprecsys.neural_networks.base_network import BaseNetwork
 from deeprecsys.rl.learning_statistics import LearningStatistics
-from deeprecsys.rl.neural_networks.base_network import BaseNetwork
 
 
 def sequential_architecture(layers: List[int], bias: bool = True) -> Module:
-    """ Fully connected layers, with bias, and ReLU activation"""
+    """Fully connected layers, with bias, and ReLU activation"""
     architecture = []
     for i in range(len(layers) - 2):
         architecture.append(Linear(layers[i], layers[i + 1], bias=bias))
         architecture.append(ReLU())
     architecture.append(Linear(layers[-2], layers[-1], bias=bias))
     return Sequential(*architecture)
 
 
 class DeepQNetwork(BaseNetwork):
     """Implementation of a Deep Q Network with a Sequential arquitecture. Layers are
-    supposed to be provided as a list of torch modules."""
+    supposed to be provided as a list of torch modules.
+    """
 
     def __init__(
         self,
         learning_rate: float,
         architecture: Module,
         discount_factor: float = 0.99,
         statistics: Optional[LearningStatistics] = None,
     ):
+        """Create the deep-Q network with the provided parameters."""
         super().__init__()
         self.model = architecture
         self.discount_factor = discount_factor
         self.statistics = statistics
         self.optimizer = Adam(self.parameters(), lr=learning_rate)
         if self.device == "cuda":
             self.model.cuda()
 
     def best_action_for_state(self, state: Any) -> Any:
+        """Return the action with the highest estimated Q-value for the given state"""
         if type(state) is tuple:
             state = array([ravel(s) for s in state])
         state_tensor = FloatTensor(state).to(device=self.device)
         q_values = self.model(state_tensor)
         best_action = max(q_values, dim=-1)[1].item()
         return best_action
 
-    def learn_from(self, experiences: List[Tuple]):
+    def learn_from(self, experiences: List[Tuple]) -> None:
+        """Run the backpropagation from a batch of experiences"""
         self.optimizer.zero_grad()
         loss = self._calculate_loss(experiences)
         loss.backward()
         self.optimizer.step()
         # store loss in statistics
         if self.statistics:
             if self.device == "cuda":
@@ -57,21 +63,17 @@
                 self.statistics.append_metric("loss", loss.detach().numpy())
 
     def _calculate_loss(self, experiences: List[Tuple]) -> Tensor:
         states, actions, rewards, dones, next_states = [i for i in experiences]
         state_tensors = FloatTensor(states).to(device=self.device)
         next_state_tensors = FloatTensor(next_states).to(device=self.device)
         reward_tensors = FloatTensor(rewards).to(device=self.device).reshape(-1, 1)
-        action_tensors = (
-            LongTensor(array(actions)).reshape(-1, 1).to(device=self.device)
-        )
+        action_tensors = LongTensor(array(actions)).reshape(-1, 1).to(device=self.device)
         done_tensors = BoolTensor(dones).to(device=self.device)
         actions_for_states = self.model(state_tensors)
         q_vals = gather(actions_for_states, 1, action_tensors)
         next_actions = [self.best_action_for_state(s) for s in next_states]
-        next_action_tensors = (
-            LongTensor(next_actions).reshape(-1, 1).to(device=self.device)
-        )
+        next_action_tensors = LongTensor(next_actions).reshape(-1, 1).to(device=self.device)
         q_vals_next = gather(self.model(next_state_tensors), 1, next_action_tensors)
         q_vals_next[done_tensors] = 0
         expected_q_vals = self.discount_factor * q_vals_next + reward_tensors
         return MSELoss()(q_vals, expected_q_vals.reshape(-1, 1))
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/neural_networks/dueling.py` & `deeprecsys-0.2.5/deeprecsys/neural_networks/dueling.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,148 +1,134 @@
-from torch import FloatTensor, LongTensor, BoolTensor, gather, Tensor
+from typing import Any, List, Optional, Tuple
+
 from numpy import array, ravel
-from torch.nn import Module, ReLU, Linear, Sequential, functional
+from torch import BoolTensor, FloatTensor, LongTensor, Tensor, gather
+from torch.nn import Linear, Module, ReLU, Sequential, functional
 from torch.optim import Adam
-from typing import List, Any, Tuple, Optional
-from deeprecsys.rl.neural_networks.noisy_layer import NoisyLayer
+
+from deeprecsys.neural_networks.base_network import BaseNetwork
+from deeprecsys.neural_networks.noisy_layer import NoisyLayer
 from deeprecsys.rl.experience_replay.priority_replay_buffer import (
     PrioritizedExperienceReplayBuffer,
 )
 from deeprecsys.rl.learning_statistics import LearningStatistics
-from deeprecsys.rl.neural_networks.base_network import BaseNetwork
 
 
 class DuelingDDQN(BaseNetwork):
-    """ Dueling DQN with Double DQN and Noisy Networks """
+    """Dueling DQN with Double DQN and Noisy Networks"""
 
     def __init__(
         self,
         n_input: int,
         n_output: int,
         learning_rate: float,
         hidden_layers: List[int] = None,
         noise_sigma: float = 0.17,
         discount_factor: float = 0.99,
         statistics: Optional[LearningStatistics] = None,
     ):
+        """Initialize the network with the provided parameters"""
         super().__init__()
         if not hidden_layers:
             hidden_layers = [256, 256, 64, 64]
         self.discount_factor = discount_factor
         self._build_network(n_input, n_output, noise_sigma, hidden_layers=hidden_layers)
         self.optimizer = Adam(self.parameters(), lr=learning_rate)
         self.statistics = statistics
 
-    def _build_network(
-        self, n_input: int, n_output: int, noise_sigma: float, hidden_layers: List[int]
-    ):
-        """Builds the dueling network with noisy layers, the value
-        subnet and the advantage subnet. TODO: add `.to_device()` to Modules"""
-        assert len(hidden_layers) == 4
+    def _build_network(self, n_input: int, n_output: int, noise_sigma: float, hidden_layers: List[int]) -> None:
+        """Build the dueling network with noisy layers, the value
+        subnet and the advantage subnet. TODO: add `.to_device()` to Modules
+        """
+        if len(hidden_layers) != 4:
+            raise ValueError("Unexpected amount of layers")
         fc_1, fc_2, value_size, advantage_size = hidden_layers
         self.fully_connected_1 = Linear(n_input, fc_1, bias=True)
         self.fully_connected_2 = NoisyLayer(fc_1, fc_2, bias=True, sigma=noise_sigma)
         self.value_subnet = Sequential(
             NoisyLayer(fc_2, value_size, bias=True, sigma=noise_sigma),
             ReLU(),
             Linear(value_size, 1, bias=True),
         )
         self.advantage_subnet = Sequential(
             NoisyLayer(fc_2, advantage_size, bias=True, sigma=noise_sigma),
             ReLU(),
             Linear(advantage_size, n_output, bias=True),
         )
 
-    def forward(self, state):
-        """Calculates the forward between the layers"""
+    def forward(self, state: Tensor) -> Tensor:
+        """Calculate the forward between the layers"""
         layer_1_out = functional.relu(self.fully_connected_1(state))
         layer_2_out = functional.relu(self.fully_connected_2(layer_1_out))
         value_of_state = self.value_subnet(layer_2_out)
         advantage_of_state = self.advantage_subnet(layer_2_out)
         # This is the Dueling DQN part
         # Combines V and A to get Q: Q(s,a) = V(s) + (A(s,a) - 1/|A| * sum A(s,a'))
         if len(state.shape) == 2:
-            q_values = value_of_state + (
-                advantage_of_state - advantage_of_state.mean(dim=1, keepdim=True)
-            )
+            q_values = value_of_state + (advantage_of_state - advantage_of_state.mean(dim=1, keepdim=True))
         else:
             q_values = value_of_state + (advantage_of_state - advantage_of_state.mean())
         return q_values
 
     def get_q_values(self, state: Any) -> Tensor:
+        """Run the state through the network and return the Q-value for each action."""
         if type(state) is tuple:
             state = array([ravel(s) for s in state])
         state_tensor = FloatTensor(state).to(device=self.device)
         return self.forward(state_tensor)
 
     def top_k_actions_for_state(self, state: Any, k: int = 1) -> List[int]:
+        """Get the top K actions ranked by their estimated Q-value."""
         q_values = self.get_q_values(state)
         _, top_indices = q_values.topk(k=k)
         return [int(v) for v in top_indices.detach().numpy()]  # TODO: cpu() ?
 
-    def learn_with(
-        self, buffer: PrioritizedExperienceReplayBuffer, target_network: Module
-    ):
+    def learn_with(self, buffer: PrioritizedExperienceReplayBuffer, target_network: Module) -> None:
+        """Train the target network using the replay buffer."""
         experiences = buffer.sample_batch()
         self.optimizer.zero_grad()
-        td_error, weights = self._calculate_td_error_and_weigths(
-            experiences, target_network
-        )
+        td_error, weights = self._calculate_td_error_and_weigths(experiences, target_network)
         loss = (td_error.pow(2) * weights).mean().to(self.device)
         loss.backward()
         self.optimizer.step()
         # store loss in statistics
         if self.statistics:
             if self.device == "cuda":
-                self.statistics.append_metric(
-                    "loss", float(loss.detach().cpu().numpy())
-                )
+                self.statistics.append_metric("loss", float(loss.detach().cpu().numpy()))
             else:
                 self.statistics.append_metric("loss", float(loss.detach().numpy()))
         # update buffer priorities
-        errors_from_batch = td_error.detach().cpu().numpy()
+        errors_from_batch = td_error.detach().cpu().numpy().flatten()
         buffer.update_priorities(experiences, errors_from_batch)
 
     def _calculate_td_error_and_weigths(
         self, experiences: List[Tuple], target_network: Module
     ) -> Tuple[Tensor, Tensor]:
-        states, actions, rewards, dones, next_states, weights, samples = [
-            i for i in experiences
-        ]
+        states, actions, rewards, dones, next_states, weights, samples = [i for i in experiences]
         # convert to tensors
         state_tensors = FloatTensor(states).to(device=self.device)
         next_state_tensors = FloatTensor(next_states).to(device=self.device)
         reward_tensors = FloatTensor(rewards).to(device=self.device).reshape(-1, 1)
-        action_tensors = (
-            LongTensor(array(actions)).reshape(-1, 1).to(device=self.device)
-        )
+        action_tensors = LongTensor(array(actions)).reshape(-1, 1).to(device=self.device)
         done_tensors = BoolTensor(dones).to(device=self.device)
         weight_tensors = FloatTensor(weights).to(device=self.device)
         # the following logic is the DDQN update
         # Then we get the predicted actions for the states that came next
         # (using the main network)
-        actions_for_next_states = [
-            self.top_k_actions_for_state(s)[0] for s in next_state_tensors
-        ]
-        actions_for_next_states_tensor = (
-            LongTensor(actions_for_next_states).reshape(-1, 1).to(device=self.device)
-        )
+        actions_for_next_states = [self.top_k_actions_for_state(s)[0] for s in next_state_tensors]
+        actions_for_next_states_tensor = LongTensor(actions_for_next_states).reshape(-1, 1).to(device=self.device)
         # Then we use them to get the estimated Q Values for these next states/actions,
         # according to the target network. Remember that the target network is a copy
         # of this one taken some steps ago
         next_q_values = target_network.forward(next_state_tensors)
         # now we get the q values for the actions that were predicted for the next state
         # we call detach() so no gradient will be backpropagated along this variable
-        next_q_values_for_actions = gather(
-            next_q_values, 1, actions_for_next_states_tensor
-        ).detach()
+        next_q_values_for_actions = gather(next_q_values, 1, actions_for_next_states_tensor).detach()
         # zero value for done timesteps
         next_q_values_for_actions[done_tensors] = 0
         # bellman equation
-        expected_q_values = (
-            self.discount_factor * next_q_values_for_actions + reward_tensors
-        )
+        expected_q_values = self.discount_factor * next_q_values_for_actions + reward_tensors
         # Then get the Q-Values of the main network for the selected actions
         q_values = gather(self.forward(state_tensors), 1, action_tensors)
         # And compare them (this is the time-difference or TD error)
         td_error = q_values - expected_q_values
         return td_error, weight_tensors.reshape(-1, 1)
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/neural_networks/gaussian_actor.py` & `deeprecsys-0.2.5/deeprecsys/neural_networks/gaussian_actor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,77 @@
-from deeprecsys.rl.neural_networks.base_network import BaseNetwork
-from deeprecsys.rl.neural_networks.deep_q_network import sequential_architecture
+from typing import Tuple
+
 import torch
-from torch.distributions import Normal
-import numpy as np
+from numpy import ndarray
 from torch import FloatTensor, Tensor
+from torch.distributions import Normal
 from torch.optim import Adam
-from deeprecsys.rl.neural_networks.q_value_estimator import TwinnedQValueEstimator
+
+from deeprecsys.neural_networks.base_network import BaseNetwork
+from deeprecsys.neural_networks.deep_q_network import sequential_architecture
+from deeprecsys.neural_networks.q_value_estimator import TwinnedQValueEstimator
 
 LOG_STD_MAX = 2
 LOG_STD_MIN = -20
 EPSILON = 1e-6
 
 
 class GaussianActor(BaseNetwork):
+    """Actor network for the soft-actor-critic agent."""
+
     def __init__(
         self,
         inputs: int,
         outputs: int,
         learning_rate: float = 1e-3,
         entropy_coefficient: float = 0.2,
         discount_factor: float = 0.99,
     ):
+        """Create the actor network with the provided parameters."""
         super().__init__()
         network_output = outputs * 2  # estimation of means and standard deviations
         layers = [inputs] + [inputs * 2, inputs * 2] + [network_output]
         self.model = sequential_architecture(layers)
         self.optimizer = Adam(self.parameters(), lr=learning_rate)
         # TODO: implement entropy learning
         self.alpha = torch.tensor(entropy_coefficient).to(self.device)
         self.gamma = discount_factor
 
-    def forward(self, states: FloatTensor):
+    def forward(self, states: FloatTensor) -> Tuple:
+        """Forward the given state in the network and return the output"""
         mean, log_std = torch.chunk(self.model(states), 2, dim=-1)
         log_std = torch.clamp(log_std, min=LOG_STD_MIN, max=LOG_STD_MAX)
         return mean, log_std
 
-    def predict(self, states: np.array):
+    def predict(self, states: ndarray) -> Tuple:
+        """Predict the next best actions for the given state."""
         states_tensor = FloatTensor(states).to(device=self.device)
-        # calculate Gaussian distribusion of (mean, std)
+        # calculate Gaussian distribution of (mean, std)
         means, log_stds = self.forward(states_tensor)
         stds = log_stds.exp()
         normals = Normal(means, stds)
         # sample actions
         xs = normals.rsample()
         actions = torch.tanh(xs)
-        # calculate entropies
+        # calculate entropy
         log_probs = normals.log_prob(xs) - torch.log(1 - actions.pow(2) + EPSILON)
         entropies = -log_probs.sum(dim=1, keepdim=True)
         return actions, entropies, torch.tanh(means)
 
     def calculate_loss(
         self,
         states: Tensor,
         actions: Tensor,
         rewards: Tensor,
         dones: Tensor,
         next_states: Tensor,
         weights: Tensor,
         critic: TwinnedQValueEstimator,
     ) -> Tensor:
-        """ Calculates the loss, backpropagates, and returns the entropy. """
+        """Calculate the loss, backpropagates, and returns the entropy."""
         # We re-sample actions to calculate expectations of Q.
         sampled_action, entropy, _ = self.predict(states)
         # expectations of Q with clipped double Q technique
         q1, q2 = critic(states, sampled_action)
         q = torch.min(q1, q2)
         # Policy objective is maximization of (Q + alpha * entropy) with
         # priority weights.
@@ -76,14 +84,15 @@
         states: Tensor,
         actions: Tensor,
         rewards: Tensor,
         next_states: Tensor,
         dones: Tensor,
         target_critic: TwinnedQValueEstimator,
     ) -> Tensor:
+        """Estimate the Q-value for the next states"""
         with torch.no_grad():
             # actor samples next actions
             next_actions, next_entropies, _ = self.predict(next_states)
             # cricic estimates q values for next actions
             next_q_critic = target_critic.predict(next_states, next_actions)
             next_q = next_q_critic + self.alpha * next_entropies
         target_q = rewards + self.gamma * next_q
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/neural_networks/noisy_layer.py` & `deeprecsys-0.2.5/deeprecsys/neural_networks/noisy_layer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,39 @@
-from torch.nn import Linear, Parameter, functional
 import torch
+from torch import Tensor
+from torch.nn import Linear, Parameter, functional
 
 
 class NoisyLayer(Linear):
+    """Special type of layer that adds random gaussian noise to the signal The gaussian noise parameters are
+    registered, and therefore the noise decreases over time. This is a better alternative to e-greedy exploration.
+    """
+
     def __init__(
-        self, in_features: int, out_features: int, bias=True, sigma: float = 0.017
-    ):
+        self,
+        in_features: int,
+        out_features: int,
+        bias: bool = True,
+        sigma: float = 0.017,
+    ) -> None:
+        """Create the layer with the given sigma weight. Registers epsilon as a parameter so that the network will
+        learn to reduce the noise.
+        """
         super().__init__(in_features, out_features, bias=bias)
         self.sigma_weight = Parameter(torch.full((out_features, in_features), sigma))
         self.register_buffer("epsilon_weight", torch.zeros(out_features, in_features))
         if bias:
             self.sigma_bias = Parameter(torch.full((out_features,), sigma))
             self.register_buffer("epsilon_bias", torch.zeros(out_features))
 
-    def forward(self, input):
+    def forward(self, input: Tensor) -> Tensor:
         """At every forward operation, feeds the weights and biases with normally
         distributed random variables with mean zero and std deviation 1. This means
         the bias and the weights will have a noise of:
-        sigma (constant) * epsilon (random in range(-1,1))"""
+        sigma (constant) * epsilon (random in range(-1,1))
+        """
         self.epsilon_weight.normal_()
         bias = self.bias
         if bias is not None:
             self.epsilon_bias.normal_()
             bias = bias + self.sigma_bias * self.epsilon_bias.clone()
-        return functional.linear(
-            input, self.weight + self.sigma_weight * self.epsilon_weight.clone(), bias
-        )
+        return functional.linear(input, self.weight + self.sigma_weight * self.epsilon_weight.clone(), bias)
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/neural_networks/policy_estimator.py` & `deeprecsys-0.2.5/deeprecsys/neural_networks/policy_estimator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,66 @@
 from typing import Any, List
-from torch.optim import Adam
-from torch.nn import Sequential, Softmax, Linear, Tanh
-from torch import FloatTensor, multinomial, Tensor
+
+import numpy as np
+from torch import FloatTensor, Tensor, multinomial
 from torch import sum as torch_sum
 from torch.distributions import Categorical
-import numpy as np
-from deeprecsys.rl.neural_networks.base_network import BaseNetwork
+from torch.nn import Linear, Sequential, Softmax, Tanh
+from torch.optim import Adam
+
+from deeprecsys.neural_networks.base_network import BaseNetwork
 
 
 class PolicyEstimator(BaseNetwork):
     """Estimates the policy function: the probability of each action being the
-    best decision in a particular state."""
+    best decision in a particular state.
+    """
 
     def __init__(
         self,
         input_size: int,
         hidden_layers: List[int],
         output_size: int,
-        learning_rate=1e-2,
+        learning_rate: float = 1e-2,
     ):
+        """Create the neural network architecture for the policy estimator with the provided values."""
         super().__init__()
         layers = [input_size] + hidden_layers + [output_size]
         architecture = []
         for i in range(len(layers) - 2):
             architecture.append(Linear(layers[i], layers[i + 1]))
             architecture.append(Tanh())
         architecture.append(Linear(layers[-2], layers[-1]))
         architecture.append(Softmax(dim=-1))
         self.model = Sequential(*architecture)
         self.optimizer = Adam(self.parameters(), lr=learning_rate)
         if self.device == "cuda":
             self.model.cuda()
 
-    def action_probabilities(self, state: Any):
+    def action_probabilities(self, state: Any) -> Tensor:
+        """Return a map of each possible action, and the probability that that's the best action to take at
+        this step.
+        """
         return self.model(FloatTensor(state))
 
     def predict(self, state: Any, k: int = 1) -> List[int]:
+        """Given a state, uses the network output to choose the `k` best next actions according to the probability
+        distribution trained so far.
+        """
         probabilities = self.action_probabilities(state)
         prediction = multinomial(probabilities, num_samples=k, replacement=False)
         if self.device == "cuda":
             return prediction.detach().cpu().numpy()
         else:
             return prediction.detach().numpy()
 
-    def update(self, state: np.array, reward_baseline: Tensor, action: np.array):
+    def update(self, state: np.array, reward_baseline: Tensor, action: np.array) -> np.ndarray:
+        """Update the network with the given state, reward, and action taken."""
         state_tensor = FloatTensor(state).to(device=self.device)
-        action_tensor = FloatTensor(np.array(action, dtype=np.float32)).to(
-            device=self.device
-        )
+        action_tensor = FloatTensor(np.array(action, dtype=np.float32)).to(device=self.device)
         """ Update logic from the Policy Gradient theorem. """
         action_probabilities = self.model(state_tensor)
         action_distribution = Categorical(action_probabilities)
         selected_log_probabilities = action_distribution.log_prob(action_tensor)
         loss = torch_sum(-selected_log_probabilities * reward_baseline)
         self.optimizer.zero_grad()
         loss.backward()
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/neural_networks/q_value_estimator.py` & `deeprecsys-0.2.5/deeprecsys/neural_networks/q_value_estimator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,55 @@
-from deeprecsys.rl.neural_networks.base_network import BaseNetwork
-from deeprecsys.rl.neural_networks.deep_q_network import sequential_architecture
+from typing import Tuple
+
 import torch
-from torch import Tensor, FloatTensor
+from torch import FloatTensor, Tensor
 from torch.nn import Module
 from torch.optim import Adam
 
+from deeprecsys.neural_networks.base_network import BaseNetwork
+from deeprecsys.neural_networks.deep_q_network import sequential_architecture
+
 
 class QValueEstimator(BaseNetwork):
-    """ Estimates the Q-value (expected return) of each (state,action) pair """
+    """Estimate the Q-value (expected return) of each (state,action) pair"""
 
     def __init__(self, inputs: int, outputs: int, learning_rate: float = 1e-3):
+        """Create the network architecture with the provided parameters."""
         super().__init__()
         layers = [inputs] + [inputs * 2, inputs * 2] + [outputs]
         self.model = sequential_architecture(layers)
         self.optimizer = Adam(self.parameters(), lr=learning_rate)
         if self.device == "cuda":
             self.model.cuda()
 
-    def predict(self, states: Tensor, actions: Tensor):
-        inputs = torch.cat([states, actions.type(FloatTensor)], dim=1).to(
-            device=self.device
-        )
+    def predict(self, states: Tensor, actions: Tensor) -> Tensor:
+        """Given a state and an action, return the estimated Q-Value"""
+        inputs = torch.cat([states, actions.type(FloatTensor)], dim=1).to(device=self.device)
         return self.model(inputs)
 
 
 class TwinnedQValueEstimator(BaseNetwork):
-    """Estimates the Q-value (expected return) of each (state,action) pair,
-    using 2 independent estimators, and predicting with the minimum estimated Q-value"""
+    """Estimate the Q-value (expected return) of each (state,action) pair,
+    using 2 independent estimators, and predicting with the minimum estimated Q-value.
+    This is the "critic" part of the Actor-Critic model.
+    """
 
     def __init__(self, inputs: int, outputs: int = 1, learning_rate: float = 1e-3):
+        """Create the two estimators with the provided parameters."""
         super().__init__()
         self.Q1 = QValueEstimator(inputs, outputs, learning_rate=learning_rate)
         self.Q2 = QValueEstimator(inputs, outputs, learning_rate=learning_rate)
 
-    def predict(self, states: Tensor, actions: Tensor):
+    def predict(self, states: Tensor, actions: Tensor) -> Tensor:
+        """Given a (state, action) pair return the smaller Q-value of the two networks."""
         q1, q2 = self.forward(states, actions)
         return torch.min(q1, q2)
 
-    def forward(self, states: Tensor, actions: Tensor):
+    def forward(self, states: Tensor, actions: Tensor) -> Tuple:
+        """Calculate the output weighs for the given (state, action) pair"""
         q1 = self.Q1.predict(states, actions)
         q2 = self.Q2.predict(states, actions)
         return q1, q2
 
     def calculate_loss(
         self,
         states: Tensor,
@@ -49,14 +57,15 @@
         rewards: Tensor,
         dones: Tensor,
         next_states: Tensor,
         weights: Tensor,
         actor: Module,
         target: "TwinnedQValueEstimator",
     ) -> Tensor:
+        """Train the network and return the loss."""
         curr_q1, curr_q2 = self(states, actions)
         target_q = actor.calculate_target_q(
             states,
             actions,
             rewards,
             next_states,
             dones,
```

### Comparing `deeprecsys-0.1.0/deeprecsys/rl/neural_networks/value_estimator.py` & `deeprecsys-0.2.5/deeprecsys/neural_networks/value_estimator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 from typing import List
-from deeprecsys.rl.neural_networks.deep_q_network import sequential_architecture
-from torch.optim import Adam
-from torch.nn import MSELoss
-from torch import FloatTensor
+
 import numpy as np
-from deeprecsys.rl.neural_networks.base_network import BaseNetwork
+from torch import FloatTensor
+from torch.nn import MSELoss
+from torch.optim import Adam
+
+from deeprecsys.neural_networks.base_network import BaseNetwork
+from deeprecsys.neural_networks.deep_q_network import sequential_architecture
 
 
 class ValueEstimator(BaseNetwork):
     """Estimates the value function: the expected return of being in a
-    particular state"""
+    particular state
+    """
 
     def __init__(
         self,
         input_size: int,
         hidden_layers: List[int],
         output_size: int,
-        learning_rate=0.1,
+        learning_rate: float = 0.1,
     ):
+        """Create the network with the given parameters. The output should always be one."""
         super().__init__()
-        self.model = sequential_architecture(
-            [input_size] + hidden_layers + [output_size]
-        )
+        self.model = sequential_architecture([input_size] + hidden_layers + [output_size])
         self.optimizer = Adam(self.parameters(), lr=learning_rate)
         if self.device == "cuda":
             self.model.cuda()
         self.loss_function = MSELoss()
 
     def predict(self, state: np.array) -> float:
+        """Estimate the expected return of being in the given state."""
         state_tensor = FloatTensor(state).to(device=self.device)
         return self.model(state_tensor)
 
-    def update(self, state: np.array, return_value: float):
+    def update(self, state: np.array, return_value: float) -> None:
+        """Run backpropagation on the given state and return."""
         expected_return = FloatTensor(np.array([return_value])).to(device=self.device)
         predicted_return = self.predict(state)
         self.optimizer.zero_grad()
         loss = self.loss_function(predicted_return, expected_return)
         loss.backward()
         self.optimizer.step()
```

