# Comparing `tmp/sigmaepsilon-0.0.34.tar.gz` & `tmp/sigmaepsilon-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaepsilon-0.0.34.tar", last modified: Sun Apr 16 09:03:47 2023, max compression
+gzip compressed data, was "sigmaepsilon-0.0.36.tar", last modified: Sun Jun  4 10:32:58 2023, max compression
```

## Comparing `sigmaepsilon-0.0.34.tar` & `sigmaepsilon-0.0.36.tar`

### file list

```diff
@@ -1,141 +1,146 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.678902 sigmaepsilon-0.0.34/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36022 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-04-16 09:03:47.678902 sigmaepsilon-0.0.34/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3777 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-04-16 09:03:47.678902 sigmaepsilon-0.0.34/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2229 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.658903 sigmaepsilon-0.0.34/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.662902 sigmaepsilon-0.0.34/src/sigmaepsilon/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      345 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      288 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.662902 sigmaepsilon-0.0.34/src/sigmaepsilon/core/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/core/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/core/material.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.662902 sigmaepsilon-0.0.34/src/sigmaepsilon/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/examples/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/examples/downloads.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3046 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/examples/examples.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.666903 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.666903 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/Q5V.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11142 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/andes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14798 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/bernoulli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/bernoulli2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/bernoulli3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11203 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/celldata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/cst.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    46938 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/elem.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.670903 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/gen/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/gen/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7675 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/gen/b2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9905 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/gen/b3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/h27.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/h8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/lst.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6554 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/q4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1134 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/q9.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/tet10.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/tet4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/wedge.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/dofmap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12459 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/ebc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11699 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/femsolver.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/linemesh.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.670903 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5804 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/beam.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2360 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/membrane.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2844 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/mindlinplate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3138 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/mindlinshell.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/solid.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3687 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/solid3d.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2372 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/surface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24692 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/mesh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/metamesh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7644 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/pointdata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19982 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/structure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fem/surfacemesh.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.670903 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3551 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/beam.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16520 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/loads.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3264 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/plate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15433 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11996 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/preproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/problem.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2355 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/proc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.670903 sigmaepsilon-0.0.34/src/sigmaepsilon/material/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       93 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.670903 sigmaepsilon-0.0.34/src/sigmaepsilon/material/beam/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/beam/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.670903 sigmaepsilon-0.0.34/src/sigmaepsilon/material/beam/bernoulli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       23 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/beam/bernoulli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7415 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/beam/bernoulli/section.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.674903 sigmaepsilon-0.0.34/src/sigmaepsilon/material/homg/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/homg/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3528 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/homg/ebc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5160 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/homg/rve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6183 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/homg/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.674903 sigmaepsilon-0.0.34/src/sigmaepsilon/material/hooke/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/hooke/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2723 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/hooke/sym.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1504 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/hooke/tensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14079 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/hooke/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.674903 sigmaepsilon-0.0.34/src/sigmaepsilon/material/surface/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/surface/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4212 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/surface/membrane.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5730 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/surface/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10528 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/material/surface/mindlin.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.674903 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.674903 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/joint/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/joint/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18323 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/joint/cubejoint.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.674903 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/oc/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/oc/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/oc/filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8481 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/oc/oc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/oc/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.674903 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.674903 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.678902 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9073 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/cells/bernoulli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10935 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/cells/cells.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7332 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/dyn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1966 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/ebc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6038 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/eigsolve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16553 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/fem.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7213 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/imap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8165 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/linsolve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6541 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17705 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/preproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4588 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/tr.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.678902 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2316 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/bernoulli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2123 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/hmh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/material.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8490 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/mindlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10269 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4180 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/surface.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.662902 sigmaepsilon-0.0.34/src/sigmaepsilon.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-04-16 09:03:47.000000 sigmaepsilon-0.0.34/src/sigmaepsilon.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4156 2023-04-16 09:03:47.000000 sigmaepsilon-0.0.34/src/sigmaepsilon.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-16 09:03:47.000000 sigmaepsilon-0.0.34/src/sigmaepsilon.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-16 09:03:47.000000 sigmaepsilon-0.0.34/src/sigmaepsilon.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-04-16 09:03:47.000000 sigmaepsilon-0.0.34/src/sigmaepsilon.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-04-16 09:03:47.000000 sigmaepsilon-0.0.34/src/sigmaepsilon.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/test-requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-16 09:03:47.678902 sigmaepsilon-0.0.34/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33548 2023-04-16 09:03:42.000000 sigmaepsilon-0.0.34/tests/test_bernoulli.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.762704 sigmaepsilon-0.0.36/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36022 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-06-04 10:32:58.762704 sigmaepsilon-0.0.36/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3777 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-06-04 10:32:58.762704 sigmaepsilon-0.0.36/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2229 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.742704 sigmaepsilon-0.0.36/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.742704 sigmaepsilon-0.0.36/src/sigmaepsilon/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      527 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      288 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.746704 sigmaepsilon-0.0.36/src/sigmaepsilon/core/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/core/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      288 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/core/material.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.746704 sigmaepsilon-0.0.36/src/sigmaepsilon/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/examples/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      762 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/examples/downloads.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3046 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/examples/examples.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.746704 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      517 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.750704 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8557 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/Q5V.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11142 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/andes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14820 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/bernoulli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      898 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/bernoulli2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      807 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/bernoulli3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11203 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/celldata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1475 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/cst.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47894 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/elem.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.750704 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/gen/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/gen/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7675 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/gen/b2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9905 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/gen/b3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/h27.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/h8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1720 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/lst.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6550 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/q4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1134 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/q9.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/tet10.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/tet4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      308 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/wedge.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1543 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/dofmap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12374 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/ebc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11699 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/femsolver.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.750704 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/homg/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/homg/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3443 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/homg/ebc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5239 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/homg/rve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4295 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/homg/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3992 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/linemesh.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.754704 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      315 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5804 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/beam.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2360 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/membrane.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2844 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/mindlinplate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3138 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/mindlinshell.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2418 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/solid.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4557 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/solid3d.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2372 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/surface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24684 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/mesh.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/metamesh.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7644 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/pointdata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19982 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/structure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fem/surfacemesh.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.754704 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3551 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/beam.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16520 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/loads.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3264 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/plate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15433 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11996 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/preproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      245 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/problem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2355 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/proc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2251 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.754704 sigmaepsilon-0.0.36/src/sigmaepsilon/material/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.754704 sigmaepsilon-0.0.36/src/sigmaepsilon/material/beam/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       62 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/beam/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.754704 sigmaepsilon-0.0.36/src/sigmaepsilon/material/beam/bernoulli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/beam/bernoulli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7415 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/beam/bernoulli/section.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.754704 sigmaepsilon-0.0.36/src/sigmaepsilon/material/hooke/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/hooke/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3202 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/hooke/elasticitytensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1623 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/straintensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      414 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/stresstensor.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.758704 sigmaepsilon-0.0.36/src/sigmaepsilon/material/surface/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/surface/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4237 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/surface/membrane.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5966 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/surface/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10088 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/surface/mindlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3302 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/material/tensor2x3.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.758704 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.758704 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/joint/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/joint/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18323 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/joint/cubejoint.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.758704 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/oc/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       42 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/oc/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1020 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/oc/filter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8481 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/oc/oc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2738 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/oc/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.758704 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.758704 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.758704 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9073 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/cells/bernoulli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10935 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/cells/cells.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7332 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/dyn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1934 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/ebc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6038 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/eigsolve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16553 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/fem.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7213 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/imap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8165 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/linsolve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6541 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17705 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/preproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4884 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/tr.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.762704 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2316 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/bernoulli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2123 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/hmh.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14224 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/hooke.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2082 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/imap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1655 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/material.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9558 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/mindlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10269 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4180 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/surface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4406 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/symbolic.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      510 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/tr.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.746704 sigmaepsilon-0.0.36/src/sigmaepsilon.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4735 2023-06-04 10:32:58.000000 sigmaepsilon-0.0.36/src/sigmaepsilon.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4352 2023-06-04 10:32:58.000000 sigmaepsilon-0.0.36/src/sigmaepsilon.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-04 10:32:58.000000 sigmaepsilon-0.0.36/src/sigmaepsilon.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-04 10:32:58.000000 sigmaepsilon-0.0.36/src/sigmaepsilon.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-06-04 10:32:58.000000 sigmaepsilon-0.0.36/src/sigmaepsilon.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-06-04 10:32:58.000000 sigmaepsilon-0.0.36/src/sigmaepsilon.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/test-requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-04 10:32:58.762704 sigmaepsilon-0.0.36/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33548 2023-06-04 10:32:52.000000 sigmaepsilon-0.0.36/tests/test_bernoulli.py
```

### Comparing `sigmaepsilon-0.0.34/LICENSE` & `sigmaepsilon-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/PKG-INFO` & `sigmaepsilon-0.0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon
-Version: 0.0.34
+Version: 0.0.36
 Summary: High-Performance Computational Mechanics in Python.
 Home-page: https://github.com/dewloosh/sigmaepsilon
-Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.34.zip
+Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.36.zip
 Author: Bence Balogh
 Author-email: benceeok@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sigmaepsilon-0.0.34/README.md` & `sigmaepsilon-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/setup.py` & `sigmaepsilon-0.0.36/setup.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/examples/downloads.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/examples/examples.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/examples/examples.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/Q5V.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/Q5V.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/__init__.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/__init__.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/andes.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/andes.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/bernoulli.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/bernoulli.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,17 @@
         forces = np.zeros((nE, nRHS, nP, 6), dtype=float)
         inds = np.array([0, 3, 4, 5], dtype=int)
         calculate_internal_forces_bulk(strains, D, forces, inds)
         # forces -> (nE, nRHS, nNE, nSTRE)
         forces = np.moveaxis(forces, 1, -1)
         # forces -> (nE, nNE, nSTRE, nRHS)
 
