# Comparing `tmp/autogluon.core-0.7.1b20230602.tar.gz` & `tmp/autogluon.core-0.7.1b20230603.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.7.1b20230602.tar", last modified: Fri Jun  2 09:03:43 2023, max compression
+gzip compressed data, was "autogluon.core-0.7.1b20230603.tar", last modified: Sat Jun  3 09:03:38 2023, max compression
```

## Comparing `autogluon.core-0.7.1b20230602.tar` & `autogluon.core-0.7.1b20230603.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.249253 autogluon.core-0.7.1b20230602/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-06-02 09:03:43.249253 autogluon.core-0.7.1b20230602/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 09:03:43.249253 autogluon.core-0.7.1b20230602/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.237252 autogluon.core-0.7.1b20230602/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.237252 autogluon.core-0.7.1b20230602/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    29675 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    94023 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59425 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3789 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.245252 autogluon.core-0.7.1b20230602/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   169723 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.249253 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.249253 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.249253 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-02 09:03:27.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-02 09:03:43.000000 autogluon.core-0.7.1b20230602/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 09:03:43.241253 autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12631 2023-06-02 09:03:43.000000 autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-02 09:03:43.000000 autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:03:43.000000 autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:03:43.000000 autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-02 09:03:43.000000 autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-02 09:03:43.000000 autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 09:03:43.000000 autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.088597 autogluon.core-0.7.1b20230603/
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-03 09:03:38.088597 autogluon.core-0.7.1b20230603/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 09:03:38.088597 autogluon.core-0.7.1b20230603/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.076597 autogluon.core-0.7.1b20230603/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.076597 autogluon.core-0.7.1b20230603/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29675 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94023 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.080597 autogluon.core-0.7.1b20230603/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.084596 autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59916 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12762 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.084596 autogluon.core-0.7.1b20230603/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.084596 autogluon.core-0.7.1b20230603/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.084596 autogluon.core-0.7.1b20230603/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.084596 autogluon.core-0.7.1b20230603/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.084596 autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.084596 autogluon.core-0.7.1b20230603/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.084596 autogluon.core-0.7.1b20230603/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.084596 autogluon.core-0.7.1b20230603/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   169723 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.088597 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.088597 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.088597 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49348 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-03 09:03:22.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-03 09:03:37.000000 autogluon.core-0.7.1b20230603/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 09:03:38.076597 autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12599 2023-06-03 09:03:38.000000 autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-03 09:03:38.000000 autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:38.000000 autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 09:03:38.000000 autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-03 09:03:38.000000 autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-03 09:03:38.000000 autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 09:03:38.000000 autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.7.1b20230602/PKG-INFO` & `autogluon.core-0.7.1b20230603/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230602
+Version: 0.7.1b20230603
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -43,27 +43,27 @@
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
         
         | AutoGluon Task      |                                                                                Quickstart                                                                                |                                                                                API                                                                                |
         |:--------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#module-0)                 |
-        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.multimodal.MultiModalPredictor) |
-        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.timeseries.TimeSeriesPredictor) |
+        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.tabular.TabularPredictor.html)                 |
+        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.multimodal.MultiModalPredictor.html) |
+        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.timeseries.TimeSeriesPredictor.html) |
         
         ## Resources
         
-        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for [documentation](https://auto.gluon.ai/stable/api/index.html) and instructions on:
+        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for documentation and instructions on:
         - [Installing AutoGluon](https://auto.gluon.ai/stable/index.html#installation)
-        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html)
-          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
+        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html)
+          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular/tabular-essentials.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
         
