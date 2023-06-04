# Comparing `tmp/vector2dggs-0.3.4.tar.gz` & `tmp/vector2dggs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.3.4.tar", max compression
+gzip compressed data, was "vector2dggs-0.4.0.tar", max compression
```

## Comparing `vector2dggs-0.3.4.tar` & `vector2dggs-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8208 2023-05-30 03:31:45.583819 vector2dggs-0.3.4/README.md
--rw-r--r--   0        0        0     1092 2023-05-30 03:31:50.231842 vector2dggs-0.3.4/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.4/vector2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.4/vector2dggs/cli.py
--rw-r--r--   0        0        0    13018 2023-05-30 03:31:02.319601 vector2dggs-0.3.4/vector2dggs/h3.py
--rw-r--r--   0        0        0     3173 2023-05-22 02:20:32.367257 vector2dggs-0.3.4/vector2dggs/katana.py
--rw-r--r--   0        0        0     9642 1970-01-01 00:00:00.000000 vector2dggs-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     8208 2023-06-04 03:24:25.334318 vector2dggs-0.4.0/README.md
+-rw-r--r--   0        0        0     1092 2023-06-04 03:24:09.972154 vector2dggs-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-06-04 03:24:32.375320 vector2dggs-0.4.0/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-29 05:44:55.043652 vector2dggs-0.4.0/vector2dggs/cli.py
+-rw-r--r--   0        0        0    12344 2023-06-04 03:20:22.172432 vector2dggs-0.4.0/vector2dggs/h3.py
+-rw-r--r--   0        0        0     3173 2023-05-29 05:44:55.043652 vector2dggs-0.4.0/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9642 1970-01-01 00:00:00.000000 vector2dggs-0.4.0/PKG-INFO
```

### Comparing `vector2dggs-0.3.4/README.md` & `vector2dggs-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -151,17 +151,17 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.4},
+  version={0.4.0},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.4) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.4.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.3.4/pyproject.toml` & `vector2dggs-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.3.4"
+version = "0.4.0"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
```

### Comparing `vector2dggs-0.3.4/vector2dggs/cli.py` & `vector2dggs-0.4.0/vector2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.3.4/vector2dggs/h3.py` & `vector2dggs-0.4.0/vector2dggs/h3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import click
-import click_log
 import errno
 import logging
 import os
 import multiprocessing
 from multiprocessing.dummy import Pool
 from pathlib import Path, PurePath
 import shutil
@@ -11,14 +9,16 @@
 import tempfile
 from typing import Union
 from urllib.parse import urlparse
 import warnings
 
 os.environ["USE_PYGEOS"] = "0"
 
+import click
+import click_log
 import dask.dataframe as dd
 import dask_geopandas as dgpd
 import geopandas as gpd
 import h3pandas
 import pandas as pd
 import pyproj
 from shapely.geometry import GeometryCollection
@@ -40,16 +40,14 @@
 
 DEFAULT_PARENT_OFFSET = 6
 
 
 class ParentResolutionException(Exception):
     pass
 
