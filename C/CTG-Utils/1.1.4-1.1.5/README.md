# Comparing `tmp/CTG_Utils-1.1.4.tar.gz` & `tmp/CTG_Utils-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTG_Utils-1.1.4.tar", last modified: Wed May 15 10:08:57 2024, max compression
+gzip compressed data, was "CTG_Utils-1.1.5.tar", last modified: Thu May 16 15:51:27 2024, max compression
```

## Comparing `CTG_Utils-1.1.4.tar` & `CTG_Utils-1.1.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:57.249082 CTG_Utils-1.1.4/
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:57.191600 CTG_Utils-1.1.4/CTG_Utils/
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:57.210541 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/
--rw-rw-rw-   0        0        0     8463 2024-05-15 08:54:53.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTGClasses.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:57.222448 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/
--rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
--rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
--rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
--rw-rw-rw-   0        0        0     1914 2024-05-15 10:01:28.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt
--rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
--rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
--rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
--rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
--rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
--rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
--rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
--rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_config.py
--rw-rw-rw-   0        0        0    19381 2024-05-15 09:51:40.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_effectif.py
--rw-rw-rw-   0        0        0    11461 2024-05-12 12:33:31.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_plot.py
--rw-rw-rw-   0        0        0    15877 2024-05-12 15:37:19.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_synthese.py
--rw-rw-rw-   0        0        0     4645 2024-05-10 17:35:42.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_utility.py
--rw-rw-rw-   0        0        0      214 2024-05-15 10:05:43.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_Func/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:57.247635 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/
--rw-rw-rw-   0        0        0    16064 2024-05-14 08:52:29.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/GUI_Globals.py
--rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageDivers.py
--rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageEffectif.py
--rw-rw-rw-   0        0        0    11622 2024-05-12 11:11:49.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageSorties.py
--rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageSynthese.py
--rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageTendance.py
--rw-rw-rw-   0        0        0    32252 2024-05-15 06:32:08.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/Page_Classes.py
--rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/Useful_Classes.py
--rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/Useful_Functions.py
--rw-rw-rw-   0        0        0      221 2024-05-15 10:06:27.000000 CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-15 10:08:57.202285 CTG_Utils-1.1.4/CTG_Utils.egg-info/
--rw-rw-rw-   0        0        0      681 2024-05-15 10:08:56.000000 CTG_Utils-1.1.4/CTG_Utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1304 2024-05-15 10:08:56.000000 CTG_Utils-1.1.4/CTG_Utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 10:08:56.000000 CTG_Utils-1.1.4/CTG_Utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-15 10:08:56.000000 CTG_Utils-1.1.4/CTG_Utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2024-05-15 10:08:56.000000 CTG_Utils-1.1.4/CTG_Utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.4/LICENSE
--rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      681 2024-05-15 10:08:57.248647 CTG_Utils-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-15 10:08:57.249082 CTG_Utils-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1367 2024-05-15 10:05:31.000000 CTG_Utils-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.165170 CTG_Utils-1.1.5/
+drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.113063 CTG_Utils-1.1.5/CTG_Utils/
+drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.130551 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/
+-rw-rw-rw-   0        0        0     9358 2024-05-15 14:59:23.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTGClasses.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.142522 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/
+-rw-rw-rw-   0        0        0       41 2024-04-03 06:31:10.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/CTG.yaml
+-rw-rw-rw-   0        0        0      605 2023-09-01 12:09:43.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml
+-rw-rw-rw-   0        0        0      194 2024-05-15 10:03:47.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/help.txt
+-rw-rw-rw-   0        0        0     1920 2024-05-15 10:17:54.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt
+-rw-rw-rw-   0        0        0   228969 2024-05-05 16:57:27.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico
+-rw-rw-rw-   0        0        0    34827 2024-05-05 14:03:57.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png
+-rw-rw-rw-   0        0        0    26973 2024-05-06 17:53:49.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG
+-rw-rw-rw-   0        0        0   100526 2024-05-06 17:57:15.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico
+-rw-rw-rw-   0        0        0     1576 2024-05-10 18:06:52.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml
+-rw-rw-rw-   0        0        0      574 2024-04-15 12:33:24.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml
+-rw-rw-rw-   0        0        0  9545867 2024-04-03 11:27:38.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv
+-rw-rw-rw-   0        0        0      488 2024-05-09 07:18:30.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_config.py
+-rw-rw-rw-   0        0        0    19497 2024-05-16 15:18:28.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_effectif.py
+-rw-rw-rw-   0        0        0    11917 2024-05-16 10:06:26.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_plot.py
+-rw-rw-rw-   0        0        0    15863 2024-05-16 13:51:41.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_synthese.py
+-rw-rw-rw-   0        0        0     4328 2024-05-16 11:35:42.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_utility.py
+-rw-rw-rw-   0        0        0      214 2024-05-15 06:16:14.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_Func/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.164173 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/
+-rw-rw-rw-   0        0        0    16064 2024-05-14 08:52:29.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/GUI_Globals.py
+-rw-rw-rw-   0        0        0    10886 2024-05-10 12:46:38.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageDivers.py
+-rw-rw-rw-   0        0        0    11530 2024-05-07 13:39:45.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageEffectif.py
+-rw-rw-rw-   0        0        0    11622 2024-05-16 07:23:59.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageSorties.py
+-rw-rw-rw-   0        0        0    10763 2024-05-09 13:49:41.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageSynthese.py
+-rw-rw-rw-   0        0        0    10944 2024-05-13 07:34:59.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageTendance.py
+-rw-rw-rw-   0        0        0    32252 2024-05-15 06:32:08.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Page_Classes.py
+-rw-rw-rw-   0        0        0    13687 2024-04-26 08:07:42.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Useful_Classes.py
+-rw-rw-rw-   0        0        0    11454 2024-05-12 12:03:55.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Useful_Functions.py
+-rw-rw-rw-   0        0        0      221 2024-05-15 06:17:11.000000 CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:51:27.123741 CTG_Utils-1.1.5/CTG_Utils.egg-info/
+-rw-rw-rw-   0        0        0      681 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1304 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2024-05-16 15:51:26.000000 CTG_Utils-1.1.5/CTG_Utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1088 2022-03-26 14:35:29.000000 CTG_Utils-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0       43 2024-05-08 19:17:34.000000 CTG_Utils-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      681 2024-05-16 15:51:27.165170 CTG_Utils-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2022-03-19 12:02:13.000000 CTG_Utils-1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 15:51:27.165170 CTG_Utils-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2024-05-16 15:50:18.000000 CTG_Utils-1.1.5/setup.py
```

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTGClasses.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTGClasses.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         
         self.effectif = df      # effectif year
         self.effectif_1 = df_1  # effectif year moins un
 
         self.moy_age_entrants, self.nbr_nouveaux_licencié, self.nouveaux_licenciés_noms = self.nouveaux_entrants()
         self.moy_age_sortants, self.nbr_sortants, self.sortants_noms = self.sortants() 
         
+        self.cotisation_licence,self.cotisation_totale, self.cotisation_ctg = self.cotisation()
+        
     @staticmethod
     def distance_(row,dh):
     
         # Standard library imports
         from math import asin, cos, radians, sin, sqrt
         
         # Third party imports        
@@ -87,17 +89,17 @@
         
         correction = read_correction_effectifs(self.year,self.ctg_path)
         if correction["dic_part_club"] is not None:
             part_club_dic = correction["dic_part_club"]
             stat.append(f'Nombre de membres sympatisant : {len(part_club_dic)}')
             part_club_list = '; '.join([f"{x.split(',')[0][0]}. {x.split(',')[1]}"  
                                         for x in correction['dic_part_club']])
-            stat.append(f'Membres sympatisant : {part_club_list}')
+            stat.append(f'Membres sympatisants : {part_club_list}')
         else:
-            stat.append(f'Nombre de membres sympatisant : inconnu ')
+            stat.append(f'Nombre de membres sympatisants : inconnu ')
         stat.append(' ')
         
         
         stat.append(f"{self.nbr_nouveaux_licencié} nouveaux licenciés de moyenne d'âge de {round(self.moy_age_entrants,1)} ans")
         stat.append(f"Liste des nouveaux :\n{self.nouveaux_licenciés_noms}")
         stat.append(f"{self.nbr_sortants} licences non renouvellées de moyenne d'âge de {round(self.moy_age_sortants,1)} ans")
         stat.append(f"Liste des sortants :\n{self.sortants_noms}")
@@ -117,14 +119,17 @@
         for pratique in da.index:
             stat.append(f'{pratique} : {da[pratique]}')
         stat.append(' ')
         
         self.effectif = self.effectif.rename(columns={'\n\t\t\t\tAbonnements':'Abonnements'})
         nbr_abonnements = len(self.effectif.query('Abonnements == "Oui"'))
         stat.append(f"Nombre d'abonnés à la revue FFCT : {nbr_abonnements} ({round(100*nbr_abonnements/nbr_membres)} %)")
+        stat.append(f"\ncotisation licence ffct : {self.cotisation_licence} €")
+        stat.append(f"cotisation assurence : {self.cotisation_totale-self.cotisation_licence} €")
+        stat.append(f"cotisation CTG : {self.cotisation_ctg} €")
         path_info_effectif = self.ctg_path / Path(str(self.year)) / Path('STATISTIQUES')/Path(f'info_effectif_{self.year}.txt')
         stat.append(f"\n Ces information sont disponibles dans le fichier : \n{path_info_effectif}")
         stat ='\n'.join(stat)
         messagebox.showinfo(f'Statistique {self.year}',stat)
         
         
         with open(path_info_effectif,'w') as f:
@@ -156,14 +161,27 @@
         sortants_list = []
         for idx,row in dg.iterrows():
             sortants_list.append(f"{row['Prénom'][0]}. {row['Nom']}")
         sortants_noms = '; '.join(sortants_list)
         nbr_sortants = len(dg)
 
         return moy_age_sortants, nbr_sortants, sortants_noms
+        
+    def cotisation(self):
+        cotisation_licence = 'inconnue'
+        if 'Cotisation Licence' in self.effectif.columns:
+            cotisation_licence = sum(self.effectif['Cotisation Licence'])
+            
+        cotisation_totale = 'inconnue'
+        if 'Cotisation Totale' in self.effectif.columns:
+            cotisation_totale = sum(self.effectif['Cotisation Totale'])
+        
+        cotisation_ctg = 15*len(self.effectif)
+        return cotisation_licence,cotisation_totale, cotisation_ctg
+        
  
     def plot_histo(self):
     
         # Third party imports
         import matplotlib.pyplot as plt
         import pandas as pd
```

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/CTG_correction.yaml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/help_config.txt`

 * *Files 0% similar despite different names*

```diff
@@ -55,8 +55,8 @@
       from CTG_Utils.CTG_GUI import AppMain
 	  app_main = AppMain()
 	  app_main.mainloop()
 	  
    7- exécuter:
        pyinstaller --noconfirm --onefile --console --icon "C:/Users/franc/PyVenv/CTG_exe/venv/Lib/site-packages/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico" --add-data "C:/Users/franc/PyVenv/CTG_exe/venv/Lib/site-packages/CTG_Utils;CTG_Utils/"  "C:/Users/franc/PyVenv/CTG_exe/CTG_METER.py"
    
-   8- L'executable CTG_METER.exe est contenu dans le dossier "dist"
+   8- L'executable CTG_METER.exe est contenu dans le dossier CTG_exe/dist
```

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logo_ffvelo.png`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.PNG`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/logoctg4.ico`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/memory_sorties_old.yml`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_RefFiles/villes_france_premium.csv`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_effectif.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_effectif.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,26 +184,27 @@
         dg = inscrit_sejour( path / Path('CSV') /Path(sejour),no_match,df_effectif)
         
         if re.findall(r'^\d{4}[-_]',sejour):
             date = sejour[2:10].replace('_','-')
         else:
             date = str(year)[2:4] + '-' +sejour[0:5].replace('_','-')
             
-        if date in info_rando.keys():
-            if info_rando[date][2]=="randonnee" : 
+        dg['nbr_jours'] = 0    
+        if date in info_rando['date'].tolist():
+            dh = info_rando.query('type=="randonnee" and date==@date')
+            if not flag_sejour and len(dh) != 0 : 
                 dg['Type'] = "RANDONNEE"
             else:
                 dg['Type'] = type_sortie_default
-                
-            if flag_sejour and info_rando[date][2] == 'sejour':
-                dg['nbr_jours'] = info_rando[date][3]
-            else:
-                dg['nbr_jours'] = 1
-        else:
-            dg['nbr_jours'] = 0
+            
+            dg['nbr_jours'] = 1
+            dh = info_rando.query('type=="sejour" and date==@date')
+            if flag_sejour and len(dh) != 0:
+                dg['nbr_jours'] = dh['nbr_jours'].tolist()[0]    
+            
         if dg.reset_index().loc[0,'Nom'] is not None:
             nbr_inscrits = len(dg)
             if nbr_inscrits != 0:
                 nbr_moyen_participants = nbr_moyen_participants + (nbr_inscrits - nbr_moyen_participants)/counter
                 counter += 1
                 print(f"{os.path.split(path)[-1]} :{sejour}, Nombre d'inscrits : {nbr_inscrits}")
         df_list.append(dg)
