# Comparing `tmp/jaxrenderer-0.2.0.tar.gz` & `tmp/jaxrenderer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxrenderer-0.2.0.tar", max compression
+gzip compressed data, was "jaxrenderer-0.2.1.tar", max compression
```

## Comparing `jaxrenderer-0.2.0.tar` & `jaxrenderer-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11367 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/LICENSE
--rw-r--r--   0        0        0     2312 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/README.md
--rw-r--r--   0        0        0     4530 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/changelog.md
--rw-r--r--   0        0        0     1540 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4851 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/renderer/README.md
--rw-r--r--   0        0        0      459 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/renderer/__init__.py
--rw-r--r--   0        0        0    33725 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/renderer/geometry.py
--rw-r--r--   0        0        0    14815 2023-06-03 14:29:52.493212 jaxrenderer-0.2.0/renderer/model.py
--rw-r--r--   0        0        0    13911 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/pipeline.py
--rw-r--r--   0        0        0    13883 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/renderer.py
--rw-r--r--   0        0        0     9726 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/scene.py
--rw-r--r--   0        0        0    10102 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shader.py
--rw-r--r--   0        0        0     4600 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/README.md
--rw-r--r--   0        0        0     1256 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/depth.py
--rw-r--r--   0        0        0     3252 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/gouraud.py
--rw-r--r--   0        0        0     4804 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/gouraud_texture.py
--rw-r--r--   0        0        0     5079 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/phong.py
--rw-r--r--   0        0        0     9571 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/phong_darboux.py
--rw-r--r--   0        0        0     7926 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/phong_reflection.py
--rw-r--r--   0        0        0     9650 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shaders/phong_reflection_shadow.py
--rw-r--r--   0        0        0     4166 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shadow.py
--rw-r--r--   0        0        0    71549 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shapes/capsule.py
--rw-r--r--   0        0        0     3574 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/shapes/cube.py
--rw-r--r--   0        0        0     3270 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/types.py
--rw-r--r--   0        0        0     3074 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/utils.py
--rw-r--r--   0        0        0      833 2023-06-03 14:29:52.497212 jaxrenderer-0.2.0/renderer/value_checker.py
--rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 jaxrenderer-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11367 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2312 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/README.md
+-rw-r--r--   0        0        0     4797 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/changelog.md
+-rw-r--r--   0        0        0     1540 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4851 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/renderer/README.md
+-rw-r--r--   0        0        0      539 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/renderer/__init__.py
+-rw-r--r--   0        0        0    33725 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/renderer/geometry.py
+-rw-r--r--   0        0        0    17155 2023-06-04 08:42:04.764875 jaxrenderer-0.2.1/renderer/model.py
+-rw-r--r--   0        0        0    13911 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/pipeline.py
+-rw-r--r--   0        0        0    13883 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/renderer.py
+-rw-r--r--   0        0        0     9130 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/scene.py
+-rw-r--r--   0        0        0    10102 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shader.py
+-rw-r--r--   0        0        0     4600 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/README.md
+-rw-r--r--   0        0        0     1256 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/depth.py
+-rw-r--r--   0        0        0     3252 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/gouraud.py
+-rw-r--r--   0        0        0     4804 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/gouraud_texture.py
+-rw-r--r--   0        0        0     5079 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/phong.py
+-rw-r--r--   0        0        0     9571 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/phong_darboux.py
+-rw-r--r--   0        0        0     7926 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/phong_reflection.py
+-rw-r--r--   0        0        0     9650 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shaders/phong_reflection_shadow.py
+-rw-r--r--   0        0        0     4166 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shadow.py
+-rw-r--r--   0        0        0    71549 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shapes/capsule.py
+-rw-r--r--   0        0        0     3574 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/shapes/cube.py
+-rw-r--r--   0        0        0     3270 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/types.py
+-rw-r--r--   0        0        0     3074 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/utils.py
+-rw-r--r--   0        0        0      833 2023-06-04 08:42:04.768875 jaxrenderer-0.2.1/renderer/value_checker.py
+-rw-r--r--   0        0        0     3766 1970-01-01 00:00:00.000000 jaxrenderer-0.2.1/PKG-INFO
```

### Comparing `jaxrenderer-0.2.0/LICENSE` & `jaxrenderer-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/README.md` & `jaxrenderer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/changelog.md` & `jaxrenderer-0.2.1/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,7 +40,12 @@
 2. Fix `geometry.py::transform_matrix_from_rotation`. Also, change the order of quaternion to `(w, x, y, z)` instead of `(x, y, z, w)` for consistency.
 3. Force convert `ShadowParameters` to JAX arrays in `Renderer.get_camera_image` to avoid downstream errors.
 
 ## 0.2.0
 
 1. Instead of clipping (planned to be implemented), now the rasteriser interpolates in homogeneous space directly. `Shader.interpolate` will not receive valid `barycentric_screen` values for now. Setting `Interpolation.SMOOTH` and `Interpolation.NOPERSPECTIVE` will result in same results, perspective-correct interpolations.
 2. Reorganise example files and rename them.
