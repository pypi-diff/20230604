# Comparing `tmp/tb-mean-field-hubbard-2.1.0.tar.gz` & `tmp/tb-mean-field-hubbard-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb-mean-field-hubbard-2.1.0.tar", last modified: Sun Jun 26 13:50:42 2022, max compression
+gzip compressed data, was "tb-mean-field-hubbard-2.2.0.tar", last modified: Sun Jun  4 09:40:25 2023, max compression
```

## Comparing `tb-mean-field-hubbard-2.1.0.tar` & `tb-mean-field-hubbard-2.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 13:50:42.723375 tb-mean-field-hubbard-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35150 2022-06-26 13:50:16.000000 tb-mean-field-hubbard-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-06-26 13:50:42.723375 tb-mean-field-hubbard-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-06-26 13:50:16.000000 tb-mean-field-hubbard-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-26 13:50:42.723375 tb-mean-field-hubbard-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-06-26 13:50:16.000000 tb-mean-field-hubbard-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 13:50:42.723375 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-26 13:50:16.000000 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10846 2022-06-26 13:50:16.000000 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard/mfh.py
--rw-r--r--   0 runner    (1001) docker     (121)     7995 2022-06-26 13:50:16.000000 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard/mfh_pp.py
--rw-r--r--   0 runner    (1001) docker     (121)     9133 2022-06-26 13:50:16.000000 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-26 13:50:42.723375 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3136 2022-06-26 13:50:42.000000 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-06-26 13:50:42.000000 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-26 13:50:42.000000 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-06-26 13:50:42.000000 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-06-26 13:50:42.000000 tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:40:25.037964 tb-mean-field-hubbard-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35150 2023-06-04 09:39:57.000000 tb-mean-field-hubbard-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-04 09:40:25.033964 tb-mean-field-hubbard-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-06-04 09:39:57.000000 tb-mean-field-hubbard-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 09:40:25.037964 tb-mean-field-hubbard-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-04 09:39:57.000000 tb-mean-field-hubbard-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:40:25.033964 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-04 09:39:57.000000 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2023-06-04 09:39:57.000000 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard/mfh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-06-04 09:39:57.000000 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard/mfh_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-06-04 09:39:57.000000 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 09:40:25.033964 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-04 09:40:25.000000 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-04 09:40:25.000000 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 09:40:25.000000 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-04 09:40:25.000000 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 09:40:25.000000 tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard.egg-info/top_level.txt
```

### Comparing `tb-mean-field-hubbard-2.1.0/LICENSE` & `tb-mean-field-hubbard-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tb-mean-field-hubbard-2.1.0/PKG-INFO` & `tb-mean-field-hubbard-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tb-mean-field-hubbard
-Version: 2.1.0
+Version: 2.2.0
 Summary: Package to run tight-binding mean field hubbard calculations
 Home-page: https://github.com/eimrek/tb-mean-field-hubbard
 Author: Kristjan Eimre
 Author-email: kristjaneimre@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tb-mean-field-hubbard-2.1.0/README.md` & `tb-mean-field-hubbard-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `tb-mean-field-hubbard-2.1.0/setup.py` & `tb-mean-field-hubbard-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="tb-mean-field-hubbard",
-    version="2.1.0",
+    version="2.2.0",
     author="Kristjan Eimre",
     author_email="kristjaneimre@gmail.com",
     description="Package to run tight-binding mean field hubbard calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eimrek/tb-mean-field-hubbard",
     packages=setuptools.find_packages(),
```

### Comparing `tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard/mfh.py` & `tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard/mfh.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,28 +15,30 @@
 ### ------------------------------------------------------------------------------
 
 
 class MeanFieldHubbardModel:
     """
     Class that takes care of running the Mean Field Hubbard calculation
     """
+
     def __init__(self, ase_geom, t_list=[2.7], charge=0, multiplicity='auto', bond_cutoff='auto'):
 
         self.t_list = t_list
         self.charge = charge
 
         if multiplicity == 'auto':
             self.multiplicity = 0
             self.relax_multiplicity = True
         else:
             self.multiplicity = multiplicity
             self.relax_multiplicity = False
 
         self.ase_geom = ase_geom
         self.num_atoms = len(ase_geom)
