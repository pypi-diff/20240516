# Comparing `tmp/ztffields-0.5.1.tar.gz` & `tmp/ztffields-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztffields-0.5.1.tar", last modified: Mon Apr  8 13:14:47 2024, max compression
+gzip compressed data, was "ztffields-0.6.0.tar", last modified: Thu May 16 12:49:46 2024, max compression
```

## Comparing `ztffields-0.5.1.tar` & `ztffields-0.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-04-08 13:14:47.930210 ztffields-0.5.1/
--rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-12-09 18:53:25.000000 ztffields-0.5.1/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)     1027 2024-04-08 13:14:47.930153 ztffields-0.5.1/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      432 2022-12-13 14:52:32.000000 ztffields-0.5.1/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)     1128 2024-04-08 13:14:47.930519 ztffields-0.5.1/setup.cfg
--rw-r--r--   0 rigault   (2358) staff       (20)       37 2022-12-11 14:43:45.000000 ztffields-0.5.1/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-04-08 13:14:47.928472 ztffields-0.5.1/ztffields/
--rw-r--r--   0 rigault   (2358) staff       (20)       95 2024-03-26 14:18:31.000000 ztffields-0.5.1/ztffields/__init__.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-04-08 13:14:47.929545 ztffields-0.5.1/ztffields/data/
--rwxr-xr-x   0 rigault   (2358) staff       (20)     1419 2022-12-11 14:44:47.000000 ztffields-0.5.1/ztffields/data/ztf_ccd_layout.tbl
--rwxr-xr-x   0 rigault   (2358) staff       (20)     6230 2022-12-11 14:44:47.000000 ztffields-0.5.1/ztffields/data/ztf_ccd_quad_layout.tbl
--rwxr-xr-x   0 rigault   (2358) staff       (20)   123430 2022-12-11 14:44:47.000000 ztffields-0.5.1/ztffields/data/ztf_fields.txt
--rw-r--r--   0 rigault   (2358) staff       (20)    20296 2023-06-29 08:00:51.000000 ztffields-0.5.1/ztffields/fields.py
--rw-r--r--   0 rigault   (2358) staff       (20)      175 2022-12-11 14:47:26.000000 ztffields-0.5.1/ztffields/io.py
--rw-r--r--   0 rigault   (2358) staff       (20)    28985 2023-09-04 19:35:33.000000 ztffields-0.5.1/ztffields/plotting.py
--rw-r--r--   0 rigault   (2358) staff       (20)    15102 2024-03-26 14:21:58.000000 ztffields-0.5.1/ztffields/projection.py
--rw-r--r--   0 rigault   (2358) staff       (20)     2317 2024-02-29 14:30:53.000000 ztffields-0.5.1/ztffields/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-04-08 13:14:47.929769 ztffields-0.5.1/ztffields.egg-info/
--rw-r--r--   0 rigault   (2358) staff       (20)     1027 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/PKG-INFO
--rw-r--r--   0 rigault   (2358) staff       (20)      458 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/SOURCES.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/dependency_links.txt
--rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-11 14:44:59.000000 ztffields-0.5.1/ztffields.egg-info/not-zip-safe
--rw-r--r--   0 rigault   (2358) staff       (20)      132 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/requires.txt
--rw-r--r--   0 rigault   (2358) staff       (20)       10 2024-04-08 13:14:47.000000 ztffields-0.5.1/ztffields.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-05-16 12:49:46.231408 ztffields-0.6.0/
+-rw-r--r--   0 rigault   (2358) staff       (20)    11357 2022-12-09 18:53:25.000000 ztffields-0.6.0/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)     1027 2024-05-16 12:49:46.231341 ztffields-0.6.0/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      432 2022-12-13 14:52:32.000000 ztffields-0.6.0/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)     1128 2024-05-16 12:49:46.231716 ztffields-0.6.0/setup.cfg
+-rw-r--r--   0 rigault   (2358) staff       (20)       37 2022-12-11 14:43:45.000000 ztffields-0.6.0/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-05-16 12:49:46.229289 ztffields-0.6.0/ztffields/
+-rw-r--r--   0 rigault   (2358) staff       (20)       95 2024-05-16 12:15:53.000000 ztffields-0.6.0/ztffields/__init__.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-05-16 12:49:46.230599 ztffields-0.6.0/ztffields/data/
+-rwxr-xr-x   0 rigault   (2358) staff       (20)     1419 2022-12-11 14:44:47.000000 ztffields-0.6.0/ztffields/data/ztf_ccd_layout.tbl
+-rwxr-xr-x   0 rigault   (2358) staff       (20)     6230 2022-12-11 14:44:47.000000 ztffields-0.6.0/ztffields/data/ztf_ccd_quad_layout.tbl
+-rwxr-xr-x   0 rigault   (2358) staff       (20)   123430 2022-12-11 14:44:47.000000 ztffields-0.6.0/ztffields/data/ztf_fields.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)    20296 2023-06-29 08:00:51.000000 ztffields-0.6.0/ztffields/fields.py
+-rw-r--r--   0 rigault   (2358) staff       (20)      175 2022-12-11 14:47:26.000000 ztffields-0.6.0/ztffields/io.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    30517 2024-05-16 12:14:54.000000 ztffields-0.6.0/ztffields/plotting.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    15102 2024-03-26 14:21:58.000000 ztffields-0.6.0/ztffields/projection.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     2317 2024-02-29 14:30:53.000000 ztffields-0.6.0/ztffields/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2024-05-16 12:49:46.230890 ztffields-0.6.0/ztffields.egg-info/
+-rw-r--r--   0 rigault   (2358) staff       (20)     1027 2024-05-16 12:49:46.000000 ztffields-0.6.0/ztffields.egg-info/PKG-INFO
+-rw-r--r--   0 rigault   (2358) staff       (20)      458 2024-05-16 12:49:46.000000 ztffields-0.6.0/ztffields.egg-info/SOURCES.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2024-05-16 12:49:46.000000 ztffields-0.6.0/ztffields.egg-info/dependency_links.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)        1 2022-12-11 14:44:59.000000 ztffields-0.6.0/ztffields.egg-info/not-zip-safe
+-rw-r--r--   0 rigault   (2358) staff       (20)      132 2024-05-16 12:49:46.000000 ztffields-0.6.0/ztffields.egg-info/requires.txt
+-rw-r--r--   0 rigault   (2358) staff       (20)       10 2024-05-16 12:49:46.000000 ztffields-0.6.0/ztffields.egg-info/top_level.txt
```

### Comparing `ztffields-0.5.1/LICENSE` & `ztffields-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.1/PKG-INFO` & `ztffields-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffields
-Version: 0.5.1
+Version: 0.6.0
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/ztffields
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ztffields-0.5.1/setup.cfg` & `ztffields-0.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.1/ztffields/data/ztf_ccd_layout.tbl` & `ztffields-0.6.0/ztffields/data/ztf_ccd_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.1/ztffields/data/ztf_ccd_quad_layout.tbl` & `ztffields-0.6.0/ztffields/data/ztf_ccd_quad_layout.tbl`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.1/ztffields/data/ztf_fields.txt` & `ztffields-0.6.0/ztffields/data/ztf_fields.txt`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.1/ztffields/fields.py` & `ztffields-0.6.0/ztffields/fields.py`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.1/ztffields/plotting.py` & `ztffields-0.6.0/ztffields/plotting.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,14 @@
 
 
 # -------------- #
 #                #
 #  FootPring     #
 #                #
 # -------------- #
-
 def show_ztf_footprint(ax=None, ccdid=None, fieldid=None,
                            ccd_color="k", focalplane_color="0.7"):
     """ displays the ZTF footprint
 
     Parameters
     ----------
     ccdid: int, list, None
@@ -139,14 +138,15 @@
             ax.text(*centroid_, f"{rcid}", va="center", ha="center", 
                     color="w", zorder=4, fontsize="x-small")
 
 
     ax.set_xlim(-5+ra,5+ra)
     ax.set_ylim(-5+dec,5+dec)
     return fig
+
 # -------------- #
 #                #
 #  FieldFigure   #
 #                #
 # -------------- #
 def skyplot_fields(fieldid, figsize=(7,4), level="focalplane",
                        system="icrs", projection=None, **kwargs):
@@ -189,34 +189,41 @@
 
     Returns
     -------
     `matplotlib.figure`
     
     """
     return FieldFigure.skyplot_fields(fieldid, figsize=figsize, level=level,
-                                          system=system, projection=projection, **kwargs)
+                                      system=system, projection=projection,
+                                      **kwargs)
+
 
 class FieldFigure( object ):
 
     def __init__(self, geodf, figsize=(7,4), system="icrs", origin=180, **kwargs):
         """ 
         
         Parameters
         ----------
 
+        geodf: geopandas.DataFrame
+        
+
         figsize : (float, float)
             Width, height in inches.
 
         level: str
             level of description of the camera.
             - focalplane: 1 polygon for the whole footprint
             - ccd: 1 polygon per CCD (16 per footprint then)
             - quadrant: 1 polygon per quadrant (64 per per footprint then)
             ccd and quadrant level will account for gaps between the CCDs.
 
+        system
+
         Returns
         -------
         None
         """
         self._geodf = geodf
         self.set_system(system, origin=origin)
         
@@ -228,73 +235,105 @@
     @classmethod
     def from_level(cls, level, figsize=(7,4), system="icrs", origin=180, **kwargs):
         """ """
         geodf = Fields.get_field_geometry(level=level, **kwargs)
         return cls(geodf=geodf, figsize=figsize, system=system, origin=origin)
 
 
+    @staticmethod
+    def _parse_system(system, default_frame="astro"):
+        """ clean the input system for self consistancy 
+
+        Parameters
+        ----------
+        system: str
+            coordinates system: 
+            - icrs (ra, dec) | shortcut for astro icrs
+            - astro icrs (ra, dec) east is right
+            - geo icrs (ra, dec) west is right
+            - galactic (l, b)
+            
+            Note: for simplicity radec<->ircs or lb<->galactic
+            such that 'geo radec' is equivalent to 'geo icrs'
+            
+        Returns
+        -------
+        system: str
+        """
+        system = system.replace("radec", "icrs").replace("lb", "galactic")
+        *frame, sys = system.split(" ")
+        if len(frame) == 0:
+            frame = default_frame
+        elif len(frame) == 1 and frame[0] in ["geo", "astro"]:
+            frame = frame[0]
+        else:
+            raise ValueError(f"cannot parse input frame, astro or geo expected, got: {frame}")
+
+        if sys == "galactic":
+            return sys
+        
+        return f"{frame} {sys}"
+        
+        
     def set_system(self, system="icrs", origin=180):
         """ set the plotting coordinate system.
 
         Parameters
         ----------
         system: str
             coordinates system: 
-            - icrs (ra, dec)
+            - icrs (ra, dec) | shortcut for astro icrs
+            - astro icrs (ra, dec) east is right
+            - geo icrs (ra, dec) west is right
             - galactic (l, b)
 
         origin: float
             where the center is (left is origin from 0)
             180 means that coordinates goes from -180->180
             
         Returns
         -------
         None
         """
-        if hasattr(self,"_is_cartopy") and self._is_cartopy:
-            is_cartopy = True
-        else:
-            is_cartopy = False
-
+        system = self._parse_system(system)
+        
         xy_icrs = np.stack(self._geodf["geometry"].apply(lambda x: ((np.asarray(x.exterior.xy)).T) ).values)
-        if system == "icrs":
+        if "astro" in system:
+            # invert ra direction
+            xy_icrs[:,:,0] *=-1
+
+        if "icrs" in system:
             xy = xy_icrs
+            
         else:
             from astropy import coordinates, units            
             shape_ = xy_icrs.shape
             new_shape = np.prod(shape_[:-1]), shape_[-1]
             icrs = coordinates.ICRS( *xy_icrs.reshape(new_shape).T*units.degree )
             if system == "galactic":
                 # Create a ICRS object and convert it to galactic coords
                 gal = icrs.transform_to(coordinates.Galactic())
                 # avoids edge effect.
                 xy = np.asarray([gal.l.value, gal.b.value]).T.reshape(shape_)
                 
             else:
                 raise NotImplementedError(f"'{system}' has not been implemented")
 
-        # identify and correct edge effects
-        flag_egde = np.any(np.diff(xy, axis=1)>300, axis=1)[:,0]
-        xy[flag_egde] = ((xy[flag_egde] + origin)%360 - origin)
-
-        if not is_cartopy:
-            xy -= [origin,0] # set the origin
-            xy *= np.pi/180 # in radian
-            
+        # identify and correct edge effects            
         self._geodf["xy"] = list(xy)
         self._system = system
         self._origin = origin
         
     # =============== #
     #   Class method  #
     # =============== #    
     @classmethod
     def skyplot_fields(cls, fieldid, figsize=(7,4), level="focalplane",
-                           system="icrs", projection=None,
-                           add_mw=True, mwcolor = "k", mwb=5,
+                           system="icrs", origin=180, projection=None,
+                           add_mw=True, mwcolor = "0.7", mwb=5,
                            colorbar="hist", facealpha=0.9, edgecolor="None",
                            bins=None, **kwargs):
         """ plot fields on a 2d sky projection.
 
         This uses self.plot_sky()
 
         Parameters
@@ -356,29 +395,30 @@
             sequencing of the colormap. 'lut' in matplotlib's get_cmap()
 
         **kwargs goes to plot_sky | e.g. cmap, vmin, vmax ...
 
         Returns
         -------
         figure
+
         """
         # Create figure and the plotting system        
-        figfield = cls.from_level(level=level,figsize=figsize,system=system)
+        figfield = cls.from_level(level=level, figsize=figsize, system=system, origin=origin)
         
         # Create the axes
         ax = figfield.add_axes(projection=projection)
         
         # Draw the fields as matplolib's polygon
         _ = figfield.plot_sky(ax=ax, fieldid=fieldid,
                               facealpha=facealpha, edgecolor=edgecolor,
                               colorbar=colorbar, bins=bins, **kwargs)
         
         # Add the Milky way if wanted.
         if add_mw:
-            _ = figfield.add_milkyway(color=mwcolor, b=mwb)
+            _ = figfield.add_milkyway(ax=ax, color=mwcolor, b=mwb)
 
         return figfield.figure
     
     # =============== #
     #   add other     #
     # =============== #
     def add_axes(self, rect=[0.15,0.22,0.75,0.75],
@@ -435,15 +475,15 @@
         self._is_cartopy = "cartopy" in str( type(projection) )
         
         ax = self.figure.add_axes(rect, projection=projection, **kwargs)
 
         if self._is_cartopy:
             self._projection = projection
             ax.set_global()
-            self.set_system(self._system)
+#            self.set_system(self._system)
             
         return ax
     
     # =============== #
     #     Main        #
     # =============== #        
     def plot_sky(self, fieldid=None, ax=None, 
@@ -556,15 +596,15 @@
             self._plotting["bins"] = None
             prop["facecolor"] = to_rgba("C0",0.1)
             prop["edgecolor"] = to_rgba("k",0.7)
             
         #
         # Calling plotter
         #
-        _ = self._show_fieldverts(fieldverts, ax=self.ax, **{**prop,**kwargs})
+        _ = self._show_fieldverts(fieldverts, ax=ax, **{**prop,**kwargs})
         if colorbar is not None:
             if type(colorbar) is str and "hist" in colorbar:
                 cbar,_ = self.add_histcolorbar()
             else:
                 cbar = self.add_colorbar()
             if label is not None:
                 cbar.set_label(label, fontsize="large")
@@ -691,15 +731,15 @@
                            width=hbins["width"], color=hcolors,
                            alpha=histalpha)
         histax.set_ylim(bottom=0)
         histax.set_xlim(vmin, vmax)
         histax.axis("off")
         return cbar, _
         
-    def add_milkyway(self, b=5, nbins=300, l_start=-241, l_stop=116, **kwargs):
+    def add_milkyway(self, b=5, nbins=400, l_start=0, l_stop=360, ax=None, zorder=2, **kwargs):
         """ add the milky way location on the main axes' figure (self.ax)
         
         Parameters
         ----------
         b: int
             width (in degree) of the band around b=0
             
@@ -712,74 +752,99 @@
         **kwargs goes to ax.plot (if b is None) or to ax.fill_between (otherwise)
         
         Returns
         -------
         output of ax.plot or ax.fill_between
         """
         from astropy import coordinates, units
+        if ax is None:
+            ax = self.ax
+
         
         prop_line = dict(ls="-", color="0.7", alpha=0.5)
-        prop_band = dict(facecolor="0.7", alpha=0.2)
+        prop_band = dict(facecolor="0.7", alpha=1)
+        kwargs["zorder"] = zorder # because explicit input
 
-        # Cartopy
+        if b is None or b==0:
+                b = 1
         
+        if "icrs" in self.system:
+            long_, lat_ = np.linspace(l_start, l_stop,nbins)*units.deg, np.zeros(nbins)*units.deg
+            gal = coordinates.Galactic( long_, lat_ ).transform_to(coordinates.ICRS())
+            ra, dec = gal.ra.value, gal.dec.value
+            if "astro" in self.system:
+                ra *=-1
+            # make sure nothign breaks
+
+        ra, dec = self._parse_radec_for_plot(ra, dec, sort=True)        
+        #              #
+        # Cartopy      #
+        #              #
+
         if self._is_cartopy:
                 
             from shapely.geometry import LineString
             import cartopy.crs as ccrs
-            if b is None or b==0:
-                b = 1
-
-            long_, lat_ = np.linspace(l_start,l_stop,nbins)*units.deg, np.zeros(nbins)*units.deg
-            if self.system == "icrs":
-                gal = coordinates.Galactic( long_, lat_ ).transform_to(coordinates.ICRS)
-                ggal = LineString( zip(gal.ra.value, gal.dec.value) ).buffer(b)
-            elif self.system == "galactic":
+            
+            if "icrs" in self.system:
+                ggal = LineString( zip(ra, dec) ).buffer(b)
+                
+            elif self.system == "galactic":                
                 ggal = LineString( zip(long_.value, lat_.value) ).buffer(b)
+                
             else:
                 raise NotImplementedError("Milky way plotting has not been implemented for the current system '{self.system}'")
-            
-            return self.ax.add_geometries([ggal], ccrs.PlateCarree(central_longitude=self._origin),
-                                  **{**prop_band, **kwargs})
-            
-
 
-        # Matplotlib
-        
+            return ax.add_geometries(ggal,
+                                     ccrs.PlateCarree(self._origin),
+                                     **{**prop_band, **kwargs}
+                                     )
+            
+        #              #
+        # Matplotlib   #
+        #              #
         # l, b
-        if self.system == "galactic":
+        if "galactic" in self.system:
             if b is None:
-                _ = self.ax.axhline(0, **{**prop_line, **kwargs})
+                _ = ax.axhline(0, **{**prop_line, **kwargs})
             else:
-                _ = self.ax.axhspan(-b*np.pi/180, b*np.pi/180, **{**prop_band,**kwargs})
+                _ = ax.axhspan(-b*np.pi/180, b*np.pi/180, **{**prop_band,**kwargs})
+                
         # RA Dec
-        elif self.system == "icrs":
-            
-            if b is None:
-                gal = coordinates.Galactic( np.linspace(l_start,l_stop,nbins)*units.deg, np.zeros(nbins)*units.deg
-                                                ).transform_to(coordinates.ICRS)
-
-                _ = self.ax.plot(*self._radec_to_plot(gal.ra, gal.dec), **{**prop_line, **kwargs})
-            
-            else:
-                gal_dw = coordinates.Galactic(np.linspace(l_start,l_stop,nbins)*units.deg,
-                                                  +b*np.ones(nbins)*units.deg
-                                                  ).transform_to(coordinates.ICRS())
-                gal_up = coordinates.Galactic(np.linspace(l_start,l_stop,nbins)*units.deg,
-                                                  -b*np.ones(nbins)*units.deg
-                                                  ).transform_to(coordinates.ICRS())
-                ra_dw,dec_dw = self._radec_to_plot(gal_dw.ra, gal_dw.dec)
-                ra_up,dec_up = self._radec_to_plot(gal_up.ra, gal_up.dec)
-
-                _ = self.ax.fill_between(ra_dw, dec_dw, dec_up, **{**prop_band, **kwargs})
+        elif "icrs" in self.system:
+            # matplotlib works in radian
+            _ = ax.fill_between(ra,
+                                dec + b*np.pi/180,
+                                dec - b*np.pi/180,
+                                **{**prop_band, **kwargs})
+                
         else:
             raise NotImplementedError("Milky way plotting has not been implemented for the current system '{self.system}'")
         
         return _
 
+    def _parse_radec_for_plot(self, ra, dec, sort=False):
+        """ """
+        if self._is_cartopy:
+            pass
+        else:
+            ra = ra+self._origin # copy
+            ra = (ra + 180)%360 - 180 # -180->+180
+            # copy
+            ra = ra * np.pi/180
+            dec = dec * np.pi/180
+
+        if sort:
+            argsort_ra = np.argsort(ra)
+            ra = ra[argsort_ra]
+            dec = dec[argsort_ra]
+
+        return ra, dec
+        
+    
     # =============== #
     #   Internal      #
     # =============== #
     def get_current_colordata(self):
         """ """
         cdata = self._plotting.get("cdata")
         if cdata is None:
@@ -788,35 +853,36 @@
         vscale = vmax-vmin
         return  cdata*vscale + vmin
         
     def reset(self):
         """ """
         self._plotting = {}
     
-    def _show_fieldverts(self, fieldverts, ax, **kwargs):
+    def _show_fieldverts(self, fieldverts, ax, zorder=4, **kwargs):
         """ """
+        kwargs["zorder"] = zorder # because explicit input
+        
         from matplotlib.patches import Polygon
         if self._is_cartopy:
             import cartopy.crs as ccrs
-            kwargs["transform"] = ccrs.PlateCarree(central_longitude=self._origin)
+            kwargs["transform"] = ccrs.PlateCarree(self._origin)
+
+        if not self._is_cartopy:
+            import warnings
+            warnings.warn("you are not using cartopy projection, issues may appear on the edge")
+            fieldverts = fieldverts.copy()
+            xy = np.stack(fieldverts["xy"].values)
+            xy[:,:, 0] += self._origin
+            xy[:,:, 0] = (xy[:,:, 0] + 180)%360 - 180 # -180->+180
+            xy *= np.pi/180
+            fieldverts["xy"] = list(xy) # feed back in
             
-        patches = [Polygon(**v_.to_dict(), **kwargs) for i_, v_ in fieldverts.iterrows()]
-        return [self.ax.add_patch(patch_) for patch_ in patches]
-        
-    def _radec_to_plot(self, ra, dec):
-        """ """
-        if self._is_cartopy:
-            coef = 1
-            origin = 0
-        else:
-            coef = np.pi/180
-            origin = self._origin
+        patches = [Polygon(**fieldvert_.to_dict(), **kwargs) for i, fieldvert_ in fieldverts.iterrows()]
+        return [ax.add_patch(patch_) for patch_ in patches]
             
-        return np.asarray([(np.asarray(ra) - origin)* coef, np.asarray(dec)* coef]) 
-    
 
     def _build_histrogram(self, data, bins=None, **kwargs):
         """ """
         intensity, binegdes = np.histogram(data, range=self._plotting["vrange"], bins=bins,  **kwargs)
         bins = {"edge":binegdes,
                 "centroid":np.mean([binegdes[1:],binegdes[:-1]], axis=0),
                 "width":binegdes[1:]-binegdes[:-1],
```

### Comparing `ztffields-0.5.1/ztffields/projection.py` & `ztffields-0.6.0/ztffields/projection.py`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.1/ztffields/utils.py` & `ztffields-0.6.0/ztffields/utils.py`

 * *Files identical despite different names*

### Comparing `ztffields-0.5.1/ztffields.egg-info/PKG-INFO` & `ztffields-0.6.0/ztffields.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ztffields
-Version: 0.5.1
+Version: 0.6.0
 Summary: Access and Interact with ZTF Fields
 Home-page: https://github.com/MickaelRigault/ztffields
 Author: Mickael Rigault
 Author-email: m.rigault@ipnl.in2p3.fr
 License: Apache Software License
 Keywords: astronomy,astrophysics
 Classifier: Development Status :: 2 - Pre-Alpha
```

