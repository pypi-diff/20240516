# Comparing `tmp/ScanLHA-0.3.tar.gz` & `tmp/ScanLHA-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScanLHA-0.3.tar", last modified: Mon Dec 31 13:45:38 2018, max compression
+gzip compressed data, was "ScanLHA-0.4.tar", last modified: Thu Apr 29 07:22:39 2021, max compression
```

## Comparing `ScanLHA-0.3.tar` & `ScanLHA-0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       19 2018-11-19 19:22:15.413651 ScanLHA-0.3/.gitattributes
--rw-r--r--   0        0        0       50 2018-07-21 00:32:14.277115 ScanLHA-0.3/.gitignore
--rw-r--r--   0        0        0       13 2018-07-21 00:32:14.277115 ScanLHA-0.3/.pylintrc
--rw-r--r--   0        0        0    32422 2018-08-04 11:55:53.638442 ScanLHA-0.3/LICENSE
--rw-r--r--   0        0        0     8540 2018-11-19 20:18:13.295416 ScanLHA-0.3/README.md
--rw-r--r--   0        0        0     1565 2018-11-10 14:50:52.984502 ScanLHA-0.3/ScanLHA/EditLHA.py
--rw-r--r--   0        0        0     2255 2018-10-27 18:59:54.554932 ScanLHA-0.3/ScanLHA/MergeLHA.py
--rw-r--r--   0        0        0    12569 2018-11-10 13:25:00.350770 ScanLHA-0.3/ScanLHA/PlotLHA.py
--rw-r--r--   0        0        0     5317 2018-12-01 16:18:46.019182 ScanLHA-0.3/ScanLHA/ScanLHA.py
--rw-r--r--   0        0        0     8947 2018-12-31 13:44:12.856450 ScanLHA-0.3/ScanLHA/__init__.py
--rw-r--r--   0        0        0    14061 2018-11-10 13:32:51.243157 ScanLHA-0.3/ScanLHA/config.py
--rw-r--r--   0        0        0     2126 2018-10-27 18:59:54.551599 ScanLHA-0.3/ScanLHA/configs/SPheno.yml
--rw-r--r--   0        0        0    14670 2018-12-01 15:51:57.207228 ScanLHA-0.3/ScanLHA/runner.py
--rw-r--r--   0        0        0    11569 2018-12-31 13:30:30.930548 ScanLHA-0.3/ScanLHA/scan.py
--rw-r--r--   0        0        0     3157 2018-10-27 18:59:54.561598 ScanLHA-0.3/ScanLHA/slha.py
--rw-r--r--   0        0        0    36811 2018-11-19 20:18:14.118738 ScanLHA-0.3/docs/EditLHA.m.html
--rw-r--r--   0        0        0    41750 2018-11-19 20:18:14.128737 ScanLHA-0.3/docs/MergeLHA.m.html
--rw-r--r--   0        0        0   173820 2018-11-19 20:18:14.222069 ScanLHA-0.3/docs/PlotLHA.m.html
--rw-r--r--   0        0        0    66298 2018-11-19 20:18:14.245402 ScanLHA-0.3/docs/ScanLHA.m.html
--rw-r--r--   0        0        0   180179 2018-11-19 20:18:14.342068 ScanLHA-0.3/docs/config.m.html
--rw-r--r--   0        0        0    47921 2018-11-19 20:18:14.108738 ScanLHA-0.3/docs/index.html
--rw-r--r--   0        0        0   277823 2018-11-19 20:18:14.528731 ScanLHA-0.3/docs/runner.m.html
--rw-r--r--   0        0        0   178199 2018-11-19 20:18:14.618730 ScanLHA-0.3/docs/scan.m.html
--rw-r--r--   0        0        0    57629 2018-11-19 20:18:14.638730 ScanLHA-0.3/docs/slha.m.html
--rwxr-xr-x   0        0        0      214 2018-11-19 19:18:33.567929 ScanLHA-0.3/makedocs
--rw-r--r--   0        0        0      647 2018-11-19 20:56:27.058492 ScanLHA-0.3/pyproject.toml
--rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 ScanLHA-0.3/setup.py
--rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 ScanLHA-0.3/PKG-INFO
+-rw-r--r--   0        0        0       19 2018-11-19 19:22:15.413651 ScanLHA-0.4/.gitattributes
+-rw-r--r--   0        0        0       63 2021-04-29 07:22:05.208171 ScanLHA-0.4/.gitignore
+-rw-r--r--   0        0        0       13 2018-07-21 00:32:14.277115 ScanLHA-0.4/.pylintrc
+-rw-r--r--   0        0        0    32422 2018-08-04 11:55:53.638442 ScanLHA-0.4/LICENSE
+-rw-r--r--   0        0        0     8540 2018-11-19 20:18:13.295416 ScanLHA-0.4/README.md
+-rw-r--r--   0        0        0     1965 2021-04-29 07:22:05.208171 ScanLHA-0.4/ScanLHA/EditLHA.py
+-rw-r--r--   0        0        0     2221 2021-04-29 07:22:05.208171 ScanLHA-0.4/ScanLHA/MergeLHA.py
+-rw-r--r--   0        0        0    16676 2021-04-29 07:22:05.208171 ScanLHA-0.4/ScanLHA/PlotLHA.py
+-rw-r--r--   0        0        0     5317 2018-12-01 16:18:46.019182 ScanLHA-0.4/ScanLHA/ScanLHA.py
+-rw-r--r--   0        0        0     8947 2021-04-29 07:22:05.208171 ScanLHA-0.4/ScanLHA/__init__.py
+-rw-r--r--   0        0        0    14312 2021-04-29 07:22:05.211504 ScanLHA-0.4/ScanLHA/config.py
+-rw-r--r--   0        0        0     2126 2018-10-27 18:59:54.551599 ScanLHA-0.4/ScanLHA/configs/SPheno.yml
+-rw-r--r--   0        0        0    14960 2021-04-29 07:22:05.211504 ScanLHA-0.4/ScanLHA/runner.py
+-rw-r--r--   0        0        0    11935 2021-04-29 07:22:05.211504 ScanLHA-0.4/ScanLHA/scan.py
+-rw-r--r--   0        0        0     3699 2020-11-04 13:11:52.376273 ScanLHA-0.4/ScanLHA/slha.py
+-rw-r--r--   0        0        0    36811 2018-11-19 20:18:14.118738 ScanLHA-0.4/docs/EditLHA.m.html
+-rw-r--r--   0        0        0    41750 2018-11-19 20:18:14.128737 ScanLHA-0.4/docs/MergeLHA.m.html
+-rw-r--r--   0        0        0   173820 2018-11-19 20:18:14.222069 ScanLHA-0.4/docs/PlotLHA.m.html
+-rw-r--r--   0        0        0    66298 2018-11-19 20:18:14.245402 ScanLHA-0.4/docs/ScanLHA.m.html
+-rw-r--r--   0        0        0   180179 2018-11-19 20:18:14.342068 ScanLHA-0.4/docs/config.m.html
+-rw-r--r--   0        0        0    47921 2018-11-19 20:18:14.108738 ScanLHA-0.4/docs/index.html
+-rw-r--r--   0        0        0   277823 2018-11-19 20:18:14.528731 ScanLHA-0.4/docs/runner.m.html
+-rw-r--r--   0        0        0   178199 2018-11-19 20:18:14.618730 ScanLHA-0.4/docs/scan.m.html
+-rw-r--r--   0        0        0    57629 2018-11-19 20:18:14.638730 ScanLHA-0.4/docs/slha.m.html
+-rwxr-xr-x   0        0        0      214 2018-11-19 19:18:33.567929 ScanLHA-0.4/makedocs
+-rw-r--r--   0        0        0      647 2018-11-19 20:56:27.058492 ScanLHA-0.4/pyproject.toml
+-rw-r--r--   0        0        0      961 1970-01-01 00:00:00.000000 ScanLHA-0.4/setup.py
+-rw-r--r--   0        0        0      254 1970-01-01 00:00:00.000000 ScanLHA-0.4/PKG-INFO
```

### Comparing `ScanLHA-0.3/LICENSE` & `ScanLHA-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/README.md` & `ScanLHA-0.4/README.md`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/ScanLHA/EditLHA.py` & `ScanLHA-0.4/ScanLHA/EditLHA.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 #!/usr/bin/env python3
 """
 Interactively load/edit/save/plot HDF files.
 """
-from pandas import read_hdf, DataFrame # noqa: F401
 try:
     from IPython import embed
     ipy = True
 except:
     import code
-    ipyt = False
+    ipy = False
+import pandas as pd # noqa: F401
 from glob import glob
-import os
-from matplotlib import pyplot as plt # noqa: F401
+from os import path, getenv, chdir
 from argparse import ArgumentParser
+import matplotlib
+matplotlib.use('Agg')
+import matplotlib.pyplot as plt # noqa: E402, F401
+from pandas import read_hdf, DataFrame, HDFStore # noqa: F401, E402
+
 __pdoc__ = {}
 __pdoc__['Edit'] = """
     Usage: EditLHA [-h] h5file.h5 [h5file.h5 ...]
 
     Loads the hdf files and saves them into the variable DATA.
 
     An IPython session with imported matplotlib.pyplot is started.
@@ -27,32 +31,42 @@
 def Edit():
     parser = ArgumentParser(description='Interactively load/edit/save/plot HDF files.')
     parser.add_argument('files', metavar='h5file.h5', type=str, nargs='+',
             help='HDF file(s) to edit.')
     args = parser.parse_args()
 
     HDFFILES = [ k for f in args.files for k in glob(f) ]
+    LHAPATH = getenv('LHAPATH') if getenv('LHAPATH') else 'results'
+    store = False
 
     DATA = {}
     header = "Your data files are stored in 'DATA'"
     for f in HDFFILES:
         print('Reading %s ...' % f)
         DATA[f] = read_hdf(f)
 
     if len(DATA) == 1:
         HDFFILE = HDFFILES[0]
         DATA = DATA[HDFFILE]
+        store = HDFStore(HDFFILE)
+        try:
+            conf = store.get_storer(LHAPATH).attrs.config
+        except:
+            print("no config stored in hdf file")
     else:
         header += "and accessible via DATA['path/to/filename.h5']"
 
     if len(DATA) == 0:
         print('No valid data files specified.\n')
     else:
-        HDFDIR = os.path.dirname(os.path.abspath(HDFFILES[0])) + '/'
+        HDFDIR = path.dirname(path.abspath(HDFFILES[0])) + '/'
         print('Changing working directory to {}.\n'.format(HDFDIR))
-        os.chdir(HDFDIR)
+        chdir(HDFDIR)
 
     if ipy:
         embed(header=header)
     else:
         print(header)
         code.interact(local=locals())
+
+    if store:
+        store.close()
```

