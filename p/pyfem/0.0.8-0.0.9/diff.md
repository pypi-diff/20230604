# Comparing `tmp/pyfem-0.0.8.tar.gz` & `tmp/pyfem-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfem-0.0.8.tar", last modified: Mon May 22 04:05:01 2023, max compression
+gzip compressed data, was "pyfem-0.0.9.tar", last modified: Sun Jun  4 04:40:09 2023, max compression
```

## Comparing `pyfem-0.0.8.tar` & `pyfem-0.0.9.tar`

### file list

```diff
@@ -1,68 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.969822 pyfem-0.0.8/
--rw-rw-rw-   0        0        0    11525 2023-05-04 02:49:52.000000 pyfem-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      793 2023-05-22 04:05:01.968822 pyfem-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-19 03:01:04.000000 pyfem-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 04:05:01.969822 pyfem-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      941 2023-05-22 04:03:18.000000 pyfem-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.904823 pyfem-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.915823 pyfem-0.0.8/src/pyfem/
--rw-rw-rw-   0        0        0      857 2023-05-22 03:57:50.000000 pyfem-0.0.8/src/pyfem/Job.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/__init__.py
--rw-rw-rw-   0        0        0      277 2023-05-22 03:59:51.000000 pyfem-0.0.8/src/pyfem/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.922823 pyfem-0.0.8/src/pyfem/assembly/
--rw-rw-rw-   0        0        0     8732 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/assembly/Assembly.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/assembly/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.926823 pyfem-0.0.8/src/pyfem/bc/
--rw-rw-rw-   0        0        0      781 2023-05-19 07:42:39.000000 pyfem-0.0.8/src/pyfem/bc/BaseBC.py
--rw-rw-rw-   0        0        0     2262 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/bc/DirichletBC.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/bc/__init__.py
--rw-rw-rw-   0        0        0      876 2023-05-19 09:14:01.000000 pyfem-0.0.8/src/pyfem/bc/get_bc_data.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.934822 pyfem-0.0.8/src/pyfem/elements/
--rw-rw-rw-   0        0        0     4293 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/elements/BaseElement.py
--rw-rw-rw-   0        0        0     1793 2023-05-15 02:23:48.000000 pyfem-0.0.8/src/pyfem/elements/IsoElementDiagram.py
--rw-rw-rw-   0        0        0    19983 2023-05-19 05:44:29.000000 pyfem-0.0.8/src/pyfem/elements/IsoElementShape.py
--rw-rw-rw-   0        0        0     4367 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/elements/SolidPlaneSmallStrain.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/elements/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-05-18 07:52:50.000000 pyfem-0.0.8/src/pyfem/elements/get_element_data.py
--rw-rw-rw-   0        0        0     1793 2023-05-18 05:01:54.000000 pyfem-0.0.8/src/pyfem/elements/get_iso_element_type.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.936823 pyfem-0.0.8/src/pyfem/fem/
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/fem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.948822 pyfem-0.0.8/src/pyfem/io/
--rw-rw-rw-   0        0        0      679 2023-05-19 08:44:54.000000 pyfem-0.0.8/src/pyfem/io/BC.py
--rw-rw-rw-   0        0        0      577 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Dof.py
--rw-rw-rw-   0        0        0     2299 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Material.py
--rw-rw-rw-   0        0        0      520 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Mesh.py
--rw-rw-rw-   0        0        0      575 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/io/Output.py
--rw-rw-rw-   0        0        0    10250 2023-05-22 03:55:12.000000 pyfem-0.0.8/src/pyfem/io/Properties.py
--rw-rw-rw-   0        0        0      815 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Section.py
--rw-rw-rw-   0        0        0      466 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/io/Solver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/io/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-05-22 04:03:27.000000 pyfem-0.0.8/src/pyfem/io/arguments.py
--rw-rw-rw-   0        0        0     3224 2023-05-22 04:02:40.000000 pyfem-0.0.8/src/pyfem/io/write_vtk.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.953823 pyfem-0.0.8/src/pyfem/materials/
--rw-rw-rw-   0        0        0      840 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/materials/BaseMaterial.py
--rw-rw-rw-   0        0        0     5986 2023-05-18 08:03:05.000000 pyfem-0.0.8/src/pyfem/materials/ElasticIsotropic.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/materials/__init__.py
--rw-rw-rw-   0        0        0     1129 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/materials/get_material_data.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.956831 pyfem-0.0.8/src/pyfem/mesh/
--rw-rw-rw-   0        0        0     3282 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/mesh/ElementSet.py
--rw-rw-rw-   0        0        0     3482 2023-05-22 03:16:36.000000 pyfem-0.0.8/src/pyfem/mesh/NodeSet.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/mesh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.960822 pyfem-0.0.8/src/pyfem/solvers/
--rw-rw-rw-   0        0        0      887 2023-05-22 02:53:25.000000 pyfem-0.0.8/src/pyfem/solvers/BaseSolver.py
--rw-rw-rw-   0        0        0      966 2023-05-22 03:16:04.000000 pyfem-0.0.8/src/pyfem/solvers/LinearSolver.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/solvers/__init__.py
--rw-rw-rw-   0        0        0      854 2023-05-22 03:15:35.000000 pyfem-0.0.8/src/pyfem/solvers/get_solver_data.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.967822 pyfem-0.0.8/src/pyfem/utils/
--rw-rw-rw-   0        0        0     2313 2023-05-18 08:06:24.000000 pyfem-0.0.8/src/pyfem/utils/IntKeyDict.py
--rw-rw-rw-   0        0        0        0 2023-05-04 02:49:52.000000 pyfem-0.0.8/src/pyfem/utils/__init__.py
--rw-rw-rw-   0        0        0      707 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/utils/colors.py
--rw-rw-rw-   0        0        0     1516 2023-05-08 04:08:44.000000 pyfem-0.0.8/src/pyfem/utils/logger.py
--rw-rw-rw-   0        0        0     1738 2023-05-19 09:23:55.000000 pyfem-0.0.8/src/pyfem/utils/visualization.py
--rw-rw-rw-   0        0        0      982 2023-05-19 02:59:20.000000 pyfem-0.0.8/src/pyfem/utils/wrappers.py
-drwxrwxrwx   0        0        0        0 2023-05-22 04:05:01.920823 pyfem-0.0.8/src/pyfem.egg-info/
--rw-rw-rw-   0        0        0      793 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1510 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 04:05:01.000000 pyfem-0.0.8/src/pyfem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.251949 pyfem-0.0.9/
+-rw-rw-rw-   0        0        0    11524 2023-05-03 09:58:16.000000 pyfem-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      793 2023-06-04 04:40:09.251453 pyfem-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-19 11:01:17.000000 pyfem-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-04 04:40:09.251949 pyfem-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1067 2023-06-04 04:29:16.000000 pyfem-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.133768 pyfem-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.149144 pyfem-0.0.9/src/pyfem/
+-rw-rw-rw-   0        0        0     1025 2023-06-02 16:36:54.000000 pyfem-0.0.9/src/pyfem/Job.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/__init__.py
+-rw-rw-rw-   0        0        0      277 2023-05-22 12:37:32.000000 pyfem-0.0.9/src/pyfem/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.164026 pyfem-0.0.9/src/pyfem/assembly/
+-rw-rw-rw-   0        0        0     8811 2023-06-01 15:32:06.000000 pyfem-0.0.9/src/pyfem/assembly/Assembly.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/assembly/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.171072 pyfem-0.0.9/src/pyfem/bc/
+-rw-rw-rw-   0        0        0      781 2023-05-19 11:01:17.000000 pyfem-0.0.9/src/pyfem/bc/BaseBC.py
+-rw-rw-rw-   0        0        0     2268 2023-05-30 15:48:17.000000 pyfem-0.0.9/src/pyfem/bc/DirichletBC.py
+-rw-rw-rw-   0        0        0        0 2023-05-19 11:01:17.000000 pyfem-0.0.9/src/pyfem/bc/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-05-19 11:01:17.000000 pyfem-0.0.9/src/pyfem/bc/get_bc_data.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.186204 pyfem-0.0.9/src/pyfem/elements/
+-rw-rw-rw-   0        0        0     5142 2023-06-02 16:35:55.000000 pyfem-0.0.9/src/pyfem/elements/BaseElement.py
+-rw-rw-rw-   0        0        0     2315 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/elements/IsoElementDiagram.py
+-rw-rw-rw-   0        0        0    30821 2023-06-02 17:14:27.000000 pyfem-0.0.9/src/pyfem/elements/IsoElementShape.py
+-rw-rw-rw-   0        0        0     6426 2023-06-02 16:09:39.000000 pyfem-0.0.9/src/pyfem/elements/SolidPlaneSmallStrain.py
+-rw-rw-rw-   0        0        0     7214 2023-06-02 14:12:56.000000 pyfem-0.0.9/src/pyfem/elements/SolidVolumeSmallStrain.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/elements/__init__.py
+-rw-rw-rw-   0        0        0     2169 2023-05-31 12:01:59.000000 pyfem-0.0.9/src/pyfem/elements/get_element_data.py
+-rw-rw-rw-   0        0        0     1792 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/elements/get_iso_element_type.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.191660 pyfem-0.0.9/src/pyfem/fem/
+-rw-rw-rw-   0        0        0      897 2023-06-01 12:24:10.000000 pyfem-0.0.9/src/pyfem/fem/Timer.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/fem/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-06-01 14:47:42.000000 pyfem-0.0.9/src/pyfem/fem/constants.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.212466 pyfem-0.0.9/src/pyfem/io/
+-rw-rw-rw-   0        0        0      679 2023-05-19 11:01:17.000000 pyfem-0.0.9/src/pyfem/io/BC.py
+-rw-rw-rw-   0        0        0      577 2023-05-18 14:20:30.000000 pyfem-0.0.9/src/pyfem/io/Dof.py
+-rw-rw-rw-   0        0        0     2411 2023-06-01 12:24:10.000000 pyfem-0.0.9/src/pyfem/io/Material.py
+-rw-rw-rw-   0        0        0      520 2023-05-18 14:20:30.000000 pyfem-0.0.9/src/pyfem/io/Mesh.py
+-rw-rw-rw-   0        0        0      575 2023-05-20 17:12:32.000000 pyfem-0.0.9/src/pyfem/io/Output.py
+-rw-rw-rw-   0        0        0    11352 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/io/Properties.py
+-rw-rw-rw-   0        0        0      815 2023-05-18 14:20:30.000000 pyfem-0.0.9/src/pyfem/io/Section.py
+-rw-rw-rw-   0        0        0      821 2023-06-01 12:26:16.000000 pyfem-0.0.9/src/pyfem/io/Solver.py
+-rw-rw-rw-   0        0        0        0 2023-04-19 14:26:23.000000 pyfem-0.0.9/src/pyfem/io/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-06-04 04:30:48.000000 pyfem-0.0.9/src/pyfem/io/arguments.py
+-rw-rw-rw-   0        0        0     4271 2023-06-01 12:24:10.000000 pyfem-0.0.9/src/pyfem/io/write_vtk.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.225461 pyfem-0.0.9/src/pyfem/materials/
+-rw-rw-rw-   0        0        0     1245 2023-05-31 12:01:59.000000 pyfem-0.0.9/src/pyfem/materials/BaseMaterial.py
+-rw-rw-rw-   0        0        0     6857 2023-06-01 12:36:14.000000 pyfem-0.0.9/src/pyfem/materials/ElasticIsotropic.py
+-rw-rw-rw-   0        0        0     1342 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/materials/PlasticIsotropicHardening.py
+-rw-rw-rw-   0        0        0     5218 2023-06-04 04:38:44.000000 pyfem-0.0.9/src/pyfem/materials/PlasticKinematicHardening.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/materials/__init__.py
+-rw-rw-rw-   0        0        0     1309 2023-05-23 13:12:51.000000 pyfem-0.0.9/src/pyfem/materials/get_material_data.py
+-rw-rw-rw-   0        0        0     5330 2023-06-01 15:48:19.000000 pyfem-0.0.9/src/pyfem/materials/run.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.230968 pyfem-0.0.9/src/pyfem/mesh/
+-rw-rw-rw-   0        0        0     4765 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/mesh/ElementSet.py
+-rw-rw-rw-   0        0        0     4994 2023-06-01 12:32:50.000000 pyfem-0.0.9/src/pyfem/mesh/NodeSet.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/mesh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.239549 pyfem-0.0.9/src/pyfem/solvers/
+-rw-rw-rw-   0        0        0      738 2023-05-31 13:50:18.000000 pyfem-0.0.9/src/pyfem/solvers/BaseSolver.py
+-rw-rw-rw-   0        0        0     1450 2023-06-01 14:20:50.000000 pyfem-0.0.9/src/pyfem/solvers/LinearSolver.py
+-rw-rw-rw-   0        0        0     7445 2023-06-02 15:54:17.000000 pyfem-0.0.9/src/pyfem/solvers/NonlinearSolver.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/solvers/__init__.py
+-rw-rw-rw-   0        0        0      954 2023-05-23 12:42:03.000000 pyfem-0.0.9/src/pyfem/solvers/get_solver_data.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.249965 pyfem-0.0.9/src/pyfem/utils/
+-rw-rw-rw-   0        0        0     2350 2023-06-01 12:30:53.000000 pyfem-0.0.9/src/pyfem/utils/IntKeyDict.py
+-rw-rw-rw-   0        0        0        0 2023-04-13 12:04:13.000000 pyfem-0.0.9/src/pyfem/utils/__init__.py
+-rw-rw-rw-   0        0        0      795 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/utils/colors.py
+-rw-rw-rw-   0        0        0     1518 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/utils/logger.py
+-rw-rw-rw-   0        0        0     1820 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/utils/visualization.py
+-rw-rw-rw-   0        0        0     1046 2023-05-30 13:27:33.000000 pyfem-0.0.9/src/pyfem/utils/wrappers.py
+drwxrwxrwx   0        0        0        0 2023-06-04 04:40:09.160690 pyfem-0.0.9/src/pyfem.egg-info/
+-rw-rw-rw-   0        0        0      793 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1799 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-04 04:40:09.000000 pyfem-0.0.9/src/pyfem.egg-info/top_level.txt
```

### Comparing `pyfem-0.0.8/LICENSE` & `pyfem-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -194,8 +194,8 @@
 
        http://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
