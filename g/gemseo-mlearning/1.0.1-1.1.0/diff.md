# Comparing `tmp/gemseo-mlearning-1.0.1.tar.gz` & `tmp/gemseo-mlearning-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gemseo-mlearning-1.0.1.tar", last modified: Thu Feb 16 09:20:03 2023, max compression
+gzip compressed data, was "gemseo-mlearning-1.1.0.tar", last modified: Sun Jun  4 18:33:39 2023, max compression
```

## Comparing `gemseo-mlearning-1.0.1.tar` & `gemseo-mlearning-1.1.0.tar`

### file list

```diff
@@ -1,135 +1,156 @@
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.295199 gemseo-mlearning-1.0.1/
--rw-r--r--   0 ad        (1000) ad        (1000)      450 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/.gitattributes
--rw-r--r--   0 ad        (1000) ad        (1000)      195 2022-07-25 05:50:08.000000 gemseo-mlearning-1.0.1/.gitignore
--rw-r--r--   0 ad        (1000) ad        (1000)       70 2023-02-16 09:19:46.000000 gemseo-mlearning-1.0.1/.gitlab-ci.yml
--rw-r--r--   0 ad        (1000) ad        (1000)     2491 2023-02-15 19:11:57.000000 gemseo-mlearning-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 ad        (1000) ad        (1000)     9105 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/.pylintrc
--rw-r--r--   0 ad        (1000) ad        (1000)     1131 2023-02-16 09:19:46.000000 gemseo-mlearning-1.0.1/CHANGELOG.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     1788 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/CREDITS.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-mlearning-1.0.1/LICENSE.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.278200 gemseo-mlearning-1.0.1/LICENSES/
--rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-mlearning-1.0.1/LICENSES/LGPLv3.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.279200 gemseo-mlearning-1.0.1/LICENSES/headers/
--rw-r--r--   0 ad        (1000) ad        (1000)      729 2022-03-24 13:18:51.000000 gemseo-mlearning-1.0.1/LICENSES/headers/BSD-0-Clause.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      334 2022-03-24 13:18:51.000000 gemseo-mlearning-1.0.1/LICENSES/headers/CC-BY-SA-4.0.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      710 2022-03-24 13:18:51.000000 gemseo-mlearning-1.0.1/LICENSES/headers/LGPL-3.0.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2506 2023-02-16 09:20:03.295199 gemseo-mlearning-1.0.1/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     1390 2022-07-27 19:22:29.000000 gemseo-mlearning-1.0.1/README.rst
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.272199 gemseo-mlearning-1.0.1/doc_src/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.272199 gemseo-mlearning-1.0.1/doc_src/examples/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.279200 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/
--rw-r--r--   0 ad        (1000) ad        (1000)      749 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/README.rst
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.281200 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/
--rw-r--r--   0 ad        (1000) ad        (1000)      751 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/README.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     5297 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_boot.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5336 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_cv.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5321 2023-02-15 19:13:59.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_cv_boot.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5163 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_krig.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5929 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_rosenbrock.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5865 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_limit_state.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.281200 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/api/
--rw-r--r--   0 ad        (1000) ad        (1000)      759 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/api/README.rst
--rw-r--r--   0 ad        (1000) ad        (1000)     2178 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/api/plot_sample_discipline.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2403 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/doc_src/examples/mlearning/api/plot_sample_disciplines.py
--rw-r--r--   0 ad        (1000) ad        (1000)      611 2022-07-08 14:05:19.000000 gemseo-mlearning-1.0.1/pyproject.toml
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.283200 gemseo-mlearning-1.0.1/requirements/
--rw-r--r--   0 ad        (1000) ad        (1000)       79 2022-05-04 19:46:48.000000 gemseo-mlearning-1.0.1/requirements/check.in
--rw-r--r--   0 ad        (1000) ad        (1000)      596 2023-02-15 19:13:59.000000 gemseo-mlearning-1.0.1/requirements/check.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       12 2022-05-04 19:46:48.000000 gemseo-mlearning-1.0.1/requirements/dist.in
--rw-r--r--   0 ad        (1000) ad        (1000)     1495 2023-02-16 09:19:46.000000 gemseo-mlearning-1.0.1/requirements/dist.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2277 2023-02-09 17:58:14.000000 gemseo-mlearning-1.0.1/requirements/doc.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2950 2023-02-16 09:19:46.000000 gemseo-mlearning-1.0.1/requirements/test-python3.10.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     3107 2023-02-16 09:19:46.000000 gemseo-mlearning-1.0.1/requirements/test-python3.7.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2948 2023-02-16 09:19:46.000000 gemseo-mlearning-1.0.1/requirements/test-python3.8.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     2948 2023-02-16 09:19:46.000000 gemseo-mlearning-1.0.1/requirements/test-python3.9.txt
--rw-r--r--   0 ad        (1000) ad        (1000)     1634 2023-02-16 09:20:03.296200 gemseo-mlearning-1.0.1/setup.cfg
--rw-r--r--   0 ad        (1000) ad        (1000)      839 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/setup.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.273200 gemseo-mlearning-1.0.1/src/
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.283200 gemseo-mlearning-1.0.1/src/gemseo_mlearning/
--rw-r--r--   0 ad        (1000) ad        (1000)      841 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.285199 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/
--rw-r--r--   0 ad        (1000) ad        (1000)      832 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     7717 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/acquisition.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.285199 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/
--rw-r--r--   0 ad        (1000) ad        (1000)      802 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.285199 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/distances/
--rw-r--r--   0 ad        (1000) ad        (1000)      855 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/distances/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2107 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/distances/criterion_min.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.286200 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/expectation/
--rw-r--r--   0 ad        (1000) ad        (1000)      844 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/expectation/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1737 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/expectation/criterion.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.286200 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/mean_std/
--rw-r--r--   0 ad        (1000) ad        (1000)      858 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/mean_std/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2531 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/mean_std/criterion.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.287200 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/optimum/
--rw-r--r--   0 ad        (1000) ad        (1000)      848 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/optimum/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1544 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/optimum/criterion.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2115 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/optimum/criterion_max.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2118 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/optimum/criterion_min.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.287200 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/quantile/
--rw-r--r--   0 ad        (1000) ad        (1000)      837 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/quantile/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1861 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/quantile/criterion.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.287200 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/standard_deviation/
--rw-r--r--   0 ad        (1000) ad        (1000)      851 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/standard_deviation/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1908 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/standard_deviation/criterion.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.288200 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/value/
--rw-r--r--   0 ad        (1000) ad        (1000)      838 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/value/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2381 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/value/criterion.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.288200 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/variance/
--rw-r--r--   0 ad        (1000) ad        (1000)      841 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/variance/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1862 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/variance/criterion.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5673 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criterion.py
--rw-r--r--   0 ad        (1000) ad        (1000)     9098 2023-02-15 20:00:56.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/distribution.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.289199 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/distributions/
--rw-r--r--   0 ad        (1000) ad        (1000)      826 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/distributions/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     4140 2023-02-15 20:00:56.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/distributions/kriging_distribution.py
--rw-r--r--   0 ad        (1000) ad        (1000)    11791 2023-02-15 20:00:56.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/distributions/regressor_distribution.py
--rw-r--r--   0 ad        (1000) ad        (1000)     4088 2023-02-15 19:24:27.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/api.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.289199 gemseo-mlearning-1.0.1/src/gemseo_mlearning/quality_measures/
--rw-r--r--   0 ad        (1000) ad        (1000)      840 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/quality_measures/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2091 2022-07-25 05:49:24.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/quality_measures/mae_measure.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2016 2023-02-15 19:13:59.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/quality_measures/me_measure.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.290200 gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/
--rw-r--r--   0 ad        (1000) ad        (1000)      799 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3212 2022-07-25 05:49:24.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/gradient_boosting.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2799 2022-07-25 05:49:24.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/mlp.py
--rw-r--r--   0 ad        (1000) ad        (1000)     5933 2023-02-16 09:19:46.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/ot_gpr.py
--rw-r--r--   0 ad        (1000) ad        (1000)     4401 2022-07-25 05:49:24.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/regressor_chain.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3030 2023-02-15 19:13:59.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/svm.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2151 2022-07-25 05:49:24.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/thin_plate_spline.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.284200 gemseo-mlearning-1.0.1/src/gemseo_mlearning.egg-info/
--rw-r--r--   0 ad        (1000) ad        (1000)     2506 2023-02-16 09:20:03.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning.egg-info/PKG-INFO
--rw-r--r--   0 ad        (1000) ad        (1000)     4196 2023-02-16 09:20:03.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning.egg-info/SOURCES.txt
--rw-r--r--   0 ad        (1000) ad        (1000)        1 2023-02-16 09:20:03.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning.egg-info/dependency_links.txt
--rw-r--r--   0 ad        (1000) ad        (1000)      105 2023-02-16 09:20:03.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning.egg-info/requires.txt
--rw-r--r--   0 ad        (1000) ad        (1000)       17 2023-02-16 09:20:03.000000 gemseo-mlearning-1.0.1/src/gemseo_mlearning.egg-info/top_level.txt
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.291200 gemseo-mlearning-1.0.1/tests/
--rw-r--r--   0 ad        (1000) ad        (1000)      735 2022-07-25 06:16:50.000000 gemseo-mlearning-1.0.1/tests/__init__.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.292199 gemseo-mlearning-1.0.1/tests/adaptive/
--rw-r--r--   0 ad        (1000) ad        (1000)      770 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/adaptive/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1376 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/adaptive/conftest.py
--rw-r--r--   0 ad        (1000) ad        (1000)     7626 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/adaptive/test_acquisition.py
--rw-r--r--   0 ad        (1000) ad        (1000)     6726 2023-02-15 20:00:56.000000 gemseo-mlearning-1.0.1/tests/adaptive/test_criteria.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3983 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/adaptive/test_criterion.py
--rw-r--r--   0 ad        (1000) ad        (1000)      853 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/conftest.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.293200 gemseo-mlearning-1.0.1/tests/distributions/
--rw-r--r--   0 ad        (1000) ad        (1000)      770 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/distributions/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1419 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/distributions/conftest.py
--rw-r--r--   0 ad        (1000) ad        (1000)     7419 2023-02-15 20:00:56.000000 gemseo-mlearning-1.0.1/tests/distributions/test_distribution.py
--rw-r--r--   0 ad        (1000) ad        (1000)     4108 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/distributions/test_kriging_distribution.py
--rw-r--r--   0 ad        (1000) ad        (1000)     8892 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/distributions/test_regressor_distribution.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.294200 gemseo-mlearning-1.0.1/tests/quality_measures/
--rw-r--r--   0 ad        (1000) ad        (1000)      770 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/quality_measures/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2104 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/quality_measures/test_mae_measure.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2112 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/quality_measures/test_me_measure.py
-drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-02-16 09:20:03.295199 gemseo-mlearning-1.0.1/tests/regression/
--rw-r--r--   0 ad        (1000) ad        (1000)      770 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/regression/__init__.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2037 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/regression/conftest.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2122 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/regression/test_gradient_boosting.py
--rw-r--r--   0 ad        (1000) ad        (1000)     2368 2022-07-25 05:49:24.000000 gemseo-mlearning-1.0.1/tests/regression/test_mlp.py
--rw-r--r--   0 ad        (1000) ad        (1000)     7250 2023-02-16 09:19:46.000000 gemseo-mlearning-1.0.1/tests/regression/test_ot_gpr.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3313 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/regression/test_regressor_chain.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1930 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/regression/test_svm.py
--rw-r--r--   0 ad        (1000) ad        (1000)     1462 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/regression/test_thin_plate_spline.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3442 2022-06-17 12:09:49.000000 gemseo-mlearning-1.0.1/tests/test_api.py
--rw-r--r--   0 ad        (1000) ad        (1000)     3215 2022-07-27 18:57:55.000000 gemseo-mlearning-1.0.1/tox.ini
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.784276 gemseo-mlearning-1.1.0/
+-rw-r--r--   0 ad        (1000) ad        (1000)      450 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/.gitattributes
+-rw-r--r--   0 ad        (1000) ad        (1000)      195 2022-07-25 05:50:08.000000 gemseo-mlearning-1.1.0/.gitignore
+-rw-r--r--   0 ad        (1000) ad        (1000)       87 2023-02-16 19:35:31.000000 gemseo-mlearning-1.1.0/.gitlab-ci.yml
+-rw-r--r--   0 ad        (1000) ad        (1000)     3051 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 ad        (1000) ad        (1000)     9105 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/.pylintrc
+-rw-r--r--   0 ad        (1000) ad        (1000)     1706 2023-06-02 18:54:01.000000 gemseo-mlearning-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     1788 2022-07-25 06:16:50.000000 gemseo-mlearning-1.1.0/CREDITS.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-mlearning-1.1.0/LICENSE.txt
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.766276 gemseo-mlearning-1.1.0/LICENSES/
+-rw-r--r--   0 ad        (1000) ad        (1000)     7652 2022-03-24 13:18:51.000000 gemseo-mlearning-1.1.0/LICENSES/LGPLv3.txt
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.766276 gemseo-mlearning-1.1.0/LICENSES/headers/
+-rw-r--r--   0 ad        (1000) ad        (1000)      729 2022-03-24 13:18:51.000000 gemseo-mlearning-1.1.0/LICENSES/headers/BSD-0-Clause.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)      334 2022-03-24 13:18:51.000000 gemseo-mlearning-1.1.0/LICENSES/headers/CC-BY-SA-4.0.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)      710 2022-03-24 13:18:51.000000 gemseo-mlearning-1.1.0/LICENSES/headers/LGPL-3.0.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2456 2023-06-04 18:33:39.784276 gemseo-mlearning-1.1.0/PKG-INFO
+-rw-r--r--   0 ad        (1000) ad        (1000)     1390 2022-07-27 19:22:29.000000 gemseo-mlearning-1.1.0/README.rst
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.759276 gemseo-mlearning-1.1.0/doc_src/
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.759276 gemseo-mlearning-1.1.0/doc_src/examples/
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.766276 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/
+-rw-r--r--   0 ad        (1000) ad        (1000)      749 2022-07-25 06:16:50.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/README.rst
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.768276 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/
+-rw-r--r--   0 ad        (1000) ad        (1000)      751 2022-07-25 06:16:50.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     5338 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_boot.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     5377 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_cv.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     5369 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_cv_boot.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     5204 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_krig.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     5964 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_rosenbrock.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     5900 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_limit_state.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.769276 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/api/
+-rw-r--r--   0 ad        (1000) ad        (1000)      759 2022-07-25 06:16:50.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/api/README.rst
+-rw-r--r--   0 ad        (1000) ad        (1000)     2178 2022-07-25 06:16:50.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/api/plot_sample_discipline.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2403 2022-07-25 06:16:50.000000 gemseo-mlearning-1.1.0/doc_src/examples/mlearning/api/plot_sample_disciplines.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.769276 gemseo-mlearning-1.1.0/doc_src/examples/optimization/
+-rw-r--r--   0 ad        (1000) ad        (1000)     1300 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/doc_src/examples/optimization/plot_sbo_rastrigin.py
+-rw-r--r--   0 ad        (1000) ad        (1000)      611 2023-03-14 13:21:46.000000 gemseo-mlearning-1.1.0/pyproject.toml
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.770276 gemseo-mlearning-1.1.0/requirements/
+-rw-r--r--   0 ad        (1000) ad        (1000)       79 2022-05-04 19:46:48.000000 gemseo-mlearning-1.1.0/requirements/check.in
+-rw-r--r--   0 ad        (1000) ad        (1000)      573 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/requirements/check.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       12 2022-05-04 19:46:48.000000 gemseo-mlearning-1.1.0/requirements/dist.in
+-rw-r--r--   0 ad        (1000) ad        (1000)     1491 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/requirements/dist.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2277 2023-02-09 17:58:14.000000 gemseo-mlearning-1.1.0/requirements/doc.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2831 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/requirements/test-python3.10.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2921 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/requirements/test-python3.8.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     2921 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/requirements/test-python3.9.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)     1699 2023-06-04 18:33:39.785276 gemseo-mlearning-1.1.0/setup.cfg
+-rw-r--r--   0 ad        (1000) ad        (1000)      839 2022-07-25 06:16:50.000000 gemseo-mlearning-1.1.0/setup.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.760276 gemseo-mlearning-1.1.0/src/
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.770276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/
+-rw-r--r--   0 ad        (1000) ad        (1000)      841 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.772276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/
+-rw-r--r--   0 ad        (1000) ad        (1000)      832 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     8715 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/acquisition.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.772276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/
+-rw-r--r--   0 ad        (1000) ad        (1000)      802 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.773276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/distances/
+-rw-r--r--   0 ad        (1000) ad        (1000)      855 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/distances/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2201 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/distances/criterion_min.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.773276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/expectation/
+-rw-r--r--   0 ad        (1000) ad        (1000)      844 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/expectation/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1851 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/expectation/criterion.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.773276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/mean_std/
+-rw-r--r--   0 ad        (1000) ad        (1000)      858 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/mean_std/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2613 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/mean_std/criterion.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.774276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/optimum/
+-rw-r--r--   0 ad        (1000) ad        (1000)      848 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/optimum/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1543 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/optimum/criterion.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2241 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/optimum/criterion_max.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2244 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/optimum/criterion_min.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.774276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/quantile/
+-rw-r--r--   0 ad        (1000) ad        (1000)      837 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/quantile/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1885 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/quantile/criterion.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.775276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/standard_deviation/
+-rw-r--r--   0 ad        (1000) ad        (1000)      851 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/standard_deviation/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1991 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/standard_deviation/criterion.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.775276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/value/
+-rw-r--r--   0 ad        (1000) ad        (1000)      838 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/value/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2459 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/value/criterion.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.775276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/variance/
+-rw-r--r--   0 ad        (1000) ad        (1000)      841 2023-02-15 19:24:27.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/variance/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1945 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/variance/criterion.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     5009 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criterion.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     9153 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/distribution.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.776276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/distributions/
+-rw-r--r--   0 ad        (1000) ad        (1000)     2391 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/distributions/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4140 2023-02-15 20:00:56.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/distributions/kriging_distribution.py
+-rw-r--r--   0 ad        (1000) ad        (1000)    11856 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/distributions/regressor_distribution.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.776276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/
+-rw-r--r--   0 ad        (1000) ad        (1000)      801 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.776276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/opt/
+-rw-r--r--   0 ad        (1000) ad        (1000)      896 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/opt/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.777276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/opt/core/
+-rw-r--r--   0 ad        (1000) ad        (1000)      830 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/opt/core/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     5659 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/opt/core/surrogate_based.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     7856 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/opt/lib_surrogate_based.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.777276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/opt/options/
+-rw-r--r--   0 ad        (1000) ad        (1000)     1386 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/opt/options/SBO_options.json
+-rw-r--r--   0 ad        (1000) ad        (1000)     4075 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/api.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.777276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/quality_measures/
+-rw-r--r--   0 ad        (1000) ad        (1000)      840 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/quality_measures/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2095 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/quality_measures/mae_measure.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2020 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/quality_measures/me_measure.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.779276 gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/
+-rw-r--r--   0 ad        (1000) ad        (1000)      799 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3217 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/gradient_boosting.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2804 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/mlp.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     6712 2023-06-02 18:53:14.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/ot_gpr.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4434 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/regressor_chain.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2967 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/svm.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2164 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/thin_plate_spline.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.771276 gemseo-mlearning-1.1.0/src/gemseo_mlearning.egg-info/
+-rw-r--r--   0 ad        (1000) ad        (1000)     2456 2023-06-04 18:33:39.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning.egg-info/PKG-INFO
+-rw-r--r--   0 ad        (1000) ad        (1000)     4843 2023-06-04 18:33:39.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning.egg-info/SOURCES.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)        1 2023-06-04 18:33:39.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning.egg-info/dependency_links.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       53 2023-06-04 18:33:39.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning.egg-info/entry_points.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)      101 2023-06-04 18:33:39.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning.egg-info/requires.txt
+-rw-r--r--   0 ad        (1000) ad        (1000)       17 2023-06-04 18:33:39.000000 gemseo-mlearning-1.1.0/src/gemseo_mlearning.egg-info/top_level.txt
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.779276 gemseo-mlearning-1.1.0/tests/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.780276 gemseo-mlearning-1.1.0/tests/adaptive/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/tests/adaptive/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1383 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/tests/adaptive/conftest.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.781276 gemseo-mlearning-1.1.0/tests/adaptive/distributions/
+-rw-r--r--   0 ad        (1000) ad        (1000)      830 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/adaptive/distributions/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1952 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/tests/adaptive/distributions/conftest.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     7424 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/tests/adaptive/distributions/test_distribution.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1457 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/adaptive/distributions/test_get_regressor_distribution.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3960 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/adaptive/distributions/test_kriging_distribution.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     8715 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/adaptive/distributions/test_regressor_distribution.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     7636 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/tests/adaptive/test_acquisition.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     6827 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/tests/adaptive/test_criteria.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     4397 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/tests/adaptive/test_criterion.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.782276 gemseo-mlearning-1.1.0/tests/algos/
+-rw-r--r--   0 ad        (1000) ad        (1000)      802 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/algos/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.782276 gemseo-mlearning-1.1.0/tests/algos/opt/
+-rw-r--r--   0 ad        (1000) ad        (1000)      827 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/algos/opt/__init__.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.782276 gemseo-mlearning-1.1.0/tests/algos/opt/core/
+-rw-r--r--   0 ad        (1000) ad        (1000)      842 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/algos/opt/core/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3080 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/algos/opt/core/test_surrogate_based.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1578 2023-03-10 14:02:53.000000 gemseo-mlearning-1.1.0/tests/algos/opt/test_surrogate_based_algos.py
+-rw-r--r--   0 ad        (1000) ad        (1000)      861 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/tests/conftest.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.783276 gemseo-mlearning-1.1.0/tests/quality_measures/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/tests/quality_measures/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2104 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/tests/quality_measures/test_mae_measure.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2112 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/tests/quality_measures/test_me_measure.py
+drwxr-xr-x   0 ad        (1000) ad        (1000)        0 2023-06-04 18:33:39.784276 gemseo-mlearning-1.1.0/tests/regression/
+-rw-r--r--   0 ad        (1000) ad        (1000)      770 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/tests/regression/__init__.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2401 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/tests/regression/conftest.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2122 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/tests/regression/test_gradient_boosting.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     2368 2022-07-25 05:49:24.000000 gemseo-mlearning-1.1.0/tests/regression/test_mlp.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     8049 2023-06-02 18:53:14.000000 gemseo-mlearning-1.1.0/tests/regression/test_ot_gpr.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3317 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/tests/regression/test_regressor_chain.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1930 2022-06-17 12:09:49.000000 gemseo-mlearning-1.1.0/tests/regression/test_svm.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     1463 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/tests/regression/test_thin_plate_spline.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3662 2023-05-17 07:03:45.000000 gemseo-mlearning-1.1.0/tests/test_api.py
+-rw-r--r--   0 ad        (1000) ad        (1000)     3272 2023-05-16 08:08:01.000000 gemseo-mlearning-1.1.0/tox.ini
```

### Comparing `gemseo-mlearning-1.0.1/.pylintrc` & `gemseo-mlearning-1.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/CHANGELOG.rst` & `gemseo-mlearning-1.1.0/CHANGELOG.rst`

 * *Files 27% similar despite different names*

```diff
@@ -21,14 +21,27 @@
 All notable changes of this project will be documented here.
 
 The format is based on
 `Keep a Changelog <https://keepachangelog.com/en/1.0.0/>`_
 and this project adheres to
 `Semantic Versioning <https://semver.org/spec/v2.0.0.html>`_.
 
