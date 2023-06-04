# Comparing `tmp/libretrofuzz-2.8.4.tar.gz` & `tmp/libretrofuzz-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.8.4.tar", max compression
+gzip compressed data, was "libretrofuzz-2.8.5.tar", max compression
```

## Comparing `libretrofuzz-2.8.4.tar` & `libretrofuzz-2.8.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-04 01:02:22.979620 libretrofuzz-2.8.4/LICENSE
--rw-r--r--   0        0        0     7166 2023-06-04 01:02:22.979620 libretrofuzz-2.8.4/README.rst
--rw-r--r--   0        0        0       22 2023-06-04 01:02:22.979620 libretrofuzz-2.8.4/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    46916 2023-06-04 01:02:22.979620 libretrofuzz-2.8.4/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      952 2023-06-04 01:02:22.979620 libretrofuzz-2.8.4/pyproject.toml
--rw-r--r--   0        0        0     8328 2023-06-04 01:02:38.642704 libretrofuzz-2.8.4/setup.py
--rw-r--r--   0        0        0     8310 2023-06-04 01:02:38.643900 libretrofuzz-2.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-04 11:50:57.198899 libretrofuzz-2.8.5/LICENSE
+-rw-r--r--   0        0        0     7166 2023-06-04 11:50:57.198899 libretrofuzz-2.8.5/README.rst
+-rw-r--r--   0        0        0       22 2023-06-04 11:50:57.198899 libretrofuzz-2.8.5/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    47407 2023-06-04 11:50:57.198899 libretrofuzz-2.8.5/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      952 2023-06-04 11:50:57.198899 libretrofuzz-2.8.5/pyproject.toml
+-rw-r--r--   0        0        0     8328 2023-06-04 11:51:06.116192 libretrofuzz-2.8.5/setup.py
+-rw-r--r--   0        0        0     8310 2023-06-04 11:51:06.117048 libretrofuzz-2.8.5/PKG-INFO
```

### Comparing `libretrofuzz-2.8.4/LICENSE` & `libretrofuzz-2.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.8.4/README.rst` & `libretrofuzz-2.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.8.4/libretrofuzz/__main__.py` & `libretrofuzz-2.8.5/libretrofuzz/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,29 +149,32 @@
             #ignore keys in buffer before we are ready
             input.read_keys()
             input.flush_keys()
             typer.echo(typer.style(f'Press escape to quit, and most other non-meta keys to skip downloads', bold=True))
             yield done
 
 #----------------non contextual str manipulation------------------------
+parenthesis_patterns = { '()': re.compile(fr'\([^)(]*\)'), '[]': re.compile(fr'\[[^][]*\]') }
 def removeparenthesis(s, open_p='(', close_p=')'):
     nb_rep = 1
+    key = open_p+close_p
+    try:
+      pattern = parenthesis_patterns[key]
+    except:
+      pattern =  re.compile(fr'\{open_p}[^{close_p}{open_p}]*\{close_p}')
+      parenthesis_patterns[key] = pattern
     while (nb_rep):
-        a = fr'\{open_p}[^{close_p}{open_p}]*\{close_p}'
-        (s, nb_rep) = re.subn(a, '', s)
+        (s, nb_rep) = re.subn(pattern, '', s)
     return s
 
 def replacemany(our_str, to_be_replaced, replace_with):
     for nextchar in to_be_replaced:
         our_str = our_str.replace(nextchar, replace_with)
     return our_str
 
-def split_camelcase(name: str):
-    return ' '.join([s.strip() for s in re.split('([A-Z][^A-Z]*)', name) if s])
-
 def removefirst(name: str, suf: str):
     return name.replace(suf, '', 1)
 
 def removeprefix(name: str, pre: str):
     if name.startswith(pre):
         return name[len(pre):]
     return name
@@ -216,27 +219,30 @@
             #is prone because it sets score to 100 if one string words are completely on the other.
             return similarity + prefix
 
 
 #-----------------------------------------------------------------------------------------------------------------------------
 # Normalization functions, part of the functions that change both local labels and remote names to be more similar to compare
 #-----------------------------------------------------------------------------------------------------------------------------
