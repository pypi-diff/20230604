# Comparing `tmp/fitsnap3-3.1.0.2.tar.gz` & `tmp/fitsnap3-3.1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fitsnap3-3.1.0.2.tar", last modified: Tue May 23 19:13:34 2023, max compression
+gzip compressed data, was "fitsnap3-3.1.0.4.tar", last modified: Sun Jun  4 12:16:21 2023, max compression
```

## Comparing `fitsnap3-3.1.0.2.tar` & `fitsnap3-3.1.0.4.tar`

### file list

```diff
@@ -1,168 +1,168 @@
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/
--rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.1.0.2/LICENSE
--rw-rw-r--   0 drew      (1000) drew      (1000)    24931 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     3795 2023-05-23 19:10:15.000000 fitsnap3-3.1.0.2/README.md
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.750412 fitsnap3-3.1.0.2/fitsnap3/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2062 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3/__main__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3/fitsnap.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.754412 fitsnap3-3.1.0.2/fitsnap3.egg-info/
--rw-rw-r--   0 drew      (1000) drew      (1000)    24931 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/PKG-INFO
--rw-rw-r--   0 drew      (1000) drew      (1000)     5206 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/SOURCES.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/dependency_links.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/requires.txt
--rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-05-23 19:13:34.000000 fitsnap3-3.1.0.2/fitsnap3.egg-info/top_level.txt
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.754412 fitsnap3-3.1.0.2/fitsnap3lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.754412 fitsnap3-3.1.0.2/fitsnap3lib/calculators/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    18640 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1240 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/calculator_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     9650 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_base.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11388 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    25241 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    28349 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10427 2023-05-23 19:10:15.000000 fitsnap3-3.1.0.2/fitsnap3lib/fitsnap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3811 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/initialize.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.754412 fitsnap3-3.1.0.2/fitsnap3lib/io/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/error.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7650 2023-05-23 19:10:15.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/input.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      374 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.758412 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1645 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      905 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/output_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8636 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/outputs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7918 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/pace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14208 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/snap.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      287 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/template_output.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.762412 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.762412 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8163 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/ace.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      346 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     7408 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2209 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/calculator.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1057 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/custom.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      850 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/eshift.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2301 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/extras.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4860 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/groups.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      881 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/memory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1022 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/outfile.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      745 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/path.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1249 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/reference.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1633 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2064 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/section_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6824 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/sections.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.762412 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1136 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      497 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4495 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5562 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      506 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/ridge.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1611 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      387 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/template.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      986 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/io/sections/trainshift.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.762412 fitsnap3-3.1.0.2/fitsnap3lib/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.766412 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/__init__.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.766412 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4754 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pairwise.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6675 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pas.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12048 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    15987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/write.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.766412 fitsnap3-3.1.0.2/fitsnap3lib/lib/ridge_solver/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:51:51.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/ridge_solver/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      664 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/ridge_solver/regressor.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.770412 fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3813 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/setup.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.770412 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5076 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.770412 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2848 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19236 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/gen_labels.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      739 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/genlib.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.774412 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13938 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    12716 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/rpi_lib.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    13467 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/tree_method.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5423 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/wigner_couple.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.774412 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3788 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     3214 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14131 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1325 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    14611 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/young.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      354 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/parallel_output.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    37710 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/parallel_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.778412 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4024 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/ase_funcs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4513 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/json_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    17005 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/scrape.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      783 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/scraper_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      494 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/template_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    27319 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/vasp_scraper.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    19569 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/scrapers/xyz_scraper.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.778412 fitsnap3-3.1.0.2/fitsnap3lib/solvers/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2906 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/anl.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2984 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/ard.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    10116 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/bcs.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8379 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/jax.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/lasso.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/lreg.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5167 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/mcmc.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     4828 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/merr.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    39329 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/network.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/opt.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    43491 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/pytorch.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2064 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/ridge.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     2868 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/scalapack.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    24358 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1110 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/solver_factory.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1622 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/svd.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      187 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/template_solver.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1733 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/solvers/tensorflowsvd.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.782412 fitsnap3-3.1.0.2/fitsnap3lib/tools/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1743 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/configuration.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/dataframe_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8055 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/dataloaders.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1157 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/group_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     5519 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/lammps_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     8648 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/nn_tools.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     6083 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/tools/test_tools.py
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/fitsnap3lib/units/
--rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/__init__.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/conversion_finder.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/energy.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/force.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/length.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/mass.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/pressure.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/temperature.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      272 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/time.py
--rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.2/fitsnap3lib/units/units.py
--rw-rw-r--   0 drew      (1000) drew      (1000)     1096 2023-05-23 19:11:06.000000 fitsnap3-3.1.0.2/pyproject.toml
--rw-rw-r--   0 drew      (1000) drew      (1000)      220 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/setup.cfg
-drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-05-23 19:13:34.786412 fitsnap3-3.1.0.2/tests/
--rw-rw-r--   0 drew      (1000) drew      (1000)     3987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.2/tests/test_examples.py
--rw-rw-r--   0 drew      (1000) drew      (1000)    11801 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.2/tests/test_pytorch.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.313147 fitsnap3-3.1.0.4/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17775 2023-02-27 06:32:59.000000 fitsnap3-3.1.0.4/LICENSE
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24931 2023-06-04 12:16:21.313147 fitsnap3-3.1.0.4/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3795 2023-05-23 19:10:15.000000 fitsnap3-3.1.0.4/README.md
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.257147 fitsnap3-3.1.0.4/fitsnap3/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2232 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3/__main__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3/fitsnap.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.261147 fitsnap3-3.1.0.4/fitsnap3.egg-info/
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24931 2023-06-04 12:16:21.000000 fitsnap3-3.1.0.4/fitsnap3.egg-info/PKG-INFO
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5206 2023-06-04 12:16:21.000000 fitsnap3-3.1.0.4/fitsnap3.egg-info/SOURCES.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)        1 2023-06-04 12:16:21.000000 fitsnap3-3.1.0.4/fitsnap3.egg-info/dependency_links.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       92 2023-06-04 12:16:21.000000 fitsnap3-3.1.0.4/fitsnap3.egg-info/requires.txt
+-rw-rw-r--   0 drew      (1000) drew      (1000)       21 2023-06-04 12:16:21.000000 fitsnap3-3.1.0.4/fitsnap3.egg-info/top_level.txt
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.261147 fitsnap3-3.1.0.4/fitsnap3lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.265147 fitsnap3-3.1.0.4/fitsnap3lib/calculators/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/calculators/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    18728 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3lib/calculators/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1240 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/calculators/calculator_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     9650 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/calculators/lammps_base.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    11388 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/calculators/lammps_custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    25241 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/calculators/lammps_pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    28410 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3lib/calculators/lammps_snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10427 2023-05-23 19:10:15.000000 fitsnap3-3.1.0.4/fitsnap3lib/fitsnap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3811 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/initialize.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.265147 fitsnap3-3.1.0.4/fitsnap3lib/io/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)       36 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/error.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8060 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/input.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      374 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.269147 fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1645 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      905 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/output_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8636 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/outputs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7918 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/pace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14337 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/snap.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      287 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/template_output.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.273147 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.273147 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8163 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/ace.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      346 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/basic_calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     7408 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/bispectrum.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2209 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/calculator.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1057 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/custom.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      850 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/eshift.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2301 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/extras.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4860 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/groups.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      881 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/memory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1022 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/outfile.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      745 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/path.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1249 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/reference.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1633 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2064 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/section_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6824 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/sections.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.277147 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1136 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      497 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4495 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5562 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      506 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1611 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      387 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/template.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      986 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/io/sections/trainshift.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.277147 fitsnap3-3.1.0.4/fitsnap3lib/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.281147 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/__init__.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.281147 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/descriptors/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/descriptors/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3488 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/descriptors/bessel.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4754 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/descriptors/g3b.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2078 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10950 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/pairwise.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6675 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/pas.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12048 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    15987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/write.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.281147 fitsnap3-3.1.0.4/fitsnap3lib/lib/ridge_solver/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-04-28 14:51:51.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/ridge_solver/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      664 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/ridge_solver/regressor.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.285147 fitsnap3-3.1.0.4/fitsnap3lib/lib/scalapack_solver/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/scalapack_solver/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2679 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/scalapack_solver/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3813 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/scalapack_solver/setup.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.289147 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5076 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.289147 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2848 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19236 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/gen_labels.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      739 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/genlib.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.289147 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/lib/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/lib/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13938 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    12716 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/rpi_lib.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      839 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    13467 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/tree_method.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5423 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/wigner_couple.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.293147 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-28 06:43:16.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3788 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3214 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14131 2023-04-28 14:39:05.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1325 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    14611 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/young.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      354 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/parallel_output.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    38404 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3lib/parallel_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.293147 fitsnap3-3.1.0.4/fitsnap3lib/scrapers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/scrapers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4024 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/scrapers/ase_funcs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4513 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/scrapers/json_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    17005 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/scrapers/scrape.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      783 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/scrapers/scraper_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      494 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/scrapers/template_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    27319 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/scrapers/vasp_scraper.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    19569 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/scrapers/xyz_scraper.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.305147 fitsnap3-3.1.0.4/fitsnap3lib/solvers/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3229 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/anl.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2984 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/ard.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    10116 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/bcs.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8379 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/jax.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/lasso.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6138 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/lreg.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5167 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/mcmc.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     4828 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/merr.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    39329 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/network.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2164 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/opt.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    44134 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/pytorch.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2131 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/ridge.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     2868 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/scalapack.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    24358 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1110 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/solver_factory.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1985 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/svd.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      187 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/template_solver.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1733 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/solvers/tensorflowsvd.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.305147 fitsnap3-3.1.0.4/fitsnap3lib/tools/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/tools/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1743 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/tools/configuration.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    21068 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/tools/dataframe_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8055 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/tools/dataloaders.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1157 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/fitsnap3lib/tools/group_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     5519 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/tools/lammps_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     8648 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/tools/nn_tools.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     6083 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/tools/test_tools.py
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.309147 fitsnap3-3.1.0.4/fitsnap3lib/units/
+-rw-rw-r--   0 drew      (1000) drew      (1000)        0 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/__init__.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1615 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/conversion_finder.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      300 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/energy.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      426 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/force.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      303 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/length.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      356 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/mass.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      244 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/pressure.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      207 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/temperature.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      272 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/time.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)      951 2023-02-27 06:33:02.000000 fitsnap3-3.1.0.4/fitsnap3lib/units/units.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)     1096 2023-06-04 12:14:52.000000 fitsnap3-3.1.0.4/pyproject.toml
+-rw-rw-r--   0 drew      (1000) drew      (1000)      220 2023-06-04 12:16:21.313147 fitsnap3-3.1.0.4/setup.cfg
+drwxrwxr-x   0 drew      (1000) drew      (1000)        0 2023-06-04 12:16:21.313147 fitsnap3-3.1.0.4/tests/
+-rw-rw-r--   0 drew      (1000) drew      (1000)     3987 2023-04-28 14:38:35.000000 fitsnap3-3.1.0.4/tests/test_examples.py
+-rw-rw-r--   0 drew      (1000) drew      (1000)    11801 2023-05-19 23:49:38.000000 fitsnap3-3.1.0.4/tests/test_pytorch.py
```

### Comparing `fitsnap3-3.1.0.2/LICENSE` & `fitsnap3-3.1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/PKG-INFO` & `fitsnap3-3.1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.1.0.2
+Version: 3.1.0.4
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991
```

### Comparing `fitsnap3-3.1.0.2/README.md` & `fitsnap3-3.1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3/__main__.py` & `fitsnap3-3.1.0.4/fitsnap3/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,20 +27,29 @@
 #     Gary Saavedra (Sandia National Labs)
 #     Peter Schultz (Sandia National Labs)
 #     Laura Swiler (Sandia National Labs)
 # <!-----------------END-HEADER------------------------------------->
 
 from fitsnap3lib.fitsnap import FitSnap
 
