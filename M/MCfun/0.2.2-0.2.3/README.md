# Comparing `tmp/MCfun-0.2.2.tar.gz` & `tmp/MCfun-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCfun-0.2.2.tar", last modified: Fri Oct  6 02:06:07 2023, max compression
+gzip compressed data, was "MCfun-0.2.3.tar", last modified: Thu May 16 03:18:05 2024, max compression
```

## Comparing `MCfun-0.2.2.tar` & `MCfun-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 02:06:07.825403 MCfun-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-06 02:06:07.000000 MCfun-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-10-06 02:06:07.000000 MCfun-0.2.2/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 02:06:07.825403 MCfun-0.2.2/MCfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-10-06 02:06:07.000000 MCfun-0.2.2/MCfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-10-06 02:06:07.000000 MCfun-0.2.2/MCfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-06 02:06:07.000000 MCfun-0.2.2/MCfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-10-06 02:06:07.000000 MCfun-0.2.2/MCfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-06 02:06:07.000000 MCfun-0.2.2/MCfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-10-06 02:06:07.825403 MCfun-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2023-10-06 02:06:07.000000 MCfun-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-06 02:06:07.825403 MCfun-0.2.2/mcfun/
--rw-r--r--   0 runner    (1001) docker     (127)   165430 2023-10-06 02:06:07.000000 MCfun-0.2.2/mcfun/LebedevGrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-10-06 02:06:07.000000 MCfun-0.2.2/mcfun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13764 2023-10-06 02:06:07.000000 MCfun-0.2.2/mcfun/eval_xc.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-06 02:06:07.825403 MCfun-0.2.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1182 2023-10-06 02:06:07.000000 MCfun-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:18:05.021395 MCfun-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 03:18:04.000000 MCfun-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-16 03:18:04.000000 MCfun-0.2.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:18:05.021395 MCfun-0.2.3/MCfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-16 03:18:05.000000 MCfun-0.2.3/MCfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-16 03:18:05.000000 MCfun-0.2.3/MCfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 03:18:05.000000 MCfun-0.2.3/MCfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 03:18:05.000000 MCfun-0.2.3/MCfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 03:18:05.000000 MCfun-0.2.3/MCfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-16 03:18:05.021395 MCfun-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-16 03:18:04.000000 MCfun-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:18:05.021395 MCfun-0.2.3/mcfun/
+-rw-r--r--   0 runner    (1001) docker     (127)   165430 2024-05-16 03:18:04.000000 MCfun-0.2.3/mcfun/LebedevGrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-16 03:18:04.000000 MCfun-0.2.3/mcfun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17511 2024-05-16 03:18:04.000000 MCfun-0.2.3/mcfun/eval_xc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 03:18:05.021395 MCfun-0.2.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1182 2024-05-16 03:18:04.000000 MCfun-0.2.3/setup.py
```

### Comparing `MCfun-0.2.2/LICENSE` & `MCfun-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MCfun-0.2.2/mcfun/LebedevGrid.py` & `MCfun-0.2.3/mcfun/LebedevGrid.py`

 * *Files identical despite different names*

### Comparing `MCfun-0.2.2/mcfun/eval_xc.py` & `MCfun-0.2.3/mcfun/eval_xc.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,19 +62,19 @@
     Returns
     -------
     XC functional and derivatives for each grid.
     * [exc] if deriv = 0
     * [exc, vxc] if deriv = 1
     * [exc, vxc, fxc] if deriv = 2
     '''
-    assert deriv < 3
+
+    assert deriv < 5
     rho_tm = np.asarray(rho_tm)
     if rho_tm.dtype != np.double:
         raise RuntimeError('rho and m must be real')
-
     ngrids = rho_tm.shape[-1]
     grids_per_task = min(ngrids//(workers*3)+1, MAX_GRIDS_PER_TASK)
     if workers == 1:
         results = []
         for p0, p1 in _prange(0, ngrids, grids_per_task):
             r = _eval_xc_lebedev(func, rho_tm[...,p0:p1], deriv, spin_samples,
                                  collinear_threshold, collinear_samples)
@@ -82,24 +82,74 @@
     else:
         if getattr(func, '__closure__', None):
             warnings.warn(f'Closure {func} cannot be parallelized by multiprocessing module. '
                           'It is recommended to generate the function with functools.partial.')
             executor = ThreadPoolExecutor
         else:
             executor = ProcessPoolExecutor
-
         with executor(max_workers=workers) as ex:
             futures = []
             for p0, p1 in _prange(0, ngrids, grids_per_task):
                 f = ex.submit(_eval_xc_lebedev, func, rho_tm[...,p0:p1], deriv,
                               spin_samples, collinear_threshold, collinear_samples)
                 futures.append(f)
             results = [f.result() for f in futures]
+        
+    return [None if x[0] is None else np.concatenate(x, axis=-1) for x in zip(*results)]
+
+
+def eval_xc_eff_sf(func, rho_tmz, deriv=1, collinear_samples=200, workers=1):
+    assert deriv < 5
+    if rho_tmz.dtype != np.double:
+        raise RuntimeError('rho and mz must be real')
+    ngrids = rho_tmz.shape[-1]
+    grids_per_task = min(ngrids//(workers*3)+1, MAX_GRIDS_PER_TASK)
+
+    if workers == 1:
+        results = []
+        for p0, p1 in _prange(0, ngrids, grids_per_task):
+            r = _eval_xc_sf(func, rho_tmz[...,p0:p1], deriv, collinear_samples)
+            results.append(r)
+    else:
+        print(collinear_samples)
+        if getattr(func, '__closure__', None):
+            warnings.warn(f'Closure {func} cannot be parallelized by multiprocessing module. '
+                          'It is recommended to generate the function with functools.partial.')
+            executor = ThreadPoolExecutor
+        else:
+            executor = ProcessPoolExecutor
+        with executor(max_workers=workers) as ex:
+            futures = []
+            for p0, p1 in _prange(0, ngrids, grids_per_task):
+                f = ex.submit(_eval_xc_sf, func, rho_tmz[...,p0:p1], deriv, collinear_samples)
+                futures.append(f)
+            results = [f.result() for f in futures]
+        
     return [None if x[0] is None else np.concatenate(x, axis=-1) for x in zip(*results)]
 
+def _eval_xc_sf(func, rho_tmz, deriv, collinear_samples):
+    ngrids = rho_tmz.shape[-1]
+    # samples on z=cos(theta) and their weights between [0, 1]
+    sgridz, weights = _make_paxis_samples(collinear_samples)
+    blksize = int(np.ceil(1e5 / ngrids)) * 8
+
+    if rho_tmz.ndim == 2:
+        nvar = 1
+    else:
+        nvar = rho_tmz.shape[1]
+    # spin-flip part
+    fxc_sf = 0.0
+    for p0, p1 in _prange(0, weights.size, blksize):
+        rho = _project_spin_paxis2(rho_tmz, sgridz[p0:p1])
+        fxc = func(rho, deriv)[2]
+        fxc = fxc.reshape(2, nvar, 2, nvar, ngrids, p1 - p0)
+        fxc_sf += fxc[1,:,1].dot(weights[p0:p1])
+
+    return None,None,fxc_sf
+
 def eval_xc_collinear_spin(func, rho_tm, deriv, spin_samples):
     '''Multi-collinear functional derivatives for collinear spins
 
     Parameters
     ----------
     func : Function to evaluate collinear functionals.
         The function signature is
