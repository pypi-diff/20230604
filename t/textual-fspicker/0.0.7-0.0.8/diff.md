# Comparing `tmp/textual_fspicker-0.0.7-py3-none-any.whl.zip` & `tmp/textual_fspicker-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17210 bytes, number of entries: 17
--rw-r--r--  2.0 unx      915 b- defN 23-Jun-03 07:21 textual_fspicker/__init__.py
--rw-r--r--  2.0 unx     3254 b- defN 23-Jun-03 06:49 textual_fspicker/__main__.py
+Zip file size: 17270 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      915 b- defN 23-Jun-04 06:41 textual_fspicker/__init__.py
+-rw-r--r--  2.0 unx     3254 b- defN 23-Jun-04 06:41 textual_fspicker/__main__.py
 -rw-r--r--  2.0 unx     4231 b- defN 23-Jun-03 06:39 textual_fspicker/base_dialog.py
--rw-r--r--  2.0 unx     5682 b- defN 23-Jun-03 06:49 textual_fspicker/file_dialog.py
+-rw-r--r--  2.0 unx     5944 b- defN 23-Jun-04 06:41 textual_fspicker/file_dialog.py
 -rw-r--r--  2.0 unx     1521 b- defN 23-May-23 20:46 textual_fspicker/file_open.py
 -rw-r--r--  2.0 unx     1570 b- defN 23-May-23 20:46 textual_fspicker/file_save.py
 -rw-r--r--  2.0 unx     1822 b- defN 23-May-21 08:58 textual_fspicker/path_filters.py
 -rw-r--r--  2.0 unx     1369 b- defN 23-Jun-03 06:49 textual_fspicker/path_maker.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 20:02 textual_fspicker/py.typed
 -rw-r--r--  2.0 unx     2174 b- defN 23-May-19 09:53 textual_fspicker/safe_tests.py
 -rw-r--r--  2.0 unx     2457 b- defN 23-May-22 20:47 textual_fspicker/select_directory.py
 -rw-r--r--  2.0 unx      389 b- defN 23-May-17 19:18 textual_fspicker/parts/__init__.py
 -rw-r--r--  2.0 unx    15288 b- defN 23-Jun-03 07:21 textual_fspicker/parts/directory_navigation.py
--rw-r--r--  2.0 unx     4235 b- defN 23-Jun-03 07:22 textual_fspicker-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-03 07:22 textual_fspicker-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-03 07:22 textual_fspicker-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-03 07:22 textual_fspicker-0.0.7.dist-info/RECORD
-17 files, 46496 bytes uncompressed, 14750 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx     4235 b- defN 23-Jun-04 06:41 textual_fspicker-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 06:41 textual_fspicker-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-04 06:41 textual_fspicker-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-04 06:41 textual_fspicker-0.0.8.dist-info/RECORD
+17 files, 46758 bytes uncompressed, 14810 bytes compressed:  68.3%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: textual_fspicker/parts/__init__.py
 Comment: 
 
 Filename: textual_fspicker/parts/directory_navigation.py
 Comment: 
 
-Filename: textual_fspicker-0.0.7.dist-info/METADATA
+Filename: textual_fspicker-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: textual_fspicker-0.0.7.dist-info/WHEEL
+Filename: textual_fspicker-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: textual_fspicker-0.0.7.dist-info/top_level.txt
+Filename: textual_fspicker-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: textual_fspicker-0.0.7.dist-info/RECORD
+Filename: textual_fspicker-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## textual_fspicker/__init__.py

```diff
@@ -3,15 +3,15 @@
 ######################################################################
 # Main app information.
 __author__     = "Dave Pearson"
 __copyright__  = "Copyright 2023, Dave Pearson"
 __credits__    = [ "Dave Pearson" ]
 __maintainer__ = "Dave Pearson"
 __email__      = "davep@davep.org"
-__version__    = "0.0.7"
+__version__    = "0.0.8"
 __licence__    = "MIT"
 
 ##############################################################################
 # Local imports.
 from .file_open        import FileOpen
 from .file_save        import FileSave
 from .select_directory import SelectDirectory
```

## textual_fspicker/__main__.py

 * *Ordering differences only*

```diff
@@ -59,18 +59,18 @@
         self.query_one( Label ).update( str( to_show ) )
 
     @on( Button.Pressed, "#open" )
     def open_file( self ) -> None:
         """Show the `FileOpen` dialog when the button is pushed."""
         self.push_screen(
             FileOpen( ".", filters=Filters(
+                ( "Python",  lambda p: p.suffix.lower() == ".py" ),
                 ( "Any",     lambda _: True ),
                 ( "Emacs",   lambda p: p.suffix.lower() == ".el" ),
                 ( "Lisp",    lambda p: p.suffix.lower() in ( ".lisp", ".lsp", ".cl" ) ),
-                ( "Python",  lambda p: p.suffix.lower() == ".py" ),
                 ( "Pascal",  lambda p: p.suffix.lower() == ".pas" ),
                 ( "Clipper", lambda p: p.suffix.lower() in ( ".prg", ".ch" ) ),
                 ( "C",       lambda p: p.suffix.lower() in ( ".c", ".h" ) ),
                 ( "C++",     lambda p: p.suffix.lower() in ( ".cpp", ".cc", ".h" ) ),
             ) ),
             callback=self.show_selected
         )
```