+try:
+    # stubs = 0 MPI is active
+    stubs = 0
+    from mpi4py import MPI
+    comm = MPI.COMM_WORLD
+except ModuleNotFoundError:
+    stubs = 1
+    comm = None
+
 
 def main():
     # Instantiate single fitsnap instance for traditional flow of control.
     # This will create an internal parallel tools instance which will detect
     # availability of MPI for parallelization.
-    snap = FitSnap()
+    snap = FitSnap(comm=comm)
     snap.scrape_configs(delete_scraper=True)
     snap.process_configs(delete_data=True)
     # Good practice after a large parallel operation is to impose a barrier.
     snap.pt.all_barrier()
     snap.perform_fit()
     snap.write_output()
     """
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3.egg-info/PKG-INFO` & `fitsnap3-3.1.0.4/fitsnap3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fitsnap3
-Version: 3.1.0.2
+Version: 3.1.0.4
 Summary: Molecular Machine Learning Interface
 Author-email: Drew Rohskopf <adrohsk@sandia.gov>
 Maintainer-email: Drew Rohskopf <adrohsk@sandia.gov>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3.egg-info/SOURCES.txt` & `fitsnap3-3.1.0.4/fitsnap3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/calculators/calculator.py` & `fitsnap3-3.1.0.4/fitsnap3lib/calculators/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from fitsnap3lib.parallel_tools import double_size, DistributedList, stubs #, ParallelTools
+#from fitsnap3lib.parallel_tools import double_size, DistributedList, stubs #, ParallelTools
+from fitsnap3lib.parallel_tools import DistributedList
 #from fitsnap3lib.io.input import Config
 #from fitsnap3lib.io.output import output
 import numpy as np
 import pandas as pd
 
 
 #config = Config()
@@ -112,15 +113,15 @@
 #                b_len += self.number_of_files_per_node * 6
 
             a_width = self.get_width()
             assert isinstance(a_width, int)
 
             # TODO: Pick a method to get RAM accurately (pt.get_ram() seems to get RAM wrong on Blake)
 
-            a_size = ( (a_len * a_width) + (dgrad_len * a_width) ) * double_size
+            a_size = ( (a_len * a_width) + (dgrad_len * a_width) ) * self.pt.double_size
             if self.config.args.verbose:
                 self.pt.single_print(">>> Matrix of descriptors and descriptor derivatives takes up ", 
                               "{:.4f}".format(100 * a_size / self.config.sections["MEMORY"].memory),
                               "% of the total memory:", 
                               "{:.4f}".format(self.config.sections["MEMORY"].memory*1e-9), "GB")
             if a_size / self.pt.get_ram() > 0.5 and not self.config.sections["MEMORY"].override:
                 raise MemoryError("The descriptor matrix is larger than 50% of your RAM. \n Aborting...!")
@@ -192,15 +193,15 @@
 #                b_len += self.number_of_files_per_node * 6
 
             a_width = 2 # types and numneighs
             neighlist_width = self.get_width()
             assert isinstance(neighlist_width, int)
 
             # TODO: Pick a method to get RAM accurately (pt.get_ram() seems to get RAM wrong on Blake)
-            a_size = (neighlist_len * neighlist_width + 2 * c_len * c_width) * double_size
+            a_size = (neighlist_len * neighlist_width + 2 * c_len * c_width) * self.pt.double_size
             if self.config.args.verbose:
                 self.pt.single_print(">>> Matrix of data takes up ", "{:.4f}".format(100 * a_size / self.config.sections["MEMORY"].memory),
                               "% of the total memory:", "{:.4f}".format(self.config.sections["MEMORY"].memory*1e-9), "GB")
             if a_size / self.pt.get_ram() > 0.5 and not self.config.sections["MEMORY"].override:
                 raise MemoryError("The data memory larger than 50% of your RAM. \n Aborting...!")
             elif a_size / self.pt.get_ram() > 0.5 and self.config.sections["MEMORY"].override:
                 self.pt.single_print("Warning: > 50 % RAM. I hope you know what you are doing!")
@@ -270,15 +271,15 @@
             if self.config.sections["CALCULATOR"].stress:
                 a_len += self.number_of_files_per_node * 6
 
             a_width = self.get_width()
             assert isinstance(a_width, int)
 
             # TODO: Pick a method to get RAM accurately (pt.get_ram() seems to get RAM wrong on Blake)
-            a_size = a_len * a_width * double_size
+            a_size = a_len * a_width * self.pt.double_size
             if self.config.args.verbose:
                 self.pt.single_print(">>> Matrix of descriptors takes up ", "{:.4f}".format(100 * a_size / self.config.sections["MEMORY"].memory),
                               "% of the total memory:", "{:.4f}".format(self.config.sections["MEMORY"].memory*1e-9), "GB") #, "on rank", "{:d}".format(self.pt._rank))
             if a_size / self.pt.get_ram() > 0.5 and not self.config.sections["MEMORY"].override:
                 raise MemoryError("The descriptor matrix is larger than 50% of your RAM. \n Aborting...!")
             elif a_size / self.pt.get_ram() > 0.5 and self.config.sections["MEMORY"].override:
                 self.pt.single_print("Warning: > 50 % RAM. I hope you know what you are doing!")
@@ -315,15 +316,15 @@
 
         Args:
             allgather: Whether to gather lists on all nodes or just the head node.
         """   
         for key in self.pt.fitsnap_dict.keys():
             if isinstance(self.pt.fitsnap_dict[key], DistributedList):
                 self.pt.gather_fitsnap(key)