-        *_, dshpf = self.Geometry.generate_class_functions(update=False, return_symbolic=False)
+        *_, dshpf = self.Geometry.generate_class_functions(
+            update=False, return_symbolic=False
+        )
         dshp_geom = np.squeeze(dshpf([[i] for i in local_points]))
         # dshp_geom -> (nNE, nNE)
         _postproc_bernoulli_internal_forces_L_(forces, dshp_geom, jac)
         # forces -> (nE, nNE, nSTRE, nRHS)
 
         if isinstance(points, Iterable):
             approx = interpolate.interp1d(
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/bernoulli2.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/bernoulli2.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/bernoulli3.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/bernoulli3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/celldata.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/celldata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/cst.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/cst.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/elem.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/elem.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 from numpy import ndarray
 
 from neumann.linalg import ReferenceFrame
 from neumann import atleast1d, atleastnd, ascont
 from neumann.utils import to_range_1d
 from neumann.linalg.sparse.jaggedarray import JaggedArray
 
+from ...material import CauchyStressTensor
+from ...utils.material.tr import _tr_stresses_3d_bulk_multi
+from ...utils.material.imap import _map_6x1_to_3x3, _map_3x3_to_6x1
 from ...utils.fem.preproc import (
     fem_coeff_matrix_coo,
     assert_min_diagonals_bulk,
     assemble_load_vector,
     condensate_Kf_bulk,
     condensate_M_bulk,
 )
@@ -27,15 +30,16 @@
 )
 from ...utils.fem.tr import (
     nodal_dcm,
     nodal_dcm_bulk,
     element_dcm,
     element_dcm_bulk,
     tr_element_vectors_bulk_multi as tr_vectors,
-    tr_element_matrices_bulk as tr2d,
+    tr_element_matrices_bulk as tr_matrices,
+    _scatter_element_frames,
 )
 from ...utils.fem.fem import (
     topo_to_gnum,
     expand_coeff_matrix_bulk,
     element_dofmap_bulk,
     topo_to_gnum_jagged,
     expand_load_vector_bulk,
@@ -67,79 +71,70 @@
     Base mixin class for all element types. Functions of this class
     can be called on any class of SigmaEpsilon.
     """
 
     def direction_cosine_matrix(
         self,
         *_,
-        source: Union[ndarray, str] = None,
-        target: Union[ndarray, str] = None,
+        source: Union[ndarray, str, ReferenceFrame] = None,
+        target: Union[ndarray, str, ReferenceFrame] = None,
         N: int = None,
         **__,
     ) -> ndarray:
         """
-        Returns the DCM matrix from local to global for all elements
-        in the block.
+        Returns the DCM matrix for all elements in the block.
 
         Parameters
         ----------
-        source : str or ReferenceFrame, Optional
+        source: Union[ndarray, str, ReferenceFrame], Optional
             A source frame. Default is None.
-        target : str or ReferenceFrame, Optional
+        target: Union[ndarray, str, ReferenceFrame], Optional
             A target frame. Default is None.
-        N : int, Optional
+        N: int, Optional
             Number of points. If not specified, the number of nodes is inferred from
             the class of the instance the function is called upon. Default is None.
 
         Returns
         -------
         numpy.ndarray
             The dcm matrix for linear transformations from source to target.
         """
         nNE = self.__class__.NNODE if N is None else N
-        nDOF = self.container.root().NDOFN
+        mesh_source = self.container.source()
+        nDOF = mesh_source.NDOFN
         c, r = divmod(nDOF, 3)
         assert r == 0, (
             "The default mechanism assumes that the number of "
             + "deegrees of freedom per node is a multiple of 3."
         )
+
         ndcm = nodal_dcm_bulk(self.frames, c)
         dcm = element_dcm_bulk(ndcm, nNE, nDOF)  # (nE, nEVAB, nEVAB)
+
         if source is None and target is None:
             target = "global"
+
+        if isinstance(target, str) and target == "global":
+            target = ReferenceFrame(mesh_source.frame)
+
+        if isinstance(source, str) and source == "global":
+            source = ReferenceFrame(mesh_source.frame)
+
         if source is not None:
-            if isinstance(source, str):
-                if source == "global":
-                    S = ReferenceFrame(dim=dcm.shape[-1])
-                    return ReferenceFrame(dcm).dcm(source=S)
-            elif isinstance(source, ReferenceFrame):
+            if isinstance(source, ReferenceFrame):
                 if len(source) == 3:
-                    c, r = divmod(nDOF, 3)
-                    assert r == 0, (
-                        "The default mechanism assumes that the number of "
-                        + "deegrees of freedom per node is a multiple of 3."
-                    )
                     s_ndcm = nodal_dcm(source.dcm(), c)
                     s_dcm = element_dcm(s_ndcm, nNE, nDOF)  # (nEVAB, nEVAB)
                     source = ReferenceFrame(s_dcm)
                 return ReferenceFrame(dcm).dcm(source=source)
             else:
                 raise NotImplementedError
         elif target is not None:
-            if isinstance(target, str):
-                if target == "global":
-                    T = ReferenceFrame(dim=dcm.shape[-1])
-                    return ReferenceFrame(dcm).dcm(target=T)
-            elif isinstance(target, ReferenceFrame):
+            if isinstance(target, ReferenceFrame):
                 if len(target) == 3:
-                    c, r = divmod(nDOF, 3)
-                    assert r == 0, (
-                        "The default mechanism assumes that the number of "
-                        + "deegrees of freedom per node is a multiple of 3."
-                    )
                     t_ndcm = nodal_dcm(target.dcm(), c)
                     t_dcm = element_dcm(t_ndcm, nNE, nDOF)  # (nEVAB, nEVAB)
                     target = ReferenceFrame(t_dcm)
                 return ReferenceFrame(dcm).dcm(target=target)
             else:
                 raise NotImplementedError
         raise NotImplementedError
@@ -155,27 +150,27 @@
         **__,
     ) -> ndarray:
         """
         Returns nodal displacements for the cells, wrt. their local frames.
 
         Parameters
         ----------
-        points : float or Iterable, Optional
+        points: float or Iterable, Optional
                 Points of evaluation. If provided, it is assumed that the given values
                 are wrt. the range [0, 1], unless specified otherwise with the 'rng'
                 parameter. If not provided, results are returned for the nodes of the
                 selected elements. Default is None.
-        rng : Iterable, Optional
+        rng: Iterable, Optional
             Range where the points of evauation are understood. Only for 1d cells.
             Default is [0, 1].
-        cells : int or Iterable[int], Optional
+        cells: int or Iterable[int], Optional
             Indices of cells. If not provided, results are returned for all cells.
             If cells are provided, the function returns a dictionary, with the cell
             indices being the keys. Default is None.
-        target : str or ReferenceFrame, Optional
+        target: str or ReferenceFrame, Optional
             Reference frame for the output. A value of None or 'local' refers to the
             local system of the cells. Default is 'local'.
 
         Returns
         -------
         numpy.ndarray
             An array of shape (nE, nEVAB, nRHS) if 'flatten' is True
@@ -258,23 +253,23 @@
         **__,
     ) -> ndarray:
         """
         Returns strains for one or more cells.
 
         Parameters
         ----------
-        points : float or Iterable[float], Optional
+        points: float or Iterable[float], Optional
                 Points of evaluation. If provided, it is assumed that the given values
                 are wrt. the range [0, 1], unless specified otherwise with the 'rng'
                 parameter. If not provided, results are returned for the nodes of the
                 selected elements. Default is None.
-        rng : Iterable, Optional
+        rng: Iterable, Optional
             Range where the points of evauation are understood. Only for 1d cells.
             Default is [0, 1].
-        cells : int or Iterable[int], Optional
+        cells: int or Iterable[int], Optional
             Indices of cells. If not provided, results are returned for all cells.
             Default is None.
 
         Returns
         -------
         numpy.ndarray
             An array of shape (nE, nP, nSTRE, nRHS).
@@ -330,22 +325,22 @@
         **__,
     ) -> ndarray:
         """
         Returns kinetic strains for one or more cells.
 
         Parameters
         ----------
-        points : float or Iterable, Optional
+        points: float or Iterable, Optional
                  Points of evaluation. If provided, it is assumed that the given values
                  are wrt. the range [0, 1], unless specified otherwise with the 'rng'
                  parameter. If not provided, results are returned for the nodes of the
                  selected elements. Default is None.
-        rng : Iterable, Optional
+        rng: Iterable, Optional
             Range where the points of evauation are understood. Default is [0, 1].
-        cells : int or Iterable[int], Optional
+        cells: int or Iterable[int], Optional
             Indices of cells. If not provided, results are returned for all cells.
             Default is None.
 
         Returns
         -------
         numpy.ndarray
             An array of shape (nE, nSTRE, nRHS), where nE is the number of cells,
@@ -395,18 +390,18 @@
     ) -> ndarray:
         """
         Evaluates :math:`\mathbf{f}_e = \mathbf{K}_e @ \mathbf{u}_e` for one
         or several cells and load cases.
 
         Parameters
         ----------
-        cells : int or Iterable[int], Optional
+        cells: int or Iterable[int], Optional
             Indices of cells. If not provided, results are returned for all cells.
             Default is None.
-        target : Union[str, ReferenceFrame], Optional
+        target: Union[str, ReferenceFrame], Optional
             The target frame. Default is 'local', which means that the returned
             forces should be understood as coordinates of generalized vectors in
             the local frames of the cells.
         flatten: bool, Optional
             Determines the shape of the resulting array. Default is True.
 
         Returns
@@ -494,14 +489,59 @@
         inds = np.arange(forces.shape[-1])
         calculate_internal_forces_bulk(strains, D, forces, inds)
         # forces -> (nE, nRHS, nP, nSTRE)
         forces = ascont(np.moveaxis(forces, 1, -1))
         # forces -> (nE, nP, nSTRE, nRHS)
         return forces
 
+    def _transform_internal_forces_(
+        self,
+        forces: ndarray,  # (nE, nP, nSTRE, nRHS)
+        target: Union[str, ReferenceFrame] = "local",
+        cells: Union[int, Iterable[int]] = None,
+    ) -> ndarray:
+        # The implementation here should apply to solidsm and dedicated mechanisms
+        # should be implemented at the corresponding base classes
+        nDIM = self.NDIM
+
+        if target is not None:
+            if isinstance(target, str) and target == "local":
+                values = forces
+            else:
+                if isinstance(target, str):
+                    assert target == "global"
+                    target = self.container.source().frame
+                else:
+                    if not isinstance(target, ReferenceFrame):
+                        raise TypeError(
+                            "'target' should be an instance of ReferenceFrame"
+                        )
+
+                if nDIM == 3:
+                    values = np.moveaxis(forces, -1, -2)
+                    nE, nP, nRHS, nSTRE = values.shape
+                    dcm = ReferenceFrame(self.frames[cells]).dcm(target=target)
+                    dcm = _scatter_element_frames(dcm, nP)
+                    values = _map_6x1_to_3x3(values)
+                    values = _tr_stresses_3d_bulk_multi(ascont(values), dcm)
+                    values = _map_3x3_to_6x1(values)
+                    values = np.moveaxis(values, -1, -2)
+                else:
+                    # FIXME Move this to the dedicated base class
+                    values = np.moveaxis(forces, -1, 1)
+                    nE, nRHS, nP, nSTRE = values.shape
+                    values = values.reshape(nE, nRHS, nP * nSTRE)
+                    dcm = self.direction_cosine_matrix(N=nP, target=target)[cells]
+                    values = tr_vectors(values, dcm)
+                    values = values.reshape(nE, nRHS, nP, nSTRE)
+                    values = np.moveaxis(values, 1, -1)
+        else:
+            values = forces
+        return values
+
     def internal_forces(
         self,
         *_,
         cells: Union[int, Iterable[int]] = None,
         rng: Iterable = None,
         points: Union[float, Iterable] = None,
         flatten: bool = True,
@@ -509,26 +549,26 @@
         **__,
     ) -> ndarray:
         """
         Returns internal forces for many cells and evaluation points.
 
         Parameters
         ----------
