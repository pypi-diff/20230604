# Comparing `tmp/tercol-0.1.3.tar.gz` & `tmp/tercol-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tercol-0.1.3.tar", last modified: Wed Oct 26 22:35:27 2022, max compression
+gzip compressed data, was "tercol-0.1.4.tar", last modified: Sat Jun  3 23:52:20 2023, max compression
```

## Comparing `tercol-0.1.3.tar` & `tercol-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-10-26 22:35:27.640773 tercol-0.1.3/
--rw-rw-rw-   0        0        0     1059 2022-09-10 20:23:17.000000 tercol-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2022-09-10 20:58:48.000000 tercol-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1685 2022-10-26 22:35:27.640773 tercol-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      934 2022-10-23 19:07:36.000000 tercol-0.1.3/README.md
--rw-rw-rw-   0        0        0      818 2022-10-26 22:33:44.000000 tercol-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-26 22:35:27.640773 tercol-0.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-26 22:35:27.633792 tercol-0.1.3/tercol/
--rw-rw-rw-   0        0        0    11545 2022-10-23 18:33:47.000000 tercol-0.1.3/tercol/__init__.py
--rw-rw-rw-   0        0        0      530 2022-10-23 18:33:57.000000 tercol-0.1.3/tercol/__main__.py
-drwxrwxrwx   0        0        0        0 2022-10-26 22:35:27.638779 tercol-0.1.3/tercol.egg-info/
--rw-rw-rw-   0        0        0     1685 2022-10-26 22:35:27.000000 tercol-0.1.3/tercol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2022-10-26 22:35:27.000000 tercol-0.1.3/tercol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-26 22:35:27.000000 tercol-0.1.3/tercol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-10-26 22:35:27.000000 tercol-0.1.3/tercol.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-03 23:52:20.534211 tercol-0.1.4/
+-rw-rw-rw-   0        0        0     1094 2023-06-03 22:41:35.000000 tercol-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       25 2023-06-01 22:00:38.000000 tercol-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1837 2023-06-03 23:52:20.534211 tercol-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-06-03 23:44:17.000000 tercol-0.1.4/README.md
+-rw-rw-rw-   0        0        0      817 2023-06-03 22:46:49.000000 tercol-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-03 23:52:20.534211 tercol-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-03 23:52:20.528228 tercol-0.1.4/tercol/
+-rw-rw-rw-   0        0        0    12136 2023-06-03 22:52:59.000000 tercol-0.1.4/tercol/__init__.py
+-rw-rw-rw-   0        0        0      886 2023-06-03 23:51:18.000000 tercol-0.1.4/tercol/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-03 23:52:20.533213 tercol-0.1.4/tercol.egg-info/
+-rw-rw-rw-   0        0        0     1837 2023-06-03 23:52:20.000000 tercol-0.1.4/tercol.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-03 23:52:20.000000 tercol-0.1.4/tercol.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-03 23:52:20.000000 tercol-0.1.4/tercol.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-03 23:52:20.000000 tercol-0.1.4/tercol.egg-info/top_level.txt
```

### Comparing `tercol-0.1.3/LICENSE.txt` & `tercol-0.1.4/LICENSE`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,21 @@
-Copyright 2022 Sultan Marzouq
+MIT License
 
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+Copyright (c) 2022-2023 Butterroach
 
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tercol-0.1.3/pyproject.toml` & `tercol-0.1.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tercol"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
-  { name="Sultan Marzouq", email="epicnoobcontactemail@gmail.com" },
+  { name="Butterroach", email="epicnoobcontactemail@gmail.com" },
 ]
 description = "TerCol is a useless library that colors your text."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.6"
 keywords = ["terminal styling", "colors", "style"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://butterroach.github.io/tercol"
 "Bug Tracker" = "https://github.com/butterroach/tercol/issues"
-"Source Code" = "https://github.com/butterroach/tercol"
+"Source Code" = "https://github.com/butterroach/tercol"
```

### Comparing `tercol-0.1.3/tercol/__init__.py` & `tercol-0.1.4/tercol/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-"""TerCol, a useless library that colors text.
-Copyright 2022 Sultan Marzouq"""
+"""
+TerCol, a library that colors text.
+"""
 
 # Imports
 from os import system as execc
 
 # DISABLE THIS TO STOP IT FROM DOING os.system('')
 autoOsSystem = True
 
@@ -31,14 +32,15 @@
 __sblink = "\u001b[5m"
 __sanotherblink = "\u001b[6m"  # I dunno what the difference between 5m and 6m is but they both blink so I'm adding this just in case someone needs it
 __sfadedout = "\u001b[2m"
 __sunderlined = "\u001b[4m"
 __sinverted = " \u001b[7m"
 __endcolor = "\u001b[0m"
 
+
 # hsv to rgb
 def hsv_to_rgb(h, s, v):
     """
     THIS IS NOT IMPORTANT AND YOU WILL NOT NEED TO USE THIS IN YOUR CODE. This is just colorsys.hsv_to_rgb(). I am defining this instead of importing colorsys to achieve compatability.
     """
     if s == 0.0:
         return v, v, v
@@ -62,15 +64,15 @@
         return v, p, q
     # Cannot get here
 
 
 # RGB
 def rgb(r, g, b, text):
     """
