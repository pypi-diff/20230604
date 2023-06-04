# Comparing `tmp/mleko-0.4.0.tar.gz` & `tmp/mleko-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mleko-0.4.0.tar", max compression
+gzip compressed data, was "mleko-0.4.1.tar", max compression
```

## Comparing `mleko-0.4.0.tar` & `mleko-0.4.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1073 2023-06-03 21:07:46.476830 mleko-0.4.0/LICENSE
--rw-r--r--   0        0        0     2561 2023-06-03 21:07:46.476830 mleko-0.4.0/README.md
--rw-r--r--   0        0        0     1323 2023-06-03 21:08:25.148945 mleko-0.4.0/mleko/__init__.py
--rw-r--r--   0        0        0      584 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/__init__.py
--rw-r--r--   0        0        0    11493 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/cache_mixin.py
--rw-r--r--   0        0        0      805 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/fingerprinters/__init__.py
--rw-r--r--   0        0        0     1167 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/fingerprinters/base_fingerprinter.py
--rw-r--r--   0        0        0     2843 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/fingerprinters/csv_fingerprinter.py
--rw-r--r--   0        0        0     1233 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/fingerprinters/vaex_fingerprinter.py
--rw-r--r--   0        0        0      398 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/format/__init__.py
--rw-r--r--   0        0        0     1933 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/format/vaex_cache_format_mixin.py
--rw-r--r--   0        0        0     5974 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/cache/lru_cache_mixin.py
--rw-r--r--   0        0        0      740 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/__init__.py
--rw-r--r--   0        0        0      491 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/convert/__init__.py
--rw-r--r--   0        0        0     1435 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/convert/base_converter.py
--rw-r--r--   0        0        0    11536 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/convert/csv_to_vaex_converter.py
--rw-r--r--   0        0        0     1613 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/__init__.py
--rw-r--r--   0        0        0     5922 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/base_feature_selector.py
--rw-r--r--   0        0        0     5268 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/composite_feature_selector.py
--rw-r--r--   0        0        0     4988 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/invariance_feature_selector.py
--rw-r--r--   0        0        0     5253 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/missing_rate_feature_selector.py
--rw-r--r--   0        0        0     7083 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
--rw-r--r--   0        0        0     5506 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/feature_select/variance_feature_selector.py
--rw-r--r--   0        0        0      877 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/ingest/__init__.py
--rw-r--r--   0        0        0     2211 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/ingest/base_ingester.py
--rw-r--r--   0        0        0    18015 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/ingest/kaggle_ingester.py
--rw-r--r--   0        0        0     9632 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/ingest/s3_ingester.py
--rw-r--r--   0        0        0      679 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/split/__init__.py
--rw-r--r--   0        0        0     1394 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/split/base_splitter.py
--rw-r--r--   0        0        0     3815 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/split/expression_splitter.py
--rw-r--r--   0        0        0     5934 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/dataset/split/random_splitter.py
--rw-r--r--   0        0        0      644 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/__init__.py
--rw-r--r--   0        0        0     1420 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/data_container.py
--rw-r--r--   0        0        0     4496 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/pipeline.py
--rw-r--r--   0        0        0     3595 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/pipeline_step.py
--rw-r--r--   0        0        0      638 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/__init__.py
--rw-r--r--   0        0        0     2359 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/convert_step.py
--rw-r--r--   0        0        0     2179 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/feature_select_step.py
--rw-r--r--   0        0        0     2141 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/ingest_step.py
--rw-r--r--   0        0        0     2248 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/pipeline/steps/split_step.py
--rw-r--r--   0        0        0        0 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/py.typed
--rw-r--r--   0        0        0      765 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/utils/__init__.py
--rw-r--r--   0        0        0     4497 2023-06-03 21:07:46.480830 mleko-0.4.0/mleko/utils/custom_logger.py
--rw-r--r--   0        0        0     3430 2023-06-03 21:07:46.484830 mleko-0.4.0/mleko/utils/decorators.py
--rw-r--r--   0        0        0      742 2023-06-03 21:07:46.484830 mleko-0.4.0/mleko/utils/file_helpers.py
--rw-r--r--   0        0        0     1403 2023-06-03 21:07:46.484830 mleko-0.4.0/mleko/utils/tqdm_helpers.py
--rw-r--r--   0        0        0     2836 2023-06-03 21:07:46.484830 mleko-0.4.0/mleko/utils/vaex_helpers.py
--rw-r--r--   0        0        0     2752 2023-06-03 21:08:25.212945 mleko-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 mleko-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-04 20:58:16.253797 mleko-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2561 2023-06-04 20:58:16.253797 mleko-0.4.1/README.md
+-rw-r--r--   0        0        0     1323 2023-06-04 20:58:49.939543 mleko-0.4.1/mleko/__init__.py
+-rw-r--r--   0        0        0      584 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/__init__.py
+-rw-r--r--   0        0        0    11493 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/cache_mixin.py
+-rw-r--r--   0        0        0      805 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/fingerprinters/__init__.py
+-rw-r--r--   0        0        0     1167 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/fingerprinters/base_fingerprinter.py
+-rw-r--r--   0        0        0     2843 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/fingerprinters/csv_fingerprinter.py
+-rw-r--r--   0        0        0     1233 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/fingerprinters/vaex_fingerprinter.py
+-rw-r--r--   0        0        0      398 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/format/__init__.py
+-rw-r--r--   0        0        0     1933 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/format/vaex_cache_format_mixin.py
+-rw-r--r--   0        0        0     5974 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/cache/lru_cache_mixin.py
+-rw-r--r--   0        0        0      740 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/dataset/__init__.py
+-rw-r--r--   0        0        0      491 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/dataset/convert/__init__.py
+-rw-r--r--   0        0        0     1435 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/dataset/convert/base_converter.py
+-rw-r--r--   0        0        0    11536 2023-06-04 20:58:16.253797 mleko-0.4.1/mleko/dataset/convert/csv_to_vaex_converter.py
+-rw-r--r--   0        0        0     1613 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/__init__.py
+-rw-r--r--   0        0        0     5918 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/base_feature_selector.py
+-rw-r--r--   0        0        0     5267 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/composite_feature_selector.py
+-rw-r--r--   0        0        0     4983 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/invariance_feature_selector.py
+-rw-r--r--   0        0        0     5248 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/missing_rate_feature_selector.py
+-rw-r--r--   0        0        0     7078 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/pearson_correlation_feature_selector.py
+-rw-r--r--   0        0        0     5501 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/feature_select/variance_feature_selector.py
+-rw-r--r--   0        0        0      877 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/ingest/__init__.py
+-rw-r--r--   0        0        0     2211 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/ingest/base_ingester.py
+-rw-r--r--   0        0        0    18015 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/ingest/kaggle_ingester.py
+-rw-r--r--   0        0        0     9632 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/ingest/s3_ingester.py
+-rw-r--r--   0        0        0      679 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/split/__init__.py
+-rw-r--r--   0        0        0     1394 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/split/base_splitter.py
+-rw-r--r--   0        0        0     3815 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/split/expression_splitter.py
+-rw-r--r--   0        0        0     5934 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/dataset/split/random_splitter.py
+-rw-r--r--   0        0        0      644 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/__init__.py
+-rw-r--r--   0        0        0     1420 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/data_container.py
+-rw-r--r--   0        0        0     4496 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/pipeline.py
+-rw-r--r--   0        0        0     3595 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/pipeline_step.py
+-rw-r--r--   0        0        0      638 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/__init__.py
+-rw-r--r--   0        0        0     2359 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/convert_step.py
+-rw-r--r--   0        0        0     2179 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/feature_select_step.py
+-rw-r--r--   0        0        0     2141 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/ingest_step.py
+-rw-r--r--   0        0        0     2248 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/pipeline/steps/split_step.py
+-rw-r--r--   0        0        0        0 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/py.typed
+-rw-r--r--   0        0        0      765 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/__init__.py
+-rw-r--r--   0        0        0     4497 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/custom_logger.py
+-rw-r--r--   0        0        0     3430 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/decorators.py
+-rw-r--r--   0        0        0      742 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/file_helpers.py
+-rw-r--r--   0        0        0     1403 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/tqdm_helpers.py
+-rw-r--r--   0        0        0     2836 2023-06-04 20:58:16.257797 mleko-0.4.1/mleko/utils/vaex_helpers.py
+-rw-r--r--   0        0        0     2752 2023-06-04 20:58:49.999546 mleko-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 mleko-0.4.1/PKG-INFO
```

### Comparing `mleko-0.4.0/LICENSE` & `mleko-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/README.md` & `mleko-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/__init__.py` & `mleko-0.4.1/mleko/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 
 Each subpackage is designed to be modular and extensible, making it easy to customize and adapt the library to a wide
 range of model building processes and requirements.
 """
 from __future__ import annotations
 
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `mleko-0.4.0/mleko/cache/__init__.py` & `mleko-0.4.1/mleko/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/cache/cache_mixin.py` & `mleko-0.4.1/mleko/cache/cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/cache/fingerprinters/__init__.py` & `mleko-0.4.1/mleko/cache/fingerprinters/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/cache/fingerprinters/base_fingerprinter.py` & `mleko-0.4.1/mleko/cache/fingerprinters/base_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/cache/fingerprinters/csv_fingerprinter.py` & `mleko-0.4.1/mleko/cache/fingerprinters/csv_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/cache/fingerprinters/vaex_fingerprinter.py` & `mleko-0.4.1/mleko/cache/fingerprinters/vaex_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/cache/format/vaex_cache_format_mixin.py` & `mleko-0.4.1/mleko/cache/format/vaex_cache_format_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/cache/lru_cache_mixin.py` & `mleko-0.4.1/mleko/cache/lru_cache_mixin.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/__init__.py` & `mleko-0.4.1/mleko/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/convert/base_converter.py` & `mleko-0.4.1/mleko/dataset/convert/base_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/convert/csv_to_vaex_converter.py` & `mleko-0.4.1/mleko/dataset/convert/csv_to_vaex_converter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/feature_select/__init__.py` & `mleko-0.4.1/mleko/dataset/feature_select/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/feature_select/base_feature_selector.py` & `mleko-0.4.1/mleko/dataset/feature_select/base_feature_selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,16 @@
         if features is not None and ignore_features is not None:
             error_msg = (
                 "Both `features` and `ignore_features` have been specified. The arguments are mutually exclusive."
             )
             logger.error(error_msg)
             raise ValueError(error_msg)
 
-        self._features: frozenset[str] | None = frozenset(features) if features is not None else None
-        self._ignore_features: frozenset[str] = (
-            frozenset(ignore_features) if ignore_features is not None else frozenset()
-        )
+        self._features: tuple[str, ...] | None = tuple(features) if features is not None else None
+        self._ignore_features: tuple[str, ...] = tuple(ignore_features) if ignore_features is not None else tuple()
 
     @abstractmethod
     def select_features(self, dataframe: vaex.DataFrame, force_recompute: bool = False) -> vaex.DataFrame:
         """Selects features from the given DataFrame and returns a list of paths to the selected features.
 
         Args:
             dataframe: DataFrame from which to select features.