-        points : float or Iterable[float], Optional
+        points: float or Iterable[float], Optional
                 Points of evaluation. If provided, it is assumed that the given values
                 are wrt. the range [0, 1], unless specified otherwise with the 'rng'
                 parameter. If not provided, results are returned for the nodes of the
                 selected elements. Default is None.
-        rng : Iterable[float], Optional
+        rng: Iterable[float], Optional
             Range where the points of evauation are understood. Only for 1d cells.
             Default is [0, 1].
-        cells : int or Iterable[int], Optional
+        cells: int or Iterable[int], Optional
             Indices of cells. If not provided, results are returned for all cells.
             Default is None.
-        target : Union[str, ReferenceFrame], Optional
+        target: Union[str, ReferenceFrame], Optional
             The target frame. Default is 'local', which means that the returned forces
             should be understood as coordinates of generalized vectors in the local
             frames of the cells.
         flatten: bool, Optional
             Determines the shape of the resulting array. Default is True.
 
         Returns
@@ -557,37 +597,22 @@
             points = to_range_1d(points, source=rng, target=[-1, 1]).flatten()
             rng = [-1, 1]
         else:
             if points is None:
                 points = np.array(self.lcoords())
 
         forces = self._internal_forces_(cells=cells, points=points)
+        forces = self._transform_internal_forces_(forces, cells=cells, target=target)
         # forces -> (nE, nP, nSTRE, nRHS)
 
-        if target is not None:
-            if isinstance(target, str) and target == "local":
-                values = forces
-            else:
-                # transform values to a destination frame, or return
-                # the forces in the local frames of the cells
-                values = np.moveaxis(forces, -1, 1)
-                nE, nRHS, nP, nSTRE = values.shape
-                values = values.reshape(nE, nRHS, nP * nSTRE)
-                dcm = self.direction_cosine_matrix(N=nP, target=target)[cells]
-                values = tr_vectors(values, dcm)
-                values = values.reshape(nE, nRHS, nP, nSTRE)
-                values = np.moveaxis(values, 1, -1)
-        else:
-            values = forces
-
         if flatten:
-            nE, nP, nSTRE, nRHS = values.shape
-            values = values.reshape(nE, nP * nSTRE, nRHS)
+            nE, nP, nSTRE, nRHS = forces.shape
+            forces = forces.reshape(nE, nP * nSTRE, nRHS)
 
-        return values
+        return forces
 
     def global_dof_numbering(self, *_, **kwargs) -> Union[JaggedArray, ndarray]:
         """
         Returns global numbering of the degrees of freedom of the cells.
         """
         topo = kwargs.get("topo", None)
         topo = self.topology() if topo is None else topo
@@ -615,21 +640,21 @@
         **kwargs,
     ) -> Union[ndarray, coo_matrix]:
         """
         Returns the elastic stiffness matrix of the cells.
 
         Parameters
         ----------
-        transform : bool, Optional
+        transform: bool, Optional
             If True, local matrices are transformed to the global frame.
             Default is True.
-        minval : float, Optional
+        minval: float, Optional
             A minimal value for the entries in the main diagonal. Set it to a negative
             value to diable its effect. Default is 1e-12.
-        sparse : bool, Optional
+        sparse: bool, Optional
             If True, the returned object is a sparse COO matrix. Default is False.
 
         Returns
         -------
         numpy.ndarray or scipy.sparse.coo_matrix
             A sparse SciPy matrix if 'sparse' is True, or a 3d numpy array, where the
             elements run along the first axis.
@@ -730,21 +755,21 @@
         **kwargs,
     ) -> Union[ndarray, coo_matrix]:
         """
         Returns the stiffness-consistent mass matrix of the cells.
 
         Parameters
         ----------
-        transform : bool, Optional
+        transform: bool, Optional
             If True, local matrices are transformed to the global frame.
             Default is True.
-        minval : float, Optional
+        minval: float, Optional
             A minimal value for the entries in the main diagonal. Set it to a
             negative value to diable its effect. Default is 1e-12.
-        sparse : bool, Optional
+        sparse: bool, Optional
             If True, the returned object is a sparse COO matrix.
             Default is False.
 
         Returns
         -------
         numpy.ndarray or scipy.sparse.coo_matrix
             A sparse SciPy matrix if 'sparse' is True, or a 3d numpy array,
@@ -852,18 +877,18 @@
     ) -> ndarray:
         """
         Builds the equivalent nodal load vector from all sources
         and returns it in either the global frame or cell-local frames.
 
         Parameters
         ----------
-        assemble : bool, Optional
+        assemble: bool, Optional
             If True, the values are returned with a matching shape to the total
             system. Default is False.
-        transform : bool, Optional
+        transform: bool, Optional
             If True, local matrices are transformed to the global frame.
             Default is True.
 
         See Also
         --------
         :func:`body_load_vector`
         :func:`strain_load_vector`
@@ -902,26 +927,26 @@
         **__,
     ) -> ndarray:
         """
         Generates a load vector from strain loads specified for all cells.
 
         Parameters
         ----------
-        values : numpy.ndarray, Optional
+        values: numpy.ndarray, Optional
             Strain loads as a 3d numpy array of shape (nE, nS, nRHS).
             The array must contain values for all cells (nE), strain
             components (nS) and load cases (nL).
-        return_zeroes : bool, Optional
+        return_zeroes: bool, Optional
             Controls what happends if there are no strain loads provided.
             If True, a zero array is retured with correct shape, otherwise None.
             Default is False.
-        transform : bool, Optional
+        transform: bool, Optional
             If True, local matrices are transformed to the global frame.
             Default is True.
-        assemble : bool, Optional
+        assemble: bool, Optional
             If True, the values are returned with a matching shape to the total
             system. Default is False.
 
         See Also
         --------
         :func:`load_vector`
         :func:`body_load_vector`
@@ -999,27 +1024,27 @@
     ) -> ndarray:
         """
         Builds the equivalent discrete representation of body loads
         and returns it in either the global frame or cell-local frames.
 
         Parameters
         ----------
-        values : numpy.ndarray, Optional
+        values: numpy.ndarray, Optional
             Body load values for all cells. Default is None.
         constant : bool, Optional
             Set this True if the input represents a constant load.
             Default is False.
-        assemble : bool, Optional
+        assemble: bool, Optional
             If True, the values are returned with a matching shape to the total
             system. Default is False.
-        return_zeroes : bool, Optional
+        return_zeroes: bool, Optional
             Controls what happends if there are no strain loads provided.
             If True, a zero array is retured with correct shape, otherwise None.
             Default is False.
-        transform : bool, Optional
+        transform: bool, Optional
             If True, local matrices are transformed to the global frame.
             Default is True.
 
         See Also
         --------
         :func:`load_vector`
         :func:`strain_load_vector`
@@ -1092,15 +1117,15 @@
 
     def integrate_body_loads(self, values: ndarray) -> ndarray:
         """
         Returns nodal representation of body loads.
 
         Parameters
         ----------
-        values : numpy.ndarray
+        values: numpy.ndarray
             2d or 3d numpy float array of material densities of shape
             (nE, nNE * nDOF, nRHS) or (nE, nNE * nDOF), where nE, nNE,
             nDOF and nRHS stand for the number of elements, nodes per
             element, number of degrees of freedom and number of load cases
             respectively.
 
         Returns
@@ -1180,37 +1205,37 @@
 
         Parameters
         ----------
         *args
             Forwarded to :func:`direction_cosine_matrix`
         **kwargs
             Forwarded to :func:`direction_cosine_matrix`
-        A : numpy.ndarray
+        A: numpy.ndarray
             The coefficient matrix in the source frame.
-        invert : bool, Optional
+        invert: bool, Optional
             If True, the DCM matrices are transposed before transformation.
             This makes this function usable in both directions.
             Default is False.
 
         Returns
         -------
         numpy.ndarray
             The coefficient matrix in the target frame.
         """
         # DCM from local to global
         dcm = self.direction_cosine_matrix(*args, **kwargs)
-        return A if dcm is None else tr2d(A, dcm, invert)
+        return A if dcm is None else tr_matrices(A, dcm, invert)
 
     def _transform_nodal_loads_(self, nodal_loads: ndarray) -> ndarray:
         """
         Transforms discrete nodal loads to the global frame.
 
         Parameters
         ----------
-        nodal_loads : numpy.ndarray
+        nodal_loads: numpy.ndarray
             A 3d array of shape (nE, nEVAB, nRHS).
 
         Returns
         -------
         numpy.ndarray
             A numpy array of shape (nE, nEVAB, nRHS).
         """
@@ -1225,15 +1250,15 @@
 
     def _assemble_nodal_loads_(self, nodal_loads: ndarray) -> ndarray:
         """
         Assembles the nodal load vector for multiple load cases.
 
         Parameters
         ----------
-        nodal_loads : numpy.ndarray
+        nodal_loads: numpy.ndarray
             A 3d array of shape (nE, nEVAB, nRHS).
 
         Returns
         -------
         numpy.ndarray
             A numpy array of shape (nX, nRHS), where nX is the total
             number of unknowns in the total structure.
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/gen/b2.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/gen/b2.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/gen/b3.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/gen/b3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/lst.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/lst.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/meta.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         raise NotImplementedError
 
     def dof_solution(self, *, cells: Iterable, flatten: bool) -> ndarray:
         raise NotImplementedError
 
     def kinetic_strains(self, *, cells: Iterable, points: Iterable) -> ndarray:
         raise NotImplementedError
-    
+
     def centers(self, *args, **kwargs) -> ndarray:
         raise NotImplementedError
 
 
 class FemMaterial(FemMixin):
     """
     Base class for FEM material classes.
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/q4.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/q4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/cells/q9.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/cells/q9.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/dofmap.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/dofmap.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/ebc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/ebc.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,147 +11,152 @@
 from polymesh.cell import PolyCell3d
 from polymesh.utils.space import index_of_closest_point
 
 from .mesh import FemMesh
 from .dofmap import DOF
 from .constants import DEFAULT_DIRICHLET_PENALTY
 from ..utils.fem.ebc import (
-    link_points_to_points, 
+    link_points_to_points,
     link_points_to_body,
     _body_to_body_stiffness_data_,
 )
 
 
 __all__ = ["NodalSupport", "NodeToNode", "FaceToFace", "BodyToBody"]
 
 
 class EssentialBoundaryCondition:
     """
     Base class for Dirichlet boundary conditions accounted for
     using Courant-type penalization.
     """
-            
+
     @abstractmethod
     def assemble(self, mesh: FemMesh) -> Tuple[coo, ndarray]:
         ...
 
 
 class BodyToBody(EssentialBoundaryCondition):
     """
     Constrains the dofs of two touching bodies by gluing them together.