-                if self.pt.fitsnap_dict[key] is not None and stubs != 1:
+                if self.pt.fitsnap_dict[key] is not None and self.pt.stubs != 1:
                     self.pt.fitsnap_dict[key] = [item for sublist in self.pt.fitsnap_dict[key] for item in sublist]
                 elif self.pt.fitsnap_dict[key] is not None:
                     self.pt.fitsnap_dict[key] = self.pt.fitsnap_dict[key].get_list()
 
     #@pt.rank_zero
     def extras(self):
         @self.pt.rank_zero
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/calculators/calculator_factory.py` & `fitsnap3-3.1.0.4/fitsnap3lib/calculators/calculator_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_base.py` & `fitsnap3-3.1.0.4/fitsnap3lib/calculators/lammps_base.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_custom.py` & `fitsnap3-3.1.0.4/fitsnap3lib/calculators/lammps_custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_pace.py` & `fitsnap3-3.1.0.4/fitsnap3lib/calculators/lammps_pace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/calculators/lammps_snap.py` & `fitsnap3-3.1.0.4/fitsnap3lib/calculators/lammps_snap.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,14 +246,16 @@
         ncols_snap = ncols_bispectrum + ncols_reference
         # index = pt.fitsnap_dict['a_indices'][self._i]
         index = 0
         dindex = self.distributed_index
 
         lmp_snap = _extract_compute_np(self._lmp, "snap", 0, 2, (nrows_snap, ncols_snap))
 
+        #print(np.shape(lmp_snap))
+
         # We want first column to be 1, 0, ... 0.
         # Next columns are bispectrum components.
         # Take last column of `lmp_snap` as the `b` vector.
 
         # Get individual A matrices for this configuration.
 
         #print(np.shape(lmp_snap))
@@ -266,23 +268,23 @@
                 nrows += num_atoms
             if self.config.sections['CALCULATOR'].force:
                 nrows += 3*num_atoms
             if self.config.sections['CALCULATOR'].stress:
                 nrows += 6
             nd = np.shape(lmp_snap)[1]-1
             na = nrows #np.shape(lmp_snap)[0]
-            a = np.zeros((na, nd))
-            b = np.zeros(na)
-            w = np.zeros(na)
         else:
             nd = np.shape(lmp_snap)[1]
             na = np.shape(lmp_snap)[0]
-            a = np.zeros((na, nd))
-            b = np.zeros(na)
-            w = np.zeros(na)
+
+        if self.config.sections['BISPECTRUM'].bzeroflag and not self.config.sections['BISPECTRUM'].bikflag:
+            nd -= 1
+        a = np.zeros((na, nd))
+        b = np.zeros(na)
+        w = np.zeros(na)
 
         if (np.isinf(lmp_snap)).any() or (np.isnan(lmp_snap)).any():
             raise ValueError('Nan in computed data of file {} in group {}'.format(self._data["File"],
                                                                                   self._data["Group"]))
         irow = 0
         bik_rows = 1
         if self.config.sections['BISPECTRUM'].bikflag:
@@ -320,14 +322,15 @@
                 for atom in self._data["AtomTypes"]:
                     onehot_atoms[self.config.sections["BISPECTRUM"].type_mapping[atom]-1] += 1
                 onehot_atoms /= len(self._data["AtomTypes"])
                 b_sum_temp = np.concatenate((onehot_atoms, b_sum_temp), axis=1)
                 b_sum_temp.shape = (num_types * n_coeff + num_types)
 
             # Get matrix of descriptors (A).
+
             a[irow:irow+bik_rows] = b_sum_temp * self.config.sections["BISPECTRUM"].blank2J[np.newaxis, :]
 
             # Get vector of truths (b).
             ref_energy = lmp_snap[irow, icolref]
             b[irow:irow+bik_rows] = 0.0
             b[irow] = (energy - ref_energy) / num_atoms
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/fitsnap.py` & `fitsnap3-3.1.0.4/fitsnap3lib/fitsnap.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/initialize.py` & `fitsnap3-3.1.0.4/fitsnap3lib/initialize.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/input.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/input.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 
         # Generate random 128 bit hash to identify this fit on rank 0.
         if self.pt._rank == 0:
             self.hash = f"{random.getrandbits(128):032x}"
         else:
             self.hash = None
 