-   limitations under the License.
+   limitations under the License.
```

### Comparing `pyfem-0.0.8/PKG-INFO` & `pyfem-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.8
+Version: 0.0.9
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyfem-0.0.8/setup.py` & `pyfem-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyfem",
-    version="0.0.8",
+    version="0.0.9",
     author="Jingyu Sun",
     author_email="sun.jingyu@outlook.com",
     description="A finite element package for learning",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sunwhale/pyfem",
     project_urls={
@@ -23,9 +23,16 @@
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.9",
     entry_points={
         'console_scripts': [
             'pyfem=pyfem.__main__:main'
         ]
-    }
+    },
+    install_requires=[
+        'numpy',
+        'scipy',
+        'meshio',
+        'tomli',
+        'colorlog'
+    ],
 )
```

### Comparing `pyfem-0.0.8/src/pyfem/Job.py` & `pyfem-0.0.9/src/pyfem/Job.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,32 @@
 
 """
 from pathlib import Path
 from typing import Union
 
 from pyfem.assembly.Assembly import Assembly
 from pyfem.io.Properties import Properties
-from pyfem.io.write_vtk import write_vtk
 from pyfem.solvers.get_solver_data import get_solver_data
+from pyfem.utils.visualization import object_dict_to_string
 
 
 class Job:
     def __init__(self, filename: Union[Path, str]) -> None:
         input_file = Path(filename)
         if input_file.is_absolute():
             abs_input_file = input_file
         else:
             abs_input_file = Path.cwd().joinpath(input_file)
         self.props = Properties()
         self.props.read_file(abs_input_file)
+        # self.props.show()
         self.assembly = Assembly(self.props)
         self.solver_data = get_solver_data(self.assembly, self.props.solver)
 
     def run(self):
         self.solver_data.run()
-        write_vtk(self.props, self.assembly)
+
+    def to_string(self, level: int = 1) -> str:
+        return object_dict_to_string(self, level)
+
+    def show(self) -> None:
+        print(self.to_string())
```

### Comparing `pyfem-0.0.8/src/pyfem/assembly/Assembly.py` & `pyfem-0.0.9/src/pyfem/assembly/Assembly.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,66 +1,78 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from typing import List, Dict
 
 from numpy import repeat, array, ndarray, empty, zeros
 from scipy.sparse import coo_matrix, csc_matrix  # type: ignore
 
 from pyfem.bc.BaseBC import BaseBC
 from pyfem.bc.get_bc_data import get_bc_data
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.elements.get_element_data import get_element_data
 from pyfem.elements.get_iso_element_type import get_iso_element_type
+from pyfem.fem.Timer import Timer
+from pyfem.fem.constants import DTYPE
 from pyfem.io.Properties import Properties
 from pyfem.materials.get_material_data import get_material_data
 from pyfem.utils.visualization import object_dict_to_string_assembly
 from pyfem.utils.wrappers import show_running_time
 
 iso_element_shape_dict = {
     'line2': IsoElementShape('line2'),
     'line3': IsoElementShape('line3'),
     'tria3': IsoElementShape('tria3'),
+    'tria6': IsoElementShape('tria6'),
     'quad4': IsoElementShape('quad4'),
     'quad8': IsoElementShape('quad8'),
     'tetra4': IsoElementShape('tetra4'),
-    'hex8': IsoElementShape('hex8')
+    'hex8': IsoElementShape('hex8'),
+    'hex20': IsoElementShape('hex20')
 }
 
 
 class Assembly:
     def __init__(self, props: Properties) -> None:
         self.total_dof_number: int = -1
         self.props: Properties = props
+        self.timer: Timer = Timer()
         self.materials_dict: Dict = {}
         self.sections_dict: Dict = {}
         self.section_of_element_set: Dict = {}
         self.element_data_list: List[BaseElement] = []
         self.bc_data_list: List[BaseBC] = []
         self.global_stiffness: csc_matrix = csc_matrix(0)
-        self.fext: ndarray = empty(0)
-        self.fint: ndarray = empty(0)
-        self.dof_solution: ndarray = empty(0)
+        self.fext: ndarray = empty(0, dtype=DTYPE)
+        self.fint: ndarray = empty(0, dtype=DTYPE)
+        self.dof_solution: ndarray = empty(0, dtype=DTYPE)
+        self.ddof_solution: ndarray = empty(0, dtype=DTYPE)
+        self.bc_dof_ids = empty(0)
         self.field_variables: Dict[str, ndarray] = {}
-        self.init_data_list()
-        self.create_global_stiffness()
-        self.apply_bcs()
+        self.init()
+        self.update_element_data()
+        self.assembly_global_stiffness()
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string_assembly(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     @show_running_time
-    def init_data_list(self) -> None:
+    def init(self) -> None:
         # 初始化 self.element_data_list
         elements = self.props.elements
         nodes = self.props.nodes
         sections = self.props.sections
         materials = self.props.materials
         dof = self.props.dof
+        timer = self.timer
         dimension = nodes.dimension
         self.total_dof_number = len(nodes) * len(dof.names)
 
         for material in materials:
             self.materials_dict[material.name] = material
 
         for section in sections:
@@ -76,130 +88,113 @@
             material = self.materials_dict[section.material_name]
             material_data = get_material_data(material=material,
                                               dimension=dimension,
                                               option=section.type)
 
             for element_id in element_ids:
                 connectivity = elements[element_id]
-                node_coords = array(nodes.get_items_by_ids(list(connectivity)))
+                node_coords = array(nodes.get_items_by_ids(list(connectivity)), dtype=DTYPE)
                 iso_element_type = get_iso_element_type(node_coords)
                 iso_element_shape = iso_element_shape_dict[iso_element_type]
                 element_data = get_element_data(element_id=element_id,
                                                 iso_element_shape=iso_element_shape,
                                                 connectivity=connectivity,
                                                 node_coords=node_coords,
                                                 section=section,
                                                 dof=dof,
                                                 material=material,
-                                                material_data=material_data)
+                                                material_data=material_data,
+                                                timer=timer)
 
                 element_data.assembly_conn = array(nodes.get_indices_by_ids(list(connectivity)))
                 element_data.create_element_dof_ids()
 
                 self.element_data_list.append(element_data)
 
         # 初始化 self.bc_data_list
         bcs = self.props.bcs
         for bc in bcs:
             bc_data = get_bc_data(bc=bc, dof=dof, nodes=nodes)
             self.bc_data_list.append(bc_data)
 
-        # 初始化 RHS: self.fext
-        self.fext = zeros(self.total_dof_number)
+        bc_dof_ids = []
+        for bc_data in self.bc_data_list:
+            for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
+                bc_dof_ids.append(dof_id)
+        self.bc_dof_ids = array(bc_dof_ids)
+
+        # 初始化 rhs, fext, fint, dof_solution, ddof_solution
+        self.fext = zeros(self.total_dof_number, dtype=DTYPE)
+        self.fint = zeros(self.total_dof_number, dtype=DTYPE)
+        self.dof_solution = zeros(self.total_dof_number, dtype=DTYPE)
+        self.ddof_solution = zeros(self.total_dof_number, dtype=DTYPE)
 
-    def create_global_stiffness(self) -> None:
+    def assembly_global_stiffness(self) -> None:
         val = []
         row = []
         col = []
 
         for element_data in self.element_data_list:
             element_dof_ids = element_data.element_dof_ids
             element_dof_number = element_data.element_dof_number
             row += [r for r in repeat(element_dof_ids, element_dof_number)]
             for _ in range(element_dof_number):
                 col += [c for c in element_dof_ids]
-            val += [v for v in element_data.stiffness.reshape(element_dof_number * element_dof_number)]
+            val += [v for v in element_data.element_stiffness.reshape(element_dof_number * element_dof_number)]
 
-        self.global_stiffness = coo_matrix((array(val), (array(row), array(col))),
+        self.global_stiffness = coo_matrix((array(val, dtype=DTYPE), (array(row, dtype=DTYPE), array(col, dtype=DTYPE))),
                                            shape=(self.total_dof_number, self.total_dof_number)).tocsc()
 
-        # 以下代码采用 numpy.append 方法，处理可变对象时效率非常低，不建议使用
+    def assembly_fint(self) -> None:
+        self.fint = zeros(self.total_dof_number, dtype=DTYPE)
+        for element_data in self.element_data_list:
+            self.fint[element_data.element_dof_ids] += element_data.element_fint
 
-        # val = array([], dtype=float)
-        # row = array([], dtype=int)
-        # col = array([], dtype=int)
-        #
-        # for element_data in self.element_data_list:
-        #     element_dof_ids = element_data.element_dof_ids
-        #     element_dof_number = element_data.element_dof_number
-        #     row = append(row, repeat(element_dof_ids, element_dof_number))
-        #     for i in range(element_dof_number):
-        #         col = append(col, element_dof_ids)
-        #     val = append(val, element_data.stiffness.reshape(element_dof_number * element_dof_number))
-        #
-        # self.global_stiffness = coo_matrix((val, (row, col)), shape=(self.total_dof_number, self.total_dof_number))
+    def update_element_data(self) -> None:
+        dof_solution = self.dof_solution
+        ddof_solution = self.ddof_solution
+        for element_data in self.element_data_list:
+            element_data.update_element_dof_values(dof_solution)
+            element_data.update_element_ddof_values(ddof_solution)
+            element_data.update_material_state()
+            element_data.update_element_stiffness()
+            element_data.update_element_fint()
 
-    def apply_bcs(self) -> None:
-        penalty = 1.0e16
-        for bc_data in self.bc_data_list:
-            for dof_id, dof_value in zip(bc_data.dof_ids, bc_data.dof_values):
-                self.global_stiffness[dof_id, dof_id] += penalty
-                self.fext[dof_id] += dof_value * penalty
+    def update_element_stiffness(self) -> None:
+        for element_data in self.element_data_list:
+            element_data.update_element_stiffness()
 
-    @show_running_time
-    def update_field_variables(self, solution: ndarray) -> None:
-        self.dof_solution = solution
-        nodes_number = len(self.props.nodes)
+    def update_element_data_without_stiffness(self) -> None:
+        dof_solution = self.dof_solution
+        ddof_solution = self.ddof_solution
+        for element_data in self.element_data_list:
+            element_data.update_element_dof_values(dof_solution)
+            element_data.update_element_ddof_values(ddof_solution)
+            element_data.update_material_state()
+            element_data.update_element_fint()
+
+    def update_element_state_variables(self) -> None:
+        for element_data in self.element_data_list:
+            element_data.update_element_state_variables()
 
+    def update_element_field_variables(self) -> None:
         for element_data in self.element_data_list:
-            element_data.update_field_variables(solution)
+            element_data.update_element_field_variables()
+
+    def assembly_field_variables(self) -> None:
+        nodes_number = len(self.props.nodes)
 
         for output in self.props.outputs:
             if output.type == 'vtk':
                 for field_name in output.field_outputs:
                     self.field_variables[field_name] = zeros(nodes_number)
                     nodes_count = zeros(nodes_number)
                     for element_data in self.element_data_list:
                         assembly_conn = element_data.assembly_conn
-                        self.field_variables[field_name][assembly_conn] += element_data.average_field_variables[
-                            field_name]
+                        self.field_variables[field_name][assembly_conn] += \
+                            element_data.average_field_variables[field_name]
                         nodes_count[assembly_conn] += 1.0
                     self.field_variables[field_name] = self.field_variables[field_name] / nodes_count
 
-        # for field_name in self.props.outputs[0].field_outputs:
-        #     self.field_variables[field_name] = zeros((nodes_number, 3))
-        #     nodes_count = zeros(nodes_number)
-        #     for element_data in self.element_data_list:
-        #         assembly_conn = element_data.assembly_conn
-        #         self.field_variables[field_name][assembly_conn] += element_data.average_field_variables[field_name]
-        #         nodes_count[assembly_conn] += 1.0
-        #     self.field_variables[field_name] = self.field_variables[field_name]/nodes_count.reshape(-1, 1)
-
-
-@show_running_time
-def main():
-    from pyfem.solvers.get_solver_data import get_solver_data
-
-    props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
-    props.verify()
-    # props.show()
-    assembly = Assembly(props)
-
-    # x, info = gmres(A.toarray(), b, tol=1e-16)
-
-    solver_data = get_solver_data(assembly, props.solver)
-
-    solver_data.solve()
-
-    solution = solver_data.solution
-
-    assembly.update_field_variables(solution)
-
-    import pprint
-    pprint.pprint(assembly.field_variables)
-
-    # print(props.nodes.node_sets['top'])
-
 
 if __name__ == "__main__":
-    main()
+    pass
```

### Comparing `pyfem-0.0.8/src/pyfem/bc/BaseBC.py` & `pyfem-0.0.9/src/pyfem/bc/BaseBC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.8/src/pyfem/bc/DirichletBC.py` & `pyfem-0.0.9/src/pyfem/bc/DirichletBC.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def show(self) -> None:
         print(self.to_string())
 
     def create_dof_values(self) -> None:
         bc_node_sets = self.bc.node_sets
         bc_node_ids = []
         for bc_node_set in bc_node_sets:
-            bc_node_ids += self.nodes.node_sets[bc_node_set]
+            bc_node_ids += list(self.nodes.node_sets[bc_node_set])
 
         # 如果发现施加当前边界条件的点集中有重复的点则抛出异常
         if len(bc_node_ids) != len(set(bc_node_ids)):
             error_msg = f'{type(self).__name__} {self.bc.name} contains repeat nodes\n'
             error_msg += f'Please check the input file'
             raise NotImplementedError(error_style(error_msg))
         else:
```

### Comparing `pyfem-0.0.8/src/pyfem/bc/get_bc_data.py` & `pyfem-0.0.9/src/pyfem/bc/get_bc_data.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.8/src/pyfem/elements/BaseElement.py` & `pyfem-0.0.9/src/pyfem/elements/BaseElement.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,56 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from typing import List, Dict
 
 from numpy import (dot, empty, array, ndarray)
 from numpy.linalg import (det, inv)
 
 from pyfem.elements.IsoElementShape import IsoElementShape
+from pyfem.fem.Timer import Timer
+from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.visualization import object_dict_to_string_ndarray
 from pyfem.utils.wrappers import show_running_time
 
 
 class BaseElement:
-    def __init__(self, element_id: int, iso_element_shape: IsoElementShape, connectivity: ndarray,
+    def __init__(self, element_id: int,
+                 iso_element_shape: IsoElementShape,
+                 connectivity: ndarray,
                  node_coords: ndarray) -> None:
         self.element_id: int = element_id  # 用户自定义的节点编号
         self.iso_element_shape: IsoElementShape = iso_element_shape
         self.connectivity: ndarray = connectivity  # 对应用户定义的节点编号
         self.assembly_conn: ndarray = empty(0)  # 对应系统组装时的节点序号
         self.node_coords: ndarray = node_coords
-        self.gp_jacobis: ndarray = empty(0)
-        self.gp_jacobi_invs: ndarray = empty(0)
-        self.gp_jacobi_dets: ndarray = empty(0)
+        self.gp_jacobis: ndarray = empty(0, dtype=DTYPE)
+        self.gp_jacobi_invs: ndarray = empty(0, dtype=DTYPE)
+        self.gp_jacobi_dets: ndarray = empty(0, dtype=DTYPE)
+        self.gp_weight_times_jacobi_dets: ndarray = empty(0, dtype=DTYPE)
         self.dof: Dof = None  # type: ignore
         self.dof_names: List[str] = []
-        self.element_dof_ids: List[int] = []  # 对应系统组装时的自由度序号
-        self.element_dof_values: ndarray = empty(0)  # 对应系统组装时的自由度的值
         self.element_dof_number: int = 0  # 单元自由度总数
+        self.element_dof_ids: List[int] = []  # 对应系统组装时的自由度序号
+        self.element_dof_values: ndarray = empty(0, dtype=DTYPE)  # 对应系统组装时的自由度的值
+        self.element_ddof_values: ndarray = empty(0, dtype=DTYPE)  # 对应系统组装时的自由度增量的值
+        self.element_fint: ndarray = empty(0, dtype=DTYPE)  # 对应系统组装时的内力值
         self.material: Material = None  # type: ignore
         self.section: Section = None  # type: ignore
         self.material_data: BaseMaterial = None  # type: ignore
-        self.stiffness: ndarray = empty(0)
-        self.gp_state_variables: ndarray = empty(0)
-        self.field_variable_dict: Dict[str, List[str]] = {}
+        self.timer: Timer = None  # type: ignore
+        self.element_stiffness: ndarray = empty(0, dtype=DTYPE)
+        self.gp_ddsddes: ndarray = empty(0, dtype=DTYPE)
+        self.gp_state_variables: List[Dict[str, ndarray]] = [{} for _ in range(self.iso_element_shape.gp_number)]
+        self.gp_state_variables_new: List[Dict[str, ndarray]] = [{} for _ in range(self.iso_element_shape.gp_number)]
         self.gp_field_variables: Dict[str, ndarray] = {}
         self.average_field_variables: Dict[str, ndarray] = {}
         self.cal_jacobi()
 
     def to_string(self, level: int = 1) -> str:
         return object_dict_to_string_ndarray(self, level)
 
@@ -62,40 +75,43 @@
         # self.jacobi_inv = array(self.jacobi_inv)
         # self.jacobi_det = array(self.jacobi_det)
 
         # 以下代码为采用numpy高维矩阵乘法的计算方法，计算效率高，但要注意矩阵维度的变化
         self.gp_jacobis = dot(self.node_coords.transpose(), self.iso_element_shape.gp_shape_gradients).swapaxes(0, 1)
         self.gp_jacobi_invs = inv(self.gp_jacobis)
         self.gp_jacobi_dets = det(self.gp_jacobis)
+        self.gp_weight_times_jacobi_dets = self.iso_element_shape.gp_weights * self.gp_jacobi_dets
 
     def create_element_dof_ids(self) -> None:
         for node_index in self.assembly_conn:
             for dof_id, _ in enumerate(self.dof_names):
                 self.element_dof_ids.append(node_index * len(self.dof_names) + dof_id)
 
-    def update_field_variables(self, solution: ndarray) -> None:
+    def create_gp_b_matrices(self) -> None:
         pass
 
+    def update_element_dof_values(self, global_dof_values: ndarray) -> None:
+        self.element_dof_values = global_dof_values[self.element_dof_ids]
 
-@show_running_time
-def main():
-    from pyfem.assembly.Assembly import iso_element_shape_dict
-    from pyfem.io.Properties import Properties
+    def update_element_ddof_values(self, global_ddof_values: ndarray) -> None:
+        self.element_ddof_values = global_ddof_values[self.element_dof_ids]
 
-    props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
+    def update_material_state(self) -> None:
+        pass
 
-    elements = props.elements
-    nodes = props.nodes
+    def update_element_stiffness(self) -> None:
+        pass
 
-    base_elements = []
+    def update_element_fint(self) -> None:
+        pass
 
-    for element_id, connectivity in elements.items():
-        node_coords = array(nodes.get_items_by_ids(list(connectivity)))
-        base_element = BaseElement(element_id, iso_element_shape_dict['quad4'], connectivity, node_coords)
-        base_elements.append(base_element)
+    def update_element_state_variables(self) -> None:
+        pass
 
-    print(base_elements[0].to_string())
+    def update_element_field_variables(self) -> None:
+        pass
 
 
 if __name__ == "__main__":
-    main()
+    pass
+    # a = array([[0,0],[0.125,0.125]])
+    # inv(a)
```

### Comparing `pyfem-0.0.8/src/pyfem/elements/IsoElementDiagram.py` & `pyfem-0.0.9/src/pyfem/elements/IsoElementDiagram.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 class IsoElementDiagram:
+    """
+    等参元的形状示意图
+    """
+
     line2 = r"""
     0---------------1
             +-->x0"""
 
     line3 = r"""
     0-------1-------2
             +-->x0"""
@@ -12,14 +16,23 @@
     * *
     *   *
     *     *
     x1      *
     |         *
     0--x0 * * * 1"""
 