## textual_fspicker/file_dialog.py

```diff
@@ -5,14 +5,15 @@
 from __future__ import annotations
 from pathlib    import Path
 
 ##############################################################################
 # Textual imports.
 from textual         import on
 from textual.app     import ComposeResult
+from textual.events  import Mount
 from textual.widgets import Button,Input, Select
 
 ##############################################################################
 # Local imports.
 from .base_dialog  import FileSystemPickerScreen
 from .parts        import DirectoryNavigation
 from .path_filters import Filters
@@ -62,14 +63,20 @@
             yield FileFilter(
                 self._filters.selections,
                 prompt      = "File filter",
                 value       = 0,
                 allow_blank = False
             )
 
+    @on( Mount )
+    def _initial_filter( self ) -> None:
+        """Set the initial filter once the DOM is ready."""
+        if self._filters:
+            self.query_one( DirectoryNavigation ).file_filter = self._filters[ 0 ]
+
     @on( DirectoryNavigation.Selected )
     def _select_file( self, event: DirectoryNavigation.Selected ) -> None:
         """Handle a file being selected in the picker.
 
         Args:
             event: The event to handle.
         """
```

## Comparing `textual_fspicker-0.0.7.dist-info/METADATA` & `textual_fspicker-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-fspicker
-Version: 0.0.7
+Version: 0.0.8
 Summary: A simple Textual filesystem picker dialog library.
 Home-page: https://github.com/davep/textual-fspicker
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
```

## Comparing `textual_fspicker-0.0.7.dist-info/RECORD` & `textual_fspicker-0.0.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-textual_fspicker/__init__.py,sha256=eBBc_6VyhXQr1WmJzcfhblDbx7OCRS75RKbtea6C7KM,915
-textual_fspicker/__main__.py,sha256=IYU475b7ao-qLClpqYeRRMrjfQksNRaMTp-luNh7mr8,3254
+textual_fspicker/__init__.py,sha256=cudg6pv8kvK26BR_CAOtiOlbnMiUKZisJ33qGGobcJQ,915
+textual_fspicker/__main__.py,sha256=v57UBTiFOMwuIvpL0zcHpYs-BjkvPzINQACRoKIzRf0,3254
 textual_fspicker/base_dialog.py,sha256=qDbghAxRYU1K8723w1YarQfPwIVkzs8BO5xcBmXK1ZA,4231
-textual_fspicker/file_dialog.py,sha256=0Jugxeqjc312D379Ag0xA11BU-tgA8ygiAi2tchhK3w,5682
+textual_fspicker/file_dialog.py,sha256=B6yyFVOzemGcVJYz0gcB-OzwxISELwWK2MfTocV_Ua4,5944
 textual_fspicker/file_open.py,sha256=eMXpA1xOmYoOPSMEcefVsk_lc2xH7Nn-x-mEJhhdblY,1521
 textual_fspicker/file_save.py,sha256=WIE9rRUvb_UCntMw47Hjmbqnq2xr8u1oE7VPGJ3I7H8,1570
 textual_fspicker/path_filters.py,sha256=XpPrynKVI_p8Tf6tUuhEmU5lxAaf3TQlsjKsRwXC5nk,1822
 textual_fspicker/path_maker.py,sha256=1wYOQ9EQKYu8kZBqH7kYv-qwdUwIpkybvwkDaZkc6zw,1369
 textual_fspicker/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 textual_fspicker/safe_tests.py,sha256=U3gpqVRr7qcv7mqF-I_sFojtr9Pv5JyqFzAxGG7qofA,2174
 textual_fspicker/select_directory.py,sha256=vE1MYCL-_QqTyPiveJrxl90oEwjQB14lfSsHteUEBNM,2457
 textual_fspicker/parts/__init__.py,sha256=vjP1jzd5ty4IhwUZnVFkOjzctZn22EbwWDHh_16x-GM,389
 textual_fspicker/parts/directory_navigation.py,sha256=2nhPZoyDZstdmvzlR5UQcdTX5wbCoJz4JzZ8DK7hXKw,15288
-textual_fspicker-0.0.7.dist-info/METADATA,sha256=Ap3axXOkAQBYVJES3KRfQic7qOrzxV5Saos0wqDGgo8,4235
-textual_fspicker-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-textual_fspicker-0.0.7.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
-textual_fspicker-0.0.7.dist-info/RECORD,,
+textual_fspicker-0.0.8.dist-info/METADATA,sha256=lUpmA-TBIJwWdwkUBFf5_7_h5UmrCarGLuTI0t3jt0w,4235
+textual_fspicker-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+textual_fspicker-0.0.8.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
+textual_fspicker-0.0.8.dist-info/RECORD,,
```