-    def parse_cmdline(self, arguments_lst=[]):
-        """ Parse command line args. """
+    def parse_cmdline(self, arguments_lst: list = []):
+        """ Parse command line args if using executable mode, or a list if using library mode. """
         parser = argparse.ArgumentParser(prog="fitsnap3")
         if (self.input is None):
             parser.add_argument("infile", action="store",
                                 help="Input file with bispectrum etc. options")
 
         # Optional args.
         parser.add_argument("--lammpslog", "-l", action="store_true", dest="lammpslog",
@@ -93,15 +93,22 @@
 
         # Check if building docs, in which case we revert to using Ta Linear example.
 
         for item in sys.argv:
             if (item=="build" or item=="html" or item=="source"):
                 # We're building docs in this case.
                 arguments_lst = arguments_lst=["../examples/Ta_Linear_JCP2014/Ta-example-nodump.in", "--overwrite"]
-        self.args = parser.parse_args(arguments_lst)
+        
+        if arguments_lst:
+            # If arg list is not empty we are feeding in arguments with library mode, and args should be parse 
+            # according to this list.
+            self.args = parser.parse_args(arguments_lst)
+        else:
+            # If arguments list is empty, we can parse the args like usual with executable mode.
+            self.args = parser.parse_args()
 
     def parse_config(self):
         tmp_config = configparser.ConfigParser(inline_comment_prefixes='#')
         tmp_config.optionxform = str
         if self.input is not None:
             if (isinstance(self.input, str)):
                 self.infile = self.input
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/custom.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/output_factory.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/output_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/outputs.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/outputs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/pace.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/pace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/outputs/snap.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/outputs/snap.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,38 +25,39 @@
     def write_lammps(self, coeffs):
         """
         Write LAMMPS-ready SNAP files.
         
         Args:
             coeffs: list of linear model coefficients.
         """
-        if self.config.sections["EXTRAS"].only_test != 1:
-            if self.config.sections["CALCULATOR"].calculator != "LAMMPSSNAP":
-                raise TypeError("SNAP output style must be paired with LAMMPSSNAP calculator")
-        with optional_open(self.config.sections["OUTFILE"].potential_name and
-                            self.config.sections["OUTFILE"].potential_name + '.snapcoeff', 'wt') as file:
-            file.write(_to_coeff_string(self.config, coeffs))
-        with optional_open(self.config.sections["OUTFILE"].potential_name and
-                            self.config.sections["OUTFILE"].potential_name + '.snapparam', 'wt') as file:
-            file.write(_to_param_string(self.config))
-        with optional_open(self.config.sections["OUTFILE"].potential_name and
-                            self.config.sections["OUTFILE"].potential_name + '.mod', 'wt') as file:
-            file.write(_to_potential_file(self.config))
-        if (self._tarball):
-            with optional_open("in.lammps", 'wt') as file:
-                file.write(_to_lammps_input())
-            # Package these files into a tarball
-            fp = tarfile.open(f"fit-{self.config.hash}.tar.gz", 'w:gz')
-            potname = self.config.sections["OUTFILE"].potential_name
-            potname_prefix = potname.split('/')[-1]
-            fp.add(potname + '.snapcoeff', arcname = potname_prefix + '.snapcoeff')
-            fp.add(potname + '.snapparam', arcname = potname_prefix + '.snapparam')
-            fp.add(potname + '.mod', arcname = potname_prefix)
-            fp.add("in.lammps")
-            fp.close()
+        if (coeffs is not None):
+            if self.config.sections["EXTRAS"].only_test != 1:
+                if self.config.sections["CALCULATOR"].calculator != "LAMMPSSNAP":
+                    raise TypeError("SNAP output style must be paired with LAMMPSSNAP calculator")
+            with optional_open(self.config.sections["OUTFILE"].potential_name and
+                                self.config.sections["OUTFILE"].potential_name + '.snapcoeff', 'wt') as file:
+                file.write(_to_coeff_string(self.config, coeffs))
+            with optional_open(self.config.sections["OUTFILE"].potential_name and
+                                self.config.sections["OUTFILE"].potential_name + '.snapparam', 'wt') as file:
+                file.write(_to_param_string(self.config))
+            with optional_open(self.config.sections["OUTFILE"].potential_name and
+                                self.config.sections["OUTFILE"].potential_name + '.mod', 'wt') as file:
+                file.write(_to_potential_file(self.config))
+            if (self._tarball):
+                with optional_open("in.lammps", 'wt') as file:
+                    file.write(_to_lammps_input())
+                # Package these files into a tarball
+                fp = tarfile.open(f"fit-{self.config.hash}.tar.gz", 'w:gz')
+                potname = self.config.sections["OUTFILE"].potential_name
+                potname_prefix = potname.split('/')[-1]
+                fp.add(potname + '.snapcoeff', arcname = potname_prefix + '.snapcoeff')
+                fp.add(potname + '.snapparam', arcname = potname_prefix + '.snapparam')
+                fp.add(potname + '.mod', arcname = potname_prefix)
+                fp.add("in.lammps")
+                fp.close()
 
     #@pt.rank_zero
     def write(self, coeffs, errors):
         """ Write both LAMMPS files and error files"""
         @self.pt.rank_zero
         def decorated_write():
             self.write_lammps(coeffs)
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/ace.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/ace.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/bispectrum.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/bispectrum.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/calculator.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/calculator.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/calculator_sections/custom.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/calculator_sections/custom.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/eshift.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/eshift.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/extras.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/extras.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/groups.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/groups.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/memory.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/memory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/outfile.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/outfile.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/path.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/path.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/reference.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/reference.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/scraper.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/section_factory.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/section_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/sections.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/sections.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/ard.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/ard.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/jax.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/network.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/network.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/pytorch.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/pytorch.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/solver_sections/solver.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/solver_sections/solver.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/io/sections/trainshift.py` & `fitsnap3-3.1.0.4/fitsnap3lib/io/sections/trainshift.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/bessel.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/descriptors/bessel.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/descriptors/g3b.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/descriptors/g3b.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/jax.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pairwise.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/pairwise.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pas.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/pas.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/pytorch.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/pytorch.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/neural_networks/write.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/neural_networks/write.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/ridge_solver/regressor.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/ridge_solver/regressor.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/scalapack.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/scalapack_solver/scalapack.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/scalapack_solver/setup.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/scalapack_solver/setup.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/coupling_coeffs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/descriptor_calc_local/convert_configs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/gen_labels.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/gen_labels.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/genlib.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/genlib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/lib/coupling_tree.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/lib/sylow_lib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/rpi_lib.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/rpi_lib.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/sym_ACE_settings.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/tree_method.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/tree_method.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/wigner_couple.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/wigner_couple.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/acecoeff_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/config_tool.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/potential.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/yamlpace_tools/yace_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/lib/sym_ACE/young.py` & `fitsnap3-3.1.0.4/fitsnap3lib/lib/sym_ACE/young.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/parallel_tools.py` & `fitsnap3-3.1.0.4/fitsnap3lib/parallel_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,23 @@
 import ctypes
 import signal
 from inspect import isclass
 from pkgutil import iter_modules
 from importlib import import_module
 from copy import deepcopy
 
-
+"""
 try:
     # stubs = 0 MPI is active
     stubs = 0
     from mpi4py import MPI
 except ModuleNotFoundError:
     stubs = 1
+"""
+
 
 def printf(*args, **kw):
     kw['flush'] = True
 
     if 'overwrite' in kw:
         del kw['overwrite']
         kw['end'] = ''
@@ -120,22 +122,23 @@
             return identity_decorator(*args, **kw)
     return check_if_rank_zero
 
 
 def dummy_function(*args, **kw):
     return None
 
-
+"""
 def stub_check(method):
     def stub_function(*args, **kw):
         if stubs == 0:
             return method(*args, **kw)
         else:
             return dummy_function(*args, **kw)
     return stub_function
+"""
 
 
 def print_lammps(method):
     def new_method(*args, **kw):
         printf(*args)
         return method(*args, **kw)
     return new_method
@@ -149,39 +152,51 @@
     Attributes:
         check_fitsnap_exist (bool): Checks whether fitsnap dictionaries exist before creating a new 
             one, set to `False` to allow recreating a dictionary.
     """
 
     def __init__(self, comm=None):
         self.check_fitsnap_exist = True # set to False if want to allow re-creating dictionary
-        if stubs == 0:
+        if comm is None:
+            self.stubs = 1
+        else:
+            self.stubs = 0
+
+        if self.stubs == 0:
+            from mpi4py import MPI
+            self.MPI = MPI
             if comm is None:
-                comm = MPI.COMM_WORLD
+                comm = self.MPI.COMM_WORLD
             self._comm = comm
             self._rank = self._comm.Get_rank()
             self._size = self._comm.Get_size()
             #print(f">>> Parallel tools comm rank {self._rank} size {self._size}: {self._comm}")
             # Set this to False if want to avoid shared arrays. This is helpful when using the library 
             # to loop over functions that create shared arrays, to avoid mem leaks.
             self.create_shared_bool = True
 
-        if stubs == 1:
+            self.double_size = self.MPI.DOUBLE.Get_size()
+
+        if self.stubs == 1:
             self._rank = 0
             self._size = 1
             self._comm = None
             self._sub_rank = 0
             self._sub_size = 1
             self._sub_comm = None
             self._sub_head_proc = 0
             self._node_index = 0
             self._number_of_nodes = 1
+            self.double_size = ctypes.sizeof(ctypes.c_double)
 
         self.killer = GracefulKiller(self._comm)
 
-        self._comm_split()
+        if self.stubs == 0:
+            self._comm_split()
+
         self._lmp = None
         self._seed = 0.0
         self._set_seed()
         self.shared_arrays = {}
         self.fitsnap_dict = {}
         self.logger = None
         self.pytest = False
@@ -198,17 +213,17 @@
         protected = ("_comm")
         if name in protected and hasattr(self, name):
             raise AttributeError(f"Overwriting {name} is not allowed.")
         else:
             super().__setattr__(name, value)
     """
 
-    @stub_check
+    #@stub_check
     def _comm_split(self):
-        self._sub_comm = self._comm.Split_type(MPI.COMM_TYPE_SHARED)
+        self._sub_comm = self._comm.Split_type(self.MPI.COMM_TYPE_SHARED)
         self._sub_rank = self._sub_comm.Get_rank()
         self._sub_size = self._sub_comm.Get_size()
         self._sub_head_proc = 0
         if self._sub_rank == 0:
             self._sub_head_proc = self._rank
         self._sub_head_proc = self._sub_comm.bcast(self._sub_head_proc)
         self._sub_head_procs = list(dict.fromkeys(self._comm.allgather(self._sub_head_proc)))
@@ -217,15 +232,15 @@
         self._node_index = self._sub_head_procs.index(self._sub_head_proc)
         self._number_of_nodes = len(self._sub_head_procs)
         self._micro_comm = self._comm.Split(self._rank)
 
     def _set_seed(self):
         if self._rank == 0.0:
             self._seed = randint(0, 1e5)
-        if stubs == 0:
+        if self.stubs == 0:
             self._seed = self._comm.bcast(self._seed)
 
     def get_seed(self):
         return self._seed
 
     def get_size(self):
         return self._size
@@ -315,44 +330,46 @@
                 return method(*args, **kw)
             return check_if_rank_zero
         else:
             return dummy_function
         
     def free(self):
         """ Free memory associated with all shared arrays. """
-        if not stubs:
+        if not self.stubs:
             for name in self.shared_arrays:
                 # There is no mpi4py native clean way to check if an array is
                 # already freed, so let's do try/except for now.
                 try:
                     self.shared_arrays[name].win.Free()
                 except:
                     pass
         else:
-            self.single_print("Trying to free a stubs array; doing nothing.")
+            #self.single_print("No need to free a stubs array.")
+            pass
 
     def create_shared_array(self, name, size1, size2=1, dtype='d', tm=0):
 
         if isinstance(name, str):
-            if (stubs == 0 and self.create_shared_bool):
+            if (self.stubs == 0 and self.create_shared_bool):
                 # If key exists, free the window memory to prevent memory leaks.
                 # TODO: Is there a way to check state of the window instead of the key?
-                if (name in self.shared_arrays and not stubs):
+                if (name in self.shared_arrays and not self.stubs):
                     try:
                         self.shared_arrays[name].win.Free()
                     except Exception as e:
                         self.single_print(f"Trouble deallocating shared array with name {name}: {e}.")
                 comms = [[self._comm, self._rank, self._size],
                          [self._sub_comm, self._sub_rank, self._sub_size],
                          [self._head_group_comm, self._node_index, self._number_of_nodes]]
 
                 self.shared_arrays[name] = SharedArray(size1, size2=size2,
                                                        dtype=dtype,
                                                        multinode=tm,
-                                                       comms=comms)
+                                                       comms=comms,
+                                                       MPI=self.MPI)
             else:   
                 self.shared_arrays[name] = StubsArray(size1, size2, dtype=dtype)
         else:
             raise TypeError("name must be a string")
 
     # @stub_check
     def add_2_fitsnap(self, name, an_object):