+    tria6 = r"""
+    2
+    * *
+    *   *
+    5     4
+    x1      *
+    |         *
+    0--x0 3 * * 1"""
+
     quad4 = r"""
     3---------------2
     |       x1      |
     |       |       |
     |       +--x0   |
     |               |
     |               |
@@ -78,12 +91,25 @@
     |   |     +--x0 |   |
     |   3-----------+---2
     |  /            |  /
     | /             | /
     |/              |/
     0---------------1"""
 
+    hex20 = r"""
+            7-------14------6
+           /|              /|
+         15 |     x2 x1  13 |
+         /  19    | /    /  18
+        4---+---12|/----5   |
+        |   |     +--x0 |   |
+        |   3-------10--+---2
+        16 /            17 /
+        |11             | 9
+        |/              |/
+        0-------8-------1"""
+
 
 if __name__ == "__main__":
     print(IsoElementDiagram.quad4)
     print(IsoElementDiagram.tetra4)
     print(IsoElementDiagram.hex8)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.0.8/src/pyfem/elements/SolidPlaneSmallStrain.py` & `pyfem-0.0.9/src/pyfem/elements/SolidPlaneSmallStrain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,19 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
+from copy import deepcopy
+
 from numpy import array, empty, zeros, dot, ndarray, average
 
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.elements.IsoElementShape import IsoElementShape
+from pyfem.fem.Timer import Timer
+from pyfem.fem.constants import DTYPE
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 
@@ -14,84 +22,116 @@
     def __init__(self, element_id: int,
                  iso_element_shape: IsoElementShape,
                  connectivity: ndarray,
                  node_coords: ndarray,
                  section: Section,
                  dof: Dof,
                  material: Material,
-                 material_data: BaseMaterial) -> None:
+                 material_data: BaseMaterial,
+                 timer: Timer) -> None:
 
         super().__init__(element_id, iso_element_shape, connectivity, node_coords)