### Comparing `ScanLHA-0.3/ScanLHA/MergeLHA.py` & `ScanLHA-0.4/ScanLHA/MergeLHA.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from glob import glob
 import sys
 from os import getenv
 __pdoc__ = {}
 __pdoc__['Merge'] = """
 Merges multiple HDF files into one file.
 
-Usage: MergeLHA mergedfile.h5 file1.h5 file2.h5 [...]
+Usage: MergeLHA file1.h5 file2.h5 [...] mergedfile.h5
 
 File names may be specified using patterns compatible with python.glob (e.g. '*.h5').
 
 Note that it is not possible to merge different `ScanLHA.config.Config` instances i.e. the `Config`
 instance of the first file is used.
 
 
@@ -38,21 +38,21 @@
 
     df = DataFrame()
     store_conf = None
     for fs in infiles:
         for f in fs:
             print('Reading %s ...' % f)
             tmp_store = HDFStore(f)
-            tmp_conf = tmp_store.get_storer(LHAPATH).attrs.config
             try:
                 tmp_conf = tmp_store.get_storer(LHAPATH).attrs.config
                 if not store_conf:
                     store_conf = tmp_conf
             except AttributeError:
                 print('No config attribute found in {}'.format(f))
+                store_conf = {}
             if 'scatterplot' in store_conf:
                 tmp_conf['scatterplot'] = store_conf['scatterplot']
             if store_conf and store_conf != tmp_conf:
                 print('Warning: merge file with different config {}'.format(f))
             tmp_df = tmp_store['results']
             try:
                 tmp_df['scan_seed'] = tmp_store.get_storer(LHAPATH).attrs.seed
```

### Comparing `ScanLHA-0.3/ScanLHA/PlotLHA.py` & `ScanLHA-0.4/ScanLHA/PlotLHA.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,77 +1,105 @@
 #!/usr/bin/env python3
 """
 Plot ScanLHA scan results.
 """
 from pandas import HDFStore
-# from IPython import embed
 import logging
 import os
+import sys
 from .config import Config
 from math import * # noqa: E403 F401 F403
 from collections import ChainMap
 from argparse import ArgumentParser
+from numpy import nan  # noqa: F401
 import matplotlib
 from matplotlib.colors import LogNorm, Normalize
 from matplotlib.colorbar import ColorbarBase
+import importlib
 matplotlib.use('Agg')
 # matplotlib.use('ps')
 import matplotlib.pyplot as plt # noqa: E402
+from IPython import embed # noqa: F402, E402
+
+if os.path.isfile('functions.py'):
+    sys.path.append(os.getcwd())
+    functions = importlib.import_module('functions')
 
 __all__ = ['Plot', 'PlotConf', 'axisdefault']
 
+def arg(re,im):
+    """argument of complex number with real part re and imaginary part im """
+    arg = 0
+    if re > 0:
+        arg = atan(im/re)       # noqa: F405
+    elif re < 0 and im >= 0:
+        arg = atan(im/re)+pi    # noqa: F405
+    elif re < 0 and im < 0:
+        arg = atan(im/re)-pi    # noqa: F405
+    elif re == 0 and im > 0:
+        arg = pi/2              # noqa: F405
+    elif re == 0 and im < 0:
+        arg = -pi/2             # noqa: F405
+    elif re == 0 and im == 0:
+        arg = 0
+    return arg
+
 axisdefault = {
         'boundaries' : [],
         'lognorm' : False,
         'vmin' : None,
         'vmax' : None,
         'ticks' :  [],
         'colorbar' : False,
         'colorbar_orientation': 'horizontal',
         'label' : None,
         'datafile' : None
 }
 """
 Default values for all axes.
 """
-
 class PlotConf(ChainMap):
     """ Config class which allows for successively defined defaults """
     def __init__(self, *args):
         super().__init__(*args)
         self.maps.append({
             'x-axis': axisdefault,
             'y-axis': axisdefault,
             'z-axis': axisdefault,
             'colorbar_only': False,
             'constraints': [],
+            'type': 'scatter',
             'legend': {
-                'loc' : 'right',
-                'bbox_to_anchor' : [1.5, 0.5]
+#                'loc' : 'right',
+#                'bbox_to_anchor' : [1.5, 0.5]
                 },
+            'figsize': None,
             'hline': False,
             'vline': False,
+            'exec': False,
             'lw': 1.0,
             's': None,
             'title': False,
             'label': None,
             'cmap': None,
             'alpha' : 1.0,
             'datafile': 'results.h5',
-            'fontsize': 28,
+            'fontsize': 11,
+            'tick_params': {},
             'rcParams': {
-                'font.size': 28,
+                'savefig.pad_inches': 0.04,
+                'font.size': 11,
                 'text.usetex': True,
-                'font.weight' : 'bold',
-                'text.latex.preamble': [
-                    r'\usepackage{xcolor}',
-                    r'\usepackage{nicefrac}',
-                    r'\usepackage{amsmath}',
-                    r'\usepackage{units}',
-                    r'\usepackage{sfmath} \boldmath']
+                'font.weight' : 'normal',
+                'text.latex.preamble': """\\usepackage{xcolor}
+\\usepackage{nicefrac}
+\\usepackage{amsmath}
+\\usepackage{units}
+\\usepackage{lmodern}
+""" # \\usepackage{sfmath}""" # \\boldmath"""
                 },
 
             'dpi': 300,
             'textbox': {}
             })
 
     def new_child(self, child = {}):
