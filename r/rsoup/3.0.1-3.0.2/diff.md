# Comparing `tmp/rsoup-3.0.1.tar.gz` & `tmp/rsoup-3.0.2.tar.gz`

## Comparing `rsoup-3.0.1.tar` & `rsoup-3.0.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0     1065 1970-01-01 00:00:00.000000 rsoup-3.0.1/Cargo.toml
--rw-r--r--   0     7641     1017     1735 2023-05-19 00:37:04.000000 rsoup-3.0.1/.github/workflows/ci.yml
--rw-r--r--   0     7641     1017     1815 2022-08-12 05:16:24.000000 rsoup-3.0.1/.gitignore
--rw-r--r--   0     7641     1017     1064 2022-08-12 05:16:24.000000 rsoup-3.0.1/LICENSE
--rw-r--r--   0     7641     1017      118 2022-11-09 03:10:03.000000 rsoup-3.0.1/README.md
--rw-r--r--   0     7641     1017     3490 2023-02-04 01:31:44.000000 rsoup-3.0.1/benches/context_recursive_extractor_benchmark.rs
--rw-r--r--   0     7641     1017     1830 2022-11-09 03:10:03.000000 rsoup-3.0.1/benches/get_text.rs
--rw-r--r--   0     7641     1017      786 2023-05-17 21:06:30.000000 rsoup-3.0.1/pyproject.toml
--rw-r--r--   0     7641     1017        0 2022-08-12 05:16:24.000000 rsoup-3.0.1/rsoup/__init__.py
--rw-r--r--   0     7641     1017     4233 2023-05-17 01:21:12.000000 rsoup-3.0.1/rsoup/core.pyi
--rw-r--r--   0     7641     1017      586 2022-08-12 05:16:24.000000 rsoup-3.0.1/rsoup/exceptions.py
--rw-r--r--   0     7641     1017      561 2022-08-12 05:16:24.000000 rsoup-3.0.1/rsoup/fetch_tables.py
--rw-r--r--   0     7641     1017    15212 2022-08-12 05:16:24.000000 rsoup-3.0.1/rsoup/python/context_extractor.py
--rw-r--r--   0     7641     1017        0 2022-08-12 05:16:24.000000 rsoup-3.0.1/rsoup/python/models/__init__.py
--rw-r--r--   0     7641     1017     3091 2022-08-12 05:16:24.000000 rsoup-3.0.1/rsoup/python/models/context.py
--rw-r--r--   0     7641     1017     9840 2022-08-12 05:16:24.000000 rsoup-3.0.1/rsoup/python/models/html_table.py
--rw-r--r--   0     7641     1017    11141 2022-08-12 05:16:24.000000 rsoup-3.0.1/rsoup/python/table_extractor.py
--rw-r--r--   0     7641     1017        4 2022-08-12 05:16:24.000000 rsoup-3.0.1/scripts/.gitignore
--rw-r--r--   0     7641     1017      722 2022-08-12 05:16:24.000000 rsoup-3.0.1/scripts/gen_data.py
--rw-r--r--   0     7641     1017     1528 2023-05-17 01:21:23.000000 rsoup-3.0.1/scripts/test_table_extractor.py
--rw-r--r--   0     7641     1017     1072 2023-05-04 20:01:25.000000 rsoup-3.0.1/src/error.rs
--rw-r--r--   0     7641     1017    25491 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/extractors/context_v1.rs
--rw-r--r--   0     7641     1017      615 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/extractors/mod.rs
--rw-r--r--   0     7641     1017    10224 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/extractors/table.rs
--rw-r--r--   0     7641     1017    11019 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/extractors/text/get_rich_text.rs
--rw-r--r--   0     7641     1017     3477 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/extractors/text/get_text_v1.rs
--rw-r--r--   0     7641     1017     2691 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/extractors/text/get_text_v2.rs
--rw-r--r--   0     7641     1017     3595 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/extractors/text/line.rs
--rw-r--r--   0     7641     1017     1302 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/extractors/text/mod.rs
--rw-r--r--   0     7641     1017      848 2023-05-17 01:31:33.000000 rsoup-3.0.1/src/lib.rs
--rw-r--r--   0     7641     1017     1042 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/misc/mod.rs
--rw-r--r--   0     7641     1017      404 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/misc/range_iter.rs
--rw-r--r--   0     7641     1017     5634 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/misc/recursive_iter.rs
--rw-r--r--   0     7641     1017     3474 2022-08-12 05:16:24.000000 rsoup-3.0.1/src/misc/tree/iterator.rs
--rw-r--r--   0     7641     1017       39 2022-08-12 05:16:24.000000 rsoup-3.0.1/src/misc/tree/mod.rs
--rw-r--r--   0     7641     1017     6158 2023-02-27 23:55:58.000000 rsoup-3.0.1/src/misc/tree/simple_tree.rs
--rw-r--r--   0     7641     1017     1600 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/misc/url_converter.rs
--rw-r--r--   0     7641     1017     4651 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/models/content_hierarchy.rs
--rw-r--r--   0     7641     1017       61 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/models/mod.rs
--rw-r--r--   0     7641     1017    13378 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/models/rich_text.rs
--rw-r--r--   0     7641     1017     1824 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/models/table/cell.rs
--rw-r--r--   0     7641     1017     2926 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/models/table/cell_iter.rs
--rw-r--r--   0     7641     1017      158 2022-11-09 03:10:03.000000 rsoup-3.0.1/src/models/table/mod.rs
--rw-r--r--   0     7641     1017     2036 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/models/table/row.rs
--rw-r--r--   0     7641     1017      591 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/models/table/row_iter.rs
--rw-r--r--   0     7641     1017    13112 2023-05-17 01:28:08.000000 rsoup-3.0.1/src/models/table/table.rs
--rw-r--r--   0     7641     1017        0 2022-08-12 05:16:24.000000 rsoup-3.0.1/tests/__init__.py
--rw-r--r--   0     7641     1017      639 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/conftest.py
--rw-r--r--   0     7641     1017        0 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/extractors/__init__.py
--rw-r--r--   0     7641     1017       79 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/extractors/mod.rs
--rw-r--r--   0     7641     1017     3639 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/extractors/test_context_extractor.rs
--rw-r--r--   0     7641     1017     3052 2023-05-17 01:41:15.000000 rsoup-3.0.1/tests/extractors/test_table_extractor.py
--rw-r--r--   0     7641     1017     1389 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/extractors/test_table_extractor.rs
--rw-r--r--   0     7641     1017     3573 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/extractors/test_text_extractor.rs
--rw-r--r--   0     7641     1017      511 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/main.rs
--rw-r--r--   0     7641     1017        0 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/models/__init__.py
--rw-r--r--   0     7641     1017       20 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/models/mod.rs
--rw-r--r--   0     7641     1017     1889 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/models/test_table.rs
--rw-r--r--   0     7641     1017      867 2023-05-17 01:27:08.000000 rsoup-3.0.1/tests/models/test_table_pickle.py
--rw-r--r--   0     7641     1017    38251 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/resources/extractors/context/list_highest_mountains.html
--rw-r--r--   0     7641     1017      326 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/resources/extractors/context/one-level.html
--rw-r--r--   0     7641     1017      568 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/resources/extractors/context/three-level.html
--rw-r--r--   0     7641     1017     4917 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/resources/extractors/table.html
--rw-r--r--   0     7641     1017     1327 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/resources/extractors/text.html
--rw-r--r--   0     7641     1017     2648 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/resources/table_span.html
--rw-r--r--   0     7641     1017    77654 2022-11-09 03:10:03.000000 rsoup-3.0.1/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html
--rw-r--r--   0     7641     1017   381850 2022-08-12 05:16:24.000000 rsoup-3.0.1/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html
--rw-r--r--   0     7641     1017    53084 2023-06-04 18:59:20.000000 rsoup-3.0.1/Cargo.lock
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 rsoup-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 rsoup-3.0.2/Cargo.toml
+-rw-r--r--   0     1001      123     1863 2023-06-04 21:27:22.000000 rsoup-3.0.2/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123     1815 2023-06-04 21:27:22.000000 rsoup-3.0.2/.gitignore
+-rw-r--r--   0     1001      123     1064 2023-06-04 21:27:22.000000 rsoup-3.0.2/LICENSE
+-rw-r--r--   0     1001      123      118 2023-06-04 21:27:22.000000 rsoup-3.0.2/README.md
+-rw-r--r--   0     1001      123     3490 2023-06-04 21:27:22.000000 rsoup-3.0.2/benches/context_recursive_extractor_benchmark.rs
+-rw-r--r--   0     1001      123     1830 2023-06-04 21:27:22.000000 rsoup-3.0.2/benches/get_text.rs
+-rw-r--r--   0     1001      123      827 2023-06-04 21:27:22.000000 rsoup-3.0.2/pyproject.toml
+-rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/__init__.py
+-rw-r--r--   0     1001      123     4233 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/core.pyi
+-rw-r--r--   0     1001      123      586 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/exceptions.py
+-rw-r--r--   0     1001      123      561 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/fetch_tables.py
+-rw-r--r--   0     1001      123    15212 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/context_extractor.py
+-rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/models/__init__.py
+-rw-r--r--   0     1001      123     3091 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/models/context.py
+-rw-r--r--   0     1001      123     9840 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/models/html_table.py
+-rw-r--r--   0     1001      123    11141 2023-06-04 21:27:22.000000 rsoup-3.0.2/rsoup/python/table_extractor.py
+-rw-r--r--   0     1001      123        4 2023-06-04 21:27:22.000000 rsoup-3.0.2/scripts/.gitignore
+-rw-r--r--   0     1001      123      722 2023-06-04 21:27:22.000000 rsoup-3.0.2/scripts/gen_data.py
+-rw-r--r--   0     1001      123     1528 2023-06-04 21:27:22.000000 rsoup-3.0.2/scripts/test_table_extractor.py
+-rw-r--r--   0     1001      123     1072 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/error.rs
+-rw-r--r--   0     1001      123    25491 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/context_v1.rs
+-rw-r--r--   0     1001      123      615 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/mod.rs
+-rw-r--r--   0     1001      123    10224 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/table.rs
+-rw-r--r--   0     1001      123    11019 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/get_rich_text.rs
+-rw-r--r--   0     1001      123     3477 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/get_text_v1.rs
+-rw-r--r--   0     1001      123     2691 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/get_text_v2.rs
+-rw-r--r--   0     1001      123     3595 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/line.rs
+-rw-r--r--   0     1001      123     1302 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/extractors/text/mod.rs
+-rw-r--r--   0     1001      123      848 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/lib.rs
+-rw-r--r--   0     1001      123     1042 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/mod.rs
+-rw-r--r--   0     1001      123      404 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/range_iter.rs
+-rw-r--r--   0     1001      123     5634 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/recursive_iter.rs
+-rw-r--r--   0     1001      123     3474 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/tree/iterator.rs
+-rw-r--r--   0     1001      123       39 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/tree/mod.rs
+-rw-r--r--   0     1001      123     6158 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/tree/simple_tree.rs
+-rw-r--r--   0     1001      123     1600 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/misc/url_converter.rs
+-rw-r--r--   0     1001      123     4651 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/content_hierarchy.rs
+-rw-r--r--   0     1001      123       61 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/mod.rs
+-rw-r--r--   0     1001      123    13378 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/rich_text.rs
+-rw-r--r--   0     1001      123     1824 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/cell.rs
+-rw-r--r--   0     1001      123     2926 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/cell_iter.rs
+-rw-r--r--   0     1001      123      158 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/mod.rs
+-rw-r--r--   0     1001      123     2036 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/row.rs
+-rw-r--r--   0     1001      123      591 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/row_iter.rs
+-rw-r--r--   0     1001      123    13112 2023-06-04 21:27:22.000000 rsoup-3.0.2/src/models/table/table.rs
+-rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/__init__.py
+-rw-r--r--   0     1001      123      639 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/conftest.py
+-rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/__init__.py
+-rw-r--r--   0     1001      123       79 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/mod.rs
+-rw-r--r--   0     1001      123     3639 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/test_context_extractor.rs
+-rw-r--r--   0     1001      123     3052 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/test_table_extractor.py
+-rw-r--r--   0     1001      123     1389 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/test_table_extractor.rs
+-rw-r--r--   0     1001      123     3573 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/extractors/test_text_extractor.rs
+-rw-r--r--   0     1001      123      511 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/main.rs
+-rw-r--r--   0     1001      123        0 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/models/__init__.py
+-rw-r--r--   0     1001      123       20 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/models/mod.rs
+-rw-r--r--   0     1001      123     1889 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/models/test_table.rs
+-rw-r--r--   0     1001      123      867 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/models/test_table_pickle.py
+-rw-r--r--   0     1001      123    38251 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/context/list_highest_mountains.html
+-rw-r--r--   0     1001      123      326 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/context/one-level.html
+-rw-r--r--   0     1001      123      568 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/context/three-level.html
+-rw-r--r--   0     1001      123     4917 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/table.html
+-rw-r--r--   0     1001      123     1327 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/extractors/text.html
+-rw-r--r--   0     1001      123     2648 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/table_span.html
+-rw-r--r--   0     1001      123    77654 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html
+-rw-r--r--   0     1001      123   381850 2023-06-04 21:27:22.000000 rsoup-3.0.2/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html
+-rw-r--r--   0     1001      123    53084 2023-06-04 21:27:22.000000 rsoup-3.0.2/Cargo.lock
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 rsoup-3.0.2/PKG-INFO
```

### Comparing `rsoup-3.0.1/Cargo.toml` & `rsoup-3.0.2/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "rsoup"
 crate-type = ["cdylib", "rlib"]
 
