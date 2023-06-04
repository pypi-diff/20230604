# Comparing `tmp/bayesianbandits-0.3.0.tar.gz` & `tmp/bayesianbandits-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayesianbandits-0.3.0.tar", max compression
+gzip compressed data, was "bayesianbandits-0.3.1.tar", max compression
```

## Comparing `bayesianbandits-0.3.0.tar` & `bayesianbandits-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1074 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/LICENSE
--rw-r--r--   0        0        0     1093 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/README.md
--rw-r--r--   0        0        0     2740 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/__init__.py
--rw-r--r--   0        0        0     3681 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_arm.py
--rw-r--r--   0        0        0    18168 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_basebandit.py
--rw-r--r--   0        0        0    28409 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_estimators.py
--rw-r--r--   0        0        0     1304 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_np_utils.py
--rw-r--r--   0        0        0     5122 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_policy_decorators.py
--rw-r--r--   0        0        0     2655 2023-06-02 18:56:02.801498 bayesianbandits-0.3.0/bayesianbandits/_typing.py
--rw-r--r--   0        0        0      705 2023-06-02 18:56:02.805498 bayesianbandits-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1093 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/README.md
+-rw-r--r--   0        0        0     2740 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/__init__.py
+-rw-r--r--   0        0        0     3848 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_arm.py
+-rw-r--r--   0        0        0    18314 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_basebandit.py
+-rw-r--r--   0        0        0    28409 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_estimators.py
+-rw-r--r--   0        0        0     1304 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_np_utils.py
+-rw-r--r--   0        0        0     5122 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_policy_decorators.py
+-rw-r--r--   0        0        0     2655 2023-06-04 16:59:06.097209 bayesianbandits-0.3.1/bayesianbandits/_typing.py
+-rw-r--r--   0        0        0      705 2023-06-04 16:59:06.101209 bayesianbandits-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 bayesianbandits-0.3.1/PKG-INFO
```

### Comparing `bayesianbandits-0.3.0/LICENSE` & `bayesianbandits-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.0/README.md` & `bayesianbandits-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.0/bayesianbandits/__init__.py` & `bayesianbandits-0.3.1/bayesianbandits/__init__.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.0/bayesianbandits/_arm.py` & `bayesianbandits-0.3.1/bayesianbandits/_arm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from __future__ import annotations
-from typing import Callable, Dict, Optional, TypeVar, cast, Any
-
+from functools import wraps
+from typing import Callable, Optional, TypeVar, cast, Any
+from typing_extensions import ParamSpec, Concatenate
 import numpy as np
 from numpy.typing import ArrayLike, NDArray
 
 from ._typing import DecayingLearner, Learner, ActionToken
 
-
-R = TypeVar("R")
+P = ParamSpec("P")
+R = TypeVar("R", covariant=True)
 
 
-def requires_learner(func: Callable[..., R]) -> Callable[..., R]:
+def requires_learner(
+    func: Callable[Concatenate[Arm, P], R]
+) -> Callable[Concatenate[Arm, P], R]:
     """Decorator to check if the arm has a learner set."""
 
-    def wrapper(self: Arm, *args: Any, **kwargs: Dict[str, Any]):
+    @wraps(func)
+    def wrapper(self: "Arm", *args: P.args, **kwargs: P.kwargs) -> R:
         if self.learner is None:
             raise ValueError("Learner is not set.")
         return func(self, *args, **kwargs)
 
     return wrapper
```

### Comparing `bayesianbandits-0.3.0/bayesianbandits/_basebandit.py` & `bayesianbandits-0.3.1/bayesianbandits/_basebandit.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,15 +392,15 @@
         """
         if X is None and self._contextual:
             raise ValueError("X must be an array-like for a contextual bandit.")
         elif X is not None and not self._contextual:
             raise ValueError("X must be None for a non-contextual bandit.")
 
         if not self._contextual:
-            X_decay = np.array([[1]])
+            X_decay = np.array([[1]], dtype=float)
         else:
             assert X is not None  # for the type checker
             X_decay = np.atleast_2d(X)
 
         for arm in self.arms.values():
             if decay_last_arm or arm is not self.last_arm_pulled:
                 arm.decay(X_decay, decay_rate=decay_rate)
@@ -413,23 +413,28 @@
 
         self.rng = np.random.default_rng(self.rng)
         self._contextual = False
 
         # initialize the arms with copies of the learner and
         # point the learner rng to the bandit rng
         for arm in self.arms.values():
-            arm.learner = cast(Learner, clone(self.learner))  # type: ignore
-            arm.learner.set_params(random_state=self.rng)
+            self._set_learner(arm)
 
         if ArmProtocol not in self.__annotations__.values():
             raise ValueError(
                 "A bandit must have at least one arm. "
                 "Add an arm to the class definition."
             )
 
+    def _set_learner(self, arm: ArmProtocol) -> None:
+        """Set the learner for an arm, if it is not already set."""
+        if arm.learner is None:
+            arm.learner = clone(self.learner)  # type: ignore
+            arm.learner.set_params(random_state=self.rng)
+
     def __setstate__(self, state: Dict[str, Any]) -> None:
         """Set the state of the bandit.
 
         This method is called by pickle when loading a bandit from disk.
         This implementation ensures that arms that are no longer defined
         are deleted and arms that are newly defined are initialized, while
         preserving the state of the arms that are still defined.
@@ -453,15 +458,15 @@
 
         # initialize arms that are newly defined
         for arm_name, _ in currently_defined_arms.items():
             if arm_name not in self.arms:
                 new_arm = self.__class__.__dataclass_fields__[
                     arm_name
                 ].default_factory()
-                new_arm.learner = cast(Learner, clone(self.learner))  # type: ignore
+                self._set_learner(new_arm)
                 setattr(self, arm_name, new_arm)  # type: ignore
                 self.arms[arm_name] = self.__dict__[arm_name]
 
     @cached_property
     def arms(self: BanditProtocol) -> Dict[str, ArmProtocol]:
         return {
             name: attr
```

### Comparing `bayesianbandits-0.3.0/bayesianbandits/_estimators.py` & `bayesianbandits-0.3.1/bayesianbandits/_estimators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.0/bayesianbandits/_np_utils.py` & `bayesianbandits-0.3.1/bayesianbandits/_np_utils.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.0/bayesianbandits/_policy_decorators.py` & `bayesianbandits-0.3.1/bayesianbandits/_policy_decorators.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.0/bayesianbandits/_typing.py` & `bayesianbandits-0.3.1/bayesianbandits/_typing.py`

 * *Files identical despite different names*

### Comparing `bayesianbandits-0.3.0/pyproject.toml` & `bayesianbandits-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bayesianbandits"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Rishi Kulkarni <rishi@kulkarni.science>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9, <3.12"
 scipy = "^1.10.0"
```

### Comparing `bayesianbandits-0.3.0/PKG-INFO` & `bayesianbandits-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bayesianbandits
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Rishi Kulkarni
 Author-email: rishi@kulkarni.science
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