@@ -80,14 +108,15 @@
                 child[ax] = ChainMap({ 'field': child[ax] }, self[ax])
             else:
                 child[ax] = ChainMap(child.get(ax,{}), self[ax])
         return self.__class__(child, *self.maps)
 
 
 def Plot():
+    global PDATA, DATA, c, conf, logging, args, path, DIR, store
     """
     Basic usage: `PlotLHA --help`
 
     Requires a YAML config file that specifies at least the `'scatterplot'` dict with the list '`plots`'.
 
       * Automatically uses the `'latex'` attribute of specified LHA blocks for labels.
       * Fields for x/y/z axes can be specified by either `BLOCKNAME.values.LHAID` or the specified `'parameter'` attribute.
@@ -143,14 +172,16 @@
                     - y-axis: MASS.values.35
                       color: blue
                       label: '$m_{A}$'
     """
     parser = ArgumentParser(description='Plot ScanLHA results.')
     parser.add_argument("config", type=str,
             help="path to YAML file config.yml containing the plot (and optional scan) config.")
+    parser.add_argument("-i", "--interactive", action="store_true",
+            help="opens interactive plot environment with IPython: plot using the 'plot()' function")
     parser.add_argument("-v", "--verbose", action="store_true",
             help="increase output verbosity")
 
     args = parser.parse_args()
 
     logging.getLogger().setLevel(logging.INFO)
     if args.verbose:
@@ -171,20 +202,40 @@
     conf = conf.new_child(c['scatterplot'].get('conf',{}))
 
     if not os.path.isfile(conf['datafile']):
         logging.error('Data file {} does not exist.'.format(conf['datafile']))
         exit(1)
 
     store = HDFStore(conf['datafile'])
+
     path = 'results' # TODO
     DATA = store[path]
+
+    attrs = store.get_storer(path).attrs
+    if hasattr(attrs, 'config') and conf.get('conf_overwrite', False):
+        attrs.config['scatterplot'] = {}
+        c.append(attrs.config)
+
+    if(args.interactive):
+        embed()
+    else:
+        plot()
+
+    store.close()
+
+def plot():
+    global DATA, store
+    c = Config(args.config)
+    conf = PlotConf()
+    conf = conf.new_child(c['scatterplot'].get('conf',{}))
     attrs = store.get_storer(path).attrs
     if hasattr(attrs, 'config') and conf.get('conf_overwrite', False):
         attrs.config['scatterplot'] = {}
         c.append(attrs.config)
+
     if not DATA.empty and 'newfields' in conf:
         for field,expr in conf['newfields'].items():
             logging.debug("executing DATA[{}] = {}]".format(field, expr))
             DATA[field] = eval(expr)
         logging.debug("done.")
 
     pcount = 0
@@ -192,14 +243,20 @@
         lcount = 0
 
         pconf = conf.new_child(p)
 
         plt.cla()
         plt.clf()
         plt.rcParams.update(pconf['rcParams'])
+
+        if pconf['figsize']:
+            plt.figure(figsize=pconf['figsize'])
+        else:
+            plt.figure()
+
         if pconf['fontsize'] != conf['fontsize']:
             plt.rcParams.update({'font.size': pconf['fontsize']})
 
         if pconf['colorbar_only']:
             plt.figure(figsize=(8, 0.25))
             ax = plt.gca()
             norm = Normalize(vmin=pconf['z-axis']['vmin'], vmax=pconf['z-axis']['vmax'])
@@ -219,15 +276,15 @@
 
         if pconf['title']:
             plt.title(conf['title'])
 
         if 'plots' not in p:
             p['plots'] = [p]
 
-        for l in p['plots']:
+        for l in p['plots']: # noqa: E741
             lconf = pconf.new_child(l)
 
             label = lconf['label']
             label = label if label else None
             cmap = lconf['cmap']
             zorder = lconf.get('zorder', lcount)
             color = lconf.get('color', "C{}".format(lcount))
@@ -258,74 +315,119 @@
 
             if hasattr(c, 'parameters'):
                 x = c.parameters.get(x,{'lha': x})['lha']
                 y = c.parameters.get(y,{'lha': y})['lha']
                 z = c.parameters.get(z,{'lha': z})['lha']
 
             PDATA = DATA
+            for constr in lconf['constraints']:
+                PDATA = PDATA[eval(constr)]
+
             if(lconf['datafile'] and lconf['datafile'] != conf['datafile']):
                 conf['datafile'] = lconf['datafile'] # TODO
-                DATA = HDFStore(lconf['datafile'])['results']  # TODO
+                store.close()
+                del DATA, PDATA, store
+                store = HDFStore(lconf['datafile'])  # TODO
+                DATA = store['results']  # TODO
                 PDATA = DATA