@@ -94,25 +92,25 @@
 
         Returns:
             DataFrame with the selected features.
         """
         raise NotImplementedError
 
     @abstractmethod
-    def _default_features(self, dataframe: vaex.DataFrame) -> frozenset[str]:
+    def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features to be used by the feature selector.
 
         Args:
             dataframe: DataFrame from which to select features.
 
         Raises:
             NotImplementedError: Must be implemented in the child class that inherits from `BaseFeatureSelector`.
 
         Returns:
-            Frozen set of feature names to be used by the feature selector.
+            Tuple of feature names to be used by the feature selector.
         """
         raise NotImplementedError
 
     @abstractmethod
     def _fingerprint(self) -> Hashable:
         """Returns a hashable object that uniquely identifies the feature selector.
 
@@ -135,9 +133,11 @@
         Args:
             dataframe: DataFrame from which to select features.
 
         Returns:
             Sorted list of feature names to be used by the feature selector.
         """
         return sorted(
-            self._default_features(dataframe) - self._ignore_features if self._features is None else self._features
+            set(self._default_features(dataframe)) - set(self._ignore_features)
+            if self._features is None
+            else self._features
         )
```

### Comparing `mleko-0.4.0/mleko/dataset/feature_select/composite_feature_selector.py` & `mleko-0.4.1/mleko/dataset/feature_select/composite_feature_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,25 +109,25 @@
                 f"Executing composite feature selection step {i+1}/{len(self._feature_selectors)}: "
                 f"{feature_selector.__class__.__name__}."
             )
             dataframe = feature_selector._select_features(dataframe).extract()
             logger.info(f"Finished composite feature selection step {i+1}/{len(self._feature_selectors)}.")
         return dataframe
 