+
         self.dof = dof
         self.dof_names = ['u1', 'u2']
-        self.field_variable_dict = {
-            'strain': ['E11', 'E22', 'E12'],
-            'stress': ['S11', 'S22', 'S12']
-        }
         if dof.names != self.dof_names:
             error_msg = f'{dof.names} is not the supported dof of {type(self).__name__} element'
             raise NotImplementedError(error_style(error_msg))
-        self.element_dof_number = len(self.dof_names) * self.iso_element_shape.nodes_number
+        element_dof_number = len(self.dof_names) * self.iso_element_shape.nodes_number
+        self.element_dof_number = element_dof_number
+        self.element_dof_values = zeros(element_dof_number, dtype=DTYPE)
+        self.element_ddof_values = zeros(element_dof_number, dtype=DTYPE)
+        self.element_fint = zeros(element_dof_number, dtype=DTYPE)
         self.material = material
         self.section = section
         self.material_data = material_data
-        self.gp_b_matrices = empty(0)
-        self.stiffness = empty(0)
-        self.update_gp_b_matrices()
-        self.update_stiffness()
+        self.timer = timer
+        self.gp_b_matrices = empty(0, dtype=DTYPE)
+        self.gp_stresses = empty(0, dtype=DTYPE)
+        self.element_stiffness = empty(0, dtype=DTYPE)
+        self.create_gp_b_matrices()
 
-    def update_gp_b_matrices(self) -> None:
-
-        self.gp_b_matrices = zeros(shape=(self.iso_element_shape.gp_number, 3, self.element_dof_number))
+    def create_gp_b_matrices(self) -> None:
+        self.gp_b_matrices = zeros(shape=(self.iso_element_shape.gp_number, 3, self.element_dof_number), dtype=DTYPE)
 
         for igp, (gp_shape_gradient, gp_jacobi_inv) in \
                 enumerate(zip(self.iso_element_shape.gp_shape_gradients, self.gp_jacobi_invs)):
             gp_dhdx = dot(gp_shape_gradient, gp_jacobi_inv)
             for i, val in enumerate(gp_dhdx):
                 self.gp_b_matrices[igp, 0, i * 2] = val[0]
                 self.gp_b_matrices[igp, 1, i * 2 + 1] = val[1]
                 self.gp_b_matrices[igp, 2, i * 2] = val[1]
                 self.gp_b_matrices[igp, 2, i * 2 + 1] = val[0]
 
-    def update_stiffness(self) -> None:
-        self.stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number))
+    def update_material_state(self) -> None:
+        gp_number = self.iso_element_shape.gp_number
+        gp_b_matrices = self.gp_b_matrices
+        gp_state_variables = self.gp_state_variables
+        element_dof_values = self.element_dof_values
+        element_ddof_values = self.element_ddof_values
+        gp_state_variables_new = self.gp_state_variables_new
+        element_id = self.element_id
+        timer = self.timer
+
+        gp_ddsddes = []
+        gp_stresses = []
 