@@ -363,60 +380,64 @@
                 if name in self.fitsnap_dict:
                     #raise NameError("name is already in dictionary")
                     self.fitsnap_dict.pop(name)
             self.fitsnap_dict[name] = an_object
         else:
             raise TypeError("name must be a string")
 
-    @stub_check
+    #@stub_check
     def _bcast_fitsnap(self, name):
 
-        if self._sub_rank == 0:
-            if name not in self.fitsnap_dict:
-                raise NameError("Dictionary element not yet in fitsnap_dictionary")
-        else:
-            self.fitsnap_dict[name] = None
+        if self.stubs == 0:
+            if self._sub_rank == 0:
+                if name not in self.fitsnap_dict:
+                    raise NameError("Dictionary element not yet in fitsnap_dictionary")
+            else:
+                self.fitsnap_dict[name] = None
 
-        self.fitsnap_dict[name] = self._sub_comm.bcast(self.fitsnap_dict[name])
+            self.fitsnap_dict[name] = self._sub_comm.bcast(self.fitsnap_dict[name])
 
-    @stub_check
+    #@stub_check
     def gather_fitsnap(self, name, allgather:bool=None):
         """
         Gather distributed lists.
         Args:
-            allgather: If true then we allgather. When number of procs is large this can 
-                       result in large (but not prohibitive) memory usage, where each proc has 
-                       ~10 lists with size of number of configs.
+            allgather: If true then we allgather. When number of procs is large this will use more memory.
         """
