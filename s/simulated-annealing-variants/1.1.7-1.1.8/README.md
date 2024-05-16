# Comparing `tmp/simulated_annealing_variants-1.1.7.tar.gz` & `tmp/simulated_annealing_variants-1.1.8.tar.gz`

## Comparing `simulated_annealing_variants-1.1.7.tar` & `simulated_annealing_variants-1.1.8.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/example_qubovert.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/mpi_simulated_annealing.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/requirements.txt
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/simulated_annealing_variants/README.md
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/simulated_annealing_variants/__init__.py
--rw-r--r--   0        0        0     2969 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/simulated_annealing_variants/simulated_annealing.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/simulated_annealing_variants/simulated_annealing_qrf.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/simulated_annealing_variants/simulated_annealing_rf.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/simulated_annealing_variants/utils.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/LICENSE
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/README.md
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/pyproject.toml
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/example_max_clique.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/example_qubovert.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/mpi_simulated_annealing.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/requirements.txt
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/simulated_annealing_variants/README.md
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/simulated_annealing_variants/__init__.py
+-rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/simulated_annealing_variants/simulated_annealing.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/simulated_annealing_variants/simulated_annealing_jax.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/simulated_annealing_variants/simulated_annealing_qrf.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/simulated_annealing_variants/simulated_annealing_rf.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/simulated_annealing_variants/temperature.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/simulated_annealing_variants/utils.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/LICENSE
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/README.md
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 simulated_annealing_variants-1.1.8/PKG-INFO
```

### Comparing `simulated_annealing_variants-1.1.7/example_qubovert.py` & `simulated_annealing_variants-1.1.8/example_qubovert.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,46 +11,41 @@
 from simulated_annealing_variants.utils import f
 
 
 if __name__ == "__main__":
     # Create a problem as in
     # https://qubovert.readthedocs.io/en/latest/problems/np/numberpartitioning.html
     t1 = timer()
-    N = 2048
+    N = 128
     np.random.seed(15)
     S = np.random.randint(1, 100, size=(N,)).tolist()
-    # problem = qv.problems.NumberPartitioning(S)
-    # H = problem.to_qubo()
-    # H[()] = 0  # Remove constant
-    # Q = qv.utils.qubo_to_matrix(H)
-    c = np.sum(S)
-    Q = np.zeros((N, N))
-    for i in range(N):
-        Q[i, i] = S[i] * (S[i] - c)
-        for j in range(i + 1, N):
-            Q[i, j] = 2 * S[i] * S[j]
+    problem = qv.problems.NumberPartitioning(S)
+    H = problem.to_qubo()
+    H[()] = 0  # Remove constant
+    Q = qv.utils.qubo_to_matrix(H)
+
     print(f"Formulation time for N = {N} is {timer() - t1:.4f}s")
 
-    # t1 = timer()
-    # res = qv.sim.anneal_qubo(H, num_anneals=10, seed=34)
-    # t2 = timer()
-    # x = np.array([res.best.state[i] for i in range(N)])
-    # energy = f(x, Q)
-    # print(f"Qubovert annealing:   {energy} ({t2 - t1:.4f}s)")
+    t1 = timer()
+    res = qv.sim.anneal_qubo(H, num_anneals=10, seed=34)
+    t2 = timer()
+    x = np.array([res.best.state[i] for i in range(N)])
+    energy = f(x, Q)
+    print(f"Qubovert annealing:   {energy} ({t2 - t1:.4f}s)")
 
     t1 = timer()
-    x, _ = simulated_annealing(Q, 10000)
+    x, _ = simulated_annealing(Q)
     t2 = timer()
     energy = f(x, Q)
     print(f"Default annealing:    {energy} ({t2 - t1:.4f}s)")
 
     t1 = timer()
-    x, _ = simulated_annealing_qrf(Q, 10000)
+    x, _ = simulated_annealing_qrf(Q)
     t2 = timer()
     energy = f(x, Q)
     print(f"Quasi rejection-free: {energy} ({t2 - t1:.4f}s)")
 
     t1 = timer()