@@ -154,15 +204,15 @@
 
     # TODO: filter s, nabla(s) ~= 0
     m = rho_tm[1:].reshape(3, nvar, ngrids)
     s = rho_ts[1].reshape(nvar, ngrids)[0]
     with np.errstate(divide='ignore', invalid='ignore'):
         omega = m[:,0] / s
     omega[:,s==0] = 0
-
+    
     xc_orig = func(rho_ts, deriv)
     exc_eff = xc_orig[0]
 
     omega = omega.reshape(3, ngrids)
     if deriv > 0:
         vxc = xc_orig[1].reshape(2, nvar, ngrids)
         vxc_eff = np.vstack((vxc[:1], np.einsum('xg,rg->rxg', vxc[1], omega)))
@@ -205,26 +255,27 @@
                      collinear_threshold=None, collinear_samples=200):
     '''Multi-collinear effective potential and effective kernel with projection
     samples on spherical surface (the Lebedev grid samples)
     '''
     ngrids = rho_tm.shape[-1]
     sgrids, weights = _make_sph_samples(spin_samples)
     blksize = int(np.ceil(1e4 / ngrids)) * 8
-
+    # import pdb
+    # pdb.set_trace()
     if rho_tm.ndim == 2:
         nvar = 1
     else:
         nvar = rho_tm.shape[1]
-
-    exc_eff = vxc_eff = fxc_eff = 0
+    exc_eff = vxc_eff = fxc_eff = kxc_eff = 0
     for p0, p1 in _prange(0, weights.size, blksize):
         nsg = p1 - p0
         p_sgrids = sgrids[p0:p1]
         p_weights = weights[p0:p1]
         rho = _project_spin_sph(rho_tm, p_sgrids)
+        
         xc_orig = func(rho, deriv+1)
 
         exc = xc_orig[0].reshape(ngrids, nsg)
         vxc = xc_orig[1].reshape(2, nvar, ngrids, nsg)
 
         rho = rho.reshape(2, nvar, ngrids, nsg)
         s = rho[1]
@@ -245,14 +296,30 @@
             kxc = xc_orig[3].reshape(2, nvar, 2, nvar, 2, nvar, ngrids, nsg)
             fxc[1,:,1] *= 3
             fxc[0,:,1] *= 2
             fxc[1,:,0] *= 2
             fxc += np.einsum('xbyczgo,xgo->byczgo', kxc[1], s)
             fxc = np.einsum('rao,axbygo->rxbygo', c_tm, fxc)
             fxc_eff += np.einsum('sbo,rxbygo->rxsyg', cw_tm, fxc)