-        if name not in self.fitsnap_dict:
-            raise NameError("Dictionary element not yet in fitsnap_dictionary")
-        # TODO: Make some sort of option to either gather or allgather.
-        #       It saves memory to simply gather, but allgather is useful in 
-        #       scenarios when using multiple instances in parallel, we might need 
-        #       the fitsnap dict on all procs.
-        # NOTE: When number of procs is large, allgather could quickly consume all memory.
-        #self.fitsnap_dict[name] = self._sub_comm.gather(self.fitsnap_dict[name], root=0)
-        self.fitsnap_dict[name] = self._sub_comm.allgather(self.fitsnap_dict[name])
+        if self.stubs == 0:
+            if name not in self.fitsnap_dict:
+                raise NameError("Dictionary element not yet in fitsnap_dictionary")
+            # TODO: Make some sort of option to either gather or allgather.
+            #       It saves memory to simply gather, but allgather is useful in 
+            #       scenarios when using multiple instances in parallel, we might need 
+            #       the fitsnap dict on all procs.
+            # NOTE: When number of procs is large, allgather could quickly consume all memory.
+            #self.fitsnap_dict[name] = self._sub_comm.gather(self.fitsnap_dict[name], root=0)
+            self.fitsnap_dict[name] = self._sub_comm.allgather(self.fitsnap_dict[name])
 
-    @stub_check
+    #@stub_check
     @_sub_rank_zero
     def gather_to_head_node(self, array):
-        return self._head_group_comm.allgather(array)
+        if self.stubs == 0:
+            return self._head_group_comm.allgather(array)
 
-    @stub_check
+    #@stub_check
     def gather_distributed_list(self, dist_list):
-        gathered_list = self._sub_comm.allgather(dist_list)
+        if self.stubs == 0:
+            gathered_list = self._sub_comm.allgather(dist_list)
 
-    @stub_check
+    #@stub_check
     def all_barrier(self):
-        self._comm.Barrier()
+        if self.stubs == 0:
+            self._comm.Barrier()
 
-    @stub_check
+    #@stub_check
     def sub_barrier(self):
-        self._sub_comm.Barrier()
+        if self.stubs == 0:
+            self._sub_comm.Barrier()
 
     def split_by_node(self, obj):
         if isinstance(obj, list):
             return obj[self._node_index::self._number_of_nodes]
         elif isinstance(obj, dict):
             for key in obj:
                 obj[key] = obj[key][self._node_index::self._number_of_nodes]
@@ -426,15 +447,15 @@
         elif isinstance(obj, SharedArray):
             scraped_length = obj.get_scraped_length()
             length = obj.get_node_length()
             lengths = np.zeros(self._number_of_nodes)
             difference = np.zeros(self._number_of_nodes)
             if self._sub_rank == 0:
                 lengths[self._node_index] = scraped_length - length
-                self._head_group_comm.Allreduce([lengths, MPI.DOUBLE], [difference, MPI.DOUBLE])
+                self._head_group_comm.Allreduce([lengths, self.MPI.DOUBLE], [difference, self.MPI.DOUBLE])
                 if self._rank == 0:
                     if np.sum(difference) != 0:
                         raise ValueError(np.sum(difference), "sum of differences must be zero")
                 difference = difference.astype(int)
                 i, j, i_val, j_val = 0, 0, 0, 0
                 while not np.all((difference == 0)):
                     for i, i_val in enumerate(difference):
@@ -467,15 +488,15 @@
                 obj[key] = obj[key][self._node_index::self._number_of_nodes]
             return obj
         else:
             raise TypeError("Parallel tools cannot split {} within node.".format(obj))
 
     def check_lammps(self, lammps_noexceptions=0):
         cmds = ["-screen", "none", "-log", "none"]
-        if stubs == 0:
+        if self.stubs == 0:
             self._lmp = lammps(comm=self._micro_comm, cmdargs=cmds)
         else:
             self._lmp = lammps(cmdargs=cmds)
 
         if not (self._lmp.has_exceptions or lammps_noexceptions):
             raise Exception("Fitting interrupted! LAMMPS not compiled with C++ exceptions handling enabled")
         self._lmp.close()
@@ -490,15 +511,15 @@
                 pass
                 
     def initialize_lammps(self, lammpslog=0, printlammps=0):
         cmds = ["-screen", "none"]
         if not lammpslog:
             cmds.append("-log")
             cmds.append("none")
-        if stubs == 0:
+        if self.stubs == 0:
             self._lmp = lammps(comm=self._micro_comm, cmdargs=cmds)
             self.initialize_mliap()
         else:
             self._lmp = lammps(cmdargs=cmds)
             self.initialize_mliap()
 
         if printlammps == 1:
@@ -518,18 +539,18 @@
 
         Args:
             nconfigs: integer number of configurations on this process, typically length of list of 
                       data dictionaries.
 
         Returns number of configs per node, reduced across procs, or just nconfigs if stubs.
         """
-        if not stubs:
+        if not self.stubs:
             ncpp = np.array([nconfigs]) # Num. configs per proc.
             ncpn = np.array([0]) # Num. configs per node.
-            self._comm.Allreduce([ncpp, MPI.INT], [ncpn, MPI.INT])
+            self._comm.Allreduce([ncpp, self.MPI.INT], [ncpn, self.MPI.INT])
             return ncpn[0]
         return nconfigs
 
     def slice_array(self, name):
         if name in self.shared_arrays:
             if name != 'a':
                 s = slice(self._sub_rank, None, self._sub_size)
@@ -760,20 +781,21 @@
             indices[i] = count, count+value-1
             count += value
         # sub indices
         self.add_2_fitsnap("sub_neighlist_indices", indices)
         self._bcast_fitsnap("sub_neighlist_indices")
         self.fitsnap_dict["sub_neighlist_indices"] = indices[self._sub_rank]
 
-    @stub_check
+    #@stub_check
     def combine_coeffs(self, coeff):
         new_coeff = None
-        if self._sub_rank == 0:
-            new_coeff = self._head_group_comm.allreduce(coeff) / self._number_of_nodes
-        return self._sub_comm.bcast(new_coeff)
+        if self.stubs == 0:
+            if self._sub_rank == 0:
+                new_coeff = self._head_group_comm.allreduce(coeff) / self._number_of_nodes
+            return self._sub_comm.bcast(new_coeff)
 
     @staticmethod
     def get_ram():
         mem = virtual_memory()
         return mem.total
 
     def set_logger(self, logger):
@@ -876,15 +898,17 @@
     def get_list(self):
         """ Returns deepcopy of internal list """
         return deepcopy(self._list)
 
 
 class SharedArray:
 
-    def __init__(self, size1, size2=1, dtype='d', multinode=0, comms=None):
+    def __init__(self, size1, size2=1, dtype='d', multinode=0, comms=None, MPI=None):
+        
+        self.MPI = MPI
 
         # total array for all procs
         self.array = None
         # sub array for this proc
         self.sliced_array = None
 
         self.energies_index = None
@@ -902,33 +926,33 @@
         # comm, rank, size
         self._comms = comms
 
         if multinode:
             self.multinode_lengths()
 
         if dtype == 'd':
-            item_size = MPI.DOUBLE.Get_size()
+            item_size = self.MPI.DOUBLE.Get_size()
         elif dtype == 'i':
-            item_size = MPI.INT.Get_size()
+            item_size = self.MPI.INT.Get_size()
         else:
             raise TypeError("dtype {} has not been implemented yet".format(dtype))
         if self._comms[1][1] == 0:
             self._nbytes = self._length * self._width * item_size
         else:
             self._nbytes = 0
 
         #win = MPI.Win.Allocate_shared(self._nbytes, item_size, Intracomm_comm=self._comms[1][0])
-        self.win = MPI.Win.Allocate_shared(self._nbytes, item_size, comm=self._comms[1][0])
+        self.win = self.MPI.Win.Allocate_shared(self._nbytes, item_size, comm=self._comms[1][0])
 
         buff, item_size = self.win.Shared_query(0)
 
         if dtype == 'd':
-            assert item_size == MPI.DOUBLE.Get_size()
+            assert item_size == self.MPI.DOUBLE.Get_size()
         elif dtype == 'i':
-            assert item_size == MPI.INT32_T.Get_size()
+            assert item_size == self.MPI.INT32_T.Get_size()
         if self._width == 1:
             self.array = np.ndarray(buffer=buff, dtype=dtype, shape=(self._length, ))
         else:
             self.array = np.ndarray(buffer=buff, dtype=dtype, shape=(self._length, self._width))
 
     def get_memory(self):
         return self._nbytes
@@ -982,13 +1006,14 @@
             self.array = np.ndarray(shape=(size1, ), dtype=dtype)
         else:
             self.array = np.ndarray(shape=(size1, size2), dtype=dtype)
 
     def get_memory(self):
         return self.array.nbytes
 
-
+"""
 if __name__.split(".")[-1] == "parallel_tools":
     if stubs == 0:
         double_size = MPI.DOUBLE.Get_size()
     else:
         double_size = ctypes.sizeof(ctypes.c_double)
