# Comparing `tmp/arrendatools.plantillas-0.2.0.tar.gz` & `tmp/arrendatools.plantillas-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrendatools.plantillas-0.2.0.tar", last modified: Wed Apr 26 20:03:34 2023, max compression
+gzip compressed data, was "arrendatools.plantillas-0.3.0.tar", last modified: Sun Jun  4 11:50:21 2023, max compression
```

## Comparing `arrendatools.plantillas-0.2.0.tar` & `arrendatools.plantillas-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1062 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3241 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1201 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.470889 arrendatools.plantillas-0.2.0/arrendatools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/arrendatools/plantillas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1700 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/fechas.py
--rw-r--r--   0 root         (0) root         (0)     3175 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/numeros.py
--rw-r--r--   0 root         (0) root         (0)     1344 2023-04-26 20:03:31.000000 arrendatools.plantillas-0.2.0/arrendatools/plantillas/plantilla.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3241 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      497 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-04-26 20:03:34.000000 arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-04-26 20:03:34.474890 arrendatools.plantillas-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1355 2023-04-26 20:03:32.000000 arrendatools.plantillas-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/arrendatools/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/arrendatools/plantillas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/fechas.py
+-rw-r--r--   0 root         (0) root         (0)     3175 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/numeros.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/arrendatools/plantillas/plantilla.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-04 11:50:21.000000 arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-04 11:50:21.627750 arrendatools.plantillas-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-06-04 11:50:19.000000 arrendatools.plantillas-0.3.0/setup.py
```

### Comparing `arrendatools.plantillas-0.2.0/LICENSE` & `arrendatools.plantillas-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.2.0/PKG-INFO` & `arrendatools.plantillas-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.2.0
+Version: 0.3.0
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,....
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT License
         
         Copyright (c) 2023 Jordi
```

### Comparing `arrendatools.plantillas-0.2.0/README.md` & `arrendatools.plantillas-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.2.0/arrendatools/plantillas/filters/numeros.py` & `arrendatools.plantillas-0.3.0/arrendatools/plantillas/filters/numeros.py`

 * *Files identical despite different names*

### Comparing `arrendatools.plantillas-0.2.0/arrendatools/plantillas/plantilla.py` & `arrendatools.plantillas-0.3.0/arrendatools/plantillas/plantilla.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from jinja2 import Environment, FileSystemLoader, BaseLoader
-from arrendatools.plantillas.filters.fechas import dias_del_año, formato_fecha, aplicar_timedelta
+from arrendatools.plantillas.filters.fechas import dias_del_año, formato_fecha, aplicar_timedelta, trimestre
 from arrendatools.plantillas.filters.numeros import formato_divisa, formato_porcentaje, numero_a_palabras
 
 
 custom_functions = {
     "aplicar_timedelta": aplicar_timedelta,
     "numero_a_palabras": numero_a_palabras,
     "formato_divisa": formato_divisa,
     "formato_porcentaje": formato_porcentaje,
     "formato_fecha": formato_fecha,
-    "dias_del_año": dias_del_año
+    "dias_del_año": dias_del_año,
+    "trimestre": trimestre
 }
 
 custom_filters = {**custom_functions}
 
 
 def aplicar_plantilla(directorio_plantillas, plantilla, datos):
-    try:
-        environment = Environment(loader=FileSystemLoader(directorio_plantillas))
-        environment.filters.update(custom_filters)
-        environment.globals.update(custom_functions)
-        template = environment.get_template(plantilla)
-        return template.render(datos)
-    except Exception as e:
-        return str(e)
+    environment = Environment(loader=FileSystemLoader(directorio_plantillas))
+    environment.filters.update(custom_filters)
+    environment.globals.update(custom_functions)
+    template = environment.get_template(plantilla)
+    return template.render(datos)
 
 
 def aplicar_plantilla_texto(texto_plantilla, datos):
     try:
         environment = Environment(loader=BaseLoader)
         environment.filters.update(custom_filters)
         environment.globals.update(custom_functions)
```

### Comparing `arrendatools.plantillas-0.2.0/arrendatools.plantillas.egg-info/PKG-INFO` & `arrendatools.plantillas-0.3.0/arrendatools.plantillas.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arrendatools.plantillas
-Version: 0.2.0
+Version: 0.3.0
 Summary: Módulo de Python que aplica plantillas jinja. Además inlcuye filtros que pueden ser útiles para la generación de recibos de alquiler, facturas, informes,....
 Home-page: https://github.com/hokus15/ArrendaToolsPlantillas
 Author: hokus15
 Author-email: hokus@hotmail.com
 License: MIT License
         
         Copyright (c) 2023 Jordi
```

### Comparing `arrendatools.plantillas-0.2.0/setup.py` & `arrendatools.plantillas-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup, find_packages
 import pkg_resources
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 with open('LICENSE', encoding='utf-8') as f:
     license = f.read()
```

