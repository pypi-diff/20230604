# Comparing `tmp/autosrt-1.3.1.tar.gz` & `tmp/autosrt-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autosrt-1.3.1.tar", last modified: Sun Jun  4 13:27:47 2023, max compression
+gzip compressed data, was "autosrt-1.3.2.tar", last modified: Sun Jun  4 20:35:01 2023, max compression
```

## Comparing `autosrt-1.3.1.tar` & `autosrt-1.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 13:27:47.943765 autosrt-1.3.1/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2018 2023-06-04 13:27:47.944515 autosrt-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 13:27:47.835138 autosrt-1.3.1/autosrt/
--rw-rw-rw-   0        0        0    15502 2023-06-03 21:05:35.000000 autosrt-1.3.1/autosrt/__init__.py
--rw-rw-rw-   0        0        0    55527 2023-06-04 11:41:51.000000 autosrt-1.3.1/autosrt/autosrt.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:27:47.878584 autosrt-1.3.1/autosrt.egg-info/
--rw-rw-rw-   0        0        0     2018 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-04 13:27:47.000000 autosrt-1.3.1/autosrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-04 13:27:47.948264 autosrt-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-04 13:27:47.942268 autosrt-1.3.1/test/
--rw-rw-rw-   0        0        0     7362 2023-05-03 15:20:29.000000 autosrt-1.3.1/test/test1.py
--rw-rw-rw-   0        0        0     4465 2023-05-02 21:51:09.000000 autosrt-1.3.1/test/test2.py
--rw-rw-rw-   0        0        0     9939 2023-05-03 13:45:31.000000 autosrt-1.3.1/test/test3.py
--rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.1/test/test4.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:35:01.111331 autosrt-1.3.2/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 autosrt-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 autosrt-1.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2018 2023-06-04 20:35:01.112829 autosrt-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5260 2023-04-30 04:22:31.000000 autosrt-1.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 20:35:00.664107 autosrt-1.3.2/autosrt/
+-rw-rw-rw-   0        0        0    15610 2023-06-04 20:19:47.000000 autosrt-1.3.2/autosrt/__init__.py
+-rw-rw-rw-   0        0        0    71211 2023-06-04 20:19:21.000000 autosrt-1.3.2/autosrt/autosrt.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:35:00.809043 autosrt-1.3.2/autosrt.egg-info/
+-rw-rw-rw-   0        0        0     2018 2023-06-04 20:34:59.000000 autosrt-1.3.2/autosrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-06-04 20:34:59.000000 autosrt-1.3.2/autosrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 20:34:59.000000 autosrt-1.3.2/autosrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-04 20:34:59.000000 autosrt-1.3.2/autosrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-04 20:34:59.000000 autosrt-1.3.2/autosrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-04 20:34:59.000000 autosrt-1.3.2/autosrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-04 20:35:01.181555 autosrt-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1682 2023-06-03 00:59:56.000000 autosrt-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 20:35:01.106835 autosrt-1.3.2/test/
+-rw-rw-rw-   0        0        0     7362 2023-05-03 15:20:29.000000 autosrt-1.3.2/test/test1.py
+-rw-rw-rw-   0        0        0     4465 2023-05-02 21:51:09.000000 autosrt-1.3.2/test/test2.py
+-rw-rw-rw-   0        0        0     9939 2023-05-03 13:45:31.000000 autosrt-1.3.2/test/test3.py
+-rw-rw-rw-   0        0        0    68819 2023-05-09 15:49:36.000000 autosrt-1.3.2/test/test4.py
```

### Comparing `autosrt-1.3.1/LICENSE` & `autosrt-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.1/PKG-INFO` & `autosrt-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.1
+Version: 1.3.2
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.1/README.md` & `autosrt-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.1/autosrt/__init__.py` & `autosrt-1.3.2/autosrt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,15 +255,16 @@
 
                     subtitle_path = None
                     if do_translate:
                         subtitle_path = translated_subtitle_filepath
                     else:
                         subtitle_path = subtitle_filepath
 