+Version 1.1.0 (June 2023)
+*************************
+
+Added
+-----
+
+- An argument ``trend_type`` of type :attr:`~.OTGaussianProcessRegressor.TREND_TYPE`` to :class:`.OTGaussianProcessRegressor`; the trend type of the Gaussian process regressor can be either constant, linear or quadratic.
+- A new optimization library :class:`SurrogateBasedOptimization` to perform EGO-like surrogate-based optimization on unconstrained problems.
+
+Fixed
+-----
+
+- The output of an :class:`.MLDataAcquisitionCriterion` based on a regressor built from constant output values is no longer ``nan``.
 
 Version 1.0.1 (February 2022)
 *****************************
 
 Fixed
 -----
```

### Comparing `gemseo-mlearning-1.0.1/CREDITS.rst` & `gemseo-mlearning-1.1.0/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/LICENSE.txt` & `gemseo-mlearning-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/LICENSES/LGPLv3.txt` & `gemseo-mlearning-1.1.0/LICENSES/LGPLv3.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/LICENSES/headers/BSD-0-Clause.txt` & `gemseo-mlearning-1.1.0/LICENSES/headers/BSD-0-Clause.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/LICENSES/headers/LGPL-3.0.txt` & `gemseo-mlearning-1.1.0/LICENSES/headers/LGPL-3.0.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/PKG-INFO` & `gemseo-mlearning-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-mlearning
-Version: 1.0.1
+Version: 1.1.0
 Summary: Miscellaneous machine learning capabilities.
 Home-page: https://gitlab.com/gemseo
 Author: Matthias De Lozzo
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-mlearning
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-mlearning/-/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-mlearning-1.0.1/README.rst` & `gemseo-mlearning-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/README.rst` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/README.rst`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/README.rst` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/README.rst`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_boot.py` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_boot.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,17 @@
 ##############################################################################
 # Plotting
 # --------
 fig, ax = plt.subplots(2, 1)
 for algo_b in distribution.algos:
     algo_data = [algo_b.predict(array([x_i])) for x_i in x_test]
     ax[0].plot(x_test, algo_data, "gray", alpha=0.2)
-ax[0].plot(x_train, dataset["y"], "ro", label="training")
+ax[0].plot(
+    x_train, dataset.get_view(variable_names="y").to_numpy(), "ro", label="training"
+)
 ax[0].plot(x_test, disc_data["y"], "r", label="original")
 ax[0].plot(x_test, surr_data, "b", label="surrogate")
 ax[0].fill_between(
     x_test, lower_data, upper_data, color="b", alpha=0.1, label="CI(95%)"
 )
 ax[0].legend(loc="upper right")
 ax[0].axvline(x=opt[0])
```

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_cv.py` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_krig.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,35 +24,36 @@
 # WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED
 # WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL
 # THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
 # OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING
 # FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT,
 # NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+#
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """
-Expected improvement based on cross-validation
-==============================================
+Expected improvement based on bootstrap
+=======================================
 """
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
 from gemseo.algos.design_space import DesignSpace
 from gemseo.disciplines.analytic import AnalyticDiscipline
-from gemseo.mlearning.regression.rbf import RBFRegressor
+from gemseo.mlearning.regression.gpr import GaussianProcessRegressor
 from gemseo_mlearning.adaptive.acquisition import MLDataAcquisition
 from gemseo_mlearning.adaptive.criteria.mean_std.criterion import MeanSigma
 from gemseo_mlearning.adaptive.criteria.optimum.criterion import (
     ExpectedImprovement,
 )
-from gemseo_mlearning.adaptive.distributions.regressor_distribution import (
-    RegressorDistribution,
+from gemseo_mlearning.adaptive.distributions.kriging_distribution import (
+    KrigingDistribution,
 )
 from numpy import array
 from numpy import linspace
 
 n_test = 200
 x_l = -3.0
 x_u = 3.0
@@ -66,21 +67,21 @@
 for x_i in x_train:
     discipline.execute({"x": array([x_i])})
 dataset = discipline.cache.export_to_dataset()
 
 ##############################################################################
 # Initial surrogate model
 # -----------------------
-algo = RBFRegressor(dataset)
+algo = GaussianProcessRegressor(dataset)
 algo.learn()
 
 ##############################################################################
 # Create MLAlgoSampler
 # --------------------
-distribution = RegressorDistribution(algo, bootstrap=False, loo=True)
+distribution = KrigingDistribution(algo)
 distribution.learn()
 
 ##############################################################################
 # Filling objectives
 # ------------------
 ego = ExpectedImprovement(distribution)
 lower = MeanSigma(distribution, -2.0)
@@ -117,18 +118,17 @@
 
 disc_data = discipline.cache.export_to_dataset()
 
 ##############################################################################
 # Plotting
 # --------
 fig, ax = plt.subplots(2, 1)
-for algo_b in distribution.algos:
-    algo_data = [algo_b.predict(array([x_i])) for x_i in x_test]
-    ax[0].plot(x_test, algo_data, "gray", alpha=0.2)
-ax[0].plot(x_train, dataset["y"], "ro", label="training")
+ax[0].plot(
+    x_train, dataset.get_view(variable_names="y").to_numpy(), "ro", label="training"
+)
 ax[0].plot(x_test, disc_data["y"], "r", label="original")
 ax[0].plot(x_test, surr_data, "b", label="surrogate")
 ax[0].fill_between(
     x_test, lower_data, upper_data, color="b", alpha=0.1, label="CI(95%)"
 )
 ax[0].legend(loc="upper right")
 ax[0].axvline(x=opt[0])
```

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_cv_boot.py` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_cv_boot.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 # %%
 # Active learning
 # ---------------
 # We compare the bootstrap and leave-one-out methods
 # in search of a new point to learn
 # in order to estimate the minimum of the discipline
 for index, bootstrap in enumerate([False, True]):
-
     # Train a RBF regression model
     algo = RBFRegressor(dataset)
     algo.learn()
 
     # Build a regressor distribution
     distribution = RegressorDistribution(algo, bootstrap=bootstrap, loo=not bootstrap)
     distribution.learn()
@@ -124,15 +123,17 @@
 
     disc_data = discipline.cache.export_to_dataset()
 
     for algo in distribution.algos:
         algo_data = [algo.predict(array([x_i])) for x_i in x_test]
         ax[0][index].plot(x_test, algo_data, "gray", alpha=0.2)
 
-    ax[0][index].plot(x_train, dataset["y"], "ro", label="training")
+    ax[0][index].plot(
+        x_train, dataset.get_view(variable_names="y").to_numpy(), "ro", label="training"
+    )
     ax[0][index].plot(x_test, disc_data["y"], "r", label="original")
     ax[0][index].plot(x_test, surr_data, "b", label="surrogate")
     ax[0][index].fill_between(
         x_test,
         array(lower_data),
         array(upper_data),
         color="b",
```

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_krig.py` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_cv.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,36 +24,35 @@
 # WARRANTIES WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED
 # WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL
 # THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT,
 # OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING
 # FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT,
 # NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION
 # WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
-#
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """
-Expected improvement based on bootstrap
-=======================================
+Expected improvement based on cross-validation
+==============================================
 """
 from __future__ import annotations
 
 import matplotlib.pyplot as plt
 from gemseo.algos.design_space import DesignSpace
 from gemseo.disciplines.analytic import AnalyticDiscipline
-from gemseo.mlearning.regression.gpr import GaussianProcessRegressor
+from gemseo.mlearning.regression.rbf import RBFRegressor
 from gemseo_mlearning.adaptive.acquisition import MLDataAcquisition
 from gemseo_mlearning.adaptive.criteria.mean_std.criterion import MeanSigma
 from gemseo_mlearning.adaptive.criteria.optimum.criterion import (
     ExpectedImprovement,
 )
-from gemseo_mlearning.adaptive.distributions.kriging_distribution import (
-    KrigingDistribution,
+from gemseo_mlearning.adaptive.distributions.regressor_distribution import (
+    RegressorDistribution,
 )
 from numpy import array
 from numpy import linspace
 
 n_test = 200
 x_l = -3.0
 x_u = 3.0
@@ -67,21 +66,21 @@
 for x_i in x_train:
     discipline.execute({"x": array([x_i])})
 dataset = discipline.cache.export_to_dataset()
 
 ##############################################################################
 # Initial surrogate model
 # -----------------------
-algo = GaussianProcessRegressor(dataset)
+algo = RBFRegressor(dataset)
 algo.learn()
 
 ##############################################################################
 # Create MLAlgoSampler
 # --------------------
-distribution = KrigingDistribution(algo)
+distribution = RegressorDistribution(algo, bootstrap=False, loo=True)
 distribution.learn()
 
 ##############################################################################
 # Filling objectives
 # ------------------
 ego = ExpectedImprovement(distribution)
 lower = MeanSigma(distribution, -2.0)
@@ -118,15 +117,20 @@
 
 disc_data = discipline.cache.export_to_dataset()
 
 ##############################################################################
 # Plotting
 # --------
 fig, ax = plt.subplots(2, 1)
-ax[0].plot(x_train, dataset["y"], "ro", label="training")
+for algo_b in distribution.algos:
+    algo_data = [algo_b.predict(array([x_i])) for x_i in x_test]
+    ax[0].plot(x_test, algo_data, "gray", alpha=0.2)
+ax[0].plot(
+    x_train, dataset.get_view(variable_names="y").to_numpy(), "ro", label="training"
+)
 ax[0].plot(x_test, disc_data["y"], "r", label="original")
 ax[0].plot(x_test, surr_data, "b", label="surrogate")
 ax[0].fill_between(
     x_test, lower_data, upper_data, color="b", alpha=0.1, label="CI(95%)"
 )
 ax[0].legend(loc="upper right")
 ax[0].axvline(x=opt[0])
```

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_ego_rosenbrock.py` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_ego_rosenbrock.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         disc_data[i, j] = discipline.execute(input_data)["z"][0]
         crit_data[i, j] = crit(xij)
         surr_data[i, j] = algo.predict(xij)[0]
 
 ##############################################################################
 # Plotting
 # --------
-train = learning_dataset[["x", "y"]]
+train = learning_dataset.get_view(variable_names=["x", "y"]).to_numpy()
 x_train = train["x"]
 y_train = train["y"]
 fig = plt.figure(constrained_layout=True)
 spec = gridspec.GridSpec(ncols=2, nrows=2, figure=fig)
 axes = [[None, None], [None, None]]
 titles = [["Discipline", "Infill criterion"], ["Surrogate model", None]]
 data = [[disc_data, crit_data], [surr_data, None]]
```

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/adaptive/plot_limit_state.py` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/adaptive/plot_limit_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         disc_data[i, j] = discipline.execute(input_data)["z"][0]
         crit_data[i, j] = crit(xij)
         surr_data[i, j] = algo.predict(xij)[0]
 
 ##############################################################################
 # Plotting
 # --------
-train = learning_dataset[["x", "y"]]
+train = learning_dataset.get_view(variable_names=["x", "y"]).to_numpy()
 x_train = train["x"]
 y_train = train["y"]
 fig = plt.figure(constrained_layout=True)
 spec = gridspec.GridSpec(ncols=2, nrows=2, figure=fig)
 axes = [[None, None], [None, None]]
 titles = [["Discipline", "Infill criterion"], ["Surrogate model", None]]
 data = [[disc_data, crit_data], [surr_data, None]]
```

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/api/README.rst` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/api/README.rst`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/api/plot_sample_discipline.py` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/api/plot_sample_discipline.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/doc_src/examples/mlearning/api/plot_sample_disciplines.py` & `gemseo-mlearning-1.1.0/doc_src/examples/mlearning/api/plot_sample_disciplines.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/pyproject.toml` & `gemseo-mlearning-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # logging settings identical to the defaults of gemseo.api.configure_logger()
 log_file_level = "INFO"
 log_file_date_format = "%H:%M:%S"
 log_file_format = "%(levelname)8s - %(asctime)s: %(message)s"
 # filterwarnings = ignore::pytest.PytestExperimentalApiWarning
 
 [tool.black]
-target-version = ['py37']
+target-version = ['py38']
```

