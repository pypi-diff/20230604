# Comparing `tmp/pydecs-2023.6.2.tar.gz` & `tmp/pydecs-2023.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydecs-2023.6.2.tar", last modified: Fri Jun  2 11:00:04 2023, max compression
+gzip compressed data, was "pydecs-2023.6.4.tar", last modified: Sun Jun  4 10:40:53 2023, max compression
```

## Comparing `pydecs-2023.6.2.tar` & `pydecs-2023.6.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-06-02 11:00:03.954791 pydecs-2023.6.2/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2023-06-02 10:33:14.000000 pydecs-2023.6.2/LICENSE.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      536 2023-06-02 11:00:03.954791 pydecs-2023.6.2/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2023-06-02 10:33:14.000000 pydecs-2023.6.2/README.md
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-06-02 11:00:03.147533 pydecs-2023.6.2/pydecs/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/__init__.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    34447 2023-06-02 10:51:12.000000 pydecs-2023.6.2/pydecs/aux_EdefCorrection_VASP.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2258 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/aux_check_equilibrium_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     5274 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/aux_convDOS.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/aux_convGasEne.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1792 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/aux_plot_defectdata.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/common.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11528 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/defects.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    18343 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/eqcond.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4946 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/host.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    51639 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/inout.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4506 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/pydecs.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     8513 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/reference_phases.py
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32129 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pydecs/solver.py
-drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-06-02 11:00:03.858086 pydecs-2023.6.2/pydecs.egg-info/
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      536 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/PKG-INFO
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2023-06-02 11:00:01.000000 pydecs-2023.6.2/pydecs.egg-info/SOURCES.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/dependency_links.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/entry_points.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2023-06-02 10:59:59.000000 pydecs-2023.6.2/pydecs.egg-info/not-zip-safe
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/requires.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2023-06-02 11:00:00.000000 pydecs-2023.6.2/pydecs.egg-info/top_level.txt
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2023-06-02 10:33:14.000000 pydecs-2023.6.2/pyproject.toml
--rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2023-06-02 11:00:03.984469 pydecs-2023.6.2/setup.cfg
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-06-04 10:40:53.859078 pydecs-2023.6.4/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11357 2023-06-04 10:06:59.000000 pydecs-2023.6.4/LICENSE.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      536 2023-06-04 10:40:53.859078 pydecs-2023.6.4/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      484 2023-06-04 10:06:59.000000 pydecs-2023.6.4/README.md
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-06-04 10:40:53.444799 pydecs-2023.6.4/pydecs/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      257 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/__init__.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    35232 2023-06-04 10:39:46.000000 pydecs-2023.6.4/pydecs/aux_EdefCorrection_VASP.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     2258 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/aux_check_equilibrium_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     5274 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/aux_convDOS.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1343 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/aux_convGasEne.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1792 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/aux_plot_defectdata.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      671 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/common.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    11528 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/defects.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    18343 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/eqcond.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4946 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/host.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    51639 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/inout.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     4506 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/pydecs.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     8513 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/reference_phases.py
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)    32129 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pydecs/solver.py
+drwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        0 2023-06-04 10:40:53.796580 pydecs-2023.6.4/pydecs.egg-info/
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      536 2023-06-04 10:40:52.000000 pydecs-2023.6.4/pydecs.egg-info/PKG-INFO
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      570 2023-06-04 10:40:52.000000 pydecs-2023.6.4/pydecs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2023-06-04 10:40:52.000000 pydecs-2023.6.4/pydecs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)      420 2023-06-04 10:40:52.000000 pydecs-2023.6.4/pydecs.egg-info/entry_points.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        1 2023-06-04 10:38:52.000000 pydecs-2023.6.4/pydecs.egg-info/not-zip-safe
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       35 2023-06-04 10:40:52.000000 pydecs-2023.6.4/pydecs.egg-info/requires.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)        7 2023-06-04 10:40:52.000000 pydecs-2023.6.4/pydecs.egg-info/top_level.txt
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)       91 2023-06-04 10:06:59.000000 pydecs-2023.6.4/pyproject.toml
+-rwxrwxrwx   0 ogawa     (1000) ogawa     (1000)     1098 2023-06-04 10:40:53.874705 pydecs-2023.6.4/setup.cfg
```

### Comparing `pydecs-2023.6.2/LICENSE.txt` & `pydecs-2023.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/PKG-INFO` & `pydecs-2023.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2023.6.2
+Version: 2023.6.4
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2023.6.2/pydecs/aux_EdefCorrection_VASP.py` & `pydecs-2023.6.4/pydecs/aux_EdefCorrection_VASP.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,16 +40,33 @@
                     e2=l2[2].strip()
                 elems.append(e2)
                 l1=fin.readline()
         if "direct lattice vectors" in l1:
             latt_list=[]
             for i1 in range(3):
                 l1=fin.readline()