+
                 if not PDATA.empty and 'newfields' in conf:
                     for field,expr in conf['newfields'].items():
                         logging.debug("executing PATA[{}] = {}]".format(field, expr))
                         PDATA[field] = eval(expr)
                     logging.debug("done.")
 
             for ax,field in {'x-axis':x, 'y-axis':y, 'z-axis':z}.items():
                 bounds = lconf[ax]['boundaries']
                 if len(bounds) == 2:
+                    logging.debug("applying boundaries [{},{}] on axis {}, field {}".format(bounds[0],bounds[1],ax,field))
                     PDATA = PDATA[(PDATA[field] >= bounds[0]) & (PDATA[field] <= bounds[1])]
 
-            for constr in lconf['constraints']:
-                PDATA = PDATA[eval(constr)]
-
             if lconf['x-axis']['lognorm']:
-                plt.xscale('log')
+                if type(lconf['x-axis']['lognorm']) == str:
+                    plt.xscale(lconf['x-axis']['lognorm'])
+                else:
+                    plt.xscale('log')
+
             if lconf['y-axis']['lognorm']:
-                plt.yscale('log')
+                if type(lconf['y-axis']['lognorm']) == str:
+                    plt.yscale(lconf['y-axis']['lognorm'])
+                else:
+                    plt.yscale('log')
 
             if z:
+                PDATA = PDATA.sort_values(by=z)
                 color = PDATA[z]
                 vmin = PDATA[z].min() if not lconf['z-axis']['vmin'] else lconf['z-axis']['vmin']
                 vmax = PDATA[z].max() if not lconf['z-axis']['vmax'] else lconf['z-axis']['vmax']
             else:
                 vmin = None
                 vmax = None
             znorm = LogNorm(vmin=vmin, vmax=vmax) if lconf['z-axis']['lognorm'] else None
 
-            cs = plt.scatter(PDATA[x], PDATA[y], zorder=zorder, label=label, cmap=cmap, c=color, vmin=vmin, vmax=vmax, norm=znorm, s=lconf['s'], alpha=lconf['alpha'])
+            if lconf['exec']:
+                exec(lconf['exec'])
+
+            if pconf.get('type', 'scatter') == 'scatter':
+                cs = plt.scatter(PDATA[x], PDATA[y], zorder=zorder, label=label, cmap=cmap, c=color, vmin=vmin, vmax=vmax, norm=znorm, s=lconf['s'], alpha=lconf['alpha'], marker=lconf.get('marker', None))
+            else:
+                PDATA = PDATA[[x,y]].dropna().sort_values(by=x)
+                cs = plt.plot(PDATA[x], PDATA[y], lconf.get('fmt', '.'), zorder=zorder, c=color, alpha=lconf['alpha'], label=label, **lconf.get('kwargs',{}))
+
+            plt.grid(b=True, which='major', color='#777777', linestyle='-', alpha=0.3, zorder=0)
+            plt.minorticks_on()
+            plt.grid(b=True, which='minor', color='#999999', linestyle='-', alpha=0.1, zorder=0)
 
             plt.margins(x=0.01,y=0.01)  # TODO
             if lconf['x-axis']['ticks']:
+                if type(lconf['x-axis']['ticks'][0]) is not list:
+                    lconf['x-axis']['ticks'] = [lconf['x-axis']['ticks'], ['${}$'.format(xt) for xt in lconf['x-axis']['ticks']]]
                 plt.xticks(lconf['x-axis']['ticks'][0],lconf['x-axis']['ticks'][1])
             if lconf['y-axis']['ticks']:
+                if type(lconf['y-axis']['ticks'][0]) is not list:
+                    lconf['y-axis']['ticks'] = [lconf['y-axis']['ticks'], ['${}$'.format(yt) for yt in lconf['y-axis']['ticks']]]
                 plt.yticks(lconf['y-axis']['ticks'][0],lconf['y-axis']['ticks'][1])
 
             if lconf['z-axis']['colorbar']:
-                cbar = plt.colorbar(cs, orientation=lconf['z-axis']['colorbar_orientation'])
+                cbar = plt.colorbar(cs, orientation=lconf['z-axis']['colorbar_orientation'], **lconf['z-axis'].get('kwargs',{}))
                 if zlabel:
                     cbar.set_label(zlabel)
                 if lconf['z-axis']['ticks']:
+                    if type(lconf['z-axis']['ticks'][0]) is not list:
+                        lconf['z-axis']['ticks'] = [lconf['z-axis']['ticks'], ['${}$'.format(zt) for zt in lconf['z-axis']['ticks']]]
                     cbar.set_ticks(lconf['z-axis']['ticks'])
+                for label in cbar.ax.yaxis.get_ticklabels():
+                    if lconf['z-axis']['colorbar_orientation'] == 'horizontal':
+                        label.set_ha('center')
+                    else:
+                        label.set_va('center')
 
             lcount += 1
 
