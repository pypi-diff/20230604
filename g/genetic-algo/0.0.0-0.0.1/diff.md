# Comparing `tmp/genetic-algo-0.0.0.tar.gz` & `tmp/genetic-algo-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genetic-algo-0.0.0.tar", last modified: Sun Jun  4 15:27:33 2023, max compression
+gzip compressed data, was "genetic-algo-0.0.1.tar", last modified: Sun Jun  4 19:41:11 2023, max compression
```

## Comparing `genetic-algo-0.0.0.tar` & `genetic-algo-0.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 15:27:33.259584 genetic-algo-0.0.0/
--rw-rw-rw-   0        0        0      115 2023-06-04 15:27:33.000000 genetic-algo-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2066 2023-06-04 15:27:33.258587 genetic-algo-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1255 2023-05-28 10:00:20.000000 genetic-algo-0.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.0.0/build.py
-drwxrwxrwx   0        0        0        0 2023-06-04 15:27:33.241077 genetic-algo-0.0.0/genetic_algo/
--rw-rw-rw-   0        0        0     8159 2023-06-03 06:53:12.000000 genetic-algo-0.0.0/genetic_algo/attributes.py
--rw-rw-rw-   0        0        0     5518 2023-05-28 10:08:23.000000 genetic-algo-0.0.0/genetic_algo/base.py
--rw-rw-rw-   0        0        0      448 2023-06-03 06:46:07.000000 genetic-algo-0.0.0/genetic_algo/document.py
--rw-rw-rw-   0        0        0     5955 2023-06-03 06:57:31.000000 genetic-algo-0.0.0/genetic_algo/driver.py
--rw-rw-rw-   0        0        0    12195 2023-06-03 06:44:36.000000 genetic-algo-0.0.0/genetic_algo/environment.py
--rw-rw-rw-   0        0        0     3584 2023-06-03 06:42:04.000000 genetic-algo-0.0.0/genetic_algo/solution.py
-drwxrwxrwx   0        0        0        0 2023-06-04 15:27:33.257616 genetic-algo-0.0.0/genetic_algo.egg-info/
--rw-rw-rw-   0        0        0     2066 2023-06-04 15:27:33.000000 genetic-algo-0.0.0/genetic_algo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2023-06-04 15:27:33.000000 genetic-algo-0.0.0/genetic_algo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 15:27:33.000000 genetic-algo-0.0.0/genetic_algo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-04 15:27:33.000000 genetic-algo-0.0.0/genetic_algo.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-04 15:27:33.000000 genetic-algo-0.0.0/genetic_algo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      645 2023-05-29 09:34:21.000000 genetic-algo-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       20 2023-05-28 10:10:01.000000 genetic-algo-0.0.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 10:10:01.000000 genetic-algo-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 15:27:33.259584 genetic-algo-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1601 2023-05-28 10:08:04.000000 genetic-algo-0.0.0/setup.py
--rw-rw-rw-   0        0        0     2645 2023-06-03 07:02:29.000000 genetic-algo-0.0.0/test.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:41:11.043917 genetic-algo-0.0.1/
+-rw-rw-rw-   0        0        0      115 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2066 2023-06-04 19:41:11.042983 genetic-algo-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1255 2023-05-28 10:00:20.000000 genetic-algo-0.0.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:12:17.000000 genetic-algo-0.0.1/build.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:41:11.028864 genetic-algo-0.0.1/genetic_algo/
+-rw-rw-rw-   0        0        0     8793 2023-06-04 19:39:54.000000 genetic-algo-0.0.1/genetic_algo/attributes.py
+-rw-rw-rw-   0        0        0     5518 2023-05-28 10:08:23.000000 genetic-algo-0.0.1/genetic_algo/base.py
+-rw-rw-rw-   0        0        0      448 2023-06-03 06:46:07.000000 genetic-algo-0.0.1/genetic_algo/document.py
+-rw-rw-rw-   0        0        0     5955 2023-06-03 06:57:31.000000 genetic-algo-0.0.1/genetic_algo/driver.py
+-rw-rw-rw-   0        0        0    12195 2023-06-03 06:44:36.000000 genetic-algo-0.0.1/genetic_algo/environment.py
+-rw-rw-rw-   0        0        0     4988 2023-06-04 19:39:54.000000 genetic-algo-0.0.1/genetic_algo/solution.py
+drwxrwxrwx   0        0        0        0 2023-06-04 19:41:11.041406 genetic-algo-0.0.1/genetic_algo.egg-info/
+-rw-rw-rw-   0        0        0     2066 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-04 19:41:10.000000 genetic-algo-0.0.1/genetic_algo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      645 2023-06-04 19:41:03.000000 genetic-algo-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       20 2023-05-28 10:10:01.000000 genetic-algo-0.0.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 10:10:01.000000 genetic-algo-0.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 19:41:11.043917 genetic-algo-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1601 2023-06-04 19:40:33.000000 genetic-algo-0.0.1/setup.py
+-rw-rw-rw-   0        0        0     2645 2023-06-03 07:02:29.000000 genetic-algo-0.0.1/test.py
```

### Comparing `genetic-algo-0.0.0/PKG-INFO` & `genetic-algo-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.0
+Version: 0.0.1
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.0.0/README.md` & `genetic-algo-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.0/build.py` & `genetic-algo-0.0.1/build.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.0/genetic_algo/attributes.py` & `genetic-algo-0.0.1/genetic_algo/attributes.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import (
     Self, Iterable, Any, Optional, Type, Union
 )
 import string
 import random
 from abc import ABCMeta
 