### Comparing `gemseo-mlearning-1.0.1/requirements/dist.txt` & `gemseo-mlearning-1.1.0/requirements/dist.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,79 +4,79 @@
 #
 #    pip-compile requirements/dist.in
 #
 bleach==6.0.0
     # via readme-renderer
 build==0.10.0
     # via -r requirements/dist.in
-certifi==2022.12.7
+certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via cryptography
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
     # via requests
-cryptography==39.0.1
+cryptography==40.0.2
     # via secretstorage
-docutils==0.19
+docutils==0.20
     # via readme-renderer
 idna==3.4
     # via requests
-importlib-metadata==6.0.0
+importlib-metadata==6.6.0
     # via
     #   keyring
     #   twine
 jaraco-classes==3.2.3
     # via keyring
 jeepney==0.8.0
     # via
     #   keyring
     #   secretstorage
 keyring==23.13.1
     # via twine
-markdown-it-py==2.1.0
+markdown-it-py==2.2.0
     # via rich
 mdurl==0.1.2
     # via markdown-it-py
-more-itertools==9.0.0
+more-itertools==9.1.0
     # via jaraco-classes
-packaging==23.0
+packaging==23.1
     # via build
 pkginfo==1.9.6
     # via twine
 pycparser==2.21
     # via cffi
-pygments==2.14.0
+pygments==2.15.1
     # via
     #   readme-renderer
     #   rich
 pyproject-hooks==1.0.0
     # via build
 readme-renderer==37.3
     # via twine
-requests==2.28.2
+requests==2.30.0
     # via
     #   requests-toolbelt
     #   twine
-requests-toolbelt==0.10.1
+requests-toolbelt==1.0.0
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.1
+rich==13.3.5
     # via twine
 secretstorage==3.3.3
     # via keyring
 six==1.16.0
     # via bleach
 tomli==2.0.1
     # via
     #   build
     #   pyproject-hooks
 twine==4.0.2
     # via -r requirements/dist.in
-urllib3==1.26.14
+urllib3==2.0.2
     # via
     #   requests
     #   twine
 webencodings==0.5.1
     # via bleach
-zipp==3.13.0
+zipp==3.15.0
     # via importlib-metadata
```

### Comparing `gemseo-mlearning-1.0.1/requirements/doc.txt` & `gemseo-mlearning-1.1.0/requirements/doc.txt`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/setup.cfg` & `gemseo-mlearning-1.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -17,27 +17,26 @@
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Intended Audience :: Science/Research
 	Topic :: Scientific/Engineering
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 
 [options]
 package_dir = 
 	=src
 packages = find:
 include_package_data = true
-python_requires = >=3.7, <3.11
+python_requires = >=3.8, <3.11
 install_requires = 
-	gemseo[all] >=4.0.0
+	gemseo[all] >=5
 	numpy
 	openturns
 	scipy
 	scikit-learn
 
 [options.packages.find]
 where = src
@@ -48,31 +47,38 @@
 	pytest
 	pytest-cov
 	pytest-xdist
 
 [bdist_wheel]
 universal = true
 
+[options.entry_points]
+gemseo_plugins = 
+	gemseo-mlearning = gemseo_mlearning
+
 [coverage:run]
 plugins = covdefaults
 source = gemseo_mlearning
 
 [coverage:report]
 fail_under = 1
 
 [flake8]
 ignore = 
 	E501
 	D105
 	E203
 	W503
-select = B,C,D,E,F,G,N,T,W,B950
+	ANN101
+	ANN102
+	ANN401
+select = ANN,B,C,D,E,F,G,N,T,W,B950
 max-line-length = 88
 docstring-convention = google
 per-file-ignores = 
-	tests/*.py:D100,D104,D417
-	doc_src/*.py:D,T001
+	tests/*.py: D100,D104,ANN
+	doc_src/*.py: D,T201
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `gemseo-mlearning-1.0.1/setup.py` & `gemseo-mlearning-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/acquisition.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/acquisition.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,18 +26,21 @@
 
 from gemseo.algos.database import Database
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.doe.doe_factory import DOEFactory
 from gemseo.algos.opt.opt_factory import OptimizersFactory
 from gemseo.algos.opt_problem import OptimizationProblem
 from gemseo.core.discipline import MDODiscipline
+from gemseo.datasets.io_dataset import IODataset
 from gemseo.mlearning.core.ml_algo import DataType
 from numpy import array
+from pandas import concat
 
 from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterionFactory
+from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterionOptionType
 from gemseo_mlearning.adaptive.distribution import MLRegressorDistribution
 
 LOGGER = logging.getLogger(__name__)
 
 _CRITERION_FACTORY = MLDataAcquisitionCriterionFactory()
 
 
@@ -45,27 +48,25 @@
     """Data acquisition for adaptive learning."""
 
     default_algo_name: ClassVar[str] = "NLOPT_COBYLA"
     """The name of the default algorithm to find the point(s).
 
     Typically a DoE or an optimizer.
     """
-
     default_opt_options: ClassVar[dict[str, Any]] = {"max_iter": 100}
     """The names and values of the default optimization options."""
-
     default_doe_options: ClassVar[dict[str, Any]] = {"n_samples": 100}
     """The names and values of the default DoE options."""
 
     def __init__(
         self,
         criterion: str,
         input_space: DesignSpace,
         distribution: MLRegressorDistribution,
-        **options: Any,
+        **options: MLDataAcquisitionCriterionOptionType,
     ) -> None:
         """# noqa: D205 D212 D415
         Args:
             criterion: The name of a data acquisition criterion
                 selecting new point(s) to reach a particular goal
                 (name of a class inheriting from :class:`.MLDataAcquisitionCriterion`).
             input_space: The input space on which to look for the new learning point.
@@ -98,20 +99,24 @@
         Approximate the Jacobian with finite differences if missing.
 
         Returns:
             The optimization problem.
         """
         problem = OptimizationProblem(self.__input_space)
         problem.objective = _CRITERION_FACTORY.create(
-            self.__criterion, self.__distribution, **self.__criterion_options
+            self.__criterion,
+            algo_distribution=self.__distribution,
+            **self.__criterion_options,
         )
         problem.objective.name = self.__criterion
 
-        if not problem.objective.has_jac():
-            problem.differentiation_method = OptimizationProblem.FINITE_DIFFERENCES
+        if not problem.objective.has_jac:
+            problem.differentiation_method = (
+                OptimizationProblem.DifferentiationMethod.FINITE_DIFFERENCES
+            )
 
         if problem.objective.MAXIMIZE:
             problem.change_objective_sign()
 
         return problem
 
     def set_acquisition_algorithm(self, algo_name: str, **options: Any) -> None:
@@ -175,21 +180,41 @@
         for index in range(n_samples):
             root_logger = logging.getLogger()
             saved_level = root_logger.level
             root_logger.setLevel(logging.WARNING)
             LOGGER.setLevel(logging.WARNING)
             input_data = self.compute_next_input_data(as_dict=True)
             for inputs, outputs in self.__problem.database.items():
-                self.__database[array([index + 1] + inputs.unwrap().tolist())] = outputs
+                self.__database.store(
+                    array([index + 1] + inputs.unwrap().tolist()), outputs
+                )
 
             discipline.execute(input_data)