-                latt0=[ float(t1) for t1 in l1.split()[:3]]
-                latt_list.append(latt0)
+                # latt0=[ float(t1) for t1 in l1.split()[:3]]
+                latt0=[]
+                for t1 in l1.split()[:3]:
+                    for t2 in t1.split():
+                        if t2.rfind("-")>0:
+                            t3=float(t2[t2.rfind("-"):])
+                            latt0.append(t3)
+                            t3=t2[:t2.rfind("-")]
+                            if t3.rfind("-")>0:
+                                t4=float(t3[t3.rfind("-"):])
+                                latt0.append(t4)
+                                t4=float(t3[:t3.rfind("-")])
+                                latt0.append(t4)
+                            else:
+                                latt0.append(float(t3))
+                        else:
+                            t3=float(t2)
+                            latt0.append(t3)
+                latt_list.append(latt0[:3])
         if "ions per type" in l1:
             natoms=[ int(t1) for t1 in l1.split("=")[-1].split()]
         if "ZVAL" in l1 and l1.find("ZVAL")<10:
             zvals=[ float(t1) for t1 in l1.split("=")[-1].split()]
         if "NELECT" in l1:
             NELECT=float(l1.split()[2])
         if "position of ions in fractional coordinates (direct lattice)" in l1:
```

### Comparing `pydecs-2023.6.2/pydecs/aux_check_equilibrium_phases.py` & `pydecs-2023.6.4/pydecs/aux_check_equilibrium_phases.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/aux_convDOS.py` & `pydecs-2023.6.4/pydecs/aux_convDOS.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/aux_convGasEne.py` & `pydecs-2023.6.4/pydecs/aux_convGasEne.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/aux_plot_defectdata.py` & `pydecs-2023.6.4/pydecs/aux_plot_defectdata.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/common.py` & `pydecs-2023.6.4/pydecs/common.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/defects.py` & `pydecs-2023.6.4/pydecs/defects.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/eqcond.py` & `pydecs-2023.6.4/pydecs/eqcond.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/host.py` & `pydecs-2023.6.4/pydecs/host.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/inout.py` & `pydecs-2023.6.4/pydecs/inout.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/pydecs.py` & `pydecs-2023.6.4/pydecs/pydecs.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/reference_phases.py` & `pydecs-2023.6.4/pydecs/reference_phases.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs/solver.py` & `pydecs-2023.6.4/pydecs/solver.py`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/pydecs.egg-info/PKG-INFO` & `pydecs-2023.6.4/pydecs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydecs
-Version: 2023.6.2
+Version: 2023.6.4
 Summary: This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 Home-page: https://gitlab.com/tkog/pydecs
 Author: Takafumi Ogawa
 Author-email: takafumi.ogawa.1+pydecs@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `pydecs-2023.6.2/pydecs.egg-info/SOURCES.txt` & `pydecs-2023.6.4/pydecs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydecs-2023.6.2/setup.cfg` & `pydecs-2023.6.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pydecs
-version = 2023.06.02
+version = 2023.06.04
 description = This tool enables us to analyze equilibrium concentrations of point and complex defects in crystalline solids
 author = Takafumi Ogawa
 author_email = takafumi.ogawa.1+pydecs@gmail.com
 url = https://gitlab.com/tkog/pydecs
 lisense_file = LICENSE.txt
 classifiers = 
 	Intended Audience :: Science/Research
```

