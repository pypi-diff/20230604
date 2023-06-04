# Comparing `tmp/uk_postcodes_parsing-0.2.0.tar.gz` & `tmp/uk_postcodes_parsing-0.3.0.tar.gz`

## Comparing `uk_postcodes_parsing-0.2.0.tar` & `uk_postcodes_parsing-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/__init__.py
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/fix.py
--rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/postcode_utils.py
--rw-r--r--   0        0        0 20547700 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/postcodes_nov_2022.py
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/ukpostcode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/tests/test_all.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/tests/data/postcode_parse_test.csv
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/LICENSE
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/README.md
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/__init__.py
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/fix.py
+-rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/postcode_utils.py
+-rw-r--r--   0        0        0 20547700 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/postcodes_nov_2022.py
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/ukpostcode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/tests/test_all.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/tests/data/postcode_parse_test.csv
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8785 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/README.md
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9591 2020-02-02 00:00:00.000000 uk_postcodes_parsing-0.3.0/PKG-INFO
```

### Comparing `uk_postcodes_parsing-0.2.0/.github/workflows/python-publish.yml` & `uk_postcodes_parsing-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.2.0/.github/workflows/test.yml` & `uk_postcodes_parsing-0.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/fix.py` & `uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/fix.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/postcode_utils.py` & `uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/postcode_utils.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/postcodes_nov_2022.py` & `uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/postcodes_nov_2022.py`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.2.0/src/uk_postcodes_parsing/ukpostcode.py` & `uk_postcodes_parsing-0.3.0/src/uk_postcodes_parsing/ukpostcode.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,18 @@
 
 # Test for a valid postcode embedded in text
 POSTCODE_CORPUS_REGEX = re.compile(r"[a-z]{1,2}\d[a-z\d]?\s*\d[a-z]{2}", re.I)
 FIXABLE_POSTCODE_CORPUS_REGEX = re.compile(
     r"[a-z01]{1,2}[0-9oi][a-z\d]?\s*[0-9oi][a-z01]{2}"
 )
 
+SPECIAL_CASE_POSTCODES = ("GIR", "NPT", "BX", "BF")
+
+logger.debug("Imported POSTCODE_NOV_2022 with length: %s", len(POSTCODE_NOV_2022))
+
 
 @dataclass(order=True)
 class Postcode:
     """Class to hold the parsed postcode.
     Constructor arguments:
         original (str): The raw (original) string of the postcode.
         postcode (str): The postcode as a string.
@@ -43,15 +47,16 @@
         sub_district (str): The sub-district of the postcode.
         sector (str): The sector of the postcode.
         unit (str): The unit of the postcode.
 
     Additional attributes:
         is_in_ons_postcode_directory (bool): Whether the postcode was successfully verified against
             [ONS Postcode Directory](https://geoportal.statistics.gov.uk/datasets/489c152010a3425f80a71dc3663f73e1/about).
-        fix_distance (int): The number of characters that the postcode string was corrected by the `fix` function during parsing.
+        fix_distance (int): The number of characters that the postcode string was corrected by the
+            `fix` function during parsing.
     """
 
     # Calculate post initialization
     is_in_ons_postcode_directory: bool = field(init=False)
     fix_distance: int = field(init=False)
     # raw text
     original: str
@@ -72,15 +77,15 @@
         """
         # Convert raw (original) string in postcode format
         original = self.original.upper().strip().replace(r"\s+", "")
         inward = original[-3:].strip()
         outward = original[:-3].strip()
         formatted = f"{outward} {inward}"
 
-        fix_distance = sum(c1 != c2 for c1, c2 in zip(formatted, self.postcode))
+        fix_distance = sum(c1 != c2 for c1, c2 in zip(formatted, self.postcode)) * -1
 
         self.fix_distance = fix_distance
         self.is_in_ons_postcode_directory = is_in_ons_postcode_directory(self.postcode)
 
     def __eq__(self, other):
         """Ignore is_in_ons_postcode_directory and fix_distance."""
         return (
@@ -100,16 +105,14 @@
     """Internal function to parse postcode string using `uk_postcodes_parsing.postcode_utils`
 
     Args:
         postcode (str): Postcode to parse. E.g. "EC1R 1UB".
     Returns:
         dict: Parsed postcode.
     """
-    if postcode.upper().startswith("NPT"):  # Edge case logging
-        logger.warning("Found 'NPT' Newport postcode discontinued in 1984.")
     if not is_valid(postcode):
         return None
     return {
         "postcode": to_normalised(postcode),
         "incode": to_incode(postcode),
         "outcode": to_outcode(postcode),
         "area": to_area(postcode),
@@ -125,14 +128,16 @@
 
     Args:
         postcode (str): Postcode to parse. E.g. "EC1R 1UB".
         attempt_fix (bool): Attempt to fix postcodes. Defaults to True.
     Returns:
         Postcode: Parsed postcode.
     """
+    if postcode.strip().upper().startswith(SPECIAL_CASE_POSTCODES):  # Edge case logging
+        logger.info("Found special case postcode: %s", postcode)
     if is_valid(postcode):
         return Postcode(**_parse(postcode), original=postcode)
     if attempt_fix:
         fixed = fix(postcode)
         if is_valid(fixed):
             logger.info("Postcode Fixed: '%s' => '%s'", postcode, fixed)
             return Postcode(**_parse(fixed), original=postcode)
```