-[package.metadata.maturin]
-name = "rsoup.core"
-
 [dependencies]
 anyhow = { version = "1.0.59", features = ["backtrace"] }
 base64 = "0.13.0"
 criterion = "0.3.6"
 ego-tree = "0.6.2"
 hashbrown = { version = "0.12.3", features = ["serde"] }
 html5ever = "0.26.0"
```

### Comparing `rsoup-3.0.1/.github/workflows/ci.yml` & `rsoup-3.0.2/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,30 @@
   push:
   pull_request:
 
 jobs:
   build:
     strategy:
       matrix:
-        python: ["3.8", "3.9", "3.10"]
+        python: ["3.8", "3.9", "3.10", "3.11"]
         platform: ["ubuntu-latest", "macos-latest", "windows-latest"]
     runs-on: ${{ matrix.platform }}
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python }}
       - name: Run test
         if: matrix.python == '3.8'
         run: cargo test --no-default-features --features pyo3/auto-initialize
       - uses: messense/maturin-action@v1
         with:
           command: build
-          args: --release -o dist -i python ${{ startsWith(matrix.platform, 'macos') && '--universal2' || '' }}
+          args: --release ${{ startsWith(matrix.platform, 'ubuntu') && startsWith(matrix.python, '3.8') && '--sdist' || '' }} -o dist -i python ${{ startsWith(matrix.platform, 'macos') && '--target universal2-apple-darwin' || '' }}
       - name: Run test
         if: matrix.python == '3.8' && !startsWith(matrix.platform, 'windows')
         run: |
           python -c "import subprocess, glob, os; file = glob.glob(os.path.join('dist', '*cp38*.whl'))[0]; subprocess.check_output(['pip', 'install', file])"
           pip install pytest
           mv rsoup rsoup2
           pytest -xs tests/
