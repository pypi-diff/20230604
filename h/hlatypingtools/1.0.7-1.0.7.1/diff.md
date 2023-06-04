# Comparing `tmp/hlatypingtools-1.0.7.tar.gz` & `tmp/hlatypingtools-1.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hlatypingtools-1.0.7.tar", max compression
+gzip compressed data, was "hlatypingtools-1.0.7.1.tar", max compression
```

## Comparing `hlatypingtools-1.0.7.tar` & `hlatypingtools-1.0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       59 2023-04-15 19:16:13.832019 hlatypingtools-1.0.7/hlatypingtools/__init__.py
--rw-r--r--   0        0        0   180071 2023-06-04 13:09:44.956765 hlatypingtools-1.0.7/hlatypingtools/data/data.pickle.aes
--rw-r--r--   0        0        0      816 2023-04-18 09:05:19.478359 hlatypingtools-1.0.7/hlatypingtools/decrypt_file.py
--rw-r--r--   0        0        0     3055 2023-06-04 12:55:07.121304 hlatypingtools-1.0.7/hlatypingtools/get_info.py
--rw-r--r--   0        0        0      529 2023-06-04 13:13:02.826536 hlatypingtools-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     2807 2023-04-15 19:16:52.738119 hlatypingtools-1.0.7/README.md
--rw-r--r--   0        0        0     3557 1970-01-01 00:00:00.000000 hlatypingtools-1.0.7/setup.py
--rw-r--r--   0        0        0     3265 1970-01-01 00:00:00.000000 hlatypingtools-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0       99 2023-06-04 13:16:17.488420 hlatypingtools-1.0.7.1/hlatypingtools/__init__.py
+-rw-r--r--   0        0        0   180071 2023-06-04 13:09:44.956765 hlatypingtools-1.0.7.1/hlatypingtools/data/data.pickle.aes
+-rw-r--r--   0        0        0      816 2023-04-18 09:05:19.478359 hlatypingtools-1.0.7.1/hlatypingtools/decrypt_file.py
+-rw-r--r--   0        0        0     3055 2023-06-04 12:55:07.121304 hlatypingtools-1.0.7.1/hlatypingtools/get_info.py
+-rw-r--r--   0        0        0      531 2023-06-04 13:16:53.535965 hlatypingtools-1.0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2807 2023-04-15 19:16:52.738119 hlatypingtools-1.0.7.1/README.md
+-rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 hlatypingtools-1.0.7.1/setup.py
+-rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 hlatypingtools-1.0.7.1/PKG-INFO
```

### Comparing `hlatypingtools-1.0.7/hlatypingtools/data/data.pickle.aes` & `hlatypingtools-1.0.7.1/hlatypingtools/data/data.pickle.aes`

 * *Files identical despite different names*

### Comparing `hlatypingtools-1.0.7/hlatypingtools/decrypt_file.py` & `hlatypingtools-1.0.7.1/hlatypingtools/decrypt_file.py`

 * *Files identical despite different names*

### Comparing `hlatypingtools-1.0.7/hlatypingtools/get_info.py` & `hlatypingtools-1.0.7.1/hlatypingtools/get_info.py`

 * *Files identical despite different names*

### Comparing `hlatypingtools-1.0.7/pyproject.toml` & `hlatypingtools-1.0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hlatypingtools"
-version = "1.0.7"
+version = "1.0.7.1"
 description = ""
 authors = ["JasonMendoza2008 <lhotteromain@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^2.0.0"
```

### Comparing `hlatypingtools-1.0.7/README.md` & `hlatypingtools-1.0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `hlatypingtools-1.0.7/setup.py` & `hlatypingtools-1.0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['hlatypingtools']
 
 package_data = \
-{'': ['*'], 'hlatypingtools': ['data/data.pickle.aes']}
+{'': ['*'], 'hlatypingtools': ['data/*']}
 
 install_requires = \
 ['openpyxl>=3.1.2,<4.0.0',
  'pandas-stubs>=2.0.0.230412,<3.0.0.0',
  'pandas>=2.0.0,<3.0.0',
  'pyaescrypt>=6.0.0,<7.0.0']
 
 setup_kwargs = {
     'name': 'hlatypingtools',
-    'version': '1.0.7',
+    'version': '1.0.7.1',
     'description': '',
     'long_description': '# HLATypingTools\n\n## Getting Started\n#### Install from PyPI (recommended)\nTo use `HLATypingTools`, run `pip install HLATypingTools` in your terminal.\nAll python packages necessary for `HLATypingTools` will automatically be downloaded.\n\n#### Usage\nIf you haven\'t decrypted the data yet (first time you are using the package and you did request access to the product),\nrun:\n```py\nfrom hlatypingtools.decrypt_file import decrypt_file\n\npassword: str = "___"   # Replace with password provided by the author \ndecrypt_file(password)\n```\nIt should print `File decrypted successfully`.\n\nThen you can use the package as follows:\n```py\nfrom hlatypingtools.get_info import get_allele_info\n\nallele: str = "A*01:01"\nprint(get_allele_info(allele, "Broad"))  # will output A1\nprint(get_allele_info(allele, "G Group"))  # will output A*01:01:01G\nprint(get_allele_info(allele, "P Group"))  # will output A*01:01P\nprint(get_allele_info(allele, "% locus"))  # will output 11.906\n```\n\nOr as follows:\n```py\nfrom hlatypingtools.get_info import get_locus\nprint(get_locus("A*01:01"))  # will output HLA_A\n```\n\nOr as follows to output all possible high-resolution alleles for a given low-resolution typing:\n```py\nfrom hlatypingtools.get_info import get_same_low_res_broad, get_same_low_res_assigned_type\nbroad = "DQ3"\nprint("DQB1*03:01" in get_same_low_res_broad(broad))  # will output True\nprint("DQB1*03:02" in get_same_low_res_broad(broad))  # will output True\n\nassigned_type = "DQ7"\nprint("DQB1*03:01" in get_same_low_res_assigned_type(assigned_type))  # will output True\nprint("DQB1*03:02" in get_same_low_res_assigned_type(assigned_type))  # will output False\n```\nNote:\n- Broad = something like A1, B7, Cw1, DR1, **DQ3** (!!!), DQA1&ast;01, DR52, DPB1&ast;01, or DPA1&ast;01\n- Assigned Type = something like A1, B7, Cw1, DR1, **DQ7** (!!!), DQA1&ast;01, DR52, DPB1&ast;01, or DPA1&ast;01\n\n#### Exit codes\n```\n0: Wrong password.\n1: Tried to acess the functions of the package without decrypting the data first.\n2: type_info requested is not available.\n3: wrong format for a low-resolution input. Has to be of the form A1, B7, Cw1, DR1, DQ3, DQA1*01, DR52, DPB1*01, or \nDPA1*01.\n```\n\n## About the source code\n- Follows [PEP8](https://peps.python.org/pep-0008/) Style Guidelines.\n- All functions are unit-tested with [pytest](https://docs.pytest.org/en/stable/).\n- All variables are correctly type-hinted, reviewed with [static type checker](https://mypy.readthedocs.io/en/stable/)\n`mypy`.\n- All functions are documented with [docstrings](https://www.python.org/dev/peps/pep-0257/).\n\n\n## Useful links:\n- [Corresponding GitHub repository](https://github.com/JasonMendoza2008/HLATypingTools)\n- [Corresponding PyPI page](https://pypi.org/project/HLATypingTools)\n',
     'author': 'JasonMendoza2008',
     'author_email': 'lhotteromain@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `hlatypingtools-1.0.7/PKG-INFO` & `hlatypingtools-1.0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hlatypingtools
-Version: 1.0.7
+Version: 1.0.7.1
 Summary: 
 Author: JasonMendoza2008
 Author-email: lhotteromain@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