-    Takes 4 values, the red, the blue, the green and the text. The color is based on what rgb you inputed.
+    Takes 4 values, the red, the green, the blue and the text. The color is based on what rgb you inputed.
     """
     if autoOsSystem:
         execc("")
     return f"\u001b[38;2;{r};{g};{b}m{text}{__endcolor}"
 
 
 def bgrgb(r, g, b, text):
@@ -79,18 +81,34 @@
     """
     if autoOsSystem:
         execc("")
     return f"\u001b[48;2;{r};{g};{b}m{text}{__endcolor}"
 
 
 # Hex
-def hex(hex: str, text):
+def hexa(hexa, text):
     """
     Takes a hex code and a text, converts it to rgb and uses the existing rgb function in this library.
     """
+
+    try:
+        if isinstance(hexa, int):
+            hexa = hex(hexa)[2:]
+            if len(hexa) != 6:
+                while len(hexa) != 6:
+                    hexa = "0" + hexa
+
+    except TypeError as exc:
+        raise TypeError(
+            red(
+                underlined(
+                    f"Expected 'int' (HEXADECIMAL NUMBERS ARE INTEGERS) or 'str' for 'hexa' argument, got '{type(hexa).__name__}'"
+                )
+            )
+        ) from exc
     try:
         RGBHEX = [
             "0",
             "1",
             "2",
             "3",
             "4",
@@ -102,91 +120,101 @@
             "a",
             "b",
             "c",
             "d",
             "e",
             "f",
         ]
-        hexcode = hex.replace("#", "").casefold()
+        hexcode = hexa.replace("#", "").casefold()
         hexr = int(RGBHEX.index(hexcode[0])) * 16
         hexr += int(RGBHEX.index(hexcode[1]))
         hexg = int(RGBHEX.index(hexcode[2])) * 16
         hexg += int(RGBHEX.index(hexcode[3]))
         hexb = int(RGBHEX.index(hexcode[4])) * 16
         hexb += int(RGBHEX.index(hexcode[5]))
         return rgb(hexr, hexg, hexb, text)
-    except IndexError:
-        raise Exception(red(underlined("Uh oh, invalid hex code...")))
-    except ValueError:
-        raise Exception(red(underlined("Uh oh, invalid hex code...")))
-    except TypeError:
-        raise Exception(
+    except (IndexError, ValueError) as exc:
+        raise ValueError(red(underlined("'hexa' argument is invalid"))) from exc
+    except TypeError as exc:
+        raise TypeError(
             red(
                 underlined(
-                    "Hex code can't be an actual hexdecimal input. Why? This is due to how the code works."
+                    f"Expected 'int' (HEXADECIMAL NUMBERS ARE INTEGERS) or 'str' for 'hexa' argument, got '{type(hexa).__name__}'"
                 )
             )
-        )
+        ) from exc
 
 
-def bghex(hex: str, text):
+def bghexa(hexa, text):
     """
     Same thing as hex(hex, text) but it colors the background instead.
     """
     try:
+        if isinstance(hexa, int):
+            hexa = hex(hexa)[2:]
+            if len(hexa) != 6:
+                while len(hexa) != 6:
+                    hexa = "0" + hexa
+    except TypeError as exc:
+        raise TypeError(
+            red(
+                underlined(
+                    f"Expected 'int' (HEXADECIMAL NUMBERS ARE INTEGERS) or 'str' for 'hexa' argument, got '{type(hexa).__name__}'"
+                )
+            )
+        ) from exc
+    try:
         RGBHEX = [
             "0",
             "1",
             "2",
             "3",
             "4",
             "5",
             "6",
             "7",
             "8",
             "9",
-            "A",
-            "B",
-            "C",
-            "D",
-            "E",
-            "F",
+            "a",
+            "b",
+            "c",
+            "d",
+            "e",
+            "f",
         ]
-        hexcode = hex
+        hexcode = hexa.replace("#", "").casefold()
         hexr = int(RGBHEX.index(hexcode[0])) * 16
         hexr += int(RGBHEX.index(hexcode[1]))
         hexg = int(RGBHEX.index(hexcode[2])) * 16
         hexg += int(RGBHEX.index(hexcode[3]))
         hexb = int(RGBHEX.index(hexcode[4])) * 16
         hexb += int(RGBHEX.index(hexcode[5]))
         return bgrgb(hexr, hexg, hexb, text)