```

### Comparing `rsoup-3.0.1/.gitignore` & `rsoup-3.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/LICENSE` & `rsoup-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/benches/context_recursive_extractor_benchmark.rs` & `rsoup-3.0.2/benches/context_recursive_extractor_benchmark.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/benches/get_text.rs` & `rsoup-3.0.2/benches/get_text.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/pyproject.toml` & `rsoup-3.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rsoup"
-version = "3.0.1"
+version = "3.0.2"
 authors = [
   { name = "Binh Vu", email = "binh@toan2.com" },
 ]
 description = "A library for web scraper that handles text correctly and is very fast (Rust backend)"
 readme = "README.md"
 license = { file = "LICENSE" }
 
@@ -25,10 +25,13 @@
 [project.optional-dependencies]
 dev = [
     'pytest >= 7.1.3, < 8.0.0',
     'pytest-cov >= 4.0.0, < 5.0.0',
     'black >= 22.10.0, < 23.0.0',
 ]
 
+[tool.maturin]
+module-name = "rsoup.core"
+
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
```

### Comparing `rsoup-3.0.1/rsoup/core.pyi` & `rsoup-3.0.2/rsoup/core.pyi`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/rsoup/exceptions.py` & `rsoup-3.0.2/rsoup/exceptions.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/rsoup/fetch_tables.py` & `rsoup-3.0.2/rsoup/fetch_tables.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/rsoup/python/context_extractor.py` & `rsoup-3.0.2/rsoup/python/context_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/rsoup/python/models/context.py` & `rsoup-3.0.2/rsoup/python/models/context.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/rsoup/python/models/html_table.py` & `rsoup-3.0.2/rsoup/python/models/html_table.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/rsoup/python/table_extractor.py` & `rsoup-3.0.2/rsoup/python/table_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/scripts/gen_data.py` & `rsoup-3.0.2/scripts/gen_data.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/scripts/test_table_extractor.py` & `rsoup-3.0.2/scripts/test_table_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/error.rs` & `rsoup-3.0.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/extractors/context_v1.rs` & `rsoup-3.0.2/src/extractors/context_v1.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/extractors/mod.rs` & `rsoup-3.0.2/src/extractors/mod.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/extractors/table.rs` & `rsoup-3.0.2/src/extractors/table.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/extractors/text/get_rich_text.rs` & `rsoup-3.0.2/src/extractors/text/get_rich_text.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/extractors/text/get_text_v1.rs` & `rsoup-3.0.2/src/extractors/text/get_text_v1.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/extractors/text/get_text_v2.rs` & `rsoup-3.0.2/src/extractors/text/get_text_v2.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/extractors/text/line.rs` & `rsoup-3.0.2/src/extractors/text/line.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/extractors/text/mod.rs` & `rsoup-3.0.2/src/extractors/text/mod.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/lib.rs` & `rsoup-3.0.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/misc/mod.rs` & `rsoup-3.0.2/src/misc/mod.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/misc/recursive_iter.rs` & `rsoup-3.0.2/src/misc/recursive_iter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/misc/tree/iterator.rs` & `rsoup-3.0.2/src/misc/tree/iterator.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/misc/tree/simple_tree.rs` & `rsoup-3.0.2/src/misc/tree/simple_tree.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/misc/url_converter.rs` & `rsoup-3.0.2/src/misc/url_converter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/models/content_hierarchy.rs` & `rsoup-3.0.2/src/models/content_hierarchy.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/models/rich_text.rs` & `rsoup-3.0.2/src/models/rich_text.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/models/table/cell.rs` & `rsoup-3.0.2/src/models/table/cell.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/models/table/cell_iter.rs` & `rsoup-3.0.2/src/models/table/cell_iter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/models/table/row.rs` & `rsoup-3.0.2/src/models/table/row.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/models/table/row_iter.rs` & `rsoup-3.0.2/src/models/table/row_iter.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/src/models/table/table.rs` & `rsoup-3.0.2/src/models/table/table.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/conftest.py` & `rsoup-3.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/extractors/test_context_extractor.rs` & `rsoup-3.0.2/tests/extractors/test_context_extractor.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/extractors/test_table_extractor.py` & `rsoup-3.0.2/tests/extractors/test_table_extractor.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/extractors/test_table_extractor.rs` & `rsoup-3.0.2/tests/extractors/test_table_extractor.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/extractors/test_text_extractor.rs` & `rsoup-3.0.2/tests/extractors/test_text_extractor.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/models/test_table.rs` & `rsoup-3.0.2/tests/models/test_table.rs`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/models/test_table_pickle.py` & `rsoup-3.0.2/tests/models/test_table_pickle.py`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/resources/extractors/context/list_highest_mountains.html` & `rsoup-3.0.2/tests/resources/extractors/context/list_highest_mountains.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/resources/extractors/context/three-level.html` & `rsoup-3.0.2/tests/resources/extractors/context/three-level.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/resources/extractors/table.html` & `rsoup-3.0.2/tests/resources/extractors/table.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/resources/extractors/text.html` & `rsoup-3.0.2/tests/resources/extractors/text.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/resources/table_span.html` & `rsoup-3.0.2/tests/resources/table_span.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html` & `rsoup-3.0.2/tests/resources/wikipedia/2016_Nova_Scotia_municipal_elections.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html` & `rsoup-3.0.2/tests/resources/wikipedia/List_of_highest_mountains_on_Earth.html`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/Cargo.lock` & `rsoup-3.0.2/Cargo.lock`

 * *Files identical despite different names*

### Comparing `rsoup-3.0.1/PKG-INFO` & `rsoup-3.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsoup
-Version: 3.0.1
+Version: 3.0.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Dist: beautifulsoup4 >=4.9.3, <5.0.0
 Requires-Dist: html5lib >=1.1.0, <2.0.0
 Requires-Dist: requests >=2.28.0, <3.0.0
 Requires-Dist: tabulate >=0.8.10
 Requires-Dist: pytest >=7.1.3, <8.0.0 ; extra == 'dev'
```