```

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_plot.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,47 +158,60 @@
                 color=color,
                 fill=True,
             ).add_to(kol)
     return kol
     
 def stat_sorties_club(path_sorties_club, ctg_path, ylim=None, file_label=None,year = None):
 
+    # Standard library imports
     import datetime
     import os
     from pathlib import Path
     from collections import Counter
     from tkinter import messagebox
     
+    # Third party imports
     import matplotlib.pyplot as plt 
-    import yaml
-    from yaml.loader import SafeLoader
+    import pandas as pd
     
+    # Internal imports
     from CTG_Utils.CTG_Func.CTG_effectif import read_effectif
     from CTG_Utils.CTG_Func.CTG_effectif import correction_effectif
     from CTG_Utils.CTG_Func.CTG_effectif import read_effectif_corrected
     from CTG_Utils.CTG_Func.CTG_effectif import count_participation
     from CTG_Utils.CTG_Func.CTG_effectif import parse_date
     
     def addlabels(x,y):
+        import os
         for i in range(len(x)):
-            if info_rando is not None:
-                if x[i] in info_rando.keys():
-                    plt.text(i-0.2,y[i]+1,
-                             info_rando[x[i]][0],
-                             size=10,
-                             rotation=90,
-                             color=info_rando[x[i]][1]
-                             )
+            d = x[i]
+            color = 'g'
+            if os.path.split(path_sorties_club)[-1] == "SEJOUR" :
+                v = info_rando.query('date==@d and type=="sejour"')['name_activite'].tolist()
+            else:
+                v = info_rando.query('date==@d and type!="sejour"')['name_activite'].tolist()
+                t = info_rando.query('date==@d and type!="sejour"')['type'].tolist()
+                if len(t) != 0:
+                    color = "k" if t[0] =='randonnee' else "g"
+                
+            name = v[0] if len(v) != 0 else ""
+        
+            plt.text(i-0.2,y[i]+1,
+                     name,
+                     size=10,
+                     rotation=90,
+                     color=color #info_rando['color']
+                     )
+            
     if file_label is not None and os.path.isfile(file_label):
         flag_labels = True
-        with open(file_label,'r') as f:
-            info_rando_dict = yaml.safe_load(f)
-            info_rando = info_rando_dict['INFO_RANDO']
+        info_rando = pd.read_excel(file_label)
     else:
         flag_labels = False
+        print(file_label)
     
     no_match,df_total,_ = count_participation(path_sorties_club,ctg_path,year,info_rando)
     if no_match is None:
         messagebox.showinfo('WARNING',"Aucun participant n'a participé à ce type de sortie" )
     else:
         text_message = ''
         for tup in no_match:
@@ -275,15 +288,15 @@
     plt.legend(bbox_to_anchor =(0.75, 1.15), ncol = 2)
     plt.tight_layout()
     plt.show()
     fig_file = os.path.split(path_sorties_club)[-1].replace(' ','_')+'.png'
     plt.savefig(ctg_path / Path(str(year)) / Path('STATISTIQUES') / Path(fig_file),bbox_inches='tight')
     
     return df_total
-
+    
 def _distance(ϕ1, λ1,ϕ2, λ2):
     from math import asin, cos, radians, sin, sqrt
     ϕ1, λ1 = radians(ϕ1), radians(λ1)
     ϕ2, λ2 = radians(ϕ2), radians(λ2)
     rad = 6371
     dist = 2 * rad * asin(
                             sqrt(
```

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_synthese.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_synthese.py`

 * *Files 1% similar despite different names*

```diff
@@ -480,514 +480,513 @@
 00001df0: 2020 2020 6467 203d 2064 665f 746f 7461      dg = df_tota
 00001e00: 6c2e 7175 6572 7928 2754 7970 653d 3d22  l.query('Type=="
 00001e10: 5241 4e44 4f4e 4e45 4522 2729 2e67 726f  RANDONNEE"').gro
 00001e20: 7570 6279 2827 7365 6a6f 7572 2729 2e61  upby('sejour').a
 00001e30: 6767 2827 636f 756e 7427 295b 274e c2b0  gg('count')['N..
 00001e40: 204c 6963 656e 6369 c3a9 275d 0d0a 2020   Licenci..']..  
 00001e50: 2020 0d0a 2020 2020 6669 6720 3d20 706c    ..    fig = pl
-00001e60: 742e 6669 6775 7265 2866 6967 7369 7a65  t.figure(figsize
-00001e70: 3d28 3130 2c35 2929 0d0a 2020 2020 706c  =(10,5))..    pl
-00001e80: 742e 6261 7228 7261 6e67 6528 6c65 6e28  t.bar(range(len(
-00001e90: 6467 2929 2c64 672e 746f 6c69 7374 2829  dg)),dg.tolist()
-00001ea0: 290d 0a20 2020 2061 6464 6c61 6265 6c73  )..    addlabels
-00001eb0: 286c 6973 7428 7261 6e67 6528 6c65 6e28  (list(range(len(
-00001ec0: 6467 2929 292c 6467 2e74 6f6c 6973 7428  dg))),dg.tolist(
-00001ed0: 292c 302e 3229 0d0a 2020 2020 706c 742e  ),0.2)..    plt.
-00001ee0: 7874 6963 6b73 2872 616e 6765 286c 656e  xticks(range(len
-00001ef0: 2864 6729 292c 2064 672e 696e 6465 782c  (dg)), dg.index,
-00001f00: 2072 6f74 6174 696f 6e3d 2776 6572 7469   rotation='verti
-00001f10: 6361 6c27 290d 0a20 2020 2070 6c74 2e74  cal')..    plt.t
-00001f20: 6963 6b5f 7061 7261 6d73 2861 7869 733d  ick_params(axis=
-00001f30: 2778 272c 2072 6f74 6174 696f 6e3d 3930  'x', rotation=90
-00001f40: 2c20 6c61 6265 6c73 697a 653d 3130 290d  , labelsize=10).
-00001f50: 0a20 2020 2070 6c74 2e74 6963 6b5f 7061  .    plt.tick_pa
-00001f60: 7261 6d73 2861 7869 733d 2779 272c 6c61  rams(axis='y',la
-00001f70: 6265 6c73 697a 653d 3130 290d 0a20 2020  belsize=10)..   
-00001f80: 200d 0a20 2020 205f 203d 2070 6c74 2e74   ..    _ = plt.t
-00001f90: 6974 6c65 2866 2723 2072 616e 646f 7320  itle(f'# randos 
-00001fa0: 3a20 7b6c 656e 2864 6729 7d20 2c20 2320  : {len(dg)} , # 
-00001fb0: 7061 7274 6963 6970 616e 7473 203a 207b  participants : {
-00001fc0: 7375 6d28 6467 297d 2729 0d0a 2020 2020  sum(dg)}')..    
-00001fd0: 706c 742e 7469 6768 745f 6c61 796f 7574  plt.tight_layout
-00001fe0: 2829 0d0a 2020 2020 706c 742e 7368 6f77  ()..    plt.show
-00001ff0: 2829 0d0a 2020 2020 0d0a 2020 2020 6669  ()..    ..    fi
-00002000: 675f 6669 6c65 203d 2027 5359 4e54 4845  g_file = 'SYNTHE
-00002010: 5345 5f52 414e 444f 4e4e 4545 532e 706e  SE_RANDONNEES.pn
-00002020: 6727 0d0a 2020 2020 706c 742e 7361 7665  g'..    plt.save
-00002030: 6669 6728 6374 675f 7061 7468 202f 2050  fig(ctg_path / P
-00002040: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
-00002050: 2050 6174 6828 2753 5441 5449 5354 4951   Path('STATISTIQ
-00002060: 5545 5327 2920 2f20 5061 7468 2866 6967  UES') / Path(fig
-00002070: 5f66 696c 6529 2c62 626f 785f 696e 6368  _file),bbox_inch
-00002080: 6573 3d27 7469 6768 7427 290d 0a20 2020  es='tight')..   
-00002090: 200d 0a64 6566 206e 6272 5f73 656a 6f75   ..def nbr_sejou
-000020a0: 7273 5f61 6468 6572 656e 7428 7965 6172  rs_adherent(year
-000020b0: 2c20 6374 675f 7061 7468 293a 0d0a 0d0a  , ctg_path):....
-000020c0: 2020 2020 2320 5374 616e 6461 7264 206c      # Standard l
-000020d0: 6962 7261 7279 2069 6d70 6f72 7473 0d0a  ibrary imports..
-000020e0: 2020 2020 6672 6f6d 2063 6f6c 6c65 6374      from collect
-000020f0: 696f 6e73 2069 6d70 6f72 7420 436f 756e  ions import Coun
-00002100: 7465 720d 0a20 2020 2066 726f 6d20 7061  ter..    from pa
-00002110: 7468 6c69 6220 696d 706f 7274 2050 6174  thlib import Pat
-00002120: 680d 0a20 2020 200d 0a20 2020 2023 2054  h..    ..    # T
-00002130: 6869 7264 2070 6172 7479 2069 6d70 6f72  hird party impor
-00002140: 7473 0d0a 2020 2020 696d 706f 7274 206d  ts..    import m
-00002150: 6174 706c 6f74 6c69 622e 7079 706c 6f74  atplotlib.pyplot
-00002160: 2061 7320 706c 740d 0a20 2020 2069 6d70   as plt..    imp
-00002170: 6f72 7420 7061 6e64 6173 2061 7320 7064  ort pandas as pd
-00002180: 0d0a 2020 2020 0d0a 2020 2020 706c 742e  ..    ..    plt.
-00002190: 7374 796c 652e 7573 6528 2767 6770 6c6f  style.use('ggplo
-000021a0: 7427 290d 0a20 2020 200d 0a20 2020 2023  t')..    ..    #
-000021b0: 2066 756e 6374 696f 6e20 746f 2061 6464   function to add
-000021c0: 2076 616c 7565 206c 6162 656c 730d 0a20   value labels.. 
-000021d0: 2020 2064 6566 2061 6464 6c61 6265 6c73     def addlabels
-000021e0: 2878 2c79 293a 0d0a 2020 2020 2020 2020  (x,y):..        
-000021f0: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00002200: 656e 2878 2929 3a0d 0a20 2020 2020 2020  en(x)):..       
-00002210: 2020 2020 2070 6c74 2e74 6578 7428 785b       plt.text(x[
-00002220: 695d 2d30 2e32 2c79 5b69 5d2b 312c 795b  i]-0.2,y[i]+1,y[
-00002230: 695d 2c73 697a 653d 6c61 6265 6c5f 7369  i],size=label_si
-00002240: 7a65 290d 0a20 2020 206c 6162 656c 5f73  ze)..    label_s
-00002250: 697a 6520 3d20 3135 0d0a 2020 2020 6669  ize = 15..    fi
-00002260: 6c65 5f69 6e20 3d20 6374 675f 7061 7468  le_in = ctg_path
-00002270: 202f 2050 6174 6828 7374 7228 7965 6172   / Path(str(year
-00002280: 2929 202f 2050 6174 6828 2753 5441 5449  )) / Path('STATI
-00002290: 5354 4951 5545 5327 2920 2f20 5061 7468  STIQUES') / Path
-000022a0: 2827 7379 6e74 6865 7365 5f61 6468 6572  ('synthese_adher
-000022b0: 656e 742e 786c 7378 2729 0d0a 2020 2020  ent.xlsx')..    
-000022c0: 6466 5f74 6f74 616c 203d 2070 642e 7265  df_total = pd.re
-000022d0: 6164 5f65 7863 656c 2866 696c 655f 696e  ad_excel(file_in
-000022e0: 290d 0a20 2020 200d 0a20 2020 2063 203d  )..    ..    c =
-000022f0: 2043 6f75 6e74 6572 2829 0d0a 2020 2020   Counter()..    
-00002300: 6320 3d20 436f 756e 7465 7228 6466 5f74  c = Counter(df_t
-00002310: 6f74 616c 5b27 4e62 725f 5345 4a4f 5552  otal['Nbr_SEJOUR
-00002320: 5327 5d2e 746f 6c69 7374 2829 290d 0a20  S'].tolist()).. 
-00002330: 2020 2063 203d 2063 2e6d 6f73 745f 636f     c = c.most_co
-00002340: 6d6d 6f6e 2829 0d0a 0d0a 2020 2020 782c  mmon()....    x,
-00002350: 2079 203d 207a 6970 282a 6329 0d0a 2020   y = zip(*c)..  
-00002360: 2020 7820 3d20 6c69 7374 2878 290d 0a20    x = list(x).. 
-00002370: 2020 2079 203d 206c 6973 7428 7929 0d0a     y = list(y)..
-00002380: 2020 2020 0d0a 2020 2020 6669 672c 2061      ..    fig, a
-00002390: 7820 3d20 706c 742e 7375 6270 6c6f 7473  x = plt.subplots
-000023a0: 2866 6967 7369 7a65 3d28 352c 3529 290d  (figsize=(5,5)).
-000023b0: 0a20 2020 2070 6c74 2e62 6172 285b 7374  .    plt.bar([st
-000023c0: 7228 785f 7329 2066 6f72 2078 5f73 2069  r(x_s) for x_s i
-000023d0: 6e20 785d 2c79 290d 0a20 2020 2070 6c74  n x],y)..    plt
-000023e0: 2e78 6c61 6265 6c28 274e 6f6d 6272 6520  .xlabel('Nombre 
-000023f0: 6465 2070 6172 7469 6369 7061 7469 6f6e  de participation
-00002400: 20c3 a020 6465 7320 73c3 a96a 6f75 7273   .. des s..jours
-00002410: 2729 0d0a 2020 2020 706c 742e 796c 6162  ')..    plt.ylab
-00002420: 656c 2827 4e6f 6d62 7265 2064 6520 6c69  el('Nombre de li
-00002430: 6365 6e63 6965 7273 2729 0d0a 2020 2020  cenciers')..    
-00002440: 706c 742e 7469 636b 5f70 6172 616d 7328  plt.tick_params(
-00002450: 6178 6973 3d27 7827 2c20 6c61 6265 6c73  axis='x', labels
-00002460: 697a 653d 6c61 6265 6c5f 7369 7a65 290d  ize=label_size).
-00002470: 0a20 2020 2070 6c74 2e74 6963 6b5f 7061  .    plt.tick_pa
-00002480: 7261 6d73 2861 7869 733d 2779 272c 206c  rams(axis='y', l
-00002490: 6162 656c 7369 7a65 3d6c 6162 656c 5f73  abelsize=label_s
-000024a0: 697a 6529 0d0a 2020 2020 706c 742e 7469  ize)..    plt.ti
-000024b0: 746c 6528 7374 7228 7965 6172 292c 7061  tle(str(year),pa
-000024c0: 643d 3230 2c20 666f 6e74 7369 7a65 3d32  d=20, fontsize=2
-000024d0: 3029 0d0a 2020 2020 0d0a 2020 2020 6178  0)..    ..    ax
-000024e0: 2e73 6574 5f78 6c61 6265 6c28 274e 2073  .set_xlabel('N s
-000024f0: c3a9 6a6f 7572 7327 2c20 666f 6e74 7369  ..jours', fontsi
-00002500: 7a65 203d 206c 6162 656c 5f73 697a 6529  ze = label_size)
-00002510: 0d0a 2020 2020 6178 2e73 6574 5f79 6c61  ..    ax.set_yla
-00002520: 6265 6c28 274e 6f6d 6272 6520 6465 2043  bel('Nombre de C
-00002530: 5447 2061 7961 6e74 205c 6e20 7061 7274  TG ayant \n part
-00002540: 6963 6970 c3a9 20c3 a020 4e20 73c3 a96a  icip.. .. N s..j
-00002550: 6f75 7273 272c 2066 6f6e 7473 697a 6520  ours', fontsize 
-00002560: 3d20 6c61 6265 6c5f 7369 7a65 290d 0a20  = label_size).. 
-00002570: 2020 200d 0a20 2020 2078 2e73 6f72 7428     ..    x.sort(
-00002580: 290d 0a20 2020 2061 6464 6c61 6265 6c73  )..    addlabels
-00002590: 2878 2c79 290d 0a20 2020 2070 6c74 2e74  (x,y)..    plt.t
-000025a0: 6967 6874 5f6c 6179 6f75 7428 290d 0a20  ight_layout().. 
-000025b0: 2020 2070 6c74 2e73 686f 7728 290d 0a0d     plt.show()...
-000025c0: 0a20 2020 2066 6967 5f66 696c 6520 3d20  .    fig_file = 
-000025d0: 2753 454a 4f55 5253 5f53 5441 545f 5041  'SEJOURS_STAT_PA
-000025e0: 5254 4943 4950 4154 494f 4e2e 706e 6727  RTICIPATION.png'
-000025f0: 0d0a 2020 2020 706c 742e 7361 7665 6669  ..    plt.savefi
-00002600: 6728 6374 675f 7061 7468 202f 2050 6174  g(ctg_path / Pat
-00002610: 6828 7374 7228 7965 6172 2929 202f 2050  h(str(year)) / P
-00002620: 6174 6828 2753 5441 5449 5354 4951 5545  ath('STATISTIQUE
-00002630: 5327 2920 2f20 5061 7468 2866 6967 5f66  S') / Path(fig_f
-00002640: 696c 6529 2c62 626f 785f 696e 6368 6573  ile),bbox_inches
-00002650: 3d27 7469 6768 7427 290d 0a20 2020 200d  ='tight')..    .
-00002660: 0a64 6566 2072 6561 645f 6d65 6d6f 7279  .def read_memory
-00002670: 5f73 6f72 7469 6573 2829 3a0d 0a0d 0a20  _sorties():.... 
-00002680: 2020 2023 2053 7461 6e64 6172 6420 6c69     # Standard li
-00002690: 6272 6172 7920 696d 706f 7274 730d 0a20  brary imports.. 
-000026a0: 2020 2069 6d70 6f72 7420 6f73 2e70 6174     import os.pat
-000026b0: 680d 0a20 2020 2066 726f 6d20 7061 7468  h..    from path
-000026c0: 6c69 6220 696d 706f 7274 2050 6174 680d  lib import Path.
-000026d0: 0a0d 0a20 2020 2023 2033 7264 2070 6172  ...    # 3rd par
-000026e0: 7479 2069 6d70 6f72 7473 0d0a 2020 2020  ty imports..    
-000026f0: 696d 706f 7274 2079 616d 6c0d 0a20 2020  import yaml..   
-00002700: 200d 0a20 2020 2023 2052 6561 6473 2074   ..    # Reads t
-00002710: 6865 2064 6566 6175 6c74 2050 5663 6861  he default PVcha
-00002720: 7261 6374 6572 697a 6174 696f 6e2e 7961  racterization.ya
-00002730: 6d6c 2063 6f6e 6669 6720 6669 6c65 0d0a  ml config file..
-00002740: 2020 2020 7061 7468 5f63 6f6e 6669 675f      path_config_
-00002750: 6669 6c65 203d 2050 6174 6828 5f5f 6669  file = Path(__fi
-00002760: 6c65 5f5f 292e 7061 7265 6e74 2e70 6172  le__).parent.par
-00002770: 656e 7420 2f20 5061 7468 2827 4354 475f  ent / Path('CTG_
-00002780: 4675 6e63 2729 202f 2050 6174 6828 2743  Func') / Path('C
-00002790: 5447 5f52 6566 4669 6c65 7327 2920 2f20  TG_RefFiles') / 
-000027a0: 5061 7468 2827 6d65 6d6f 7279 5f73 6f72  Path('memory_sor
-000027b0: 7469 6573 2e79 6d6c 2729 0d0a 2020 2020  ties.yml')..    
-000027c0: 7769 7468 206f 7065 6e28 7061 7468 5f63  with open(path_c
-000027d0: 6f6e 6669 675f 6669 6c65 2920 6173 2066  onfig_file) as f
-000027e0: 696c 653a 0d0a 2020 2020 2020 2020 6d65  ile:..        me
-000027f0: 6d6f 7279 203d 2079 616d 6c2e 7361 6665  mory = yaml.safe
-00002800: 5f6c 6f61 6428 6669 6c65 290d 0a20 2020  _load(file)..   
-00002810: 2020 2020 200d 0a20 2020 2020 2020 0d0a       ..       ..
-00002820: 2020 2020 7265 7475 726e 206d 656d 6f72      return memor
-00002830: 790d 0a20 2020 200d 0a64 6566 2065 766f  y..    ..def evo
-00002840: 6c75 7469 6f6e 5f73 6f72 7469 6573 2874  lution_sorties(t
-00002850: 7970 652c 6374 675f 7061 7468 293a 0d0a  ype,ctg_path):..
-00002860: 0d0a 2020 2020 2320 5374 616e 6461 7264  ..    # Standard
-00002870: 206c 6962 7261 7279 2069 6d70 6f72 7420   library import 
-00002880: 2020 200d 0a20 2020 2069 6d70 6f72 7420     ..    import 
-00002890: 6461 7465 7469 6d65 0d0a 2020 2020 6672  datetime..    fr
-000028a0: 6f6d 2070 6174 686c 6962 2069 6d70 6f72  om pathlib impor
-000028b0: 7420 5061 7468 0d0a 2020 2020 6672 6f6d  t Path..    from
-000028c0: 2063 6f6c 6c65 6374 696f 6e73 2069 6d70   collections imp
-000028d0: 6f72 7420 6e61 6d65 6474 7570 6c65 0d0a  ort namedtuple..
-000028e0: 0d0a 2020 2020 2320 5468 6972 6420 7061  ..    # Third pa
-000028f0: 7274 7920 6c69 6272 6172 7920 696d 706f  rty library impo
-00002900: 7274 2020 2020 200d 0a20 2020 2069 6d70  rt     ..    imp
-00002910: 6f72 7420 6d61 7470 6c6f 746c 6962 2e70  ort matplotlib.p
-00002920: 7970 6c6f 7420 6173 2070 6c74 0d0a 2020  yplot as plt..  
-00002930: 2020 696d 706f 7274 2070 616e 6461 7320    import pandas 
-00002940: 6173 2070 640d 0a20 2020 2020 200d 0a20  as pd..      .. 
-00002950: 2020 2023 2049 6e74 6572 6e61 6c20 696d     # Internal im
-00002960: 706f 7274 0d0a 2020 2020 696d 706f 7274  port..    import
-00002970: 2043 5447 5f55 7469 6c73 2061 7320 6374   CTG_Utils as ct
-00002980: 670d 0a20 2020 2066 726f 6d20 4354 475f  g..    from CTG_
-00002990: 5574 696c 732e 4354 475f 4755 492e 4755  Utils.CTG_GUI.GU
-000029a0: 495f 476c 6f62 616c 7320 696d 706f 7274  I_Globals import
-000029b0: 2041 4354 4956 4954 455f 4c49 5354 200d   ACTIVITE_LIST .
-000029c0: 0a20 2020 200d 0a20 2020 2064 6566 2061  .    ..    def a
-000029d0: 6464 5f6d 656d 6f72 7928 7374 6174 5f64  dd_memory(stat_d
-000029e0: 6963 2c79 6561 7273 293a 0d0a 2020 2020  ic,years):..    
-000029f0: 2020 2020 6d65 6d6f 7279 203d 2072 6561      memory = rea
-00002a00: 645f 6d65 6d6f 7279 5f73 6f72 7469 6573  d_memory_sorties
-00002a10: 2829 0d0a 2020 2020 0d0a 2020 2020 0d0a  ()..    ..    ..
-00002a20: 2020 2020 2020 2020 666f 7220 7965 6172          for year
-00002a30: 2c76 2069 6e20 6d65 6d6f 7279 5b27 6d65  ,v in memory['me
-00002a40: 6d6f 7279 275d 2e69 7465 6d73 2829 3a0d  mory'].items():.
-00002a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a70: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-00002a80: 2020 2020 2020 2020 2020 7374 6174 5f64            stat_d
-00002a90: 6963 5b73 7472 2879 6561 7229 5d20 3d20  ic[str(year)] = 
-00002aa0: 7374 6174 7965 6172 2876 5b27 5041 5254  statyear(v['PART
-00002ab0: 4943 4950 4154 494f 4e5f 5345 4a4f 5552  ICIPATION_SEJOUR
-00002ac0: 5327 5d2c 2020 2020 2020 2020 2020 2020  S'],            
-00002ad0: 2020 2020 2320 6e62 725f 7365 6a6f 7572      # nbr_sejour
-00002ae0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+00001e60: 742e 6669 6775 7265 2829 0d0a 2020 2020  t.figure()..    
+00001e70: 706c 742e 6261 7228 7261 6e67 6528 6c65  plt.bar(range(le
+00001e80: 6e28 6467 2929 2c64 672e 746f 6c69 7374  n(dg)),dg.tolist
+00001e90: 2829 290d 0a20 2020 2061 6464 6c61 6265  ())..    addlabe
+00001ea0: 6c73 286c 6973 7428 7261 6e67 6528 6c65  ls(list(range(le
+00001eb0: 6e28 6467 2929 292c 6467 2e74 6f6c 6973  n(dg))),dg.tolis
+00001ec0: 7428 292c 302e 3229 0d0a 2020 2020 706c  t(),0.2)..    pl
+00001ed0: 742e 7874 6963 6b73 2872 616e 6765 286c  t.xticks(range(l
+00001ee0: 656e 2864 6729 292c 2064 672e 696e 6465  en(dg)), dg.inde
+00001ef0: 782c 2072 6f74 6174 696f 6e3d 2776 6572  x, rotation='ver
+00001f00: 7469 6361 6c27 290d 0a20 2020 2070 6c74  tical')..    plt
+00001f10: 2e74 6963 6b5f 7061 7261 6d73 2861 7869  .tick_params(axi
+00001f20: 733d 2778 272c 2072 6f74 6174 696f 6e3d  s='x', rotation=
+00001f30: 3930 2c20 6c61 6265 6c73 697a 653d 3130  90, labelsize=10
+00001f40: 290d 0a20 2020 2070 6c74 2e74 6963 6b5f  )..    plt.tick_
+00001f50: 7061 7261 6d73 2861 7869 733d 2779 272c  params(axis='y',
+00001f60: 6c61 6265 6c73 697a 653d 3130 290d 0a20  labelsize=10).. 
+00001f70: 2020 200d 0a20 2020 205f 203d 2070 6c74     ..    _ = plt
+00001f80: 2e74 6974 6c65 2866 2723 2072 616e 646f  .title(f'# rando
+00001f90: 7320 3a20 7b6c 656e 2864 6729 7d20 2c20  s : {len(dg)} , 
+00001fa0: 2320 7061 7274 6963 6970 616e 7473 203a  # participants :
+00001fb0: 207b 7375 6d28 6467 297d 2729 0d0a 2020   {sum(dg)}')..  
+00001fc0: 2020 706c 742e 7469 6768 745f 6c61 796f    plt.tight_layo
+00001fd0: 7574 2829 0d0a 2020 2020 706c 742e 7368  ut()..    plt.sh
+00001fe0: 6f77 2829 0d0a 2020 2020 0d0a 2020 2020  ow()..    ..    
+00001ff0: 6669 675f 6669 6c65 203d 2027 5359 4e54  fig_file = 'SYNT
+00002000: 4845 5345 5f52 414e 444f 4e4e 4545 532e  HESE_RANDONNEES.
+00002010: 706e 6727 0d0a 2020 2020 706c 742e 7361  png'..    plt.sa
+00002020: 7665 6669 6728 6374 675f 7061 7468 202f  vefig(ctg_path /
+00002030: 2050 6174 6828 7374 7228 7965 6172 2929   Path(str(year))
+00002040: 202f 2050 6174 6828 2753 5441 5449 5354   / Path('STATIST
+00002050: 4951 5545 5327 2920 2f20 5061 7468 2866  IQUES') / Path(f
+00002060: 6967 5f66 696c 6529 2c62 626f 785f 696e  ig_file),bbox_in
+00002070: 6368 6573 3d27 7469 6768 7427 290d 0a20  ches='tight').. 
+00002080: 2020 200d 0a64 6566 206e 6272 5f73 656a     ..def nbr_sej
+00002090: 6f75 7273 5f61 6468 6572 656e 7428 7965  ours_adherent(ye
+000020a0: 6172 2c20 6374 675f 7061 7468 293a 0d0a  ar, ctg_path):..
+000020b0: 0d0a 2020 2020 2320 5374 616e 6461 7264  ..    # Standard
+000020c0: 206c 6962 7261 7279 2069 6d70 6f72 7473   library imports
+000020d0: 0d0a 2020 2020 6672 6f6d 2063 6f6c 6c65  ..    from colle
+000020e0: 6374 696f 6e73 2069 6d70 6f72 7420 436f  ctions import Co
+000020f0: 756e 7465 720d 0a20 2020 2066 726f 6d20  unter..    from 
+00002100: 7061 7468 6c69 6220 696d 706f 7274 2050  pathlib import P
+00002110: 6174 680d 0a20 2020 200d 0a20 2020 2023  ath..    ..    #
+00002120: 2054 6869 7264 2070 6172 7479 2069 6d70   Third party imp
+00002130: 6f72 7473 0d0a 2020 2020 696d 706f 7274  orts..    import
+00002140: 206d 6174 706c 6f74 6c69 622e 7079 706c   matplotlib.pypl
+00002150: 6f74 2061 7320 706c 740d 0a20 2020 2069  ot as plt..    i
+00002160: 6d70 6f72 7420 7061 6e64 6173 2061 7320  mport pandas as 
+00002170: 7064 0d0a 2020 2020 0d0a 2020 2020 706c  pd..    ..    pl
+00002180: 742e 7374 796c 652e 7573 6528 2767 6770  t.style.use('ggp
+00002190: 6c6f 7427 290d 0a20 2020 200d 0a20 2020  lot')..    ..   
+000021a0: 2023 2066 756e 6374 696f 6e20 746f 2061   # function to a
+000021b0: 6464 2076 616c 7565 206c 6162 656c 730d  dd value labels.
+000021c0: 0a20 2020 2064 6566 2061 6464 6c61 6265  .    def addlabe
+000021d0: 6c73 2878 2c79 293a 0d0a 2020 2020 2020  ls(x,y):..      
+000021e0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+000021f0: 286c 656e 2878 2929 3a0d 0a20 2020 2020  (len(x)):..     
+00002200: 2020 2020 2020 2070 6c74 2e74 6578 7428         plt.text(
+00002210: 785b 695d 2d30 2e32 2c79 5b69 5d2b 312c  x[i]-0.2,y[i]+1,
+00002220: 795b 695d 2c73 697a 653d 6c61 6265 6c5f  y[i],size=label_
+00002230: 7369 7a65 290d 0a20 2020 206c 6162 656c  size)..    label
+00002240: 5f73 697a 6520 3d20 3135 0d0a 2020 2020  _size = 15..    
+00002250: 6669 6c65 5f69 6e20 3d20 6374 675f 7061  file_in = ctg_pa
+00002260: 7468 202f 2050 6174 6828 7374 7228 7965  th / Path(str(ye
+00002270: 6172 2929 202f 2050 6174 6828 2753 5441  ar)) / Path('STA
+00002280: 5449 5354 4951 5545 5327 2920 2f20 5061  TISTIQUES') / Pa
+00002290: 7468 2827 7379 6e74 6865 7365 5f61 6468  th('synthese_adh
+000022a0: 6572 656e 742e 786c 7378 2729 0d0a 2020  erent.xlsx')..  
+000022b0: 2020 6466 5f74 6f74 616c 203d 2070 642e    df_total = pd.
+000022c0: 7265 6164 5f65 7863 656c 2866 696c 655f  read_excel(file_
+000022d0: 696e 290d 0a20 2020 200d 0a20 2020 2063  in)..    ..    c
+000022e0: 203d 2043 6f75 6e74 6572 2829 0d0a 2020   = Counter()..  
+000022f0: 2020 6320 3d20 436f 756e 7465 7228 6466    c = Counter(df
+00002300: 5f74 6f74 616c 5b27 4e62 725f 5345 4a4f  _total['Nbr_SEJO
+00002310: 5552 5327 5d2e 746f 6c69 7374 2829 290d  URS'].tolist()).
+00002320: 0a20 2020 2063 203d 2063 2e6d 6f73 745f  .    c = c.most_
+00002330: 636f 6d6d 6f6e 2829 0d0a 0d0a 2020 2020  common()....    
+00002340: 782c 2079 203d 207a 6970 282a 6329 0d0a  x, y = zip(*c)..
+00002350: 2020 2020 7820 3d20 6c69 7374 2878 290d      x = list(x).
+00002360: 0a20 2020 2079 203d 206c 6973 7428 7929  .    y = list(y)
+00002370: 0d0a 2020 2020 0d0a 2020 2020 6669 672c  ..    ..    fig,
+00002380: 2061 7820 3d20 706c 742e 7375 6270 6c6f   ax = plt.subplo
+00002390: 7473 2866 6967 7369 7a65 3d28 352c 3529  ts(figsize=(5,5)
+000023a0: 290d 0a20 2020 2070 6c74 2e62 6172 285b  )..    plt.bar([
+000023b0: 7374 7228 785f 7329 2066 6f72 2078 5f73  str(x_s) for x_s
+000023c0: 2069 6e20 785d 2c79 290d 0a20 2020 2070   in x],y)..    p
+000023d0: 6c74 2e78 6c61 6265 6c28 274e 6f6d 6272  lt.xlabel('Nombr
+000023e0: 6520 6465 2070 6172 7469 6369 7061 7469  e de participati
+000023f0: 6f6e 20c3 a020 6465 7320 73c3 a96a 6f75  on .. des s..jou
+00002400: 7273 2729 0d0a 2020 2020 706c 742e 796c  rs')..    plt.yl
+00002410: 6162 656c 2827 4e6f 6d62 7265 2064 6520  abel('Nombre de 
+00002420: 6c69 6365 6e63 6965 7273 2729 0d0a 2020  licenciers')..  
+00002430: 2020 706c 742e 7469 636b 5f70 6172 616d    plt.tick_param
+00002440: 7328 6178 6973 3d27 7827 2c20 6c61 6265  s(axis='x', labe
+00002450: 6c73 697a 653d 6c61 6265 6c5f 7369 7a65  lsize=label_size
+00002460: 290d 0a20 2020 2070 6c74 2e74 6963 6b5f  )..    plt.tick_
+00002470: 7061 7261 6d73 2861 7869 733d 2779 272c  params(axis='y',
+00002480: 206c 6162 656c 7369 7a65 3d6c 6162 656c   labelsize=label
+00002490: 5f73 697a 6529 0d0a 2020 2020 706c 742e  _size)..    plt.
+000024a0: 7469 746c 6528 7374 7228 7965 6172 292c  title(str(year),
+000024b0: 7061 643d 3230 2c20 666f 6e74 7369 7a65  pad=20, fontsize
+000024c0: 3d32 3029 0d0a 2020 2020 0d0a 2020 2020  =20)..    ..    
+000024d0: 6178 2e73 6574 5f78 6c61 6265 6c28 274e  ax.set_xlabel('N
+000024e0: 2073 c3a9 6a6f 7572 7327 2c20 666f 6e74   s..jours', font
+000024f0: 7369 7a65 203d 206c 6162 656c 5f73 697a  size = label_siz
+00002500: 6529 0d0a 2020 2020 6178 2e73 6574 5f79  e)..    ax.set_y
+00002510: 6c61 6265 6c28 274e 6f6d 6272 6520 6465  label('Nombre de
+00002520: 2043 5447 2061 7961 6e74 205c 6e20 7061   CTG ayant \n pa
+00002530: 7274 6963 6970 c3a9 20c3 a020 4e20 73c3  rticip.. .. N s.
+00002540: a96a 6f75 7273 272c 2066 6f6e 7473 697a  .jours', fontsiz
+00002550: 6520 3d20 6c61 6265 6c5f 7369 7a65 290d  e = label_size).
+00002560: 0a20 2020 200d 0a20 2020 2078 2e73 6f72  .    ..    x.sor
+00002570: 7428 290d 0a20 2020 2061 6464 6c61 6265  t()..    addlabe
+00002580: 6c73 2878 2c79 290d 0a20 2020 2070 6c74  ls(x,y)..    plt
+00002590: 2e74 6967 6874 5f6c 6179 6f75 7428 290d  .tight_layout().
+000025a0: 0a20 2020 2070 6c74 2e73 686f 7728 290d  .    plt.show().
+000025b0: 0a0d 0a20 2020 2066 6967 5f66 696c 6520  ...    fig_file 
+000025c0: 3d20 2753 454a 4f55 5253 5f53 5441 545f  = 'SEJOURS_STAT_
+000025d0: 5041 5254 4943 4950 4154 494f 4e2e 706e  PARTICIPATION.pn
+000025e0: 6727 0d0a 2020 2020 706c 742e 7361 7665  g'..    plt.save
+000025f0: 6669 6728 6374 675f 7061 7468 202f 2050  fig(ctg_path / P
+00002600: 6174 6828 7374 7228 7965 6172 2929 202f  ath(str(year)) /
+00002610: 2050 6174 6828 2753 5441 5449 5354 4951   Path('STATISTIQ
+00002620: 5545 5327 2920 2f20 5061 7468 2866 6967  UES') / Path(fig
+00002630: 5f66 696c 6529 2c62 626f 785f 696e 6368  _file),bbox_inch
+00002640: 6573 3d27 7469 6768 7427 290d 0a20 2020  es='tight')..   
+00002650: 200d 0a64 6566 2072 6561 645f 6d65 6d6f   ..def read_memo
+00002660: 7279 5f73 6f72 7469 6573 2829 3a0d 0a0d  ry_sorties():...
+00002670: 0a20 2020 2023 2053 7461 6e64 6172 6420  .    # Standard 
+00002680: 6c69 6272 6172 7920 696d 706f 7274 730d  library imports.
+00002690: 0a20 2020 2069 6d70 6f72 7420 6f73 2e70  .    import os.p
+000026a0: 6174 680d 0a20 2020 2066 726f 6d20 7061  ath..    from pa
+000026b0: 7468 6c69 6220 696d 706f 7274 2050 6174  thlib import Pat
+000026c0: 680d 0a0d 0a20 2020 2023 2033 7264 2070  h....    # 3rd p
+000026d0: 6172 7479 2069 6d70 6f72 7473 0d0a 2020  arty imports..  
+000026e0: 2020 696d 706f 7274 2079 616d 6c0d 0a20    import yaml.. 
+000026f0: 2020 200d 0a20 2020 2023 2052 6561 6473     ..    # Reads
+00002700: 2074 6865 2064 6566 6175 6c74 2050 5663   the default PVc
+00002710: 6861 7261 6374 6572 697a 6174 696f 6e2e  haracterization.
+00002720: 7961 6d6c 2063 6f6e 6669 6720 6669 6c65  yaml config file
+00002730: 0d0a 2020 2020 7061 7468 5f63 6f6e 6669  ..    path_confi
+00002740: 675f 6669 6c65 203d 2050 6174 6828 5f5f  g_file = Path(__
+00002750: 6669 6c65 5f5f 292e 7061 7265 6e74 2e70  file__).parent.p
+00002760: 6172 656e 7420 2f20 5061 7468 2827 4354  arent / Path('CT
+00002770: 475f 4675 6e63 2729 202f 2050 6174 6828  G_Func') / Path(
+00002780: 2743 5447 5f52 6566 4669 6c65 7327 2920  'CTG_RefFiles') 
+00002790: 2f20 5061 7468 2827 6d65 6d6f 7279 5f73  / Path('memory_s
+000027a0: 6f72 7469 6573 2e79 6d6c 2729 0d0a 2020  orties.yml')..  
+000027b0: 2020 7769 7468 206f 7065 6e28 7061 7468    with open(path
+000027c0: 5f63 6f6e 6669 675f 6669 6c65 2920 6173  _config_file) as
+000027d0: 2066 696c 653a 0d0a 2020 2020 2020 2020   file:..        
+000027e0: 6d65 6d6f 7279 203d 2079 616d 6c2e 7361  memory = yaml.sa
+000027f0: 6665 5f6c 6f61 6428 6669 6c65 290d 0a20  fe_load(file).. 
+00002800: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00002810: 0d0a 2020 2020 7265 7475 726e 206d 656d  ..    return mem
+00002820: 6f72 790d 0a20 2020 200d 0a64 6566 2065  ory..    ..def e
+00002830: 766f 6c75 7469 6f6e 5f73 6f72 7469 6573  volution_sorties
+00002840: 2874 7970 652c 6374 675f 7061 7468 293a  (type,ctg_path):
+00002850: 0d0a 0d0a 2020 2020 2320 5374 616e 6461  ....    # Standa
+00002860: 7264 206c 6962 7261 7279 2069 6d70 6f72  rd library impor
+00002870: 7420 2020 200d 0a20 2020 2069 6d70 6f72  t    ..    impor
+00002880: 7420 6461 7465 7469 6d65 0d0a 2020 2020  t datetime..    
+00002890: 6672 6f6d 2070 6174 686c 6962 2069 6d70  from pathlib imp
+000028a0: 6f72 7420 5061 7468 0d0a 2020 2020 6672  ort Path..    fr
+000028b0: 6f6d 2063 6f6c 6c65 6374 696f 6e73 2069  om collections i
+000028c0: 6d70 6f72 7420 6e61 6d65 6474 7570 6c65  mport namedtuple
+000028d0: 0d0a 0d0a 2020 2020 2320 5468 6972 6420  ....    # Third 
+000028e0: 7061 7274 7920 6c69 6272 6172 7920 696d  party library im
+000028f0: 706f 7274 2020 2020 200d 0a20 2020 2069  port     ..    i
+00002900: 6d70 6f72 7420 6d61 7470 6c6f 746c 6962  mport matplotlib
+00002910: 2e70 7970 6c6f 7420 6173 2070 6c74 0d0a  .pyplot as plt..
+00002920: 2020 2020 696d 706f 7274 2070 616e 6461      import panda
+00002930: 7320 6173 2070 640d 0a20 2020 2020 200d  s as pd..      .
+00002940: 0a20 2020 2023 2049 6e74 6572 6e61 6c20  .    # Internal 
+00002950: 696d 706f 7274 0d0a 2020 2020 696d 706f  import..    impo
+00002960: 7274 2043 5447 5f55 7469 6c73 2061 7320  rt CTG_Utils as 
+00002970: 6374 670d 0a20 2020 2066 726f 6d20 4354  ctg..    from CT
+00002980: 475f 5574 696c 732e 4354 475f 4755 492e  G_Utils.CTG_GUI.
+00002990: 4755 495f 476c 6f62 616c 7320 696d 706f  GUI_Globals impo
+000029a0: 7274 2041 4354 4956 4954 455f 4c49 5354  rt ACTIVITE_LIST
+000029b0: 200d 0a20 2020 200d 0a20 2020 2064 6566   ..    ..    def
+000029c0: 2061 6464 5f6d 656d 6f72 7928 7374 6174   add_memory(stat
+000029d0: 5f64 6963 2c79 6561 7273 293a 0d0a 2020  _dic,years):..  
+000029e0: 2020 2020 2020 6d65 6d6f 7279 203d 2072        memory = r
+000029f0: 6561 645f 6d65 6d6f 7279 5f73 6f72 7469  ead_memory_sorti
+00002a00: 6573 2829 0d0a 2020 2020 0d0a 2020 2020  es()..    ..    
+00002a10: 0d0a 2020 2020 2020 2020 666f 7220 7965  ..        for ye
+00002a20: 6172 2c76 2069 6e20 6d65 6d6f 7279 5b27  ar,v in memory['
+00002a30: 6d65 6d6f 7279 275d 2e69 7465 6d73 2829  memory'].items()
+00002a40: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a60: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00002a70: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00002a80: 5f64 6963 5b73 7472 2879 6561 7229 5d20  _dic[str(year)] 
+00002a90: 3d20 7374 6174 7965 6172 2876 5b27 5041  = statyear(v['PA
+00002aa0: 5254 4943 4950 4154 494f 4e5f 5345 4a4f  RTICIPATION_SEJO
+00002ab0: 5552 5327 5d2c 2020 2020 2020 2020 2020  URS'],          
+00002ac0: 2020 2020 2020 2320 6e62 725f 7365 6a6f        # nbr_sejo
+00002ad0: 7572 730d 0a20 2020 2020 2020 2020 2020  urs..           
+00002ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2020 2020 2020 2020 2020 2020 2020 302c                0,
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 2020 2020 2020 2020 2020 2320 6a6f 7572            # jour
-00002b30: 735f 7365 6a6f 7572 0d0a 2020 2020 2020  s_sejour..      
+00002b00: 302c 2020 2020 2020 2020 2020 2020 2020  0,              
+00002b10: 2020 2020 2020 2020 2020 2020 2320 6a6f              # jo
+00002b20: 7572 735f 7365 6a6f 7572 0d0a 2020 2020  urs_sejour..    
+00002b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b60: 2020 2020 2076 5b27 534f 5254 4945 535f       v['SORTIES_
-00002b70: 434c 5542 5f44 494d 414e 4348 4527 5d2c  CLUB_DIMANCHE'],
-00002b80: 2023 2073 6f72 7469 655f 6469 6d61 6e63   # sortie_dimanc
-00002b90: 6865 5f63 6c75 620d 0a20 2020 2020 2020  he_club..       
+00002b50: 2020 2020 2020 2076 5b27 534f 5254 4945         v['SORTIE
+00002b60: 535f 434c 5542 5f44 494d 414e 4348 4527  S_CLUB_DIMANCHE'
+00002b70: 5d2c 2023 2073 6f72 7469 655f 6469 6d61  ], # sortie_dima
+00002b80: 6e63 6865 5f63 6c75 620d 0a20 2020 2020  nche_club..     
+00002b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bc0: 2020 2020 765b 2753 4f52 5449 4553 5f43      v['SORTIES_C
-00002bd0: 4c55 425f 5341 4d45 4449 275d 2c20 2020  LUB_SAMEDI'],   
-00002be0: 2320 736f 7274 6965 5f73 616d 6564 695f  # sortie_samedi_
-00002bf0: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
+00002bb0: 2020 2020 2020 765b 2753 4f52 5449 4553        v['SORTIES
+00002bc0: 5f43 4c55 425f 5341 4d45 4449 275d 2c20  _CLUB_SAMEDI'], 
+00002bd0: 2020 2320 736f 7274 6965 5f73 616d 6564    # sortie_samed
+00002be0: 695f 636c 7562 0d0a 2020 2020 2020 2020  i_club..        
+00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c20: 2076 5b27 534f 5254 4945 535f 4849 5645   v['SORTIES_HIVE
-00002c30: 5227 5d2c 2020 2020 2020 2020 2023 2073  R'],         # s
-00002c40: 6f72 7469 655f 6869 7665 725f 636c 7562  ortie_hiver_club
-00002c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2020 2020 2020 2020 2020 2020 2076 5b27               v['
-00002c80: 534f 5254 4945 535f 434c 5542 5f4a 4555  SORTIES_CLUB_JEU
-00002c90: 4449 275d 2c20 2020 2023 2073 6f72 7469  DI'],    # sorti
-00002ca0: 655f 6a65 7564 695f 636c 7562 0d0a 2020  e_jeudi_club..  
+00002c10: 2020 2076 5b27 534f 5254 4945 535f 4849     v['SORTIES_HI
+00002c20: 5645 5227 5d2c 2020 2020 2020 2020 2023  VER'],         #
+00002c30: 2073 6f72 7469 655f 6869 7665 725f 636c   sortie_hiver_cl
+00002c40: 7562 0d0a 2020 2020 2020 2020 2020 2020  ub..            
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00002c70: 5b27 534f 5254 4945 535f 434c 5542 5f4a  ['SORTIES_CLUB_J
+00002c80: 4555 4449 275d 2c20 2020 2023 2073 6f72  EUDI'],    # sor
+00002c90: 7469 655f 6a65 7564 695f 636c 7562 0d0a  tie_jeudi_club..
+00002ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2020 2020 2020 2020 2076 5b27 5241 4e44           v['RAND
-00002ce0: 4f4e 4e45 4553 275d 2c20 2020 2020 2020  ONNEES'],       
-00002cf0: 2020 2020 2023 2072 616e 646f 6e6e 6565       # randonnee
-00002d00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d20: 2020 2020 2020 2020 2020 2020 2076 5b27               v['
-00002d30: 4e6f 6d62 7265 5f73 656a 6f75 7273 275d  Nombre_sejours']
-00002d40: 2c20 2020 2020 2020 2023 206e 6272 5f73  ,        # nbr_s
-00002d50: 656a 6f75 7273 0d0a 2020 2020 2020 2020  ejours..        
+00002cc0: 2020 2020 2020 2020 2020 2076 5b27 5241             v['RA
+00002cd0: 4e44 4f4e 4e45 4553 275d 2c20 2020 2020  NDONNEES'],     
+00002ce0: 2020 2020 2020 2023 2072 616e 646f 6e6e         # randonn
+00002cf0: 6565 0d0a 2020 2020 2020 2020 2020 2020  ee..            
+00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d10: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00002d20: 5b27 4e6f 6d62 7265 5f73 656a 6f75 7273  ['Nombre_sejours
+00002d30: 275d 2c20 2020 2020 2020 2023 206e 6272  '],        # nbr
+00002d40: 5f73 656a 6f75 7273 0d0a 2020 2020 2020  _sejours..      
+00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d80: 2020 2030 2c29 2020 2020 2020 2020 2020     0,)          
-00002d90: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00002da0: 206e 6272 5f6a 6f75 7273 5f73 656a 6f75   nbr_jours_sejou
-00002db0: 7273 0d0a 2020 2020 2020 2020 2020 2020  rs..            
+00002d70: 2020 2020 2030 2c29 2020 2020 2020 2020       0,)        
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2023 206e 6272 5f6a 6f75 7273 5f73 656a   # nbr_jours_sej
+00002da0: 6f75 7273 0d0a 2020 2020 2020 2020 2020  ours..          
+00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002df0: 0d0a 2020 2020 2020 2020 2020 2020 7965  ..            ye
-00002e00: 6172 732e 6170 7065 6e64 2873 7472 2879  ars.append(str(y
-00002e10: 6561 7229 290d 0a20 2020 2020 2020 2020  ear))..         
-00002e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e30: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
-00002e40: 2066 696c 6c5f 7374 6174 5f79 6561 7228   fill_stat_year(
-00002e50: 7965 6172 293a 0d0a 2020 2020 0d0a 2020  year):..    ..  
-00002e60: 2020 2020 2020 2320 496e 7465 726e 616c        # Internal
-00002e70: 206c 6962 7261 7279 2069 6d70 6f72 7473   library imports
-00002e80: 0d0a 2020 2020 2020 2020 6672 6f6d 2043  ..        from C
-00002e90: 5447 5f55 7469 6c73 2e43 5447 5f46 756e  TG_Utils.CTG_Fun
-00002ea0: 632e 4354 475f 7574 696c 6974 7920 696d  c.CTG_utility im
-00002eb0: 706f 7274 2067 6574 5f73 656a 6f75 725f  port get_sejour_
-00002ec0: 696e 666f 0d0a 2020 2020 2020 2020 0d0a  info..        ..
-00002ed0: 2020 2020 2020 2020 7365 6a6f 7572 5f69          sejour_i
-00002ee0: 6e66 6f20 3d20 6765 745f 7365 6a6f 7572  nfo = get_sejour
-00002ef0: 5f69 6e66 6f28 6374 675f 7061 7468 2c79  _info(ctg_path,y
-00002f00: 6561 7229 0d0a 2020 2020 2020 2020 0d0a  ear)..        ..
-00002f10: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002f20: 2020 6669 6c65 5f69 6e20 3d20 6374 675f    file_in = ctg_
-00002f30: 7061 7468 202f 2050 6174 6828 7374 7228  path / Path(str(
-00002f40: 7965 6172 2929 202f 2050 6174 6828 2753  year)) / Path('S
-00002f50: 5441 5449 5354 4951 5545 5327 2920 2f20  TATISTIQUES') / 
-00002f60: 5061 7468 2827 7379 6e74 6865 7365 5f61  Path('synthese_a
-00002f70: 6468 6572 656e 742e 786c 7378 2729 0d0a  dherent.xlsx')..
-00002f80: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00002f90: 2020 6466 203d 2070 642e 7265 6164 5f65    df = pd.read_e
-00002fa0: 7863 656c 2866 696c 655f 696e 290d 0a20  xcel(file_in).. 
-00002fb0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00002fc0: 2073 7461 745f 7965 6172 203d 2073 7461   stat_year = sta
-00002fd0: 7479 6561 7228 6466 5b27 4e62 725f 5345  tyear(df['Nbr_SE
-00002fe0: 4a4f 5552 5327 5d2e 7375 6d28 292c 2020  JOURS'].sum(),  
-00002ff0: 2020 2020 2020 2020 2020 2023 206e 6272             # nbr
-00003000: 5f6a 6f75 7273 5f70 6172 7469 6369 7061  _jours_participa
-00003010: 7469 6f6e 5f73 656a 6f75 7273 0d0a 2020  tion_sejours..  
-00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003030: 2020 2020 2020 2020 2020 2064 665b 2753             df['S
-00003040: 454a 4f55 522d 4a4f 5552 275d 2e73 756d  EJOUR-JOUR'].sum
-00003050: 2829 2c20 2020 2020 2020 2020 2020 2020  (),             
-00003060: 2320 6e62 725f 7061 7274 6963 6970 6174  # nbr_participat
-00003070: 696f 6e73 5f73 656a 6f75 720d 0a20 2020  ions_sejour..   
-00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003090: 2020 2020 2020 2020 2020 6466 5b27 534f            df['SO
-000030a0: 5254 4945 2044 5520 4449 4d41 4e43 4845  RTIE DU DIMANCHE
-000030b0: 2043 4c55 4227 5d2e 7375 6d28 292c 2023   CLUB'].sum(), #
-000030c0: 2073 6f72 7469 655f 6469 6d61 6e63 6865   sortie_dimanche
-000030d0: 5f63 6c75 620d 0a20 2020 2020 2020 2020  _club..         
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 2020 2020 6466 5b27 534f 5254 4945 2044      df['SORTIE D
-00003100: 5520 5341 4d45 4449 2043 4c55 4227 5d2e  U SAMEDI CLUB'].
-00003110: 7375 6d28 292c 2020 2023 2073 6f72 7469  sum(),   # sorti
-00003120: 655f 7361 6d65 6469 5f63 6c75 620d 0a20  e_samedi_club.. 
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 2020 2020 2020 2020 2020 6466 5b27              df['
-00003150: 534f 5254 4945 2048 4956 4552 275d 2e73  SORTIE HIVER'].s
-00003160: 756d 2829 2c20 2020 2020 2020 2020 2020  um(),           
-00003170: 2023 2073 6f72 7469 655f 6869 7665 725f   # sortie_hiver_
-00003180: 636c 7562 0d0a 2020 2020 2020 2020 2020  club..          
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2020 2064 665b 2753 4f52 5449 4520 4455     df['SORTIE DU
-000031b0: 204a 4555 4449 2043 4c55 4227 5d2e 7375   JEUDI CLUB'].su
-000031c0: 6d28 292c 2020 2020 2320 736f 7274 6965  m(),    # sortie
-000031d0: 5f6a 6575 6469 5f63 6c75 620d 0a20 2020  _jeudi_club..   
-000031e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031f0: 2020 2020 2020 2020 2020 6466 5b27 5241            df['RA
-00003200: 4e44 4f4e 4e45 4527 5d2e 7375 6d28 292c  NDONNEE'].sum(),
-00003210: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00003220: 2072 616e 646f 6e6e 6565 0d0a 2020 2020   randonnee..    
-00003230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003240: 2020 2020 2020 2020 2073 656a 6f75 725f           sejour_
-00003250: 696e 666f 2e6e 6272 5f73 656a 6f75 7273  info.nbr_sejours
-00003260: 2c20 2020 2020 2020 2020 2020 2020 2320  ,             # 
-00003270: 6e62 725f 7365 6a6f 7572 7320 0d0a 2020  nbr_sejours ..  
-00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003290: 2020 2020 2020 2020 2020 2073 656a 6f75             sejou
-000032a0: 725f 696e 666f 2e6e 6272 5f6a 6f75 7273  r_info.nbr_jours
-000032b0: 2920 2020 2020 2020 2020 2020 2020 2020  )               
-000032c0: 2320 6e62 725f 6a6f 7572 735f 7365 6a6f  # nbr_jours_sejo
-000032d0: 7572 7320 2020 2020 2020 2020 2020 2020  urs             
-000032e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003310: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00003320: 2073 7461 745f 7965 6172 0d0a 2020 2020   stat_year..    
-00003330: 0d0a 2020 2020 6465 6620 6164 646c 6162  ..    def addlab
-00003340: 656c 7328 782c 792c 6f66 6673 6574 293a  els(x,y,offset):
-00003350: 0d0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
-00003360: 696e 2072 616e 6765 286c 656e 2878 2929  in range(len(x))
-00003370: 3a0d 0a20 2020 2020 2020 2020 2020 2070  :..            p
-00003380: 6c74 2e74 6578 7428 785b 695d 2c79 5b69  lt.text(x[i],y[i
-00003390: 5d2b 6f66 6673 6574 2c72 6f75 6e64 2879  ]+offset,round(y
-000033a0: 5b69 5d2c 3129 2c73 697a 653d 3130 290d  [i],1),size=10).
-000033b0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-000033c0: 2020 2064 6566 2070 6c6f 745f 7374 6174     def plot_stat
-000033d0: 2879 6561 7273 2c6e 625f 7061 7274 6963  (years,nb_partic
-000033e0: 6970 616e 7473 2c74 6974 6c65 2c6c 6162  ipants,title,lab
-000033f0: 656c 5f79 293a 0d0a 2020 2020 2020 2020  el_y):..        
-00003400: 706c 742e 6669 6775 7265 2866 6967 7369  plt.figure(figsi
-00003410: 7a65 3d28 382c 2036 2929 0d0a 2020 2020  ze=(8, 6))..    
-00003420: 2020 2020 636f 6c6f 7273 203d 205b 2723      colors = ['#
-00003430: 6664 6161 3438 275d 200d 0a20 2020 2020  fdaa48'] ..     
-00003440: 2020 2073 697a 655f 6c61 6265 6c20 3d20     size_label = 
-00003450: 3230 0d0a 2020 2020 2020 2020 706c 742e  20..        plt.
-00003460: 6261 7228 7965 6172 732c 6e62 5f70 6172  bar(years,nb_par
-00003470: 7469 6369 7061 6e74 732c 636f 6c6f 723d  ticipants,color=
-00003480: 636f 6c6f 7273 290d 0a20 2020 2020 2020  colors)..       
-00003490: 2070 6c74 2e79 6c61 6265 6c28 6c61 6265   plt.ylabel(labe
-000034a0: 6c5f 792c 7369 7a65 3d73 697a 655f 6c61  l_y,size=size_la
-000034b0: 6265 6c29 0d0a 2020 2020 2020 2020 6164  bel)..        ad
-000034c0: 646c 6162 656c 7328 7965 6172 732c 6e62  dlabels(years,nb
-000034d0: 5f70 6172 7469 6369 7061 6e74 732c 3129  _participants,1)
-000034e0: 0d0a 2020 2020 2020 2020 706c 742e 7874  ..        plt.xt
-000034f0: 6963 6b73 2872 6f74 6174 696f 6e3d 3930  icks(rotation=90
-00003500: 290d 0a20 2020 2020 2020 2070 6c74 2e74  )..        plt.t
-00003510: 6963 6b5f 7061 7261 6d73 2861 7869 733d  ick_params(axis=
-00003520: 2778 272c 206c 6162 656c 7369 7a65 3d73  'x', labelsize=s
-00003530: 697a 655f 6c61 6265 6c29 0d0a 2020 2020  ize_label)..    
-00003540: 2020 2020 706c 742e 7469 636b 5f70 6172      plt.tick_par
-00003550: 616d 7328 6178 6973 3d27 7927 2c20 6c61  ams(axis='y', la
-00003560: 6265 6c73 697a 653d 7369 7a65 5f6c 6162  belsize=size_lab
-00003570: 656c 290d 0a20 2020 2020 2020 2070 6c74  el)..        plt
-00003580: 2e74 6974 6c65 2874 6974 6c65 2c66 6f6e  .title(title,fon
-00003590: 7473 697a 653d 3138 290d 0a20 2020 2020  tsize=18)..     
-000035a0: 2020 2070 6c74 2e74 6967 6874 5f6c 6179     plt.tight_lay
-000035b0: 6f75 7428 290d 0a20 2020 2020 2020 2070  out()..        p
-000035c0: 6c74 2e73 686f 7728 290d 0a20 2020 200d  lt.show()..    .
-000035d0: 0a20 2020 2073 7461 7479 6561 7220 3d20  .    statyear = 
-000035e0: 6e61 6d65 6474 7570 6c65 2827 6163 7469  namedtuple('acti
-000035f0: 7669 7465 272c 2041 4354 4956 4954 455f  vite', ACTIVITE_
-00003600: 4c49 5354 290d 0a20 0d0a 2020 2020 706c  LIST).. ..    pl
-00003610: 742e 7374 796c 652e 7573 6528 2767 6770  t.style.use('ggp
-00003620: 6c6f 7427 290d 0a20 2020 2079 6561 7273  lot')..    years
-00003630: 203d 205b 5d0d 0a20 2020 2073 7461 745f   = []..    stat_
-00003640: 6469 6320 3d20 7b7d 0d0a 2020 2020 6164  dic = {}..    ad
-00003650: 645f 6d65 6d6f 7279 2873 7461 745f 6469  d_memory(stat_di
-00003660: 632c 7965 6172 7329 0d0a 0d0a 2020 2020  c,years)....    
-00003670: 746f 6461 7920 3d20 6461 7465 7469 6d65  today = datetime
-00003680: 2e64 6174 6574 696d 652e 6e6f 7728 290d  .datetime.now().
-00003690: 0a20 2020 2079 6561 7273 5f6e 6577 203d  .    years_new =
-000036a0: 205b 7374 7228 7965 6172 2920 666f 7220   [str(year) for 
-000036b0: 7965 6172 2069 6e20 7261 6e67 6528 3230  year in range(20
-000036c0: 3232 2c74 6f64 6179 2e79 6561 722b 3129  22,today.year+1)
-000036d0: 5d0d 0a20 2020 2066 6f72 2079 6561 7220  ]..    for year 
-000036e0: 696e 2079 6561 7273 5f6e 6577 3a0d 0a20  in years_new:.. 
-000036f0: 2020 2020 2020 2073 7461 745f 6469 635b         stat_dic[
-00003700: 7965 6172 5d20 3d20 6669 6c6c 5f73 7461  year] = fill_sta
-00003710: 745f 7965 6172 2879 6561 7229 0d0a 2020  t_year(year)..  
-00003720: 2020 2020 2020 0d0a 2020 2020 7965 6172        ..    year
-00003730: 7320 3d20 7965 6172 7320 2b20 7965 6172  s = years + year
-00003740: 735f 6e65 7720 2020 0d0a 2020 2020 0d0a  s_new   ..    ..
-00003750: 2020 2020 0d0a 2020 2020 6966 2074 7970      ..    if typ
-00003760: 6520 3d3d 2027 6e62 725f 6a6f 7572 735f  e == 'nbr_jours_
-00003770: 7061 7274 6963 6970 6174 696f 6e5f 7365  participation_se
-00003780: 6a6f 7572 7327 3a0d 0a20 2020 2020 2020  jours':..       
-00003790: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
-000037a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000037b0: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
-000037c0: 6561 725d 2e6e 6272 5f6a 6f75 7273 5f70  ear].nbr_jours_p
-000037d0: 6172 7469 6369 7061 7469 6f6e 5f73 656a  articipation_sej
-000037e0: 6f75 7273 2066 6f72 2079 6561 7220 696e  ours for year in
-000037f0: 2079 6561 7273 5d2c 0d0a 2020 2020 2020   years],..      
-00003800: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00003810: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003820: 2020 2020 2074 7970 6529 0d0a 2020 2020       type)..    
-00003830: 656c 6966 2020 7479 7065 203d 3d20 2773  elif  type == 's
-00003840: 6f72 7469 655f 6469 6d61 6e63 6865 5f63  ortie_dimanche_c
-00003850: 6c75 6227 3a0d 0a20 2020 2020 2020 2070  lub':..        p
-00003860: 6c6f 745f 7374 6174 2879 6561 7273 2c0d  lot_stat(years,.
-00003870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003880: 2020 205b 7374 6174 5f64 6963 5b79 6561     [stat_dic[yea
-00003890: 725d 2e73 6f72 7469 655f 6469 6d61 6e63  r].sortie_dimanc
-000038a0: 6865 5f63 6c75 6220 666f 7220 7965 6172  he_club for year
-000038b0: 2069 6e20 7965 6172 735d 2c0d 0a20 2020   in years],..   
-000038c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000038d0: 7970 652c 0d0a 2020 2020 2020 2020 2020  ype,..          
-000038e0: 2020 2020 2020 2020 2723 7061 7274 6963          '#partic
-000038f0: 6970 616e 7473 2729 0d0a 2020 2020 656c  ipants')..    el
-00003900: 6966 2020 7479 7065 203d 3d20 2773 6f72  if  type == 'sor
-00003910: 7469 655f 7361 6d65 6469 5f63 6c75 6227  tie_samedi_club'
-00003920: 3a0d 0a20 2020 2020 2020 2070 6c6f 745f  :..        plot_
-00003930: 7374 6174 2879 6561 7273 2c0d 0a20 2020  stat(years,..   
-00003940: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00003950: 7374 6174 5f64 6963 5b79 6561 725d 2e73  stat_dic[year].s
-00003960: 6f72 7469 655f 7361 6d65 6469 5f63 6c75  ortie_samedi_clu
-00003970: 6220 666f 7220 7965 6172 2069 6e20 7965  b for year in ye
-00003980: 6172 735d 2c0d 0a20 2020 2020 2020 2020  ars],..         
-00003990: 2020 2020 2020 2020 2074 7970 652c 0d0a           type,..
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039b0: 2020 2723 7061 7274 6963 6970 616e 7473    '#participants
-000039c0: 2729 0d0a 2020 2020 656c 6966 2020 7479  ')..    elif  ty
-000039d0: 7065 203d 3d20 2773 6f72 7469 655f 6a65  pe == 'sortie_je
-000039e0: 7564 695f 636c 7562 273a 0d0a 2020 2020  udi_club':..    
-000039f0: 2020 2020 706c 6f74 5f73 7461 7428 7965      plot_stat(ye
-00003a00: 6172 732c 0d0a 2020 2020 2020 2020 2020  ars,..          
-00003a10: 2020 2020 2020 2020 5b73 7461 745f 6469          [stat_di
-00003a20: 635b 7965 6172 5d2e 736f 7274 6965 5f6a  c[year].sortie_j
-00003a30: 6575 6469 5f63 6c75 6220 666f 7220 7965  eudi_club for ye
-00003a40: 6172 2069 6e20 7965 6172 735d 2c0d 0a20  ar in years],.. 
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a60: 2074 7970 652c 0d0a 2020 2020 2020 2020   type,..        
-00003a70: 2020 2020 2020 2020 2020 2723 7061 7274            '#part
-00003a80: 6963 6970 616e 7473 2729 2020 0d0a 2020  icipants')  ..  
-00003a90: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
-00003aa0: 2772 616e 646f 6e6e 6565 273a 0d0a 2020  'randonnee':..  
-00003ab0: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
-00003ac0: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
-00003ad0: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
-00003ae0: 6469 635b 7965 6172 5d2e 7261 6e64 6f6e  dic[year].randon
-00003af0: 6e65 6520 666f 7220 7965 6172 2069 6e20  nee for year in 
-00003b00: 7965 6172 735d 2c0d 0a20 2020 2020 2020  years],..       
-00003b10: 2020 2020 2020 2020 2020 2074 7970 652c             type,
-00003b20: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003b30: 2020 2020 2723 7061 7274 6963 6970 616e      '#participan
-00003b40: 7473 2729 2020 0d0a 2020 2020 656c 6966  ts')  ..    elif
-00003b50: 2020 7479 7065 203d 3d20 276e 6272 5f70    type == 'nbr_p
-00003b60: 6172 7469 6369 7061 7469 6f6e 735f 7365  articipations_se
-00003b70: 6a6f 7572 7327 3a0d 0a20 2020 2020 2020  jours':..       
-00003b80: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
-00003b90: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00003ba0: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
-00003bb0: 6561 725d 2e6e 6272 5f70 6172 7469 6369  ear].nbr_partici
-00003bc0: 7061 7469 6f6e 735f 7365 6a6f 7572 7320  pations_sejours 
-00003bd0: 666f 7220 7965 6172 2069 6e20 7965 6172  for year in year
-00003be0: 735d 2c0d 0a20 2020 2020 2020 2020 2020  s],..           
-00003bf0: 2020 2020 2020 2027 4e6f 6d62 7265 2064         'Nombre d
-00003c00: 6520 7061 7274 6963 6970 6174 696f 6e73  e participations
-00003c10: 2061 7578 2073 c3a9 6a6f 7572 7327 2c0d   aux s..jours',.
-00003c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003c30: 2020 2027 2320 7061 7274 6963 6970 6174     '# participat
-00003c40: 696f 6e73 2061 7578 2073 c3a9 6a6f 7572  ions aux s..jour
-00003c50: 7327 2920 0d0a 2020 2020 656c 6966 2020  s') ..    elif  
-00003c60: 7479 7065 203d 3d20 276e 6272 5f73 656a  type == 'nbr_sej
-00003c70: 6f75 7273 273a 0d0a 2020 2020 2020 2020  ours':..        
-00003c80: 706c 6f74 5f73 7461 7428 7965 6172 732c  plot_stat(years,
-00003c90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00003ca0: 2020 2020 5b73 7461 745f 6469 635b 7965      [stat_dic[ye
-00003cb0: 6172 5d2e 6e62 725f 7365 6a6f 7572 7320  ar].nbr_sejours 
-00003cc0: 666f 7220 7965 6172 2069 6e20 7965 6172  for year in year
-00003cd0: 735d 2c0d 0a20 2020 2020 2020 2020 2020  s],..           
-00003ce0: 2020 2020 2020 2027 4e6f 6d62 7265 2064         'Nombre d
-00003cf0: 6520 73c3 a96a 6f75 7273 272c 0d0a 2020  e s..jours',..  
-00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2723 2073 c3a9 6a6f 7572 7327 290d 0a20  '# s..jours').. 
-00003d20: 2020 2065 6c69 6620 2074 7970 6520 3d3d     elif  type ==
-00003d30: 2027 6e62 725f 6a6f 7572 735f 7365 6a6f   'nbr_jours_sejo
-00003d40: 7572 7327 3a0d 0a20 2020 2020 2020 2070  urs':..        p
-00003d50: 6c6f 745f 7374 6174 2879 6561 7273 2c0d  lot_stat(years,.
-00003d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003d70: 2020 205b 7374 6174 5f64 6963 5b79 6561     [stat_dic[yea
-00003d80: 725d 2e6e 6272 5f6a 6f75 7273 5f73 656a  r].nbr_jours_sej
-00003d90: 6f75 7273 2066 6f72 2079 6561 7220 696e  ours for year in
-00003da0: 2079 6561 7273 5d2c 0d0a 2020 2020 2020   years],..      
-00003db0: 2020 2020 2020 2020 2020 2020 274e 6f6d              'Nom
-00003dc0: 6272 6520 6465 206a 6f75 7273 2073 c3a9  bre de jours s..
-00003dd0: 6a6f 7572 7327 2c0d 0a20 2020 2020 2020  jours',..       
-00003de0: 2020 2020 2020 2020 2020 2027 2320 6a6f             '# jo
-00003df0: 7572 7320 73c3 a96a 6f75 7227 2920 2020  urs s..jour')   
-00003e00: 2020 2020 20                                  
+00002de0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+00002df0: 7965 6172 732e 6170 7065 6e64 2873 7472  years.append(str
+00002e00: 2879 6561 7229 290d 0a20 2020 2020 2020  (year))..       
+00002e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002e20: 2020 2020 2020 2020 200d 0a20 2020 2064           ..    d
+00002e30: 6566 2066 696c 6c5f 7374 6174 5f79 6561  ef fill_stat_yea
+00002e40: 7228 7965 6172 293a 0d0a 2020 2020 0d0a  r(year):..    ..
+00002e50: 2020 2020 2020 2020 2320 496e 7465 726e          # Intern
+00002e60: 616c 206c 6962 7261 7279 2069 6d70 6f72  al library impor
+00002e70: 7473 0d0a 2020 2020 2020 2020 6672 6f6d  ts..        from
+00002e80: 2043 5447 5f55 7469 6c73 2e43 5447 5f46   CTG_Utils.CTG_F
+00002e90: 756e 632e 4354 475f 7574 696c 6974 7920  unc.CTG_utility 
+00002ea0: 696d 706f 7274 2067 6574 5f73 656a 6f75  import get_sejou
+00002eb0: 725f 696e 666f 0d0a 2020 2020 2020 2020  r_info..        
+00002ec0: 0d0a 2020 2020 2020 2020 7365 6a6f 7572  ..        sejour
+00002ed0: 5f69 6e66 6f20 3d20 6765 745f 7365 6a6f  _info = get_sejo
+00002ee0: 7572 5f69 6e66 6f28 6374 675f 7061 7468  ur_info(ctg_path
+00002ef0: 2c79 6561 7229 0d0a 2020 2020 2020 2020  ,year)..        
+00002f00: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00002f10: 2020 2020 6669 6c65 5f69 6e20 3d20 6374      file_in = ct
+00002f20: 675f 7061 7468 202f 2050 6174 6828 7374  g_path / Path(st
+00002f30: 7228 7965 6172 2929 202f 2050 6174 6828  r(year)) / Path(
+00002f40: 2753 5441 5449 5354 4951 5545 5327 2920  'STATISTIQUES') 
+00002f50: 2f20 5061 7468 2827 7379 6e74 6865 7365  / Path('synthese
+00002f60: 5f61 6468 6572 656e 742e 786c 7378 2729  _adherent.xlsx')
+00002f70: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00002f80: 2020 2020 6466 203d 2070 642e 7265 6164      df = pd.read
+00002f90: 5f65 7863 656c 2866 696c 655f 696e 290d  _excel(file_in).
+00002fa0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
+00002fb0: 2020 2073 7461 745f 7965 6172 203d 2073     stat_year = s
+00002fc0: 7461 7479 6561 7228 6466 5b27 4e62 725f  tatyear(df['Nbr_
+00002fd0: 5345 4a4f 5552 5327 5d2e 7375 6d28 292c  SEJOURS'].sum(),
+00002fe0: 2020 2020 2020 2020 2020 2020 2023 206e               # n
+00002ff0: 6272 5f6a 6f75 7273 5f70 6172 7469 6369  br_jours_partici
+00003000: 7061 7469 6f6e 5f73 656a 6f75 7273 0d0a  pation_sejours..
+00003010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003020: 2020 2020 2020 2020 2020 2020 2064 665b               df[
+00003030: 2753 454a 4f55 522d 4a4f 5552 275d 2e73  'SEJOUR-JOUR'].s
+00003040: 756d 2829 2c20 2020 2020 2020 2020 2020  um(),           
+00003050: 2020 2320 6e62 725f 7061 7274 6963 6970    # nbr_particip
+00003060: 6174 696f 6e73 5f73 656a 6f75 720d 0a20  ations_sejour.. 
+00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003080: 2020 2020 2020 2020 2020 2020 6466 5b27              df['
+00003090: 534f 5254 4945 2044 5520 4449 4d41 4e43  SORTIE DU DIMANC
+000030a0: 4845 2043 4c55 4227 5d2e 7375 6d28 292c  HE CLUB'].sum(),
+000030b0: 2023 2073 6f72 7469 655f 6469 6d61 6e63   # sortie_dimanc
+000030c0: 6865 5f63 6c75 620d 0a20 2020 2020 2020  he_club..       
+000030d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000030e0: 2020 2020 2020 6466 5b27 534f 5254 4945        df['SORTIE
+000030f0: 2044 5520 5341 4d45 4449 2043 4c55 4227   DU SAMEDI CLUB'
+00003100: 5d2e 7375 6d28 292c 2020 2023 2073 6f72  ].sum(),   # sor
+00003110: 7469 655f 7361 6d65 6469 5f63 6c75 620d  tie_samedi_club.
+00003120: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003130: 2020 2020 2020 2020 2020 2020 2020 6466                df
+00003140: 5b27 534f 5254 4945 2048 4956 4552 275d  ['SORTIE HIVER']
+00003150: 2e73 756d 2829 2c20 2020 2020 2020 2020  .sum(),         
+00003160: 2020 2023 2073 6f72 7469 655f 6869 7665     # sortie_hive
+00003170: 725f 636c 7562 0d0a 2020 2020 2020 2020  r_club..        
+00003180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003190: 2020 2020 2064 665b 2753 4f52 5449 4520       df['SORTIE 
+000031a0: 4455 204a 4555 4449 2043 4c55 4227 5d2e  DU JEUDI CLUB'].
+000031b0: 7375 6d28 292c 2020 2020 2320 736f 7274  sum(),    # sort
+000031c0: 6965 5f6a 6575 6469 5f63 6c75 620d 0a20  ie_jeudi_club.. 
+000031d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031e0: 2020 2020 2020 2020 2020 2020 6466 5b27              df['
+000031f0: 5241 4e44 4f4e 4e45 4527 5d2e 7375 6d28  RANDONNEE'].sum(
+00003200: 292c 2020 2020 2020 2020 2020 2020 2020  ),              
+00003210: 2023 2072 616e 646f 6e6e 6565 0d0a 2020   # randonnee..  
+00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003230: 2020 2020 2020 2020 2020 2073 656a 6f75             sejou
+00003240: 725f 696e 666f 2e6e 6272 5f73 656a 6f75  r_info.nbr_sejou
+00003250: 7273 2c20 2020 2020 2020 2020 2020 2020  rs,             
+00003260: 2320 6e62 725f 7365 6a6f 7572 7320 0d0a  # nbr_sejours ..
+00003270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003280: 2020 2020 2020 2020 2020 2020 2073 656a               sej
+00003290: 6f75 725f 696e 666f 2e6e 6272 5f6a 6f75  our_info.nbr_jou
+000032a0: 7273 2920 2020 2020 2020 2020 2020 2020  rs)             
+000032b0: 2020 2320 6e62 725f 6a6f 7572 735f 7365    # nbr_jours_se
+000032c0: 6a6f 7572 7320 2020 2020 2020 2020 2020  jours           
+000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032e0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003300: 2020 0d0a 2020 2020 2020 2020 7265 7475    ..        retu
+00003310: 726e 2073 7461 745f 7965 6172 0d0a 2020  rn stat_year..  
+00003320: 2020 0d0a 2020 2020 6465 6620 6164 646c    ..    def addl
+00003330: 6162 656c 7328 782c 792c 6f66 6673 6574  abels(x,y,offset
+00003340: 293a 0d0a 2020 2020 2020 2020 666f 7220  ):..        for 
+00003350: 6920 696e 2072 616e 6765 286c 656e 2878  i in range(len(x
+00003360: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
+00003370: 2070 6c74 2e74 6578 7428 785b 695d 2c79   plt.text(x[i],y
+00003380: 5b69 5d2b 6f66 6673 6574 2c72 6f75 6e64  [i]+offset,round
+00003390: 2879 5b69 5d2c 3129 2c73 697a 653d 3130  (y[i],1),size=10
+000033a0: 290d 0a20 2020 2020 2020 2020 2020 200d  )..            .
+000033b0: 0a20 2020 2064 6566 2070 6c6f 745f 7374  .    def plot_st
+000033c0: 6174 2879 6561 7273 2c6e 625f 7061 7274  at(years,nb_part
+000033d0: 6963 6970 616e 7473 2c74 6974 6c65 2c6c  icipants,title,l
+000033e0: 6162 656c 5f79 293a 0d0a 2020 2020 2020  abel_y):..      
+000033f0: 2020 706c 742e 6669 6775 7265 2866 6967    plt.figure(fig
+00003400: 7369 7a65 3d28 382c 2036 2929 0d0a 2020  size=(8, 6))..  
+00003410: 2020 2020 2020 636f 6c6f 7273 203d 205b        colors = [
+00003420: 2723 6664 6161 3438 275d 200d 0a20 2020  '#fdaa48'] ..   
+00003430: 2020 2020 2073 697a 655f 6c61 6265 6c20       size_label 
+00003440: 3d20 3230 0d0a 2020 2020 2020 2020 706c  = 20..        pl
+00003450: 742e 6261 7228 7965 6172 732c 6e62 5f70  t.bar(years,nb_p
+00003460: 6172 7469 6369 7061 6e74 732c 636f 6c6f  articipants,colo
+00003470: 723d 636f 6c6f 7273 290d 0a20 2020 2020  r=colors)..     
+00003480: 2020 2070 6c74 2e79 6c61 6265 6c28 6c61     plt.ylabel(la
+00003490: 6265 6c5f 792c 7369 7a65 3d73 697a 655f  bel_y,size=size_
+000034a0: 6c61 6265 6c29 0d0a 2020 2020 2020 2020  label)..        
+000034b0: 6164 646c 6162 656c 7328 7965 6172 732c  addlabels(years,
+000034c0: 6e62 5f70 6172 7469 6369 7061 6e74 732c  nb_participants,
+000034d0: 3129 0d0a 2020 2020 2020 2020 706c 742e  1)..        plt.
+000034e0: 7874 6963 6b73 2872 6f74 6174 696f 6e3d  xticks(rotation=
+000034f0: 3930 290d 0a20 2020 2020 2020 2070 6c74  90)..        plt
+00003500: 2e74 6963 6b5f 7061 7261 6d73 2861 7869  .tick_params(axi
+00003510: 733d 2778 272c 206c 6162 656c 7369 7a65  s='x', labelsize
+00003520: 3d73 697a 655f 6c61 6265 6c29 0d0a 2020  =size_label)..  
+00003530: 2020 2020 2020 706c 742e 7469 636b 5f70        plt.tick_p
+00003540: 6172 616d 7328 6178 6973 3d27 7927 2c20  arams(axis='y', 
+00003550: 6c61 6265 6c73 697a 653d 7369 7a65 5f6c  labelsize=size_l
+00003560: 6162 656c 290d 0a20 2020 2020 2020 2070  abel)..        p
+00003570: 6c74 2e74 6974 6c65 2874 6974 6c65 2c66  lt.title(title,f
+00003580: 6f6e 7473 697a 653d 3138 290d 0a20 2020  ontsize=18)..   
+00003590: 2020 2020 2070 6c74 2e74 6967 6874 5f6c       plt.tight_l
+000035a0: 6179 6f75 7428 290d 0a20 2020 2020 2020  ayout()..       
+000035b0: 2070 6c74 2e73 686f 7728 290d 0a20 2020   plt.show()..   
+000035c0: 200d 0a20 2020 2073 7461 7479 6561 7220   ..    statyear 
+000035d0: 3d20 6e61 6d65 6474 7570 6c65 2827 6163  = namedtuple('ac
+000035e0: 7469 7669 7465 272c 2041 4354 4956 4954  tivite', ACTIVIT
+000035f0: 455f 4c49 5354 290d 0a20 0d0a 2020 2020  E_LIST).. ..    
+00003600: 706c 742e 7374 796c 652e 7573 6528 2767  plt.style.use('g
+00003610: 6770 6c6f 7427 290d 0a20 2020 2079 6561  gplot')..    yea
+00003620: 7273 203d 205b 5d0d 0a20 2020 2073 7461  rs = []..    sta
+00003630: 745f 6469 6320 3d20 7b7d 0d0a 2020 2020  t_dic = {}..    
+00003640: 6164 645f 6d65 6d6f 7279 2873 7461 745f  add_memory(stat_
+00003650: 6469 632c 7965 6172 7329 0d0a 0d0a 2020  dic,years)....  
+00003660: 2020 746f 6461 7920 3d20 6461 7465 7469    today = dateti
+00003670: 6d65 2e64 6174 6574 696d 652e 6e6f 7728  me.datetime.now(
+00003680: 290d 0a20 2020 2079 6561 7273 5f6e 6577  )..    years_new
+00003690: 203d 205b 7374 7228 7965 6172 2920 666f   = [str(year) fo
+000036a0: 7220 7965 6172 2069 6e20 7261 6e67 6528  r year in range(
+000036b0: 3230 3232 2c74 6f64 6179 2e79 6561 722b  2022,today.year+
+000036c0: 3129 5d0d 0a20 2020 2066 6f72 2079 6561  1)]..    for yea
+000036d0: 7220 696e 2079 6561 7273 5f6e 6577 3a0d  r in years_new:.
+000036e0: 0a20 2020 2020 2020 2073 7461 745f 6469  .        stat_di
+000036f0: 635b 7965 6172 5d20 3d20 6669 6c6c 5f73  c[year] = fill_s
+00003700: 7461 745f 7965 6172 2879 6561 7229 0d0a  tat_year(year)..
+00003710: 2020 2020 2020 2020 0d0a 2020 2020 7965          ..    ye
+00003720: 6172 7320 3d20 7965 6172 7320 2b20 7965  ars = years + ye
+00003730: 6172 735f 6e65 7720 2020 0d0a 2020 2020  ars_new   ..    
+00003740: 0d0a 2020 2020 0d0a 2020 2020 6966 2074  ..    ..    if t
+00003750: 7970 6520 3d3d 2027 6e62 725f 6a6f 7572  ype == 'nbr_jour
+00003760: 735f 7061 7274 6963 6970 6174 696f 6e5f  s_participation_
+00003770: 7365 6a6f 7572 7327 3a0d 0a20 2020 2020  sejours':..     
+00003780: 2020 2070 6c6f 745f 7374 6174 2879 6561     plot_stat(yea
+00003790: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
+000037a0: 2020 2020 2020 205b 7374 6174 5f64 6963         [stat_dic
+000037b0: 5b79 6561 725d 2e6e 6272 5f6a 6f75 7273  [year].nbr_jours
+000037c0: 5f70 6172 7469 6369 7061 7469 6f6e 5f73  _participation_s
+000037d0: 656a 6f75 7273 2066 6f72 2079 6561 7220  ejours for year 
+000037e0: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
+000037f0: 2020 2020 2020 2020 2020 2020 2020 7479                ty
+00003800: 7065 2c0d 0a20 2020 2020 2020 2020 2020  pe,..           
+00003810: 2020 2020 2020 2074 7970 6529 0d0a 2020         type)..  
+00003820: 2020 656c 6966 2020 7479 7065 203d 3d20    elif  type == 
+00003830: 2773 6f72 7469 655f 6469 6d61 6e63 6865  'sortie_dimanche
+00003840: 5f63 6c75 6227 3a0d 0a20 2020 2020 2020  _club':..       
+00003850: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
+00003860: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003870: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
+00003880: 6561 725d 2e73 6f72 7469 655f 6469 6d61  ear].sortie_dima
+00003890: 6e63 6865 5f63 6c75 6220 666f 7220 7965  nche_club for ye
+000038a0: 6172 2069 6e20 7965 6172 735d 2c0d 0a20  ar in years],.. 
+000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038c0: 2074 7970 652c 0d0a 2020 2020 2020 2020   type,..        
+000038d0: 2020 2020 2020 2020 2020 2723 7061 7274            '#part
+000038e0: 6963 6970 616e 7473 2729 0d0a 2020 2020  icipants')..    
+000038f0: 656c 6966 2020 7479 7065 203d 3d20 2773  elif  type == 's
+00003900: 6f72 7469 655f 7361 6d65 6469 5f63 6c75  ortie_samedi_clu
+00003910: 6227 3a0d 0a20 2020 2020 2020 2070 6c6f  b':..        plo
+00003920: 745f 7374 6174 2879 6561 7273 2c0d 0a20  t_stat(years,.. 
+00003930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003940: 205b 7374 6174 5f64 6963 5b79 6561 725d   [stat_dic[year]
+00003950: 2e73 6f72 7469 655f 7361 6d65 6469 5f63  .sortie_samedi_c
+00003960: 6c75 6220 666f 7220 7965 6172 2069 6e20  lub for year in 
+00003970: 7965 6172 735d 2c0d 0a20 2020 2020 2020  years],..       
+00003980: 2020 2020 2020 2020 2020 2074 7970 652c             type,
+00003990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000039a0: 2020 2020 2723 7061 7274 6963 6970 616e      '#participan
+000039b0: 7473 2729 0d0a 2020 2020 656c 6966 2020  ts')..    elif  
+000039c0: 7479 7065 203d 3d20 2773 6f72 7469 655f  type == 'sortie_
+000039d0: 6a65 7564 695f 636c 7562 273a 0d0a 2020  jeudi_club':..  
+000039e0: 2020 2020 2020 706c 6f74 5f73 7461 7428        plot_stat(
+000039f0: 7965 6172 732c 0d0a 2020 2020 2020 2020  years,..        
+00003a00: 2020 2020 2020 2020 2020 5b73 7461 745f            [stat_
+00003a10: 6469 635b 7965 6172 5d2e 736f 7274 6965  dic[year].sortie
+00003a20: 5f6a 6575 6469 5f63 6c75 6220 666f 7220  _jeudi_club for 
+00003a30: 7965 6172 2069 6e20 7965 6172 735d 2c0d  year in years],.
+00003a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003a50: 2020 2074 7970 652c 0d0a 2020 2020 2020     type,..      
+00003a60: 2020 2020 2020 2020 2020 2020 2723 7061              '#pa
+00003a70: 7274 6963 6970 616e 7473 2729 2020 0d0a  rticipants')  ..
+00003a80: 2020 2020 656c 6966 2020 7479 7065 203d      elif  type =
+00003a90: 3d20 2772 616e 646f 6e6e 6565 273a 0d0a  = 'randonnee':..
+00003aa0: 2020 2020 2020 2020 706c 6f74 5f73 7461          plot_sta
+00003ab0: 7428 7965 6172 732c 0d0a 2020 2020 2020  t(years,..      
+00003ac0: 2020 2020 2020 2020 2020 2020 5b73 7461              [sta
+00003ad0: 745f 6469 635b 7965 6172 5d2e 7261 6e64  t_dic[year].rand
+00003ae0: 6f6e 6e65 6520 666f 7220 7965 6172 2069  onnee for year i
+00003af0: 6e20 7965 6172 735d 2c0d 0a20 2020 2020  n years],..     
+00003b00: 2020 2020 2020 2020 2020 2020 2074 7970               typ
+00003b10: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+00003b20: 2020 2020 2020 2723 7061 7274 6963 6970        '#particip
+00003b30: 616e 7473 2729 2020 0d0a 2020 2020 656c  ants')  ..    el
+00003b40: 6966 2020 7479 7065 203d 3d20 276e 6272  if  type == 'nbr
+00003b50: 5f70 6172 7469 6369 7061 7469 6f6e 735f  _participations_
+00003b60: 7365 6a6f 7572 7327 3a0d 0a20 2020 2020  sejours':..     
+00003b70: 2020 2070 6c6f 745f 7374 6174 2879 6561     plot_stat(yea
+00003b80: 7273 2c0d 0a20 2020 2020 2020 2020 2020  rs,..           
+00003b90: 2020 2020 2020 205b 7374 6174 5f64 6963         [stat_dic
+00003ba0: 5b79 6561 725d 2e6e 6272 5f70 6172 7469  [year].nbr_parti
+00003bb0: 6369 7061 7469 6f6e 735f 7365 6a6f 7572  cipations_sejour
+00003bc0: 7320 666f 7220 7965 6172 2069 6e20 7965  s for year in ye
+00003bd0: 6172 735d 2c0d 0a20 2020 2020 2020 2020  ars],..         
+00003be0: 2020 2020 2020 2020 2027 4e6f 6d62 7265           'Nombre
+00003bf0: 2064 6520 7061 7274 6963 6970 6174 696f   de participatio
+00003c00: 6e73 2061 7578 2073 c3a9 6a6f 7572 7327  ns aux s..jours'
+00003c10: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003c20: 2020 2020 2027 2320 7061 7274 6963 6970       '# particip
+00003c30: 6174 696f 6e73 2061 7578 2073 c3a9 6a6f  ations aux s..jo
+00003c40: 7572 7327 2920 0d0a 2020 2020 656c 6966  urs') ..    elif
+00003c50: 2020 7479 7065 203d 3d20 276e 6272 5f73    type == 'nbr_s
+00003c60: 656a 6f75 7273 273a 0d0a 2020 2020 2020  ejours':..      
+00003c70: 2020 706c 6f74 5f73 7461 7428 7965 6172    plot_stat(year
+00003c80: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
+00003c90: 2020 2020 2020 5b73 7461 745f 6469 635b        [stat_dic[
+00003ca0: 7965 6172 5d2e 6e62 725f 7365 6a6f 7572  year].nbr_sejour
+00003cb0: 7320 666f 7220 7965 6172 2069 6e20 7965  s for year in ye
+00003cc0: 6172 735d 2c0d 0a20 2020 2020 2020 2020  ars],..         
+00003cd0: 2020 2020 2020 2020 2027 4e6f 6d62 7265           'Nombre
+00003ce0: 2064 6520 73c3 a96a 6f75 7273 272c 0d0a   de s..jours',..
+00003cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d00: 2020 2723 2073 c3a9 6a6f 7572 7327 290d    '# s..jours').
+00003d10: 0a20 2020 2065 6c69 6620 2074 7970 6520  .    elif  type 
+00003d20: 3d3d 2027 6e62 725f 6a6f 7572 735f 7365  == 'nbr_jours_se
+00003d30: 6a6f 7572 7327 3a0d 0a20 2020 2020 2020  jours':..       
+00003d40: 2070 6c6f 745f 7374 6174 2879 6561 7273   plot_stat(years
+00003d50: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00003d60: 2020 2020 205b 7374 6174 5f64 6963 5b79       [stat_dic[y
+00003d70: 6561 725d 2e6e 6272 5f6a 6f75 7273 5f73  ear].nbr_jours_s
+00003d80: 656a 6f75 7273 2066 6f72 2079 6561 7220  ejours for year 
+00003d90: 696e 2079 6561 7273 5d2c 0d0a 2020 2020  in years],..    
+00003da0: 2020 2020 2020 2020 2020 2020 2020 274e                'N
+00003db0: 6f6d 6272 6520 6465 206a 6f75 7273 2073  ombre de jours s
+00003dc0: c3a9 6a6f 7572 7327 2c0d 0a20 2020 2020  ..jours',..     
+00003dd0: 2020 2020 2020 2020 2020 2020 2027 2320               '# 
+00003de0: 6a6f 7572 7320 73c3 a96a 6f75 7227 2920  jours s..jour') 
+00003df0: 2020 2020 2020 20
```

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_Func/CTG_utility.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_Func/CTG_utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,41 +108,33 @@
 def yamlinfo_randos2df(ctg_path,year):
     
     # Standard library imports
     import os
     from pathlib import Path
 
     # 3rd party imports
-    import yaml
     import pandas as pd
     
     # Reads the yaml file
-    yaml_path = ctg_path / Path(str(year)) / Path('DATA') / Path('info_randos.yaml')
+    info_path = ctg_path / Path(str(year)) / Path('DATA') / Path('info_randos.xlsx')
     
-    with open(yaml_path,  'r' ) as file:
-        yaml_content = yaml.safe_load(file)
     
-    df = pd.DataFrame.from_dict(yaml_content['INFO_RANDO']).T
-    df = df.rename(columns={0:'name_activite',
-                            1:'color',
-                            2:'type',
-                            3:'nbr_jours'})
-
+    df = pd.read_excel(info_path)
     
     return df
     
 def get_sejour_info(ctg_path,year):
 
     # Standard library imports 
     from collections import namedtuple
     from collections import Counter
     
     sejour_info = namedtuple('sejour_info', 'nbr_jours nbr_sejours histo')
     df =  yamlinfo_randos2df(ctg_path,year)
-    info_sejour = [nbr_jours for nbr_jours in df['nbr_jours'] if nbr_jours>1]
+    info_sejour = df.query('type=="sejour"')['nbr_jours'].tolist()
     
     c = Counter()
     c = Counter(info_sejour)
 
     
     sejour_info_tup = sejour_info( sum(info_sejour),len(info_sejour),c)
```

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/GUI_Globals.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/GUI_Globals.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageDivers.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageDivers.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageEffectif.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageEffectif.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageSorties.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageSorties.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from pathlib import Path
     from tkinter import messagebox
     
     # Local imports
     from CTG_Utils.CTG_Func.CTG_plot import stat_sorties_club
     
     path_sorties =  ctg_path / Path(str(year)) / Path(type_sortie)
-    file_label =  ctg_path / Path(str(year)) / Path(r'DATA/info_randos.yaml')    
+    file_label =  ctg_path / Path(str(year)) / Path(r'DATA/info_randos.xlsx')    
     df_total = stat_sorties_club(path_sorties,ctg_path,None,file_label,year)
     
     
     #info_title = "- Information -"
     #info_text  = f"L'analyse des IFs a été effectuée pour l'année {year_select} "
     #info_text += f"avec les valeurs {analysis_if}. "
     #info_text += f"\n\nLes fichiers obtenus ont été créés dans le dossier :"
```

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageSynthese.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageSynthese.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/PageTendance.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/PageTendance.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/Page_Classes.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Page_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/Useful_Classes.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Useful_Classes.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils/CTG_GUI/Useful_Functions.py` & `CTG_Utils-1.1.5/CTG_Utils/CTG_GUI/Useful_Functions.py`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/CTG_Utils.egg-info/PKG-INFO` & `CTG_Utils-1.1.5/CTG_Utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG-Utils
-Version: 1.1.4
+Version: 1.1.5
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.4/CTG_Utils.egg-info/SOURCES.txt` & `CTG_Utils-1.1.5/CTG_Utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/LICENSE` & `CTG_Utils-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CTG_Utils-1.1.4/PKG-INFO` & `CTG_Utils-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTG_Utils
-Version: 1.1.4
+Version: 1.1.5
 Summary: A toolbox for ctg statistics analysis
 Home-page: https://github.com/Bertin-fap/CTG_Utils 
 Author: f. bertin
 Author-email: francois.bertin7@wanadoo.fr
 License: MIT
 Keywords: ffvelo,ctg
 Platform: UNKNOWN
```

### Comparing `CTG_Utils-1.1.4/setup.py` & `CTG_Utils-1.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     long_description = f.read()
 
 install_requires = open(path.join(this_directory, 'requirements.txt'), encoding='utf-8').read().strip().split('\n') 
 
 # This setup is suitable for "python setup.py develop".
 
 setup(name='CTG_Utils',
-      version='1.1.4',
+      version='1.1.5',
       description='A toolbox for ctg statistics analysis',
       long_description=long_description,
       long_description_content_type='text/markdown',
       include_package_data = True,
       license = 'MIT',
       classifiers = [
         'Development Status :: 4 - Beta',
```

