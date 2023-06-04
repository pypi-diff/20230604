# Comparing `tmp/can_message_data_generator-0.7.1.tar.gz` & `tmp/can_message_data_generator-0.7.3.tar.gz`

## Comparing `can_message_data_generator-0.7.1.tar` & `can_message_data_generator-0.7.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 can_message_data_generator-0.7.1/Cargo.toml
--rw-r--r--   0      501       20     6731 2023-06-04 18:31:29.000000 can_message_data_generator-0.7.1/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0      501       20      273 2023-06-04 17:14:16.000000 can_message_data_generator-0.7.1/.gitignore
--rwxr-xr-x   0      501       20      361 2023-06-04 17:08:17.000000 can_message_data_generator-0.7.1/build_and_install.sh
--rw-r--r--   0      501       20      388 2023-06-04 18:36:04.000000 can_message_data_generator-0.7.1/pyproject.toml
--rw-r--r--   0      501       20     6367 2023-06-04 18:27:18.000000 can_message_data_generator-0.7.1/reference.yml
--rw-r--r--   0      501       20      419 2023-06-04 18:38:48.000000 can_message_data_generator-0.7.1/src/lib.rs
--rw-r--r--   0      501       20    25257 2023-06-04 17:08:17.000000 can_message_data_generator-0.7.1/src/signal_generator.rs
--rw-r--r--   0      501       20     9707 2023-06-04 17:08:17.000000 can_message_data_generator-0.7.1/src/signal_type.rs
--rw-r--r--   0      501       20    11560 2023-06-04 18:39:54.000000 can_message_data_generator-0.7.1/Cargo.lock
--rw-r--r--   0        0        0      275 1970-01-01 00:00:00.000000 can_message_data_generator-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      597 1970-01-01 00:00:00.000000 can_message_data_generator-0.7.3/Cargo.toml
+-rw-r--r--   0      501       20     7328 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/.github/workflows/build_and_publish.yml
+-rw-r--r--   0      501       20      273 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/.gitignore
+-rw-r--r--   0      501       20      427 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/CONTRIBUTING.md
+-rw-r--r--   0      501       20      103 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/README.md
+-rwxr-xr-x   0      501       20      361 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/build_and_install.sh
+-rw-r--r--   0      501       20       10 2023-06-04 19:44:54.000000 can_message_data_generator-0.7.3/dist/can_message_data_generator-0.7.3.tar.gz
+-rw-r--r--   0      501       20      388 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/pyproject.toml
+-rw-r--r--   0      501       20      419 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/src/lib.rs
+-rw-r--r--   0      501       20    25257 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/src/signal_generator.rs
+-rw-r--r--   0      501       20     9707 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/src/signal_type.rs
+-rw-r--r--   0      501       20    11560 2023-06-04 19:44:34.000000 can_message_data_generator-0.7.3/Cargo.lock
+-rw-r--r--   0        0        0      448 1970-01-01 00:00:00.000000 can_message_data_generator-0.7.3/PKG-INFO
```

### Comparing `can_message_data_generator-0.7.1/Cargo.toml` & `can_message_data_generator-0.7.3/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "can-message-data-generator"
-version = "0.7.1"
+version = "0.7.3"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "can_message_data_generator"
 crate-type = ["cdylib"]
```

### Comparing `can_message_data_generator-0.7.1/.github/workflows/publish_to_pypi.yml` & `can_message_data_generator-0.7.3/.github/workflows/build_and_publish.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,54 @@
-name: Publish to PyPI
+name: Bulid and Publish
 
 on:
   push:
     branches:
       - main
   pull_request:
     branches:
       - main
 
+env:
+  PYTHON_VERSION: 3.7
+
 jobs:
   macos:
     runs-on: macos-latest
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: ${{ env.PYTHON_VERSION }}
           architecture: x64
 
       - uses: dtolnay/rust-toolchain@stable
 
       - name: Build Wheels -x86_64
         uses: PyO3/maturin-action@v1
         with:
           target: x86_64
           args: --release --out dist --sdist
 
       - name: Install Built Wheel - x86_64
         run: |
-          pip install simulated_signal_data --no-index --find-links dist --force-reinstall
-          python -c "import simulated_signal_data"
+          pip install can_message_data_generator --no-index --find-links dist --force-reinstall
+          python -c "import can_message_data_generator"
 
       - name: Build Wheels - universal2
         uses: PyO3/maturin-action@v1
         with:
           target: universal2-apple-darwin
           args: --release --out dist
 
       - name: Install Built Wheel - universal2
         run: |
-          pip install simulated_signal_data --no-index --find-links dist --force-reinstall
-          python -c "import simulated_signal_data"
+          pip install can_message_data_generator --no-index --find-links dist --force-reinstall
+          python -c "import can_message_data_generator"
 
       # Uploads to server to publish at the end
       - name: Upload Wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
@@ -56,29 +59,29 @@
       matrix:
         target: [x64, x86]
     steps:
       - uses: actions/checkout@v3
       
       - uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: ${{ env.PYTHON_VERSION }}
           architecture: ${{ matrix.target }}
 
       - uses: dtolnay/rust-toolchain@stable
 
       - name: Build Wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist
 
       - name: Install Built Wheel
         run: |