+        self.onsite_energies = np.zeros(self.num_atoms)  # by default, no on-site energies
 
         self.figure_size = (np.ptp(self.ase_geom.positions, axis=0)[:2] + 1.0) / 4.0
         self.figure_size[0] = max([self.figure_size[0], 3.5])  # to have enough space for titles
 
         self.spin_guess = self._load_spin_guess(self.ase_geom)
 
         if bond_cutoff == 'auto':
@@ -154,14 +156,30 @@
             if not (0 <= i1 < self.num_atoms) or not (0 <= i2 < self.num_atoms):
                 print("Error: index out of range.")
                 return
             if i1 < i2: i1, i2 = i2, i1
             self.model_a.set_hop(-t, i1, i2, mode='reset')
             self.model_b.set_hop(-t, i1, i2, mode='reset')
 
+    def set_onsite_energies(self, onsites_list):
+        """ Set the on-site energy/potentials for a list of sites
+
+        onsites_list - list of tuples (atom index, on-site energy)
+        """
+
+        for onsite in onsites_list:
+            if len(onsite) != 2:
+                print("Error: please specify (atom index, on-site energy)")
+                return
+            i, e = onsite
+            if not (0 <= i < self.num_atoms):
+                print("Error: index out of range.")
+                return
+            self.onsite_energies[i] = e
+
     def visualize_tb_model(self):
         self.model_a.visualize(0, 1)
         plt.show()
 
     def visualize_spin_guess(self):
         plt.figure(figsize=self.figure_size)
         spin_guess_plot = 0.5 * (self.spin_guess[:, 0] - self.spin_guess[:, 1])
@@ -209,16 +227,16 @@
 
     def mfh_iteration(self, u):
 
         # Update MFH Hubbard on-site potential
 
         for i_at, d in enumerate(self.spin_resolved_dens):
 
-            self.model_a.set_onsite(u * d[1], i_at, mode="reset")
-            self.model_b.set_onsite(u * d[0], i_at, mode="reset")
+            self.model_a.set_onsite(u * d[1] + self.onsite_energies[i_at], i_at, mode="reset")
+            self.model_b.set_onsite(u * d[0] + self.onsite_energies[i_at], i_at, mode="reset")
 
         # Solve the new TB
         (evals_a, evecs_a) = self.model_a.solve_all(eig_vectors=True)
         (evals_b, evecs_b) = self.model_b.solve_all(eig_vectors=True)
 
         # Update spin-resolved density
         self.spin_resolved_dens[:] = self.new_spin_res_dens([evals_a, evals_b], [evecs_a, evecs_b])
@@ -305,8 +323,8 @@
             gap_a = lumo_a - homo_a
             gap_b = lumo_b - homo_b
             gap = np.min([lumo_a, lumo_b]) - np.max([homo_a, homo_b])
 
             return gap_a, gap_b, gap
 
         except IndexError:
-            return np.nan, np.nan, np.nan
+            return np.nan, np.nan, np.nan
```

### Comparing `tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard/mfh_pp.py` & `tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard/mfh_pp.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,19 +72,28 @@
             p = at.position
             local_i, local_grid = utils.get_local_grid(x_arr, y_arr, p, cutoff=1.2 * h + 4.0)
             pz_orb = utils.carbon_2pz_slater(local_grid[0] - p[0], local_grid[1] - p[1], h, z_eff)
             orb_map[local_i[0]:local_i[1], local_i[2]:local_i[3]] += coef * pz_orb
 
         return orb_map, extent
 
-    def plot_orb_squared_map(self, ax, evec, h=10.0, edge_space=5.0, dx=0.1, title=None, cmap='seismic', z_eff=3.25):
+    def plot_orb_squared_map(self, evec, h=10.0, edge_space=5.0, dx=0.1, title=None, cmap='seismic', z_eff=3.25, ax=None):
         orb_map, extent = self.calc_orb_map(evec, h, edge_space, dx, z_eff)
