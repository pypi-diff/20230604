# Comparing `tmp/neuralprocesses-0.2.0.tar.gz` & `tmp/neuralprocesses-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuralprocesses-0.2.0.tar", last modified: Mon Mar  6 18:05:40 2023, max compression
+gzip compressed data, was "neuralprocesses-0.2.1.tar", last modified: Sun Jun  4 12:54:02 2023, max compression
```

## Comparing `neuralprocesses-0.2.0.tar` & `neuralprocesses-0.2.1.tar`

### file list

```diff
@@ -1,163 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.221700 neuralprocesses-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.205700 neuralprocesses-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.205700 neuralprocesses-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/.github/workflows/build_book.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/.github/workflows/style.yml
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-03-06 18:05:40.221700 neuralprocesses-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.209700 neuralprocesses-0.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/_toc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/advanced_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/architectures.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/basic_usage.md
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/build_your_own_model.md
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/coders.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/docs/references.bib
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.209700 neuralprocesses-0.2.0/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.209700 neuralprocesses-0.2.0/experiment/data/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/data/antarctica.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/data/eeg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/data/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/data/predprey.py
--rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/data/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/experiment/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.209700 neuralprocesses-0.2.0/neuralprocesses/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-06 18:05:40.000000 neuralprocesses-0.2.0/neuralprocesses/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.213700 neuralprocesses-0.2.0/neuralprocesses/architectures/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/architectures/agnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/architectures/climate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/architectures/convgnp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/architectures/fullconvgnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7943 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/architectures/gnp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/architectures/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.213700 neuralprocesses-0.2.0/neuralprocesses/coders/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/deepset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/densecov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/fuse.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/mapdiag.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/nn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.213700 neuralprocesses-0.2.0/neuralprocesses/coders/setconv/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/setconv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/setconv/density.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/setconv/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/setconv/setconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coders/shaping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/coding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.213700 neuralprocesses-0.2.0/neuralprocesses/data/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/antarctica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/eeg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/mixgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/predefined.py
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/predprey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/sawtooth.py
--rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/data/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/datadims.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/disc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.217700 neuralprocesses-0.2.0/neuralprocesses/dist/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/dist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/dist/dirac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/dist/dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/dist/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/dist/normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/dist/transformed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/dist/uniform.py
--rw-r--r--   0 runner    (1001) docker     (123)     9188 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/materialise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.217700 neuralprocesses-0.2.0/neuralprocesses/model/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/model/ar.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/model/elbo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/model/loglik.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/model/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/model/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/numdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.217700 neuralprocesses-0.2.0/neuralprocesses/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/tensorflow/nn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.217700 neuralprocesses-0.2.0/neuralprocesses/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/neuralprocesses/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.209700 neuralprocesses-0.2.0/neuralprocesses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-03-06 18:05:40.000000 neuralprocesses-0.2.0/neuralprocesses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-03-06 18:05:40.000000 neuralprocesses-0.2.0/neuralprocesses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 18:05:40.000000 neuralprocesses-0.2.0/neuralprocesses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-06 18:05:40.000000 neuralprocesses-0.2.0/neuralprocesses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-06 18:05:40.000000 neuralprocesses-0.2.0/neuralprocesses.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.217700 neuralprocesses-0.2.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/scripts/predprey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/scripts/predprey_visualise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/scripts/sawtooth_sample_ar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/scripts/synthetic_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/scripts/synthetic_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/scripts/temperature_mae.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/scripts/temperature_summarise_folds.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/scripts/temperature_visualise.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-06 18:05:40.221700 neuralprocesses-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    27121 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tables.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.217700 neuralprocesses-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.217700 neuralprocesses-0.2.0/tests/coders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/coders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/coders/test_shaping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.217700 neuralprocesses-0.2.0/tests/dists/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/dists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/dists/test_normal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:40.221700 neuralprocesses-0.2.0/tests/gnp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/gnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/gnp/autoencoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/gnp/gnp.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/gnp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_augment.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_discretisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_unet.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/todo.tasks
--rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-03-06 18:05:30.000000 neuralprocesses-0.2.0/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.636667 neuralprocesses-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.644667 neuralprocesses-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.github/workflows/build_book.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.github/workflows/style.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.644667 neuralprocesses-0.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/_toc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/advanced_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/architectures.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/basic_usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/build_your_own_model.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/coders.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/docs/references.bib
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.648667 neuralprocesses-0.2.1/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.648667 neuralprocesses-0.2.1/experiment/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/antarctica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/eeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/predprey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5348 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8322 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/experiment/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.652667 neuralprocesses-0.2.1/neuralprocesses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.652667 neuralprocesses-0.2.1/neuralprocesses/architectures/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/agnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/climate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/convgnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/fullconvgnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/gnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/architectures/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.656667 neuralprocesses-0.2.1/neuralprocesses/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/deepset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/densecov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/fuse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/mapdiag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/nn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.656667 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/setconv/setconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coders/shaping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/coding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.660667 neuralprocesses-0.2.1/neuralprocesses/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/antarctica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/bimodal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/eeg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/mixgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/predefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/predprey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/sawtooth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27362 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/data/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/datadims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/disc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.664667 neuralprocesses-0.2.1/neuralprocesses/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/dirac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7430 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/spikeslab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/transformed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/dist/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/materialise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.664667 neuralprocesses-0.2.1/neuralprocesses/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/elbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/loglik.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/model/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/numdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.664667 neuralprocesses-0.2.1/neuralprocesses/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/tensorflow/nn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.668667 neuralprocesses-0.2.1/neuralprocesses/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6413 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/neuralprocesses/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.652667 neuralprocesses-0.2.1/neuralprocesses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3954 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-04 12:54:02.000000 neuralprocesses-0.2.1/neuralprocesses.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11863 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.668667 neuralprocesses-0.2.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/predprey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/predprey_visualise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/sawtooth_sample_ar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/synthetic_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15625 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/synthetic_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/temperature_mae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/temperature_summarise_folds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/scripts/temperature_visualise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      355 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27121 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tables.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/tests/coders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/coders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/coders/test_shaping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/tests/dists/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/dists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/dists/test_normal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 12:54:02.672667 neuralprocesses-0.2.1/tests/gnp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/gnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/gnp/autoencoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/gnp/gnp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/gnp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13948 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_augment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_discretisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9301 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/todo.tasks
+-rw-r--r--   0 runner    (1001) docker     (123)    26899 2023-06-04 12:53:45.000000 neuralprocesses-0.2.1/train.py
```

### Comparing `neuralprocesses-0.2.0/.github/workflows/build_book.yml` & `neuralprocesses-0.2.1/.github/workflows/build_book.yml`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/.github/workflows/ci.yml` & `neuralprocesses-0.2.1/.github/workflows/ci.yml`

 * *Files 24% similar despite different names*

```diff
@@ -8,36 +8,39 @@
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-version: [3.7, 3.8, 3.9]
     steps:
       - uses: actions/checkout@v2
+        with:
+          fetch-depth: 0
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v2
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           sudo apt-get install gfortran
-          python -m pip install --upgrade pip
+          pip install --upgrade pip setuptools 'setuptools_scm[toml]' setuptools_scm_git_archive numpy Cython
+          python setup.py --version
           pip install --no-cache-dir -U -r requirements.txt | cat
+          pip install --upgrade numpy
       - name: Test
-        env:
-          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
-          COVERALLS_FLAG_NAME: ${{ matrix.python-version }}
-          COVERALLS_PARALLEL: true
         run: |
           pytest -v --cov=neuralprocesses --cov-report term-missing
           coveralls --service=github
-  coveralls:
-    name: Finish coverage
+        env:
+          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+          COVERALLS_FLAG_NAME: ${{ matrix.test-name }}
+          COVERALLS_PARALLEL: true
+
+  finish:
+    name: Finish Coveralls
     needs: test
     runs-on: ubuntu-latest
-    container: python:3-slim
     steps:
-    - name: Finished
-      run: |
-        pip3 install --upgrade coveralls
-        coveralls --finish
-      env:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+    - name: Finish Coveralls
+      uses: coverallsapp/github-action@v1
+      with:
+        github-token: ${{ secrets.github_token }}
+        parallel-finished: true
```

### Comparing `neuralprocesses-0.2.0/.github/workflows/publish.yml` & `neuralprocesses-0.2.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/.github/workflows/style.yml` & `neuralprocesses-0.2.1/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/LICENCE.txt` & `neuralprocesses-0.2.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/PKG-INFO` & `neuralprocesses-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralprocesses
-Version: 0.2.0
+Version: 0.2.1
 Summary: A framework for composing Neural Processes in Python
 Home-page: https://github.com/wesselb/neuralprocesses
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `neuralprocesses-0.2.0/README.md` & `neuralprocesses-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/docs/_config.yml` & `neuralprocesses-0.2.1/docs/_config.yml`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/docs/advanced_usage.md` & `neuralprocesses-0.2.1/docs/advanced_usage.md`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/docs/architectures.rst` & `neuralprocesses-0.2.1/docs/architectures.rst`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/docs/basic_usage.md` & `neuralprocesses-0.2.1/docs/basic_usage.md`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/docs/build_your_own_model.md` & `neuralprocesses-0.2.1/docs/build_your_own_model.md`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/docs/coders.rst` & `neuralprocesses-0.2.1/docs/coders.rst`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/docs/logo.png` & `neuralprocesses-0.2.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/experiment/data/antarctica.py` & `neuralprocesses-0.2.1/experiment/data/antarctica.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/experiment/data/eeg.py` & `neuralprocesses-0.2.1/experiment/data/eeg.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/experiment/data/gp.py` & `neuralprocesses-0.2.1/experiment/data/gp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/experiment/data/predprey.py` & `neuralprocesses-0.2.1/experiment/data/predprey.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/experiment/data/temperature.py` & `neuralprocesses-0.2.1/experiment/data/temperature.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/experiment/data/util.py` & `neuralprocesses-0.2.1/experiment/data/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/experiment/plot.py` & `neuralprocesses-0.2.1/experiment/plot.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/experiment/util.py` & `neuralprocesses-0.2.1/experiment/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/__init__.py` & `neuralprocesses-0.2.1/neuralprocesses/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/aggregate.py` & `neuralprocesses-0.2.1/neuralprocesses/aggregate.py`

 * *Files 14% similar despite different names*