-                    subtitle_renderer = MediaSubtitleRenderer(media_ext=ext, subtitle_path=subtitle_path, output_path=rendered_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
+                    ffmpeg_language_code = language.ffmpeg_code_of_code[args.src_language]
+                    subtitle_renderer = MediaSubtitleRenderer(subtitle_path=subtitle_path, language=ffmpeg_language_code, output_path=rendered_media_filepath, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     widgets = [f"Rendering subtitles with {media_type}          : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     result = subtitle_renderer(media_filepath)
                     pbar.finish()
 
                     if result and os.path.isfile(result):
                         print("Rendered video created at               : {}".format(rendered_media_filepath))
```

### Comparing `autosrt-1.3.1/autosrt/autosrt.py` & `autosrt-1.3.2/autosrt/autosrt.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 except ImportError:
     JSONDecodeError = ValueError
 from progressbar import ProgressBar, Percentage, Bar, ETA
 import pysrt
 import six
 import shlex
 
-VERSION = "1.3.1"
+VERSION = "1.3.2"
 
 
 #======================================================== ffmpeg_progress_yield ========================================================#
 
 
 import re
 #import subprocess
@@ -671,17 +671,156 @@
         self.list_names.append("Vietnamese")
         self.list_names.append("Welsh")
         self.list_names.append("Xhosa")
         self.list_names.append("Yiddish")
         self.list_names.append("Yoruba")
         self.list_names.append("Zulu")
 
+        self.list_ffmpeg_codes = []
+        self.list_ffmpeg_codes.append("afr")  # Afrikaans
+        self.list_ffmpeg_codes.append("alb")  # Albanian
+        self.list_ffmpeg_codes.append("amh")  # Amharic
+        self.list_ffmpeg_codes.append("ara")  # Arabic
+        self.list_ffmpeg_codes.append("hye")  # Armenian
+        self.list_ffmpeg_codes.append("asm")  # Assamese
+        self.list_ffmpeg_codes.append("aym")  # Aymara
+        self.list_ffmpeg_codes.append("aze")  # Azerbaijani
+        self.list_ffmpeg_codes.append("bam")  # Bambara
+        self.list_ffmpeg_codes.append("eus")  # Basque
+        self.list_ffmpeg_codes.append("bel")  # Belarusian
+        self.list_ffmpeg_codes.append("ben")  # Bengali
+        self.list_ffmpeg_codes.append("bho")  # Bhojpuri
+        self.list_ffmpeg_codes.append("bos")  # Bosnian
+        self.list_ffmpeg_codes.append("bul")  # Bulgarian
+        self.list_ffmpeg_codes.append("cat")  # Catalan
+        self.list_ffmpeg_codes.append("ceb")  # Cebuano
+        self.list_ffmpeg_codes.append("nya")  # Chichewa
+        self.list_ffmpeg_codes.append("zho")  # Chinese
+        self.list_ffmpeg_codes.append("zho-CN")  # Chinese (Simplified)
+        self.list_ffmpeg_codes.append("zho-TW")  # Chinese (Traditional)
+        self.list_ffmpeg_codes.append("cos")  # Corsican
+        self.list_ffmpeg_codes.append("hrv")  # Croatian
+        self.list_ffmpeg_codes.append("ces")  # Czech
+        self.list_ffmpeg_codes.append("dan")  # Danish
+        self.list_ffmpeg_codes.append("div")  # Dhivehi
+        self.list_ffmpeg_codes.append("doi")  # Dogri
+        self.list_ffmpeg_codes.append("nld")  # Dutch
+        self.list_ffmpeg_codes.append("eng")  # English
+        self.list_ffmpeg_codes.append("epo")  # Esperanto
+        self.list_ffmpeg_codes.append("est")  # Estonian
+        self.list_ffmpeg_codes.append("ewe")  # Ewe
+        self.list_ffmpeg_codes.append("fil")  # Filipino
+        self.list_ffmpeg_codes.append("fin")  # Finnish
+        self.list_ffmpeg_codes.append("fra")  # French
+        self.list_ffmpeg_codes.append("fry")  # Frisian
+        self.list_ffmpeg_codes.append("glg")  # Galician
+        self.list_ffmpeg_codes.append("kat")  # Georgian
+        self.list_ffmpeg_codes.append("deu")  # German
+        self.list_ffmpeg_codes.append("ell")  # Greek
+        self.list_ffmpeg_codes.append("grn")  # Guarani
+        self.list_ffmpeg_codes.append("guj")  # Gujarati
+        self.list_ffmpeg_codes.append("hat")  # Haitian Creole
+        self.list_ffmpeg_codes.append("hau")  # Hausa
+        self.list_ffmpeg_codes.append("haw")  # Hawaiian
+        self.list_ffmpeg_codes.append("heb")  # Hebrew
+        self.list_ffmpeg_codes.append("hin")  # Hindi
+        self.list_ffmpeg_codes.append("hmn")  # Hmong
+        self.list_ffmpeg_codes.append("hun")  # Hungarian
+        self.list_ffmpeg_codes.append("isl")  # Icelandic
+        self.list_ffmpeg_codes.append("ibo")  # Igbo
+        self.list_ffmpeg_codes.append("ilo")  # Ilocano
+        self.list_ffmpeg_codes.append("ind")  # Indonesian
+        self.list_ffmpeg_codes.append("gle")  # Irish
+        self.list_ffmpeg_codes.append("ita")  # Italian
+        self.list_ffmpeg_codes.append("jpn")  # Japanese
+        self.list_ffmpeg_codes.append("jav")  # Javanese
+        self.list_ffmpeg_codes.append("kan")  # Kannada
+        self.list_ffmpeg_codes.append("kaz")  # Kazakh
+        self.list_ffmpeg_codes.append("khm")  # Khmer
+        self.list_ffmpeg_codes.append("kin")  # Kinyarwanda
+        self.list_ffmpeg_codes.append("kok")  # Konkani
+        self.list_ffmpeg_codes.append("kor")  # Korean
+        self.list_ffmpeg_codes.append("kri")  # Krio
+        self.list_ffmpeg_codes.append("kmr")  # Kurdish (Kurmanji)
+        self.list_ffmpeg_codes.append("ckb")  # Kurdish (Sorani)
+        self.list_ffmpeg_codes.append("kir")  # Kyrgyz
+        self.list_ffmpeg_codes.append("lao")  # Lao
+        self.list_ffmpeg_codes.append("lat")  # Latin
+        self.list_ffmpeg_codes.append("lav")  # Latvian
+        self.list_ffmpeg_codes.append("lin")  # Lingala
+        self.list_ffmpeg_codes.append("lit")  # Lithuanian
+        self.list_ffmpeg_codes.append("lug")  # Luganda
+        self.list_ffmpeg_codes.append("ltz")  # Luxembourgish
+        self.list_ffmpeg_codes.append("mkd")  # Macedonian
+        self.list_ffmpeg_codes.append("mlg")  # Malagasy
+        self.list_ffmpeg_codes.append("msa")  # Malay
+        self.list_ffmpeg_codes.append("mal")  # Malayalam
+        self.list_ffmpeg_codes.append("mlt")  # Maltese
+        self.list_ffmpeg_codes.append("mri")  # Maori
+        self.list_ffmpeg_codes.append("mar")  # Marathi
+        self.list_ffmpeg_codes.append("mni-Mtei")  # Meiteilon (Manipuri)
+        self.list_ffmpeg_codes.append("lus")  # Mizo
+        self.list_ffmpeg_codes.append("mon")  # Mongolian
+        self.list_ffmpeg_codes.append("mya")  # Myanmar (Burmese)
+        self.list_ffmpeg_codes.append("nep")  # Nepali
+        self.list_ffmpeg_codes.append("nor")  # Norwegian
+        self.list_ffmpeg_codes.append("ori")  # Odiya (Oriya)
+        self.list_ffmpeg_codes.append("orm")  # Oromo
+        self.list_ffmpeg_codes.append("pus")  # Pashto
+        self.list_ffmpeg_codes.append("fas")  # Persian
+        self.list_ffmpeg_codes.append("pol")  # Polish
+        self.list_ffmpeg_codes.append("por")  # Portuguese
+        self.list_ffmpeg_codes.append("pan")  # Punjabi
+        self.list_ffmpeg_codes.append("que")  # Quechua
+        self.list_ffmpeg_codes.append("ron")  # Romanian
+        self.list_ffmpeg_codes.append("rus")  # Russian
+        self.list_ffmpeg_codes.append("smo")  # Samoan
+        self.list_ffmpeg_codes.append("san")  # Sanskrit
+        self.list_ffmpeg_codes.append("gla")  # Scots Gaelic
+        self.list_ffmpeg_codes.append("nso")  # Sepedi
+        self.list_ffmpeg_codes.append("srp")  # Serbian
+        self.list_ffmpeg_codes.append("sot")  # Sesotho
+        self.list_ffmpeg_codes.append("sna")  # Shona
+        self.list_ffmpeg_codes.append("snd")  # Sindhi
+        self.list_ffmpeg_codes.append("sin")  # Sinhala
+        self.list_ffmpeg_codes.append("slk")  # Slovak
+        self.list_ffmpeg_codes.append("slv")  # Slovenian
+        self.list_ffmpeg_codes.append("som")  # Somali
+        self.list_ffmpeg_codes.append("spa")  # Spanish
+        self.list_ffmpeg_codes.append("sun")  # Sundanese
+        self.list_ffmpeg_codes.append("swa")  # Swahili
+        self.list_ffmpeg_codes.append("swe")  # Swedish
+        self.list_ffmpeg_codes.append("tgk")  # Tajik
+        self.list_ffmpeg_codes.append("tam")  # Tamil
+        self.list_ffmpeg_codes.append("tat")  # Tatar
+        self.list_ffmpeg_codes.append("tel")  # Telugu
+        self.list_ffmpeg_codes.append("tha")  # Thai
+        self.list_ffmpeg_codes.append("tir")  # Tigrinya
+        self.list_ffmpeg_codes.append("tso")  # Tsonga
+        self.list_ffmpeg_codes.append("tur")  # Turkish
+        self.list_ffmpeg_codes.append("tuk")  # Turkmen
+        self.list_ffmpeg_codes.append("twi")  # Twi (Akan)
+        self.list_ffmpeg_codes.append("ukr")  # Ukrainian
+        self.list_ffmpeg_codes.append("urd")  # Urdu
+        self.list_ffmpeg_codes.append("uig")  # Uyghur
+        self.list_ffmpeg_codes.append("uzb")  # Uzbek
+        self.list_ffmpeg_codes.append("vie")  # Vietnamese
+        self.list_ffmpeg_codes.append("wel")  # Welsh
+        self.list_ffmpeg_codes.append("xho")  # Xhosa
+        self.list_ffmpeg_codes.append("yid")  # Yiddish
+        self.list_ffmpeg_codes.append("yor")  # Yoruba
+        self.list_ffmpeg_codes.append("zul")  # Zulu
+
         self.code_of_name = dict(zip(self.list_names, self.list_codes))
         self.name_of_code = dict(zip(self.list_codes, self.list_names))
 
+        self.ffmpeg_code_of_name = dict(zip(self.list_names, self.list_ffmpeg_codes))
+        self.ffmpeg_code_of_code = dict(zip(self.list_codes, self.list_ffmpeg_codes))
+        self.name_of_ffmpeg_code = dict(zip(self.list_ffmpeg_codes, self.list_names))
+
         self.dict = {
                         'af': 'Afrikaans',
                         'sq': 'Albanian',
                         'am': 'Amharic',
                         'ar': 'Arabic',
                         'hy': 'Armenian',
                         'as': 'Assamese',
@@ -810,23 +949,162 @@
                         'cy': 'Welsh',
                         'xh': 'Xhosa',
                         'yi': 'Yiddish',
                         'yo': 'Yoruba',
                         'zu': 'Zulu',
                     }
 
+        self.ffmpeg_dict = {
+                                'af': 'afr', # Afrikaans
+                                'sq': 'alb', # Albanian
+                                'am': 'amh', # Amharic
+                                'ar': 'ara', # Arabic
+                                'hy': 'arm', # Armenian
+                                'as': 'asm', # Assamese
+                                'ay': 'aym', # Aymara
+                                'az': 'aze', # Azerbaijani
+                                'bm': 'bam', # Bambara
+                                'eu': 'baq', # Basque
+                                'be': 'bel', # Belarusian
+                                'bn': 'ben', # Bengali
+                                'bho': 'bho', # Bhojpuri
+                                'bs': 'bos', # Bosnian
+                                'bg': 'bul', # Bulgarian
+                                'ca': 'cat', # Catalan
+                                'ceb': 'ceb', # Cebuano
+                                'ny': 'nya', # Chichewa
+                                'zh': 'chi', # Chinese
+                                'zh-CN': 'chi', # Chinese (Simplified)
+                                'zh-TW': 'chi', # Chinese (Traditional)
+                                'co': 'cos', # Corsican
+                                'hr': 'hrv', # Croatian
+                                'cs': 'cze', # Czech
+                                'da': 'dan', # Danish
+                                'dv': 'div', # Dhivehi
+                                'doi': 'doi', # Dogri
+                                'nl': 'dut', # Dutch
+                                'en': 'eng', # English
+                                'eo': 'epo', # Esperanto
+                                'et': 'est', # Estonian
+                                'ee': 'ewe', # Ewe
+                                'fil': 'fil', # Filipino
+                                'fi': 'fin', # Finnish
+                                'fr': 'fre', # French
+                                'fy': 'fry', # Frisian
+                                'gl': 'glg', # Galician
+                                'ka': 'geo', # Georgian
+                                'de': 'ger', # German
+                                'el': 'gre', # Greek
+                                'gn': 'grn', # Guarani
+                                'gu': 'guj', # Gujarati
+                                'ht': 'hat', # Haitian Creole
+                                'ha': 'hau', # Hausa
+                                'haw': 'haw', # Hawaiian
+                                'he': 'heb', # Hebrew
+                                'hi': 'hin', # Hindi
+                                'hmn': 'hmn', # Hmong
+                                'hu': 'hun', # Hungarian
+                                'is': 'ice', # Icelandic
+                                'ig': 'ibo', # Igbo
+                                'ilo': 'ilo', # Ilocano
+                                'id': 'ind', # Indonesian
+                                'ga': 'gle', # Irish
+                                'it': 'ita', # Italian
+                                'ja': 'jpn', # Japanese
+                                'jv': 'jav', # Javanese
+                                'kn': 'kan', # Kannada
+                                'kk': 'kaz', # Kazakh
+                                'km': 'khm', # Khmer
+                                'rw': 'kin', # Kinyarwanda
+                                'gom': 'kok', # Konkani
+                                'ko': 'kor', # Korean
+                                'kri': 'kri', # Krio
+                                'kmr': 'kur', # Kurdish (Kurmanji)
+                                'ckb': 'kur', # Kurdish (Sorani)
+                                'ky': 'kir', # Kyrgyz
+                                'lo': 'lao', # Lao
+                                'la': 'lat', # Latin
+                                'lv': 'lav', # Latvian
+                                'ln': 'lin', # Lingala
+                                'lt': 'lit', # Lithuanian
+                                'lg': 'lug', # Luganda
+                                'lb': 'ltz', # Luxembourgish
+                                'mk': 'mac', # Macedonian
+                                'mg': 'mlg', # Malagasy
+                                'ms': 'may', # Malay
+                                'ml': 'mal', # Malayalam
+                                'mt': 'mlt', # Maltese
+                                'mi': 'mao', # Maori
+                                'mr': 'mar', # Marathi
+                                'mni-Mtei': 'mni', # Meiteilon (Manipuri)
+                                'lus': 'lus', # Mizo
+                                'mn': 'mon', # Mongolian
+                                'my': 'bur', # Myanmar (Burmese)
+                                'ne': 'nep', # Nepali
+                                'no': 'nor', # Norwegian
+                                'or': 'ori', # Odiya (Oriya)
+                                'om': 'orm', # Oromo
+                                'ps': 'pus', # Pashto
+                                'fa': 'per', # Persian
+                                'pl': 'pol', # Polish
+                                'pt': 'por', # Portuguese
+                                'pa': 'pan', # Punjabi
+                                'qu': 'que', # Quechua
+                                'ro': 'rum', # Romanian
+                                'ru': 'rus', # Russian
+                                'sm': 'smo', # Samoan
+                                'sa': 'san', # Sanskrit
+                                'gd': 'gla', # Scots Gaelic
+                                'nso': 'nso', # Sepedi
+                                'sr': 'srp', # Serbian
+                                'st': 'sot', # Sesotho
+                                'sn': 'sna', # Shona
+                                'sd': 'snd', # Sindhi
+                                'si': 'sin', # Sinhala
+                                'sk': 'slo', # Slovak
+                                'sl': 'slv', # Slovenian
+                                'so': 'som', # Somali
+                                'es': 'spa', # Spanish
+                                'su': 'sun', # Sundanese
+                                'sw': 'swa', # Swahili
+                                'sv': 'swe', # Swedish
+                                'tg': 'tgk', # Tajik
+                                'ta': 'tam', # Tamil
+                                'tt': 'tat', # Tatar
+                                'te': 'tel', # Telugu
+                                'th': 'tha', # Thai
+                                'ti': 'tir', # Tigrinya
+                                'ts': 'tso', # Tsonga
+                                'tr': 'tur', # Turkish
+                                'tk': 'tuk', # Turkmen
+                                'tw': 'twi', # Twi (Akan)
+                                'uk': 'ukr', # Ukrainian
+                                'ur': 'urd', # Urdu
+                                'ug': 'uig', # Uyghur
+                                'uz': 'uzb', # Uzbek
+                                'vi': 'vie', # Vietnamese
+                                'cy': 'wel', # Welsh
+                                'xh': 'xho', # Xhosa
+                                'yi': 'yid', # Yiddish
+                                'yo': 'yor', # Yoruba
+                                'zu': 'zul', # Zulu
+                           }
+
     def get_name(self, get_code):
         return self.dict.get(get_code.lower(), "")
 
     def get_code(self, language):
         for get_code, lang in self.dict.items():
             if lang.lower() == language.lower():
                 return get_code
         return ""
 
+    def get_ffmpeg_code(self, get_code):
+        return self.ffmpeg_dict.get(get_code.lower(), "")
+
 
 class WavConverter:
     @staticmethod
     def which(program):
         def is_exe(file_path):
             return os.path.isfile(file_path) and os.access(file_path, os.X_OK)
         fpath, _ = os.path.split(program)
```

### Comparing `autosrt-1.3.1/autosrt.egg-info/PKG-INFO` & `autosrt-1.3.2/autosrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosrt
-Version: 1.3.1
+Version: 1.3.2
 Summary: a utility for automatic speech recognition and subtitle generation
 Home-page: https://github.com/botbahlul/autosrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `autosrt-1.3.1/setup.py` & `autosrt-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.1/test/test1.py` & `autosrt-1.3.2/test/test1.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.1/test/test2.py` & `autosrt-1.3.2/test/test2.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.1/test/test3.py` & `autosrt-1.3.2/test/test3.py`

 * *Files identical despite different names*

### Comparing `autosrt-1.3.1/test/test4.py` & `autosrt-1.3.2/test/test4.py`

 * *Files identical despite different names*