-        ddsdde = self.material_data.get_tangent()
-        gp_weights = self.iso_element_shape.gp_weights
-        gp_jacobi_dets = self.gp_jacobi_dets
+        for i in range(gp_number):
+            gp_strain = dot(gp_b_matrices[i], element_dof_values)
+            gp_dstrain = dot(gp_b_matrices[i], element_ddof_values)
+            gp_ddsdde, gp_stress = self.material_data.get_tangent(state_variable=gp_state_variables[i],
+                                                                  state_variable_new=gp_state_variables_new[i],
+                                                                  state=gp_strain,
+                                                                  dstate=gp_dstrain,
+                                                                  element_id=element_id,
+                                                                  igp=i,
+                                                                  ntens=3,
+                                                                  ndi=2,
+                                                                  nshr=1,
+                                                                  timer=timer)
+            gp_ddsddes.append(gp_ddsdde)
+            gp_stresses.append(gp_stress)
+
+        self.gp_ddsddes = array(gp_ddsddes, dtype=DTYPE)
+        self.gp_stresses = array(gp_stresses, dtype=DTYPE)
+
+    def update_element_stiffness(self) -> None:
+        self.element_stiffness = zeros(shape=(self.element_dof_number, self.element_dof_number), dtype=DTYPE)
+
+        gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
         gp_b_matrices = self.gp_b_matrices
         gp_number = self.iso_element_shape.gp_number
+        gp_ddsddes = self.gp_ddsddes
 
         for i in range(gp_number):
-            self.stiffness += dot(gp_b_matrices[i].transpose(), dot(ddsdde, gp_b_matrices[i])) * gp_weights[i] * \
-                              gp_jacobi_dets[i]
+            self.element_stiffness += dot(gp_b_matrices[i].transpose(), dot(gp_ddsddes[i], gp_b_matrices[i])) * \
+                                      gp_weight_times_jacobi_dets[i]
 
-    def update_field_variables(self, solution: ndarray) -> None:
+    def update_element_fint(self) -> None:
+        gp_weight_times_jacobi_dets = self.gp_weight_times_jacobi_dets
         gp_b_matrices = self.gp_b_matrices
         gp_number = self.iso_element_shape.gp_number
-        ddsdde = self.material_data.get_tangent()
+        gp_stresses = self.gp_stresses
 
-        self.element_dof_values = solution[self.element_dof_ids]
-
-        gp_strains = []
-        gp_stresses = []
+        self.element_fint = zeros(self.element_dof_number, dtype=DTYPE)
         for i in range(gp_number):
-            gp_strain = dot(gp_b_matrices[i], self.element_dof_values)
-            gp_stress = dot(ddsdde, gp_strain)
-            gp_strains.append(gp_strain)
-            gp_stresses.append(gp_stress)
+            self.element_fint += dot(gp_b_matrices[i].transpose(), gp_stresses[i]) * gp_weight_times_jacobi_dets[i]
+
+    def update_element_state_variables(self) -> None:
+        self.gp_state_variables = deepcopy(self.gp_state_variables_new)
 
-        self.gp_field_variables['strain'] = array(gp_strains)
-        self.gp_field_variables['stress'] = array(gp_stresses)
+    def update_element_field_variables(self) -> None:
+        gp_stresses = self.gp_stresses
+        gp_strains = dot(self.gp_b_matrices, self.element_dof_values)
 
-        # self.average_field_variables['strain'] = average(self.gp_field_variables['strain'], axis=0)
-        # self.average_field_variables['stress'] = average(self.gp_field_variables['stress'], axis=0)
+        average_strain = average(gp_strains, axis=0)
+        average_stress = average(gp_stresses, axis=0)
 
-        average_strain = average(self.gp_field_variables['strain'], axis=0)
-        average_stress = average(self.gp_field_variables['stress'], axis=0)
+        self.gp_field_variables['strain'] = gp_strains
+        self.gp_field_variables['stress'] = gp_stresses
 
         self.average_field_variables['E11'] = average_strain[0]
         self.average_field_variables['E22'] = average_strain[1]
         self.average_field_variables['E12'] = average_strain[2]
         self.average_field_variables['S11'] = average_stress[0]
         self.average_field_variables['S22'] = average_stress[1]
         self.average_field_variables['S12'] = average_stress[2]
```

### Comparing `pyfem-0.0.8/src/pyfem/elements/get_element_data.py` & `pyfem-0.0.9/src/pyfem/elements/get_element_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,49 @@
 from numpy import ndarray
 
 from pyfem.elements.BaseElement import BaseElement
 from pyfem.elements.IsoElementShape import IsoElementShape
 from pyfem.elements.SolidPlaneSmallStrain import SolidPlaneSmallStrain
+from pyfem.elements.SolidVolumeSmallStrain import SolidVolumeSmallStrain
+from pyfem.fem.Timer import Timer
 from pyfem.io.Dof import Dof
 from pyfem.io.Material import Material
 from pyfem.io.Section import Section
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.utils.colors import error_style
 
 element_data_dict = {
     'SolidPlaneStressSmallStrain': SolidPlaneSmallStrain,
-    'SolidPlaneStrainSmallStrain': SolidPlaneSmallStrain
+    'SolidPlaneStrainSmallStrain': SolidPlaneSmallStrain,
+    'SolidVolumeSmallStrain': SolidVolumeSmallStrain
 }
 
 
+# @trace_calls
 def get_element_data(element_id: int,
                      iso_element_shape: IsoElementShape,
                      connectivity: ndarray,
                      node_coords: ndarray,
                      section: Section,
                      dof: Dof,
                      material: Material,
-                     material_data: BaseMaterial) -> BaseElement:
+                     material_data: BaseMaterial,
+                     timer: Timer) -> BaseElement:
     class_name = f'{section.category}{section.type}{section.option}'.strip().replace(' ', '')
 
     if class_name in element_data_dict:
         return element_data_dict[class_name](element_id=element_id,
                                              iso_element_shape=iso_element_shape,
                                              connectivity=connectivity,
                                              node_coords=node_coords,
                                              section=section,
                                              dof=dof,
                                              material=material,
-                                             material_data=material_data)
+                                             material_data=material_data,
+                                             timer=timer)
     else:
         error_msg = f'{class_name} element is not supported.\n'
         error_msg += f'The allowed element types are {list(element_data_dict.keys())}.'
         raise NotImplementedError(error_style(error_msg))
 
 
 if __name__ == "__main__":
```

### Comparing `pyfem-0.0.8/src/pyfem/elements/get_iso_element_type.py` & `pyfem-0.0.9/src/pyfem/elements/get_iso_element_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         if element_node_number == 4:
             return 'tetra4'
         elif element_node_number == 5:
             return 'pyramid5'
         elif element_node_number == 6:
             return 'prism6'
         elif element_node_number == 8:
-            return 'hexa8'
+            return 'hex8'
         elif element_node_number == 18:
             return 'prism18'
         elif element_node_number == 20:
             return 'hex20'
         else:
             error_msg = f'no 3D element with {element_node_number} nodes available'
             raise NotImplementedError(error_style(error_msg))
```

### Comparing `pyfem-0.0.8/src/pyfem/io/BC.py` & `pyfem-0.0.9/src/pyfem/io/BC.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.8/src/pyfem/io/Dof.py` & `pyfem-0.0.9/src/pyfem/io/Dof.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.8/src/pyfem/io/Material.py` & `pyfem-0.0.9/src/pyfem/io/Material.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-from typing import Optional, List, Tuple, Dict
+# -*- coding: utf-8 -*-
+"""
+
+"""
+from typing import List, Tuple, Dict
 
 from pyfem.utils.colors import error_style
 from pyfem.utils.visualization import object_dict_to_string
 
 
 class Material:
     """
     Material类用于存储配置文件中定义的材料属性。
-    当 self.is_read_only = True 时：
 
-    1. Material 类的所有属性在首次被赋非None值后不能再被修改和删除，
-
-    2. 此时许可的属性关键字存储在self.slots中。
+    当 self.is_read_only = True 时：
+        1. Material 类的所有属性在首次被赋非None值后不能再被修改和删除，
+        2. 此时许可的属性关键字存储在self.slots中。
     """
     is_read_only: bool = True
     slots: Tuple = ('name', 'category', 'type', 'data')
     allowed_keys_values: Dict = {
-        'category': [None, 'Elastic'],
-        'type': [None, 'Isotropic']
+        'category': [None, 'Elastic', 'Plastic'],
+        'type': [None, 'Isotropic', 'IsotropicHardening', 'KinematicHardening']
     }
 
     def __init__(self) -> None:
-        self.name: Optional[str] = None
-        self.category: Optional[str] = None
-        self.type: Optional[str] = None
-        self.data: Optional[List[float]] = None
+        self.name: str = None  # type: ignore
+        self.category: str = None  # type: ignore
+        self.type: str = None  # type: ignore
+        self.data: List[float] = None  # type: ignore
 
     def __setattr__(self, key, value) -> None:
         if self.is_read_only:
             if key not in self.slots:
                 error_msg = f'{key} is not an allowable attribute keyword of {type(self).__name__}'
                 raise AttributeError(error_style(error_msg))
