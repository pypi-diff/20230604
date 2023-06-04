# Comparing `tmp/thunder-ase-0.2.2.tar.gz` & `tmp/thunder-ase-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder-ase-0.2.2.tar", last modified: Mon Mar 27 08:42:26 2023, max compression
+gzip compressed data, was "thunder-ase-0.3.tar", last modified: Sun Jun  4 11:14:44 2023, max compression
```

## Comparing `thunder-ase-0.2.2.tar` & `thunder-ase-0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:42:26.714325 thunder-ase-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-27 08:42:26.714325 thunder-ase-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-27 08:42:14.000000 thunder-ase-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-03-27 08:42:14.000000 thunder-ase-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 08:42:26.714325 thunder-ase-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 08:42:14.000000 thunder-ase-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:42:26.710325 thunder-ase-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-03-27 08:42:14.000000 thunder-ase-0.2.2/tests/test_Si_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:42:26.710325 thunder-ase-0.2.2/thunder_ase/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 08:42:14.000000 thunder-ase-0.2.2/thunder_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24627 2023-03-27 08:42:14.000000 thunder-ase-0.2.2/thunder_ase/fireball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 08:42:26.714325 thunder-ase-0.2.2/thunder_ase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-27 08:42:26.000000 thunder-ase-0.2.2/thunder_ase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-27 08:42:26.000000 thunder-ase-0.2.2/thunder_ase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 08:42:26.000000 thunder-ase-0.2.2/thunder_ase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-27 08:42:26.000000 thunder-ase-0.2.2/thunder_ase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:14:44.042675 thunder-ase-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-04 11:14:44.042675 thunder-ase-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-04 11:14:34.000000 thunder-ase-0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-04 11:14:34.000000 thunder-ase-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 11:14:44.042675 thunder-ase-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 11:14:34.000000 thunder-ase-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:14:44.042675 thunder-ase-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-06-04 11:14:34.000000 thunder-ase-0.3/tests/test_Si_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:14:44.042675 thunder-ase-0.3/thunder_ase/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 11:14:34.000000 thunder-ase-0.3/thunder_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30732 2023-06-04 11:14:34.000000 thunder-ase-0.3/thunder_ase/fireball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 11:14:44.042675 thunder-ase-0.3/thunder_ase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-04 11:14:44.000000 thunder-ase-0.3/thunder_ase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-04 11:14:44.000000 thunder-ase-0.3/thunder_ase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 11:14:44.000000 thunder-ase-0.3/thunder_ase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-04 11:14:44.000000 thunder-ase-0.3/thunder_ase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-04 11:14:44.000000 thunder-ase-0.3/thunder_ase.egg-info/top_level.txt
```

### Comparing `thunder-ase-0.2.2/PKG-INFO` & `thunder-ase-0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.2.2
+Version: 0.3
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![Upload Python Package](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml)
+
 # Thunder ASE
 
 ### Description
 The interface of ASE for FIREBALL.  
 
 [FIREBALL](https://sites.google.com/site/fireballofficialsite/) is a local-orbital ab-initio tight binding implementation of  molecular dynamics. The method allows for the simulation and calculation of very large supercells of thousands of atoms or very long MD  simulations with ease.
 
 [ASE](https://wiki.fysik.dtu.dk/ase/index.html) is a popular python package for atomic structure modeling. ASE provide interfaces with many QM and MM software. This package is the interface for FIREBALL. 
 
 ### Installation
 
-`pip install git+https://github.com/thunder-dft/thunder-ase.git`
+`pip install thunder-ase`
 
 #### Requirements
+
 * ase
 
 ## Roadmap
 
 * v0.1: run basic fireball calculation and read basic result from it.
   * v0.1.1: jupyter-notebook for examples
   * v0.1.2: multiple atoms for one calculator
```

### Comparing `thunder-ase-0.2.2/README.md` & `thunder-ase-0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+[![Upload Python Package](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml)
+
 # Thunder ASE
 
 ### Description
 The interface of ASE for FIREBALL.  
 
 [FIREBALL](https://sites.google.com/site/fireballofficialsite/) is a local-orbital ab-initio tight binding implementation of  molecular dynamics. The method allows for the simulation and calculation of very large supercells of thousands of atoms or very long MD  simulations with ease.
 
 [ASE](https://wiki.fysik.dtu.dk/ase/index.html) is a popular python package for atomic structure modeling. ASE provide interfaces with many QM and MM software. This package is the interface for FIREBALL. 
 
 ### Installation
 
-`pip install git+https://github.com/thunder-dft/thunder-ase.git`
+`pip install thunder-ase`
 
 #### Requirements
+
 * ase
 
 ## Roadmap
 
 * v0.1: run basic fireball calculation and read basic result from it.
   * v0.1.1: jupyter-notebook for examples
   * v0.1.2: multiple atoms for one calculator
@@ -23,8 +26,8 @@
 * v0.2: band structure calculation.
   * v0.2.1: DOS calculation.
   * v0.2.2: fit basis to gaussian.
   * v0.2.3: write basis to mwfn.
   * v0.2.4: interface to multiwfn.
 * v0.3: MD calculation.
 * v0.4: Fdata management.
-* v0.5: interactive running.
+* v0.5: interactive running.
```

### Comparing `thunder-ase-0.2.2/tests/test_Si_lightning.py` & `thunder-ase-0.3/tests/test_Si_lightning.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.2.2/thunder_ase/fireball.py` & `thunder-ase-0.3/thunder_ase/fireball.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,21 +4,26 @@
 * run fireball calculations
 * read output
 """
 import os
 import subprocess
 from typing import Dict, Any
 import ase
+from ase.units import Hartree
 import numpy as np
 from ase.calculators.calculator import Calculator, CalculationFailed, all_changes
 from ase.dft.kpoints import monkhorst_pack, kpoint_convert
 from ase.geometry import get_distances
 import ase.spacegroup
 from ase.io import jsonio
 from ase.dft.kpoints import BandPath
+from thunder_ase.utils.mwfn import MWFN_FORMAT, MWFN_DEFAULT, MWFN_TEMPLATE, \
+    CELL_TEMPLATE, format_data, read_cdcoeffs, reorder_cdcoeffs
+from thunder_ase.utils.basis_set import read_info, read_gaussian
+from thunder_ase.utils.shell_dict import SHELL_NUM, SHELL_NAME, SHELL_PRIMARY_NUMS, SHELL_PRIMITIVE
 
 
 def get_kpts(atoms, size=None, offset=None, reduced=False, **kwargs):
     """
     Get reduced kpoints.
     Reference:
     * https://wiki.fysik.dtu.dk/ase/ase/dft/kpoints.html
@@ -129,15 +134,16 @@
 }
 
 calc_params = {
     'kpt_size': {'type': (list, np.array), 'name': 'kpt_size', 'default': [1, 1, 1]},
     'kpt_offset': {'type': (list, np.array), 'name': 'kpt_offset', 'default': [0., 0., 0.]},
     'kpt_interval': {'type': (list, np.array, float, int), 'name': 'kpt_interval', 'default': None},
     'kpt_path': {'type': (BandPath, str, list, np.array), 'name': 'kpt_path', 'default': None},
-    'nkpt': {'type': (int,), 'name': 'nkpt', 'default': None},  # number of kpoints on path, use it if kpt_path is string
+    'nkpt': {'type': (int,), 'name': 'nkpt', 'default': None},
+    # number of kpoints on path, use it if kpt_path is string
 }
 
 fireball_params = options_params | output_params | xsfoptions_params | calc_params
 
 
 def get_params_from_string(s):
     k, v = s.split('=')
@@ -205,15 +211,15 @@
             elif type(self.kpt_path) in (BandPath,):  # TODO: kpt_path must be BandPath
                 kpts = self.kpt_path.kpts
             else:
                 raise TypeError
 
             kpts = kpoint_convert(cell_cv=self.atoms.cell, skpts_kc=kpts)  # convert to Cartesian coordinate
             self.nkpt = len(kpts)
-            self._kpoints = [[k[0], k[1], k[2], 1.0/self.nkpt]for k in kpts]
+            self._kpoints = [[k[0], k[1], k[2], 1.0 / self.nkpt] for k in kpts]
             return self._kpoints
 
         if self.kpt_offset is None:
             offset = [0., 0., 0.]
         else:
             offset = self.kpt_offset
         if self.kpt_size is None:
@@ -225,15 +231,15 @@
             size = self.kpt_size
 
         self._kpoints = get_kpts(self.atoms, size=size, offset=offset, reduced=reduced, **kwargs)
         self.nkpt = len(self._kpoints)
         return self._kpoints
 
     def get_k_point_weights(self):
-        return np.asarray(self.get_kpoints())[:,-1]
+        return np.asarray(self.get_kpoints())[:, -1]
 
     def set_kpoints(self, kpoints):
         self._kpoints = kpoints
 
     def write_Fdata_inp(self, atoms=None, Fdata_path=None):
         if atoms is None:
             atoms = self.atoms
@@ -324,18 +330,19 @@
             f.write("{}\n".format(len(self.get_kpoints(reduced=reduced, **kwargs))))
             for k in self.get_kpoints(reduced=reduced, **kwargs):
                 f.write("{:8.6f} {:8.6f} {:8.6f} {:8.6f}\n".format(*k))
 
     def write_input(self, atoms=None, Fdata_path=None):
         if atoms is not None:
             self.atoms = atoms.copy()
-        self.write_Fdata_inp(atoms=atoms, Fdata_path=Fdata_path)
+        self.write_Fdata_inp(atoms=self.atoms, Fdata_path=Fdata_path)
         self.write_options()
         self.write_atoms(pbc=self.atoms.pbc)
-        self.write_kpts()
+        if np.any(self.atoms.pbc):
+            self.write_kpts()
 
     def read_options(self, input_file='structures.inp', read_atoms=False):
         # read structures.inp, get names for atoms and kpoints
         with open(input_file, 'r') as f:
             lines = f.readlines()
 
         natoms_list = int(lines[0].strip())
@@ -413,18 +420,20 @@
     def __init__(self, atoms=None,
                  Fdata_path='Fdata',
                  command='fireball.x',
                  **kwargs):
         self.__name__ = 'fireball'
         self._atoms = None
         self._eigenvalues = None
+        self._shell_info = None
         GenerateFireballInput.__init__(self, **kwargs)  # TODO: set kwargs use set() function, see vasp calculator
         Calculator.__init__(self, atoms=atoms, **kwargs)
         if not os.path.isdir(Fdata_path):
             # check the existence of Fdata directory
+            print("Error: Can't find Fdata! Pls Check the setting!")
             raise FileNotFoundError
         self.Fdata_path = Fdata_path
         self.command = command
 
     @property
     def atoms(self):
         return self._atoms
@@ -475,14 +484,18 @@
         return errorcode
 
     def read_results(self):
         output = self.sname + ".log.json"
         result = jsonio.read_json(output)
         self.results = result['fireball'][-1]
 
+    def get_forces(self, atoms=None):
+        forces = self.get_property('forces', atoms)
+        return np.asarray(forces)
+
     def get_fermi_level(self):
         return self.get_property('fermi')
 
     def get_ibz_k_points(self):
         if self.kpt_path is None:
             raise ValueError
         kpts = np.asarray(self.get_kpoints())[:, :3]
@@ -500,15 +513,15 @@
             raise FileExistsError
 
         with open(filename, 'r') as f:
             lines = f.readlines()
 
         eigenvalues = []
         eigen = []
-        kpts_count = [str(k+1) for k in range(self.nkpt)]
+        kpts_count = [str(k + 1) for k in range(self.nkpt)]
         for line in lines:
             content = [i.strip() for i in line.strip().split() if len(i.strip()) != 0]
             if len(content) == 0:
                 pass
             if len(kpts_count) != 0:
                 if content[0] == kpts_count[0]:
                     if len(eigen) != 0:
@@ -569,14 +582,124 @@
             if os.path.isfile(kpts_file):
                 self.read_kpts(kpts_file)
             atoms.set_calculator(self)
             atoms_list.append(atoms)
         multicalc = MultiFireball(atoms_list=atoms_list, sname_list=sname_list, calc=self)
         return multicalc
 
+    @property
+    def shell_info(self):
+        if self._shell_info is None:
+            # read Fdata/info.dat
+            self._shell_info = read_info(os.path.join(self.Fdata_path, 'info.dat'))
+
+            # TODO: this is a dirty way to get exicted_label.
+            #  The excited label can be obtained by set(ishell). However, still dirty.
+            for symbol, value in self._shell_info.items():
+                ishell = value['shells']
+                len_ground = len(SHELL_PRIMARY_NUMS[value['number']])
+                assert len(set(ishell)) <= len_ground  # if not, something wrong during generating Fdata
+                excited_label = [0] * len_ground + [1] * (len(ishell) - len_ground)
+                self._shell_info[symbol]['excited'] = excited_label
+        return self._shell_info
+
+    def get_valence_charge(self, i):
+        isymbol = self.atoms.symbols[i]
+        shell_info = self.shell_info[isymbol]
+        return sum(shell_info['occupation'])
+
+    def write_mwfn(self, kpoint=0):
+        mwfn_dict = MWFN_DEFAULT.copy()
+        # Initialize default data format
+        for k, v in mwfn_dict.items():
+            if v is not None:
+                mwfn_dict[k] = MWFN_FORMAT[k].format(v)
+
+        # atom information
+        mwfn_dict['ncenter'] = MWFN_FORMAT['ncenter'].format(len(self.atoms))
+        atoms_coord = [MWFN_FORMAT['atoms_coord'].format(idx+1,
+                                                         iatom.symbol,
+                                                         iatom.number,
+                                                         self.get_valence_charge(idx),
+                                                         *iatom.position)
+                       for idx, iatom in enumerate(self.atoms)]
+        mwfn_dict['atoms_coord'] = '\n'.join(atoms_coord)
+
+        # cell info
+        if np.any(self.atoms.pbc):
+            cell_info = {
+                'ndim': MWFN_FORMAT['ndim'].format(3),
+                'cellv1': (MWFN_FORMAT['cellv1'] * 3).format(*self.atoms.cell[0]),
+                'cellv2': (MWFN_FORMAT['cellv2'] * 3).format(*self.atoms.cell[1]),
+                'cellv3': (MWFN_FORMAT['cellv3'] * 3).format(*self.atoms.cell[2]),
+            }
+            mwfn_dict['cell_info'] = CELL_TEMPLATE.substitute(cell_info)
+        else:
+            mwfn_dict['cell_info'] = ''
+
+        # electron for alpha and beta
+        tot_elec = sum([self.get_valence_charge(i) for i in range(len(self.atoms))])
+        naelec = 0.5 * tot_elec
+        nbelec = 0.5 * tot_elec
+        mwfn_dict['naelec'] = MWFN_FORMAT['naelec'].format(naelec)
+        mwfn_dict['nbelec'] = MWFN_FORMAT['nbelec'].format(nbelec)
+        # total energy
+        mwfn_dict['e_tot'] = MWFN_FORMAT['e_tot'].format(self.get_potential_energy() / Hartree)
+        # Basis set info
+        shell_types = []
+        shell_centers = []
+        shell_contraction_degress = []
+        primitive_exponents = []
+        contraction_coefficients = []
+        for idx, symbol in enumerate(self.atoms.symbols):
+            ishells = self.shell_info[symbol]['shells']
+            shell_centers += [idx+1] * len(ishells)
+            shell_types += ishells
+            excited_label = self.shell_info[symbol]['excited']
+            for shell, is_excited in zip(ishells, excited_label):
+                gbs = read_gaussian(self.shell_info[symbol]['number'], shell, is_excited, Fdata_path=self.Fdata_path)
+                shell_contraction_degress.append(gbs['degree'])
+                primitive_exponents += gbs['alpha'].tolist()
+                contraction_coefficients += gbs['coefficient'].tolist()
+        nbasis = sum([shell*2+1 for shell in shell_types])
+        nshell = len(shell_types)
+        nprimshell = len(primitive_exponents)
+        nprims = sum([SHELL_PRIMITIVE[st]*degree
+                      for st, degree in zip(shell_types, shell_contraction_degress)])
+        shell_types = [((i < 2) * 2 - 1) * i for i in shell_types]  # if i >= 2, use negative value
+
+        mwfn_dict['nbasis'] = MWFN_FORMAT['nbasis'].format(nbasis)
+        mwfn_dict['nindbasis'] = MWFN_FORMAT['nindbasis'].format(nbasis)
+        mwfn_dict['nprims'] = MWFN_FORMAT['nprims'].format(nprims)
+        mwfn_dict['nshell'] = MWFN_FORMAT['nshell'].format(nshell)
+        mwfn_dict['nprimshell'] = MWFN_FORMAT['nprimshell'].format(nprimshell)
+
+        mwfn_dict['shell_types'] = format_data('shell_types', shell_types)
+        mwfn_dict['shell_centers'] = format_data('shell_centers', shell_centers)
+        mwfn_dict['shell_contraction_degress'] = format_data('shell_contraction_degress', shell_contraction_degress)
+        mwfn_dict['primitive_exponents'] = format_data('primitive_exponents', primitive_exponents)
+        mwfn_dict['contraction_coefficients'] = format_data('contraction_coefficients', contraction_coefficients)
+
+        cdcoeffs = read_cdcoeffs(self.sname+'.cdcoeffs-mwfn')[kpoint]
+        orbital_coeffs = []
+        for orbital in cdcoeffs:
+            info = ''.join(orbital['info'])
+            coeff = orbital['coeff']
+            coeff = reorder_cdcoeffs(coeff, shell_types)
+            orbital_coeffs += [info + format_data('MO_coefficients', coeff)]
+        mwfn_dict['orbital_coeffs'] = '\n\n'.join(orbital_coeffs)
+
+        self.mwfn_dict = mwfn_dict
+        content = MWFN_TEMPLATE.substitute(mwfn_dict)
+        # TODO: read orbital info, append to the content
+
+        # write out
+        with open(self.sname + '.mwfn', 'w') as f:
+            f.write(content)
+
 
 class MultiFireball:
     name = 'multi_fireball'
 
     def __init__(self, atoms_list=None, calc=None, sname_list=None):
         if calc is not None:
             self.calc = calc
```

### Comparing `thunder-ase-0.2.2/thunder_ase.egg-info/PKG-INFO` & `thunder-ase-0.3/thunder_ase.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.2.2
+Version: 0.3
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![Upload Python Package](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml/badge.svg)](https://github.com/thunder-dft/thunder-ase/actions/workflows/python-publish.yml)
+
 # Thunder ASE
 
 ### Description
 The interface of ASE for FIREBALL.  
 
 [FIREBALL](https://sites.google.com/site/fireballofficialsite/) is a local-orbital ab-initio tight binding implementation of  molecular dynamics. The method allows for the simulation and calculation of very large supercells of thousands of atoms or very long MD  simulations with ease.
 
 [ASE](https://wiki.fysik.dtu.dk/ase/index.html) is a popular python package for atomic structure modeling. ASE provide interfaces with many QM and MM software. This package is the interface for FIREBALL. 
 
 ### Installation
 
-`pip install git+https://github.com/thunder-dft/thunder-ase.git`
+`pip install thunder-ase`
 
 #### Requirements
+
 * ase
 
 ## Roadmap
 
 * v0.1: run basic fireball calculation and read basic result from it.
   * v0.1.1: jupyter-notebook for examples
   * v0.1.2: multiple atoms for one calculator
```