-from represent import BaseModel
+from represent import BaseModel, Modifiers
 
 __all__ = [
     "Arguments",
     "Attribute",
     "NumericAttribute",
     "StringAttribute",
     "IntegerAttribute",
@@ -63,25 +63,29 @@
 
     NAME: Optional[str] = None
 
     EXCLUDED: Iterable[Any] = []
 
     arguments = Arguments()
 
+    modifiers = Modifiers(**BaseModel.modifiers)
+
+    modifiers.properties = True
+
     def __init__(self, value: Any, name: Optional[str] = None) -> None:
         """
         Defines the class attributes.
 
         :param value: The value of the attribute.
         :param name: The name of the attribute.
         """
 
         self.name = name or self.NAME
 
-        self.value = value
+        self._value = value
     # end __init__
 
     def __hash__(self) -> int:
         """
         Returns the hash of the object.
 
         :return: The hash of the object.
@@ -102,14 +106,30 @@
         return (
             (type(self) is type(other)) and
             (self.name == other.name) and
             (self.value == other.value)
         )
     # end __eq__
 
+    @property
+    def value(self) -> Any:
+        """
+        Returns the value of the attribute.
+
+        :return: The value.
+        """
+
+        if not isinstance(self._value, Attribute):
+            return self._value
+
+        else:
+            return self._value.value
+        # end if
+    # end value
+
     @classmethod
     def build(cls, *args: Any, **kwargs: Any) -> Self:
         """
         Generates the random attribute.
 
         :param args: Any positional arguments.
         :param kwargs: Any keyword arguments.
@@ -131,14 +151,24 @@
 
         :param args: Any positional arguments.
         :param kwargs: Any keyword arguments.
 
         :return: The attribute value.
         """
     # end generate
+
+    def copy(self) -> Self:
+        """
+        Copies the object.
+
+        :return: A new copy of the object.
+        """
+
+        return type(self)(value=self._value, name=self.name)
+    # end copy
 # end Attribute
 
 Number = Union[int, float]
 
 class NumericAttribute(Attribute):
     """A class to represent an attribute of a solution."""
```

### Comparing `genetic-algo-0.0.0/genetic_algo/base.py` & `genetic-algo-0.0.1/genetic_algo/base.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.0/genetic_algo/driver.py` & `genetic-algo-0.0.1/genetic_algo/driver.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.0/genetic_algo/environment.py` & `genetic-algo-0.0.1/genetic_algo/environment.py`

 * *Files identical despite different names*

### Comparing `genetic-algo-0.0.0/genetic_algo/solution.py` & `genetic-algo-0.0.1/genetic_algo/solution.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # solution.py
 
 from typing import (
-    Self, Iterable, Optional, Type, List
+    Self, Iterable, Optional, Type, List, Union
 )
 
 from represent import BaseModel
 
 from genetic_algo.attributes import Attribute
 
 __all__ = [
@@ -112,20 +112,32 @@
     return unique
 # end eliminate_repetitions
 
 class Template(BaseModel):
     """A class to represent a template for solution attributes."""
 
     SOLUTION = Solution
-    ATTRIBUTES: List[Attribute] = []
+    ATTRIBUTES: List[
+        Union[
+            Union[Attribute, Type[Attribute]],
+            Iterable[Union[Attribute, Type[Attribute]]]
+        ]
+    ] = []
 
     def __init__(
             self,
             solution: Optional[Type[Solution]] = None,
-            attributes: Optional[Iterable[Type[Attribute]]] = None
+            attributes: Optional[
+                List[
+                    Union[
+                        Union[Attribute, Type[Attribute]],
+                        Iterable[Union[Attribute, Type[Attribute]]]
+                    ]
+                ]
+            ] = None
     ) -> None:
         """
         Defines the class attributes.
 
         :param solution: The type of the solution object.
         :param attributes: The attributes of the solution.
         """
@@ -138,16 +150,48 @@
     def build(self) -> Solution:
         """
         Generates the random attribute.
 
         :return: The attribute object.
         """
 
-        return self.solution.build(
-            attribute.build(
-                *attribute.arguments.args,
-                **attribute.arguments.kwargs
-            )
-            for attribute in self.attributes
-        )
+        attributes = []
+
+        for attribute in self.attributes:
+            if issubclass(attribute, Attribute):
+                attribute = attribute.build(
+                    *attribute.arguments.args,
+                    **attribute.arguments.kwargs
+                )
+
+            elif isinstance(attributes, Attribute):
+                attribute = attribute.copy()
+
+            else:
+                try:
+                    values = list(attribute)
+
+                    attribute = (
+                        type(values[0])
+                        if isinstance(values[0], Attribute) else
+                        values[0]
+                    )(
+                        value=Template(
+                            solution=self.solution,
+                            attributes=values
+                        ).build().attributes
+                    )
+
+                except (ValueError, TypeError) as e:
+                    raise ValueError(
+                        f"Invalid attributes structure: "
+                        f"{attribute}. {str(e)}"
+                    )
+                # end try
+            # end if
+
+            attributes.append(attribute)
+        # end for
+
+        return self.solution.build(attributes=attributes)
     # end build
 # end Template
```

### Comparing `genetic-algo-0.0.0/genetic_algo.egg-info/PKG-INFO` & `genetic-algo-0.0.1/genetic_algo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genetic-algo
-Version: 0.0.0
+Version: 0.0.1
 Summary: A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.
 Home-page: https://github.com/Shahaf-F-S/auto-screener
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `genetic-algo-0.0.0/pyproject.toml` & `genetic-algo-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'genetic-algo'
-version = '0.0.0'
+version = '0.0.1'
 description = 'A framework for developing Genetic-Algorithm programs to solve problems dynamically and explicitly.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `genetic-algo-0.0.0/setup.py` & `genetic-algo-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ],
         include=[
             "test.py"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='genetic-algo',
-        version='0.0.0',
+        version='0.0.1',
         description=(
             "A framework for developing Genetic-Algorithm "
             "programs to solve problems dynamically and explicitly."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
         author_email='shahaffrs@gmail.com',
```

### Comparing `genetic-algo-0.0.0/test.py` & `genetic-algo-0.0.1/test.py`

 * *Files identical despite different names*