```

### Comparing `pyfem-0.0.8/src/pyfem/io/Mesh.py` & `pyfem-0.0.9/src/pyfem/io/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.8/src/pyfem/io/Output.py` & `pyfem-0.0.9/src/pyfem/io/Output.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.8/src/pyfem/io/Properties.py` & `pyfem-0.0.9/src/pyfem/io/Properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,16 +26,15 @@
     1. Properties 类的所有属性在首次被赋非None值后不能再被修改和删除，
 
     2. 此时许可的属性关键字存储在self.slots中。
     """
     is_read_only: bool = True
     slots: Tuple = (
         'work_path', 'input_file', 'toml', 'title', 'mesh', 'dof', 'materials', 'sections', 'bcs',
-        'solver',
-        'outputs', 'nodes', 'elements')
+        'solver', 'outputs', 'nodes', 'elements')
 
     def __init__(self) -> None:
         self.work_path: Path = None  # type: ignore
         self.input_file: Path = None  # type: ignore
         self.toml: Dict = None  # type: ignore
         self.title: str = None  # type: ignore
         self.mesh: Mesh = None  # type: ignore
@@ -107,14 +106,17 @@
             if key in allowed_keys:
                 self.mesh.__setattr__(key, item)
             else:
                 raise AttributeError(self.key_error_message(key, self.mesh))
         if self.mesh.type == 'gmsh':
             self.set_nodes_from_gmsh()
             self.set_elements_from_gmsh()
+        if self.mesh.type == 'abaqus':
+            self.set_nodes_from_abaqus()
+            self.set_elements_from_abaqus()
 
     def set_dofs(self, dofs_dict: Dict) -> None:
         self.dof = Dof()
         allowed_keys = self.dof.__dict__.keys()
         for key, item in dofs_dict.items():
             if key in allowed_keys:
                 self.dof.__setattr__(key, item)
@@ -193,14 +195,33 @@
         if gmsh_path.is_absolute():  # 判断 self.mesh.file 是不是绝对路径
             abs_gmsh_file = gmsh_path
         else:  # 如果 self.mesh.file 不是绝对路径，则用工作目录 self.work_path 补全为绝对路径
             abs_gmsh_file = self.work_path.joinpath(gmsh_path)
         self.elements = ElementSet()
         self.elements.read_gmsh_file(abs_gmsh_file, self.sections)
 
+    def set_nodes_from_abaqus(self):
+        inp_path = Path(self.mesh.file)
+        if inp_path.is_absolute():  # 判断 self.mesh.file 是不是绝对路径
+            abs_inp_path = inp_path
+        else:  # 如果 self.mesh.file 不是绝对路径，则用工作目录 self.work_path 补全为绝对路径
+            abs_inp_path = self.work_path.joinpath(inp_path)
+        self.nodes = NodeSet()
+        self.nodes.read_inp_file(abs_inp_path)
+        self.nodes.update_indices()
+
+    def set_elements_from_abaqus(self):
+        inp_path = Path(self.mesh.file)
+        if inp_path.is_absolute():  # 判断 self.mesh.file 是不是绝对路径
+            abs_inp_file = inp_path
+        else:  # 如果 self.mesh.file 不是绝对路径，则用工作目录 self.work_path 补全为绝对路径
+            abs_inp_file = self.work_path.joinpath(inp_path)
+        self.elements = ElementSet()
+        self.elements.read_inp_file(abs_inp_file, self.sections)
+
     @staticmethod
     def key_error_message(key: Any, obj: Any) -> str:
         return error_style(f'{key} is not an allowable attribute keyword of {type(obj).__name__}')
 
     def read_file(self, filename: Union[Path, str]) -> None:
         """
         读取 .toml 格式的配置文件。
```

### Comparing `pyfem-0.0.8/src/pyfem/io/Section.py` & `pyfem-0.0.9/src/pyfem/io/Section.py`

 * *Files identical despite different names*

### Comparing `pyfem-0.0.8/src/pyfem/io/arguments.py` & `pyfem-0.0.9/src/pyfem/io/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     # 添加帮助选项
     parser.add_argument('-h', '--help', action='help', default=SUPPRESS,
                         help='Show this help message and exit.')
 
     # 添加版本选项
     parser.add_argument('-v', '--version', action='version', help='Show program\'s version number and exit.',
-                        version='pyfem 0.0.8')
+                        version='pyfem 0.0.9')
 
     # 解析命令行参数
     args = parser.parse_args()
 
     # 如果未指定程序输入文件，则打印帮助并退出
     if not args.i:
         print('--------------------------------------')
```

### Comparing `pyfem-0.0.8/src/pyfem/materials/BaseMaterial.py` & `pyfem-0.0.9/src/pyfem/io/Solver.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from typing import Optional
+# -*- coding: utf-8 -*-
+"""
 
-from numpy import ndarray, dot, empty
+"""
+from pyfem.utils.visualization import object_dict_to_string
 
-from pyfem.io.Material import Material
-from pyfem.utils.visualization import object_dict_to_string_ndarray
 
-
-class BaseMaterial:
-    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
-        self.material: Material = material
-        self.dimension: int = dimension
-        self.option: Optional[str] = option
-        self.ddsdde: ndarray = empty(0)
+class Solver:
+    def __init__(self) -> None:
+        self.type: str = None  # type: ignore
+        self.option: str = None  # type: ignore
+        self.total_time: float = 1.0
+        self.start_time: float = 0.0
+        self.max_increment: int = 100
+        self.initial_dtime: float = 1.0
+        self.max_dtime: float = 1.0
+        self.min_dtime: float = 0.001
+        self.dtype: str = 'float64'
 
     def to_string(self, level: int = 1) -> str:
-        return object_dict_to_string_ndarray(self, level)
+        return object_dict_to_string(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
-    def get_stress(self, strain: ndarray) -> ndarray:
-        sigma = dot(self.ddsdde, strain)
-        return sigma
 
-    def get_tangent(self) -> ndarray:
-        return self.ddsdde
+if __name__ == "__main__":
+    solver = Solver()
+    print(solver.__dict__.keys())
+    print(solver)
+    print(solver.to_string())
```

### Comparing `pyfem-0.0.8/src/pyfem/materials/ElasticIsotropic.py` & `pyfem-0.0.9/src/pyfem/materials/ElasticIsotropic.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,182 +1,202 @@
-from typing import Optional, Tuple
-
-from numpy import array, outer, diag, float64, ndarray
-
-from pyfem.io.Material import Material
-from pyfem.materials.BaseMaterial import BaseMaterial
-from pyfem.utils.colors import error_style
-
-
-class ElasticIsotropic(BaseMaterial):
-    allowed_option = ['PlaneStress', 'PlaneStrain', None]
-
-    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
-        super().__init__(material, dimension, option)
-        self.create_tangent()
-
-    def create_tangent(self):
-        young = self.material.data[0]
-        poisson = self.material.data[1]
-
-        if self.option in self.allowed_option:
-            if self.dimension == 3:
-                self.option = None
-            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.option)
-        else:
-            error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
-            raise NotImplementedError(error_style(error_msg))
-
-
-def get_lame_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> Tuple[float, float]:
-    r"""
-    Compute Lamé parameters from Young's modulus and Poisson's ratio.
-
-    The relationship between Lamé parameters and Young's modulus, Poisson's
-    ratio (see [1],[2]):
-
-    .. math::
-        \lambda = {\nu E \over (1+\nu)(1-2\nu)},\qquad \mu = {E \over 2(1+\nu)}
-
-    The plain stress hypothesis:
-
-    .. math::
-       \bar\lambda = {2\lambda\mu \over \lambda + 2\mu}
-
-    [1] I.S. Sokolnikoff: Mathematical Theory of Elasticity. New York, 1956.
-
-    [2] T.J.R. Hughes: The Finite Element Method, Linear Static and Dynamic
-    Finite Element Analysis. New Jersey, 1987.
-    """
-    mu = young / (2.0 * (1.0 + poisson))
-    lam = young * poisson / ((1.0 + poisson) * (1.0 - 2.0 * poisson))
-
-    if plane == 'PlaneStress':
-        lam = 2 * lam * mu / (lam + 2 * mu)
-
-    return lam, mu
-
-
-def get_stiffness_from_lame(dim: int, lam: float, mu: float) -> ndarray:
-    r"""
-    Compute stiffness tensor corresponding to Lamé parameters.
-
-    .. math::
-        {\bf D}_{(2D)} = \begin{bmatrix} \lambda + 2\mu & \lambda & 0\\
-        \lambda & \lambda + 2\mu & 0\\ 0 & 0 & \mu \end{bmatrix}
-
-    .. math::
-        {\bf D}_{(3D)} = \begin{bmatrix} \lambda + 2\mu & \lambda &
-        \lambda & 0 & 0 & 0\\ \lambda & \lambda + 2\mu & \lambda & 0 & 0 & 0 \\
-        \lambda & \lambda & \lambda + 2\mu & 0 & 0 & 0 \\ 0 & 0 & 0 & \mu & 0 &
-        0 \\ 0 & 0 & 0 & 0 & \mu & 0 \\ 0 & 0 & 0 & 0 & 0 & \mu\\ \end{bmatrix}
-    """
-    sym = (dim + 1) * dim // 2
-    o = array([1.] * dim + [0.] * (sym - dim), dtype=float64)
-    oot = outer(o, o)
-    do1 = diag(o + 1.0)
-
-    lam_array = array(lam)[..., None, None]
-    mu_array = array(mu)[..., None, None]
-    return lam_array * oot + mu_array * do1
-
-
-def get_stiffness_from_young_poisson(dim: int, young: float, poisson: float, plane: Optional[str]) -> ndarray:
-    """
-    Compute stiffness tensor corresponding to Young's modulus and Poisson's
-    ratio.
-    """
-
-    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
-
-    return get_stiffness_from_lame(dim, lam, mu)
-
-
-def get_stiffness_from_lame_mixed(dim: int, lam: float, mu: float) -> ndarray:
-    r"""
-    Compute stiffness tensor corresponding to Lamé parameters for mixed
-    formulation.
-
-    .. math::
-        {\bf D}_{(2D)} = \begin{bmatrix} \widetilde\lambda + 2\mu &
-        \widetilde\lambda & 0\\ \widetilde\lambda & \widetilde\lambda + 2\mu &
-        0\\ 0 & 0 & \mu \end{bmatrix}
-
-    .. math::
-        {\bf D}_{(3D)} = \begin{bmatrix} \widetilde\lambda + 2\mu &
-        \widetilde\lambda & \widetilde\lambda & 0 & 0 & 0\\ \widetilde\lambda &
-        \widetilde\lambda + 2\mu & \widetilde\lambda & 0 & 0 & 0 \\
-        \widetilde\lambda & \widetilde\lambda & \widetilde\lambda + 2\mu & 0 &
-        0 & 0 \\ 0 & 0 & 0 & \mu & 0 & 0 \\ 0 & 0 & 0 & 0 & \mu & 0 \\ 0 & 0 &
-        0 & 0 & 0 & \mu\\ \end{bmatrix}
-
-    where
-
-    .. math::
-       \widetilde\lambda = -{2\over 3} \mu
-    """
-    lam = - 2.0 / 3.0 * mu
-
-    return get_stiffness_from_lame(dim, lam, mu)
-
-
-def get_stiffness_from_young_poisson_mixed(dim: int, young: float, poisson: float, plane) -> ndarray:
-    """
-    Compute stiffness tensor corresponding to Young's modulus and Poisson's
-    ratio for mixed formulation.
-    """
-    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
-
-    return get_stiffness_from_lame_mixed(dim, lam, mu)
-
-
-def get_bulk_from_lame(lam: float, mu: float) -> float:
-    r"""
-    Compute bulk modulus from Lamé parameters.
-
-    .. math::
-        \gamma = \lambda + {2 \over 3} \mu
-    """
-    return lam + 2.0 * mu / 3.0
-
-
-def get_bulk_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> float:
-    """
-    Compute bulk modulus corresponding to Young's modulus and Poisson's ratio.
-    """
-    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
-
-    return get_bulk_from_lame(lam, mu)
-
-
-def get_lame_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
-    """
-    Compute Lamé parameters from an isotropic stiffness tensor.
-    """
-    lam = float(stiffness[..., 0, 1])
-    mu = float(stiffness[..., -1, -1])
-    if plane == 'PlaneStress':
-        lam = - 2.0 * mu * lam / (lam - 2.0 * mu)
-
-    return lam, mu
-
-
-def get_young_poisson_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
-    """
-    Compute Young's modulus and Poisson's ratio from an isotropic stiffness
-    tensor.
-    """
-    lam, mu = get_lame_from_stiffness(stiffness, plane)
-    young = (3 * lam * mu + 2 * mu ** 2) / (lam + mu)
-    poisson = lam / (2 * lam + 2 * mu)
-
-    return young, poisson
-
-
-if __name__ == "__main__":
-    from pyfem.io.Properties import Properties
-
-    props = Properties()
-    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
-
-    material_data = ElasticIsotropic(props.materials[0], 3)
-    print(material_data.to_string())
+# -*- coding: utf-8 -*-
+"""
+
+"""
+from typing import Optional, Tuple, Dict
+
+from numpy import array, outer, diag, float64, ndarray, dot
+
+from pyfem.fem.Timer import Timer
+from pyfem.fem.constants import DTYPE
+from pyfem.io.Material import Material
+from pyfem.materials.BaseMaterial import BaseMaterial
+from pyfem.utils.colors import error_style
+
+
+class ElasticIsotropic(BaseMaterial):
+    allowed_option = ['Volume', 'PlaneStress', 'PlaneStrain', None]
+
+    def __init__(self, material: Material, dimension: int, option: Optional[str] = None) -> None:
+        super().__init__(material, dimension, option)
+        self.create_tangent()
+
+    def create_tangent(self):
+        young = self.material.data[0]
+        poisson = self.material.data[1]
+
+        if self.option in self.allowed_option:
+            if self.dimension == 3:
+                self.option = None
+            self.ddsdde = get_stiffness_from_young_poisson(self.dimension, young, poisson, self.option)
+        else:
+            error_msg = f'{self.option} is not the allowed options {self.allowed_option}'
+            raise NotImplementedError(error_style(error_msg))
+
+    def get_tangent(self, state_variable: Dict[str, ndarray],
+                    state_variable_new: Dict[str, ndarray],
+                    state: ndarray,
+                    dstate: ndarray,
+                    element_id: int,
+                    igp: int,
+                    ntens: int,
+                    ndi: int,
+                    nshr: int,
+                    timer: Timer) -> Tuple[ndarray, ndarray]:
+        strain = state
+        stress = dot(self.ddsdde, strain)
+        return self.ddsdde, stress
+
+
+def get_lame_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> Tuple[float, float]:
+    r"""
+    Compute Lamé parameters from Young's modulus and Poisson's ratio.
+
+    The relationship between Lamé parameters and Young's modulus, Poisson's
+    ratio (see [1],[2]):
+
+    .. math::
+        \lambda = {\nu E \over (1+\nu)(1-2\nu)},\qquad \mu = {E \over 2(1+\nu)}
+
+    The plain stress hypothesis:
+
+    .. math::
+       \bar\lambda = {2\lambda\mu \over \lambda + 2\mu}
+
+    [1] I.S. Sokolnikoff: Mathematical Theory of Elasticity. New York, 1956.
+
+    [2] T.J.R. Hughes: The Finite Element Method, Linear Static and Dynamic
+    Finite Element Analysis. New Jersey, 1987.
+    """
+    mu = young / (2.0 * (1.0 + poisson))
+    lam = young * poisson / ((1.0 + poisson) * (1.0 - 2.0 * poisson))
+
+    if plane == 'PlaneStress':
+        lam = 2 * lam * mu / (lam + 2 * mu)
+
+    return lam, mu
+
+
+def get_stiffness_from_lame(dim: int, lam: float, mu: float) -> ndarray:
+    r"""
+    Compute stiffness tensor corresponding to Lamé parameters.
+
+    .. math::
+        {\bf D}_{(2D)} = \begin{bmatrix} \lambda + 2\mu & \lambda & 0\\
+        \lambda & \lambda + 2\mu & 0\\ 0 & 0 & \mu \end{bmatrix}
+
+    .. math::
+        {\bf D}_{(3D)} = \begin{bmatrix} \lambda + 2\mu & \lambda &
+        \lambda & 0 & 0 & 0\\ \lambda & \lambda + 2\mu & \lambda & 0 & 0 & 0 \\
+        \lambda & \lambda & \lambda + 2\mu & 0 & 0 & 0 \\ 0 & 0 & 0 & \mu & 0 &
+        0 \\ 0 & 0 & 0 & 0 & \mu & 0 \\ 0 & 0 & 0 & 0 & 0 & \mu\\ \end{bmatrix}
+    """
+    sym = (dim + 1) * dim // 2
+    o = array([1.] * dim + [0.] * (sym - dim), dtype=DTYPE)
+    oot = outer(o, o)
+    do1 = diag(o + 1.0)
+
+    lam_array = array(lam, dtype=DTYPE)[..., None, None]
+    mu_array = array(mu, dtype=DTYPE)[..., None, None]
+    return lam_array * oot + mu_array * do1
+
+
+def get_stiffness_from_young_poisson(dim: int, young: float, poisson: float, plane: Optional[str]) -> ndarray:
+    """
+    Compute stiffness tensor corresponding to Young's modulus and Poisson's
+    ratio.
+    """
+
+    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
+
+    return get_stiffness_from_lame(dim, lam, mu)
+
+
+def get_stiffness_from_lame_mixed(dim: int, lam: float, mu: float) -> ndarray:
+    r"""
+    Compute stiffness tensor corresponding to Lamé parameters for mixed
+    formulation.
+
+    .. math::
+        {\bf D}_{(2D)} = \begin{bmatrix} \widetilde\lambda + 2\mu &
+        \widetilde\lambda & 0\\ \widetilde\lambda & \widetilde\lambda + 2\mu &
+        0\\ 0 & 0 & \mu \end{bmatrix}
+
+    .. math::
+        {\bf D}_{(3D)} = \begin{bmatrix} \widetilde\lambda + 2\mu &
+        \widetilde\lambda & \widetilde\lambda & 0 & 0 & 0\\ \widetilde\lambda &
+        \widetilde\lambda + 2\mu & \widetilde\lambda & 0 & 0 & 0 \\
+        \widetilde\lambda & \widetilde\lambda & \widetilde\lambda + 2\mu & 0 &
+        0 & 0 \\ 0 & 0 & 0 & \mu & 0 & 0 \\ 0 & 0 & 0 & 0 & \mu & 0 \\ 0 & 0 &
+        0 & 0 & 0 & \mu\\ \end{bmatrix}
+
+    where
+
+    .. math::
+       \widetilde\lambda = -{2\over 3} \mu
+    """
+    lam = - 2.0 / 3.0 * mu
+
+    return get_stiffness_from_lame(dim, lam, mu)
+
+
+def get_stiffness_from_young_poisson_mixed(dim: int, young: float, poisson: float, plane) -> ndarray:
+    """
+    Compute stiffness tensor corresponding to Young's modulus and Poisson's
+    ratio for mixed formulation.
+    """
+    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
+
+    return get_stiffness_from_lame_mixed(dim, lam, mu)
+
+
+def get_bulk_from_lame(lam: float, mu: float) -> float:
+    r"""
+    Compute bulk modulus from Lamé parameters.
+
+    .. math::
+        \gamma = \lambda + {2 \over 3} \mu
+    """
+    return lam + 2.0 * mu / 3.0
+
+
+def get_bulk_from_young_poisson(young: float, poisson: float, plane: Optional[str]) -> float:
+    """
+    Compute bulk modulus corresponding to Young's modulus and Poisson's ratio.
+    """
+    lam, mu = get_lame_from_young_poisson(young, poisson, plane)
+
+    return get_bulk_from_lame(lam, mu)
+
+
+def get_lame_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
+    """
+    Compute Lamé parameters from an isotropic stiffness tensor.
+    """
+    lam = float(stiffness[..., 0, 1])
+    mu = float(stiffness[..., -1, -1])
+    if plane == 'PlaneStress':
+        lam = - 2.0 * mu * lam / (lam - 2.0 * mu)
+
+    return lam, mu
+
+
+def get_young_poisson_from_stiffness(stiffness: ndarray, plane: Optional[str]) -> Tuple[float, float]:
+    """
+    Compute Young's modulus and Poisson's ratio from an isotropic stiffness
+    tensor.
+    """
+    lam, mu = get_lame_from_stiffness(stiffness, plane)
+    young = (3 * lam * mu + 2 * mu ** 2) / (lam + mu)
+    poisson = lam / (2 * lam + 2 * mu)
+
+    return young, poisson
+
+
+if __name__ == "__main__":
+    from pyfem.io.Properties import Properties
+
+    props = Properties()
+    props.read_file(r'F:\Github\pyfem\examples\rectangle\rectangle.toml')
+
+    material_data = ElasticIsotropic(props.materials[0], 3)
+    print(material_data.ddsdde.dtype)
```

### Comparing `pyfem-0.0.8/src/pyfem/materials/get_material_data.py` & `pyfem-0.0.9/src/pyfem/materials/get_material_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from typing import Optional
 
 from pyfem.io.Material import Material
 from pyfem.materials.BaseMaterial import BaseMaterial
 from pyfem.materials.ElasticIsotropic import ElasticIsotropic