```diff
@@ -75,22 +75,27 @@
             _assert_equal_lengths(*args)
             return Aggregate(*(getattr(B, name)(*xs, **kw_args) for xs in zip(*args)))
 
     else:
         raise ValueError(f"Invalid number of arguments {num_args}.")
 
 
+_map_f("expand_dims", 1)
+_map_f("exp", 1)
+_map_f("one", 1)
+_map_f("zero", 1)
 _map_f("mean", 1)
+_map_f("sum", 1)
+_map_f("logsumexp", 1)
 
 _map_f("add", 2)
 _map_f("subtract", 2)
 _map_f("multiply", 2)
 _map_f("divide", 2)
 
-
 _map_f("stack", "*")
 _map_f("concat", "*")
 _map_f("squeeze", "*")
 
 
 @B.dispatch
 def max(a: Aggregate):
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/architectures/agnp.py` & `neuralprocesses-0.2.1/neuralprocesses/architectures/agnp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import neuralprocesses as nps  # This fixes inspection below.
+
 from ..util import register_model
 
 __all__ = ["construct_agnp"]
 
 
 @register_model
 def construct_agnp(*args, nps=nps, num_heads=8, **kw_args):
@@ -30,15 +31,15 @@
         width (int, optional): Widths of all intermediate MLPs. Defaults to 512.
         likelihood (str, optional): Likelihood. Must be one of `"het"` or `"lowrank"`.
             Defaults to `"lowrank"`.
         num_basis_functions (int, optional): Number of basis functions for the
             low-rank likelihood. Defaults to 512.
         dim_lv (int, optional): Dimensionality of the latent variable. Defaults to 0.
         lv_likelihood (str, optional): Likelihood of the latent variable. Must be one of
-            `"het"` or `"dense"`. Defaults to `"het"`.
+            `"het"`, `"dense"`, or `"spikes-beta"`. Defaults to `"het"`.
         transform (str or tuple[float, float]): Bijection applied to the
             output of the model. This can help deal with positive of bounded data.
             Must be either `"positive"`, `"exp"`, `"softplus"`, or
             `"softplus_of_square"` for positive data or `(lower, upper)` for data in
             this open interval.
         dtype (dtype, optional): Data type.
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/architectures/climate.py` & `neuralprocesses-0.2.1/neuralprocesses/architectures/climate.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/architectures/convgnp.py` & `neuralprocesses-0.2.1/neuralprocesses/architectures/convgnp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-import lab as B
-import wbml.out as out
+import neuralprocesses as nps  # This fixes inspection below.
 from plum import convert
 
-import neuralprocesses as nps  # This fixes inspection below.
-from .util import construct_likelihood, parse_transform
 from ..util import register_model
+from .util import construct_likelihood, parse_transform
 
 __all__ = ["construct_convgnp"]
 
 
 def _convgnp_init_dims(dim_yc, dim_yt, dim_y):
     # Make sure that `dim_yc` is initialised and a tuple.
     dim_yc = convert(dim_yc or dim_y, tuple)
@@ -26,15 +24,15 @@
     conv_receptive_field,
 ):
     if "unet" in conv_arch:
         conv_out_channels = unet_channels[0]
     elif "conv" in conv_arch:
         conv_out_channels = conv_channels
         if conv_receptive_field is None:
-            raise ValueError(f"Must specify `conv_receptive_field`.")
+            raise ValueError("Must specify `conv_receptive_field`.")
     else:
         raise ValueError(f'Architecture "{conv_arch}" invalid.')
     return conv_out_channels
 
 
 def _convgnp_construct_encoder_setconvs(
     nps,
@@ -58,14 +56,24 @@
         *(
             nps.SetConv(s, dtype=dtype, learnable=encoder_scales_learnable)
             for s in encoder_scales
         )
     )
 
 
+def _convgnp_assert_form_contexts(nps, dim_yc):
+    if len(dim_yc) == 1:
+        return nps.Chain(
+            nps.SqueezeParallel(),
+            nps.AssertNoParallel(),
+        )
+    else:
+        return nps.AssertParallel(len(dim_yc))
+
+
 def _convgnp_construct_decoder_setconv(
     nps,
     decoder_scale,
     disc,
     dtype=None,
     init_factor=1,
     decoder_scale_learnable=True,
@@ -136,16 +144,16 @@
             not equal to the dimensionality of the outputs of the context set.
         dim_aux_t (int, optional): Dimensionality of target-specific auxiliary
             variables.
         points_per_unit (float, optional): Density of the internal discretisation.
             Defaults to 64.
         margin (float, optional): Margin of the internal discretisation. Defaults to
             0.1.
-        likelihood (str, optional): Likelihood. Must be one of `"het"` or `"lowrank".
-            Defaults to `"lowrank"`.
+        likelihood (str, optional): Likelihood. Must be one of `"het"`, `"lowrank"`,
+            or `"spikes-beta"`. Defaults to `"lowrank"`.
         conv_arch (str, optional): Convolutional architecture to use. Must be one of
             `"unet[-res][-sep]"` or `"conv[-res][-sep]"`. Defaults to `"unet"`.
         unet_channels (tuple[int], optional): Channels of every layer of the UNet.
             Defaults to six layers each with 64 channels.
         unet_kernels (int or tuple[int], optional): Sizes of the kernels in the UNet.
             Defaults to 5.
         unet_strides (int or tuple[int], optional): Strides in the UNet. Defaults to 2.
@@ -155,16 +163,16 @@
             transposed convolutions in the UNet. Defaults to `False`.
         unet_resize_conv_interp_method (str, optional): Interpolation method for the
             resize convolutions in the UNet. Can be set to `"bilinear"`. Defaults
             to "nearest".
         conv_receptive_field (float, optional): Receptive field of the standard
             architecture. Must be specified if `conv_arch` is set to `"conv"`.
         conv_layers (int, optional): Layers of the standard architecture. Defaults to 8.
-        conv_channels (int, optional): Channels of the standard architecture. Defaults to
-            64.
+        conv_channels (int, optional): Channels of the standard architecture. Defaults
+            to 64.
         num_basis_functions (int, optional): Number of basis functions for the
             low-rank likelihood. Defaults to `512`.
         dim_lv (int, optional): Dimensionality of the latent variable. Defaults to 0.
         lv_likelihood (str, optional): Likelihood of the latent variable. Must be one of
             `"het"` or `"lowrank"`. Defaults to `"het"`.
         encoder_scales (float or tuple[float], optional): Initial value for the length
             scales of the set convolutions for the context sets embeddings. Defaults
@@ -251,14 +259,16 @@
                 out_channels=likelihood_in_channels,
                 dtype=dtype,
             )
         else:
             # Not necessary. Just let the CNN produce the right number of channels.
             conv_out_channels = likelihood_in_channels
             linear_after_set_conv = lambda x: x
+        # Also assert that there is no augmentation given.
+        likelihood = nps.Chain(nps.AssertNoAugmentation(), likelihood)
 
     # Construct the core CNN architectures for the encoder, which is only necessary
     # if we're using a latent variable, and for the decoder. First, we determine
     # how many channels these architectures should take in and produce.
     if dim_lv > 0:
         lv_in_channels = conv_in_channels
         lv_out_channels = lv_likelihood_in_channels
