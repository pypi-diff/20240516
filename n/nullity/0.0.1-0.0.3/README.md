# Comparing `tmp/nullity-0.0.1.tar.gz` & `tmp/nullity-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nullity-0.0.1.tar", last modified: Thu May 16 07:49:27 2024, max compression
+gzip compressed data, was "nullity-0.0.3.tar", last modified: Thu May 16 08:19:46 2024, max compression
```

## Comparing `nullity-0.0.1.tar` & `nullity-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:49:27.319955 nullity-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 07:49:20.000000 nullity-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-16 07:49:27.319955 nullity-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-16 07:49:20.000000 nullity-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:49:27.315955 nullity-0.0.1/nullity/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 07:49:20.000000 nullity-0.0.1/nullity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16627 2024-05-16 07:49:20.000000 nullity-0.0.1/nullity/matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:49:27.319955 nullity-0.0.1/nullity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-16 07:49:27.000000 nullity-0.0.1/nullity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 07:49:27.000000 nullity-0.0.1/nullity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:49:27.000000 nullity-0.0.1/nullity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 07:49:27.000000 nullity-0.0.1/nullity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 07:49:27.000000 nullity-0.0.1/nullity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 07:49:27.319955 nullity-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 07:49:20.000000 nullity-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:19:46.136546 nullity-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-16 08:19:40.000000 nullity-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-16 08:19:46.136546 nullity-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2024-05-16 08:19:40.000000 nullity-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:19:46.132546 nullity-0.0.3/nullity/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 08:19:40.000000 nullity-0.0.3/nullity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18903 2024-05-16 08:19:40.000000 nullity-0.0.3/nullity/matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:19:46.132546 nullity-0.0.3/nullity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 08:19:46.000000 nullity-0.0.3/nullity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:19:46.136546 nullity-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 08:19:40.000000 nullity-0.0.3/setup.py
```

### Comparing `nullity-0.0.1/LICENSE` & `nullity-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nullity-0.0.1/PKG-INFO` & `nullity-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nullity
-Version: 0.0.1
+Version: 0.0.3
 Summary: A package for all things linear algebra
 Author: Mihir Aggarwal
 Author-email: mail@mihiraggarwal.me
 Keywords: linear,algebra,linear algebra,linalg,lin-alg,linearalgebra,eigen,eigenvalue,eigenvector,nullity,null,null space,rank nullity
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `nullity-0.0.1/README.md` & `nullity-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nullity-0.0.1/nullity/matrix.py` & `nullity-0.0.3/nullity/matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,66 +18,73 @@
     ru_ = None
     sp_ = None
     det_ = None
 
     def __init__(self, m:int, n:int, *args):
         self.m = m
         self.n = n
-        self.ls = [list(args[i: i+n]) for i in range(0, m*n, n)]
+        try:
+            self.ls = [list(args[i: i+n]) for i in range(0, m*n, n)]
+        except:
+            raise Exception("Dimensions and the number of values don't match")
 
     def nrows(self):
         return self.m
     
     def ncolumns(self):
         return self.n
     
     def is_square(self):
         return self.m == self.n
     
     def rref(self):
         if self.rref_:
             return self.rref_
 
-        ls = self.ls.copy()
-        i = 0
-        row = 0
-
-        while not self._checkRREF(ls):
-            zrow = True
-
-            for j in range(row, self.m):
-                if ls[j][i] != 0:
-                    zrow = False
-                    ls[row], ls[j] = ls[j], ls[row]
-                    break
-            
-            if zrow:
-                i += 1
-                continue
-            
-            ls[row] = [x / ls[row][i] for x in ls[row]]
+        try:
+            ls = self.ls.copy()
+            i = 0
+            row = 0
+
+            while not self._checkRREF(ls):
+                zrow = True
+
+                for j in range(row, self.m):
+                    if ls[j][i] != 0:
+                        zrow = False
+                        ls[row], ls[j] = ls[j], ls[row]
+                        break
+                
+                if zrow:
+                    i += 1
+                    continue
+                
+                ls[row] = [x / ls[row][i] for x in ls[row]]
 
-            for j in range(self.m):
-                if j != row:
-                    ls[j] = [ls[j][x] - (ls[j][i] * ls[row][x]) for x in range(self.n)]
-        
-            row += 1
+                for j in range(self.m):
+                    if j != row:
+                        ls[j] = [ls[j][x] - (ls[j][i] * ls[row][x]) for x in range(self.n)]
+            
+                row += 1
 
-            ls = [list(map(lambda x: round(x, 10), ls[i])) for i in range(self.m)]
+                ls = [list(map(lambda x: round(x, 10), ls[i])) for i in range(self.m)]
 
-            if row == self.m:
-                return Matrix(self.m, self.n, *[i for j in ls for i in j])
-            
-            i += 1
+                if row == self.m:
+                    return Matrix(self.m, self.n, *[i for j in ls for i in j])
+                
+                i += 1
 
-            if i == self.n:
-                return Matrix(self.m, self.n, *[i for j in ls for i in j])
+                if i == self.n:
+                    return Matrix(self.m, self.n, *[i for j in ls for i in j])
 
-        self.rref_ = Matrix(self.m, self.n, *[i for j in ls for i in j])
-        return self.rref_
+            self.rref_ = Matrix(self.m, self.n, *[i for j in ls for i in j])
+            return self.rref_
+        
+        except:
+            raise Exception("Something went wrong. Couldn't calculate RREF")
     
     def _checkRREF(self, ls):
         zrows = []
         place1 = []
         flag = True
 
         for i in range(len(ls)):
@@ -145,98 +152,106 @@
     def inverse(self):
         if not self.is_invertible():
             raise Exception("Matrix is not invertible")
         
         if self.inverse_:
             return self.inverse_
         
-        ls = self.ls.copy()
-        ils = [[0 for i in range(self.n)] for j in range(self.n)]
-        for i in range(self.n):
-            ils[i][i] = 1
-
-        i = 0
-        row = 0
-        while not self._checkRREF(ls):
-            zrow = True
-            for j in range(row, self.m):
-                if ls[j][i] != 0:
-                    zrow = False
-                    ls[row], ls[j] = ls[j], ls[row]
-                    ils[row], ils[j] = ils[j], ils[row]
-                    break
+        try:
+            ls = self.ls.copy()
+            ils = [[0 for i in range(self.n)] for j in range(self.n)]
+            for i in range(self.n):
+                ils[i][i] = 1
+
+            i = 0
+            row = 0
+            while not self._checkRREF(ls):
+                zrow = True
+                for j in range(row, self.m):
+                    if ls[j][i] != 0:
+                        zrow = False
+                        ls[row], ls[j] = ls[j], ls[row]
+                        ils[row], ils[j] = ils[j], ils[row]
+                        break
+                    
+                if zrow:
+                    i += 1
+                    continue
                 
-            if zrow:
-                i += 1
-                continue
-            
-            ils[row] = [x / ls[row][i] for x in ils[row]]
-            ls[row] = [x / ls[row][i] for x in ls[row]]
+                ils[row] = [x / ls[row][i] for x in ils[row]]
+                ls[row] = [x / ls[row][i] for x in ls[row]]
 
-            for j in range(self.m):
-                if j != row:
-                    ils[j] = [ils[j][x] - (ls[j][i] * ils[row][x]) for x in range(self.n)]
-                    ls[j] = [ls[j][x] - (ls[j][i] * ls[row][x]) for x in range(self.n)]
-        
-            row += 1
-            if row == self.m:
-                self.inverse_ = Matrix(self.m, self.n, *[i for j in ils for i in j])
-                return self.inverse_
+                for j in range(self.m):
+                    if j != row:
+                        ils[j] = [ils[j][x] - (ls[j][i] * ils[row][x]) for x in range(self.n)]
+                        ls[j] = [ls[j][x] - (ls[j][i] * ls[row][x]) for x in range(self.n)]
             
-            i += 1
-            if i == self.n:
-                self.inverse_ = Matrix(self.m, self.n, *[i for j in ils for i in j])
-                return self.inverse_
+                row += 1
+                if row == self.m:
+                    self.inverse_ = Matrix(self.m, self.n, *[i for j in ils for i in j])
+                    return self.inverse_
+                
+                i += 1
+                if i == self.n:
+                    self.inverse_ = Matrix(self.m, self.n, *[i for j in ils for i in j])
+                    return self.inverse_
 
-        self.inverse_ = Matrix(self.m, self.n, *[i for j in ils for i in j])
-        return self.inverse_
+            self.inverse_ = Matrix(self.m, self.n, *[i for j in ils for i in j])
+            return self.inverse_
+        
+        except:
+            raise Exception("Something went wrong. Couldn't invert")
 
     def rank_factorization(self):
         if self.r_ and self.c_:
             return self.r_, self.c_
 
         if not self.rref_:
             self.rref_ = self.rref()
 
         if not self.rank_:
             self.rank_ = self.rank()
 
-        r = [self.rref_[i] for i in range(self.rank_)]
-        k = 0
-        c = []
-        cols = []
-        for i in range(self.n):
-            t = []
-            flag = True
-            if self.rref_[k][i] != 1:
-                flag = False
-                continue
-            else:
-                for j in range(self.m):
-                    if j != k and self.rref_[j][i] != 0:
-                        flag = False
+        try:
+            r = [self.rref_[i] for i in range(self.rank_)]
+            k = 0
+            c = []
+            cols = []
+            for i in range(self.n):
+                t = []
+                flag = True
+                if self.rref_[k][i] != 1:
+                    flag = False
+                    continue
+                else:
+                    for j in range(self.m):
+                        if j != k and self.rref_[j][i] != 0:
+                            flag = False
+                            break
+                        
+                if flag:
+                    cols.append(i)
+                    k += 1
+
+                    if k >= self.m:
                         break
-                    
-            if flag:
-                cols.append(i)
-                k += 1
 
-                if k >= self.m:
-                    break
+            self.pivot_cols_ = cols
+            for i in range(self.m):
+                t = []
+                for j in cols:
+                    t.append(self.ls[i][j])
+                c.append(t)
 
-        self.pivot_cols_ = cols
-        for i in range(self.m):
-            t = []
-            for j in cols:
-                t.append(self.ls[i][j])
-            c.append(t)
-
-        self.r_ = Matrix(len(r), len(r[0]), *[i for j in r for i in j])
-        self.c_ = Matrix(len(c), len(c[0]), *[i for j in c for i in j])
-        return self.r_, self.c_
+            self.r_ = Matrix(len(r), len(r[0]), *[i for j in r for i in j])
+            self.c_ = Matrix(len(c), len(c[0]), *[i for j in c for i in j])
+            return self.r_, self.c_
+        
+        except:
+            raise Exception("Something went wrong. Couldn't factorize")
     
     def row_basis(self):
         if not self.r_:
             self.r_, self.c_ = self.rank_factorization()
 
         return self.r_
     
@@ -251,155 +266,175 @@
             self.rank_factorization()
 
         non_pivot = []
         for i in range(self.n):
             if i not in self.pivot_cols_:
                 non_pivot.append(i)
 
-        soln_set = []
-        k = 0
-        for i in range(self.n):
-            ind = []
-            if i in non_pivot:
+        try:
+            soln_set = []
+            k = 0
+            for i in range(self.n):
+                ind = []
+                if i in non_pivot:
+                    for j in non_pivot:
+                        if i == j:
+                            ind.append(1)
+                        else:
+                            ind.append(0)
+                    soln_set.append(ind)
+                    continue
                 for j in non_pivot:
-                    if i == j:
-                        ind.append(1)
-                    else:
-                        ind.append(0)
+                    ind.append(-self.rref_[k][j])
                 soln_set.append(ind)
-                continue
-            for j in non_pivot:
-                ind.append(-self.rref_[k][j])
-            soln_set.append(ind)
-            k += 1
-
-        null_mt = [[0 for i in range(len(soln_set))] for j in range(len(soln_set[0]))]
-        for i in range(len(soln_set)):
-            for j in range(len(soln_set[i])):
-                null_mt[j][i] = soln_set[i][j]
+                k += 1
+
+            null_mt = [[0 for i in range(len(soln_set))] for j in range(len(soln_set[0]))]
+            for i in range(len(soln_set)):
+                for j in range(len(soln_set[i])):
+                    null_mt[j][i] = soln_set[i][j]
 
-        if null_mt == []:
-            return null_mt
+            if null_mt == []:
+                return null_mt
+            
+            self.null_basis_ = Matrix(len(null_mt), len(null_mt[0]), *[i for j in null_mt for i in j]).transpose()
+            return self.null_basis_
         
-        self.null_basis_ = Matrix(len(null_mt), len(null_mt[0]), *[i for j in null_mt for i in j]).transpose()
-        return self.null_basis_
+        except:
+            raise Exception("Something went wrong. Couldn't find the null basis")
     
     def transpose(self):
         t = [[0 for i in range(self.m)] for j in range(self.n)]
         for i in range(self.m):
             for j in range(self.n):
                 t[j][i] = self.ls[i][j]
         return Matrix(self.n, self.m, *[i for j in t for i in j])
     
     def plu(self):
         if not self.is_square():
             raise Exception("Matrix is not square")
         
-        p = [[0 if j != i else 1 for j in range(self.n)] for i in range(self.n)]
-        l = [[0 if j != i else 1 for j in range(self.n)] for i in range(self.n)]
-
-        sp = 0
-        mt = self.ls.copy()
-        for col in range(self.n):
-            r = col
-            while r < self.n and mt[r][col] == 0:
-                r += 1
-            if r < self.n:
-                if col != r:
-                    mt[col], mt[r] = mt[r], mt[col]
-                    p[col], p[r] = p[r], p[col]
-                    sp += 1
-            else:
-                continue
+        try:
+            p = [[0 if j != i else 1 for j in range(self.n)] for i in range(self.n)]
+            l = [[0 if j != i else 1 for j in range(self.n)] for i in range(self.n)]
+
+            sp = 0
+            mt = self.ls.copy()
+            for col in range(self.n):
+                r = col
+                while r < self.n and mt[r][col] == 0:
+                    r += 1
+                if r < self.n:
+                    if col != r:
+                        mt[col], mt[r] = mt[r], mt[col]
+                        p[col], p[r] = p[r], p[col]
+                        sp += 1
+                else:
+                    continue
 
-            for i in range(col+1, self.n):
-                if mt[i][col] != 0:
-                    sub = mt[i][col] / mt[col][col]
-                    for j in range(self.n):
-                        mt[i][j] = mt[i][j] - (sub * mt[col][j])
-                    l[i][col] = sub
-        
-        self.p_ = Matrix(len(p), len(p[0]), *[i for j in p for i in j])
-        self.l_ = Matrix(len(l), len(l[0]), *[i for j in l for i in j])
-        self.u_ = Matrix(len(mt), len(mt[0]), *[i for j in mt for i in j])
-        self.sp_ = sp
-        return self.p_, self.l_, self.u_
+                for i in range(col+1, self.n):
+                    if mt[i][col] != 0:
+                        sub = mt[i][col] / mt[col][col]
+                        for j in range(self.n):
+                            mt[i][j] = mt[i][j] - (sub * mt[col][j])
+                        l[i][col] = sub
+            
+            self.p_ = Matrix(len(p), len(p[0]), *[i for j in p for i in j])
+            self.l_ = Matrix(len(l), len(l[0]), *[i for j in l for i in j])
+            self.u_ = Matrix(len(mt), len(mt[0]), *[i for j in mt for i in j])
+            self.sp_ = sp
+            return self.p_, self.l_, self.u_
+        
+        except:
+            raise Exception("Something went wrong. Couldn't factorize")
     
     def det(self):
         if not self.is_square():
             raise Exception("Matrix is not square")
         if not (self.p_ and self.l_ and self.u_):
             self.plu()
 
-        p = 1
-        for i in range(self.n):
-            p *= self.u_[i][i]
+        try:
+            p = 1
+            for i in range(self.n):
+                p *= self.u_[i][i]
 
-        self.det_ = self.sp_ * p
-        return self.sp_ * p
+            self.det_ = self.sp_ * p
+            return self.sp_ * p
+        
+        except:
+            raise Exception("Something went wrong")
     
     def qr(self):
-        v = self.transpose()
-        onb = []
-
-        for k in range(len(v)):
-            u = [0 for i in range(self.m)]
-            s = [0 for i in range(self.m)]
-
-            for i in range(k):
-                st = 0
-                for j in range(len(v)):
-                    st += (v[k][j] * onb[i][j])
-                ml = tuple(map(lambda i: st*i, onb[i]))
-                for j in range(self.m):
-                    s[j] += ml[j]
-
-            for i in range(self.m):
-                u[i] = v[k][i] - s[i]
-            if list(map(lambda x: round(x, 5), u)) == [0 for x in range(len(u))]:
-                continue
-            sw = 0
-
-            for i in range(len(u)):
-                sw += (u[i]**2)
-            w = list(map(lambda i: i / (sw**0.5), u))
-            onb.append(w)
+        try:
+            v = self.transpose()
+            onb = []
+
+            for k in range(len(v)):
+                u = [0 for i in range(self.m)]
+                s = [0 for i in range(self.m)]
+
+                for i in range(k):
+                    st = 0
+                    for j in range(len(v)):
+                        st += (v[k][j] * onb[i][j])
+                    ml = tuple(map(lambda i: st*i, onb[i]))
+                    for j in range(self.m):
+                        s[j] += ml[j]
+
+                for i in range(self.m):
+                    u[i] = v[k][i] - s[i]
+                if list(map(lambda x: round(x, 5), u)) == [0 for x in range(len(u))]:
+                    continue
+                sw = 0
+
+                for i in range(len(u)):
+                    sw += (u[i]**2)
+                w = list(map(lambda i: i / (sw**0.5), u))
+                onb.append(w)
 
-        if (len(onb) < self.n):
+            if (len(onb) < self.n):
 
-            onbc = [[onb[j][i] for i in range(len(onb[0]))] for j in range(len(onb))]
-            basis = Matrix(len(onbc), len(onbc[0]), *[ind for ionb in onbc for ind in ionb]).null_basis().transpose()
+                onbc = [[onb[j][i] for i in range(len(onb[0]))] for j in range(len(onb))]
+                basis = Matrix(len(onbc), len(onbc[0]), *[ind for ionb in onbc for ind in ionb]).null_basis().transpose()
+                
+                sv = 0
+                for i in range(len(basis[0])):
+                    sv += (basis[0][i]**2)
+                w = list(map(lambda i: i / (sv**0.5), basis[0]))
+                onb.append(w)
             
-            sv = 0
-            for i in range(len(basis[0])):
-                sv += (basis[0][i]**2)
-            w = list(map(lambda i: i / (sv**0.5), basis[0]))
-            onb.append(w)
-        
-        r = Matrix(len(onb), len(onb[0]), *[o for nb in onb for o in nb]) * Matrix(self.m, self.n, *[o for nb in self.ls for o in nb])
-
-        self.q_ = Matrix(len(onb), len(onb[0]), *[o for nb in onb for o in nb]).transpose()
-        self.ru_ = Matrix(len(r), len(r[0]), *[a for b in r for a in b])
-        return self.q_, self.ru_
+            r = Matrix(len(onb), len(onb[0]), *[o for nb in onb for o in nb]) * Matrix(self.m, self.n, *[o for nb in self.ls for o in nb])
+
+            self.q_ = Matrix(len(onb), len(onb[0]), *[o for nb in onb for o in nb]).transpose()
+            self.ru_ = Matrix(len(r), len(r[0]), *[a for b in r for a in b])
+            return self.q_, self.ru_
+        
+        except:
+            raise Exception("Something went wrong. Couldn't factorize")
 
     def charpol(self):
-        mc = [[self.ls[j][i] for i in range(self.n)] for j in range(self.m)]
-        for i in range(self.m):
-            for j in range(self.n):
-                if i == j:
-                    mc[i][j] = [mc[i][j], -1]
-                else:
-                    mc[i][j] = [mc[i][j]]
-        d = self._cdet(self.n, mc)
-        self.charpol_ = d
-        cp = []
-        for i in range(self.n, -1, -1):
-            cp.append(f"({d[i]}x^{i})")
+        try:
+            mc = [[self.ls[j][i] for i in range(self.n)] for j in range(self.m)]
+            for i in range(self.m):
+                for j in range(self.n):
+                    if i == j:
+                        mc[i][j] = [mc[i][j], -1]
+                    else:
+                        mc[i][j] = [mc[i][j]]
+            d = self._cdet(self.n, mc)
+            self.charpol_ = d
+            cp = []
+            for i in range(self.n, -1, -1):
+                cp.append(f"({d[i]}x^{i})")
 
-        return f"{'+'.join(cp)}"
+            return f"{'+'.join(cp)}"
+        
+        except:
+            raise Exception("Something went wrong")        
     
     def _cdet(self, n, ls):
         def _padd(a, b):
             l = max(len(a), len(b))
             c = [0 for i in range(l)]
             if len(a) < len(b):
                 for i in range(len(a)):
@@ -432,71 +467,80 @@
                         c += 1
                 r += 1
             s = _padd(s, (_pmul([(-1)**(i)], _pmul(ls[0][i], self._cdet(n-1, t)))))
         return s
 
     def eigenvals(self):
         import numpy as np
-        return sorted(np.linalg.eigvals(self.ls), reverse=True)
+        try: return sorted(np.linalg.eigvals(self.ls), reverse=True)
+        except: raise Exception("Something went wrong. Couldn't find the eigenvalues")
 
     def eigenvecs(self):
         if not self.eigenvals_:
             self.eigenvals_ = self.eigenvals()
 
-        eigenvecs_ = []
-        for i in range(len(self.eigenvals_)):
-            mt = [[self.ls[j][i] for i in range(self.n)] for j in range(self.m)]
-            for j in range(self.n):
-                mt[j][j] -= self.eigenvals_[i]
-            nb = Matrix(self.m, self.n, *[i for j in mt for i in j]).null_basis().transpose()
-
-            for i in range(len(nb)):
-                c = []
-                for j in range(len(nb[0])):
-                    c.append(nb[i][j])
-                eigenvecs_.append(c)
+        try:
+            eigenvecs_ = []
+            for i in range(len(self.eigenvals_)):
+                mt = [[self.ls[j][i] for i in range(self.n)] for j in range(self.m)]
+                for j in range(self.n):
+                    mt[j][j] -= self.eigenvals_[i]
+                nb = Matrix(self.m, self.n, *[i for j in mt for i in j]).null_basis().transpose()
+
+                for i in range(len(nb)):
+                    c = []
+                    for j in range(len(nb[0])):
+                        c.append(nb[i][j])
+                    eigenvecs_.append(c)
+            
+            self.eigenvecs_ = Matrix(len(eigenvecs_), len(eigenvecs_[0]), *[i for j in eigenvecs_ for i in j]).transpose()
+            return self.eigenvecs_
         
-        self.eigenvecs_ = Matrix(len(eigenvecs_), len(eigenvecs_[0]), *[i for j in eigenvecs_ for i in j]).transpose()
-        return self.eigenvecs_
+        except:
+            raise Exception("Something went wrong. Couldn't find the eigenvectors")
     
     def svd(self):
-        lst = self.transpose()
-        mls = Matrix(self.m, self.n, *[i for j in self.ls for i in j])
-        lstls = lst * mls
-        
-        lm = Matrix(self.n, self.n, *[i for j in lstls for i in j])
-
-        print(lm)
-        evals = lm.eigenvals()
-        evecs = lm.eigenvecs().transpose()
-
-        v_t = []
-        for i in range(len(evecs)):
-            s = 0
-            for j in range(len(evecs[i])):
-                s += (evecs[i][j]**2)
-            t = s**0.5
-            v_t.append(list(map(lambda x: x / t, evecs[i])))
-
-        v_t = Matrix(self.n, self.n, *[i for j in v_t for i in j])
-        v = v_t.transpose()
-        
-        sig = [[0 for a in range(self.n)] for b in range(self.m)]
-        for i in range(min(self.m, self.n)):
-            sig[i][i] = evals[i]**0.5
-        sig = Matrix(self.m, self.n, *[i for j in sig for i in j])
+        try:
+            lst = self.transpose()
+            mls = Matrix(self.m, self.n, *[i for j in self.ls for i in j])
+            lstls = lst * mls
+            
+            lm = Matrix(self.n, self.n, *[i for j in lstls for i in j])
 
-        u = [[0 for a in range(self.m)] for b in range(self.m)]
-        for i in range(self.m):
-            mid = [[v[k][i]] for k in range(self.n)]
-            mml = mls * Matrix(len(mid), len(mid[0]), *[l for j in mid for l in j])
-            u[i] = list(map(lambda x: x[0]/evals[i]**0.5, mls * Matrix(len(mid), len(mid[0]), *[l for j in mid for l in j])))
-        u = Matrix(self.m, self.m, *[i for j in u for i in j])
+            print(lm)
+            evals = lm.eigenvals()
+            evecs = lm.eigenvecs().transpose()
+
+            v_t = []
+            for i in range(len(evecs)):
+                s = 0
+                for j in range(len(evecs[i])):
+                    s += (evecs[i][j]**2)
+                t = s**0.5
+                v_t.append(list(map(lambda x: x / t, evecs[i])))
 
-        return u, sig, v_t
+            v_t = Matrix(self.n, self.n, *[i for j in v_t for i in j])
+            v = v_t.transpose()
+            
+            sig = [[0 for a in range(self.n)] for b in range(self.m)]
+            for i in range(min(self.m, self.n)):
+                sig[i][i] = evals[i]**0.5
+            sig = Matrix(self.m, self.n, *[i for j in sig for i in j])
+
+            u = [[0 for a in range(self.m)] for b in range(self.m)]
+            for i in range(self.m):
+                mid = [[v[k][i]] for k in range(self.n)]
+                mml = mls * Matrix(len(mid), len(mid[0]), *[l for j in mid for l in j])
+                u[i] = list(map(lambda x: x[0]/evals[i]**0.5, mls * Matrix(len(mid), len(mid[0]), *[l for j in mid for l in j])))
+            u = Matrix(self.m, self.m, *[i for j in u for i in j])
+
+            return u, sig, v_t
+        
+        except:
+            raise Exception("Something went wrong. Couldn't factorize")
 
     def __add__(self, other):
         if not (self.m == other.m and self.n == other.n):
             raise Exception("Unequal matrix dimensions")
         
         t = [[0 for i in range(self.n)] for j in range(self.m)]
         for i in range(self.m):
```

### Comparing `nullity-0.0.1/nullity.egg-info/PKG-INFO` & `nullity-0.0.3/nullity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nullity
-Version: 0.0.1
+Version: 0.0.3
 Summary: A package for all things linear algebra
 Author: Mihir Aggarwal
 Author-email: mail@mihiraggarwal.me
 Keywords: linear,algebra,linear algebra,linalg,lin-alg,linearalgebra,eigen,eigenvalue,eigenvector,nullity,null,null space,rank nullity
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `nullity-0.0.1/setup.py` & `nullity-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.3'
 DESCRIPTION = 'A package for all things linear algebra'
 
 here = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(here, "README.md")) as f:
     long_description = f.read()
 
 setup(
```

