# Comparing `tmp/uk_postcodes_parsing-0.1.0.tar.gz` & `tmp/uk_postcodes_parsing-0.2.0.tar.gz`

## Comparing `uk_postcodes_parsing-0.1.0.tar` & `uk_postcodes_parsing-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/__init__.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/fix.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/postcode_utils.py
--rw-r--r--   0        0        0     5788 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/ukpostcode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/tests/test_all.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/tests/data/postcode_parse_test.csv
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/LICENSE
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/README.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6220 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/__init__.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/fix.py
+-rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/postcode_utils.py
+-rw-r--r--   0        0        0 20547700 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/postcodes_nov_2022.py
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/ukpostcode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/tests/test_all.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/tests/data/postcode_parse_test.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/README.md
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/PKG-INFO
```

### Comparing `uk_postcodes_parsing-0.1.0/.github/workflows/python-publish.yml` & `uk_postcodes_parsing-0.2.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.1.0/.github/workflows/test.yml` & `uk_postcodes_parsing-0.2.0/.github/workflows/test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -23,11 +23,11 @@
         run: |
           python -m pip install --upgrade pip
           pip install .
           pip install black pytest pandas
           if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
       - name: Lint check with black
         run: |
-          black src/uk_postcodes_parsing/ --check 
+          black src/uk_postcodes_parsing/ --check --exclude src/uk_postcodes_parsing/postcodes_nov_2022.py
       - name: Test with pytest
         run: |
           pytest -v
```

### Comparing `uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/fix.py` & `uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/fix.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/postcode_utils.py` & `uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/postcode_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """
 postcode_utils.py: Utilities for working with postcodes.
 """
 import re
 from typing import Union
 
-import requests
-
 # Tests for district
 DISTRICT_SPLIT_REGEX = re.compile(r"^([a-z]{1,2}\d)([a-z])$", re.I)
 
 # Tests for the unit section of a postcode
 UNIT_REGEX = re.compile(r"[a-z]{2}$", re.I)
 
 # Tests for the inward code section of a postcode
@@ -54,27 +52,14 @@
         outcode (str): The postcode to check
     Returns:
         bool: True if the postcode is valid, False otherwise
     """
     return re.match(OUTCODE_REGEX, outcode) is not None
 
 
-def check_with_postcode_io(postcode: str) -> bool:
-    """Check if the postcode is valid with postcodes.io
-
-    Args:
-        postcode (str): The postcode to check
-
-    Returns:
-        bool: True if the postcode is valid, False otherwise
-    """
-    response = requests.get(f"https://api.postcodes.io/postcodes/{postcode}").json()
-    return response["status"] == 200
-
-
 def to_normalised(postcode: str) -> Union[str, None]:
     """
     Normalises a postcode by removing whitespace, converting to uppercase, and formatting.
     Args:
         postcode (str): The postcode to normalise
     Returns:
         str: The normalised postcode
```

### Comparing `uk_postcodes_parsing-0.1.0/src/uk_postcodes_parsing/ukpostcode.py` & `uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/ukpostcode.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,29 +2,27 @@
 ukpostcode.py: main module for parsing UK postcodes from text.
 """
 import re
 import logging
 from dataclasses import dataclass, field
 from typing import Union, List, Optional
 
-import requests
-
 from uk_postcodes_parsing.postcode_utils import (
     is_valid,
-    check_with_postcode_io,
     to_normalised,
     to_outcode,
     to_incode,
     to_area,
     to_sector,
     to_unit,
     to_district,
     to_sub_district,
 )
 from uk_postcodes_parsing.fix import fix
+from uk_postcodes_parsing.postcodes_nov_2022 import POSTCODE_NOV_2022
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger("uk-postcodes-parsing")
 
 # Test for a valid postcode embedded in text
 POSTCODE_CORPUS_REGEX = re.compile(r"[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}", re.I)
 FIXABLE_POSTCODE_CORPUS_REGEX = re.compile(
@@ -43,22 +41,21 @@
         area (str): The area of the postcode.
         district (str): The district of the postcode.
         sub_district (str): The sub-district of the postcode.
         sector (str): The sector of the postcode.
         unit (str): The unit of the postcode.
 
     Additional attributes:
-        verified_against_postcode_io (bool): Whether the postcode was successfully verified against
-            postcode [api.postcodes.io/postcodes/](https://postcodes.io/) which uses the
+        is_in_ons_postcode_directory (bool): Whether the postcode was successfully verified against
             [ONS Postcode Directory](https://geoportal.statistics.gov.uk/datasets/489c152010a3425f80a71dc3663f73e1/about).
         fix_distance (int): The number of characters that the postcode string was corrected by the `fix` function during parsing.
     """
 
     # Calculate post initialization