-        if any([l.get('label', False) for l in p['plots']]):
-            plt.legend(**pconf['legend'])
-
         if pconf['textbox'] and 'text' in pconf['textbox']:
             bbox = pconf['textbox'].get('bbox', dict(boxstyle='round', facecolor='white', alpha=0.2))
             va = pconf['textbox'].get('va', 'top')
             ha = pconf['textbox'].get('ha', 'left')
             textsize = pconf['textbox'].get('fontsize', pconf['rcParams'].get('font.size',15))
             xtext = pconf['textbox'].get('x', 0.95)
             ytext = pconf['textbox'].get('y', 0.85)
             plt.gcf().text(xtext, ytext, pconf['textbox']['text'], fontsize=textsize ,va=va, ha=ha, bbox=bbox)
 
+        if pconf['tick_params']:
+            plt.tick_params(**pconf['tick_params'])
+
+        ax = plt.gca()
+        for label in ax.yaxis.get_ticklabels():
+            label.set_verticalalignment('center')
+        for label in ax.xaxis.get_ticklabels():
+            label.set_horizontalalignment('center')
+
+        for ann in p.get('annotiations',[]):
+            plt.annotate(ann['label'], ann['pos'], **ann.get('kwargs',{}))
+
+        if any([lbl.get('label', False) for lbl in p['plots']]):
+            plt.legend(**pconf['legend'])
+
         plotfile = DIR + p.get('filename', 'plot{}.png'.format(pcount))
         logging.info("Saving {}.".format(plotfile))
         plt.savefig(plotfile, bbox_inches="tight", dpi=pconf['dpi'])
         pcount += 1
-
-    store.close()
```

### Comparing `ScanLHA-0.3/ScanLHA/ScanLHA.py` & `ScanLHA-0.4/ScanLHA/ScanLHA.py`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/ScanLHA/__init__.py` & `ScanLHA-0.4/ScanLHA/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,9 +163,9 @@
  * ask me if you wish to be listed here
 
 """
 from .scan import Scan, RandomScan, FileScan
 from .config import Config
 from  .runner import RUNNERS
 from  .slha import genSLHA, parseSLHA
-__version__ = '0.3'
+__version__ = '0.4'
 __all__ = []
```

### Comparing `ScanLHA-0.3/ScanLHA/config.py` & `ScanLHA-0.4/ScanLHA/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -317,18 +317,18 @@
                     self.valid = False
                 if [block['block'],line['id']] in lines_seen:
                     logging.error('Parameter {} in block {} set twice! Taking the first occurence.'.format(line['id'], block['block']))
                     self.valid = False
                 if 'parameter' not in line:
                     line['parameter'] = '{}.{}'.format(block['block'],line['id'])
                 elif line['parameter'] in self.parameters.keys():
-                        para = line['parameter'] + '1'
-                        logging.error('Parameter {} set twice! Renaming to {}.'.format(line['parameter'], para))
-                        line['parameter'] = para
-                        self.valid = False
+                    para = line['parameter'] + '1'
+                    logging.error('Parameter {} set twice! Renaming to {}.'.format(line['parameter'], para))
+                    line['parameter'] = para
+                    self.valid = False
                 self.parameters[line['parameter']] = line
                 if 'value' in line and line.get('dependent', False) and type(line['value']) != str:
                     print(line.get('dependent', False))
                     logging.error("'value' with attribute 'dependent' must be string not {} ({}, {}).".format(type(line['value']), block['block'], line['id']))
                     self.valid = False
                 if 'value' in line and not line.get('dependent', False):
                     try:
@@ -343,8 +343,14 @@
                     logging.error("'scan' must be a nonemtpy list ({}, {}).".format(block['block'], line['id']))
                     self.valid = False
                 if 'latex' not in line:
                     line['latex'] = line['parameter']
                 if 'lha' not in line:
                     line['lha'] = '{}.values.{}'.format(block['block'],line['id'])
                 lines_seen.append([block['block'], line['id']])
+
+        # check for other stuff
+        self['runner']['writeevery'] = self['runner'].get('writeevery', 0)
+        if not isinstance(self['runner']['writeevery'], int):
+            logging.error("runner['writeevery'] must be integer")
+            self.valid = False
         return self.valid