-            learning_cache = self.__distribution.algo.learning_set.export_to_cache()
-            learning_cache[input_data] = (
-                {k: discipline.local_data[k] for k in self.__distribution.output_names},
-                None,
+
+            # TODO: This is a dirty fix. Please refactor this function.
+            # WARNING: Using concat like this could lead to performance issues.
+            dataset_to_add = IODataset()
+            for input_name, input_value in input_data.items():
+                dataset_to_add.add_variable(
+                    input_name, input_value, group_name=dataset_to_add.INPUT_GROUP
+                )
+            for output_name in self.__distribution.output_names:
+                dataset_to_add.add_variable(
+                    output_name,
+                    discipline.local_data[output_name],
+                    group_name=dataset_to_add.OUTPUT_GROUP,
+                )
+            dataset = concat(
+                [self.__distribution.algo.learning_set, dataset_to_add],
+                ignore_index=True,
             )
-            self.__distribution.change_learning_set(learning_cache.export_to_dataset())
-            self.__problem = self.__build_optimization_problem()
+
+            self.__distribution.change_learning_set(dataset)
+            self.update_problem()
             LOGGER.setLevel(saved_level)
             LOGGER.info("Add sample %s out of %s", index + 1, n_samples)
 
         return self.__database, self.__problem
+
+    def update_problem(self) -> None:
+        """Update the optimization problem."""
+        self.__problem = self.__build_optimization_problem()
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/distances/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/distances/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/distances/criterion_min.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/distances/criterion_min.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,41 +16,43 @@
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Minimum distance between a point and the learning dataset."""
 from __future__ import annotations
 
-from numpy import ndarray
+from typing import Callable
+
 from numpy import nonzero
+from numpy.typing import NDArray
 from scipy.spatial.distance import cdist
 
 from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterion
 
 
 class MinimumDistance(MLDataAcquisitionCriterion):
     """Minimum distance to the learning dataset.
 
     This infill criterion computes the minimum distance between a new point and the
     point of the learning dataset, scaled by the maximum distance between two learning
     points.
     """
 
-    def _get_func(self):
-        def func(input_data: ndarray) -> float:
+    def _get_func(self) -> Callable[[NDArray[float]], float]:
+        def func(input_data: NDArray[float]) -> float:
             """Evaluation function.
 
             Args:
                 input_data: The model input data.
 
             Returns:
                 The acquisition criterion value.
             """
             train = self.algo_distribution.learning_set
-            train = train.get_data_by_group(train.INPUT_GROUP)
+            train = train.get_view(group_names=train.INPUT_GROUP).to_numpy()
             distance = cdist(input_data.reshape((1, -1)), train).min()
             dist_train = cdist(train, train)
             d_max = dist_train[nonzero(dist_train)].min() / 2.0
             distance /= d_max
             return distance
 
         return func
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/expectation/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/expectation/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/expectation/criterion.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/expectation/criterion.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,35 +25,38 @@
    E[x] = E[Y(x)]
 
 Bootstrap estimator:
 
 .. math::
 
    \widehat{E}[x] = \frac{1}{B}\sum_{b=1}^B Y_b(x)
-
 """
 from __future__ import annotations
 
-from numpy import ndarray
+from typing import Callable
+
+from numpy.typing import NDArray
 
 from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterion
 
 
 class Expectation(MLDataAcquisitionCriterion):
     """Expectation of the regression model.".
 
     This criterion is scaled by the output range.
     """
 
-    def _get_func(self):
-        def func(input_data: ndarray) -> float:
+    def _get_func(self) -> Callable[[NDArray[float]], float]:
+        def func(input_data: NDArray[float]) -> float:
             """Evaluation function.
 
             Args:
                 input_data: The model input data.
 
             Returns:
                 The acquisition criterion value.
             """
-            return self.algo_distribution.compute_mean(input_data) / self.output_range
+            return (
+                self.algo_distribution.compute_mean(input_data) / self._scaling_factor
+            )
 
         return func
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/mean_std/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/mean_std/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/mean_std/criterion.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/mean_std/criterion.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,19 +26,20 @@
    E_sigma[x] = E[x] + \kappa \times sigma[x]
 
 Estimator:
 
 .. math::
 
    \widehat{E_sigma}[x] = \widehat{E}[x] + \kappa \times \widehat{sigma}[x]
-
 """
 from __future__ import annotations
 
-from numpy import ndarray
+from typing import Callable
+
+from numpy.typing import NDArray
 
 from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterion
 from gemseo_mlearning.adaptive.distribution import MLRegressorDistribution
 
 
 class MeanSigma(MLDataAcquisitionCriterion):
     """Combination of the expectation and standard deviation of the regression model.
@@ -56,22 +57,22 @@
         Args:
             kappa: A factor associated with the standard deviation
                 to increase or decrease the mean value.
         """
         self.kappa = kappa
         super().__init__(algo_distribution)
 
-    def _get_func(self):
-        def func(input_data: ndarray) -> float:
+    def _get_func(self) -> Callable[[NDArray[float]], float]:
+        def func(input_data: NDArray[float]) -> float:
             """Evaluation function.
 
             Args:
                 input_data: The model input data.
 
             Returns:
                 The acquisition criterion value.
             """
             mean = self.algo_distribution.compute_mean(input_data)
             sigma = self.algo_distribution.compute_standard_deviation(input_data)
-            return (mean + self.kappa * sigma) / self.output_range
+            return (mean + self.kappa * sigma) / self._scaling_factor
 
         return func
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/optimum/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/optimum/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/optimum/criterion.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/optimum/criterion.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 where :math:`y_{min}=\min_{1\leq i \leq n}~y^{(i)}`.
 
 Bootstrap estimator:
 
 .. math::
 
    \widehat{EI}[x] = \frac{1}{B}\sum_{b=1}^B \max(f_{min}-Y_b(x),0)
-
 """
 from __future__ import annotations
 
 from gemseo_mlearning.adaptive.criteria.optimum.criterion_min import (
     MinExpectedImprovement,
 )
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/optimum/criterion_max.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/optimum/criterion_min.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,55 +12,58 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
-r"""Expected improvement for the maximum.
+r"""Expected improvement for the minimum.
 
 Statistics:
 
 .. math::
 
-   EI[x] = E[\max(Y(x)-y_{max},0)]
+   EI[x] = E[\max(y_{min}-Y(x),0)]
 
-where :math:`y_{max}=\max_{1\leq i \leq n}~y^{(i)}`.
+where :math:`y_{min}=\min_{1\leq i \leq n}~y^{(i)}`.
 
 Bootstrap estimator:
 
 .. math::
 
-   \widehat{EI}[x] = \frac{1}{B}\sum_{b=1}^B \max(Y_b(x)-f_{max},0)
-
+   \widehat{EI}[x] = \frac{1}{B}\sum_{b=1}^B \max(f_{min}-Y_b(x),0)
 """
 from __future__ import annotations
 
-from numpy import ndarray
+from typing import Callable
+
+from numpy.typing import NDArray
 
 from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterion
 
 
-class MaxExpectedImprovement(MLDataAcquisitionCriterion):
-    """Expected Improvement of the regression model for the maximum.
+class MinExpectedImprovement(MLDataAcquisitionCriterion):
+    """Expected Improvement of the regression model for the minimum.
 
     This criterion is scaled by the output range.
     """
 
-    def _get_func(self):
-        def func(input_data: ndarray) -> float:
+    def _get_func(self) -> Callable[[NDArray[float]], float]:
+        def func(input_data: NDArray[float]) -> float:
             """Evaluation function.
 
             Args:
                 input_data: The model input data.
 
             Returns:
                 The acquisition criterion value.
             """
-            data = self.algo_distribution.learning_set
-            maximum_output = max(data.get_data_by_group(data.OUTPUT_GROUP))
+            dataset = self.algo_distribution.learning_set
+            minimum_output = min(
+                dataset.get_view(group_names=dataset.OUTPUT_GROUP).to_numpy()
+            )
             expected_improvement = self.algo_distribution.compute_expected_improvement(
-                input_data, maximum_output, True
+                input_data, minimum_output
             )
-            return expected_improvement / self.output_range
+            return expected_improvement / self._scaling_factor
 
         return func
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/optimum/criterion_min.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/optimum/criterion_max.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,55 +12,58 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
-r"""Expected improvement for the minimum.
+r"""Expected improvement for the maximum.
 
 Statistics:
 
 .. math::
 
-   EI[x] = E[\max(y_{min}-Y(x),0)]
+   EI[x] = E[\max(Y(x)-y_{max},0)]
 
-where :math:`y_{min}=\min_{1\leq i \leq n}~y^{(i)}`.
+where :math:`y_{max}=\max_{1\leq i \leq n}~y^{(i)}`.
 
 Bootstrap estimator:
 
 .. math::
 
-   \widehat{EI}[x] = \frac{1}{B}\sum_{b=1}^B \max(f_{min}-Y_b(x),0)
-
+   \widehat{EI}[x] = \frac{1}{B}\sum_{b=1}^B \max(Y_b(x)-f_{max},0)
 """
 from __future__ import annotations
 
-from numpy import ndarray
+from typing import Callable
+
+from numpy.typing import NDArray
 
 from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterion
 
 
-class MinExpectedImprovement(MLDataAcquisitionCriterion):
-    """Expected Improvement of the regression model for the minimum.
+class MaxExpectedImprovement(MLDataAcquisitionCriterion):
+    """Expected Improvement of the regression model for the maximum.
 
     This criterion is scaled by the output range.
     """
 
-    def _get_func(self):
-        def func(input_data: ndarray) -> float:
+    def _get_func(self) -> Callable[[NDArray[float]], float]:
+        def func(input_data: NDArray[float]) -> float:
             """Evaluation function.
 
             Args:
                 input_data: The model input data.
 
             Returns:
                 The acquisition criterion value.
             """
-            dataset = self.algo_distribution.learning_set
-            minimum_output = min(dataset.get_data_by_group(dataset.OUTPUT_GROUP))
+            data = self.algo_distribution.learning_set
+            maximum_output = max(
+                data.get_view(group_names=data.OUTPUT_GROUP).to_numpy()
+            )
             expected_improvement = self.algo_distribution.compute_expected_improvement(
-                input_data, minimum_output
+                input_data, maximum_output, True
             )
-            return expected_improvement / self.output_range
+            return expected_improvement / self._scaling_factor
 
         return func
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/quantile/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/quantile/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/quantile/criterion.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/quantile/criterion.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 where :math:`q` is a quantile with level :math:`\alpha`.
 
 Bootstrap estimator:
 
 .. math::
 
    \widehat{EI}[x] = \frac{1}{B}\sum_{b=1}^B |q-Y_b(x)|
-
 """
 from __future__ import annotations
 
 from numpy import quantile
 
 from gemseo_mlearning.adaptive.criteria.value.criterion import LimitState
 from gemseo_mlearning.adaptive.distribution import MLRegressorDistribution
@@ -49,9 +48,11 @@
         self, algo_distribution: MLRegressorDistribution, level: float
     ) -> None:
         """# noqa: D205 D212 D415
         Args:
             level: A quantile level.
         """
         dataset = algo_distribution.learning_set
-        limit_state = quantile(dataset.get_data_by_group(dataset.OUTPUT_GROUP), level)
+        limit_state = quantile(
+            dataset.get_view(group_names=dataset.OUTPUT_GROUP), level
+        )
         super().__init__(algo_distribution, limit_state)
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/standard_deviation/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/standard_deviation/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/standard_deviation/criterion.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/standard_deviation/criterion.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,32 +31,34 @@
 
    \hat{\sigma}[x] = \sqrt{\frac{1}{B-1}\sum_{b=1}^B (Y_b(x)-\widehat{E}[x])^2}
 
 where :math:`\widehat{E}[x]= \frac{1}{B}\sum_{b=1}^B Y_b(x)`.
 """
 from __future__ import annotations
 
-from numpy import ndarray
+from typing import Callable
+
+from numpy.typing import NDArray
 
 from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterion
 
 
 class StandardDeviation(MLDataAcquisitionCriterion):
     """Standard Deviation of the regression model.
 
     This criterion is scaled by the output range.
     """
 
-    def _get_func(self):
-        def func(input_data: ndarray) -> float:
+    def _get_func(self) -> Callable[[NDArray[float]], float]:
+        def func(input_data: NDArray[float]) -> float:
             """Evaluation function.
 
             Args:
                 input_data: The model input data.
 
             Returns:
                 The acquisition criterion value.
             """
             std = self.algo_distribution.compute_standard_deviation(input_data)
-            return std / self.output_range
+            return std / self._scaling_factor
 
         return func
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/value/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/value/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/value/criterion.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/value/criterion.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 where :math:`q` is a value provided by the user.
 
 Bootstrap estimator:
 
 .. math::
 
    \widehat{EI}[x] = \frac{1}{B}\sum_{b=1}^B |q-Y_b(x)|
-
 """
 from __future__ import annotations
 
+from typing import Callable
 from typing import ClassVar
 
-from numpy import ndarray
+from numpy.typing import NDArray
 
 from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterion
 from gemseo_mlearning.adaptive.distribution import MLRegressorDistribution
 
 
 class LimitState(MLDataAcquisitionCriterion):
     """Expected Improvement of the regression model for a particular value."""
@@ -58,16 +58,16 @@
         """# noqa: D205 D212 D415
         Args:
             value: A value of interest.
         """
         self.value = value
         super().__init__(algo_distribution)
 
-    def _get_func(self):
-        def func(input_data: ndarray) -> float:
+    def _get_func(self) -> Callable[[NDArray[float]], float]:
+        def func(input_data: NDArray[float]) -> float:
             """Evaluation function.
 
             Args:
                 input_data: The model input data.
 
             Returns:
                 The acquisition criterion value.
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/variance/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/variance/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criteria/variance/criterion.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criteria/variance/criterion.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,32 +31,34 @@
 
    \widehat{V}[x] = \frac{1}{B-1}\sum_{b=1}^B (Y_b(x)-\widehat{E}[x])^2
 
 where :math:`\widehat{E}[x]= \frac{1}{B}\sum_{b=1}^B Y_b(x)`.
 """
 from __future__ import annotations
 
-from numpy import ndarray
+from typing import Callable
+
+from numpy.typing import NDArray
 
 from gemseo_mlearning.adaptive.criterion import MLDataAcquisitionCriterion
 
 
 class Variance(MLDataAcquisitionCriterion):
     """Variance of the regression model.
 
     This criterion is scaled by the output range.
     """
 
-    def _get_func(self):
-        def func(input_data: ndarray) -> float:
+    def _get_func(self) -> Callable[[NDArray[float]], float]:
+        def func(input_data: NDArray[float]) -> float:
             """Evaluation function.
 
             Args:
                 input_data: The model input data.
 
             Returns:
                 The acquisition criterion value.
             """
             variance = self.algo_distribution.compute_variance(input_data)
-            return variance / self.output_range**2
+            return variance / self._scaling_factor**2
 
         return func
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/criterion.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/criterion.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,24 +26,25 @@
 This notion of acquisition criterion is implemented through the
 :class:`.MLDataAcquisitionCriterion` class which is built from a
 :class:`.MLSupervisedAlgo` and inherits from :class:`.MDOFunction`.
 """
 from __future__ import annotations
 
 from abc import abstractmethod
-from typing import Any
 from typing import Callable
 from typing import ClassVar
 
-from gemseo.core.factory import Factory
+from gemseo.core.base_factory import BaseFactory
 from gemseo.core.mdofunctions.mdo_function import MDOFunction
 from numpy import ndarray
 
 from gemseo_mlearning.adaptive.distribution import MLRegressorDistribution
 
+MLDataAcquisitionCriterionOptionType = float
+
 
 class MLDataAcquisitionCriterion(MDOFunction):
     """Acquisition criterion."""
 
     algo_distribution: MLRegressorDistribution
     """The distribution of a machine learning algorithm assessor."""
 
@@ -51,28 +52,36 @@
     """The output range."""
 
     MAXIMIZE: ClassVar[bool] = True
 
     def __init__(
         self,
         algo_distribution: MLRegressorDistribution,
-        **options: Any,
+        **options: MLDataAcquisitionCriterionOptionType,
     ) -> None:
         """# noqa: D205 D212 D415
         Args:
             algo_distribution: The distribution of a machine learning algorithm.
             **options: The acquisition criterion options.
         """
         self.algo_distribution = algo_distribution
         dataset = self.algo_distribution.learning_set
-        data = dataset.get_data_by_group(dataset.OUTPUT_GROUP)
+        data = dataset.get_view(group_names=dataset.OUTPUT_GROUP).to_numpy()
         self.output_range = data.max() - data.min()
         func = self._get_func()
         super().__init__(func, func.__name__, jac=self._get_jac())
 
+    @property
+    def _scaling_factor(self) -> float:
+        """The factor to scale values in the output space."""
+        if self.output_range == 0:
+            return 1.0
+
+        return self.output_range
+
     @abstractmethod
     def _get_func(self) -> Callable:
         """Build the evaluation function.
 
         Returns:
             The evaluation function.
         """
@@ -111,46 +120,17 @@
     def __mul__(self, other: MDOFunction | float) -> MDOFunction:
         new_criterion = super().__mul__(other)
         new_criterion.algo_distribution = self.algo_distribution
         new_criterion.output_range = self.output_range
         return new_criterion
 
 
-class MLDataAcquisitionCriterionFactory:
+class MLDataAcquisitionCriterionFactory(BaseFactory):
     """A factory of :class:`.MLDataAcquisitionCriterion`."""
 
-    def __init__(self) -> None:  # noqa: D205 D415 D107
-        self.__factory = Factory(
-            MLDataAcquisitionCriterion, ("gemseo_mlearning.adaptive.criteria",)
-        )
-
-    def create(
-        self, criterion: str, algo_distribution: MLRegressorDistribution, **options: Any
-    ) -> MLDataAcquisitionCriterion:
-        """Create a :class:`.MLDataAcquisitionCriterion`.
-
-        Args:
-            criterion: A name of data acquisition criterion.
-                (its class name).
-            algo_distribution: The distribution
-                of a machine learning algorithm.
-            **options: The acquisition criterion options.
-
-        Returns:
-            An acquisition criterion.
-        """
-        return self.__factory.create(
-            criterion, algo_distribution=algo_distribution, **options
-        )
-
-    def is_available(self, name: str) -> bool:
-        """Check if a name is an available acquisition criterion.
-
-        Args:
-            name: The name to check.
-        """
-        return self.__factory.is_available(name)
+    _CLASS = MLDataAcquisitionCriterion
+    _MODULE_NAMES = ("gemseo_mlearning.adaptive.criteria",)
 
     @property
     def available_criteria(self) -> list[str]:
         """The names of the available criteria."""
-        return self.__factory.classes
+        return self.class_names
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/distribution.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,16 @@
     MLDataAcquisitionCriterionFactory
 """
 from __future__ import annotations
 
 import logging
 from abc import abstractmethod
 
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
+from gemseo.datasets.io_dataset import IODataset
 from gemseo.mlearning.core.ml_algo import DataType
 from gemseo.mlearning.regression import regression
 from gemseo.mlearning.regression.regression import MLRegressionAlgo
 from gemseo.utils.metaclasses import ABCGoogleDocstringInheritanceMeta
 from numpy import ndarray
 
 LOGGER = logging.getLogger(__name__)
@@ -101,15 +102,15 @@
         self._samples = []
         self._transform_input_group = self.algo._transform_input_group
         self._transform_output_group = self.algo._transform_output_group
         self._input_variables_to_transform = self.algo._input_variables_to_transform
         self._output_variables_to_transform = self.algo._output_variables_to_transform
 
     @property
-    def learning_set(self) -> Dataset:
+    def learning_set(self) -> IODataset:
         """The learning dataset used by the original machine learning algorithm."""
         return self.algo.learning_set
 
     @property
     def input_names(self) -> list[str]:
         """The names of the original machine learning algorithm inputs."""
         return self.algo.input_names
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/distributions/__init__.py` & `gemseo-mlearning-1.1.0/tests/adaptive/distributions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-"""The distributions of machine learning algorithms."""
+"""Tests for the distributions of regression algorithms."""
 from __future__ import annotations
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/distributions/kriging_distribution.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/distributions/kriging_distribution.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/adaptive/distributions/regressor_distribution.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/adaptive/distributions/regressor_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,21 +33,21 @@
 - etc.
 """
 from __future__ import annotations
 
 import logging
 from typing import Callable
 from typing import ClassVar
+from typing import Final
 
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
 from gemseo.mlearning.core.ml_algo import DataType
 from gemseo.mlearning.regression import regression
 from gemseo.mlearning.regression.regression import MLRegressionAlgo
 from gemseo.utils.data_conversion import concatenate_dict_of_arrays_to_array
-from gemseo.utils.python_compatibility import Final
 from numpy import array
 from numpy import array_split
 from numpy import atleast_2d
 from numpy import delete as npdelete
 from numpy import dot
 from numpy import exp
 from numpy import maximum
@@ -157,15 +157,17 @@
         Args:
             indices: The indices of the samples
                 removed from the learning dataset during the training phase.
 
         Returns:
             The weight function returning a weight from a 1D input array.
         """
-        dat = self.learning_set.get_data_by_group(self.learning_set.INPUT_GROUP)
+        dat = self.learning_set.get_view(
+            group_names=self.learning_set.INPUT_GROUP
+        ).to_numpy()
         all_indices = set(self._samples)
         rho = max(
             min(euclidean(dat[id1], dat[id2]) for id2 in all_indices - {id1})
             for id1 in all_indices
         )
         in_grp = self.learning_set.INPUT_GROUP
 
@@ -184,15 +186,17 @@
                 input_data = concatenate_dict_of_arrays_to_array(
                     input_data, self.input_names
                 )
             only_one_element = input_data.ndim == 1
             input_data = atleast_2d(input_data)
             distance = ones(input_data.shape[0])
             for index in indices:
-                index_data = self.learning_set.get_data_by_group(in_grp)[index]
+                index_data = self.learning_set.get_view(group_names=in_grp).to_numpy()[
+                    index
+                ]
                 for index, value in enumerate(input_data):
                     term = 1 - exp(-euclidean(index_data, value) ** 2 / rho**2)
                     distance[index] *= term
             if only_one_element:
                 distance = distance[0]
             return distance
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/api.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 from __future__ import annotations
 
 from typing import Any
 from typing import Iterable
 from typing import Mapping
 from typing import Sequence
 
+from gemseo import create_scenario
 from gemseo.algos.design_space import DesignSpace
-from gemseo.algos.doe.doe_lib import DOELibrary
-from gemseo.algos.doe.doe_lib import DOELibraryOptionType
-from gemseo.api import create_scenario
-from gemseo.core.dataset import Dataset
+from gemseo.algos.doe.doe_library import DOELibrary
+from gemseo.algos.doe.doe_library import DOELibraryOptionType
 from gemseo.core.discipline import MDODiscipline
 from gemseo.core.scenario import Scenario
+from gemseo.datasets.dataset import Dataset
 
 
 def sample_discipline(
     discipline: MDODiscipline,
     input_space: DesignSpace,
     output_names: str | Iterable[str],
     algo_name: str,
@@ -113,10 +113,8 @@
         {
             Scenario.ALGO: algo_name,
             DOELibrary.N_SAMPLES: n_samples,
             Scenario.ALGO_OPTIONS: algo_options,
         }
     )
 
-    return scenario.formulation.opt_problem.export_to_dataset(
-        name=name, opt_naming=False
-    )
+    return scenario.formulation.opt_problem.to_dataset(name=name, opt_naming=False)
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/quality_measures/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/quality_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/quality_measures/mae_measure.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/quality_measures/mae_measure.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     \operatorname{MAE}(\hat{y})=\frac{1}{n}\sum_{i=1}^n\|\hat{y}_i-y_i\|,
 
 where :math:`\hat{y}` are the predictions and :math:`y` are the data points.
 """
 from __future__ import annotations
 
-from gemseo.mlearning.qual_measure.error_measure import MLErrorMeasure
+from gemseo.mlearning.quality_measures.error_measure import MLErrorMeasure
 from gemseo.mlearning.regression.regression import MLRegressionAlgo
 from numpy import ndarray
 from sklearn.metrics import mean_absolute_error
 
 
 class MAEMeasure(MLErrorMeasure):
     """The mean absolute error measure for machine learning."""
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/quality_measures/me_measure.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/quality_measures/me_measure.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     \operatorname{ME}(\hat{y})=\max_{1\leq i \leq n}\|\hat{y}_i-y_i\|,
 
 where :math:`\hat{y}` are the predictions and :math:`y` are the data points.
 """
 from __future__ import annotations
 
-from gemseo.mlearning.qual_measure.error_measure import MLErrorMeasure
+from gemseo.mlearning.quality_measures.error_measure import MLErrorMeasure
 from gemseo.mlearning.regression.regression import MLRegressionAlgo
 from numpy import ndarray
 
 
 class MEMeasure(MLErrorMeasure):
     """The maximum error measure for machine learning."""
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/__init__.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/gradient_boosting.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/gradient_boosting.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,22 +22,23 @@
 The gradient boosting model relies on the ``GradientBoostingRegressor`` class
 of the `scikit-learn library <https://scikit-learn.org/stable/modules/
 generated/sklearn.ensemble.GradientBoostingRegressor.html>`_.
 """
 from __future__ import annotations
 
 import logging
+from typing import Any
 from typing import ClassVar
+from typing import Final
 from typing import Iterable
 from typing import Mapping
 
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
 from gemseo.mlearning.core.ml_algo import TransformerType
 from gemseo.mlearning.regression.regression import MLRegressionAlgo
-from gemseo.utils.python_compatibility import Final
 from numpy import array
 from numpy import ndarray
 from sklearn.ensemble import GradientBoostingRegressor as SKLGradientBoosting
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -50,15 +51,15 @@
     def __init__(
         self,
         data: Dataset,
         transformer: Mapping[str, TransformerType] | None = None,
         input_names: Iterable[str] = None,
         output_names: Iterable[str] = None,
         n_estimators: int = 100,
-        **parameters,
+        **parameters: Any,
     ) -> None:
         """# noqa: D205 D212 D415
         Args:
             n_estimators: The number of boosting stages to perform.
         """
         super().__init__(
             data,
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/mlp.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/mlp.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,23 +17,24 @@
 #                         documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Interface to the OpenTURNS' multilayer perceptron (MLP)."""
 from __future__ import annotations
 
 import logging
+from typing import Any
 from typing import ClassVar
+from typing import Final
 from typing import Iterable
 from typing import Mapping
 
 import sklearn.neural_network
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
 from gemseo.mlearning.core.ml_algo import TransformerType
 from gemseo.mlearning.regression.regression import MLRegressionAlgo
-from gemseo.utils.python_compatibility import Final
 from numpy import ndarray
 
 LOGGER = logging.getLogger(__name__)
 
 
 class MLPRegressor(MLRegressionAlgo):
     """MultiLayer perceptron (MLP)."""
@@ -44,15 +45,15 @@
     def __init__(
         self,
         data: Dataset,
         transformer: Mapping[str, TransformerType] | None = None,
         input_names: Iterable[str] = None,
         output_names: Iterable[str] = None,
         hidden_layer_sizes: tuple[int] = (100,),
-        **parameters,
+        **parameters: Any,
     ) -> None:
         """# noqa: D205 D212 D415
         Args:
             hidden_layer_sizes: The number of neurons per hidden layer.
         """
         super().__init__(
             data,
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/ot_gpr.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/ot_gpr.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,34 +12,37 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Gaussian process regression model from OpenTURNS."""
 from __future__ import annotations
 
 from typing import ClassVar
+from typing import Final
 from typing import Iterable
 
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
 from gemseo.mlearning.core.ml_algo import DataType
 from gemseo.mlearning.core.ml_algo import TransformerType
 from gemseo.mlearning.regression.regression import MLRegressionAlgo
 from gemseo.utils.data_conversion import (
     concatenate_dict_of_arrays_to_array,
 )
-from gemseo.utils.python_compatibility import Final
 from numpy import array
 from numpy import atleast_2d
 from numpy import diag
 from numpy import ndarray
 from openturns import ConstantBasisFactory
 from openturns import KrigingAlgorithm
+from openturns import LinearBasisFactory
 from openturns import Point
+from openturns import QuadraticBasisFactory
 from openturns import ResourceMap
 from openturns import SquaredExponential
 from openturns import TensorizedCovarianceModel
+from strenum import StrEnum
 
 
 class OTGaussianProcessRegressor(MLRegressionAlgo):
     """Gaussian process regression model from OpenTURNS."""
 
     LIBRARY: Final[str] = "OpenTURNS"
     SHORT_ALGO_NAME: ClassVar[str] = "GPR"
@@ -58,37 +61,58 @@
 
     HMATRIX_RECOMPRESSION_EPSILON: ClassVar[float] = 1e-4
     """The epsilon used for the recompression of the H-matrix.
 
     Used when ``use_hmat`` is ``True``.
     """
 
+    class TrendType(StrEnum):
+        """The trend type of the Gaussian process regressor."""
+
+        CONSTANT = "constant"
+        LINEAR = "linear"
+        QUADRATIC = "quadratic"
+
+    __TREND_TYPES_TO_FACTORIES: Final[dict[str, type]] = {
+        TrendType.CONSTANT: ConstantBasisFactory,
+        TrendType.LINEAR: LinearBasisFactory,
+        TrendType.QUADRATIC: QuadraticBasisFactory,
+    }
+
+    __use_hmat: bool
+    """Whether to use the HMAT or LAPACK as linear algebra method."""
+
+    __trend_type: TrendType
+    """The type of the trend."""
+
     def __init__(
         self,
         data: Dataset,
         transformer: TransformerType | None = None,
         input_names: Iterable[str] = None,
         output_names: Iterable[str] = None,
         use_hmat: bool = None,
+        trend_type: TrendType = TrendType.CONSTANT,
     ) -> None:
         """# noqa: D205 D212 D415
         Args:
             use_hmat: Whether to use the HMAT or LAPACK as linear algebra method.
                 If ``None``,
                 use HMAT when the learning size is greater
                 than :attr:`MAX_SIZE_FOR_LAPACK`.
+            trend_type: The type of the trend.
         """
         super().__init__(
             data,
             transformer=transformer,
             input_names=input_names,
             output_names=output_names,
             use_hmat=use_hmat,
         )
-        self.__use_hmat = None
+        self.__trend_type = trend_type
         if use_hmat is None:
             self.use_hmat = len(data) > self.MAX_SIZE_FOR_LAPACK
         else:
             self.use_hmat = use_hmat
 
     @property
     def use_hmat(self) -> bool:
@@ -122,15 +146,15 @@
         else:
             covariance_model = TensorizedCovarianceModel(covariance_models)
 
         algo = KrigingAlgorithm(
             input_data,
             output_data,
             covariance_model,
-            ConstantBasisFactory(input_dimension).build(),
+            self.__TREND_TYPES_TO_FACTORIES[self.__trend_type](input_dimension).build(),
         )
         algo.run()
         self.algo = algo.getResult()
 
     def _predict(self, input_data: ndarray) -> ndarray:
         return atleast_2d(self.algo.getConditionalMean(input_data))
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/regressor_chain.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/regressor_chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,32 @@
 # Contributors:
 #    INITIAL AUTHORS - initial API and implementation and/or initial
 #                         documentation
 #        :author: Matthias
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """A model chaining regression models.
 
-During the training stage,
-the first regression model learns the learning dataset,
-the second regression model learns the learning error of the first regression model,
-and the $i$-th regression model learns the learning error of its predecessor.
-
-During the prediction stage,
-the different regression models are evaluated from a new input data
-and the sum of their output data is returned.
+During the training stage, the first regression model learns the learning dataset, the
+second regression model learns the learning error of the first regression model, and the
+$i$-th regression model learns the learning error of its predecessor.
+
+During the prediction stage, the different regression models are evaluated from a new
+input data and the sum of their output data is returned.
 """
 from __future__ import annotations
 
 import logging
 from collections import namedtuple
+from typing import Any
 from typing import ClassVar
 from typing import Iterable
 from typing import Mapping
 
-from gemseo.core.dataset import Dataset
-from gemseo.mlearning.api import create_regression_model
+from gemseo.datasets.dataset import Dataset
+from gemseo.mlearning import create_regression_model
 from gemseo.mlearning.core.ml_algo import TransformerType
 from gemseo.mlearning.regression.regression import MLRegressionAlgo
 from numpy import ndarray
 
 LOGGER = logging.getLogger(__name__)
 
 _AlgoDefinition = namedtuple("AlgoDefinition", "name,transformer,parameters")
@@ -54,30 +53,30 @@
 
     def __init__(  # noqa: D107
         self,
         data: Dataset,
         transformer: Mapping[str, TransformerType] | None = None,
         input_names: Iterable[str] = None,
         output_names: Iterable[str] = None,
-        **parameters,
+        **parameters: Any,
     ) -> None:
         super().__init__(
             data,
             transformer=transformer,
             input_names=input_names,
             output_names=output_names,
             **parameters,
         )
         self.__algos = []
 
     def add_algo(
         self,
         name: str,
         transformer: Mapping[str, TransformerType] | None = None,
-        **parameters,
+        **parameters: Any,
     ) -> None:
         """Add a new regression algorithm in the chain.
 
         Args:
             name: The name of the regression algorithm.
             transformer: The strategies to transform the variables.
                 The values are instances of :class:`.Transformer`
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/svm.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/svm.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 # Contributors:
 #    INITIAL AUTHORS - initial API and implementation and/or initial
 #                         documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 """Support vector machine for regression.
 
-The support vector machine model relies on the ``SVR`` class of the `scikit-learn
-library <https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html>`_.
+The support vector machine model relies on the :class:`SVR` class of ``sklearn``.
 """
 from __future__ import annotations
 
 import logging
+from typing import Any
 from typing import ClassVar
+from typing import Final
 from typing import Iterable
 from typing import Mapping
 
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
 from gemseo.mlearning.core.ml_algo import TransformerType
 from gemseo.mlearning.regression.regression import MLRegressionAlgo
-from gemseo.utils.python_compatibility import Final
 from numpy import array
 from numpy import ndarray
 from sklearn.svm import SVR
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -46,23 +46,23 @@
     LIBRARY: Final[str] = "scikit-learn"
     SHORT_ALGO_NAME: ClassVar[str] = "SVMRegression"
 
     def __init__(
         self,
         data: Dataset,
         transformer: Mapping[str, TransformerType] | None = None,
-        input_names: Iterable[str] = None,
-        output_names: Iterable[str] = None,
+        input_names: Iterable[str] | None = None,
+        output_names: Iterable[str] | None = None,
         kernel: str = "rbf",
-        **parameters,
+        **parameters: Any,
     ) -> None:
-        """# noqa: D205 D212 D415
+        """
         Args:
             kernel: The kernel type to be used.
-        """
+        """  # noqa: D205 D212 D415
         super().__init__(
             data,
             transformer=transformer,
             input_names=input_names,
             output_names=output_names,
             kernel=kernel,
             **parameters,
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning/regression/thin_plate_spline.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/regression/thin_plate_spline.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import logging
 from typing import Any
 from typing import Callable
 from typing import ClassVar
 from typing import Iterable
 from typing import Mapping
 
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.dataset import Dataset
 from gemseo.mlearning.core.ml_algo import TransformerType
 from gemseo.mlearning.regression.rbf import RBFRegressor
 from numpy import ndarray
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -51,12 +51,12 @@
         **parameters: Any,
     ) -> None:
         super().__init__(
             data,
             transformer=transformer,
             input_names=input_names,
             output_names=output_names,
-            function=RBFRegressor.THIN_PLATE,
+            function=RBFRegressor.Function.THIN_PLATE,
             smooth=smooth,
             norm=norm,
             **parameters,
         )
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning.egg-info/PKG-INFO` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: gemseo-mlearning
-Version: 1.0.1
+Version: 1.1.0
 Summary: Miscellaneous machine learning capabilities.
 Home-page: https://gitlab.com/gemseo
 Author: Matthias De Lozzo
 Author-email: contact@gemseo.org
 License: GNU Lesser General Public License v3
 Project-URL: Source, https://gitlab.com/gemseo/dev/gemseo-mlearning
 Project-URL: Tracker, https://gitlab.com/gemseo/dev/gemseo-mlearning/-/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.7
+Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE.txt
 License-File: CREDITS.rst
 
 ..
     Copyright 2021 IRT Saint Exupéry, https://www.irt-saintexupery.com
```

### Comparing `gemseo-mlearning-1.0.1/src/gemseo_mlearning.egg-info/SOURCES.txt` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -22,28 +22,29 @@
 doc_src/examples/mlearning/adaptive/plot_ego_cv_boot.py
 doc_src/examples/mlearning/adaptive/plot_ego_krig.py
 doc_src/examples/mlearning/adaptive/plot_ego_rosenbrock.py
 doc_src/examples/mlearning/adaptive/plot_limit_state.py
 doc_src/examples/mlearning/api/README.rst
 doc_src/examples/mlearning/api/plot_sample_discipline.py
 doc_src/examples/mlearning/api/plot_sample_disciplines.py
+doc_src/examples/optimization/plot_sbo_rastrigin.py
 requirements/check.in
 requirements/check.txt
 requirements/dist.in
 requirements/dist.txt
 requirements/doc.txt
 requirements/test-python3.10.txt
-requirements/test-python3.7.txt
 requirements/test-python3.8.txt
 requirements/test-python3.9.txt
 src/gemseo_mlearning/__init__.py
 src/gemseo_mlearning/api.py
 src/gemseo_mlearning.egg-info/PKG-INFO
 src/gemseo_mlearning.egg-info/SOURCES.txt
 src/gemseo_mlearning.egg-info/dependency_links.txt
+src/gemseo_mlearning.egg-info/entry_points.txt
 src/gemseo_mlearning.egg-info/requires.txt
 src/gemseo_mlearning.egg-info/top_level.txt
 src/gemseo_mlearning/adaptive/__init__.py
 src/gemseo_mlearning/adaptive/acquisition.py
 src/gemseo_mlearning/adaptive/criterion.py
 src/gemseo_mlearning/adaptive/distribution.py
 src/gemseo_mlearning/adaptive/criteria/__init__.py
@@ -64,14 +65,20 @@
 src/gemseo_mlearning/adaptive/criteria/value/__init__.py
 src/gemseo_mlearning/adaptive/criteria/value/criterion.py
 src/gemseo_mlearning/adaptive/criteria/variance/__init__.py
 src/gemseo_mlearning/adaptive/criteria/variance/criterion.py
 src/gemseo_mlearning/adaptive/distributions/__init__.py
 src/gemseo_mlearning/adaptive/distributions/kriging_distribution.py
 src/gemseo_mlearning/adaptive/distributions/regressor_distribution.py
+src/gemseo_mlearning/algos/__init__.py
+src/gemseo_mlearning/algos/opt/__init__.py
+src/gemseo_mlearning/algos/opt/lib_surrogate_based.py
+src/gemseo_mlearning/algos/opt/core/__init__.py
+src/gemseo_mlearning/algos/opt/core/surrogate_based.py
+src/gemseo_mlearning/algos/opt/options/SBO_options.json
 src/gemseo_mlearning/quality_measures/__init__.py
 src/gemseo_mlearning/quality_measures/mae_measure.py
 src/gemseo_mlearning/quality_measures/me_measure.py
 src/gemseo_mlearning/regression/__init__.py
 src/gemseo_mlearning/regression/gradient_boosting.py
 src/gemseo_mlearning/regression/mlp.py
 src/gemseo_mlearning/regression/ot_gpr.py
@@ -82,19 +89,25 @@
 tests/conftest.py
 tests/test_api.py
 tests/adaptive/__init__.py
 tests/adaptive/conftest.py
 tests/adaptive/test_acquisition.py
 tests/adaptive/test_criteria.py
 tests/adaptive/test_criterion.py
-tests/distributions/__init__.py
-tests/distributions/conftest.py
-tests/distributions/test_distribution.py
-tests/distributions/test_kriging_distribution.py
-tests/distributions/test_regressor_distribution.py
+tests/adaptive/distributions/__init__.py
+tests/adaptive/distributions/conftest.py
+tests/adaptive/distributions/test_distribution.py
+tests/adaptive/distributions/test_get_regressor_distribution.py
+tests/adaptive/distributions/test_kriging_distribution.py
+tests/adaptive/distributions/test_regressor_distribution.py
+tests/algos/__init__.py
+tests/algos/opt/__init__.py
+tests/algos/opt/test_surrogate_based_algos.py
+tests/algos/opt/core/__init__.py
+tests/algos/opt/core/test_surrogate_based.py
 tests/quality_measures/__init__.py
 tests/quality_measures/test_mae_measure.py
 tests/quality_measures/test_me_measure.py
 tests/regression/__init__.py
 tests/regression/conftest.py
 tests/regression/test_gradient_boosting.py
 tests/regression/test_mlp.py
```

### Comparing `gemseo-mlearning-1.0.1/tests/__init__.py` & `gemseo-mlearning-1.1.0/tests/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+from __future__ import annotations
```

### Comparing `gemseo-mlearning-1.0.1/tests/adaptive/__init__.py` & `gemseo-mlearning-1.1.0/tests/adaptive/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/tests/adaptive/conftest.py` & `gemseo-mlearning-1.1.0/tests/adaptive/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,23 +15,24 @@
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 from __future__ import annotations
 
 import pytest
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.io_dataset import IODataset
 from numpy import array
 
 
 @pytest.fixture(scope="module")
-def dataset() -> Dataset:
+def dataset() -> IODataset:
     """A learning dataset."""
-    dataset = Dataset()
-    dataset.add_variable("x", array([0.0, 1.0])[:, None], group=dataset.INPUT_GROUP)
+    dataset = IODataset()
+    dataset.add_variable(
+        "x", array([0.0, 1.0])[:, None], group_name=dataset.INPUT_GROUP
+    )
     dataset.add_variable(
         "y",
         array([1.0, 2.0])[:, None],
-        group=dataset.OUTPUT_GROUP,
-        cache_as_input=False,
+        group_name=dataset.OUTPUT_GROUP,
     )
     return dataset
```

### Comparing `gemseo-mlearning-1.0.1/tests/adaptive/test_acquisition.py` & `gemseo-mlearning-1.1.0/tests/adaptive/test_acquisition.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,35 +19,36 @@
 from __future__ import annotations
 
 from operator import eq
 
 import pytest
 from gemseo.algos.design_space import DesignSpace
 from gemseo.algos.opt_problem import OptimizationProblem
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.io_dataset import IODataset
 from gemseo.disciplines.analytic import AnalyticDiscipline
 from gemseo.mlearning.regression.linreg import LinearRegressor
 from gemseo_mlearning.adaptive.acquisition import MLDataAcquisition
 from gemseo_mlearning.adaptive.distributions.regressor_distribution import (
     RegressorDistribution,
 )
 from numpy import array
 from numpy import ndarray
 
 
 @pytest.fixture(scope="module")
-def dataset() -> Dataset:
+def dataset() -> IODataset:
     """A learning dataset."""
-    dataset = Dataset()
-    dataset.add_variable("x", array([0.0, 1.0])[:, None], group=dataset.INPUT_GROUP)
+    dataset = IODataset()
+    dataset.add_variable(
+        "x", array([0.0, 1.0])[:, None], group_name=dataset.INPUT_GROUP
+    )
     dataset.add_variable(
         "y",
         array([1.0, 2.0])[:, None],
-        group=dataset.OUTPUT_GROUP,
-        cache_as_input=False,
+        group_name=dataset.OUTPUT_GROUP,
     )
     return dataset
 
 
 @pytest.fixture(scope="module")
 def algo_distribution_for_update(dataset) -> RegressorDistribution:
     """The distribution of a linear regression model to be updated."""
@@ -77,34 +78,33 @@
     acquisition = MLDataAcquisition(
         "ExpectedImprovement", input_space, algo_distribution
     )
     assert acquisition._MLDataAcquisition__algo_name == acquisition.default_algo_name
     assert (
         acquisition._MLDataAcquisition__algo_options == acquisition.default_opt_options
     )
-    assert acquisition._MLDataAcquisition__problem.design_space.variables_names == ["x"]
+    assert acquisition._MLDataAcquisition__problem.design_space.variable_names == ["x"]
     assert acquisition._MLDataAcquisition__criterion == "ExpectedImprovement"
     assert acquisition._MLDataAcquisition__input_space == input_space
     assert acquisition._MLDataAcquisition__distribution == algo_distribution
     assert acquisition._MLDataAcquisition__algo.algo_name == "NLOPT_COBYLA"
 
 
 def test_init_with_bad_output_dimension(input_space):
     """Check MLDataAcquisition initialization raising errors.
 
     The initialization should raise a NotImplementedError when the output dimension of
     the algorithm is greater than 1.
     """
-    dataset = Dataset()
-    dataset.add_variable("x", array([[0.0], [1.0]]), group=dataset.INPUT_GROUP)
+    dataset = IODataset()
+    dataset.add_variable("x", array([[0.0], [1.0]]), group_name=dataset.INPUT_GROUP)
     dataset.add_variable(
         "y",
         array([[1.0, 1.0], [2.0, 2.0]]),
-        group=dataset.OUTPUT_GROUP,
-        cache_as_input=False,
+        group_name=dataset.OUTPUT_GROUP,
     )
     algo = LinearRegressor(dataset)
     algo.learn()
     algo_distribution = RegressorDistribution(algo, size=3)
     with pytest.raises(
         NotImplementedError, match="MLDataAcquisition works only with scalar output."
     ):
@@ -190,11 +190,11 @@
 ):
     """Check that the optimization problem can use approximated or analytic Jacobian."""
     acquisition = MLDataAcquisition(criterion, input_space, algo_distribution)
     acquisition._MLDataAcquisition__build_optimization_problem()
     assert (
         eq(
             acquisition._MLDataAcquisition__problem.differentiation_method,
-            OptimizationProblem.FINITE_DIFFERENCES,
+            OptimizationProblem.DifferentiationMethod.FINITE_DIFFERENCES,
         )
         == use_finite_differences
     )
```

### Comparing `gemseo-mlearning-1.0.1/tests/adaptive/test_criteria.py` & `gemseo-mlearning-1.1.0/tests/adaptive/test_criteria.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 from __future__ import annotations
 
 import pytest
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.io_dataset import IODataset
 from gemseo.mlearning.regression.linreg import LinearRegressor
-from gemseo.utils.pytest_conftest import concretize_classes
+from gemseo.utils.testing.helpers import concretize_classes
 from gemseo_mlearning.adaptive.criteria.distances.criterion_min import (
     MinimumDistance,
 )
 from gemseo_mlearning.adaptive.criteria.expectation.criterion import Expectation
 from gemseo_mlearning.adaptive.criteria.mean_std.criterion import MeanSigma
 from gemseo_mlearning.adaptive.criteria.optimum.criterion import (
     ExpectedImprovement,
@@ -49,23 +49,22 @@
 
 @pytest.fixture(scope="module")
 def algo_distribution() -> MLRegressorDistribution:
     """A mock distribution of a regression model.
 
     This distribution uses mocks for the methods compute_variance and compute_mean.
     """
-    dataset = Dataset()
+    dataset = IODataset()
     dataset.add_variable(
-        "x", array([0.0, 0.5, 1.0])[:, None], group=dataset.INPUT_GROUP
+        "x", array([0.0, 0.5, 1.0])[:, None], group_name=dataset.INPUT_GROUP
     )
     dataset.add_variable(
         "y",
         array([1.0, 0.0, 1.0])[:, None],
-        group=dataset.OUTPUT_GROUP,
-        cache_as_input=False,
+        group_name=dataset.OUTPUT_GROUP,
     )
     with concretize_classes(MLRegressorDistribution):
         distribution = MLRegressorDistribution(LinearRegressor(dataset))
 
     distribution.learn()
     distribution.compute_variance = lambda input_data: 2 * input_data
     distribution.compute_mean = lambda input_data: 3 * input_data
@@ -93,34 +92,34 @@
     criterion = StandardDeviation(algo_distribution)
     assert criterion(value) * criterion.output_range == expected_std
 
 
 def test_expected_improvement(algo_distribution):
     """Check the criterion ExpectedImprovement."""
     value = array([0.0])
-    minimum = algo_distribution.learning_set["y"].min()
+    minimum = algo_distribution.learning_set.get_view(variable_names="y").min()
     criterion = ExpectedImprovement(algo_distribution)
     expected = algo_distribution.compute_expected_improvement(value, minimum)
     assert criterion(value) * criterion.output_range == expected
 
 
 def test_expected_improvement_for_minimum(algo_distribution):
     """Check the criterion MinExpectedImprovement."""
     value = array([0.0])
-    minimum = algo_distribution.learning_set["y"].min()
+    minimum = algo_distribution.learning_set.get_view(variable_names="y").min()
     criterion = MinExpectedImprovement(algo_distribution)
     expected = algo_distribution.compute_expected_improvement(value, minimum)
     assert criterion(value) * criterion.output_range == expected
 
 
 def test_expected_improvement_for_maximum(algo_distribution):
     """Check the criterion MinExpectedImprovement."""
     value = array([0.0])
     criterion = MaxExpectedImprovement(algo_distribution)
-    maximum = algo_distribution.learning_set["y"].max()
+    maximum = algo_distribution.learning_set.get_view(variable_names="y").max()
     expected = algo_distribution.compute_expected_improvement(value, maximum, True)
     assert criterion(value) * criterion.output_range == expected
 
 
 def test_expectation(algo_distribution):
     """Check the criterion Expectation."""
     value = array([0.5])
@@ -157,14 +156,16 @@
     criterion = LimitState(algo_distribution, limit_state)
     assert criterion(value) == expected
 
 
 def test_quantile(algo_distribution):
     """Check the criterion Quantile."""
     level = 0.8
-    quantile_ = quantile(algo_distribution.learning_set["y"], level)
+    quantile_ = quantile(
+        algo_distribution.learning_set.get_view(variable_names="y"), level
+    )
     value = array([0.25])
     mean = algo_distribution.compute_mean(value)
     std = algo_distribution.compute_standard_deviation(value)
     expected = abs(quantile_ - mean) / std
     criterion = Quantile(algo_distribution, level)
     assert criterion(value) == expected
```

### Comparing `gemseo-mlearning-1.0.1/tests/adaptive/test_criterion.py` & `gemseo-mlearning-1.1.0/tests/adaptive/test_criterion.py`

 * *Files 7% similar despite different names*

```diff
@@ -48,15 +48,17 @@
     distribution.learn()
     return distribution
 
 
 def test_factory(algo_distribution):
     """Check the MLDataAcquisitionCriterionFactory."""
     factory = MLDataAcquisitionCriterionFactory()
-    criterion = factory.create("ExpectedImprovement", algo_distribution)
+    criterion = factory.create(
+        "ExpectedImprovement", algo_distribution=algo_distribution
+    )
     assert isinstance(criterion, ExpectedImprovement)
     assert "ExpectedImprovement" in factory.available_criteria
     assert factory.is_available("ExpectedImprovement")
 
 
 @pytest.fixture(scope="module")
 def criterion_1(algo_distribution):
@@ -100,7 +102,17 @@
     """Check that a combination of MLDataAcquisitionCriterion is an MDOFunction."""
     criterion_1 = ExpectedImprovement(algo_distribution)
     criterion_2 = MinimumDistance(algo_distribution)
     criterion_3 = criterion_1 * 0.2 + criterion_2 * 0.8
     assert isinstance(criterion_3, MDOFunction)
     x_new = array([0.5])
     assert criterion_3(x_new) == criterion_1(x_new) * 0.2 + criterion_2(x_new) * 0.8
+
+
+def test_scaling_factor(dataset, algo_distribution):
+    """Check that the scaling factor is updated with the output range."""
+    criterion = ExpectedImprovement(algo_distribution)
+    assert criterion._scaling_factor == 1.0
+    criterion.output_range = 2.0
+    assert criterion._scaling_factor == 2.0
+    criterion.output_range = 0.0
+    assert criterion._scaling_factor == 1.0
```

### Comparing `gemseo-mlearning-1.0.1/tests/conftest.py` & `gemseo-mlearning-1.1.0/src/gemseo_mlearning/algos/opt/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,11 +8,13 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
-"""Test helpers."""
+"""Wrappers for optimization algorithms."""
 from __future__ import annotations
 
-from gemseo.utils.pytest_conftest import *  # noqa: F401 F403
+from typing import Union
+
+OptimizationLibraryOptionType = Union[str, int, float]
```

### Comparing `gemseo-mlearning-1.0.1/tests/distributions/__init__.py` & `gemseo-mlearning-1.1.0/tests/quality_measures/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/tests/distributions/conftest.py` & `gemseo-mlearning-1.1.0/tests/adaptive/distributions/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -15,25 +15,40 @@
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 from __future__ import annotations
 
 import pytest
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.io_dataset import IODataset
+from gemseo.mlearning.regression.gpr import GaussianProcessRegressor
+from gemseo.mlearning.regression.linreg import LinearRegressor
 from numpy import array
 
 
 @pytest.fixture(scope="module")
-def dataset() -> Dataset:
+def dataset() -> IODataset:
     """A learning dataset with three samples."""
-    dataset = Dataset()
+    dataset = IODataset()
     dataset.add_variable(
-        "x", array([0.0, 0.5, 1.0])[:, None], group=dataset.INPUT_GROUP
+        "x", array([0.0, 0.5, 1.0])[:, None], group_name=dataset.INPUT_GROUP
     )
     dataset.add_variable(
         "y",
         array([1.0, 0.0, 1.0])[:, None],
-        group=dataset.OUTPUT_GROUP,
-        cache_as_input=False,
+        group_name=dataset.OUTPUT_GROUP,
     )
     return dataset
+
+
+@pytest.fixture(scope="module")
+def linear_algo(dataset) -> LinearRegressor:
+    """A linear regression model used in different tests."""
+    model = LinearRegressor(dataset)
+    model.learn()
+    return model
+
+
+@pytest.fixture(scope="module")
+def kriging_algo(dataset) -> GaussianProcessRegressor:
+    """A Kriging regression model used in different tests."""
+    return GaussianProcessRegressor(dataset)
```

### Comparing `gemseo-mlearning-1.0.1/tests/distributions/test_distribution.py` & `gemseo-mlearning-1.1.0/tests/adaptive/distributions/test_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # Contributors:
 #    INITIAL AUTHORS - API and implementation and/or documentation
 #        :author: Matthias De Lozzo
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 from __future__ import annotations
 
 import pytest
-from gemseo.core.dataset import Dataset
+from gemseo.datasets.io_dataset import IODataset
 from gemseo.mlearning.regression.linreg import LinearRegressor
 from gemseo.mlearning.regression.rbf import RBFRegressor
-from gemseo.utils.pytest_conftest import concretize_classes
+from gemseo.utils.testing.helpers import concretize_classes
 from gemseo_mlearning.adaptive.distribution import MLRegressorDistribution
 from gemseo_mlearning.adaptive.distributions.regressor_distribution import (
     RegressorDistribution,
 )
 from numpy import array
 from numpy import linspace
 from numpy import newaxis
@@ -51,18 +51,18 @@
     distribution.compute_variance = lambda input_data: input_data
     return distribution
 
 
 @pytest.fixture(scope="module")
 def distribution_with_transformers() -> RegressorDistribution:
     """The distribution of an algorithm using variable transformation."""
-    dataset = Dataset()
+    dataset = IODataset()
     x = linspace(-1, 1, 10)[:, None]
-    dataset.add_variable("x", x, group=dataset.INPUT_GROUP)
-    dataset.add_variable("y", x**2, group=dataset.OUTPUT_GROUP)
+    dataset.add_variable("x", x, group_name=dataset.INPUT_GROUP)
+    dataset.add_variable("y", x**2, group_name=dataset.OUTPUT_GROUP)
 
     algo = RBFRegressor(dataset, transformer=RBFRegressor.DEFAULT_TRANSFORMER)
 
     distribution = RegressorDistribution(algo)
     distribution.learn()
     return distribution
 
@@ -75,15 +75,15 @@
     """
     assert isinstance(distribution.algo, LinearRegressor)
     assert distribution._samples == []
 
 
 def test_learning_set(distribution):
     """Check the property ``learning_set``."""
-    assert isinstance(distribution.learning_set, Dataset)
+    assert isinstance(distribution.learning_set, IODataset)
 
 
 def test_inputs_names(distribution):
     """Check the property 'input_names'.
 
     Must be equal to the names of the inputs of the regression algorithm.
     """
@@ -160,23 +160,22 @@
 
 
 def test_change_learning_set(dataset):
     """Check that changing the learning set updates the algorithm."""
     with concretize_classes(MLRegressorDistribution):
         distribution = MLRegressorDistribution(LinearRegressor(dataset))
 
-    new_dataset = Dataset()
+    new_dataset = IODataset()
     new_dataset.add_variable(
-        "x", array([0.0, 1.0])[:, None], group=new_dataset.INPUT_GROUP
+        "x", array([0.0, 1.0])[:, None], group_name=new_dataset.INPUT_GROUP
     )
     new_dataset.add_variable(
         "y",
         array([1.0, 1.0])[:, None],
-        group=new_dataset.OUTPUT_GROUP,
-        cache_as_input=False,
+        group_name=new_dataset.OUTPUT_GROUP,
     )
     distribution.change_learning_set(new_dataset)
     assert len(distribution.learning_set) == 2
     assert distribution.predict(array([0.5])) == array([1.0])
 
 
 @pytest.mark.parametrize("as_dict", [False, True])
```

### Comparing `gemseo-mlearning-1.0.1/tests/distributions/test_kriging_distribution.py` & `gemseo-mlearning-1.1.0/tests/adaptive/distributions/test_kriging_distribution.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,30 +23,24 @@
 from gemseo_mlearning.adaptive.distributions.kriging_distribution import (
     KrigingDistribution,
 )
 from numpy import array
 
 
 @pytest.fixture(scope="module")
-def algo(dataset) -> GaussianProcessRegressor:
-    """A Kriging regression model used in different tests."""
-    return GaussianProcessRegressor(dataset)
-
-
-@pytest.fixture(scope="module")
-def distribution(algo: GaussianProcessRegressor) -> KrigingDistribution:
+def distribution(kriging_algo: GaussianProcessRegressor) -> KrigingDistribution:
     """The distribution of the Kriging regression model."""
-    distribution = KrigingDistribution(algo)
+    distribution = KrigingDistribution(kriging_algo)
     distribution.learn()
     return distribution
 
 
-def test_init(algo):
+def test_init(kriging_algo):
     """Check the initialization of the distribution."""
-    assert KrigingDistribution(algo).algo == algo
+    assert KrigingDistribution(kriging_algo).algo == kriging_algo
 
 
 @pytest.mark.parametrize(
     "point",
     [
         array([0.0]),
         array([0.5]),
```

### Comparing `gemseo-mlearning-1.0.1/tests/distributions/test_regressor_distribution.py` & `gemseo-mlearning-1.1.0/tests/adaptive/distributions/test_regressor_distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,55 +24,47 @@
     RegressorDistribution,
 )
 from numpy import array
 from numpy import exp
 from numpy import quantile
 
 
-@pytest.fixture(scope="module")
-def algo(dataset) -> LinearRegressor:
-    """A linear regression model used in different tests."""
-    model = LinearRegressor(dataset)
-    model.learn()
-    return model
-
-
 def __weight_func(value, indices):
     terms = [
         1 - exp(-((value - 0.0) ** 2) / 0.5**2),
         1 - exp(-((value - 0.5) ** 2) / 0.5**2),
         1 - exp(-((value - 1.0) ** 2) / 0.5**2),
     ]
     result = 1
     for index in indices:
         result *= terms[index]
     return result
 
 
 @pytest.fixture(scope="module")
-def distribution(algo) -> RegressorDistribution:
+def distribution(linear_algo) -> RegressorDistribution:
     """The distribution of the linear regression model."""
-    distribution = RegressorDistribution(algo, bootstrap=False, loo=True)
+    distribution = RegressorDistribution(linear_algo, bootstrap=False, loo=True)
     distribution.learn()
     return distribution
 
 
 @pytest.mark.parametrize(
     "bootstrap,loo,size",
     [
         (True, False, None),
         (True, False, 3),
         (False, False, None),
         (False, False, 3),
         (False, True, None),
     ],
 )
-def test_init(algo, bootstrap, loo, size):
+def test_init(linear_algo, bootstrap, loo, size):
     """Check the initialization of the distribution."""
-    distribution = RegressorDistribution(algo, bootstrap, loo, size)
+    distribution = RegressorDistribution(linear_algo, bootstrap, loo, size)
     if bootstrap:
         assert distribution.method == distribution.BOOTSTRAP
         assert distribution.size == size or distribution.N_BOOTSTRAP
     elif loo:
         assert distribution.method == distribution.LOO
         assert distribution.size == len(distribution.learning_set)
     else:
```

### Comparing `gemseo-mlearning-1.0.1/tests/quality_measures/__init__.py` & `gemseo-mlearning-1.1.0/tests/regression/__init__.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/tests/quality_measures/test_mae_measure.py` & `gemseo-mlearning-1.1.0/tests/quality_measures/test_mae_measure.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/tests/quality_measures/test_me_measure.py` & `gemseo-mlearning-1.1.0/tests/quality_measures/test_me_measure.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/tests/regression/__init__.py` & `gemseo-mlearning-1.1.0/tests/algos/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
+"""Tests for the algorithms."""
 from __future__ import annotations
```

### Comparing `gemseo-mlearning-1.0.1/tests/regression/conftest.py` & `gemseo-mlearning-1.1.0/tests/regression/conftest.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,41 +16,56 @@
 #    INITIAL AUTHORS - initial API and implementation and/or initial
 #                         documentation
 #        :author: Matthias
 #    OTHER AUTHORS   - MACROSCOPIC CHANGES
 from __future__ import annotations
 
 import pytest
-from gemseo.core.dataset import Dataset
-from gemseo.problems.dataset.rosenbrock import RosenbrockDataset
+from gemseo.datasets.io_dataset import IODataset
+from gemseo.problems.dataset.rosenbrock import create_rosenbrock_dataset
 from numpy import hstack
 from numpy import ndarray
 
 
 @pytest.fixture(scope="module")
-def dataset() -> RosenbrockDataset:
+def dataset() -> IODataset:
     """The Rosenbrock dataset."""
-    return RosenbrockDataset(opt_naming=False)
+    return create_rosenbrock_dataset(opt_naming=False)
 
 
 @pytest.fixture(scope="module")
-def dataset_2(dataset) -> RosenbrockDataset:
+def dataset_2(dataset) -> IODataset:
     """The Rosenbrock dataset with 2d-output."""
-    data = Dataset()
-    data.add_variable("x", dataset["x"], group=data.INPUT_GROUP)
-    data.add_variable("rosen", dataset["rosen"], group=data.OUTPUT_GROUP)
+    data = IODataset()
     data.add_variable(
-        "rosen2", hstack((dataset["rosen"], dataset["rosen"])), group=data.OUTPUT_GROUP
+        "x",
+        dataset.get_view(variable_names="x").to_numpy(),
+        group_name=data.INPUT_GROUP,
+    )
+    data.add_variable(
+        "rosen",
+        dataset.get_view(variable_names="rosen").to_numpy(),
+        group_name=data.OUTPUT_GROUP,
+    )
+    data.add_variable(
+        "rosen2",
+        hstack(
+            (
+                dataset.get_view(variable_names="rosen").to_numpy(),
+                dataset.get_view(variable_names="rosen").to_numpy(),
+            )
+        ),
+        group_name=data.OUTPUT_GROUP,
     )
     return data
 
 
 @pytest.fixture(scope="module")
-def input_data(dataset) -> ndarray:
+def input_data(dataset: IODataset) -> ndarray:
     """The learning input data."""
-    return dataset.get_data_by_group(dataset.INPUT_GROUP)
+    return dataset.get_view(group_names=dataset.INPUT_GROUP).to_numpy()
 
 
 @pytest.fixture(scope="module")
-def output_data(dataset) -> ndarray:
+def output_data(dataset: IODataset) -> ndarray:
     """The learning output data."""
-    return dataset.get_data_by_group(dataset.OUTPUT_GROUP)
+    return dataset.get_view(group_names=dataset.OUTPUT_GROUP).to_numpy()
```

### Comparing `gemseo-mlearning-1.0.1/tests/regression/test_gradient_boosting.py` & `gemseo-mlearning-1.1.0/tests/regression/test_gradient_boosting.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/tests/regression/test_mlp.py` & `gemseo-mlearning-1.1.0/tests/regression/test_mlp.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/tests/regression/test_ot_gpr.py` & `gemseo-mlearning-1.1.0/tests/regression/test_ot_gpr.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 """Test the interface to the OpenTURNS' Kriging."""
 from __future__ import annotations
 
 import pytest
-from gemseo.api import execute_algo
-from gemseo.core.dataset import Dataset
+from gemseo import execute_algo
 from gemseo.core.mdofunctions.mdo_function import MDOFunction
+from gemseo.datasets.io_dataset import IODataset
 from gemseo.problems.analytical.rosenbrock import Rosenbrock
 from gemseo_mlearning.regression.ot_gpr import OTGaussianProcessRegressor
 from numpy import array
 from numpy import hstack
 from numpy import ndarray
 from numpy import zeros
 from numpy.testing import assert_allclose
@@ -53,27 +53,34 @@
     """The Rosenbrock problem with an observable summing the inputs."""
     rosenbrock = Rosenbrock()
     rosenbrock.add_observable(MDOFunction(func, "sum"))
     return rosenbrock
 
 
 @pytest.fixture(scope="module")
-def dataset(problem) -> Dataset:
+def dataset(problem) -> IODataset:
     """A 9-length full-factorial sampling of the Rosenbrock problem."""
     execute_algo(problem, "fullfact", n_samples=9, algo_type="doe")
-    return problem.export_to_dataset(opt_naming=False)
+    return problem.to_dataset(opt_naming=False)
 
 
 @pytest.fixture(scope="module")
-def dataset_2(problem) -> Dataset:
+def dataset_2(problem) -> IODataset:
     """A 9-length full-factorial sampling of the Rosenbrock problem."""
     execute_algo(problem, "fullfact", n_samples=9, algo_type="doe")
-    data = problem.export_to_dataset(opt_naming=False)
+    data = problem.to_dataset(opt_naming=False)
     data.add_variable(
-        "rosen2", hstack((data["rosen"], -data["rosen"])), group=data.OUTPUT_GROUP
+        "rosen2",
+        hstack(
+            (
+                data.get_view(variable_names="rosen").to_numpy(),
+                -data.get_view(variable_names="rosen").to_numpy(),
+            )
+        ),
+        group_name=data.OUTPUT_GROUP,
     )
     return data
 
 
 @pytest.fixture(scope="module")
 def kriging(dataset) -> OTGaussianProcessRegressor:
     """A Kriging model trained on the Rosenbrock dataset."""
@@ -94,19 +101,21 @@
         (1, False),
         (OTGaussianProcessRegressor.MAX_SIZE_FOR_LAPACK, False),
         (OTGaussianProcessRegressor.MAX_SIZE_FOR_LAPACK + 1, True),
     ],
 )
 def test_kriging_use_hmat_default(n_samples, use_hmat):
     """Check the default library (LAPACK or HMAT) according to the sample size."""
-    dataset = Dataset()
-    dataset.set_from_array(
+    dataset = IODataset.from_array(
         zeros((n_samples, 2)),
-        variables=["in", "out"],
-        groups={"in": Dataset.INPUT_GROUP, "out": Dataset.OUTPUT_GROUP},
+        variable_names=["in", "out"],
+        variable_names_to_group_names={
+            "in": IODataset.INPUT_GROUP,
+            "out": IODataset.OUTPUT_GROUP,
+        },
     )
     assert OTGaussianProcessRegressor(dataset).use_hmat is use_hmat
 
 
 @pytest.mark.parametrize("use_hmat", [True, False])
 def test_kriging_use_hmat(dataset, use_hmat):
     """Check that the HMAT can be specified at initialization or after."""
@@ -119,15 +128,17 @@
     assert kriging.use_hmat is not use_hmat
 
 
 def test_kriging_predict_on_learning_set(dataset):
     """Check that the Kriging interpolates the learning set."""
     kriging = OTGaussianProcessRegressor(dataset)
     kriging.learn()
-    for x in kriging.learning_set.get_data_by_group(Dataset.INPUT_GROUP):
+    for x in kriging.learning_set.get_view(
+        group_names=IODataset.INPUT_GROUP
+    ).to_numpy():
         prediction = kriging.predict({"x": x})
         assert_allclose(prediction["sum"], sum(x), atol=1e-3)
         assert_allclose(prediction["rosen"], rosen(x))
 
 
 @pytest.mark.parametrize("x1", [-1, 1])
 @pytest.mark.parametrize("x2", [-1, 1])
@@ -145,15 +156,17 @@
 def test_kriging_predict_std_on_learning_set(transformer, dataset):
     """Check that the Kriging interpolates the learning set.
 
     The standard deviation should be equal to zero.
     """
     kriging = OTGaussianProcessRegressor(dataset, transformer=transformer)
     kriging.learn()
-    for x in kriging.learning_set.get_data_by_group(Dataset.INPUT_GROUP):
+    for x in kriging.learning_set.get_view(
+        group_names=IODataset.INPUT_GROUP
+    ).to_numpy():
         predicted_std = kriging.predict_std(x)
         assert predicted_std[0] == pytest.approx(0.0, abs=1e-1)
         assert predicted_std[1] == pytest.approx(0.0, abs=1e-1)
 
 
 @pytest.mark.parametrize("x1", [-1, 1])
 @pytest.mark.parametrize("x2", [-1, 1])
@@ -196,7 +209,22 @@
         one_sample = input_data.ndim == 1
     if one_sample:
         shape = (ndim,)
     else:
         shape = (1, ndim)
 
     assert model.predict_std(input_data).shape == shape
+
+
+@pytest.mark.parametrize(
+    "trend_type,shape",
+    [
+        (OTGaussianProcessRegressor.TrendType.CONSTANT, (2, 1)),
+        (OTGaussianProcessRegressor.TrendType.LINEAR, (2, 3)),
+        (OTGaussianProcessRegressor.TrendType.QUADRATIC, (2, 6)),
+    ],
+)
+def test_trend_type(dataset, trend_type, shape):
+    """Check the trend type of the Gaussian process regressor."""
+    model = OTGaussianProcessRegressor(dataset, trend_type=trend_type)
+    model.learn()
+    assert array(model.algo.getTrendCoefficients()).shape == shape
```

### Comparing `gemseo-mlearning-1.0.1/tests/regression/test_regressor_chain.py` & `gemseo-mlearning-1.1.0/tests/regression/test_regressor_chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 
 import pytest
-from gemseo.mlearning.qual_measure.mse_measure import MSEMeasure
+from gemseo.mlearning.quality_measures.mse_measure import MSEMeasure
 from gemseo.mlearning.regression.linreg import LinearRegressor
 from gemseo.mlearning.regression.polyreg import PolynomialRegressor
 from gemseo_mlearning.regression.regressor_chain import RegressorChain
 from numpy import array
 from numpy.testing import assert_equal
```

### Comparing `gemseo-mlearning-1.0.1/tests/regression/test_svm.py` & `gemseo-mlearning-1.1.0/tests/regression/test_svm.py`

 * *Files identical despite different names*

### Comparing `gemseo-mlearning-1.0.1/tests/regression/test_thin_plate_spline.py` & `gemseo-mlearning-1.1.0/tests/regression/test_thin_plate_spline.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 def test_init(dataset):
     """Check the default initialization of a TPSRegressor."""
     algo = TPSRegressor(dataset)
     algo.learn()
     assert isinstance(algo, RBFRegressor)
-    assert algo.algo.function == RBFRegressor.THIN_PLATE
+    assert algo.algo.function == algo.Function.THIN_PLATE
     assert algo.algo.smooth == 0.0
     assert algo.algo.norm == "euclidean"
 
 
 def test_init_custom(dataset):
     """Check the custom initialization of a TPSRegressor."""
     algo = TPSRegressor(dataset, norm="minkowski", smooth=0.1)
```

### Comparing `gemseo-mlearning-1.0.1/tox.ini` & `gemseo-mlearning-1.1.0/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     pytest {env:__COVERAGE_POSARGS:} {posargs}
 
 [testenv:check]
 description = run code formatting and checking
 basepython = python3.9
 deps = -r requirements/check.txt
 skip_install = true
-whitelist_externals =
-    git
+whitelist_externals = pre-commit
 commands =
     pre-commit install
     pre-commit run --all-files
 
 [testenv:doc]
 description = build documentation
 basepython = python3.9
@@ -66,35 +65,38 @@
 whitelist_externals = rm
 commands =
     rm -rf dist build
     python -m build
     twine check dist/*
     python setup.py check --metadata
 
-[testenv:pypi-py{37,38,39,310}]
+[testenv:pypi-py{38,39,310}]
 description = test the pypi distribution
 deps = gemseo-mlearning[test]
 skip_install = true
 
 [testenv:update-deps-{doc,dist,check}]
 description = update the non test envs dependencies
 basepython = python3.9
 extras =
     doc: {[testenv:doc]extras}
 setenv =
 passenv =
 deps = pip-tools
 skip_install = true
+whitelist_externals =
+    pip-compile
+    check: pre-commit
 commands =
     doc: pip-compile --upgrade --upgrade-package {[deps]gemseo} --extra doc -o requirements/doc.txt
     dist: pip-compile --upgrade requirements/dist.in
     check: pip-compile --upgrade requirements/check.in
     check: pre-commit autoupdate
 
-[testenv:update-deps-test-py{37,38,39,310}]
+[testenv:update-deps-test-py{38,39,310}]
 description = update the test envs dependencies
 extras = {[testenv]extras}
 setenv =
 passenv =
 deps = pip-tools
 skip_install = true
 commands =
```