+
+## 0.2.1
+
+1. Refactor `Scene.set_object_*` methods to be a simple wrapper of `self._replace` and `ModelObject.replace_with_*`, to expose APIs of `ModelObject`s and allows manipulation and rendering without `Scene`.
+2. Expose `create_capsule` and `create_cube` APIs.
```

### Comparing `jaxrenderer-0.2.0/pyproject.toml` & `jaxrenderer-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaxrenderer"
-version = "0.2.0"
+version = "0.2.1"
 description = "Jax implementation of rasterizer renderer."
 authors = ["Joey Teng <joey.teng.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/JoeyTeng/jaxrenderer"
 repository = "https://github.com/JoeyTeng/jaxrenderer"
 classifiers = [
```

### Comparing `jaxrenderer-0.2.0/renderer/README.md` & `jaxrenderer-0.2.1/renderer/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/geometry.py` & `jaxrenderer-0.2.1/renderer/geometry.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/model.py` & `jaxrenderer-0.2.1/renderer/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import jax.experimental.checkify as checkify
 import jax.lax as lax
 import jax.numpy as jnp
 from jax.tree_util import tree_map
 from jaxtyping import (Array, Bool, Float, Integer, Num, PyTree, Shaped,
                        jaxtyped)
 
-from .geometry import Camera
+from .geometry import Camera, transform_matrix_from_rotation
 from .types import (FALSE_ARRAY, FaceIndices, Normals, SpecularMap, Texture,
-                    UVCoordinates, Vec3f, Vertices)
+                    UVCoordinates, Vec3f, Vec4f, Vertices)
 from .value_checker import index_in_bound
 
 ModelMatrix = Float[Array, "4 4"]
 
 
 class Model(NamedTuple):
     """Model with vertices specification and attached maps.
@@ -314,14 +314,85 @@
     """Local scaling factors of the object, in x, y, z."""
     transform: ModelMatrix = jnp.identity(4)
     """Transform matrix (model matrix) of the model."""
     # TODO: Support double_sided
     double_sided: Bool[Array, ""] = FALSE_ARRAY
     """Whether the object is double-sided."""
 
+    @jaxtyped
+    def replace_with_position(self, position: Vec3f) -> "ModelObject":
+        """Return a new ModelObject with given position.
+
+        !!This does not change the original object.
+
+        Parameters:
+          - position: the new position of the object.
+        """
+        return self._replace(transform=self.transform.at[:3, 3].set(position))
+
+    @jaxtyped
+    def replace_with_orientation(
+        self,
+        orientation: Optional[Vec4f] = None,
+        rotation_matrix: Optional[Float[Array, "3 3"]] = None,
+    ) -> "ModelObject":
+        """Return a new ModelObject with given orientation or rotation_matrix.
+
+        If rotation_matrix is specified, it takes precedence over orientation.
+        If none is specified, the object's orientation is set to identity.
+
+        !!This does not change the original object.
+
+        Parameters:
+          - orientation: the new orientation of the object, optional.
+          - rotation_matrix: the new rotation matrix of the object, optional
+        """
+        if rotation_matrix is None:
+            if orientation is None:
+                orientation = jnp.array((0., 0., 0., 1.))
+
+            assert isinstance(orientation, Vec4f), f"{orientation}"
+            rotation_matrix = transform_matrix_from_rotation(orientation)
+
+        assert isinstance(
+            rotation_matrix,
+            Float[Array, "3 3"],
+        ), f"{rotation_matrix}"
+
+        return self._replace(
+            transform=self.transform.at[:3, :3].set(rotation_matrix))
+
+    @jaxtyped
+    def replace_with_local_scaling(
+        self,
+        local_scaling: Vec3f,
+    ) -> "ModelObject":
+        """Return a new ModelObject with given local_scaling.
+
+        !!This does not change the original object.
+
+        Parameters:
+          - local_scaling: the new local scaling of the object.
+        """
+        return self._replace(local_scaling=local_scaling)
+
+    @jaxtyped
+    def replace_with_double_sided(
+        self,
+        double_sided: Bool[Array, ""],
+    ) -> "ModelObject":
+        """Return a new ModelObject with given double_sided.
+
+        !!This does not change the original object.
+
+        Parameters:
+          - double_sided: whether the object is double-sided.
+        """
+        return self._replace(double_sided=double_sided)
+
 
 def batch_models(models: Sequence[MergedModel]) -> MergedModel:
     """Merge multiple MergedModel into one, with each field being a batch, with
         batch axis at 0. This is intended to facilitate `jax.vmap`.
     """
     merged_model = MergedModel._make((lax.concatenate(
         [jnp.asarray(model[i])[None, ...] for model in models],
```

### Comparing `jaxrenderer-0.2.0/renderer/pipeline.py` & `jaxrenderer-0.2.1/renderer/pipeline.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/renderer.py` & `jaxrenderer-0.2.1/renderer/renderer.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/scene.py` & `jaxrenderer-0.2.1/renderer/scene.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import NamedTuple, NewType, Optional, Union
 
 import jax
 import jax.lax as lax
 import jax.numpy as jnp
 from jaxtyping import Array, Bool, Float, jaxtyped
 
-from .geometry import transform_matrix_from_rotation
 from .model import Model, ModelObject
 from .shapes.capsule import UpAxis, create_capsule
 from .shapes.cube import create_cube
 from .types import SpecularMap, Texture, Vec3f, Vec4f
 
 GUID = NewType("GUID", int)
 
@@ -191,17 +190,15 @@
         Parameters:
           - object_id: the unique identifier of the object.
           - position: the new position of the object.
         """
         position = jnp.asarray(position, dtype=float)
         assert isinstance(position, Vec3f), f"{position}"
 
-        obj: ModelObject = self.objects[object_id]
-        new_mat: Float[Array, "4 4"] = obj.transform.at[:3, 3].set(position)
-        new_obj: ModelObject = obj._replace(transform=new_mat)
+        new_obj = self.objects[object_id].replace_with_position(position)
 
         return self._replace(objects=self.objects | {object_id: new_obj})
 
     @jaxtyped
     def set_object_orientation(
         self,
         object_id: GUID,
@@ -215,31 +212,23 @@
         If none is specified, the object's orientation is set to identity.
 
         Parameters:
           - object_id: the unique identifier of the object.
           - orientation: the new orientation of the object, optional.
           - rotation_matrix: the new rotation matrix of the object, optional
         """
-        if rotation_matrix is None:
-            if orientation is None:
-                orientation = (0., 0., 0., 1.)
-
-            _orientation = jnp.asarray(orientation, dtype=float)
-            assert isinstance(_orientation, Vec4f), f"{orientation}"
-            rotation_matrix = transform_matrix_from_rotation(_orientation)
-
-        assert isinstance(
-            rotation_matrix,
-            Float[Array, "3 3"],
-        ), f"{rotation_matrix}"
-
-        obj: ModelObject = self.objects[object_id]
-        new_mat: Float[Array, "4 4"]
-        new_mat = obj.transform.at[:3, :3].set(rotation_matrix)
-        new_obj: ModelObject = obj._replace(transform=new_mat)
+        if orientation is not None:
+            orientation = jnp.asarray(orientation)
+        if rotation_matrix is not None:
+            rotation_matrix = jnp.asarray(rotation_matrix)
+
+        new_obj = self.objects[object_id].replace_with_orientation(
+            orientation=orientation,
+            rotation_matrix=rotation_matrix,
+        )
 
         return self._replace(objects=self.objects | {object_id: new_obj})
 
     @jaxtyped
     def set_object_local_scaling(
         self,
         object_id: GUID,
@@ -247,18 +236,18 @@
     ) -> "Scene":
         """Set the local scaling of an object in the scene.
 
         Parameters:
           - object_id: the unique identifier of the object.
           - local_scaling: the new local scaling of the object.
         """
-        local_scaling = jnp.asarray(local_scaling, dtype=float)
-        assert isinstance(local_scaling, Vec3f), f"{local_scaling}"
-        obj: ModelObject = self.objects[object_id]
-        new_obj: ModelObject = obj._replace(local_scaling=local_scaling)
+        scaling = jnp.asarray(local_scaling, dtype=float)
+        assert isinstance(scaling, Vec3f), f"{scaling}"
+
+        new_obj = self.objects[object_id].replace_with_local_scaling(scaling)
 
         return self._replace(objects=self.objects | {object_id: new_obj})
 
     @jaxtyped
     def set_object_double_sided(
         self,
         object_id: GUID,
@@ -266,12 +255,11 @@
     ) -> "Scene":
         """Set whether an object in the scene is double-sided.
 
         Parameters:
           - object_id: the unique identifier of the object.
           - double_sided: whether the object is double-sided.
         """
-        obj: ModelObject = self.objects[object_id]
-        new_obj: ModelObject
-        new_obj = obj._replace(double_sided=jnp.asarray(double_sided))
+        new_obj = self.objects[object_id].replace_with_double_sided(
+            jnp.asarray(double_sided))
 
         return self._replace(objects=self.objects | {object_id: new_obj})
```

### Comparing `jaxrenderer-0.2.0/renderer/shader.py` & `jaxrenderer-0.2.1/renderer/shader.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shaders/README.md` & `jaxrenderer-0.2.1/renderer/shaders/README.md`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shaders/depth.py` & `jaxrenderer-0.2.1/renderer/shaders/depth.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shaders/gouraud.py` & `jaxrenderer-0.2.1/renderer/shaders/gouraud.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shaders/gouraud_texture.py` & `jaxrenderer-0.2.1/renderer/shaders/gouraud_texture.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shaders/phong.py` & `jaxrenderer-0.2.1/renderer/shaders/phong.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shaders/phong_darboux.py` & `jaxrenderer-0.2.1/renderer/shaders/phong_darboux.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shaders/phong_reflection.py` & `jaxrenderer-0.2.1/renderer/shaders/phong_reflection.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shaders/phong_reflection_shadow.py` & `jaxrenderer-0.2.1/renderer/shaders/phong_reflection_shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shadow.py` & `jaxrenderer-0.2.1/renderer/shadow.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shapes/capsule.py` & `jaxrenderer-0.2.1/renderer/shapes/capsule.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/shapes/cube.py` & `jaxrenderer-0.2.1/renderer/shapes/cube.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/types.py` & `jaxrenderer-0.2.1/renderer/types.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/utils.py` & `jaxrenderer-0.2.1/renderer/utils.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/renderer/value_checker.py` & `jaxrenderer-0.2.1/renderer/value_checker.py`

 * *Files identical despite different names*

### Comparing `jaxrenderer-0.2.0/PKG-INFO` & `jaxrenderer-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxrenderer
-Version: 0.2.0
+Version: 0.2.1
 Summary: Jax implementation of rasterizer renderer.
 Home-page: https://github.com/JoeyTeng/jaxrenderer
 License: Apache-2.0
 Author: Joey Teng
 Author-email: joey.teng.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