-    x, _ = simulated_annealing_rf(Q, 10000)
+    x, _ = simulated_annealing_rf(Q)
     t2 = timer()
     energy = f(x, Q)
     print(f"Rejection-free:       {energy} ({t2 - t1:.4f}s)")
```

### Comparing `simulated_annealing_variants-1.1.7/mpi_simulated_annealing.py` & `simulated_annealing_variants-1.1.8/mpi_simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `simulated_annealing_variants-1.1.7/simulated_annealing_variants/simulated_annealing.py` & `simulated_annealing_variants-1.1.8/simulated_annealing_variants/simulated_annealing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 import numpy as np
 from typing import Tuple
 
-from .utils import temperature_schedule, sample_temperature_range, sample_temperature, f
+from .utils import f
+from .temperature import temperature_schedule, TEMPERATURE_SAMPLING_MODE
 
 
 def simulated_annealing(
-    Q: np.ndarray, num_t_values: int, seed: int | None = None
+    Q: np.ndarray,
+    num_t_values: int | None = None,
+    temperature_sampling_mode: TEMPERATURE_SAMPLING_MODE = TEMPERATURE_SAMPLING_MODE.deterministic,
+    seed: int | None = None,
 ) -> Tuple[np.ndarray, float]:
     """Simulated annealing with a computational complexity of O(n * t),
     where t is the number of timesteps.
     This is achieved by computing only the updated values which are at most
     n per update step.
 
     Args:
         Q (np.ndarray): The QUBO matrix.
-        num_t_values (int): Number of update steps.
+        num_t_values (int | None, optional): Number of update steps. Defaults to the size of the QUBO squared.
+        temperature_sampling_mode (TEMPERATURE_SAMPLING_TYPE): The way of sampling the temperature start and end values. Defaults to deterministic.
+        seed (int | None, optional): Random seed. Defaults to None.
+
 
     Returns:
         Tuple[np.ndarray, float]: The best solutions and its energy.
     """
     rng = np.random.Generator(np.random.PCG64(seed=seed))
 
     # Create helper matrix
     n = Q.shape[0]
     Q_outer = Q + Q.T
     np.fill_diagonal(Q_outer, 0)
 
+    if num_t_values is None:
+        num_t_values = n**2
+
     # Random initial
     x = rng.integers(0, high=2, size=(n,))
     f_x = f(x, Q)
 
-    t0, t_end = sample_temperature_range(Q)  # Sample randomly
-
     # Create the inverted temperature values
     betas = temperature_schedule(
-        t0=t0, t_end=t_end, num_t_values=num_t_values, generate_inverse=True
+        Q,
+        num_t_values=num_t_values,
+        temperature_sampling_mode=temperature_sampling_mode,
+        generate_inverse=True,
     )
 
     for beta in betas:
         # Random flip in x
         idx = rng.integers(0, high=n)
 
         # Compute the difference between the flip and the previous energy
@@ -51,51 +62,51 @@
             x[idx] = 1 - x[idx]
             f_x = f_y
 
     return x, f_x
 
 
 def simulated_annealing_slow(
-    Q: np.ndarray, num_t_values: int, seed: int | None = None
+    Q: np.ndarray, num_t_values: int | None = None, seed: int | None = None
 ) -> Tuple[np.ndarray, float]:
     """Classical simulated annealing with a computational complexity of O(n^2 * t),
     where t is the number of timesteps.
     This is achieved by computing only the updated values which are at most
     n per update step.
 
     Args:
         Q (np.ndarray): The QUBO matrix.
-        num_t_values (int): Number of update steps.
+        num_t_values (int | None, optional): Number of update steps. Defaults to the size of the QUBO squared.
+        seed (int | None, optional): Random seed. Defaults to None.
 
     Returns:
         Tuple[np.ndarray, float]: The best solutions and its energy.
     """
     rng = np.random.Generator(np.random.PCG64(seed=seed))
     n = Q.shape[0]
 
-    t0, t_end, _ = sample_temperature(Q)  # Sample randomly
+    if num_t_values is None:
+        num_t_values = n**2
 
-    # Create the inverted temperature values
-    ts = temperature_schedule(
-        t0=t0, t_end=t_end, num_t_values=num_t_values, generate_inverse=True
-    )
+    # Create the beta schedule.
+    betas = temperature_schedule(Q, num_t_values=num_t_values, generate_inverse=True)
 
     # Random initial x
     x = rng.integers(0, high=2, size=(n,))
     f_x = f(x, Q)
 
-    for t in ts:
+    for beta in betas:
         # Random flip in x
         idx = np.random.randint(n)
         x[idx] = 1 - x[idx]
 
         # Compute differences
         f_y = f(x, Q)
 
         # Accept the new one if better
-        if f_y <= f_x or (np.exp(-(f_y - f_x) * t) > np.random.uniform()):
+        if f_y <= f_x or (np.exp(-(f_y - f_x) * beta) > np.random.uniform()):
             f_x = f_y
         else:
             # Otherwise flip back
             x[idx] = 1 - x[idx]
 
     return x, f_x
```