```

### Comparing `ScanLHA-0.3/ScanLHA/configs/SPheno.yml` & `ScanLHA-0.4/ScanLHA/configs/SPheno.yml`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/ScanLHA/runner.py` & `ScanLHA-0.4/ScanLHA/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from subprocess import Popen, STDOUT, PIPE, DEVNULL, TimeoutExpired
 from .slha import parseSLHA
 from random import randrange,randint
 import os
 from sys import exit
 from math import * # noqa: F403 F401
 from shutil import copy2,copytree, rmtree
-from tempfile import mkdtemp
-from pandas.io.json import json_normalize
+from tempfile import mkdtemp, gettempdir
+from pandas import json_normalize
 
 __all__ = ['RUNNERS', 'BaseRunner', 'SLHARunner', 'MicrOmegas']
 
 RUNNERS = {}
 """
 Contains all available runner classes.
 
@@ -69,27 +69,30 @@
         For a correct behaviour use `super().__init__(conf)` in the `__init__` of your child runner.
         """
         self.config = conf
         self.rundir = os.getcwd()
         self.binaries = []
         self.tmp = False
         self.initialized = False
+        self.id = randint(10000,99999)
 
     def makedirs(self, tocopy=[]):
         """
           * Create temporary directories (default: `/dev/shm/run<runnerid>`).
 
           * Copy all binaries listed in `self.config['binaries']` to the temporary directory
         """
         if 'tmpfs' not in self.config:
             if os.path.exists('/dev/shm/'):
                 self.config['tmpfs'] = '/dev/shm/'
             else:
                 self.config['tmpfs'] = mkdtemp()
-        self.rundir = os.path.join(self.config['tmpfs'], 'run%d' % randint(10000,99999))
+        if self.config['tmpfs'] == '$TMP':
+            self.config['tmpfs'] = gettempdir()
+        self.rundir = os.path.join(self.config['tmpfs'], 'run%d' % self.id)
         if not os.path.exists(self.rundir):
             logging.debug('Creating temporary directory {}.'.format(self.rundir))
             os.makedirs(self.rundir)
         tocopy = tocopy if type(tocopy) == list else [tocopy]
         if 'binary' in self.config:
             self.binaries = [os.path.join(self.rundir, os.path.basename(self.config['binary'])), '{input_file}', '{output_file}']
             tocopy.append(self.config['binary'])
@@ -240,15 +243,15 @@
             return {}
         return slha
 
     def execute(self, params):
         """
         * Prepare all files for the run with the parameters `params` (dict).
         * iterate over the binaries in `self.binaries`
-          * check for fulfilled constraints
+          * check for fulfilled constraints. If runner['all_constraints'] is set to True (default: False), the binary-chain is stopped on the first failed constraint.
 
         Example for `self.binaries` that passes results trough the different runs:
 
             config['runner']['binaries'] = [
                 ['./SPheno', '{input_file}', '{output_file}'],
                 ['./HiggsBounds', '{output_file}']
             ]
@@ -265,15 +268,15 @@
                 'input_file': fin,
                 'output_file': fout,
                 'log_file': flog
                 }
 
         slha = True
         for binary in self.binaries:
-            if not slha:
+            if not slha and self.config.get('all_constraints', False):
                 continue
             if type(binary) == list:
                 # insert file names into the executable command
                 binary = [ b.format(**slha_base) for b in binary ]
             else:
                 binary = [binary]
             logging.debug("executing {}".format(' '.join(binary)))
```

### Comparing `ScanLHA-0.3/ScanLHA/scan.py` & `ScanLHA-0.4/ScanLHA/scan.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,26 @@
 from concurrent.futures import as_completed
 from tqdm import tqdm
 from math import * # noqa: F403 F401
 from itertools import product
 from pandas import HDFStore, concat, DataFrame
 from .slha import genSLHA
 from .runner import RUNNERS
-from numpy.random import seed, uniform, normal, exponential, poisson
-from time import time
+# import numpy.random import uniform, normal, exponential, poisson, seed
+import numpy.random as random
 from glob import glob
-import importlib
 
 if os.path.isdir('runner_plugins'):
-    # dynamically import custom runners from the directory "./runner_plugins"
-    for runner in glob('runner_plugins/*.py'):
-        importlib.import_module(runner.replace('/', '.').replace('.py', ''))
+    for file_path in glob('runner_plugins/*.py'):
+        module_name = file_path.replace('runner_plugins/', '').replace('.py', '')
+        print('importing: ' + module_name + ' from runner_plugins/')
+        try:
+            exec('from {} import *'.format(module_name))
+        except ImportError:
+            print("could not import {} do you append {} to $PYTHONPATH?".format(module_name, file_path))
 
 def substitute(param_dict):
     """ recusively apply format_map onto keys of <param_dict> using <param_dict> """
     subst = { p : str(v).format_map(param_dict) for p,v in param_dict.items() }
     if param_dict == subst:
         return { p : eval(v) for p,v in subst.items() }
     else:
@@ -181,17 +184,15 @@
     def __init__(self, c, seed=None):
         self.config = c
         self.numparas = eval(str(c['runner']['numparas']))
         self.config['runner']['template'] = genSLHA(c['blocks'])
         self.getblocks = self.config.get('getblocks', [])
         self.runner = RUNNERS[self.config['runner'].get('type','SLHARunner')]
         self.parallel = os.cpu_count()
-        self.seed = round(time()) if not seed else seed
-        self.distributions = {'uniform': uniform, 'exponential': exponential, 'normal': normal, 'poisson': poisson}
-        self.randoms = { p : { 'args': [eval(str(k)) for k in v['random']], 'dist': self.distributions[v.get('distribution', 'uniform')], 'norm': v.get('norm', 1)} for p,v in c.parameters.items() if 'random' in v }
+        #  self.seed = seed
         self.dependent = { p : v['value'] for p,v in c.parameters.items() if v.get('dependent',False) and 'value' in v }
 
     def generate(self):
         """
         Generate random numbers for specified SLHA blocks.
 
         Substitute the numbers in dependend blocks, if necessary.
@@ -207,23 +208,29 @@
         Returns a `pandas.DataFrame`.
         """
         numresults = 0
         runner = self.runner(self.config['runner'])
         if not runner.initialized:
             logging.error('Could not initialize runner.')
             return DataFrame()
+
         results = []