+            
+        if deriv > 2:
+            lxc = xc_orig[4].reshape(2, nvar, 2, nvar, 2, nvar, 2, nvar, ngrids, nsg)
+            kxc[1,:,1,:,1] *= 4
+            kxc[1,:,1,:,0] *= 3
+            kxc[1,:,0,:,1] *= 3
+            kxc[0,:,1,:,1] *= 3
+            kxc[1,:,0,:,0] *= 2
+            kxc[0,:,1,:,0] *= 2
+            kxc[0,:,0,:,1] *= 2
+
+            kxc += np.einsum('wbxcydzgo,wgo->bxcydzgo', lxc[1], s)
+            kxc = np.einsum('rao,axbyczgo->rxbyczgo', c_tm, kxc)
+            kxc = np.einsum('sbo,rxbyczgo->rxsyczgo', c_tm, kxc)
+            # kxc = np.einsum('rao,sbo,axbyczgo->rxsyczgo', c_tm, c_tm,kxc)
+            kxc_eff += np.einsum('tco,rxsyczgo->rxsytzg', cw_tm, kxc)
 
     # exc in libxc is defined as Exc per particle. exc_eff calculated above is exc*rho.
     # Divide exc_eff by rho so as to follow the convention of libxc
     if rho_tm.ndim == 2:
         rho_pure = rho_tm[0]
     else:
         rho_pure = rho_tm[0,0]
@@ -268,21 +335,25 @@
             xc_cs = eval_xc_collinear_spin(func, rho_tm[...,cs_idx], deriv,
                                            collinear_samples)
             exc_eff[...,cs_idx] = xc_cs[0]
             if deriv > 0:
                 vxc_eff[...,cs_idx] = xc_cs[1]
             if deriv > 1:
                 fxc_eff[...,cs_idx] = xc_cs[2]
+            if deriv > 2:
+                kxc_eff[...,cs_idx] = xc_cs[3]
 
     ret = [exc_eff]
     if deriv > 0:
         ret.append(vxc_eff)
     if deriv > 1:
         ret.append(fxc_eff)
     if deriv > 2:
+        ret.append(kxc_eff)
+    if deriv > 3:
         raise NotImplementedError
     return ret
 
 def _make_sph_samples(spin_samples):
     '''Integration samples on spherical surface'''
     ang_grids = MakeAngularGrid(spin_samples)
     directions = ang_grids[:,:3].copy(order='F')
@@ -331,25 +402,52 @@
     wt *= .5  # normalized to 1
     return rt, wt
 
 def _project_spin_paxis(rho_tm, sgridz=None):
     '''Projects spins onto the principal axis'''
     rho = rho_tm[0]
     m = rho_tm[1:]
+    
     s = np.linalg.norm(m, axis=0)
     if sgridz is None:
         rho_ts = np.stack([rho, s])
     else:
         ngrids = rho.shape[-1]
         nsg = sgridz.shape[0]
         if rho_tm.ndim == 2:
             rho_ts = np.empty((2, ngrids, nsg))
             rho_ts[0] = rho[:,np.newaxis]
             rho_ts[1] = s[:,np.newaxis] * sgridz
             rho_ts = rho_ts.reshape(2, ngrids * nsg)
         else:
+            print('222')
             nvar = rho_tm.shape[1]
             rho_ts = np.empty((2, nvar, ngrids, nsg))
             rho_ts[0] = rho[:,:,np.newaxis]
             rho_ts[1] = s[:,:,np.newaxis] * sgridz
             rho_ts = rho_ts.reshape(2, nvar, ngrids * nsg)
     return rho_ts
+
+def _project_spin_paxis2(rho_tm, sgridz=None):
+    # ToDo: be written into the function _project_spin_paxis().
+    # Because use mz rather than |mz| here
+    '''Projects spins onto the principal axis'''
+    rho = rho_tm[0]
+    mz = rho_tm[1]
+    
+    if sgridz is None:
+        rho_ts = np.stack([rho, mz])
+    else:
+        ngrids = rho.shape[-1]
+        nsg = sgridz.shape[0]
+        if rho_tm.ndim == 2:
+            rho_ts = np.empty((2, ngrids, nsg))
+            rho_ts[0] = rho[:,np.newaxis]
+            rho_ts[1] = mz[:,np.newaxis] * sgridz
+            rho_ts = rho_ts.reshape(2, ngrids * nsg)
+        else:
+            nvar = rho_tm.shape[1]
+            rho_ts = np.empty((2, nvar, ngrids, nsg))
+            rho_ts[0] = rho[:,:,np.newaxis]
+            rho_ts[1] = mz[:,:,np.newaxis] * sgridz
+            rho_ts = rho_ts.reshape(2, nvar, ngrids * nsg)
+    return rho_ts
```

### Comparing `MCfun-0.2.2/setup.py` & `MCfun-0.2.3/setup.py`

 * *Files identical despite different names*