### Comparing `simulated_annealing_variants-1.1.7/simulated_annealing_variants/simulated_annealing_qrf.py` & `simulated_annealing_variants-1.1.8/simulated_annealing_variants/simulated_annealing_qrf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 import numpy as np
 from typing import Tuple
 
-from .utils import sample_temperature, temperature_schedule, f
+from .utils import f
+from .temperature import (
+    temperature_schedule,
+    expectation_delta_x,
+    TEMPERATURE_SAMPLING_MODE,
+)
 
 
 def metropolis_hastings_criterion(deltaE: np.ndarray, t: float) -> np.ndarray:
     """Metropolis-Hastings criterion with with inverse.
 
     Args:
         deltaE (np.ndarray): The energy difference.
@@ -16,63 +21,74 @@
     """
     # Clamp the inverted delta values to remove overflow warning
     criterion = np.minimum(0, -deltaE)
     return np.minimum(1, np.exp(criterion * t))
 
 
 def simulated_annealing_qrf(
-    Q: np.ndarray, num_t_values: int, seed: int | None = None
+    Q: np.ndarray,
+    num_t_values: int | None = None,
+    temperature_sampling_mode: TEMPERATURE_SAMPLING_MODE = TEMPERATURE_SAMPLING_MODE.deterministic,
+    seed: int | None = None,
 ) -> Tuple[np.ndarray, float]:
     """Quasi rejection-free simulated annealing with parallelized update scheme.
 
     Args:
         Q (np.ndarray): The QUBO matrix.
-        num_t_values (int): Number of update steps.
+        num_t_values (int | None, optional): Number of update steps. Defaults to the size of the QUBO squared.
+        temperature_sampling_mode (TEMPERATURE_SAMPLING_TYPE): The way of sampling the temperature start and end values. Defaults to deterministic.
+        seed (int | None, optional): Random seed. Defaults to None.
 
     Returns:
         Tuple[np.ndarray, float]: The best solutions and its energy.
     """
     rng = np.random.Generator(np.random.PCG64(seed=seed))
 
     # Number of bits
     n = Q.shape[0]
 
     # For easier computation create a dense matrix
     Q_diag = np.diag(Q)
     Q_full = Q + Q.T
     np.fill_diagonal(Q_full, Q_diag)
 
-    t0, t_end, offset_increase_rate = sample_temperature(Q, k=3)  # Sample randomly
+    if num_t_values is None:
+        num_t_values = n**2
 
     # Create the inverted temperature values
