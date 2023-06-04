# Comparing `tmp/leuci-geo-0.0.2.tar.gz` & `tmp/leuci-geo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leuci-geo-0.0.2.tar", last modified: Sun Jun  4 14:01:08 2023, max compression
+gzip compressed data, was "leuci-geo-0.0.3.tar", last modified: Sun Jun  4 18:18:02 2023, max compression
```

## Comparing `leuci-geo-0.0.2.tar` & `leuci-geo-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 14:01:08.490136 leuci-geo-0.0.2/
--rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.2/LICENSE
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-04 14:01:08.490136 leuci-geo-0.0.2/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.2/README.md
--rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.2/pyproject.toml
--rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-06-04 14:01:08.490136 leuci-geo-0.0.2/setup.cfg
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 14:01:08.480136 leuci-geo-0.0.2/src/
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 14:01:08.480136 leuci-geo-0.0.2/src/leuci_geo/
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.2/src/leuci_geo/__init__.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     2963 2023-05-29 13:51:47.000000 leuci-geo-0.0.2/src/leuci_geo/geocalculator.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)    27001 2023-06-04 13:12:00.000000 leuci-geo-0.0.2/src/leuci_geo/pdbgeometry.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     2844 2023-05-29 13:40:46.000000 leuci-geo-0.0.2/src/leuci_geo/pdbloader.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)     9405 2023-06-04 13:05:42.000000 leuci-geo-0.0.2/src/leuci_geo/pdbobject.py
--rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-05-29 10:54:24.000000 leuci-geo-0.0.2/src/leuci_geo/pdbspace.py
-drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 14:01:08.490136 leuci-geo-0.0.2/src/leuci_geo.egg-info/
--rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-04 14:01:08.000000 leuci-geo-0.0.2/src/leuci_geo.egg-info/PKG-INFO
--rw-r--r--   0 rachel    (1000) rachel    (1000)      356 2023-06-04 14:01:08.000000 leuci-geo-0.0.2/src/leuci_geo.egg-info/SOURCES.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-06-04 14:01:08.000000 leuci-geo-0.0.2/src/leuci_geo.egg-info/dependency_links.txt
--rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-06-04 14:01:08.000000 leuci-geo-0.0.2/src/leuci_geo.egg-info/top_level.txt
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 18:18:02.247368 leuci-geo-0.0.3/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    35149 2023-05-25 20:00:31.000000 leuci-geo-0.0.3/LICENSE
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-04 18:18:02.247368 leuci-geo-0.0.3/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       22 2023-05-25 20:00:31.000000 leuci-geo-0.0.3/README.md
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      104 2023-02-09 09:20:26.000000 leuci-geo-0.0.3/pyproject.toml
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      656 2023-06-04 18:18:02.247368 leuci-geo-0.0.3/setup.cfg
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 18:18:02.237368 leuci-geo-0.0.3/src/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 18:18:02.237368 leuci-geo-0.0.3/src/leuci_geo/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-02-09 09:20:26.000000 leuci-geo-0.0.3/src/leuci_geo/__init__.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2963 2023-05-29 13:51:47.000000 leuci-geo-0.0.3/src/leuci_geo/geocalculator.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)    27123 2023-06-04 18:16:10.000000 leuci-geo-0.0.3/src/leuci_geo/pdbgeometry.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     2844 2023-05-29 13:40:46.000000 leuci-geo-0.0.3/src/leuci_geo/pdbloader.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     9405 2023-06-04 13:05:42.000000 leuci-geo-0.0.3/src/leuci_geo/pdbobject.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2023-05-29 10:54:24.000000 leuci-geo-0.0.3/src/leuci_geo/pdbspace.py
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2023-06-04 18:18:02.247368 leuci-geo-0.0.3/src/leuci_geo.egg-info/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      553 2023-06-04 18:18:02.000000 leuci-geo-0.0.3/src/leuci_geo.egg-info/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      356 2023-06-04 18:18:02.000000 leuci-geo-0.0.3/src/leuci_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2023-06-04 18:18:02.000000 leuci-geo-0.0.3/src/leuci_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       10 2023-06-04 18:18:02.000000 leuci-geo-0.0.3/src/leuci_geo.egg-info/top_level.txt
```

### Comparing `leuci-geo-0.0.2/LICENSE` & `leuci-geo-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.2/PKG-INFO` & `leuci-geo-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.2
+Version: 0.0.3
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `leuci-geo-0.0.2/setup.cfg` & `leuci-geo-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = leuci-geo
-version = 0.0.2
+version = 0.0.3
 author = Rachel Alcraft
 author_email = rachelalcraft@gmail.com
 description = geometric paramaters and searches of protein structures
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pypa/sampleproject
 project_urls =
```