+"""
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/ase_funcs.py` & `fitsnap3-3.1.0.4/fitsnap3lib/scrapers/ase_funcs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/json_scraper.py` & `fitsnap3-3.1.0.4/fitsnap3lib/scrapers/json_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/scrape.py` & `fitsnap3-3.1.0.4/fitsnap3lib/scrapers/scrape.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/scraper_factory.py` & `fitsnap3-3.1.0.4/fitsnap3lib/scrapers/scraper_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/vasp_scraper.py` & `fitsnap3-3.1.0.4/fitsnap3lib/scrapers/vasp_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/scrapers/xyz_scraper.py` & `fitsnap3-3.1.0.4/fitsnap3lib/scrapers/xyz_scraper.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/anl.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/anl.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,31 @@
 
 class ANL(Solver):
 
     def __init__(self, name, pt, config):
         super().__init__(name ,pt, config)
 
     #@pt.sub_rank_zero
-    def perform_fit(self):
+    def perform_fit(self, a=None, b=None, w=None, trainall=False):
         @self.pt.sub_rank_zero
-        def decorated_perform_fit():
+        def decorated_perform_fit(a=None, b=None, w=None):
             pt = self.pt   
             config = self.config
-            training = [not elem for elem in pt.fitsnap_dict['Testing']]
-            w = pt.shared_arrays['w'].array[training]
-            aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[training], w * pt.shared_arrays['b'].array[training]
+
+            if not trainall:
+                training = [not elem for elem in pt.fitsnap_dict['Testing']]
+            else:
+                training = [True]*np.shape(a)[0]
+
+            if a is None and b is None and w is None:
+                w = pt.shared_arrays['w'].array[training]
+                aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[training], w * pt.shared_arrays['b'].array[training]
+            else:
+                aw, bw = w[:, np.newaxis] * a[training], w * b[training]
+
     #       TODO: See if the transpose trick works or is nonsense when feeding into the UQ algos (probably nonsense)
             if config.sections['EXTRAS'].apply_transpose:
                 if np.linalg.cond(aw)**2 < 1 / fi.epsilon:
                     bw = aw[:, :].T @ bw
                     aw = aw[:, :].T @ aw
                 else:
                     print("The Matrix is ill-conditioned for the transpose trick")
@@ -52,15 +61,15 @@
             np.save('mean.npy', self.fit)
 
             nsam = config.sections["SOLVER"].nsam
             if nsam:
                 self.fit_sam = np.random.multivariate_normal(self.fit, self.cov, size=(nsam,))
             # self.fit_sam = self.fit + np.sqrt(np.diag(self.cov))*np.random.randn(nsam,nbas)
 
-        decorated_perform_fit()
+        decorated_perform_fit(a,b,w)
 
 
     @staticmethod
     def _dump_a(self):
         pt = self.pt
         np.savez_compressed('a.npz', a=pt.shared_arrays['a'].array)
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/ard.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/ard.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/bcs.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/bcs.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/jax.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/jax.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/lasso.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/lasso.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/lreg.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/lreg.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/mcmc.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/mcmc.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/merr.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/merr.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/network.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/network.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/opt.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/opt.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/pytorch.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 
 import sys
 from fitsnap3lib.solvers.solver import Solver
 from time import time
 import numpy as np
 import psutil
+import sys
+from copy import deepcopy
 
 try:
     from fitsnap3lib.lib.neural_networks.pytorch import FitTorch, create_torch_network
     from fitsnap3lib.lib.neural_networks.pas import FitTorchPAS
     from fitsnap3lib.tools.dataloaders import InRAMDatasetPyTorch, torch_collate, DataLoader
     from fitsnap3lib.tools.configuration import Configuration
     import torch
@@ -282,14 +284,15 @@
                 target_force_plot_val = []
                 model_force_plot_val = []
                 target_energy_plot_val = []
                 model_energy_plot_val = []
                 target_pas_plot_val = []
                 model_pas_plot_val = []
                 natoms_per_config = [] # stores natoms per config for calculating eV/atom errors later.
+                min_val_loss = sys.float_info.max # Store min validation loss
                 if (self.config.args.verbose or verbose):
                     self.pt.single_print(f"{'Epoch': <2} {'Train': ^10} {'Val': ^10} {'Time (s)': >2}")
                 for epoch in range(self.config.sections["PYTORCH"].num_epochs):
                     start = time()
 
                     # loop over training data
 
@@ -493,23 +496,31 @@
                             #loss = torch.sqrt(self.loss_function(pas, targets))
                             loss = self.loss_function(pas, targets)
                         
                         val_losses_step.append(loss.item())
 
                     # average training and validation losses across all batches
 
-                    progress_str = f"{epoch: <2} {np.mean(np.asarray(train_losses_step)): ^10.3e} {np.mean(np.asarray(val_losses_step)): ^10.3e} {time()-start: >2.3e}"
+                    mean_val_loss = np.mean(np.asarray(val_losses_step))
+                    mean_train_loss = np.mean(np.asarray(train_losses_step))
+                    progress_str = f"{epoch: <2} {mean_train_loss: ^10.3e} {mean_val_loss: ^10.3e} {time()-start: >2.3e}"
                     #self.pt.single_print(progress_str)
                     if (self.config.args.verbose or verbose):
                         self.pt.single_print(progress_str)
                     if outfile is not None:
                         fh.write(progress_str + "\n")
-                    train_losses_epochs.append(np.mean(np.asarray(train_losses_step)))
-                    val_losses_epochs.append(np.mean(np.asarray(val_losses_step)))
-                    if epoch % self.config.sections['PYTORCH'].save_freq == 0:
+                    train_losses_epochs.append(mean_train_loss)
+                    val_losses_epochs.append(mean_val_loss)
+                    # TODO: Use conditional here to save minimum validation loss.
+                    #       Base this on 
+                    #if epoch % self.config.sections['PYTORCH'].save_freq == 0:
+                    if mean_val_loss < min_val_loss:
+                        print(">>> New best model! Saving.")
+                        min_val_loss = mean_val_loss
+                        self.model_best = deepcopy(self.model)
                         torch.save({
                             'epoch': epoch,
                             'model_state_dict': self.model.state_dict(),
                             'optimizer_state_dict': self.optimizer.state_dict(),
                             'loss': loss},
                             self.config.sections['PYTORCH'].save_state_output
                         )
@@ -619,14 +630,18 @@
             Returns:
                 A tuple (energy, force) for the config given by `config_idx`. The tuple will contain 
                 lists of energy/force for each config if `config_idx` is None.
             """
 
             @self.pt.sub_rank_zero
             def decorated_evaluate_configs():