@@ -344,14 +354,15 @@
     )
 
     # Construct model.
     model = nps.Model(
         nps.FunctionalCoder(
             disc,
             nps.Chain(
+                _convgnp_assert_form_contexts(nps, dim_yc),
                 nps.PrependDensityChannel(),
                 _convgnp_construct_encoder_setconvs(
                     nps,
                     encoder_scales,
                     dim_yc,
                     disc,
                     dtype,
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/architectures/fullconvgnp.py` & `neuralprocesses-0.2.1/neuralprocesses/architectures/fullconvgnp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+import neuralprocesses as nps  # This fixes inspection below.
 import wbml.out as out
 
-import neuralprocesses as nps  # This fixes inspection below.
+from ..util import register_model
 from .convgnp import (
-    _convgnp_init_dims,
-    _convgnp_resolve_architecture,
+    _convgnp_assert_form_contexts,
+    _convgnp_construct_decoder_setconv,
     _convgnp_construct_encoder_setconvs,
+    _convgnp_init_dims,
     _convgnp_optional_division_by_density,
-    _convgnp_construct_decoder_setconv,
+    _convgnp_resolve_architecture,
 )
 from .util import parse_transform
-from ..util import register_model
 
 __all__ = ["construct_fullconvgnp"]
 
 
 @register_model
 def construct_fullconvgnp(
     dim_x=1,
@@ -207,14 +208,15 @@
     model = nps.Model(
         nps.Chain(
             nps.Copy(2),
             nps.Parallel(
                 nps.FunctionalCoder(
                     disc_mean,
                     nps.Chain(
+                        _convgnp_assert_form_contexts(nps, dim_yc),
                         nps.PrependDensityChannel(),
                         _convgnp_construct_encoder_setconvs(
                             nps,
                             encoder_scales,
                             dim_yc,
                             disc_mean,
                             dtype,
@@ -228,14 +230,15 @@
                         nps.DeterministicLikelihood(),
                     ),
                 ),
                 nps.FunctionalCoder(
                     disc_kernel,
                     nps.MapDiagonal(  # Map to diagonal of squared space.
                         nps.Chain(
+                            _convgnp_assert_form_contexts(nps, dim_yc),
                             nps.PrependDensityChannel(),
                             _convgnp_construct_encoder_setconvs(
                                 nps,
                                 encoder_scales,
                                 dim_yc,
                                 disc_kernel,
                                 dtype,
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/architectures/gnp.py` & `neuralprocesses-0.2.1/neuralprocesses/architectures/gnp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+import neuralprocesses as nps  # This fixes inspection below.
 from plum import convert
 
-import neuralprocesses as nps  # This fixes inspection below.
-from .util import construct_likelihood, parse_transform
 from ..util import register_model
+from .convgnp import _convgnp_assert_form_contexts
+from .util import construct_likelihood, parse_transform
 
 __all__ = ["construct_gnp"]
 
 
 @register_model
 def construct_gnp(
     dim_x=1,
@@ -54,15 +55,15 @@
         width (int, optional): Widths of all intermediate MLPs. Defaults to 512.
         likelihood (str, optional): Likelihood. Must be one of `"het"` or `"lowrank"`.
             Defaults to `"lowrank"`.
         num_basis_functions (int, optional): Number of basis functions for the
             low-rank likelihood. Defaults to 512.
         dim_lv (int, optional): Dimensionality of the latent variable. Defaults to 0.
         lv_likelihood (str, optional): Likelihood of the latent variable. Must be one of
-            `"het"` or `"dense"`. Defaults to `"het"`.
+            `"het"`, `"dense"`, or `"spikes-beta"`. Defaults to `"het"`.
         transform (str or tuple[float, float]): Bijection applied to the
             output of the model. This can help deal with positive of bounded data.
             Must be either `"positive"`, `"exp"`, `"softplus"`, or
             `"softplus_of_square"` for positive data or `(lower, upper)` for data in
             this open interval.
         dtype (dtype, optional): Data type.
 
@@ -181,14 +182,15 @@
             ),
             lv_likelihood,
         )
 
     encoder = nps.Chain(
         # We need to explicitly copy, because there will be multiple context sets in
         # parallel, which will otherwise dispatch to the wrong method.
+        _convgnp_assert_form_contexts(nps, dim_yc),
         nps.Copy(2 + (dim_lv > 0)),
         nps.Parallel(
             nps.Chain(
                 nps.RepeatForAggregateInputs(
                     nps.InputsCoder(),
                 ),
                 nps.DeterministicLikelihood(),
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/architectures/util.py` & `neuralprocesses-0.2.1/neuralprocesses/architectures/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 
 def construct_likelihood(nps=nps, *, spec, dim_y, num_basis_functions, dtype):
     """Construct the likelihood.
 
     Args:
         nps (module): Appropriate backend-specific module.
-        spec (str, optional): Specification. Must be one of `"het"`, `"lowrank"`, or
-            `"dense"`. Defaults to `"lowrank"`. Must be given as a keyword argument.
+        spec (str, optional): Specification. Must be one of `"het"`, `"lowrank"`,
+            `"dense"`, or `"spikes-beta"`. Defaults to `"lowrank"`. Must be given as
+            a keyword argument.
         dim_y (int): Dimensionality of the outputs. Must be given as a keyword argument.
         num_basis_functions (int): Number of basis functions for the low-rank
             likelihood. Must be given as a keyword argument.
         dtype (dtype): Data type. Must be given as a keyword argument.
 
     Returns:
         int: Number of channels that the likelihood requires.
@@ -43,14 +44,18 @@
                 nps.Chain(
                     nps.ToDenseCovariance(),
                     nps.DenseCovariancePSDTransform(),
                 ),
             ),
             nps.DenseGaussianLikelihood(),
         )
+    elif spec == "spikes-beta":
+        num_channels = (2 + 3) * dim_y  # Alpha, beta, and three log-probabilities
+        selector = nps.SelectFromChannels(dim_y, dim_y, dim_y, dim_y, dim_y)
+        lik = nps.SpikesBetaLikelihood()
 
     else:
         raise ValueError(f'Incorrect likelihood specification "{spec}".')
     return num_channels, selector, lik
 
 
 def parse_transform(nps=nps, *, transform):
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/augment.py` & `neuralprocesses-0.2.1/neuralprocesses/augment.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/chain.py` & `neuralprocesses-0.2.1/neuralprocesses/chain.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/aggregate.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/aggregate.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/attention.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/attention.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/augment.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/augment.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import lab as B
 
 from .. import _dispatch
 from ..augment import AugmentedInput
 from ..datadims import data_dims
 from ..materialise import _repeat_concat
-from ..util import register_module, register_composite_coder
+from ..util import register_composite_coder, register_module
 
-__all__ = ["Augment"]
+__all__ = ["Augment", "AssertNoAugmentation"]
 
 
 @register_composite_coder
 @register_module
 class Augment:
     """Concatenate the augmentation of the input to the encoding, and remove any
     augmentation of target inputs.
@@ -43,7 +43,22 @@
 def _augment(xz: AugmentedInput, z: B.Numeric):
     return xz.x, _repeat_concat(data_dims(xz), z, xz.augmentation)
 
 
 @_dispatch
 def _augment(xz: AugmentedInput):
     return xz.x
+
+
+@register_module
+class AssertNoAugmentation:
+    """Assert no augmentation of the target inputs."""
+
+
+@_dispatch
+def code(coder: AssertNoAugmentation, xz, z, x, **kw_args):
+    return xz, z
+
+
+@_dispatch
+def code(coder: AssertNoAugmentation, xz, z, x: AugmentedInput, **kw_args):
+    raise AssertionError("Did not expect augmentation of the target inputs.")
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/deepset.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/deepset.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/densecov.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/densecov.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/functional.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/functional.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/fuse.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/fuse.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/mapdiag.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/mapdiag.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/nn.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/nn.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/setconv/density.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/setconv/density.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/setconv/identity.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/setconv/identity.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coders/setconv/setconv.py` & `neuralprocesses-0.2.1/neuralprocesses/coders/setconv/setconv.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/coding.py` & `neuralprocesses-0.2.1/neuralprocesses/coding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import matrix  # noqa
 from plum import isinstance, issubclass
 
 from . import _dispatch
-from .dist import AbstractMultiOutputDistribution, Dirac
+from .dist import AbstractDistribution, Dirac
 from .parallel import Parallel
 from .util import is_composite_coder
 
 __all__ = [
     "code",
     "code_track",
     "recode",
@@ -66,15 +66,15 @@
 
 
 @_dispatch
 def code_track(coder, xz, z, x, h, **kw_args):
     if is_composite_coder(coder):
         raise RuntimeError(
             f"Dispatched to fallback implementation of `code_track` for "
-            f"`{ptype(type(coder))}`, but the coder is composite."
+            f"`{type(coder)}`, but the coder is composite."
         )
     xz, z = code(coder, xz, z, x, **kw_args)
     return xz, z, h + [x]
 
 
 @_dispatch
 def recode(coder, xz, z, h, **kw_args):
@@ -91,15 +91,15 @@
         input: Input of encoding.
         tensor: Encoding.
         list: Remainder of the target history.
     """
     if is_composite_coder(coder):
         raise RuntimeError(
             f"Dispatched to fallback implementation of `recode` for "
-            f"`{ptype(type(coder))}`, but the coder is composite."
+            f"`{type(coder)}`, but the coder is composite."
         )
     xz, z = code(coder, xz, z, h[0], **kw_args)
     return xz, z, h[1:]
 
 
 @_dispatch
 def recode_stochastic(coders: Parallel, codings: Parallel, xc, yc, h, **kw_args):
@@ -147,10 +147,10 @@
 @_dispatch
 def _choose(new: Dirac, old: Dirac):
     # Do not recode `Dirac`s.
     return old
 
 
 @_dispatch
-def _choose(new: AbstractMultiOutputDistribution, old: AbstractMultiOutputDistribution):
+def _choose(new: AbstractDistribution, old: AbstractDistribution):
     # Do recode other distributions.
     return new
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/antarctica.py` & `neuralprocesses-0.2.1/neuralprocesses/data/antarctica.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/batch.py` & `neuralprocesses-0.2.1/neuralprocesses/data/batch.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/data.py` & `neuralprocesses-0.2.1/neuralprocesses/data/data.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/eeg.py` & `neuralprocesses-0.2.1/neuralprocesses/data/eeg.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/gp.py` & `neuralprocesses-0.2.1/neuralprocesses/data/gp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/mixgp.py` & `neuralprocesses-0.2.1/neuralprocesses/data/mixgp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/mixture.py` & `neuralprocesses-0.2.1/neuralprocesses/data/mixture.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/predefined.py` & `neuralprocesses-0.2.1/neuralprocesses/data/predefined.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/predprey.py` & `neuralprocesses-0.2.1/neuralprocesses/data/predprey.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/sawtooth.py` & `neuralprocesses-0.2.1/neuralprocesses/data/sawtooth.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/temperature.py` & `neuralprocesses-0.2.1/neuralprocesses/data/temperature.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/data/util.py` & `neuralprocesses-0.2.1/neuralprocesses/data/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/datadims.py` & `neuralprocesses-0.2.1/neuralprocesses/datadims.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/disc.py` & `neuralprocesses-0.2.1/neuralprocesses/disc.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/dist/dirac.py` & `neuralprocesses-0.2.1/neuralprocesses/dist/dirac.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,96 +1,98 @@
 import lab as B
+from plum import parametric
 from wbml.util import indented_kv
 
-from .dist import AbstractMultiOutputDistribution
 from .. import _dispatch
 from ..aggregate import Aggregate
 from ..util import batch
+from .dist import AbstractDistribution
 
 __all__ = ["Dirac"]
 
 
-class Dirac(AbstractMultiOutputDistribution):
+@parametric
+class Dirac(AbstractDistribution):
     """A Dirac delta.
 
-    Also accepts aggregated of its arguments.
-
     Args:
-        x (tensor): Position of the Dirac delta of shape `(*b, c, *n)`.
-        d (int): Dimensionality of the data, i.e. `len(n)`.
+        x (tensor): Position of the Dirac delta.
+        d (int): Dimensionality of the data.
 
     Attributes:
-        x (tensor): Position of the Dirac delta of shape `(*b, c, *n)`.
-        d (int): Dimensionality of the data, i.e. `len(n)`.
+        x (tensor): Position of the Dirac delta.
+        d (int): Dimensionality of the data.
     """
 
     def __init__(self, x, d):
         self.x = x
         self.d = d
 
     def __repr__(self):
-        return f"<Dirac:\n" + indented_kv("x", repr(self.x), suffix=">")
+        return "<Dirac:\n" + indented_kv("x", repr(self.x), suffix=">")
 
     def __str__(self):
-        return f"<Dirac:\n" + indented_kv("x", str(self.x), suffix=">")
+        return "<Dirac:\n" + indented_kv("x", str(self.x), suffix=">")
 
     @property
     def mean(self):
         return self.x
 
     @property
     def var(self):
-        return self._var(self.x)
+        return self._var()
 
-    @staticmethod
     @_dispatch
-    def _var(x: B.Numeric):
-        with B.on_device(x):
-            return B.zeros(x)
+    def _var(self: "Dirac[B.Numeric, B.Numeric]"):
+        with B.on_device(self.x):
+            return B.zeros(self.x)
 
-    @staticmethod
     @_dispatch
-    def _var(x: Aggregate):
-        return Aggregate(*(Dirac._var(xi) for xi in x))
-
-    def logpdf(self, x):
-        return self._logpdf(self.x, self.d)
+    def _var(self: "Dirac[Aggregate, Aggregate]"):
+        return Aggregate(*(Dirac(xi, di).var for xi, di in zip(self.x, self.d)))
 
-    @staticmethod
     @_dispatch
-    def _logpdf(x: B.Numeric, d: B.Int):
-        with B.on_device(x):
-            return B.zeros(B.dtype(x), *batch(x, d + 1))
+    def logpdf(self: "Dirac[B.Numeric, B.Int]", x):
+        with B.on_device(self.x):
+            return B.zeros(B.dtype(self.x), *batch(self.x, self.d + 1))
 
-    @staticmethod
     @_dispatch
-    def _logpdf(x: Aggregate, d: Aggregate):
+    def logpdf(self: "Dirac[Aggregate, Aggregate]", x):
         # Just take the first one. It doesn't matter.
-        return Dirac._logpdf(x[0], d[0])
-
-    @_dispatch
-    def sample(self, num=None):
-        return self._sample(self.x, num=num)
+        return Dirac(self.x[0], self.d[0]).logpdf(None)
 
     @_dispatch
-    def sample(self, state: B.RandomState, num=None):
-        return state, self.sample(num=num)
-
-    @staticmethod
-    @_dispatch
-    def _sample(x: B.Numeric, *, num):
+    def sample(
+        self: "Dirac[B.Numeric, B.Int]",
+        state: B.RandomState,
+        dtype: B.DType,
+        *shape,
+    ):
         # If no number of samples was specified, don't add a sample dimension.
-        if num is None:
-            return x
+        if shape == ():
+            return state, self.x
         else:
             # Don't tile. This way is more efficient.
-            return x[None, ...]
+            return state, B.expand_dims(self.x, axis=0, times=len(shape))
 
-    @staticmethod
     @_dispatch
-    def _sample(x: Aggregate, *, num):
-        return Aggregate(*(Dirac._sample(xi, num=num) for xi in x))
+    def sample(
+        self: "Dirac[Aggregate, Aggregate]",
+        state: B.RandomState,
+        dtype: B.DType,
+        *shape,
+    ):
+        samples = []
+        for xi, di in zip(self.x, self.d):
+            state, sample = Dirac(xi, di).sample(state, dtype, *shape)
+            samples.append(sample)
+        return state, Aggregate(*samples)
 
     @_dispatch
     def kl(self, other: "Dirac"):
         # Same result as `logpdf`, so just reuse that method.
         return self.logpdf(None)
+
+
+@B.dtype.dispatch
+def dtype(dist: Dirac):
+    return B.dtype(dist.x)
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/dist/dist.py` & `neuralprocesses-0.2.1/neuralprocesses/dist/dist.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,128 @@
 import abc
 
-__all__ = ["AbstractDistribution", "AbstractMultiOutputDistribution"]
+import lab as B
 
+from .. import _dispatch
 
-class AbstractDistribution(metaclass=abc.ABCMeta):
-    """An interface for distributions, mostly used for sampling in the data
-    generators."""
-
-    @abc.abstractmethod
-    def sample(self, state, dtype, *shape):
-        """Sample.
-
-        Args:
-            state (random state, optional): Random state.
-            dtype (dtype, optional): Data type.
-            *shape (int): Batch shape of the sample.
-
-        Returns:
-            random state, optional: Random state.
-            tensor: Sample of dtype `dtype` and shape `(*shape, *d)` where `d`
-                specifies the dimensionality of the sample.
-        """
+__all__ = ["AbstractDistribution", "AbstractMultiOutputDistribution", "shape_batch"]
 
 
-class AbstractMultiOutputDistribution(AbstractDistribution):
-    """An interface for multi-output distributions."""
+class AbstractDistribution(metaclass=abc.ABCMeta):
+    """An interface for distributions."""
 
     @abc.abstractmethod
     def __repr__(self):
         pass
 
     @abc.abstractmethod
     def __str__(self):
         pass
 
-    @abc.abstractmethod
-    def mean(self):
-        """tensor: Marginal means of shape `(*b, c, n)`."""
+    @_dispatch
+    def sample(self, state: B.RandomState, dtype: B.DType, *shape):
+        """Sample from the distribution.
 
-    @abc.abstractmethod
-    def var(self):
-        """tensor: Marginal variances of shape `(*b, c, n)`."""
+        Args:
+            state (random state, optional): Random state.
+            dtype (dtype, optional): Data type.
+            *shape (int): Batch shape of the sample.
+
+        Returns:
+            state (random state, optional): Random state.
+            tensor: Samples of shape `(*shape, *d)` where typically `d = (*b, c, n)`.
+        """
+        raise NotImplementedError(f"{self} cannot be sampled.")
+
+    @_dispatch
+    def sample(self, dtype: B.DType, *shape):
+        state = B.global_random_state(dtype)
+        state, sample = self.sample(state, dtype, *shape)
+        B.set_global_random_state(state)
+        return sample
+
+    @_dispatch
+    def sample(self, state: B.RandomState, *shape):
+        return self.sample(state, B.dtype(self), *shape)
+
+    @_dispatch
+    def sample(self, *shape):
+        return self.sample(B.dtype(self), *shape)
 
-    @abc.abstractmethod
     def logpdf(self, x):
         """Compute the log-pdf at inputs `x`.
 
         Args:
-            x (tensor): Inputs of shape `(*b, c, n)`.
+            x (tensor): Inputs of shape `(*b, *d)` where `b` is the batch shape and.
+                `d` the dimensionality of the random variable.
 
         Returns:
             tensor: Log-pdfs of shape `(*b,)`.
         """
+        raise NotImplementedError(f"Log-pdf of {self} cannot be computed.")
 
-    @abc.abstractmethod
-    def sample(self, state, num=None):
-        """Sample from the distribution.
-
-        Args:
-            state (random state, optional): Random state.
-            num (int, optional): Number of samples. Defaults to one.
+    @property
+    def mean(self):
+        """tensor: Mean."""
+        return self.m1
 
-        Returns:
-            state (random state, optional): Random state.
-            tensor: Samples of shape `(num, *b, c, n)` if `num > 1` and of shape .
-                `(*b, c, n)` otherwise.
-        """
+    @property
+    def var(self):
+        """tensor: Marginal variance."""
+        m1 = self.m1
+        return B.subtract(self.m2, B.multiply(m1, m1))
+
+    @property
+    def m1(self):
+        """tensor: First moment."""
+        return self.mean
+
+    @property
+    def m2(self):
+        """tensor: Second moment."""
+        mean = self.mean
+        return B.add(self.var, B.multiply(mean, mean))
 
     def kl(self, other):
         """Compute the KL-divergence with respect to another distribution.
 
         Args:
-            other (:class:`.AbstractMultiOutputDistribution`): Other.
+            other (:class:`.AbstractDistribution`): Other.
 
         Returns:
-            tensor: KL-divergences `kl(self, other)` of shape `(*b,)`.
+            tensor: KL-divergences `kl(self, other)`.
         """
         raise NotImplementedError(
             f"Cannot compute the KL-divergence between {self} and {other}."
         )
 
     def entropy(self):
         """Compute entropy.
 
         Returns:
-            tensor: Entropies of shape `(*b,)`.
+            tensor: Entropy.
         """
         raise NotImplementedError(f"Cannot compute the entropy of {self}.")
+
+
+# Support this for backwards compatibility.
+AbstractMultiOutputDistribution = AbstractDistribution
+
+
+@_dispatch
+def shape_batch(dist: AbstractDistribution):
+    """Determine the batch shape of a distribution.
+
+    Args:
+        dist (:class:`.AbstractDistribution`): Distribution.
+        *dims (int, optional): Dimensions to get.
+
+    Returns:
+        shape or int: Batch shape of the prediction of `dist`.
+    """
+    raise NotImplementedError(f"Cannot determine the batch shape of {dist}.")
+
+
+@_dispatch
+def shape_batch(dist, *dims: B.Int):
+    dist_shape_batch = shape_batch(dist)
+    return B.squeeze(tuple(dist_shape_batch[d] for d in dims))
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/dist/geom.py` & `neuralprocesses-0.2.1/neuralprocesses/dist/geom.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,7 +46,21 @@
         if self.upper > self.lower:
             lam = B.log(self.factor) / (self.factor_at - self.lower)
             lam = B.cast(dtype_float, B.to_active_device(lam))
             probs = B.exp(-lam * B.cast(dtype_float, realisations))
         else:
             probs = B.to_active_device(B.ones(dtype_float, 1))
         return B.choice(state, realisations, *shape, p=probs)
+
+    def __str__(self):
+        return (
+            f"TruncatedGeometric("
+            f"{self.lower}, {self.upper}, {self.factor}, {self.factor_at}"
+            f")"
+        )
+
+    def __repr__(self):
+        return (
+            f"TruncatedGeometric("
+            f"{self.lower!r}, {self.uppers!r}, {self.factor!r}, {self.factor_at!r}"
+            f")"
+        )
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/dist/normal.py` & `neuralprocesses-0.2.1/neuralprocesses/dist/normal.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from plum import parametric
 from stheno import Normal
 from wbml.util import indented_kv
 
 from .. import _dispatch
 from ..aggregate import Aggregate
 from ..util import batch, split
-from .dist import AbstractMultiOutputDistribution
+from .dist import AbstractDistribution, shape_batch
 
 __all__ = ["MultiOutputNormal"]
 
 
 @_dispatch
 def _map_sample_output(f, state_res: tuple):
     state, res = state_res
@@ -33,32 +33,32 @@
 
 @_dispatch
 def _monormal_vectorise(x: Aggregate, shape: Aggregate):
     return B.concat(*(_monormal_vectorise(xi, si) for xi, si in zip(x, shape)), axis=-2)
 
 
 @_dispatch
-def _monormal_unvectorise(x: B.Numeric, shape, *, squeeze_sample_dim=False):
-    x = B.reshape(x, *B.shape(x)[:-1], *shape)
+def _monormal_unvectorise(x: B.Numeric, data_shape, *, squeeze_sample_dim=False):
+    x = B.reshape(x, *B.shape(x)[:-1], *data_shape)
     if squeeze_sample_dim:
         x = B.squeeze(x, axis=0)
     return x
 
 
 @_dispatch
-def _monormal_unvectorise(x: B.Numeric, shape: Aggregate, **kw_args):
-    ns = [np.prod(si) for si in shape]
+def _monormal_unvectorise(x: B.Numeric, data_shape: Aggregate, **kw_args):
+    ns = [np.prod(si) for si in data_shape]
     xs = split(x, ns, -1)
     return Aggregate(
-        *(_monormal_unvectorise(xi, si, **kw_args) for xi, si in zip(xs, shape))
+        *(_monormal_unvectorise(xi, di, **kw_args) for xi, di in zip(xs, data_shape))
     )
 
 
 @parametric
-class MultiOutputNormal(AbstractMultiOutputDistribution):
+class MultiOutputNormal(AbstractDistribution):
     """A normal distribution for multiple outputs. Use one of the class methods to
     construct the object.
 
     Args:
         mean (matrix): Mean of the underlying vectorised multivariate normal.
         var (matrix): Variance of the underlying vectorised multivariate normal.
         noise (matrix): Noise of the underlying vectorised multivariate normal.
@@ -163,15 +163,15 @@
     @property
     def var(self):
         return _monormal_unvectorise(B.diag(self.vectorised_normal.var), self.shape)
 
     def logpdf(self, x):
         x = _monormal_vectorise(x, self.shape)
         d = self.vectorised_normal
-        if B.all(~B.isnan(x)):
+        if B.jit_to_numpy(B.all(~B.isnan(x))):
             return d.logpdf(x)
         else:
             # Data is missing. Unfortunately, which elements are missing can differ
             # between batches. The only thing we can now do is to loop over batches.
             # For now, we only support a single batch dimension.
             if B.rank(x) > 3:
                 raise NotImplementedError(
@@ -189,61 +189,55 @@
                     B.take(d_b.mean, mask, axis=-2),
                     B.submatrix(d_b.var, mask),
                 )
                 logpdfs.append(d_b.logpdf(x_b[mask, :]))
             return B.stack(*logpdfs, axis=-1)
 
     @_dispatch
-    def sample(self, state: B.RandomState, num: Union[B.Int, None] = None):
+    def sample(self, state: B.RandomState, dtype: B.DType, *shape: B.Int):
         def f(sample):
             # Put the sample dimension first.
             perm = list(range(B.rank(sample)))
             perm = perm[-1:] + perm[:-1]
             sample = B.transpose(sample, perm=perm)
             # Undo the vectorisation.
-            sample = _monormal_unvectorise(
+            return _monormal_unvectorise(
                 sample,
                 self.shape,
-                # Squeeze the sample dimension if no number of samples was specified.
-                squeeze_sample_dim=num is None,
+                # If `shape` is not specified, then the sample dimension of
+                # :class:`stheno.Normal` needs to be squeezed.
+                squeeze_sample_dim=shape == (),
             )
-            return sample
 
-        return _map_sample_output(f, self.vectorised_normal.sample(state, num or 1))
-
-    @_dispatch
-    def sample(self, num: Union[B.Int, None] = None):
-        state = B.global_random_state(B.dtype(self._mean, self._var, self._noise))
-        state, sample = self.sample(state, num)
-        B.set_global_random_state(state)
-        return sample
+        # TODO: Use `dtype` here. :class:`stheno.Normal` doesn't yet support `dtype`.
+        return _map_sample_output(f, self.vectorised_normal.sample(state, *shape))
 
     def kl(self, other: "MultiOutputNormal"):
         return self.vectorised_normal.kl(other.vectorised_normal)
 
     def entropy(self):
         return self.vectorised_normal.entropy()
 
 
 @B.dispatch
 def dtype(dist: MultiOutputNormal):
-    return B.dtype(dist.vectorised_normal)
+    return B.dtype(dist._mean, dist._var, dist._noise)
 
 
 @B.dispatch
 def cast(dtype: B.DType, dist: MultiOutputNormal):
     return MultiOutputNormal(
         B.cast(dtype, dist._mean),
         B.cast(dtype, dist._var),
         B.cast(dtype, dist._noise),
         dist.shape,
     )
 
 
-@B.dispatch
+@shape_batch.dispatch
 def shape_batch(dist: MultiOutputNormal):
     return B.shape_batch_broadcast(dist._mean, dist._var, dist._noise)
 
 
 @_dispatch
 def _possibly_densify_variance(var: AbstractMatrix):
     return var
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/dist/transformed.py` & `neuralprocesses-0.2.1/neuralprocesses/dist/transformed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from functools import partial
 
 import lab as B
 from wbml.util import indented_kv
 
-from .dist import AbstractMultiOutputDistribution
+from .dist import AbstractDistribution, shape_batch
 from .normal import _map_sample_output
 from .. import _dispatch
 from ..aggregate import Aggregate
 from ..util import register_module
 
 __all__ = ["Transform", "TransformedMultiOutputDistribution"]
 
@@ -153,15 +153,15 @@
             transform=transform,
             transform_deriv=transform_deriv,
             untransform=untransform,
             untransform_logdet=untransform_logdet,
         )
 
 
-class TransformedMultiOutputDistribution(AbstractMultiOutputDistribution):
+class TransformedMultiOutputDistribution(AbstractDistribution):
     """A transformed multi-output distribution.
 
     Args:
         dist (:class:`.AbstractMultiOutputDistribution`): Transformed distribution.
         transform (:class:`.Transform`): Transform.
 
     Attributes:
@@ -237,17 +237,17 @@
 
 
 @B.dispatch
 def cast(dtype: B.DType, dist: TransformedMultiOutputDistribution):
     return TransformedMultiOutputDistribution(B.cast(dtype, dist.dist), dist.transform)
 
 
-@B.dispatch
+@shape_batch.dispatch
 def shape_batch(dist: TransformedMultiOutputDistribution):
-    return B.shape_batch(dist.dist)
+    return shape_batch(dist.dist)
 
 
 @_dispatch
 def _map_aggregate(f, *xs):
     return f(*xs)
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/dist/uniform.py` & `neuralprocesses-0.2.1/neuralprocesses/dist/uniform.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,15 +29,22 @@
 
     @_dispatch
     def __init__(self, *bounds: Tuple[B.Number, B.Number]):
         lowers, uppers = zip(*bounds)
         self.lowers = B.stack(*lowers)
         self.uppers = B.stack(*uppers)
 
-    def sample(self, state, dtype, *shape):
+    def __str__(self):
+        return f"UniformContinuous({self.lower}, {self.upper})"
+
+    def __repr__(self):
+        return f"UniformContinuous({self.lower!r}, {self.uppers!r})"
+
+    @_dispatch
+    def sample(self, state: B.RandomState, dtype: B.DType, *shape):
         lowers = B.to_active_device(B.cast(dtype, self.lowers))
         uppers = B.to_active_device(B.cast(dtype, self.uppers))
         # Wrap everything in `Dimension`s to make dispatch work.
         shape = (Dimension(d) for d in shape)
         state, rand = B.rand(state, dtype, *shape, B.shape(lowers, 0))
         return state, lowers + (uppers - lowers) * rand
 
@@ -55,9 +62,16 @@
     """
 
     @_dispatch
     def __init__(self, lower: B.Int, upper: B.Int):
         self.lower = lower
         self.upper = upper
 
-    def sample(self, state, dtype, *shape):
+    @_dispatch
+    def sample(self, state: B.RandomState, dtype: B.DType, *shape):
         return B.randint(state, dtype, lower=self.lower, upper=self.upper + 1, *shape)
+
+    def __str__(self):
+        return f"UniformDiscrete({self.lower}, {self.upper})"
+
+    def __repr__(self):
+        return f"UniformDiscrete({self.lower!r}, {self.uppers!r})"
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/likelihood.py` & `neuralprocesses-0.2.1/neuralprocesses/likelihood.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import lab as B
 from lab.util import resolve_axis
 
 from . import _dispatch
 from .aggregate import AggregateInput, Aggregate
 from .datadims import data_dims
-from .dist import MultiOutputNormal, Dirac
+from .dist import MultiOutputNormal, Dirac, SpikesSlab, Beta
 from .parallel import Parallel
 from .util import register_module, split, split_dimension
 
 __all__ = [
     "DeterministicLikelihood",
     "HeterogeneousGaussianLikelihood",
     "LowRankGaussianLikelihood",
@@ -85,56 +85,54 @@
     def __init__(self, epsilon: float = 1e-6):
         self.epsilon = epsilon
 
     def __str__(self):
         return repr(self)
 
     def __repr__(self):
-        return "HeterogeneousGaussianLikelihood()"
+        return f"HeterogeneousGaussianLikelihood(epsilon={self.epsilon!r})"
 
 
 @_dispatch
 def code(
     coder: HeterogeneousGaussianLikelihood,
     xz,
     z,
     x,
     *,
     dtype_lik=None,
     **kw_args,
 ):
-    mean, noise, shape = _code_het(coder, xz, z)
+    mean, noise, shape = _het(coder, xz, z)
 
     # Cast parameters to the right data type.
     if dtype_lik:
         mean = B.cast(dtype_lik, mean)
         noise = B.cast(dtype_lik, noise)
     return xz, MultiOutputNormal.diagonal(mean, noise, shape)
 
 
 @_dispatch
-def _code_het(
+def _het(
     coder: HeterogeneousGaussianLikelihood,
     xz: AggregateInput,
     z: Aggregate,
 ):
-    means, noises, shapes = zip(
-        *[_code_het(coder, xzi, zi) for (xzi, _), zi in zip(xz, z)]
-    )
+    means, noises, shapes = zip(*[_het(coder, xzi, zi) for (xzi, _), zi in zip(xz, z)])
 
     # Concatenate into one big Gaussian.
     mean = B.concat(*means, axis=-1)
     noise = B.concat(*noises, axis=-1)
     shape = Aggregate(*shapes)
 
     return mean, noise, shape
 
 
 @_dispatch
-def _code_het(coder: HeterogeneousGaussianLikelihood, xz, z: B.Numeric):
+def _het(coder: HeterogeneousGaussianLikelihood, xz, z: B.Numeric):
     d = data_dims(xz)
     dim_y = B.shape(z, -d - 1) // 2
 
     z_mean, z_noise = split(z, (dim_y, dim_y), -d - 1)
 
     # Vectorise the data. Record the shape!
     z_mean, shape = _vectorise(z_mean, d + 1)
@@ -165,15 +163,17 @@
         self.rank = rank
         self.epsilon = epsilon
 
     def __str__(self):
         return repr(self)
 
     def __repr__(self):
-        return f"LowRankGaussianLikelihood(rank={self.rank})"
+        return (
+            f"LowRankGaussianLikelihood(rank={self.rank!r}, epsilon={self.epsilon!r})"
+        )
 
 
 @_dispatch
 def code(
     coder: LowRankGaussianLikelihood,
     xz,
     z,
@@ -256,15 +256,15 @@
     def __init__(self, epsilon: float = 1e-6):
         self.epsilon = epsilon
 
     def __str__(self):
         return repr(self)
 
     def __repr__(self):
-        return "DenseGaussianLikelihood()"
+        return r"DenseGaussianLikelihood(epsilon={self.epsilon!r})"
 
 
 @_dispatch
 def code(
     coder: DenseGaussianLikelihood,
     xz: Parallel,
     z: Parallel,
@@ -351,7 +351,103 @@
     d = data_dims(xz) // 2
 
     # First vectorise inner channels and then vectorise outer channels.
     z, _ = _vectorise(z, d + 1, offset=d + 1)
     z, _ = _vectorise(z, d + 1)
 
     return z
+
+
+@register_module
+class SpikesBetaLikelihood(AbstractLikelihood):
+    """Gaussian likelihood with heterogeneous noise.
+
+    Args:
+        epsilon (float, optional): Tolerance for equality checking. Defaults to `1e-6`.
+
+    Args:
+        epsilon (float): Tolerance for equality checking.
+    """
+
+    @_dispatch
+    def __init__(self, epsilon: float = 1e-6):
+        self.epsilon = epsilon
+
+    def __str__(self):
+        return repr(self)
+
+    def __repr__(self):
+        return f"SpikesBetaLikelihood(epsilon={self.epsilon!r})"
+
+
+@_dispatch
+def code(
+    coder: SpikesBetaLikelihood,
+    xz,
+    z,
+    x,
+    *,
+    dtype_lik=None,
+    **kw_args,
+):
+    alpha, beta, logp0, logp1, logps, d = _spikesbeta(coder, xz, z)
+
+    # Cast parameters to the right data type.
+    if dtype_lik:
+        alpha = B.cast(dtype_lik, alpha)
+        beta = B.cast(dtype_lik, beta)
+        logp0 = B.cast(dtype_lik, logp0)
+        logp1 = B.cast(dtype_lik, logp1)
+        logps = B.cast(dtype_lik, logps)
+
+    # Create the spikes vector.
+    with B.on_device(z):
+        dtype = dtype_lik or B.dtype(z)
+        spikes = B.stack(B.one(dtype), B.zero(dtype))
+
+    return xz, SpikesSlab(
+        spikes,
+        Beta(alpha, beta, d),
+        B.stack(logp0, logp1, logps, axis=-1),
+        d,
+        epsilon=coder.epsilon,
+    )
+
+
+@_dispatch
+def _spikesbeta(
+    coder: SpikesBetaLikelihood,
+    xz: AggregateInput,
+    z: Aggregate,
+):
+    alphas, betas, logp0s, logp1s, logpss, ds = zip(
+        *[_spikesbeta(coder, xzi, zi) for (xzi, _), zi in zip(xz, z)]
+    )
+
+    # Concatenate into one big distribution.
+    alpha = Aggregate(*alphas)
+    beta = Aggregate(*betas)
+    logp0 = Aggregate(*logp0s)
+    logp1 = Aggregate(*logp1s)
+    logps = Aggregate(*logpss)
+    d = Aggregate(*ds)
+
+    return alpha, beta, logp0, logp1, logps, d
+
+
+@_dispatch
+def _spikesbeta(coder: SpikesBetaLikelihood, xz, z: B.Numeric):
+    d = data_dims(xz)
+    dim_y = B.shape(z, -d - 1) // 5
+
+    z_alpha, z_beta, z_logp0, z_logp1, z_logps = split(
+        z, (dim_y, dim_y, dim_y, dim_y, dim_y), -d - 1
+    )
+
+    # Transform into parameters.
+    alpha = 1e-3 + B.softplus(z_alpha)
+    beta = 1e-3 + B.softplus(z_beta)
+    logp0 = z_logp0
+    logp1 = z_logp1
+    logps = z_logps
+
+    return alpha, beta, logp0, logp1, logps, d + 1
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/mask.py` & `neuralprocesses-0.2.1/neuralprocesses/mask.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 __all__ = ["Masked", "mask_context", "merge_contexts"]
 
 
 class Masked:
     """A masked output.
 
     Args:
-        y (tensor): Output to mask.
+        y (tensor): Output to mask. The masked values can have any non-NaN value, but
+            they cannot be NaN!
         mask (tensor): A mask consisting of zeros and ones and just one channel.
 
     Attributes:
         y (tensor): Masked output.
         mask (tensor): A mask consisting of zeros and ones and just one channel.
     """
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/materialise.py` & `neuralprocesses-0.2.1/neuralprocesses/materialise.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/model/ar.py` & `neuralprocesses-0.2.1/neuralprocesses/model/ar.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/model/elbo.py` & `neuralprocesses-0.2.1/neuralprocesses/model/elbo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import lab as B
 import numpy as np
 
-from .model import Model
-from .util import sample, fix_noise as fix_noise_in_pred, compress_contexts
 from .. import _dispatch
 from ..aggregate import Aggregate, AggregateInput
 from ..coding import code, code_track, recode_stochastic
-from ..dist import AbstractMultiOutputDistribution
+from ..dist import AbstractDistribution
 from ..numdata import num_data
 from ..parallel import Parallel
+from .model import Model
+from .util import compress_contexts
+from .util import fix_noise as fix_noise_in_pred
+from .util import sample
 
 __all__ = ["elbo"]
 
 
 @_dispatch
 def elbo(
     state: B.RandomState,
@@ -74,15 +76,16 @@
         h,
         root=True,
         dtype_lik=float64,
         **kw_args,
     )
 
     # Sample from posterior.
-    state, z = sample(state, qz, num=num_samples)
+    shape = () if num_samples is None else (num_samples,)
+    state, z = sample(state, qz, *shape)
     z = B.cast(float, z)
 
     # Run sample through decoder.
     _, d = code(
         model.decoder,
         xz,
         z,
@@ -113,15 +116,15 @@
     state = B.global_random_state(B.dtype(args[-1]))
     state, elbos = elbo(state, model, *args, **kw_args)
     B.set_global_random_state(state)
     return elbos
 
 
 @_dispatch
-def _kl(q: AbstractMultiOutputDistribution, p: AbstractMultiOutputDistribution):
+def _kl(q: AbstractDistribution, p: AbstractDistribution):
     return q.kl(p)
 
 
 @_dispatch
 def _kl(q: Parallel, p: Parallel):
     return sum([_kl(qi, pi) for qi, pi in zip(q, p)])
 
@@ -153,15 +156,15 @@
         xti = B.concat(xci, xti, axis=-1)
         yti = B.concat(yci, yti, axis=-1)
 
         # At this point, `(xti, yti)` contains all data for output `i`. Hence, make this
         # the context set for output `i` for the approximate posterior.
         if q_context_updates[i] is not None:
             raise ValueError(
-                f"Aggregate target inputs specified the same output multiple times."
+                "Aggregate target inputs specified the same output multiple times."
             )
         q_context_updates[i] = (xti, yti)
 
         updated_xt.append((xti, i))
         updated_yt.append(yti)
 
     # Update the target inputs.
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/model/loglik.py` & `neuralprocesses-0.2.1/neuralprocesses/model/loglik.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/model/model.py` & `neuralprocesses-0.2.1/neuralprocesses/model/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
         # decoder.
         enc_kw_args = dict(kw_args)
         if "noiseless" in enc_kw_args:
             del enc_kw_args["noiseless"]
         xz, pz = code(self.encoder, xc, yc, xt, root=True, **enc_kw_args)
 
         # Sample and convert sample to the right data type.
-        state, z = sample(state, pz, num=num_samples)
+        shape = () if num_samples is None else (num_samples,)
+        state, z = sample(state, pz, *shape)
         if dtype_enc_sample:
             z = B.cast(dtype_enc_sample, z)
 
         _, d = code(self.decoder, xz, z, xt, root=True, **kw_args)
 
         return state, d
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/model/predict.py` & `neuralprocesses-0.2.1/neuralprocesses/model/predict.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import lab as B
 import numpy as np
 
-from .model import Model
 from .. import _dispatch
+from ..aggregate import Aggregate
+from ..dist import shape_batch
+from .model import Model
 
 __all__ = ["predict"]
 
 
 @_dispatch
 def predict(
     state: B.RandomState,
@@ -56,17 +58,21 @@
             dtype_lik=float64,
             num_samples=this_num_samples,
         )
 
         # If the number of samples is equal to one but `num_samples > 1`, then the
         # encoding was a `Dirac`, so we can stop batching. In this case, we can
         # efficiently compute everything that we need and exit.
-        if this_num_samples > 1 and B.shape_batch(pred, 0) == 1:
+        if this_num_samples > 1 and shape_batch(pred, 0) == 1:
             state, ft = pred.noiseless.sample(state, num_samples)
             state, yt = pred.sample(state, num_samples)
+            # If `pred` or `pred.noiseless` were `Dirac`s, then `ft` or `yt` might not
+            # have the right number of samples.
+            ft = _possibly_tile(ft, num_samples)
+            yt = _possibly_tile(yt, num_samples)
             return (
                 state,
                 # Squeeze the newly introduced sample dimension.
                 B.squeeze(pred.mean, axis=0),
                 B.squeeze(pred.var, axis=0),
                 # Squeeze the previously introduced sample dimension.
                 B.squeeze(ft, axis=1),
@@ -105,7 +111,20 @@
 @_dispatch
 def predict(model: Model, *args, **kw_args):
     state = B.global_random_state(B.dtype(args[-1]))
     res = predict(state, model, *args, **kw_args)
     state, res = res[0], res[1:]
     B.set_global_random_state(state)
     return res
+
+
+@_dispatch
+def _possibly_tile(x: B.Numeric, n: B.Int):
+    if B.shape(x, 0) == 1 and n > 1:
+        return B.tile(x, n, *((1,) * (B.rank(x) - 1)))
+    else:
+        return x
+
+
+@_dispatch
+def _possibly_tile(x: Aggregate, n: B.Int):
+    return Aggregate(*(_possibly_tile(xi, n) for xi in x))
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/model/util.py` & `neuralprocesses-0.2.1/neuralprocesses/model/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,63 @@
-from typing import Union
-
 import lab as B
 from matrix import Diagonal
 
 from .. import _dispatch
 from ..aggregate import Aggregate, AggregateInput
 from ..dist import (
-    AbstractMultiOutputDistribution,
+    AbstractDistribution,
     MultiOutputNormal,
+    SpikesSlab,
     TransformedMultiOutputDistribution,
 )
 from ..parallel import Parallel
 
 __all__ = ["sample", "fix_noise", "compress_contexts", "tile_for_sampling"]
 
 
 @_dispatch
 def sample(
     state: B.RandomState,
-    x: AbstractMultiOutputDistribution,
-    num: Union[B.Int, None] = None,
+    x: AbstractDistribution,
+    *shape: B.Int,
 ):
-    """Sample an encoding:
+    """Sample an encoding.
 
     Args:
         state (random state): Random state.
         x (object): Encoding.
-        num (int, optional): Number of samples.
+        *shape (int): Batch shape of the sample.
 
     Returns:
         random state: Random state.
         object: Sample.
     """
-    return x.sample(state, num=num)
+    return x.sample(state, *shape)
 
 
 @_dispatch
-def sample(state: B.RandomState, x: Parallel, num: Union[B.Int, None] = None):
+def sample(state: B.RandomState, x: Parallel, *shape: B.Int):
     samples = []
     for xi in x:
-        state, s = sample(state, xi, num=num)
+        state, s = sample(state, xi, *shape)
         samples.append(s)
     return state, Parallel(*samples)
 
 
 @_dispatch
 def fix_noise(d, value: None):
     """Fix the noise of a prediction.
 
     Args:
-        d (:class:`neuralprocesses.dist.dist.AbstractMultiOutputDistribution`):
+        d (:class:`neuralprocesses.dist.dist.AbstractDistribution`):
             Prediction.
         value (float or None): Value to fix it to.
 
     Returns:
-        :class:`neuralprocesses.dist.dist.AbstractMultiOutputDistribution`: Prediction
+        :class:`neuralprocesses.dist.dist.AbstractDistribution`: Prediction
             with noise fixed.
     """
     return d
 
 
 @_dispatch
 def fix_noise(d: MultiOutputNormal, value: float):
@@ -76,14 +75,19 @@
     return TransformedMultiOutputDistribution(
         fix_noise(d.dist, value),
         d.transform,
     )
 
 
 @_dispatch
+def fix_noise(d: SpikesSlab, value: float):
+    return d
+
+
+@_dispatch
 def compress_contexts(contexts: list):
     """Compress multiple context sets into a single `(x, y)` pair.
 
     Args:
         contexts (list): Context sets.
 
     Returns:
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/numdata.py` & `neuralprocesses-0.2.1/neuralprocesses/numdata.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/parallel.py` & `neuralprocesses-0.2.1/neuralprocesses/parallel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import lab as B
 from matrix.util import indent
 
 from . import _dispatch
-from .util import register_module, is_framework_module
+from .util import is_framework_module, register_module
 
-__all__ = ["Parallel", "broadcast_coder_over_parallel"]
+__all__ = [
+    "Parallel",
+    "broadcast_coder_over_parallel",
+]
 
 
 @register_module
 class Parallel:
     """A parallel of elements.
 
     Args:
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses/tensorflow/__init__.py` & `neuralprocesses-0.2.1/neuralprocesses/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/tensorflow/nn.py` & `neuralprocesses-0.2.1/neuralprocesses/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/torch/__init__.py` & `neuralprocesses-0.2.1/neuralprocesses/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/torch/nn.py` & `neuralprocesses-0.2.1/neuralprocesses/torch/nn.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses/util.py` & `neuralprocesses-0.2.1/neuralprocesses/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/neuralprocesses.egg-info/PKG-INFO` & `neuralprocesses-0.2.1/neuralprocesses.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuralprocesses
-Version: 0.2.0
+Version: 0.2.1
 Summary: A framework for composing Neural Processes in Python
 Home-page: https://github.com/wesselb/neuralprocesses
 Author: Wessel Bruinsma
 Author-email: wessel.p.bruinsma@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `neuralprocesses-0.2.0/neuralprocesses.egg-info/SOURCES.txt` & `neuralprocesses-0.2.1/neuralprocesses.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -79,29 +79,32 @@
 neuralprocesses/coders/setconv/__init__.py
 neuralprocesses/coders/setconv/density.py
 neuralprocesses/coders/setconv/identity.py
 neuralprocesses/coders/setconv/setconv.py
 neuralprocesses/data/__init__.py
 neuralprocesses/data/antarctica.py
 neuralprocesses/data/batch.py
+neuralprocesses/data/bimodal.py
 neuralprocesses/data/data.py
 neuralprocesses/data/eeg.py
 neuralprocesses/data/gp.py
 neuralprocesses/data/mixgp.py
 neuralprocesses/data/mixture.py
 neuralprocesses/data/predefined.py
 neuralprocesses/data/predprey.py
 neuralprocesses/data/sawtooth.py
 neuralprocesses/data/temperature.py
 neuralprocesses/data/util.py
 neuralprocesses/dist/__init__.py
+neuralprocesses/dist/beta.py
 neuralprocesses/dist/dirac.py
 neuralprocesses/dist/dist.py
 neuralprocesses/dist/geom.py
 neuralprocesses/dist/normal.py
+neuralprocesses/dist/spikeslab.py
 neuralprocesses/dist/transformed.py
 neuralprocesses/dist/uniform.py
 neuralprocesses/model/__init__.py
 neuralprocesses/model/ar.py
 neuralprocesses/model/elbo.py
 neuralprocesses/model/loglik.py
 neuralprocesses/model/model.py
```

### Comparing `neuralprocesses-0.2.0/schedule.py` & `neuralprocesses-0.2.1/schedule.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/scripts/predprey.py` & `neuralprocesses-0.2.1/scripts/predprey.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/scripts/predprey_visualise.py` & `neuralprocesses-0.2.1/scripts/predprey_visualise.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/scripts/sawtooth_sample_ar.py` & `neuralprocesses-0.2.1/scripts/sawtooth_sample_ar.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/scripts/synthetic_extra.py` & `neuralprocesses-0.2.1/scripts/synthetic_extra.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/scripts/synthetic_parse.py` & `neuralprocesses-0.2.1/scripts/synthetic_parse.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/scripts/temperature_mae.py` & `neuralprocesses-0.2.1/scripts/temperature_mae.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/scripts/temperature_summarise_folds.py` & `neuralprocesses-0.2.1/scripts/temperature_summarise_folds.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/scripts/temperature_visualise.py` & `neuralprocesses-0.2.1/scripts/temperature_visualise.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tables.ipynb` & `neuralprocesses-0.2.1/tables.ipynb`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/coders/test_shaping.py` & `neuralprocesses-0.2.1/tests/coders/test_shaping.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/dists/test_normal.py` & `neuralprocesses-0.2.1/tests/dists/test_normal.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/gnp/autoencoding.py` & `neuralprocesses-0.2.1/tests/gnp/autoencoding.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/gnp/gnp.py` & `neuralprocesses-0.2.1/tests/gnp/gnp.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/gnp/util.py` & `neuralprocesses-0.2.1/tests/gnp/util.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/test_architectures.py` & `neuralprocesses-0.2.1/tests/test_architectures.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from itertools import product
 
 import lab as B
 import numpy as np
 import pytest
+from neuralprocesses.aggregate import Aggregate, AggregateInput
+from neuralprocesses.parallel import Parallel
 from plum import isinstance
 
 from .util import approx, generate_data
 from .util import nps as nps_fixed_dtype  # noqa
 
 
 def generate_conv_arch_variations(configs):
@@ -59,71 +61,71 @@
             "dim_embedding": 4,
             "width": 4,
             "num_basis_functions": 4,
             "dim_lv": 0,
         },
         dim_x=[1, 2],
         dim_y=[1, 2],
-        likelihood=["het", "lowrank"],
+        likelihood=["het", "lowrank", "spikes-beta"],
     )
     # NP:
     + product_kw_args(
         {
             "constructor": "construct_gnp",
             "dim_embedding": 4,
             "width": 4,
             "num_basis_functions": 4,
             "dim_lv": 3,
         },
         dim_x=[1, 2],
         dim_y=[1, 2],
-        likelihood=["het", "lowrank"],
+        likelihood=["het", "lowrank", "spikes-beta"],
         lv_likelihood=["het", "dense"],
     )
     # ACNP:
     + product_kw_args(
         {
             "constructor": "construct_agnp",
             "dim_embedding": 4,
             "num_heads": 2,
             "width": 4,
             "num_basis_functions": 4,
             "dim_lv": 0,
         },
         dim_x=[1, 2],
         dim_y=[1, 2],
-        likelihood=["het", "lowrank"],
+        likelihood=["het", "lowrank", "spikes-beta"],
     )
     # ANP:
     + product_kw_args(
         {
             "constructor": "construct_agnp",
             "dim_embedding": 4,
             "num_heads": 2,
             "width": 4,
             "num_basis_functions": 4,
             "dim_lv": 3,
         },
         dim_x=[1, 2],
         dim_y=[1, 2],
-        likelihood=["het", "lowrank"],
+        likelihood=["het", "lowrank", "spikes-beta"],
         lv_likelihood=["het", "dense"],
     )
     # ConvCNP and ConvGNP:
     + generate_conv_arch_variations(
         product_kw_args(
             {
                 "constructor": "construct_convgnp",
                 "num_basis_functions": 4,
                 "points_per_unit": 8,
                 "dim_lv": 0,
             },
             dim_x=[1, 2],
             dim_y=[1, 2],
-            likelihood=["het", "lowrank"],
+            likelihood=["het", "lowrank", "spikes-beta"],
             encoder_scales_learnable=[True, False],
             decoder_scale_learnable=[True, False],
         )
     )
     # ConvNP:
     + generate_conv_arch_variations(
         product_kw_args(
@@ -131,15 +133,15 @@
                 "constructor": "construct_convgnp",
                 "num_basis_functions": 4,
                 "points_per_unit": 8,
                 "dim_lv": 3,
             },
             dim_x=[1, 2],
             dim_y=[1, 2],
-            likelihood=["het", "lowrank"],
+            likelihood=["het", "lowrank", "spikes-beta"],
             lv_likelihood=["het", "lowrank"],
         )
     )
     # FullConvGNP:
     + generate_conv_arch_variations(
         product_kw_args(
             {
@@ -211,91 +213,126 @@
                 p.data = p.data + 1e-2 * B.randn(p)
             return model
 
     else:
         raise RuntimeError("I don't know how to resample the parameters of the model.")
 
     def sample():
-        return generate_data(nps, dim_x=config["dim_x"], dim_y=config["dim_y"])
+        if "likelihood" in config:
+            binary = config["likelihood"] == "spikes-beta"
+        else:
+            binary = False
+        return generate_data(
+            nps,
+            dim_x=config["dim_x"],
+            dim_y=config["dim_y"],
+            binary=binary,
+        )
 
     return construct_model, sample
 
 
+def shape(x, extra=()):
+    if isinstance(x, Aggregate):
+        return tuple(extra + B.shape(xi) for xi in x)
+    else:
+        return extra + B.shape(x)
+
+
 def check_prediction(nps, pred, yt):
     # Ensure that there is sufficient noise.
     try:
         pred._noise = pred._noise + 1e-2 * B.eye(pred._noise)
     except AttributeError:
         pass
 
     # Check that the log-pdf at the target data is finite and of the right data type.
     objective = pred.logpdf(yt)
     assert B.rank(objective) == 1
     assert np.isfinite(B.to_numpy(B.sum(objective)))
     assert B.dtype(objective) == nps.dtype
 
-    if not isinstance(yt, nps.Aggregate):
-        # Check mean, variance, and samples.
-        assert B.shape(pred.mean) == B.shape(yt)
-        assert B.shape(pred.var) == B.shape(yt)
-        assert B.shape(pred.sample()) == B.shape(yt)
-        assert B.shape(pred.sample(1)) == (1,) + B.shape(yt)
-        assert B.shape(pred.sample(2)) == (2,) + B.shape(yt)
+    # Check mean, variance, and samples.
+    assert shape(pred.mean) == shape(yt)
+    assert shape(pred.var) == shape(yt)
+    assert shape(pred.sample()) == shape(yt)
+    assert shape(pred.sample(1)) == shape(yt, (1,))
+    assert shape(pred.sample(2)) == shape(yt, (2,))
+
 
+def _aggregate_xt_yt(xt, yt):
+    xt = AggregateInput(*((xt, i) for i in range(B.shape(yt, 1))))
+    yt = Aggregate(*(yt[:, i : i + 1, :] for i in range(B.shape(yt, 1))))
+    return xt, yt
 
+
+@pytest.mark.parametrize("aggregate", [False, True])
 @pytest.mark.flaky(reruns=3)
-def test_forward(nps, model_sample):
+def test_forward(nps, model_sample, aggregate):
     model, sample = model_sample
     model = model()
     xc, yc, xt, yt = sample()
+    if aggregate:
+        xt, yt = _aggregate_xt_yt(xt, yt)
     pred = model(xc, yc, xt, batch_size=2, unused_arg=None)
     check_prediction(nps, pred, yt)
 
 
 @pytest.mark.parametrize("normalise", [False, True])
 @pytest.mark.flaky(reruns=3)
 def test_elbo(nps, model_sample, normalise):
+    """Test the ELBO.
+
+    We don't test aggregates here, because `nps.elbo` assumes a particular structure of
+    the context sets in that case.
+    """
     model, sample = model_sample
     model = model()
     xc, yc, xt, yt = sample()
     elbos = nps.elbo(model, xc, yc, xt, yt, num_samples=2, normalise=normalise)
     assert B.rank(elbos) == 1
     assert np.isfinite(B.to_numpy(B.sum(elbos)))
     assert B.dtype(elbos) == nps.dtype64
 
 
+@pytest.mark.parametrize("aggregate", [False, True])
 @pytest.mark.parametrize("normalise", [False, True])
 @pytest.mark.flaky(reruns=3)
-def test_loglik(nps, model_sample, normalise):
+def test_loglik(nps, model_sample, normalise, aggregate):
     model, sample = model_sample
     model = model()
     xc, yc, xt, yt = sample()
+    if aggregate:
+        xt, yt = _aggregate_xt_yt(xt, yt)
     logpdfs = nps.loglik(model, xc, yc, xt, yt, num_samples=2, normalise=normalise)
     assert B.rank(logpdfs) == 1
     assert np.isfinite(B.to_numpy(B.sum(logpdfs)))
     assert B.dtype(logpdfs) == nps.dtype64
 
 
+@pytest.mark.parametrize("aggregate", [False, True])
 @pytest.mark.flaky(reruns=3)
-def test_predict(nps, model_sample):
+def test_predict(nps, model_sample, aggregate):
     model, sample = model_sample
     model = model()
     xc, yc, xt, yt = sample()
+    if aggregate:
+        xt, yt = _aggregate_xt_yt(xt, yt)
     mean, var, samples, noisy_samples = nps.predict(
         model,
         xc,
         yc,
         xt,
         num_samples=3,
         batch_size=2,
     )
-    assert B.shape(mean) == B.shape(yt)
-    assert B.shape(var) == B.shape(yt)
-    assert B.shape(samples) == (3,) + B.shape(yt)
-    assert B.shape(noisy_samples) == (3,) + B.shape(yt)
+    assert shape(mean) == shape(yt)
+    assert shape(var) == shape(yt)
+    assert shape(samples) == shape(yt, (3,))
+    assert shape(noisy_samples) == shape(yt, (3,))
 
 
 @pytest.mark.flaky(reruns=3)
 def test_batching(nps, model_sample):
     model, sample = model_sample
     model = model()
     xc, yc, xt, yt = sample()
@@ -380,7 +417,46 @@
         dim_lv=dim_lv,
         dtype=nps.dtype,
         **config,
     )
     batch = gen.generate_batch()
     pred = model(batch["contexts"], batch["xt"])
     check_prediction(nps, pred, batch["yt"])
+
+
+@pytest.mark.parametrize(
+    "constructor_kw_args",
+    [
+        ("construct_gnp", {}),
+        ("construct_agnp", {}),
+        ("construct_convgnp", {"points_per_unit": 4}),
+        ("construct_fullconvgnp", {"points_per_unit": 4}),
+    ],
+)
+def test_context_verification(nps, constructor_kw_args):
+    constructor, kw_args = constructor_kw_args
+
+    c = (B.randn(nps.dtype, 4, 1, 5), B.randn(nps.dtype, 4, 1, 5))
+    xt = B.randn(nps.dtype, 4, 1, 15)
+
+    # Test one context set.
+    model = getattr(nps, constructor)(dim_yc=1, dtype=nps.dtype, **kw_args)
+    pred1 = model(*c, xt)
+    pred2 = model([c], xt)
+    approx(pred1.mean, pred2.mean)
+    with pytest.raises(AssertionError, match="(?i)got inputs and outputs in parallel"):
+        model([c, c], xt)
+    with pytest.raises(AssertionError, match="(?i) got inputs in parallel"):
+        model(Parallel(c[0], c[0]), c[1], xt)
+    with pytest.raises(AssertionError, match="(?i) got outputs in parallel"):
+        model(c[0], Parallel(c[1], c[1]), xt)
+
+    # Test two context sets.
+    model = getattr(nps, constructor)(dim_yc=(1, 1), dtype=nps.dtype, **kw_args)
+    model([c, c], xt)
+    with pytest.raises(AssertionError, match="(?i)expected a parallel of elements"):
+        model([c], xt)
+    with pytest.raises(
+        AssertionError,
+        match="(?i)expected a parallel of 2 elements, but got 4 inputs and 4 outputs",
+    ):
+        model([c, c, c, c], xt)
```

### Comparing `neuralprocesses-0.2.0/tests/test_data.py` & `neuralprocesses-0.2.1/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/test_discretisation.py` & `neuralprocesses-0.2.1/tests/test_discretisation.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/test_distribution.py` & `neuralprocesses-0.2.1/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/test_mask.py` & `neuralprocesses-0.2.1/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/test_model.py` & `neuralprocesses-0.2.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/test_unet.py` & `neuralprocesses-0.2.1/tests/test_unet.py`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/tests/util.py` & `neuralprocesses-0.2.1/tests/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,19 +51,30 @@
 
 
 @pytest.fixture(params=[nps_torch, nps_tf], scope="module")
 def nps(request):
     return request.param
 
 
-def generate_data(nps, batch_size=4, dim_x=1, dim_y=1, n_context=5, n_target=7):
+def generate_data(
+    nps,
+    batch_size=4,
+    dim_x=1,
+    dim_y=1,
+    n_context=5,
+    n_target=7,
+    binary=False,
+):
     xc = B.randn(nps.dtype, batch_size, dim_x, n_context)
     yc = B.randn(nps.dtype, batch_size, dim_y, n_context)
     xt = B.randn(nps.dtype, batch_size, dim_x, n_target)
     yt = B.randn(nps.dtype, batch_size, dim_y, n_target)
+    if binary:
+        yc = B.cast(nps.dtype, yc >= 0)
+        yt = B.cast(nps.dtype, yt >= 0)
     return xc, yc, xt, yt
 
 
 if socket.gethostname().lower().startswith("wessel"):
     remote_xfail = lambda f: f  #: `xfail` only on CI.
     remote_skip = lambda f: f  #: `skip` only on CI.
 else:
```

### Comparing `neuralprocesses-0.2.0/todo.tasks` & `neuralprocesses-0.2.1/todo.tasks`

 * *Files identical despite different names*

### Comparing `neuralprocesses-0.2.0/train.py` & `neuralprocesses-0.2.1/train.py`

 * *Files identical despite different names*