-    ts = temperature_schedule(
-        t0=t0, t_end=t_end, num_t_values=num_t_values, generate_inverse=True
+    betas = temperature_schedule(
+        Q,
+        num_t_values=num_t_values,
+        temperature_sampling_mode=temperature_sampling_mode,
+        generate_inverse=True,
     )
 
+    offset_increase_rate = expectation_delta_x(Q, 8) / 3
+
     # Random initial x
     x = rng.integers(0, high=2, size=(n,))
 
     # Remember best values
     best_x = np.copy(x)
     f_x = f(x, Q)
     best_energy = f_x
 
     # ---------------- Start
 
     # The change of delta E with respect to a bitflip at index [i]
     # Initial flip
     h = np.sum(Q_full * x, axis=1) + (1 - x) * Q_diag
 
-    for t in ts:
+    for beta in betas:
         # Compute the differene for all flipped x at once
         delta_E = -(1 - 2 * (1 - x)) * h
         delta = 0.0
         while True:
             # Check for accepted elements
-            criteria = metropolis_hastings_criterion(delta_E - delta, t)
+            criteria = metropolis_hastings_criterion(delta_E - delta, beta)
             u_s = rng.uniform(0, 1, size=criteria.shape)
 
             # Then some acceptance probabilities
             accepted = np.where(criteria > u_s)[0]  # Only care about true elements
 
             # If at least one element got accepted, jump out
             if len(accepted):
```

### Comparing `simulated_annealing_variants-1.1.7/simulated_annealing_variants/simulated_annealing_rf.py` & `simulated_annealing_variants-1.1.8/simulated_annealing_variants/simulated_annealing_rf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 import numpy as np
 from typing import Tuple
 
-from .utils import sample_temperature, temperature_schedule, f
+from .utils import f
+from .temperature import temperature_schedule, TEMPERATURE_SAMPLING_MODE
 
 
 def simulated_annealing_rf(
-    Q: np.ndarray, num_t_values: int, seed: int | None = None
+    Q: np.ndarray,
+    num_t_values: int | None = None,
+    temperature_sampling_mode: TEMPERATURE_SAMPLING_MODE = TEMPERATURE_SAMPLING_MODE.deterministic,
+    seed: int | None = None,
 ) -> Tuple[np.ndarray, float]:
     """Rejection-free simulated annealing with parallelized update scheme.
 
     Args:
         Q (np.ndarray): The QUBO matrix.
-        num_t_values (int): Number of update steps.
+        num_t_values (int | None, optional): Number of update steps. Defaults to the size of the QUBO squared.
+        temperature_sampling_mode (TEMPERATURE_SAMPLING_TYPE): The way of sampling the temperature start and end values. Defaults to deterministic.
+        seed (int | None, optional): Random seed. Defaults to None.
+
 
     Returns:
         Tuple[np.ndarray, float]: The best solutions and its energy.
     """
     rng = np.random.Generator(np.random.PCG64(seed=seed))
 
     # Number of bits
     n = Q.shape[0]
 
     # For easier computation create a dense matrix
     Q_diag = np.diag(Q)
     Q_full = Q + Q.T
     np.fill_diagonal(Q_full, Q_diag)
 
-    t0, t_end, _ = sample_temperature(Q)  # Sample randomly
+    if num_t_values is None:
+        num_t_values = n**2
 
-    # Create the inverted temperature values
+    # Sample the inverse temperature schedule
     ts = temperature_schedule(
-        t0=t0, t_end=t_end, num_t_values=num_t_values, generate_inverse=False
+        Q,
+        num_t_values=num_t_values,
+        temperature_sampling_mode=temperature_sampling_mode,
+        generate_inverse=False,
     )
 
     # Random initial x
     x = rng.integers(0, high=2, size=(n,))
 
     # Remember best values
     best_x = np.copy(x)
```

### Comparing `simulated_annealing_variants-1.1.7/.gitignore` & `simulated_annealing_variants-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `simulated_annealing_variants-1.1.7/LICENSE` & `simulated_annealing_variants-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simulated_annealing_variants-1.1.7/README.md` & `simulated_annealing_variants-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `simulated_annealing_variants-1.1.7/pyproject.toml` & `simulated_annealing_variants-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simulated-annealing-variants"
-version = "1.1.7"
+version = "1.1.8"
 license = "MIT"
 authors = [
   { name="Michel Krispin", email="michel.krispin@tuhh.de" },
 ]
 description = "Python implementations of simulated annealing variants such as quasi rejection-free and rejection-free simulated annealing to optimize QUBO problems."
 requires-python = ">=3.7"
 readme = 'README.md'
```

### Comparing `simulated_annealing_variants-1.1.7/PKG-INFO` & `simulated_annealing_variants-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: simulated-annealing-variants
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python implementations of simulated annealing variants such as quasi rejection-free and rejection-free simulated annealing to optimize QUBO problems.
 Project-URL: Homepage, https://github.com/MichelKrispin/rf-simulated-annealing
 Author-email: Michel Krispin <michel.krispin@tuhh.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