-        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)
-        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)
+        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)
+        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)
         
         Refer to the [AutoGluon Roadmap](https://github.com/autogluon/autogluon/blob/master/ROADMAP.md) for details on upcoming features and releases.
         
         ### Scientific Publications
         - [AutoGluon-Tabular: Robust and Accurate AutoML for Structured Data](https://arxiv.org/pdf/2003.06505.pdf) (*Arxiv*, 2020)
         - [Fast, Accurate, and Simple Models for Tabular Data via Augmented Distillation](https://proceedings.neurips.cc/paper/2020/hash/62d75fb2e3075506e8837d8f55021ab1-Abstract.html) (*NeurIPS*, 2020)
         - [Multimodal AutoML on Structured Tables with Text Fields](https://openreview.net/pdf?id=OHAIVOOl7Vl) (*ICML AutoML Workshop*, 2021)
```

### Comparing `autogluon.core-0.7.1b20230602/setup.py` & `autogluon.core-0.7.1b20230603/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/__init__.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/_setup_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/augmentation/distill_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/calibrate/conformity_score.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/constants.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/data/cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/data/label_cleaner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/dataset.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/executors.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/ray_hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/ray_tune_scheduler_factory.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/ray_tune_scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/hpo/space_converter.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/learner/abstract_learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/metrics/classification_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/_utils.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/_tags.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,16 +397,21 @@
                 else:
                     logger.warning('\tWARNING: `use_child_oof` was specified but child model does not have a dedicated `get_oof_pred_proba` method. This model may have heavily overfit validation scores.')
                     self._oof_pred_proba = model_base.predict_proba(X=X)
                 self._child_oof = True
                 model_base.predict_time = time.time() - time_start_predict
                 model_base.val_score = model_base.score_with_y_pred_proba(y=y, y_pred_proba=self._oof_pred_proba)
             else:
-                logger.log(30, f'\tWARNING: Setting `self._oof_pred_proba` by predicting on train directly! '
-                               f'This is probably a bug and should be investigated...')
+                can_get_oof_from_train = self._get_tags().get('can_get_oof_from_train', False)
+                if not can_get_oof_from_train:
+                    # TODO: Consider raising an exception in v1.0 release, we don't want this happening when not intended.
+                    logger.log(30, f'\tWARNING: Setting `self._oof_pred_proba` by predicting on train directly! '
+                                   f'This is probably a bug and should be investigated...\n'
+                                   f'\tIf this is intended, set the model tag "can_get_oof_from_train" to True '
+                                   f'in `{self.__class__.__name__}._more_tags` to avoid this warning.')
                 self._oof_pred_proba = model_base.predict_proba(X=X)  # TODO: Cheater value, will be overfit to valid set
             self._oof_pred_model_repeats = np.ones(shape=len(X), dtype=np.uint8)
         model_base.reduce_memory_size(remove_fit=True, remove_info=False, requires_save=True)
         if not self.params.get('save_bag_folds', True):
             model_base.model = None
         if self.low_memory:
             self.save_child(model_base)
```

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,7 +68,15 @@
         return fi_df
 
     def _set_default_params(self):
         default_params = {'use_orig_features': False}
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
         super()._set_default_params()
+
+    def _more_tags(self):
+        """
+        This model can generate out-of-fold (oof) predictions by predicting directly on the training data.
+        This will make the result slightly overfit, but the weighted ensemble has limited degrees of freedom intentionally, making the overfitting negligible.
+        """
+        tags = {'can_get_oof_from_train': True}
+        return tags
```

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/problem_type.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/problem_type.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/ray/resources_calculator.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/local_searcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/searcher/searcher_factory.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/space.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/space.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/task/base/base_task.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/trainer/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/early_stopping.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/feature_selection.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/files.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/files.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/infer_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/miscs.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/plots.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/plots.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/time.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/time.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/utils.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.7.1b20230603/src/autogluon/core/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.7.1b20230602
+Version: 0.7.1b20230603
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
@@ -43,27 +43,27 @@
         test_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/test.csv')
         predictor = TabularPredictor(label='class').fit(train_data, time_limit=120)  # Fit models for 120s
         leaderboard = predictor.leaderboard(test_data)
         ```
         
         | AutoGluon Task      |                                                                                Quickstart                                                                                |                                                                                API                                                                                |
         |:--------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------:|
-        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#module-0)                 |
-        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.multimodal.MultiModalPredictor) |
-        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.predictor.html#autogluon.timeseries.TimeSeriesPredictor) |
+        | TabularPredictor    | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html) |                 [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.tabular.TabularPredictor.html)                 |
+        | MultiModalPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.multimodal.MultiModalPredictor.html) |
+        | TimeSeriesPredictor | [![Quick Start](https://img.shields.io/static/v1?label=&message=tutorial&color=grey)](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)            | [![API](https://img.shields.io/badge/api-reference-blue.svg)](https://auto.gluon.ai/stable/api/autogluon.timeseries.TimeSeriesPredictor.html) |
         
         ## Resources
         
-        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for [documentation](https://auto.gluon.ai/stable/api/index.html) and instructions on:
+        See the [AutoGluon Website](https://auto.gluon.ai/stable/index.html) for documentation and instructions on:
         - [Installing AutoGluon](https://auto.gluon.ai/stable/index.html#installation)
-        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html)
-          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular_prediction/tabular-quickstart.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
+        - [Learning with tabular data](https://auto.gluon.ai/stable/tutorials/tabular/tabular-quick-start.html)
+          - [Tips to maximize accuracy](https://auto.gluon.ai/stable/tutorials/tabular/tabular-essentials.html#maximizing-predictive-performance) (if **benchmarking**, make sure to run `fit()` with argument `presets='best_quality'`).  
         
-        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/index.html)
-        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quickstart.html)
+        - [Learning with multimodal data (image, text, etc.)](https://auto.gluon.ai/stable/tutorials/multimodal/multimodal_prediction/multimodal-quick-start.html)
+        - [Learning with time series data](https://auto.gluon.ai/stable/tutorials/timeseries/forecasting-quick-start.html)
         
         Refer to the [AutoGluon Roadmap](https://github.com/autogluon/autogluon/blob/master/ROADMAP.md) for details on upcoming features and releases.
         
         ### Scientific Publications
         - [AutoGluon-Tabular: Robust and Accurate AutoML for Structured Data](https://arxiv.org/pdf/2003.06505.pdf) (*Arxiv*, 2020)
         - [Fast, Accurate, and Simple Models for Tabular Data via Augmented Distillation](https://proceedings.neurips.cc/paper/2020/hash/62d75fb2e3075506e8837d8f55021ab1-Abstract.html) (*NeurIPS*, 2020)
         - [Multimodal AutoML on Structured Tables with Text Fields](https://openreview.net/pdf?id=OHAIVOOl7Vl) (*ICML AutoML Workshop*, 2021)
```

### Comparing `autogluon.core-0.7.1b20230602/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.7.1b20230603/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