-          python -m pip install simulated_signal_data --no-index --find-links dist --force-reinstall
-          python -c "import simulated_signal_data"
+          python -m pip install can_message_data_generator --no-index --find-links dist --force-reinstall
+          python -c "import can_message_data_generator"
       
       # Uploads to server to publish at the end
       - name: Upload Wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
@@ -89,28 +92,34 @@
       matrix:
         target: [x86_64, i686]
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: ${{ env.PYTHON_VERSION }}
           architecture: x64
       
+      - name: Get Linker for 32 bit Architecture
+        if: matrix.target == 'i686'
+        run: |
+          sudo apt-get update
+          sudo apt-get install -y gcc-multilib
+      
       - name: Build Wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           args: --release --out dist
       
       - name: Install Built Wheel
         if: matrix.target == 'x86_64'
         run: |
-          python -m pip install simulated_signal_data --no-index --find-links dist --force-reinstall
-          python -c "import simulated_signal_data"
+          python -m pip install can_message_data_generator --no-index --find-links dist --force-reinstall
+          python -c "import can_message_data_generator"
       
       # Uploads to server to publish at the end
       - name: Upload Wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
@@ -121,15 +130,15 @@
       matrix:
         target: [aarch64, armv7, s390x, ppc64le, ppc64]
     steps:
       - uses: actions/checkout@v3
 
       - uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: ${{ env.PYTHON_VERSION }}
       
       - name: Build Wheels
         uses: PyO3/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           manylinux: auto
           args: --release --out dist
@@ -142,16 +151,16 @@
           distro: ubuntu20.04
           githubToken: ${{ github.token }}
           install: |
             apt-get update
             apt-get install -y --no-install-recommends python3 python3-pip
             pip3 install -U pip
           run: |
-            pip3 install simulated_signal_data --no-index --find-links dist --force-reinstall
-            python3 -c "import simulated_signal_data"
+            pip3 install can_message_data_generator --no-index --find-links dist --force-reinstall
+            python3 -c "import can_message_data_generator"
 
       - name: Upload Wheels
         uses: actions/upload-artifact@v3
         with:
           name: wheels
           path: dist
 
@@ -163,34 +172,35 @@
           - x86_64-unknown-linux-musl
           - i686-unknown-linux-musl
     steps:
     - uses: actions/checkout@v3
 
     - uses: actions/setup-python@v4
       with:
-        python-version: 3.7
+        python-version: ${{ env.PYTHON_VERSION }}
         architecture: x64
 
     - name: Build Wheels
       uses: PyO3/maturin-action@v1
       with:
         target: ${{ matrix.target }}
         manylinux: musllinux_1_2
         args: --release --out dist
 
     - name: Install Built Wheel
       if: matrix.target == 'x86_64-unknown-linux-musl'
       uses: addnab/docker-run-action@v3
       with:
         image: alpine:latest
+        options: -v ${{ github.workspace }}:/io -w /io
         run: |
           apk add py3-pip
           pip3 install -U pip
-          pip3 install simulated_signal_data --no-index --find-links dist --force-reinstall
-          python3 -c "import simulated_signal_data"
+          pip3 install can_message_data_generator --no-index --find-links /io/dist/ --force-reinstall
+          python3 -c "import can_message_data_generator"
 
     - name: Upload Wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
@@ -204,15 +214,15 @@
           - target: armv7-unknown-linux-musleabihf
             arch: armv7
     steps:
     - uses: actions/checkout@v3
 
     - uses: actions/setup-python@v4
       with:
-        python-version: 3.7
+        python-version: ${{ env.PYTHON_VERSION }}
 
     - name: Build Wheels
       uses: PyO3/maturin-action@v1
       with:
         target: ${{ matrix.platform.target }}
         manylinux: musllinux_1_2
         args: --release --out dist
@@ -223,35 +233,37 @@
         arch: ${{ matrix.platform.arch }}
         distro: alpine_latest
         githubToken: ${{ github.token }}
         install: |
           apk add py3-pip
           pip3 install -U pip
         run: |
-          pip3 install simulated_signal_data --no-index --find-links dist --force-reinstall
-          python3 -c "import simulated_signal_data"
+          pip3 install can_message_data_generator --no-index --find-links dist --force-reinstall
+          python3 -c "import can_message_data_generator"
 
     - name: Upload Wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
 
   release:
+    environment: production
     name: Release
+    if: github.ref == 'refs/heads/main' && github.event_name == 'push'
     runs-on: ubuntu-latest
     needs: [linux, macos, windows, musllinux, linux-cross, musllinux-cross]
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
 
       - uses: actions/setup-python@v4
         with:
-          python-version: 3.7
+          python-version: ${{ env.PYTHON_VERSION }}
 
       - name: Publish to PyPI
         env:
           TWINE_USERNAME: __token__
           TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
         run: |
           python -m pip install twine
```

### Comparing `can_message_data_generator-0.7.1/src/signal_generator.rs` & `can_message_data_generator-0.7.3/src/signal_generator.rs`

 * *Files identical despite different names*

### Comparing `can_message_data_generator-0.7.1/src/signal_type.rs` & `can_message_data_generator-0.7.3/src/signal_type.rs`

 * *Files identical despite different names*

### Comparing `can_message_data_generator-0.7.1/Cargo.lock` & `can_message_data_generator-0.7.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "can-message-data-generator"
-version = "0.7.1"
+version = "0.7.3"
 dependencies = [
  "pyo3",
  "rand",
  "serde",
  "serde_json",
  "serde_test",
  "strum",
```