-    def _default_features(self, dataframe: vaex.DataFrame) -> frozenset[str]:  # pragma: no cover
+    def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:  # pragma: no cover
         """Returns the default features of the DataFrame.
 
         Args:
             dataframe: DataFrame from which the default features will be extracted.
 
         Returns:
-            Set of default features.
+            Tuple of default features.
         """
         features = dataframe.get_column_names()
-        return frozenset(str(feature) for feature in features)
+        return tuple(str(feature) for feature in features)
 
     def _fingerprint(self) -> Hashable:
         """Returns the fingerprint of the feature selector.
 
         Returns:
             Fingerprint of the feature selector.
         """
```

### Comparing `mleko-0.4.0/mleko/dataset/feature_select/invariance_feature_selector.py` & `mleko-0.4.1/mleko/dataset/feature_select/invariance_feature_selector.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,25 +103,25 @@
             cardinality[feature] = column.nunique(limit=2, limit_raise=False)
 
         dropped_features = {feature for feature in features if cardinality[feature] == 1}
         logger.info(f"Dropping ({len(dropped_features)}) invariant features: {dropped_features}.")
         selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
         return get_columns(dataframe, selected_features)
 
-    def _default_features(self, dataframe: vaex.DataFrame) -> frozenset[str]:
+    def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features.
 
         Args:
             dataframe: The DataFrame to select features from.
 
         Returns:
-            The default set of features.
+            Tuple of default features.
         """
         features = dataframe.get_column_names(dtype=["bool", "string"])
-        return frozenset(str(feature) for feature in features)
+        return tuple(str(feature) for feature in features)
 
     def _fingerprint(self) -> Hashable:
         """Returns the fingerprint of the feature selector.
 
         Appends the missing rate threshold to the fingerprint.
 
         Returns:
```

### Comparing `mleko-0.4.0/mleko/dataset/feature_select/missing_rate_feature_selector.py` & `mleko-0.4.1/mleko/dataset/feature_select/missing_rate_feature_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,25 +109,25 @@
             f"Dropping ({len(dropped_features)}) features with missing rate >= {self._missing_rate_threshold}: "
             f"{dropped_features}."
         )
 
         selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
         return get_columns(dataframe, selected_features)
 
-    def _default_features(self, dataframe: vaex.DataFrame) -> frozenset[str]:
+    def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features.
 
         Args:
             dataframe: The DataFrame to select features from.
 
         Returns:
-            The default set of features.
+            Tuple of default features.
         """
         features = dataframe.get_column_names()
-        return frozenset(str(feature) for feature in features)
+        return tuple(str(feature) for feature in features)
 
     def _fingerprint(self) -> Hashable:
         """Returns the fingerprint of the feature selector.
 
         Appends the missing rate threshold to the fingerprint.
 
         Returns:
```

### Comparing `mleko-0.4.0/mleko/dataset/feature_select/pearson_correlation_feature_selector.py` & `mleko-0.4.1/mleko/dataset/feature_select/pearson_correlation_feature_selector.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,25 +148,25 @@
             f"Dropping ({len(dropped_features)}) features with correlation >= {self._correlation_threshold}: "
             f"{dropped_features}."
         )
 
         selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
         return get_columns(dataframe, selected_features)
 
-    def _default_features(self, dataframe: vaex.DataFrame) -> frozenset[str]:
+    def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features.
 
         Args:
             dataframe: The DataFrame to select features from.
 
         Returns:
-            The default set of features.
+            Tuple of default features.
         """
         features = dataframe.get_column_names(dtype="numeric")
-        return frozenset(str(feature) for feature in features)
+        return tuple(str(feature) for feature in features)
 
     def _fingerprint(self) -> Hashable:
         """Returns a hashable fingerprint of the feature selector.
 
         Append the pearson correlation threshold to the fingerprint.
 
         Returns:
```

### Comparing `mleko-0.4.0/mleko/dataset/feature_select/variance_feature_selector.py` & `mleko-0.4.1/mleko/dataset/feature_select/variance_feature_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,25 +114,25 @@
         logger.info(
             f"Dropping ({len(dropped_features)}) features with normalized variance <= {self._variance_threshold}: "
             f"{dropped_features}."
         )
         selected_features = [feature for feature in dataframe.get_column_names() if feature not in dropped_features]
         return get_columns(dataframe, selected_features)
 
-    def _default_features(self, dataframe: vaex.DataFrame) -> frozenset[str]:
+    def _default_features(self, dataframe: vaex.DataFrame) -> tuple[str, ...]:
         """Returns the default set of features.
 
         Args:
             dataframe: The DataFrame to select features from.
 
         Returns:
-            The default set of features.
+            Tuple of default features.
         """
         features = dataframe.get_column_names(dtype="numeric")
-        return frozenset(str(feature) for feature in features)
+        return tuple(str(feature) for feature in features)
 
     def _fingerprint(self) -> Hashable:
         """Returns a hashable fingerprint of the feature selector.
 
         Append the variance threshold to the fingerprint.
 
         Returns:
```

### Comparing `mleko-0.4.0/mleko/dataset/ingest/__init__.py` & `mleko-0.4.1/mleko/dataset/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/ingest/base_ingester.py` & `mleko-0.4.1/mleko/dataset/ingest/base_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/ingest/kaggle_ingester.py` & `mleko-0.4.1/mleko/dataset/ingest/kaggle_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/ingest/s3_ingester.py` & `mleko-0.4.1/mleko/dataset/ingest/s3_ingester.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/split/__init__.py` & `mleko-0.4.1/mleko/dataset/split/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/split/base_splitter.py` & `mleko-0.4.1/mleko/dataset/split/base_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/split/expression_splitter.py` & `mleko-0.4.1/mleko/dataset/split/expression_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/dataset/split/random_splitter.py` & `mleko-0.4.1/mleko/dataset/split/random_splitter.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/pipeline/__init__.py` & `mleko-0.4.1/mleko/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/pipeline/data_container.py` & `mleko-0.4.1/mleko/pipeline/data_container.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/pipeline/pipeline.py` & `mleko-0.4.1/mleko/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/pipeline/pipeline_step.py` & `mleko-0.4.1/mleko/pipeline/pipeline_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/pipeline/steps/__init__.py` & `mleko-0.4.1/mleko/pipeline/steps/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/pipeline/steps/convert_step.py` & `mleko-0.4.1/mleko/pipeline/steps/convert_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/pipeline/steps/feature_select_step.py` & `mleko-0.4.1/mleko/pipeline/steps/feature_select_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/pipeline/steps/ingest_step.py` & `mleko-0.4.1/mleko/pipeline/steps/ingest_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/pipeline/steps/split_step.py` & `mleko-0.4.1/mleko/pipeline/steps/split_step.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/utils/__init__.py` & `mleko-0.4.1/mleko/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/utils/custom_logger.py` & `mleko-0.4.1/mleko/utils/custom_logger.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/utils/decorators.py` & `mleko-0.4.1/mleko/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/utils/file_helpers.py` & `mleko-0.4.1/mleko/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/utils/tqdm_helpers.py` & `mleko-0.4.1/mleko/utils/tqdm_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/mleko/utils/vaex_helpers.py` & `mleko-0.4.1/mleko/utils/vaex_helpers.py`

 * *Files identical despite different names*

### Comparing `mleko-0.4.0/pyproject.toml` & `mleko-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mleko"
-version = "0.4.0"
+version = "0.4.1"
 description = "ML-Ekosystem"
 authors = ["Erik Båvenstrand <erik@bavenstrand.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/ErikBavenstrand/mleko"
 repository = "https://github.com/ErikBavenstrand/mleko"
 documentation = "https://mleko.readthedocs.io"
```

### Comparing `mleko-0.4.0/PKG-INFO` & `mleko-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mleko
-Version: 0.4.0
+Version: 0.4.1
 Summary: ML-Ekosystem
 Home-page: https://github.com/ErikBavenstrand/mleko
 License: MIT
 Author: Erik Båvenstrand
 Author-email: erik@bavenstrand.se
 Requires-Python: >=3.8.0,<3.11.0
 Classifier: Development Status :: 3 - Alpha
```