-    except IndexError:
-        raise Exception(red(underlined("Uh oh, invalid hex code...")))
-    except ValueError:
-        raise Exception(red(underlined("Uh oh, invalid hex code...")))
-    except TypeError:
-        raise Exception(
+    except (IndexError, ValueError) as exc:
+        raise ValueError(red(underlined("Uh oh, invalid hex code..."))) from exc
+    except TypeError as exc:
+        raise TypeError(
             red(
                 underlined(
-                    "Hex code can't be an actual hexadecimal input. Why? This is due to how the code works."
+                    f"Expected 'int' (HEXADECIMAL NUMBERS ARE INTEGERS) for 'hexa' argument, got '{type(hexa).__name__}'"
                 )
             )
-        )
+        ) from exc
 
 
 # HSV
 def hsv(h, s, v, text):
     """
     Takes a hue, saturation, and value, and then converts it to RGB, and returns the value of rgb(ConvertedHue, ConvertedSaturation, ConvertedValue, text).
     This does not take a floating point number, it does actually take numbers from 0 to 100! (0 to 360 for hue)
     """
     try:
         h, s, v = int(h), int(s), int(v)
-    except ValueError:
-        raise ValueError(red(underlined("HSV is invalid.")))
+    except ValueError as exc:
+        raise ValueError(red(underlined("HSV is invalid."))) from exc
     if h > 360 or h < 0:
         raise ValueError(red(underlined("HSV is invalid. Hue must be between 0-360!")))
     if s > 100 or s < 0:
         raise ValueError(
             red(underlined("HSV is invalid. Saturation must be between 0-100!"))
         )
     if v > 100 or v < 0:
@@ -203,16 +231,16 @@
 def bghsv(h, s, v, text):
     """
     hsv(Hue, Saturation, Value, Text) but for the background,
     This does not take a floating point number, it does actually take numbers from 0 to 100! (0 to 360 for hue)
     """
     try:
         h, s, v = int(h), int(s), int(v)
-    except ValueError:
-        raise ValueError(red(underlined("HSV is invalid.")))
+    except ValueError as exc:
+        raise ValueError(red(underlined("HSV is invalid."))) from exc
     if h > 360 or h < 0:
         raise ValueError(red(underlined("HSV is invalid. Hue must be between 0-360!")))
     if s > 100 or s < 0:
         raise ValueError(
             red(underlined("HSV is invalid. Saturation must be between 0-100!"))
         )
     if v > 100 or v < 0:
@@ -298,32 +326,32 @@
     Enjoy I guess
     """
     if autoOsSystem:
         execc("")
     formedstr = ""
     i = 0
     for char in text:
-        if char in " \t\n":
+        if char in (" ", "\t", "\n", "\r"):
             formedstr += char
             continue
         mi = i % 7
         if mi == 0:
-            formedstr += hex("f33444", char)
+            formedstr += hexa(0xF33444, char)
         elif mi == 1:
-            formedstr += hex("ff8901", char)
+            formedstr += hexa(0xFF8901, char)
         elif mi == 2:
-            formedstr += hex("fad716", char)
+            formedstr += hexa(0xFAD716, char)
         elif mi == 3:
-            formedstr += hex("00ba70", char)
+            formedstr += hexa(0x00BA70, char)
         elif mi == 4:
-            formedstr += hex("00c0dd", char)
+            formedstr += hexa(0x00C0DD, char)
         elif mi == 5:
-            formedstr += hex("00408a", char)
+            formedstr += hexa(0x00408A, char)
         elif mi == 6:
-            formedstr += hex("5e2779", char)
+            formedstr += hexa(0x5E2779, char)
         i += 1
     return formedstr
 
 
 # Background colors
 
 
@@ -418,34 +446,20 @@
     """
     if autoOsSystem:
         execc("")
     return f"{__sunderlined}{text}{__endcolor}"
 
 
 def inverted(text):
-    """
-    I can't explain this, just try it and see what it looks like for you.
-    """
     if autoOsSystem:
         execc("")
     return f"{__sinverted}{text}{__endcolor}"
 
 
 def blink(text):
-    """Blink
-
-    [insert faded out version of "Blink"]
-
-    Blink
-
-    [insert faded out version of "Blink"]
-
-    Blink
-
-    [insert faded out version of "Blink"]"""
     if autoOsSystem:
         execc("")
     return f"{__sblink}{text}{__endcolor}"
 
 
 def anotherblink(text):
     """
@@ -453,17 +467,14 @@
     """
     if autoOsSystem:
         execc("")
     return f"{__sanotherblink}{text}{__endcolor}"
 
 
 def fadedout(text):
-    """
-    You can use this to do a manual blinking text if you want.
-    """
     return f"{__sfadedout}{text}{__endcolor}"
 
 
 def dim(text):
     """
     Alias for fadedout()
     """
```