-    
+
     Parameters
     ----------
     source: PolyCell
         The source body.
     target: PolyCell
         The target body.
     dofs: Iterable, Optinal
-        An iterable of the constrained global degrees of freedom. It not specified, 
+        An iterable of the constrained global degrees of freedom. It not specified,
         all degrees of freedom are constrained.
     penalty: float, Optional
         The penalty value.
     lazy: bool, Optional
         Default is True.
     tol: float, Optional
         Floating point tolerance for detecting point in polygons. Default is 1e-12.
     k: int, Optional
         THe number of neighbours.
-        
+
     Notes
     -----
     The two bodies must have a common surface.
     """
+
     def __init__(
         self,
-        source: PolyCell3d=None,
-        target: PolyCell3d=None,
+        source: PolyCell3d = None,
+        target: PolyCell3d = None,
         dofs: Iterable = None,
         penalty: float = DEFAULT_DIRICHLET_PENALTY,
         lazy: bool = True,
         tol: float = 1e-12,
         k: int = 4,
-        touching: bool=False,
-        factors: ndarray=None,
-        indices: ndarray=None
-    ):  
+        touching: bool = False,
+        factors: ndarray = None,
+        indices: ndarray = None,
+    ):
         if source and target:
             assert source.NDIM == 3, "Source must be a 3 dimensional body!"
             assert target.NDIM == 3, "Source must be a 3 dimensional body!"
-            assert source.container.source() is target.container.source(), (
-                "The source and the target must belong to the same pointcloud!"
-            )
-            assert source.container.source() is source.container.root(), (
-                "The mesh must be brought to a standard form!"
-            )
-            assert isinstance(target.__class__.monomsfnc, Callable), (
-                "The class is not equipped with the tools for this operation."
-            )
+            assert (
+                source.container.source() is target.container.source()
+            ), "The source and the target must belong to the same pointcloud!"
+            assert (
+                source.container.source() is source.container.root()
+            ), "The mesh must be brought to a standard form!"
+            assert isinstance(
+                target.__class__.monomsfnc, Callable
+            ), "The class is not equipped with the tools for this operation."
         self.source = source
         self.target = target
         self.penalty = penalty
         self.lazy = lazy
         self.k = k
         self.tol = tol
         self.touching = touching
-        self.factors=factors
-        self.indices=indices
-        
+        self.factors = factors
+        self.indices = indices
+
         if isinstance(dofs, Iterable):
             self.dofmap = DOF.dofmap(dofs)
         else:
             self.dofmap = None
-    
-    def assemble(self, mesh: FemMesh) -> Tuple[coo, ndarray]: 
+
+    def assemble(self, mesh: FemMesh) -> Tuple[coo, ndarray]:
         if (self.factors is None) or (self.indices is None):
             S: PolyCell3d = self.source
             T: PolyCell3d = self.target
-            
-            assert S.container.root() == mesh, \
-                "The input mesh must be the root of both the source and the target."
-            assert T.container.root() == mesh, \
-                "The input mesh must be the root of both the source and the target."
-            
+
+            assert (
+                S.container.root() == mesh
+            ), "The input mesh must be the root of both the source and the target."
+            assert (
+                T.container.root() == mesh
+            ), "The input mesh must be the root of both the source and the target."
+
             if self.touching:
                 coords, topo_source_surface = S.extract_surface(detach=False)
                 source_indices = np.unique(topo_source_surface)
             else:
                 coords = S.source_coords()
                 source_indices = S.unique_indices()
-            
+
             source_coords = coords[source_indices]
             factors, indices = link_points_to_body(
                 PointCloud(source_coords, inds=source_indices),
-                T, self.lazy, self.tol, self.k
+                T,
+                self.lazy,
+                self.tol,
+                self.k,
             )
         else:
             factors, indices = self.factors, self.indices
-            
+
         nDOF = mesh.NDOFN
         nN = len(mesh.pointdata)
         N = nDOF * nN
         if self.dofmap is None:
             dmap = np.arange(nDOF)
         else:
             dmap = self.dofmap
         dmap = np.array(dmap, dtype=int)
-        
-        factors, indices = \
-            _body_to_body_stiffness_data_(factors, indices, dmap, nDOF)
+
+        factors, indices = _body_to_body_stiffness_data_(factors, indices, dmap, nDOF)
         fdata = factors.flatten()
         frows = np.repeat(np.arange(factors.shape[0]), factors.shape[1])
         fcols = indices.flatten()
         factors = coo((fdata, (frows, fcols)), shape=(factors.shape[0], N))
-                
+
         Kp = self.penalty * (factors.T @ factors)
         fp = np.zeros(N, dtype=float)
         Kp.eliminate_zeros()
         return Kp, fp
-            
-    
+
+
 class NodeToNode(EssentialBoundaryCondition):
     """
     Constrains relative motion of nodes.
 
     Parameters
     ----------
     imap : Union[dict, ndarray, list]
@@ -161,15 +166,15 @@
         Default is `~sigmaepsilon.fem.constants.DEFAULT_DIRICHLET_PENALTY`.
     dofs: Iterable, Optinal
         An iterable of the constrained degrees of freedom. It not specified, all
         degrees of freedom are constrained.
     source: PointCloud, Optional
         The source pointcloud. Only if 'imap' is not provided.
     target: PointCloud, Optional
-        The target pointcloud. Only if 'imap' is not provided. 
+        The target pointcloud. Only if 'imap' is not provided.
 
     Example
     -------
     The following lines tie together all DOFs of nodes 1 with node 2 and node 3 with 4.
     The large penalty value means that the tied nodes should have the same displacements.
 
     >>> from sigmaepsilon.fem import NodeToNode
@@ -205,33 +210,33 @@
         """
         imap = None
         if isinstance(self.imap, dict):
             imap = np.stack([list(self.imap.keys()), list(self.imap.values())], axis=1)
         else:
             imap = np.array(self.imap).astype(int)
         nI = len(imap)
-        
+
         nDOF = mesh.NDOFN
         nN = len(mesh.pointdata)
         N = nDOF * nN
-        
+
         if self.dofmap is None:
             dmap = np.arange(nDOF)
         else:
             dmap = self.dofmap
         dmap = np.array(dmap, dtype=int)
-        
+
         nF = nI * len(dmap)
         fdata = np.tile([1, -1], nF)
         frows = np.repeat(np.arange(nF), 2)
         i_source = conc([dmap + (i_ * nDOF) for i_ in imap[:, 0]])
         i_target = conc([dmap + (i_ * nDOF) for i_ in imap[:, 1]])
         fcols = np.stack([i_source, i_target], axis=1).flatten()
         factors = coo((fdata, (frows, fcols)), shape=(nF, N))
-        
+
         Kp = self.penalty * (factors.T @ factors)
         fp = np.zeros(N, dtype=float)
         Kp.eliminate_zeros()
         return Kp, fp
 
 
 class NodalSupport(EssentialBoundaryCondition):
@@ -332,17 +337,17 @@
         else:
             i = atleast1d(self.i)
         nI = len(i)
         nDOF = mesh.NDOFN
         nN = len(mesh.pointdata)
         N = nDOF * nN
         c, r = divmod(nDOF, 3)
-        assert r == 0, (
-            "The number of deegrees of freedom per node must be a multiple of 3."
-        )
+        assert (
+            r == 0
+        ), "The number of deegrees of freedom per node must be a multiple of 3."
         dcm = self.frame.dcm(source=mesh.frame)
         nodal_dcm = repeat_diagonal_2d(dcm, c)[self.dofmap]
         factors = repeat_diagonal_2d(nodal_dcm, nI)
         dofs = np.arange(nDOF)
         inds = conc([dofs + (i_ * nDOF) for i_ in i])
         kdata = (factors.T @ factors).flatten()
         krows = np.repeat(inds, len(inds))
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/femsolver.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/femsolver.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/linemesh.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/linemesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/beam.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/beam.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/membrane.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/membrane.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/mindlinplate.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/mindlinplate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/mindlinshell.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/mindlinshell.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/solid.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/solid.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/material/surface.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/material/surface.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/mesh.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         self, *args, cell_fields: dict = None, point_fields: dict = None, **kwargs
     ):
         point_fields = {} if point_fields is None else point_fields
         cell_fields = {} if cell_fields is None else cell_fields
         super().__init__(
             *args, point_fields=point_fields, cell_fields=cell_fields, **kwargs
         )
-        
+
     def __getitem__(self, key) -> "FemMesh":
         return super().__getitem__(key)
 
     @property
     def pd(self) -> PointData:
         """
         Returns the attached pointdata.
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/metamesh.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/metamesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/pointdata.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/pointdata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/structure.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/structure.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fem/surfacemesh.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/surfacemesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/beam.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/beam.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/loads.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/loads.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/plate.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/plate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/postproc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/postproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/preproc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/preproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/proc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/proc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/fourier/utils.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fourier/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/material/beam/bernoulli/section.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/material/beam/bernoulli/section.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/material/homg/ebc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/homg/ebc.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,69 +35,68 @@
         i = index_of_closest_point(source, target)
         id_source = points[i_source].id[i]
         id_target = points[i_target].id
         links.append(np.stack([id_source, id_target], axis=1))
     return NodeToNode(np.vstack(links))
 
 
-def _link_opposite_sides(
-    mesh: FemMesh, axis: Union[int, Iterable[int]] = 0
-) -> ndarray:
+def _link_opposite_sides(mesh: FemMesh, axis: Union[int, Iterable[int]] = 0) -> ndarray:
     if isinstance(axis, int):
         axis = [axis]
     assert isinstance(
         axis, Iterable
     ), "'axis' must be an integer or an 1d iterable of integers."
-        
+
     surface = mesh.surface()
     points = surface.points()
     triangles = surface.topology()
     centers = surface.centers()
     coords = points.show()
     bounds = points.bounds()
-    
+
     def _link_points_to_cells_(source_indices, target_indices):
         source_coords = coords[source_indices]
         target_triangles = triangles[target_indices]
-        
-        i_source, i_target, locations_target = \
-            locate_tri_2d(source_coords[:, mask], coords[:, mask], target_triangles)
-        source_indices = source_indices[i_source]   
+
+        i_source, i_target, locations_target = locate_tri_2d(
+            source_coords[:, mask], coords[:, mask], target_triangles
+        )
+        source_indices = source_indices[i_source]
         target_triangles = target_triangles[i_target]
-        
+
         shp_target = Triangle.shape_function_values(locations_target)
-        
+
         nE, nNE = target_triangles.shape
         factors = np.zeros((nE, nNE + 1), dtype=float)
         indices = np.zeros((nE, nNE + 1), dtype=int)
         factors[:, -1] = -1
         factors[:, :nNE] = shp_target
         indices[:, -1] = source_indices
         indices[:, :nNE] = target_triangles
-        
+
         return factors, indices
-    
+
     factors, indices = [], []
-    
+
     for axid in axis:
         bmin, bmax = bounds[axid]