-    verified_against_postcode_io: bool = field(init=False)
+    is_in_ons_postcode_directory: bool = field(init=False)
     fix_distance: int = field(init=False)
     # raw text
     original: str
     # The rest of the fields are parsed from the postcode using regex
     postcode: str
     incode: str
     outcode: str
@@ -66,33 +63,30 @@
     district: str
     sub_district: Union[str, None]
     sector: str
     unit: str
 
     def __post_init__(self):
         """calculate class attributes after initialization.
-        - `verified_against_postcode_io` (bool)
+        - `is_in_ons_postcode_directory` (bool)
         - `fix_distance` (int): the "edit distance" between the raw postcode and final postcode
         """
         # Convert raw (original) string in postcode format
         original = self.original.upper().strip().replace(r"\s+", "")
         inward = original[-3:].strip()
         outward = original[:-3].strip()
         formatted = f"{outward} {inward}"
 
         fix_distance = sum(c1 != c2 for c1, c2 in zip(formatted, self.postcode))
-        self.fix_distance = fix_distance
 
-        try:
-            self.verified_against_postcode_io = check_with_postcode_io(self.postcode)
-        except requests.exceptions.RequestException:
-            logger.error("Failed to check postcode against postcode.io")
+        self.fix_distance = fix_distance
+        self.is_in_ons_postcode_directory = is_in_ons_postcode_directory(self.postcode)
 
     def __eq__(self, other):