+                
+                if hasattr(self, "model_best"):
+                    self.model = self.model_best
+
                 #self.create_datasets()
                 # Convert model to dtype
                 self.model.to(dtype)
                 # Send model to device
                 self.model.to(eval_device)
 
                 if (standardize_bool):
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/ridge.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/ridge.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 #pt = ParallelTools()
 
 class RIDGE(Solver):
 
     def __init__(self, name, pt, config):
         super().__init__(name, pt, config)
 
-    def perform_fit(self):
+    def perform_fit(self, a=None, b=None, w=None, trainall=False):
         @self.pt.sub_rank_zero
-        def decorated_perform_fit():
+        def decorated_perform_fit(a=None, b=None, w=None):
 
             training = [not elem for elem in self.pt.fitsnap_dict['Testing']]
             w = self.pt.shared_arrays['w'].array[training]
             aw, bw = w[:, np.newaxis] * self.pt.shared_arrays['a'].array[training], w * self.pt.shared_arrays['b'].array[training]
             if 'EXTRAS' in self.config.sections and self.config.sections['EXTRAS'].apply_transpose:
                 bw = aw.T @ bw
                 aw = aw.T @ aw
@@ -33,15 +33,15 @@
             elif self.config.sections['RIDGE'].local_solver:
                 reg = Local_Ridge(alpha = alval, fit_intercept = False)
 
             reg.fit(aw, bw)
             self.pt.single_print('printing fit: ', reg.coef_)
             self.fit = reg.coef_
             residues = np.matmul(aw,reg.coef_) - bw
-        decorated_perform_fit()
+        decorated_perform_fit(a,b,w)
 
 
     #@staticmethod
     def _dump_a():
         np.savez_compressed('a.npz', a= self.pt.shared_arrays['a'].array)
 
     def _dump_x(self):
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/scalapack.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/scalapack.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/solver.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/solver.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/solver_factory.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/solver_factory.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/svd.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/svd.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,29 +14,39 @@
 
     def __init__(self, name, pt, config):
         super().__init__(name, pt, config)
         #self.config = Config()
         #self.pt = ParallelTools()
 
     #@pt.sub_rank_zero
-    def perform_fit(self):
+    def perform_fit(self, a=None, b=None, w=None, trainall=False):
         @self.pt.sub_rank_zero
-        def decorated_perform_fit():
-            training = [not elem for elem in self.pt.fitsnap_dict['Testing']]
-            w = self.pt.shared_arrays['w'].array[training]
-            aw, bw = w[:, np.newaxis] * self.pt.shared_arrays['a'].array[training], w * self.pt.shared_arrays['b'].array[training]
+        def decorated_perform_fit(a=None, b=None, w=None):
+            pt = self.pt   
+            config = self.config
+
+            if not trainall:
+                training = [not elem for elem in pt.fitsnap_dict['Testing']]
+            else:
+                training = [True]*np.shape(a)[0]
+
+            if a is None and b is None and w is None:
+                w = pt.shared_arrays['w'].array[training]
+                aw, bw = w[:, np.newaxis] * pt.shared_arrays['a'].array[training], w * pt.shared_arrays['b'].array[training]
+            else:
+                aw, bw = w[:, np.newaxis] * a[training], w * b[training]
     #       Look into gradient based linear solvers as well.
             if 'EXTRAS' in self.config.sections and self.config.sections['EXTRAS'].apply_transpose:
                 if np.linalg.cond(aw)**2 < 1 / fi.epsilon:
                     bw = aw[:, :].T @ bw
                     aw = aw[:, :].T @ aw
                 else:
                     print("The Matrix is ill-conditioned for the transpose trick")
             self.fit, residues, rank, s = lstsq(aw, bw, 1.0e-13)
-        decorated_perform_fit()
+        decorated_perform_fit(a,b,w)
 
     def _dump_a(self):
         np.savez_compressed('a.npz', a=self.pt.shared_arrays['a'].array)
 
     def _dump_x(self):
         np.savez_compressed('x.npz', x=self.fit)
```

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/solvers/tensorflowsvd.py` & `fitsnap3-3.1.0.4/fitsnap3lib/solvers/tensorflowsvd.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/tools/configuration.py` & `fitsnap3-3.1.0.4/fitsnap3lib/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/tools/dataframe_tools.py` & `fitsnap3-3.1.0.4/fitsnap3lib/tools/dataframe_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/tools/dataloaders.py` & `fitsnap3-3.1.0.4/fitsnap3lib/tools/dataloaders.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/tools/group_tools.py` & `fitsnap3-3.1.0.4/fitsnap3lib/tools/group_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/tools/lammps_tools.py` & `fitsnap3-3.1.0.4/fitsnap3lib/tools/lammps_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/tools/nn_tools.py` & `fitsnap3-3.1.0.4/fitsnap3lib/tools/nn_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/tools/test_tools.py` & `fitsnap3-3.1.0.4/fitsnap3lib/tools/test_tools.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/units/conversion_finder.py` & `fitsnap3-3.1.0.4/fitsnap3lib/units/conversion_finder.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/fitsnap3lib/units/units.py` & `fitsnap3-3.1.0.4/fitsnap3lib/units/units.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/pyproject.toml` & `fitsnap3-3.1.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
 ]
 build-backend = 'setuptools.build_meta' 
 
 [project]
 name = "fitsnap3"
-version = "3.1.0.2"
+version = "3.1.0.4"
 description = "Molecular Machine Learning Interface"
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.9.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `fitsnap3-3.1.0.2/tests/test_examples.py` & `fitsnap3-3.1.0.4/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `fitsnap3-3.1.0.2/tests/test_pytorch.py` & `fitsnap3-3.1.0.4/tests/test_pytorch.py`

 * *Files identical despite different names*