-        
+
         mask = np.ones(3, dtype=bool)
         mask[axid] = False
-        
+
         mask_source = coords[:, axid] < (bmin + 1e-12)
         source_indices = np.where(mask_source)[0]
         mask_target = centers[:, axid] > (bmax - 1e-12)
         target_indices = np.where(mask_target)[0]
         f, i = _link_points_to_cells_(source_indices, target_indices)
         factors.append(f)
         indices.append(i)
-        
+
         mask_source = coords[:, axid] > (bmax - 1e-12)
         source_indices = np.where(mask_source)[0]
         mask_target = centers[:, axid] < (bmin + 1e-12)
         target_indices = np.where(mask_target)[0]
         f, i = _link_points_to_cells_(source_indices, target_indices)
         factors.append(f)
         indices.append(i)
-        
+
     return BodyToBody(factors=np.vstack(factors), indices=np.vstack(indices))
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/material/homg/rve.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/fem/homg/rve.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,82 +1,89 @@
 from typing import Iterable, Union
 
 import numpy as np
 from numpy import ndarray
 
+from neumann.linalg import ReferenceFrame
+
+from ..structure import Structure
+from ..ebc import NodeToNode
 from .ebc import _link_opposite_sides_sym, _link_opposite_sides
 from .utils import (
     _strain_field_3d_bulk,
     _postproc_3d_gauss_stresses,
     _calc_avg_hooke_3d_to_shell,
+    _tr_strains_to_local_frames,
 )
-from sigmaepsilon.fem import Structure
-from sigmaepsilon.fem.ebc import NodeToNode
+
+__all__ = ["RepresentativeVolumeElement"]
 
 
 class RepresentativeVolumeElement(Structure):
-    
-    def __init__(self, *args, symmetric:bool=False, **kwargs):
+    def __init__(self, *args, symmetric: bool = False, **kwargs):
         super().__init__(*args, **kwargs)
         self.symmetric = symmetric
-    
+
     def _periodic_essential_ebc(
-        self, axis: Union[int, Iterable[int]] = 0,
+        self,
+        axis: Union[int, Iterable[int]] = 0,
     ) -> NodeToNode:
         if self.symmetric:
             return _link_opposite_sides_sym(self.mesh.points(), axis)
         else:
             return _link_opposite_sides(self.mesh, axis)
-        
+
     def ABD(self) -> ndarray:
         """
         Returns the elasticity matrix for a Kirchhoff-Love plate.
-        
+
         Returns
         -------
         numpy.ndarray
             The 6x6 elastic stiffness matrix.
         """
         return self.homogenize(target="KL")
 
     def ABDS(self) -> ndarray:
         """
         Returns the elasticity matrix for a Mindlin-Reissner plate.
-        
+
         Returns
         -------
         numpy.ndarray
             The 8x8 elastic stiffness matrix.
         """
         return self.homogenize(target="MR")
 
     def homogenize(self, target: str = "MR") -> ndarray:
         """
         Returns the homogenized elasticity matrix for a Mindlin-Reissner or a
         Kirchhoff-Love plate.
-        
+
         Parameters
         ----------
         target: str, Optional
             The target model. Accepted values are 'MR' for Mindlin-Reissner
             shells and 'KL' for Kirchhoff-Love shells.
-        
+
         Returns
         -------
         numpy.ndarray
             The elastic stiffness matrix.
         """
         target = target.lower()
         if target in ["mr", "kl"]:
             return self._to_shell(target)
-    
+
     def _to_shell(self, target: str = "MR") -> ndarray:
         mesh = self.mesh
         NDOFN = mesh.NDOFN
 
+        global_frame: ReferenceFrame = mesh.frame
+
         if target.lower() == "mr":
             NSTRE = 8
         elif target.lower() == "kl":
             NSTRE = 6
 
         # mesh data
         points = mesh.points()
@@ -102,46 +109,46 @@
         # nodal supports to guarantee peridic displacement solution
         periodicity_constraints = self._periodic_essential_ebc(axis=[0, 1])
 
         # initial strain loads
         blocks = list(mesh.cellblocks(inclusive=True))
         for block in blocks:
             centers = block.cd.centers()
-            strain_loads = np.zeros((centers.shape[0], 6, NSTRE))
+            strain_loads = np.zeros((centers.shape[0], NSTRE, 6))
             _strain_field_3d_bulk(centers, out=strain_loads, NSTRE=NSTRE)
+            strain_loads[...] = _tr_strains_to_local_frames(
+                strain_loads, global_frame, block.cd.frames
+            )
             if block.cd.NDIM == 3:
-                block.cd.strain_loads = strain_loads
-            elif block.cd.NDIM == 2:
-                raise NotImplementedError
+                block.cd.strain_loads = np.moveaxis(strain_loads, -1, -2)
             else:
                 raise NotImplementedError
 
         # solve BVP
         self.constraints.append(periodicity_constraints)
         self.linear_static_analysis()
 
         # postproc
         hooke = np.zeros((NSTRE, NSTRE), dtype=float)
         hooke_avg = np.zeros_like(hooke)
         for block in blocks:
             block.cd.strain_loads = None
-            hooke_block = block.cd.elastic_material_stiffness_matrix()
+            hooke_block = block.cd.elastic_material_stiffness_matrix(target="global")
             gp, gw = block.cd.quadrature["full"]
             if block.cd.NDIM == 3:
-                cell_forces = block.cd.internal_forces(points=gp, flatten=False)
-                # cell_forces = block.internal_forces(points=gp, flatten=False, target='global')
+                cell_forces = block.cd.internal_forces(
+                    points=gp, flatten=False, target="global"
+                )
                 ec = block.cd.coords()
                 dshp = block.cd.shape_function_derivatives(gp)
                 jac = block.cd.jacobian_matrix(dshp=dshp, ecoords=ec)
                 djac = block.cd.jacobian(jac=jac)
                 ec = block.cd.coords(points=gp)
                 _postproc_3d_gauss_stresses(cell_forces, ec, gw, djac, hooke)
                 _calc_avg_hooke_3d_to_shell(hooke_block, ec, gw, djac, hooke_avg)
-            elif block.cd.NDIM == 2:
-                raise NotImplementedError
             else:
                 raise NotImplementedError
 
         self.constraints.pop(-1)
 
         hooke /= area
         hooke_avg /= area
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/material/hooke/utils.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/hooke.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from numpy import ndarray
 from scipy.optimize import minimize
 
 from dewloosh.core.tools.kwargtools import getasany
 from neumann.function import Function
 from neumann.linalg import is_pos_def
 
-from .sym import smat_sym_ortho_3d
+from .symbolic import smat_sym_ortho_3d
+
 
 __all__ = ["elastic_compliance_matrix", "elastic_stiffness_matrix"]
 
 
 poisson_ratios = ["NU12", "NU13", "NU23", "NU21", "NU32", "NU31"]
 elastic_moduli = ["E1", "E2", "E3"]
 shear_moduli = ["G12", "G13", "G23"]
@@ -21,15 +22,14 @@
 
 
 class HookeError(Exception):
     ...
 
 
 def _find_all_ortho_params(**params):
-
     # select 9 parameters (3 shear moduli and 6 from the others)
     _params = dict()
     Young, Poisson, Shear = _group_params(**params)
     _params.update(Shear)
     Young.update(Poisson)
     for i, (k, v) in enumerate(Young.items()):
         if i < 6:
@@ -122,15 +122,15 @@
         params["NU21"] = params["NU12"] * params["E2"] / params["E1"]
         params["NU31"] = params["NU13"] * params["E3"] / params["E1"]
         params["NU32"] = params["NU23"] * params["E3"] / params["E2"]
         return params
     else:
         E, NU, G = _group_params(**params)
         nE, nNU, nG = len(E), len(NU), len(G)
-        
+
         if not nG == 3:
             msg = "The three shear moduli must be provided!"
             raise HookeError(msg)
 
         if not (nE + nNU) >= 6:
             msg = (
                 "6 from the 3 Young's moduli and the 6 Poisson's"
@@ -373,25 +373,32 @@
         "G12": G12,
         "G13": G13,
         "G23": G23,
     }
     return _finalize_ortho(**params)
 
 
+def _has_elastic_params(**kwargs) -> bool:
+    try:
+        _get_elastic_params(**kwargs)
+        return True
+    except Exception:
+        return False
+
+
 def _get_elastic_params(isoplane: str = None, **params):
     E, NU, G = _group_params(**params)
     nE, nNU, nG = len(E), len(NU), len(G)
     nParams = sum([nE, nNU, nG])
 
     if nParams == 2:
         params = _get_iso_params(**E, **NU, **G)
     elif nParams == 5:
         if not isinstance(isoplane, str):
-            raise ValueError(
-                "The plane of isotropy must be specified. See the docs!")
+            raise ValueError("The plane of isotropy must be specified. See the docs!")
         if isoplane in ["23", "32"]:
             params = _get_triso_params_23(**E, **NU, **G)
         elif isoplane in ["12", "21"]:
             params = _get_triso_params_12(**E, **NU, **G)
         elif isoplane in ["13", "31"]:
             params = _get_triso_params_13(**E, **NU, **G)
     elif nParams == 9:
@@ -415,15 +422,15 @@
         Index mapping. Default is the Voigt-map.
     verify: bool, Optional
         If True, the resulting matrix is verified before getting returned. Default is False.
     isoplane: str, Optional
         If the number of specified engineering constants is 5, it suggests a transversely
         orthotropic material. In this case, the parameter 'isoplane' defines the plane of
         isotropy. Valid choices are '12', '23' and '13'. Default is None.
-        
+
     Raises
     ------
     ~sigmaepsilon.material.hooke.utils.HookeError
 
     Returns
     -------
     numpy.ndarray
@@ -431,15 +438,16 @@
     """
     params = _get_elastic_params(**params)
     sympy_matrix = smat_sym_ortho_3d(imap=imap, **params)
     S = np.array(sympy_matrix.tolist()).astype(float)
     if verify:
         if not is_pos_def(S):
             raise HookeError(
-                "The parameters does not result in a positive definite material!")
+                "The parameters does not result in a positive definite material!"
+            )
     return S
 
 
 def elastic_stiffness_matrix(*args, verify: bool = False, **kwargs) -> ndarray:
     """
     Returns the elastic stiffness matrix for a Hooke-type material model from
     a set of engineering constants.
@@ -450,23 +458,24 @@
         Index mapping. Default is the Voigt-map.
     verify: bool, Optional
         If True, the resulting matrix is verified before getting returned. Default is False.
     isoplane: str, Optional
         If the number of specified engineering constants is 5, it suggests a transversely
         orthotropic material. In this case, the parameter 'isoplane' defines the plane of
         isotropy. Valid choices are '12', '23' and '13'. Default is None.