-        """Ignore verified_against_postcode_io and fix_distance."""
+        """Ignore is_in_ons_postcode_directory and fix_distance."""
         return (
             self.original == other.original
             and self.postcode == other.postcode
             and self.incode == other.incode
             and self.outcode == other.outcode
             and self.area == other.area
             and self.district == other.district
@@ -139,15 +133,15 @@
         return Postcode(**_parse(postcode), original=postcode)
     if attempt_fix:
         fixed = fix(postcode)
         if is_valid(fixed):
             logger.info("Postcode Fixed: '%s' => '%s'", postcode, fixed)
             return Postcode(**_parse(fixed), original=postcode)
         logger.error("Unable to fix postcode")
-    logger.error("Failed to parse postcode")
+    logger.error("Failed to parse postcode: %s", postcode)
     return None
 
 
 def parse_from_corpus(text: str, attempt_fix=False) -> List[str]:
     """Parse postcodes from a text corpus
 
     Args:
@@ -159,7 +153,19 @@
     """
     if attempt_fix:
         postcodes = re.findall(FIXABLE_POSTCODE_CORPUS_REGEX, text.lower())
     else:
         postcodes = re.findall(POSTCODE_CORPUS_REGEX, text.lower())
     logger.info("Found %d postcodes in corpus", len(postcodes))
     return list(map(parse, postcodes))
+
+
+def is_in_ons_postcode_directory(postcode: str) -> bool:
+    """Check if the postcode is valid with postcodes.io
+
+    Args:
+        postcode (str): The postcode to check
+
+    Returns:
+        bool: True if the postcode is valid, False otherwise
+    """
+    return postcode in POSTCODE_NOV_2022
```

### Comparing `uk_postcodes_parsing-0.1.0/tests/test_all.py` & `uk_postcodes_parsing-0.2.0/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.1.0/.gitignore` & `uk_postcodes_parsing-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.1.0/LICENSE` & `uk_postcodes_parsing-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.1.0/README.md` & `uk_postcodes_parsing-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 # uk-postcodes-parsing
 
 [![Test](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/test.yml/badge.svg)](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/test.yml) 
 [![Upload Python Package](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/python-publish.yml/badge.svg)](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/python-publish.yml)
 
-A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP.
+A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP.
 
 ## Install
 
 ```bash
 pip install uk-postcodes-parsing
 ```
 
 ## Capabilities
 
 - Search and parse UK postcode from text/OCR results
   - Extract parts of the postcode: incode, outcode etc.  
+  - Fix common mistakes in UK postcode OCR
 
 
 | Postcode | .outcode | .incode | .area | .district | .subDistrict | .sector | .unit |
 |----------|----------|---------|-------|-----------|--------------|---------|-------|
 | AA9A 9AA | AA9A     | 9AA     | AA    | AA9       | AA9A         | AA9A 9  | AA    |
 | A9A 9AA  | A9A      | 9AA     | A     | A9        | A9A          | A9A 9   | AA    |
 | A9 9AA   | A9       | 9AA     | A     | A9        | `None`       | A9 9    | AA    |
 | A99 9AA  | A99      | 9AA     | A     | A99       | `None`       | A99 9   | AA    |
 | AA9 9AA  | AA9      | 9AA     | AA    | AA9       | `None`       | AA9 9   | AA    |
 | AA99 9AA | AA99     | 9AA     | AA    | AA99      | `None`       | AA99 9  | AA    |  
 
-- Fix common mistakes in UK postcode
+
 - Utilities to validate postcode
+- NEW: Validate postcode against ~1.8M UK postcodes from the ONS Postcode Directory (Nov 2022)
 
 
 ## Usage
 
 - Parsing text to get a list of postcodes.
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
 >>> postcodes = ukpostcode.parse_from_corpus(corpus)
 INFO:uk-postcodes-parsing:Found 2 postcodes in corpus
->>> print(postcodes)
-[Postcode(verified_against_postcode_io=True, fix_distance=0, original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'), Postcode(verified_against_postcode_io=True, fix_distance=0, original='e3 4ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
+>>> postcodes
+[Postcode(is_in_ons_postcode_directory=True, fix_distance=0, original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'),
+ Postcode(is_in_ons_postcode_directory=True, fix_distance=0, original='e3 4ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
 ```
 
 - Optional auto-correct: Attempt correcting common mistakes in postcodes such as reading "O" and "0" and vice-versa.
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
@@ -54,21 +57,21 @@
 ```
 
 - Parsing
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> ukpostcode.parse("EC1r 1ub")
-Postcode(verified_against_postcode_io=True, fix_distance=0, original='EC1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
+Postcode(is_in_ons_postcode_directory=True, fix_distance=0, original='EC1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
 ```
 
 ```python
 >>> ukpostcode.parse("EH16 50Y")
 INFO:uk-postcodes-parsing:Postcode Fixed: 'EH16 50Y' => 'EH16 5OY'
-Postcode(verified_against_postcode_io=False, fix_distance=1, original='EH16 50Y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
+Postcode(is_in_ons_postcode_directory=False, fix_distance=1, original='EH16 50Y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
 ```
 
 ```python
 >>> ukpostcode.parse("EH16 50Y", attempt_fix=False) # Don't attempt fixes during parsing
 ERROR:uk-postcodes-parsing:Failed to parse postcode
 >>> ukpostcode.parse("0W1") 
 ERROR:uk-postcodes-parsing:Unable to fix postcode
@@ -89,21 +92,31 @@
 
 ```python
 >>> from uk_postcodes_parsing.fix import fix
 >>> fix("0W1 OAA") 
 'OW1 0AA'
 ```
 
+- Validate against ONS Postcode directory (1.7M+ UK postcode upto Nov 2022)
+
+```python
+>>> ukpostcode.is_in_ons_postcode_directory("EC1R 1UB") 
+True
+>>> ukpostcode.is_in_ons_postcode_directory("ec1r 1ub") # Expects normalised format (caps + space)
+False
+```
+
+
 # Postcode class definition
 
 ```python
 @dataclass(order=True)
 class Postcode:
     # Calculate post initialization
-    verified_against_postcode_io: bool = field(init=False)
+    is_in_ons_postcode_directory: bool = field(init=False)
     fix_distance: int = field(init=False)
     # raw text
     original: str 
     # The rest of the fields are parsed from the postcode using regex
     postcode: str
     incode: str
     outcode: str
@@ -112,23 +125,23 @@
     sub_district: Union[str, None]
     sector: str
     unit: str
 
 ```
 
 - 2 fileds calculated after init of class
-  - `verified_against_postcode_io`: Check against [`api.postcodes.io/postcodes/`](https://postcodes.io/) which uses the [ONS Postcode Directory](https://geoportal.statistics.gov.uk/datasets/489c152010a3425f80a71dc3663f73e1/about)
+  - `is_in_ons_postcode_directory`: Checked against the [ONS Postcode Directory](https://geoportal.statistics.gov.uk/datasets/489c152010a3425f80a71dc3663f73e1/about)
   - `fix_distance`: A measure of number of characters changed from raw text via auto-fix to get a valid post code. 
     - E.g. `SW1A OAA` => `SW1A 0AA` has fix_distance=1. Where as, `SWIA OAA` => `SW1A 0AA` has fix_distance=2.
   - These fields are particularly helpful using `parse_from_corpus` with `attempt_fix=True` which might return many potential postcodes. These field can be used as proxy for confidence on which parsed postcodes are correct.
 - `raw_text`: To keep track of the original string without formatting changes and auto-fixes.
 - 8 fileds are parsed using regex
 
 # Testing
 
 ```bash
 pytest tests/
 ```
 
-## Similar works
+## Similar work
 
-Most of this work is based on this JavaScript library: https://github.com/ideal-postcodes/postcode
+This package started as a Python replica of the postcode.io JavaScript library: https://github.com/ideal-postcodes/postcode
```

### Comparing `uk_postcodes_parsing-0.1.0/pyproject.toml` & `uk_postcodes_parsing-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uk_postcodes_parsing"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name="Anirudh Gangwal", email="angangwa@amazon.com" },
 ]
-dependencies = ["requests"]
-description = "A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP."
+description = "A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `uk_postcodes_parsing-0.1.0/PKG-INFO` & `uk_postcodes_parsing-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 Metadata-Version: 2.1
 Name: uk_postcodes_parsing
-Version: 0.1.0
-Summary: A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP.
+Version: 0.2.0
+Summary: A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP.
 Project-URL: Homepage, https://github.com/anirudhgangwal/ukpostcodes
 Project-URL: Bug Tracker, https://github.com/anirudhgangwal/ukpostcodes/issues
 Author-email: Anirudh Gangwal <angangwa@amazon.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
-Requires-Dist: requests
 Provides-Extra: lint
 Requires-Dist: black; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 # uk-postcodes-parsing
 
 [![Test](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/test.yml/badge.svg)](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/test.yml) 
 [![Upload Python Package](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/python-publish.yml/badge.svg)](https://github.com/anirudhgangwal/ukpostcodes/actions/workflows/python-publish.yml)
 
-A Python package to parge UK postcodes from text. Useful in applications such as OCR and IDP.
+A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP.
 
 ## Install
 
 ```bash
 pip install uk-postcodes-parsing
 ```
 
 ## Capabilities
 
 - Search and parse UK postcode from text/OCR results
   - Extract parts of the postcode: incode, outcode etc.  
+  - Fix common mistakes in UK postcode OCR
 
 
 | Postcode | .outcode | .incode | .area | .district | .subDistrict | .sector | .unit |
 |----------|----------|---------|-------|-----------|--------------|---------|-------|
 | AA9A 9AA | AA9A     | 9AA     | AA    | AA9       | AA9A         | AA9A 9  | AA    |
 | A9A 9AA  | A9A      | 9AA     | A     | A9        | A9A          | A9A 9   | AA    |
 | A9 9AA   | A9       | 9AA     | A     | A9        | `None`       | A9 9    | AA    |
 | A99 9AA  | A99      | 9AA     | A     | A99       | `None`       | A99 9   | AA    |
 | AA9 9AA  | AA9      | 9AA     | AA    | AA9       | `None`       | AA9 9   | AA    |
 | AA99 9AA | AA99     | 9AA     | AA    | AA99      | `None`       | AA99 9  | AA    |  
 
-- Fix common mistakes in UK postcode
+
 - Utilities to validate postcode
+- NEW: Validate postcode against ~1.8M UK postcodes from the ONS Postcode Directory (Nov 2022)
 
 
 ## Usage
 
 - Parsing text to get a list of postcodes.
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
 >>> postcodes = ukpostcode.parse_from_corpus(corpus)
 INFO:uk-postcodes-parsing:Found 2 postcodes in corpus
->>> print(postcodes)
-[Postcode(verified_against_postcode_io=True, fix_distance=0, original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'), Postcode(verified_against_postcode_io=True, fix_distance=0, original='e3 4ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
+>>> postcodes
+[Postcode(is_in_ons_postcode_directory=True, fix_distance=0, original='ec1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB'),
+ Postcode(is_in_ons_postcode_directory=True, fix_distance=0, original='e3 4ss', postcode='E3 4SS', incode='4SS', outcode='E3', area='E', district='E3', sub_district=None, sector='E3 4', unit='SS')]
 ```
 
 - Optional auto-correct: Attempt correcting common mistakes in postcodes such as reading "O" and "0" and vice-versa.
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> corpus = "this is a check to see if we can get post codes liek thia ec1r 1ub , and that e3 4ss. But also eh16 50y and ei412"          
@@ -74,21 +76,21 @@
 ```
 
 - Parsing
 
 ```python
 >>> from uk_postcodes_parsing import ukpostcode
 >>> ukpostcode.parse("EC1r 1ub")
-Postcode(verified_against_postcode_io=True, fix_distance=0, original='EC1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
+Postcode(is_in_ons_postcode_directory=True, fix_distance=0, original='EC1r 1ub', postcode='EC1R 1UB', incode='1UB', outcode='EC1R', area='EC', district='EC1', sub_district='EC1R', sector='EC1R 1', unit='UB')
 ```
 
 ```python
 >>> ukpostcode.parse("EH16 50Y")
 INFO:uk-postcodes-parsing:Postcode Fixed: 'EH16 50Y' => 'EH16 5OY'
-Postcode(verified_against_postcode_io=False, fix_distance=1, original='EH16 50Y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
+Postcode(is_in_ons_postcode_directory=False, fix_distance=1, original='EH16 50Y', postcode='EH16 5OY', incode='5OY', outcode='EH16', area='EH', district='EH16', sub_district=None, sector='EH16 5', unit='OY')
 ```
 
 ```python
 >>> ukpostcode.parse("EH16 50Y", attempt_fix=False) # Don't attempt fixes during parsing
 ERROR:uk-postcodes-parsing:Failed to parse postcode
 >>> ukpostcode.parse("0W1") 
 ERROR:uk-postcodes-parsing:Unable to fix postcode
@@ -109,21 +111,31 @@
 
 ```python
 >>> from uk_postcodes_parsing.fix import fix
 >>> fix("0W1 OAA") 
 'OW1 0AA'
 ```
 
+- Validate against ONS Postcode directory (1.7M+ UK postcode upto Nov 2022)
+
+```python
+>>> ukpostcode.is_in_ons_postcode_directory("EC1R 1UB") 
+True
+>>> ukpostcode.is_in_ons_postcode_directory("ec1r 1ub") # Expects normalised format (caps + space)
+False
+```
+
+
 # Postcode class definition
 
 ```python
 @dataclass(order=True)
 class Postcode:
     # Calculate post initialization
-    verified_against_postcode_io: bool = field(init=False)
+    is_in_ons_postcode_directory: bool = field(init=False)
     fix_distance: int = field(init=False)
     # raw text
     original: str 
     # The rest of the fields are parsed from the postcode using regex
     postcode: str
     incode: str
     outcode: str
@@ -132,23 +144,23 @@
     sub_district: Union[str, None]
     sector: str
     unit: str
 
 ```
 
 - 2 fileds calculated after init of class
-  - `verified_against_postcode_io`: Check against [`api.postcodes.io/postcodes/`](https://postcodes.io/) which uses the [ONS Postcode Directory](https://geoportal.statistics.gov.uk/datasets/489c152010a3425f80a71dc3663f73e1/about)
+  - `is_in_ons_postcode_directory`: Checked against the [ONS Postcode Directory](https://geoportal.statistics.gov.uk/datasets/489c152010a3425f80a71dc3663f73e1/about)
   - `fix_distance`: A measure of number of characters changed from raw text via auto-fix to get a valid post code. 
     - E.g. `SW1A OAA` => `SW1A 0AA` has fix_distance=1. Where as, `SWIA OAA` => `SW1A 0AA` has fix_distance=2.
   - These fields are particularly helpful using `parse_from_corpus` with `attempt_fix=True` which might return many potential postcodes. These field can be used as proxy for confidence on which parsed postcodes are correct.
 - `raw_text`: To keep track of the original string without formatting changes and auto-fixes.
 - 8 fileds are parsed using regex
 
 # Testing
 
 ```bash
 pytest tests/
 ```
 
-## Similar works
+## Similar work
 
-Most of this work is based on this JavaScript library: https://github.com/ideal-postcodes/postcode
+This package started as a Python replica of the postcode.io JavaScript library: https://github.com/ideal-postcodes/postcode
```