+camelcase_pattern = re.compile(r'([A-Z][^A-Z]*)')
+#number sequences in the middle (not start or end) of a string that start with 0
+zero_lead_pattern = re.compile(r'([^\d])0+([1-9])')
 def normalizer(t, nometa, hack):
     if nometa:
         t = removeparenthesis(t,'(',')')
     if not hack:
         t = removeparenthesis(t,'[',']')
     #change all common ascci symbol characters we aren't going to use after this (, and ')
     t = replacemany(t, '_()[]{}-.!?#"', ' ')
     #strips just because the user may have made a mistake naming the source
     #(or the replacement above introduce boundary spaces)
     t = t.strip()
     #CamelCaseNames for local labels are common when there are no spaces,
     #do this to normalize definite articles in normalization with spaces only (minimizes changes)
-    t = split_camelcase(t)
+    t = ' '.join([s.strip() for s in re.split(camelcase_pattern, t) if s])
     #normalize case
     t = t.lower()
     #beginning and end definite articles in several european languages (people move them)
     #make sure we're only removing the start and end forms with spaces
     t = removefirst(t, ', the')
     t = removeprefix(t, 'the ')
     t = removefirst(t, ', los')
@@ -272,14 +278,16 @@
     t = replacemany(t, ',\'', '')
     #this makes sure that if a remote name has ' and ' instead of ' _ ' to replace ' & ' it works
     #': ' doesn't need this because ':' is a forbidden character and both '_' and '-' turn to ''
     t = t.replace(' and ',  '')
     #although all names have spaces (now), the local names may have weird spaces,
     #so to equalize them after the space dependent checks (this also strips)
     t = ''.join(t.split())
+    #remove any number leading 0 (except at the end or the start of the string)
+    t = re.sub(zero_lead_pattern, r'\1\2', t)
     #Tries to make roman numerals in the range 1-20 equivalent to normal numbers (to handle names that change it).
     #If both sides are roman numerals there is no harm done if XXIV gets turned into 204 in both sides.
     t = t.replace('xviii', '18')
     t = t.replace('xvii',  '17')
     t = t.replace('xvi' ,  '16')
     t = t.replace('xiii',  '13')
     t = t.replace('xii' ,  '12')
```

### Comparing `libretrofuzz-2.8.4/pyproject.toml` & `libretrofuzz-2.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.8.4"
+version = "2.8.5"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.8.4/setup.py` & `libretrofuzz-2.8.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.8.4',
+    'version': '2.8.5',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get non-standard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will dowload for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with grey border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n ``libretro-fuzz --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels don't have subtitles and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads and the system name ``Commodore - Amiga`` to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then mostly be from the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass the similarity test. Common false positives from this are sequels or prequels, or different releases, most often regions/languages.\n\nExample:\n  ``libretro-fuzz --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, the Ishar series in the WHDLoad playlist.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy\n                        matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails.\n                        If not provided, asked from the user.\n  --delay-after FLOAT   Seconds after download to skip replacing thumbnails.\n                        No-op with --no-image.  [1<=x<=10]\n  --delay FLOAT         Seconds to skip thumbnails download.  [1<=x<=10]\n  --filter GLOB         Restricts downloads to game labels globs - not paths -\n                        in the playlist, can be used multiple times and\n                        matches reset thumbnails, --filter '\\*' downloads all.\n  --score FUZZ          Download fuzz (less is more fuzz, 100 being average).\n                        No-op with --no-fail.  [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to --score 0.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if\n                        there is at least one in cache to avoid mixing\n                        thumbnails from different server directories on\n                        repeated calls. No-op with --filter.\n  --no-subtitle         Ignores text after last ' - ' or ': '. ':' can't occur\n                        in server names, so if the server has 'Name\\_\n                        subtitle.png' and not 'Name - subtitle.png'\n                        (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false\n                        positives. Forced with --before.\n  --hack                Matches [] delimited metadata and may cause false\n                        positives, Best used if the hack has thumbnails.\n                        Ignored with --before.\n  --before TEXT         Use only the part of the label before TEXT to match.\n                        TEXT may not be inside of brackets of any kind, may\n                        cause false positives but some labels do not have\n                        traditional separators. Forces ignoring metadata.\n  --verbose             Shows the failures, score and normalized local and\n                        server names in output.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-2.8.4/PKG-INFO` & `libretrofuzz-2.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.8.4
+Version: 2.8.5
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