-        
+
     Raises
     ------
     ~sigmaepsilon.material.hooke.utils.HookeError
 
     Returns
     -------
     numpy.ndarray
         A 6x6 NumPy float array.
     """
     C = np.linalg.inv(elastic_compliance_matrix(*args, **kwargs))
     if verify:
         if not is_pos_def(C):
             raise HookeError(
-                "The parameters does not result in a positive definite material!")
+                "The parameters does not result in a positive definite material!"
+            )
     return C
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/material/surface/membrane.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/material/surface/membrane.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Union
 import numpy as np
 import sympy as sy
 from numpy import ndarray
 from numpy.linalg import inv
 
-from ..hooke.utils import _get_elastic_params
-from ..hooke.sym import smat_sym_ortho_3d
+from ...utils.material.hooke import _get_elastic_params
+from ...utils.material.symbolic import smat_sym_ortho_3d
 
 from .meta import Surface, SurfaceLayer
 
 
 __all__ = ["Membrane", "MembraneLayer"]
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/material/surface/meta.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/material/surface/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,14 +117,22 @@
 class Surface(MetaSurface):
     """
     Helper base class for laminates.
     """
 
     __layerclass__ = SurfaceLayer
 
+    @property
+    def eccentricity(self):
+        return self.get("eccentricity", 0.0)
+
+    @eccentricity.setter
+    def eccentricity(self, value: float):
+        self["eccentricity"] = value
+
     @abstractclassmethod
     def Hooke(cls):
         raise NotImplementedError
 
     def Layer(self, *args, **kwargs) -> SurfaceLayer:
         """
         Returns a Layer compatible with the model.
@@ -153,22 +161,23 @@
             res += layer.elastic_stiffness_matrix()
         return res
 
     def _set_layers(self):
         """
         Sets thickness ranges for the layers.
         """
+        ecc = self.eccentricity
         layers = self.layers()
         t = sum([layer.t for layer in layers])
-        layers[0].tmin = -t / 2
+        layers[0].tmin = ecc - t / 2
         nLayers = len(layers)
         for i in range(nLayers - 1):
             layers[i].tmax = layers[i].tmin + layers[i].t
             layers[i + 1].tmin = layers[i].tmax
-        layers[-1].tmax = t / 2
+        layers[-1].tmax = ecc + t / 2
         for layer in layers:
             layer.zi = [layer.loc_to_z(l_) for l_ in layer.__loc__]
         return True
 
     @classmethod
     def from_dict(cls, d: dict = None, **kwargs) -> "Surface":
         """
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/material/surface/mindlin.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/material/surface/mindlin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
-from typing import Tuple, Union, Callable
+from typing import Tuple, Union, Callable, Iterable
+
 import numpy as np
 from numpy import ndarray
 from numpy.linalg import inv
 import sympy as sy
 
-from ..hooke.utils import _get_elastic_params
-from ..hooke.sym import smat_sym_ortho_3d
-
+from ...utils.material.hooke import _get_elastic_params
+from ...utils.material.mindlin import (
+    _get_shell_material_stiffness_matrix,
+    shell_rotation_matrix,
+)
+from ...utils.material.symbolic import smat_sym_ortho_3d
 from .meta import Surface, SurfaceLayer
 
 
 __all__ = ["MindlinShell", "MindlinPlate", "MindlinShellLayer", "MindlinPlateLayer"]
 
 
 class MindlinShellLayer(SurfaceLayer):
@@ -32,115 +36,89 @@
         self.shear_factors_x = np.array([0.0, 0.0, 0.0])
         self.shear_factors_y = np.array([0.0, 0.0, 0.0])
 
         # polinomial coefficients for shear factor interpoaltion
         self.sfx = None
         self.sfy = None
 
-    def material_elastic_stiffness_matrices(self) -> Tuple[ndarray, ndarray]:
+    def material_elastic_stiffness_matrix(self) -> Tuple[ndarray, ndarray]:
+        """
+        Returns the transformed material stiffness matrix.
+        """
+        Cm = _get_shell_material_stiffness_matrix(self.hooke)
+        T = self.rotation_matrix()
+        R = np.diag([1.0, 1.0, 2.0, 2.0, 2.0])
+        self._hooke = inv(T) @ Cm @ R @ T @ inv(R)
+        # self._hooke = T @ Cm @ inv(R) @ T.T @ R
+        return self._hooke
+
+    def rotation_matrix(self) -> Tuple[ndarray, ndarray]:
         """
-        Returns and stores transformed material stiffness matrices.
+        Returns the rotation matrix.
         """
-        Cm = self.hooke
-        Cm_126 = Cm[0:3, 0:3]
-        Cm_45 = Cm[3:, 3:]
-        T_126, T_45 = self.rotation_matrices()
-        R_126 = np.diag([1, 1, 2])
-        R_45 = np.diag([2, 2])
-        C_126 = T_126 @ Cm_126 @ inv(R_126) @ T_126.T @ R_126
-        C_45 = T_45 @ Cm_45 @ inv(R_45) @ T_45.T @ R_45
-        C_126[np.abs(C_126) < 1e-12] = 0.0
-        C_45[np.abs(C_45) < 1e-12] = 0.0
-        self.C_126 = C_126
-        self.C_45 = C_45
-        return C_126, C_45
-
-    def rotation_matrices(self) -> Tuple[ndarray, ndarray]:
-        """
-        Produces transformation matrices T_126 and T_45.
-        """
-        T_126 = np.zeros([3, 3])
-        T_45 = np.zeros([2, 2])
-        angle = self.angle * np.pi / 180
-        #
-        T_126[0, 0] = np.cos(angle) ** 2
-        T_126[0, 1] = np.sin(angle) ** 2
-        T_126[0, 2] = -np.sin(2 * angle)
-        T_126[1, 0] = T_126[0, 1]
-        T_126[1, 1] = T_126[0, 0]
-        T_126[1, 2] = -T_126[0, 2]
-        T_126[2, 0] = np.cos(angle) * np.sin(angle)
-        T_126[2, 1] = -T_126[2, 0]
-        T_126[2, 2] = np.cos(angle) ** 2 - np.sin(angle) ** 2
-        #
-        T_45[0, 0] = np.cos(angle)
-        T_45[0, 1] = -np.sin(angle)
-        T_45[1, 1] = T_45[0, 0]
-        T_45[1, 0] = -T_45[0, 1]
-        #
-        return T_126, T_45
+        return shell_rotation_matrix(self.angle, rad=False)
 
     def elastic_stiffness_matrix(self) -> ndarray:
         """
         Returns the uncorrected stiffness contribution to the layer.
         """
-        C_126, C_45 = self.material_elastic_stiffness_matrices()
+        C = self.material_elastic_stiffness_matrix()
         tmin = self.tmin
         tmax = self.tmax
-        A = C_126 * (tmax - tmin)
-        B = (1 / 2) * C_126 * (tmax**2 - tmin**2)
-        D = (1 / 3) * C_126 * (tmax**3 - tmin**3)
-        S = C_45 * (tmax - tmin)
-        ABDS = np.zeros([8, 8])
+        A = C[:3, :3] * (tmax - tmin)
+        B = (1 / 2) * C[:3, :3] * (tmax**2 - tmin**2)
+        D = (1 / 3) * C[:3, :3] * (tmax**3 - tmin**3)
+        S = C[3:, 3:] * (tmax - tmin)
+        ABDS = np.zeros([8, 8], dtype=float)
         ABDS[0:3, 0:3] = A
         ABDS[0:3, 3:6] = B
         ABDS[3:6, 0:3] = B
         ABDS[3:6, 3:6] = D
         ABDS[6:8, 6:8] = S
         return ABDS
 
     def compile_shear_factors(self):
         """
         Prepares data for continuous interpolation of shear factors. Should
         be called if shear factors are already set.
         """
-        coeff_inv = np.linalg.inv(np.array([[1, z, z**2] for z in self.zi]))
+        coeff_inv = inv(np.array([[1, z, z**2] for z in self.zi]))
         self.sfx = np.matmul(coeff_inv, self.shear_factors_x)
         self.sfy = np.matmul(coeff_inv, self.shear_factors_y)
 
-    def loc_to_shear_factors(self, loc: float):
+    def loc_to_shear_factors(self, loc: float) -> Tuple[float, float]:
         """
         Returns shear factor for local z direction by quadratic interpolation.
         Local coordinate is expected between -1 and 1.
         """
         z = self.loc_to_z(loc)
         monoms = np.array([1, z, z**2])
         return np.dot(monoms, self.sfx), np.dot(monoms, self.sfy)
 
     def approxfunc(self, data) -> Callable:
         z0, z1, z2 = self.zi
         z = np.array([[1, z0, z0**2], [1, z1, z1**2], [1, z2, z2**2]])
-        a, b, c = np.linalg.inv(z) @ np.array(data)
+        a, b, c = inv(z) @ np.array(data)
         return lambda z: a + b * z + c * z**2
 
 
 class MindlinPlateLayer(MindlinShellLayer):
     """
     Helper object for the stress analysis of a layer of a plate.
     """
 
     def elastic_stiffness_matrix(self) -> ndarray:
         """
         Returns the uncorrected stiffness contribution to the layer.
         """
-        C_126, C_45 = self.material_elastic_stiffness_matrices()
+        C = self.material_elastic_stiffness_matrix()
         tmin = self.tmin
         tmax = self.tmax
-        D = (1 / 3) * C_126 * (tmax**3 - tmin**3)
-        S = C_45 * (tmax - tmin)
+        D = (1 / 3) * C[:3, :3] * (tmax**3 - tmin**3)
+        S = C[3:, 3:] * (tmax - tmin)
         ABDS = np.zeros([5, 5])
         ABDS[:3, :3] = D
         ABDS[3:, 3:] = S
         return ABDS
 
 
 class MindlinShell(Surface):
@@ -148,110 +126,118 @@
     Helper object for the stress analysis of a shell.
 
     Example
     -------
     >>> from sigmaepsilon.material import MindlinShell
     >>> model = {
     >>>     '0' : {
-    >>>         'hooke' : MindlinShell.Hooke(E=2100000, nu=0.3),
+    >>>         'hooke' : MindlinShell.Hooke(E=2100000, NU=0.3),
     >>>         'angle' : 0.,
     >>>         'thickness' : 0.1
     >>>         },
     >>>     }
     >>> C = MindlinShell.from_dict(model).elastic_stiffness_matrix()
     """
 
     __layerclass__ = MindlinShellLayer
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
     @classmethod
     def Hooke(cls, symbolic: bool = False, **kwargs) -> Union[sy.Matrix, np.ndarray]:
         """
         Returns a Hooke matrix appropriate for shells.
 
         Parameters
         ----------
-        symbolic : bool, Optional
-            If Truem a symbolic matrix is returned.
+        symbolic: bool, Optional
+            If True, a symbolic matrix is returned.
 
         Returns
         -------
         Union[sympy.Matrix, numpy.ndarray]
             The matrix in symbolic or numeric form.
 
         Examples
         --------
         >>> from sigmaepsilon.material import MindlinShell
-        >>> MindlinShell.Hooke(E=2100000, nu=0.3)
+        >>> MindlinShell.Hooke(E=2100000, NU=0.3)
         >>> MindlinShell.Hooke(symbolic=True)
         """
         S = smat_sym_ortho_3d()
         S.row_del(2)
         S.col_del(2)
 
         if symbolic:
             return S.inv()
 
         constants = _get_elastic_params(**kwargs)
         subs = {s: constants[str(s)] for s in S.free_symbols}
         S = S.subs([(sym, val) for sym, val in subs.items()])
         S = np.array(S, dtype=float)