-        seed(self.seed + pos)
+
+        self.distributions = {'uniform': random.RandomState().uniform, 'exponential': random.RandomState().exponential, 'normal': random.RandomState().normal, 'poisson': random.RandomState().poisson}
+        self.randoms = { p : { 'args': [eval(str(k)) for k in v['random']], 'dist': self.distributions[v.get('distribution', 'uniform')], 'norm': v.get('norm', 1)} for p,v in self.config.parameters.items() if 'random' in v }
+
         with tqdm(total=numparas, unit='point', position=pos) as bar:
             while numresults < numparas:
                 result = runner.run(self.generate())
                 if not result.isnull().values.all():
                     results.append(result)
                     numresults += 1
                     bar.update(1)
+                if runner.config['writeevery'] > 0 and numresults % runner.config['writeevery'] == 0:
+                    pass
         return concat(results, ignore_index=True)
 
     def submit(self,num_workers=None):
         """
         Start a scan and distribute it on `num_workers` threads.
 
         If `num_workers` is omitted, the value of `os.cpu_count()` is used.
@@ -253,15 +260,15 @@
         print('Saving to {} ({})'.format(filename,path))
         if path == 'config':
             logging.error('Cant use "config" as path, using "config2" instead.')
             path = "config2"
         store = HDFStore(filename)
         store[path] = self.results
         store.get_storer(path).attrs.config = self.config
-        store.get_storer(path).attrs.seed = self.seed
+        #  store.get_storer(path).attrs.seed = self.seed
         store.get_storer(path).attrs.parallel = self.parallel
         store.close()
 
 class FileScan(Scan):
     """
     Performs a scan based on input file(s) from a previous scan.
```

### Comparing `ScanLHA-0.3/ScanLHA/slha.py` & `ScanLHA-0.4/ScanLHA/slha.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,15 +48,30 @@
 
     `slhafile` : path tp file
 
     `blocks`   : list of BLOCKs (strings) to read, if empty all blocks are read
 
     Uses [pylha](https://github.com/DavidMStraub/pylha pylha) but gives a more meaningful output
     the result is stored in a nested dictionary.
+
+    Converts (i.e. reverses) non-standard SLHA entrys (such as HiggsBounds).
     """
+    reversed_blocks = [
+            'HiggsBoundsInputHiggsCouplingsBosons',
+            'HiggsBoundsInputHiggsCouplingsFermions',
+            'HiggsCouplingsFermions',
+            'HiggsCouplingsBosons'
+            ]
+
+    # blocks which have more than one numerical value are joined into a "|"-separated string
+    list_blocks = {
+            'HiggsCouplingsFermions': 2,
+            'HiggsBoundsInputHiggsCouplingsFermions': 2,
+            }
+
     try:
         with open(slhafile,'r') as f:
             slha = pylha.load(f)
     except FileNotFoundError:
         logging.error('File %s not found.' % slhafile)
         return {}
     except:
@@ -64,22 +79,22 @@
         return {}
     try:
         slha_blocks = slha['BLOCK']
     except KeyError:
         slha_blocks = {}
     if blocks:
         slha_blocks = { b : v for b,v in slha_blocks.items() if b in blocks }
-    try: # TODO convert into valid slha instead of dropping
-        slha_blocks.pop('HiggsBoundsInputHiggsCouplingsBosons')
-        slha_blocks.pop('HiggsBoundsInputHiggsCouplingsFermions')
-    except KeyError:
-        pass
     for b,v in slha_blocks.items():
         try:
+            if b in list_blocks:
+                v['values'] = [ ['|'.join(str(y) for y in x[:list_blocks[b]])] + x[list_blocks[b]:] for x in v['values']]
+            if b in reversed_blocks:
+                [x.reverse() for x in v['values']]
             v['values'] = mergedicts([list2dict(l) for l in v['values']],{})
+
             v['info'] = ''.join(str(i) for i in v['info'])
         except:
             pass
 
     if 'DECAY' not in slha:
         return slha_blocks
```

### Comparing `ScanLHA-0.3/docs/EditLHA.m.html` & `ScanLHA-0.4/docs/EditLHA.m.html`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/docs/MergeLHA.m.html` & `ScanLHA-0.4/docs/MergeLHA.m.html`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/docs/PlotLHA.m.html` & `ScanLHA-0.4/docs/PlotLHA.m.html`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/docs/ScanLHA.m.html` & `ScanLHA-0.4/docs/ScanLHA.m.html`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/docs/config.m.html` & `ScanLHA-0.4/docs/config.m.html`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/docs/index.html` & `ScanLHA-0.4/docs/index.html`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/docs/runner.m.html` & `ScanLHA-0.4/docs/runner.m.html`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/docs/scan.m.html` & `ScanLHA-0.4/docs/scan.m.html`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/docs/slha.m.html` & `ScanLHA-0.4/docs/slha.m.html`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/pyproject.toml` & `ScanLHA-0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ScanLHA-0.3/setup.py` & `ScanLHA-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 entry_points = \
 {'console_scripts': ['EditLHA = ScanLHA.EditLHA:Edit',
                      'MergeLHA = ScanLHA.MergeLHA:Merge',
                      'PlotLHA = ScanLHA.PlotLHA:Plot',
                      'ScanLHA = ScanLHA.ScanLHA:ScanLHA']}
 
 setup(name='ScanLHA',
-      version='0.3',
+      version='0.4',
       description='Perform parameter scans with HEP tools that use (not only) (S)LHA in- and output.',
       author='Martin Gabelmann',
       author_email='martin@gabelmann.biz',
       url='https://github.com/martingabelmann/ScanLHA',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