+from pyfem.materials.PlasticKinematicHardening import PlasticKinematicHardening
 from pyfem.utils.colors import error_style
 
 material_data_dict = {
-    'ElasticIsotropic': ElasticIsotropic
+    'ElasticIsotropic': ElasticIsotropic,
+    'PlasticKinematicHardening': PlasticKinematicHardening,
 }
 
 
 def get_material_data(material: Material, dimension: int, option: Optional[str] = None) -> BaseMaterial:
     class_name = f'{material.category}{material.type}'.strip().replace(' ', '')
 
     if class_name in material_data_dict:
```

### Comparing `pyfem-0.0.8/src/pyfem/mesh/NodeSet.py` & `pyfem-0.0.9/src/pyfem/mesh/NodeSet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
 from pathlib import Path
-from typing import List, Any, Dict, Union
+from typing import List, Dict, Union
 
 import meshio  # type: ignore
-import numpy as np
+from numpy import array, ndarray
 
 from pyfem.utils.IntKeyDict import IntKeyDict
 from pyfem.utils.logger import get_logger
 from pyfem.utils.wrappers import show_running_time
+from pyfem.fem.constants import DTYPE
 
 logger = get_logger()
 
 
 class NodeSet(IntKeyDict):
 
     def __init__(self) -> None:
@@ -68,30 +69,67 @@
                         cell_nodes = mesh.cells_dict[mesh_type][element_id]
                         for node_id in cell_nodes:
                             self.add_to_sets_by_id(cell_name, node_id)
 
         for key in self.node_sets:
             self.node_sets[key] = list(set(self.node_sets[key]))
 
+    def read_inp_file(self, file_name: Union[Path, str]) -> None:
+        """
+        从 ABAQUS inp文件中读取节点信息。
+            1. 首先使用meshio.read函数读取文件，获取网格数据。
+            2. 然后根据读取到的单元类型确定节点的维度。
+            3. 接着遍历节点和单元，将节点添加到节点集合中。
+            4. 最后，将节点集合中的重复节点去重。
+        """
+        logger.info(f"Reading nodes from {file_name}")
+        # 从inp文件读取mesh信息
+        mesh = meshio.read(file_name, file_format="abaqus")
+
+        # keywords_1d = ['line']
+        # keywords_2d = ['triangle', 'quad']
+        keywords_3d = ['pyramid', 'hexahedron', 'wedge', 'tetra']
+
+        self.dimension = 2
+
+        # If any 3D mesh type is found, set the dimension to 3
+        for cell_name, cell_dict in mesh.cell_sets_dict.items():
+            for mesh_type in cell_dict.keys():
+                if mesh_type in keywords_3d:
+                    self.dimension = 3
+
+        for node_id, coords in enumerate(mesh.points.astype(DTYPE)):
+            self.add_item_by_id(node_id, coords[:self.dimension])
+
+        self.node_sets = mesh.point_sets
+
     def add_to_sets_by_id(self, node_set_name: str, node_id: int) -> None:
         if node_set_name not in self.node_sets:
             self.node_sets[node_set_name] = [int(node_id)]
         else:
             self.node_sets[node_set_name].append(int(node_id))
 
-    def get_coords_by_ids(self, node_ids: List[int]) -> np.ndarray[Any, np.dtype[np.float64]]:
-        return np.array(self.get_items_by_ids(node_ids))
+    def get_coords_by_ids(self, node_ids: List[int]) -> ndarray:
+        return array(self.get_items_by_ids(node_ids))
 
 
 if __name__ == "__main__":
     from pyfem.utils.logger import set_logger
 
     set_logger()
 
     nodes = NodeSet()
-    os.chdir(r'/examples/rectangle')
-    # nodes.read_gmsh_file('rectangle100.msh')
-    nodes.read_gmsh_file('rectangle10000.msh')
-    # print(nodes.dimension)
-    # print(nodes.node_sets)
-    print(nodes.get_coords_by_ids([0, 1, 2]))
+    # os.chdir(r'/examples/rectangle')
+    # # nodes.read_gmsh_file('rectangle100.msh')
+    # nodes.read_gmsh_file('rectangle10000.msh')
+    # # print(nodes.dimension)
+    # # print(nodes.node_sets)
+    # print(nodes.get_coords_by_ids([0, 1, 2]))
+    # nodes.show()
+
+    os.chdir(r'F:\Github\pyfem\examples\specimen')
+    nodes.read_inp_file('Job-1.inp')
     nodes.show()
+    print(nodes.dimension)
+    print(nodes.node_sets)
+    print(nodes.get_coords_by_ids([0, 1, 2]).dtype)
+    # nodes.show()
```

### Comparing `pyfem-0.0.8/src/pyfem/solvers/BaseSolver.py` & `pyfem-0.0.9/src/pyfem/solvers/BaseSolver.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,18 +15,14 @@
         return object_dict_to_string_ndarray(self, level)
 
     def show(self) -> None:
         print(self.to_string())
 
     def run(self) -> None:
         self.solve()
-        self.update_field_variables()
 
     def solve(self) -> None:
         self.solution = empty(0)
 
-    def update_field_variables(self) -> None:
-        self.assembly.update_field_variables(self.solution)
-
 
 if __name__ == "__main__":
     pass
```

### Comparing `pyfem-0.0.8/src/pyfem/solvers/get_solver_data.py` & `pyfem-0.0.9/src/pyfem/solvers/get_solver_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from pyfem.assembly.Assembly import Assembly
 from pyfem.io.Solver import Solver
 from pyfem.solvers.BaseSolver import BaseSolver
 from pyfem.solvers.LinearSolver import LinearSolver
+from pyfem.solvers.NonlinearSolver import NonlinearSolver
 from pyfem.utils.colors import error_style
 
 solver_data_dict = {
-    'LinearSolver': LinearSolver
+    'LinearSolver': LinearSolver,
+    'NonlinearSolver': NonlinearSolver
 }
 
 
 def get_solver_data(assembly: Assembly, solver: Solver) -> BaseSolver:
     class_name = f'{solver.type}'.strip().replace(' ', '')
 
     if class_name in solver_data_dict:
```

### Comparing `pyfem-0.0.8/src/pyfem/utils/IntKeyDict.py` & `pyfem-0.0.9/src/pyfem/utils/IntKeyDict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+"""
+
+"""
 from typing import Dict, List, Any
 
 
 class IntKeyDict(dict):
     """
     关键字只能为整数（Integer）类型的字典，已经存在的键值无法通过赋值方法（__setitem__）更改。
     """
```

### Comparing `pyfem-0.0.8/src/pyfem/utils/colors.py` & `pyfem-0.0.9/src/pyfem/utils/colors.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+"""
+定义色彩关键字，用于对字符串着色。
+"""
 import os
 
 IS_COLORED = True
 
 if os.environ.get('TERM', '') != '' or IS_COLORED:
     CYAN = '\033[36m'
     MAGENTA = '\033[35m'
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.0.8/src/pyfem/utils/logger.py` & `pyfem-0.0.9/src/pyfem/utils/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import colorlog
 
 
 def set_logger(log_file: Optional[str] = None, level: int = logging.INFO) -> Optional[logging.Logger]:
     """
     设置 logging 模块的基础配置，并返回一个 logger 对象。
+
     :param log_file: 日志文件名，None 表示将日志输出到控制台
     :param level: 输出日志的最低级别，默认是 INFO 级别
     """
     # 创建 logger 对象
     logger = logging.getLogger()
 
     # 设置日志级别
```

### Comparing `pyfem-0.0.8/src/pyfem/utils/visualization.py` & `pyfem-0.0.9/src/pyfem/utils/visualization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+"""
+定义一些函数用于程序的可视化。
+"""
 from numpy import ndarray
 
 from pyfem.utils.colors import GREEN, BLUE, END
 
 
 def insert_spaces(n: int, text: str) -> str:
     lines = text.split('\n')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.0.8/src/pyfem/utils/wrappers.py` & `pyfem-0.0.9/src/pyfem/utils/wrappers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+# -*- coding: utf-8 -*-
+"""
+定义一些函数装饰器
+"""
 import inspect
 import time
 
 from pyfem.utils.colors import BOLD, MAGENTA, YELLOW, BLUE, END
 
 
 def show_running_time(func):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyfem-0.0.8/src/pyfem.egg-info/PKG-INFO` & `pyfem-0.0.9/src/pyfem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfem
-Version: 0.0.8
+Version: 0.0.9
 Summary: A finite element package for learning
 Home-page: https://github.com/sunwhale/pyfem
 Author: Jingyu Sun
 Author-email: sun.jingyu@outlook.com
 Project-URL: Bug Tracker, https://github.com/sunwhale/pyfem/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