-        return np.linalg.inv(S)
+        return inv(S)
 
     def elastic_stiffness_matrix(self) -> ndarray:
         """
         Returns the stiffness matrix of the shell.
 
         Returns
         -------
         numpy.ndarray
             The ABDS matrix of the shell.
         """
         ABDS = super().elastic_stiffness_matrix()
-        layers = self.layers()
+        layers: Iterable[MindlinShellLayer] = self.layers()
         A11 = ABDS[0, 0]
         B11 = ABDS[0, 3]
         D11 = ABDS[3, 3]
         S55 = ABDS[6, 6]
         A22 = ABDS[1, 1]
         B22 = ABDS[1, 4]
         D22 = ABDS[4, 4]
         S44 = ABDS[7, 7]
+
+        ABDS_inv = np.linalg.inv(ABDS[:6, :6])
+        alpha_x = ABDS_inv[0, 3]
+        beta_x = ABDS_inv[3, 3]
+        alpha_y = ABDS_inv[1, 4]
+        beta_y = ABDS_inv[4, 4]
+
         eta_x = 1 / (A11 * D11 - B11**2)
         eta_y = 1 / (A22 * D22 - B22**2)
+        alpha_x = -B11 * eta_x
+        beta_x = A11 * eta_x
+        alpha_y = -B22 * eta_y
+        beta_y = A22 * eta_y
 
         # Create shear factors. These need to be multiplied with the shear
         # force in order to obtain shear stress at a given height. Since the
         # shear stress distribution is of 2nd order, the factors are
         # determined at 3 locations per layer.
         for i, layer in enumerate(layers):
             zi = layer.zi
-            Exi = layer.C_126[0, 0]
-            Eyi = layer.C_126[1, 1]
+            Exi = layer._hooke[0, 0]
+            Eyi = layer._hooke[1, 1]
 
             # first point through the thickness
             layer.shear_factors_x[0] = layers[i - 1].shear_factors_x[-1]
             layer.shear_factors_y[0] = layers[i - 1].shear_factors_y[-1]
 
             # second point through the thickness