-class EmptyDataException(Exception):
-    pass
 
 def _get_parent_res(parent_res: Union[None, int], resolution: int):
     """
     Uses a parent resolution,
     OR,
     Given a target resolution, returns our recommended parent resolution.
 
@@ -79,16 +77,15 @@
         .drop(columns=[spatial_sort_col])
         .h3.polyfill_resample(resolution, return_geometry=False)
     )
     df = pd.DataFrame(df).drop(columns=["index", "geometry"])
     df.index.rename(f"h3_{resolution:02}", inplace=True)
     parent_res: int = _get_parent_res(parent_res, resolution)
     # Secondary (parent) H3 index, used later for partitioning
-    df = df.h3.h3_to_parent(parent_res).reset_index()
-    df.to_parquet(
+    df.h3.h3_to_parent(parent_res).to_parquet(
         PurePath(output_directory, pq_in.name),
         engine="auto",
         compression="ZSTD",
     )
     return None
 
 
@@ -98,53 +95,36 @@
 
 def _parent_partitioning(
     input_dir: Path,
     output_dir: Path,
     resolution,
     parent_res: Union[None, int],
     **kwargs,
-) -> Path:
+) -> None:
     parent_res: int = _get_parent_res(parent_res, resolution)
-    with TqdmCallback(desc="Reading spatial partitions"):
-        # Set index as parent cell
-        ddf = dd.read_parquet(input_dir, engine="pyarrow").set_index(
-            f"h3_{parent_res:02}"
-        )
-    with TqdmCallback(desc="Counting parents"):
-        # Count parents, to get target number of partitions
-        uniqueh3 = sorted(list(ddf.index.unique().compute()))
-
-    if not len(uniqueh3):
-        raise EmptyDataException('No data to write; input data appears empty. Requested output "{output_dir}" will not be written.'.format(output_dir=output_dir))
-
-    LOGGER.debug(
-        "Repartitioning into %d partitions, based on parent cells",
-        len(uniqueh3) + 1,
-    )
+    partition_col = f"h3_{parent_res:02}"
 
     with TqdmCallback(desc="Repartitioning"):
-        ddf = (
-            ddf.repartition(  # See "notes" on why divisions expects repetition of the last item https://docs.dask.org/en/stable/generated/dask.dataframe.DataFrame.repartition.html
-                divisions=(uniqueh3 + [uniqueh3[-1]]), force=True
-            )
-            .reset_index()
-            .set_index(f"h3_{resolution:02}")
-            .drop(columns=[f"h3_{parent_res:02}"])
-            .to_parquet(
-                output_dir,
-                overwrite=kwargs.get("overwrite", False),
-                engine=kwargs.get("engine", "pyarrow"),
-                write_index=True,
-                # append=False,
-                name_function=lambda i: f"{uniqueh3[i]}.parquet",
-                compression=kwargs.get("compression", "ZSTD"),
-            )
+        dd.read_parquet(input_dir, engine="pyarrow").to_parquet(
+            output_dir,
+            overwrite=kwargs.get("overwrite", False),
+            engine=kwargs.get("engine", "pyarrow"),
+            partition_on=partition_col,
+            compression=kwargs.get("compression", "ZSTD"),
         )
     LOGGER.debug("Parent cell repartitioning complete")
-    return output_dir
+
+    # Rename output to just be the partition key, suffix .parquet
+    for f in os.listdir(output_dir):
+        os.rename(
+            os.path.join(output_dir, f),
+            os.path.join(output_dir, f.replace(f"{partition_col}=", "") + ".parquet"),
+        )
+
+    return
 
 
 def _index(
     input_file: Union[Path, str],
     output_directory: Union[Path, str],
     resolution: int,
     parent_res: Union[None, int],
@@ -234,15 +214,15 @@
             with Pool(processes=processes) as pool:
                 args = [
                     (filepath, spatial_sort_col, resolution, parent_res, tmpdir2)
                     for filepath in filepaths
                 ]
                 list(tqdm(pool.imap(polyfill_star, args), total=len(args)))
 
-            output_directory = _parent_partitioning(
+            _parent_partitioning(
                 tmpdir2, output_directory, resolution, parent_res, overwrite=overwrite
             )
 
     return output_directory
 
 
 @click.command(context_settings={"show_default": True})
@@ -338,14 +318,20 @@
     "--geom_col",
     required=False,
     default="geom",
     type=str,
     help="Column name to use when using a spatial database connection as input",
     nargs=1,
 )
+@click.option(
+    "--tempdir",
+    default=tempfile.tempdir,
+    type=click.Path(),
+    help="Temporary data is created during the execution of this program. This parameter allows you to control where this data will be written."
+)
 @click.option("-o", "--overwrite", is_flag=True)
 @click.version_option(version=__version__)
 def h3(
     vector_input: Union[str, Path],
     output_directory: Union[str, Path],
     resolution: str,
     parent_res: str,
@@ -354,22 +340,24 @@
     partitions: int,
     spatial_sorting: str,
     cut_crs: int,
     cut_threshold: int,
     threads: int,
     table: str,
     geom_col: str,
+    tempdir: Union[str, Path],
     overwrite: bool,
 ):
     """
     Ingest a vector dataset and index it to the H3 DGGS.
 
     VECTOR_INPUT is the path to input vector geospatial data.
     OUTPUT_DIRECTORY should be a directory, not a file or database table, as it will instead be the write location for an Apache Parquet data store.
     """
+    tempfile.tempdir = tempdir
     if parent_res is not None and not int(parent_res) < int(resolution):
         raise ParentResolutionException(
             "Parent resolution ({pr}) must be less than target resolution ({r})".format(
                 pr=parent_res, r=resolution
             )
         )
     con: sqlalchemy.engine.Connection = None
```

### Comparing `vector2dggs-0.3.4/vector2dggs/katana.py` & `vector2dggs-0.4.0/vector2dggs/katana.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.3.4/PKG-INFO` & `vector2dggs-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.3.4
+Version: 0.4.0
 Summary: CLI DGGS indexer for vector geospatial data
 Home-page: https://github.com/manaakiwhenua/vector2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,vector,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -186,18 +186,18 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.4},
+  version={0.4.0},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.4) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.4.0) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