### Comparing `leuci-geo-0.0.2/src/leuci_geo/geocalculator.py` & `leuci-geo-0.0.3/src/leuci_geo/geocalculator.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.2/src/leuci_geo/pdbgeometry.py` & `leuci-geo-0.0.3/src/leuci_geo/pdbgeometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
         :param geos: A list of geometric measures to calculate in the format 2,3 or 4 atoms for distance, angle or dihedral, e.g. 'N:CA', 'N:CA:C', or 'N:CA:C:N+1'
         :param hues:A list of hues hat will associate with the geoemtric values, can be bfactor, amino acid (aa), residue number (rid) etc see docs
         :returns: the pandas dataframe with a r per geoemtric calculation per residue wh columns of geoemtric measures and hues
         """                        
         geo2 = ["val","blob"]
         vals = []
-        hues=['pdb_code','resolution','aa','rid']        
+        hues=['pdb_code','resolution','aa','chain','rid']        
         for geopdb in self.pobjs:
             hue_pdb = geopdb.pdb_code
             if log > 0:
                 print('leuci-geo(1) df calc for ' + hue_pdb, count, '/', len(self.pobjs))
                 count += 1
 
             hue_res = geopdb.resolution
@@ -58,14 +58,15 @@
                             geo_cols[geo_col].append([val,info,occ,avgbfac])
 
 
                         all_hues = {}
                         all_hues['pdb_code'] = hue_pdb
                         all_hues['resolution'] =hue_res
                         all_hues['aa'] =hue_aa                            
+                        all_hues['chain'] =chain
                         all_hues['rid'] = rid                            
                         
                                                                                                         
                         # a cross product of the geos - using itertools
                         
                         if len(geo_cols) == len(geos):  
                             row_vals = {}                            
@@ -460,24 +461,25 @@
             atom_name = ""
             if "(" in geo_a and ")" in geo_a:
                 atom_type = geo_a[1]
             else:
                 atom_name = geo_a
             res_match = resno + geo_atom[1]
             
-            for chain,resdic in pobj.chains.items():
-                for no,res in resdic.items():
-                    if res.rid == res_match:
-                        for attype,atm in res.atoms.items():
-                            if atm.matchesCriteria(criteria):
-                                if atom_type != "" and atm.atom_type == atom_type:
-                                    atom_starts.append((chain,res,atm))
-                                elif atom_name != "" and atm.atom_name == atom_name:
-                                    atom_starts.append((chain,res,atm))
-                        break
+            for ch,resdic in pobj.chains.items():
+                if ch == chain:
+                    for no,res in resdic.items():
+                        if res.rid == res_match:
+                            for attype,atm in res.atoms.items():
+                                if atm.matchesCriteria(criteria):
+                                    if atom_type != "" and atm.atom_type == atom_type:
+                                        atom_starts.append((chain,res,atm))
+                                    elif atom_name != "" and atm.atom_name == atom_name:
+                                        atom_starts.append((chain,res,atm))
+                            break
         
         return atom_starts
     
     def getMatchingAtoms(self,pobj, resno,chain, res,atom, geo_atom):
         
         need_same_residue = True
         atom_matches = []
```

### Comparing `leuci-geo-0.0.2/src/leuci_geo/pdbloader.py` & `leuci-geo-0.0.3/src/leuci_geo/pdbloader.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.2/src/leuci_geo/pdbobject.py` & `leuci-geo-0.0.3/src/leuci_geo/pdbobject.py`

 * *Files identical despite different names*

### Comparing `leuci-geo-0.0.2/src/leuci_geo.egg-info/PKG-INFO` & `leuci-geo-0.0.3/src/leuci_geo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leuci-geo
-Version: 0.0.2
+Version: 0.0.3
 Summary: geometric paramaters and searches of protein structures
 Home-page: https://github.com/pypa/sampleproject
 Author: Rachel Alcraft
 Author-email: rachelalcraft@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