-            layer.shear_factors_x[1] = layer.shear_factors_x[0] - eta_x * Exi * (
-                0.5 * (zi[1] ** 2 - zi[0] ** 2) * A11 - (zi[1] - zi[0]) * B11
+            layer.shear_factors_x[1] = layer.shear_factors_x[0] - Exi * (
+                0.5 * (zi[1] ** 2 - zi[0] ** 2) * beta_x + (zi[1] - zi[0]) * alpha_x
             )
-            layer.shear_factors_y[1] = layer.shear_factors_y[0] - eta_y * Eyi * (
-                0.5 * (zi[1] ** 2 - zi[0] ** 2) * A22 - (zi[1] - zi[0]) * B22
+            layer.shear_factors_y[1] = layer.shear_factors_y[0] - Eyi * (
+                0.5 * (zi[1] ** 2 - zi[0] ** 2) * beta_y + (zi[1] - zi[0]) * alpha_y
             )
 
             # third point through the thickness
-            layer.shear_factors_x[2] = layer.shear_factors_x[0] - eta_x * Exi * (
-                0.5 * (zi[2] ** 2 - zi[0] ** 2) * A11 - (zi[2] - zi[0]) * B11
+            layer.shear_factors_x[2] = layer.shear_factors_x[0] - Exi * (
+                0.5 * (zi[2] ** 2 - zi[0] ** 2) * beta_x + (zi[2] - zi[0]) * alpha_x
             )
-            layer.shear_factors_y[2] = layer.shear_factors_y[0] - eta_y * Eyi * (
-                0.5 * (zi[2] ** 2 - zi[0] ** 2) * A22 - (zi[2] - zi[0]) * B22
+            layer.shear_factors_y[2] = layer.shear_factors_y[0] - Eyi * (
+                0.5 * (zi[2] ** 2 - zi[0] ** 2) * beta_y + (zi[2] - zi[0]) * alpha_y
             )
 
         # remove numerical junk from the end
         layers[-1].shear_factors_x[-1] = 0.0
         layers[-1].shear_factors_y[-1] = 0.0
 
         # prepare data for interpolation of shear stresses in a layer
@@ -268,42 +254,42 @@
         gW = np.array([5 / 9, 8 / 9, 5 / 9])
 
         # potential energy using parabolic stress distribution
         # and unit shear force
         pot_p_x, pot_p_y = 0.0, 0.0
         for layer in layers:
             dJ = 0.5 * (layer.tmax - layer.tmin)
-            Gxi = layer.C_45[0, 0]
-            Gyi = layer.C_45[1, 1]
+            Gxi = layer._hooke[-2, -2]
+            Gyi = layer._hooke[-1, -1]
             for loc, weight in zip(gP, gW):
                 sfx, sfy = layer.loc_to_shear_factors(loc)
                 pot_p_x += 0.5 * (sfx**2) * dJ * weight / Gxi
                 pot_p_y += 0.5 * (sfy**2) * dJ * weight / Gyi
         kx = pot_c_x / pot_p_x
         ky = pot_c_y / pot_p_y
 
         ABDS[6, 6] = kx * S55
         ABDS[7, 7] = ky * S44
         self.kx = kx
         self.ky = ky
         self.ABDS = ABDS
-        self.SDBA = np.linalg.inv(ABDS)
+        self.SDBA = inv(ABDS)
         return ABDS
 
 
 class MindlinPlate(MindlinShell):
     """
     Helper object for the stress analysis of a membrane.
 
     Example
     -------
     >>> from sigmaepsilon.model import MindlinPlate
     >>> model = {
     >>>     '0' : {
-    >>>         'hooke' : MindlinPlate.Hooke(E=2100000, nu=0.3),
+    >>>         'hooke' : MindlinPlate.Hooke(E=2100000, NU=0.3),
     >>>         'angle' : 0.,
     >>>         'thickness' : 0.1
     >>>         },
     >>>     }
     >>> C = MindlinPlate.from_dict(model).elastic_stiffness_matrix()
     """
 
@@ -313,11 +299,11 @@
 
         Returns
         -------
         numpy.ndarray
             The ABDS matrix of the plate.
         """
         ABDS_ = super().elastic_stiffness_matrix()
-        ABDS = np.zeros([5, 5])
+        ABDS = np.zeros([5, 5], dtype=ABDS_.dtype)
         ABDS[:3, :3] = ABDS_[3:6, 3:6]
-        ABDS[3:, 3:] = ABDS_[6:8, 6:8]
+        ABDS[3:, 3:] = ABDS_[6:, 6:]
         return ABDS
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/joint/cubejoint.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/joint/cubejoint.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/oc/filter.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/oc/filter.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/oc/oc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/oc/oc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/topopt/oc/utils.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/topopt/oc/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/cells/bernoulli.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/cells/bernoulli.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/cells/cells.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/cells/cells.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/dyn.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/dyn.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/ebc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/ebc.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,52 +17,51 @@
 ) -> ndarray:
     i = index_of_closest_point(source.show(), target.show())
     link = np.stack([source.id[i], target.id], axis=1)
     return link
 
 
 def link_points_to_body(
-    points: PointCloud, 
+    points: PointCloud,
     body: PolyCell3d,
     lazy: bool = True,
     tol: float = 1e-12,
     k: int = 4,
 ) -> Tuple[ndarray]:
     source_coords = points.show()
     source_indices = points.id
     topo_target = body.topology()
-        
-    i_source, i_target, locations_target = \
-        body.locate(source_coords, lazy, tol, k)
+
+    i_source, i_target, locations_target = body.locate(source_coords, lazy, tol, k)
     source_indices = source_indices[i_source]
     topo_target = topo_target[i_target]
-    
+
     shp_target = body.shape_function_values(locations_target)
-            
+
     nE, nNE = topo_target.shape
     factors = np.zeros((nE, nNE + 1), dtype=float)
     indices = np.zeros((nE, nNE + 1), dtype=int)
     factors[:, -1] = -1
     factors[:, :nNE] = shp_target
     indices[:, -1] = source_indices
     indices[:, :nNE] = topo_target
-    
+
     return factors, indices
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def _body_to_body_stiffness_data_(
-    nodal_factors:ndarray, nodal_indices:ndarray, dofmap:ndarray, ndof:int
+    nodal_factors: ndarray, nodal_indices: ndarray, dofmap: ndarray, ndof: int
 ) -> Tuple[ndarray]:
     nN, nV = nodal_factors.shape
     nDOF = dofmap.shape[0]
     nR = nN * nDOF
     factors = np.zeros((nR, nV), dtype=nodal_factors.dtype)
     indices = np.zeros((nR, nV), dtype=nodal_indices.dtype)
     for i in prange(nN):
         for j in prange(nDOF):
-            ii = i*nDOF + j
+            ii = i * nDOF + j
             for k in prange(nV):
                 ik = nodal_indices[i, k] * ndof + dofmap[j]
                 factors[ii, k] = nodal_factors[i, k]
                 indices[ii, k] = ik
-    return factors, indices
+    return factors, indices
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/eigsolve.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/eigsolve.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/fem.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/fem.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/imap.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/imap.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/linsolve.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/linsolve.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/postproc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/postproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/preproc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/preproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/fem/tr.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/fem/tr.py`

 * *Files 3% similar despite different names*

```diff
@@ -156,7 +156,17 @@
     nodal_loads = np.swapaxes(nodal_loads, 1, 2)
     # (nE, nNE * nDOF, nRHS) -> (nE, nRHS, nNE * nDOF)
     nodal_loads = ascont(nodal_loads)
     nodal_loads = tr_element_vectors_bulk_multi(nodal_loads, dcm)
     nodal_loads = np.swapaxes(nodal_loads, 1, 2)
     # (nE, nRHS, nNE * nDOF) -> (nE, nNE * nDOF, nRHS)
     return nodal_loads
+
+
+@njit(nogil=True, parallel=True, cache=__cache)
+def _scatter_element_frames(frames: ndarray, N: int):
+    nE = frames.shape[0]
+    res = np.zeros((nE, N, 3, 3), dtype=frames.dtype)
+    for iE in prange(nE):
+        for iN in prange(N):
+            res[iE, iN, :, :] = frames[iE]
+    return res
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/bernoulli.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/bernoulli.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/hmh.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/hmh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/material.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/material.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/mindlin.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/mindlin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,52 @@
+from typing import Tuple
+
 import numpy as np
+from numpy import ndarray
 from numpy.linalg import inv
 from numba import njit, prange
 
 from .surface import points_of_layers
 
 __cache = True
 
 
+def _get_shell_material_stiffness_matrix(hooke: ndarray) -> Tuple[ndarray, ndarray]:
+    """
+    Returns the material stiffness matrices C126 and C45 from the 6x6
+    material stiffness matrix.
+    """
+    offset = 0 if hooke.shape[-1] == 6 else 1
+    imap = [0, 1, 5 - offset, 4 - offset, 3 - offset]
+    res = np.zeros((5, 5), dtype=float)
+    for i in range(5):
+        for j in range(5):
+            res[i, j] = hooke[imap[i], imap[j]]
+    return res
+
+
+def shell_rotation_matrix(angle: float, rad: bool = False) -> Tuple[ndarray, ndarray]:
+    if not rad:
+        angle *= np.pi / 180
+    S = np.sin(angle)
+    C = np.cos(angle)
+    return np.array(
+        [
+            [C**2, S**2, 2 * C * S, 0, 0],
+            [S**2, C**2, -2 * C * S, 0, 0],
+            [-C * S, C * S, C**2 - S**2, 0, 0],
+            [0, 0, 0, C, S],
+            [0, 0, 0, -S, C],
+        ],
+        dtype=float,
+    )
+
+
 @njit(nogil=True, parallel=True, cache=__cache)
-def rotation_matrices(angles: np.ndarray):
+def rotation_matrices(angles: ndarray) -> Tuple[ndarray, ndarray]:
     """
     Returns transformation matrices T_126 and T_45 for each angle.
     Angles are expected in radians.
     """
     nL = len(angles)
     T_126 = np.zeros((nL, 3, 3), dtype=angles.dtype)
     T_45 = np.zeros((nL, 2, 2), dtype=angles.dtype)
@@ -32,16 +66,16 @@
         T_45[iL, 1, 1] = T_45[iL, 0, 0]
         T_45[iL, 1, 0] = -T_45[iL, 0, 1]
     return T_126, T_45
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def material_stiffness_matrices(
-    C_126: np.ndarray, C_45: np.ndarray, angles: np.ndarray
-):
+    C_126: ndarray, C_45: ndarray, angles: ndarray
+) -> Tuple[ndarray, ndarray]:
     """
     Returns the components of the material stiffness matrices C_126 and C_45
     in the global system.
     """
     nL = len(C_126)
     C_126_g = np.zeros_like(C_126)
     C_45_g = np.zeros_like(C_45)
@@ -53,15 +87,15 @@
     for iL in prange(nL):
         C_126_g[iL] = T_126[iL] @ C_126[iL] @ R_126_inv @ T_126[iL].T @ R_126
         C_45_g[iL] = T_45[iL] @ C_45[iL] @ R_45_inv @ T_45[iL].T @ R_45
     return C_126_g, C_45_g
 
 
 @njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
-def shear_factors_MT(ABDS: np.ndarray, C_126: np.ndarray, z: np.ndarray):
+def shear_factors_MT(ABDS: ndarray, C_126: ndarray, z: ndarray) -> ndarray:
     """
     # FIXME Should work with parallel = True, does not. Reason is
     propably a race condition due to using explicit parallel loops.
     """
     A11 = ABDS[0, 0]
     B11 = ABDS[0, 3]
     D11 = ABDS[3, 3]
@@ -112,15 +146,15 @@
         )
         shear_factors[iL, 1, iP + 1 :] += dsfy
     shear_factors[iL, :, 2] = 0.0
     return shear_factors
 
 
 @njit(nogil=True, cache=__cache)
-def shear_factors_ST(ABDS: np.ndarray, C_126: np.ndarray, z: np.ndarray):
+def shear_factors_ST(ABDS: ndarray, C_126: ndarray, z: ndarray):
     """
     Single-thread implementation of calculation of shear factors for
     multi-layer Mindlin shells.
     """
     A11 = ABDS[0, 0]
     B11 = ABDS[0, 3]
     D11 = ABDS[3, 3]
@@ -155,16 +189,16 @@
         )
     shear_factors[nL - 1, :, 2] = 0.0
     return shear_factors
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def shear_correction_data(
-    ABDS: np.ndarray, C_126: np.ndarray, C_45: np.ndarray, bounds: np.ndarray
-):
+    ABDS: ndarray, C_126: ndarray, C_45: ndarray, bounds: ndarray
+) -> Tuple[ndarray, ndarray]:
     """
     FIXME : Results are OK, but a bit slower than expected when measured
     against the pure python implementation.
     """
 
     nL = bounds.shape[0]  # number of layers
 
@@ -211,16 +245,16 @@
     ky = pot_c_y / pot_p_y
 
     return np.array([[kx, 0], [0, ky]]), shear_factors
 
 
 @njit(nogil=True, parallel=False, fastmath=True, cache=__cache)
 def stiffness_data(
-    C_126: np.ndarray, C_45: np.ndarray, angles: np.ndarray, bounds: np.ndarray
-):
+    C_126: ndarray, C_45: ndarray, angles: ndarray, bounds: ndarray
+) -> Tuple[ndarray, ndarray, ndarray]:
     """
     FIXME Call
         Ks, sf = shear_correction_data(ABDS, C_126_g, C_45_g, bounds)
     is a bit slow for some reason.
     """
     ABDS = np.zeros((8, 8), dtype=C_126.dtype)
     nL = C_126.shape[0]
@@ -236,10 +270,10 @@
         ABDS[6:8, 6:8] += C_45_g[iL] * (bounds[iL, 1] - bounds[iL, 0])
     ABDS[3:6, 0:3] = ABDS[0:3, 3:6]
     Ks, sf = shear_correction_data(ABDS, C_126_g, C_45_g, bounds)
     return ABDS, Ks, sf
 
 
 @njit(nogil=True, cache=__cache)
-def z_to_shear_factors(z, sfx, sfy):
+def z_to_shear_factors(z: float, sfx: float, sfy: float) -> Tuple[float, float]:
     monoms = np.array([1, z, z**2], dtype=sfx.dtype)
     return np.dot(monoms, sfx), np.dot(monoms, sfy)
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/postproc.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/postproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon/utils/material/surface.py` & `sigmaepsilon-0.0.36/src/sigmaepsilon/utils/material/surface.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon.egg-info/PKG-INFO` & `sigmaepsilon-0.0.36/src/sigmaepsilon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon
-Version: 0.0.34
+Version: 0.0.36
 Summary: High-Performance Computational Mechanics in Python.
 Home-page: https://github.com/dewloosh/sigmaepsilon
-Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.34.zip
+Download-URL: https://github.com/dewloosh/sigmaepsilon/archive/refs/tags/0.0.36.zip
 Author: Bence Balogh
 Author-email: benceeok@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: Free for non-commercial use
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `sigmaepsilon-0.0.34/src/sigmaepsilon.egg-info/SOURCES.txt` & `sigmaepsilon-0.0.36/src/sigmaepsilon.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -46,14 +46,18 @@
 src/sigmaepsilon/fem/cells/q9.py
 src/sigmaepsilon/fem/cells/tet10.py
 src/sigmaepsilon/fem/cells/tet4.py
 src/sigmaepsilon/fem/cells/wedge.py
 src/sigmaepsilon/fem/cells/gen/__init__.py
 src/sigmaepsilon/fem/cells/gen/b2.py
 src/sigmaepsilon/fem/cells/gen/b3.py
+src/sigmaepsilon/fem/homg/__init__.py
+src/sigmaepsilon/fem/homg/ebc.py
+src/sigmaepsilon/fem/homg/rve.py
+src/sigmaepsilon/fem/homg/utils.py
 src/sigmaepsilon/fem/material/__init__.py
 src/sigmaepsilon/fem/material/beam.py
 src/sigmaepsilon/fem/material/membrane.py
 src/sigmaepsilon/fem/material/mindlinplate.py
 src/sigmaepsilon/fem/material/mindlinshell.py
 src/sigmaepsilon/fem/material/solid.py
 src/sigmaepsilon/fem/material/solid3d.py
@@ -64,25 +68,22 @@
 src/sigmaepsilon/fourier/plate.py
 src/sigmaepsilon/fourier/postproc.py
 src/sigmaepsilon/fourier/preproc.py
 src/sigmaepsilon/fourier/problem.py
 src/sigmaepsilon/fourier/proc.py
 src/sigmaepsilon/fourier/utils.py
 src/sigmaepsilon/material/__init__.py
+src/sigmaepsilon/material/straintensor.py
+src/sigmaepsilon/material/stresstensor.py
+src/sigmaepsilon/material/tensor2x3.py
 src/sigmaepsilon/material/beam/__init__.py
 src/sigmaepsilon/material/beam/bernoulli/__init__.py
 src/sigmaepsilon/material/beam/bernoulli/section.py
-src/sigmaepsilon/material/homg/__init__.py
-src/sigmaepsilon/material/homg/ebc.py
-src/sigmaepsilon/material/homg/rve.py
-src/sigmaepsilon/material/homg/utils.py
 src/sigmaepsilon/material/hooke/__init__.py
-src/sigmaepsilon/material/hooke/sym.py
-src/sigmaepsilon/material/hooke/tensor.py
-src/sigmaepsilon/material/hooke/utils.py
+src/sigmaepsilon/material/hooke/elasticitytensor.py
 src/sigmaepsilon/material/surface/__init__.py
 src/sigmaepsilon/material/surface/membrane.py
 src/sigmaepsilon/material/surface/meta.py
 src/sigmaepsilon/material/surface/mindlin.py
 src/sigmaepsilon/topopt/__init__.py
 src/sigmaepsilon/topopt/joint/__init__.py
 src/sigmaepsilon/topopt/joint/cubejoint.py
@@ -103,12 +104,16 @@
 src/sigmaepsilon/utils/fem/tr.py
 src/sigmaepsilon/utils/fem/cells/__init__.py
 src/sigmaepsilon/utils/fem/cells/bernoulli.py
 src/sigmaepsilon/utils/fem/cells/cells.py
 src/sigmaepsilon/utils/material/__init__.py
 src/sigmaepsilon/utils/material/bernoulli.py
 src/sigmaepsilon/utils/material/hmh.py
+src/sigmaepsilon/utils/material/hooke.py
+src/sigmaepsilon/utils/material/imap.py
 src/sigmaepsilon/utils/material/material.py
 src/sigmaepsilon/utils/material/mindlin.py
 src/sigmaepsilon/utils/material/postproc.py
 src/sigmaepsilon/utils/material/surface.py
+src/sigmaepsilon/utils/material/symbolic.py
+src/sigmaepsilon/utils/material/tr.py
 tests/test_bernoulli.py
```

### Comparing `sigmaepsilon-0.0.34/tests/test_bernoulli.py` & `sigmaepsilon-0.0.36/tests/test_bernoulli.py`

 * *Files identical despite different names*