-        ax.imshow((np.abs(orb_map)**2).T, origin='lower', cmap=cmap, extent=extent)
-        ax.axis('off')
-        ax.set_title(title)
+
+        use_ax = ax
+        if ax is None:
+            plt.figure(figsize=self.mfh.figure_size)
+            use_ax = plt.gca()
+
+        use_ax.imshow((np.abs(orb_map)**2).T, origin='lower', cmap=cmap, extent=extent)
+        use_ax.axis('off')
+        use_ax.set_title(title)
+
+        if ax is None:
+            plt.show()
 
     def calc_sts_map(self, energy, broadening=0.05, h=10.0, edge_space=5.0, dx=0.1, z_eff=3.25):
 
         final_map = None
         extent = None
 
         for i_spin in range(2):
@@ -97,29 +106,38 @@
                         final_map = broad_coef * np.abs(orb_map)**2
                     else:
                         final_map += broad_coef * np.abs(orb_map)**2
 
         return final_map, extent
 
     def plot_sts_map(self,
-                     ax,
                      energy,
                      broadening=0.05,
                      h=10.0,
                      edge_space=5.0,
                      dx=0.1,
                      title=None,
                      cmap='seismic',
-                     z_eff=3.25):
+                     z_eff=3.25,
+                     ax=None):
 
         final_map, extent = self.calc_sts_map(energy, broadening, h, edge_space, dx, z_eff)
 
-        ax.imshow(final_map.T, origin='lower', cmap=cmap, extent=extent)
-        ax.axis('off')
-        ax.set_title(title)
+        use_ax = ax
+        if ax is None:
+            plt.figure(figsize=self.mfh.figure_size)
+            use_ax = plt.gca()
+
+        use_ax.imshow(final_map.T, origin='lower', cmap=cmap, extent=extent)
+        use_ax.axis('off')
+        use_ax.set_title(title)
+
+        if ax is None:
+            plt.show()
+
 
     def plot_eigenvector(self, ax, evec, title=None):
         utils.make_evec_plot(ax, self.mfh.ase_geom, self.mfh.neighbor_list, evec, title=title)
 
     def plot_mo_eigenvector(self, mo_index, spin=0, ax=None):
         title = "mo%d s%d %s, en: %.2f" % (mo_index, spin, utils.orb_label(
             mo_index, self.mfh.num_spin_el[spin]), self.mfh.evals[spin][mo_index])
@@ -170,18 +188,18 @@
 
             _fig, axs = plt.subplots(nrows=1, ncols=4, figsize=(4 * self.mfh.figure_size[0], self.mfh.figure_size[1]))
 
             self.plot_mo_eigenvector(i_mo, spin=0, ax=axs[0])
             self.plot_mo_eigenvector(i_mo, spin=1, ax=axs[1])
 
             title1 = "sts h=%.1f, en: %.2f" % (sts_h, self.mfh.evals[0][i_mo])
-            self.plot_sts_map(axs[2], self.mfh.evals[0][i_mo], broadening=sts_broad, h=sts_h, title=title1)
+            self.plot_sts_map(self.mfh.evals[0][i_mo], broadening=sts_broad, h=sts_h, title=title1, ax=axs[2])
 
             title2 = "sts h=%.1f, en: %.2f" % (sts_h, self.mfh.evals[1][i_mo])
-            self.plot_sts_map(axs[3], self.mfh.evals[1][i_mo], broadening=sts_broad, h=sts_h, title=title2)
+            self.plot_sts_map(self.mfh.evals[1][i_mo], broadening=sts_broad, h=sts_h, title=title2, ax=axs[3])
 
             plt.show()
 
     def calculate_natural_orbitals(self):
         # build the one particle reduced density matrix
         dens_mat = None
```

### Comparing `tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard/utils.py` & `tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard/utils.py`

 * *Files identical despite different names*

### Comparing `tb-mean-field-hubbard-2.1.0/tb_mean_field_hubbard.egg-info/PKG-INFO` & `tb-mean-field-hubbard-2.2.0/tb_mean_field_hubbard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tb-mean-field-hubbard
-Version: 2.1.0
+Version: 2.2.0
 Summary: Package to run tight-binding mean field hubbard calculations
 Home-page: https://github.com/eimrek/tb-mean-field-hubbard
 Author: Kristjan Eimre
 Author-email: kristjaneimre@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