### Comparing `uk_postcodes_parsing-0.2.0/tests/test_all.py` & `uk_postcodes_parsing-0.3.0/tests/test_all.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -147,51 +147,51 @@
 
 
 def test_sort_by_fix_distance():
     corpus = "this EC1r 1ub followed by to one, ecir iub e0 i00"
     lst = parse_from_corpus(corpus, attempt_fix=True)
     assert sorted(lst, reverse=True) == [
         Postcode(
-            original="ecir iub",
+            original="ec1r 1ub",
             postcode="EC1R 1UB",
             incode="1UB",
             outcode="EC1R",
             area="EC",
             district="EC1",
             sub_district="EC1R",
             sector="EC1R 1",
             unit="UB",
         ),
         Postcode(
-            original="ec1r 1ub",
+            original="ecir iub",
             postcode="EC1R 1UB",
             incode="1UB",
             outcode="EC1R",
             area="EC",
             district="EC1",
             sub_district="EC1R",
             sector="EC1R 1",
             unit="UB",
         ),
         Postcode(
-            original="e0 i00",
-            postcode="E0 1OO",
-            incode="1OO",
-            outcode="E0",
-            area="E",
-            district="E0",
-            sub_district=None,
-            sector="E0 1",
-            unit="OO",
-        ),
-        Postcode(
             original="to one",
             postcode="T0 0NE",
             incode="0NE",
             outcode="T0",
             area="T",
             district="T0",
             sub_district=None,
             sector="T0 0",
             unit="NE",
         ),
+        Postcode(
+            original="e0 i00",
+            postcode="E0 1OO",
+            incode="1OO",
+            outcode="E0",
+            area="E",
+            district="E0",
+            sub_district=None,
+            sector="E0 1",
+            unit="OO",
+        ),
     ]
```

### Comparing `uk_postcodes_parsing-0.2.0/.gitignore` & `uk_postcodes_parsing-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.2.0/LICENSE` & `uk_postcodes_parsing-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uk_postcodes_parsing-0.2.0/pyproject.toml` & `uk_postcodes_parsing-0.3.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uk_postcodes_parsing"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
   { name="Anirudh Gangwal", email="angangwa@amazon.com" },
 ]
 description = "A Python package to parse UK postcodes from text. Useful in applications such as OCR and IDP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
-test = ["pytest", "pytest-cov"]
+test = ["pytest", "pytest-cov", "bandit[toml]"]
 lint = [ "black"]
 
 [project.urls]
 "Homepage" = "https://github.com/anirudhgangwal/ukpostcodes"
 "Bug Tracker" = "https://github.com/anirudhgangwal/ukpostcodes/issues"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
 testpaths = [
     "tests/",
 ]
+
+[tool.bandit]
+skips = ["B101"]
```

