# Comparing `tmp/textual_fspicker-0.0.8-py3-none-any.whl.zip` & `tmp/textual_fspicker-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 17270 bytes, number of entries: 17
--rw-r--r--  2.0 unx      915 b- defN 23-Jun-04 06:41 textual_fspicker/__init__.py
--rw-r--r--  2.0 unx     3254 b- defN 23-Jun-04 06:41 textual_fspicker/__main__.py
--rw-r--r--  2.0 unx     4231 b- defN 23-Jun-03 06:39 textual_fspicker/base_dialog.py
--rw-r--r--  2.0 unx     5944 b- defN 23-Jun-04 06:41 textual_fspicker/file_dialog.py
--rw-r--r--  2.0 unx     1521 b- defN 23-May-23 20:46 textual_fspicker/file_open.py
--rw-r--r--  2.0 unx     1570 b- defN 23-May-23 20:46 textual_fspicker/file_save.py
+Zip file size: 17409 bytes, number of entries: 17
+-rw-r--r--  2.0 unx      915 b- defN 23-Jun-04 07:57 textual_fspicker/__init__.py
+-rw-r--r--  2.0 unx     3335 b- defN 23-Jun-04 07:57 textual_fspicker/__main__.py
+-rw-r--r--  2.0 unx     4337 b- defN 23-Jun-04 07:57 textual_fspicker/base_dialog.py
+-rw-r--r--  2.0 unx     5999 b- defN 23-Jun-04 07:57 textual_fspicker/file_dialog.py
+-rw-r--r--  2.0 unx     1513 b- defN 23-Jun-04 07:57 textual_fspicker/file_open.py
+-rw-r--r--  2.0 unx     1562 b- defN 23-Jun-04 07:57 textual_fspicker/file_save.py
 -rw-r--r--  2.0 unx     1822 b- defN 23-May-21 08:58 textual_fspicker/path_filters.py
--rw-r--r--  2.0 unx     1369 b- defN 23-Jun-03 06:49 textual_fspicker/path_maker.py
+-rw-r--r--  2.0 unx     1399 b- defN 23-Jun-04 07:57 textual_fspicker/path_maker.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-18 20:02 textual_fspicker/py.typed
 -rw-r--r--  2.0 unx     2174 b- defN 23-May-19 09:53 textual_fspicker/safe_tests.py
--rw-r--r--  2.0 unx     2457 b- defN 23-May-22 20:47 textual_fspicker/select_directory.py
+-rw-r--r--  2.0 unx     2735 b- defN 23-Jun-04 07:57 textual_fspicker/select_directory.py
 -rw-r--r--  2.0 unx      389 b- defN 23-May-17 19:18 textual_fspicker/parts/__init__.py
--rw-r--r--  2.0 unx    15288 b- defN 23-Jun-03 07:21 textual_fspicker/parts/directory_navigation.py
--rw-r--r--  2.0 unx     4235 b- defN 23-Jun-04 06:41 textual_fspicker-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 06:41 textual_fspicker-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jun-04 06:41 textual_fspicker-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-04 06:41 textual_fspicker-0.0.8.dist-info/RECORD
-17 files, 46758 bytes uncompressed, 14810 bytes compressed:  68.3%
+-rw-r--r--  2.0 unx    15251 b- defN 23-Jun-04 07:57 textual_fspicker/parts/directory_navigation.py
+-rw-r--r--  2.0 unx     4235 b- defN 23-Jun-04 07:57 textual_fspicker-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-04 07:57 textual_fspicker-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-04 07:57 textual_fspicker-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1480 b- defN 23-Jun-04 07:57 textual_fspicker-0.0.9.dist-info/RECORD
+17 files, 47255 bytes uncompressed, 14949 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: textual_fspicker/parts/__init__.py
 Comment: 
 
 Filename: textual_fspicker/parts/directory_navigation.py
 Comment: 
 
-Filename: textual_fspicker-0.0.8.dist-info/METADATA
+Filename: textual_fspicker-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: textual_fspicker-0.0.8.dist-info/WHEEL
+Filename: textual_fspicker-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: textual_fspicker-0.0.8.dist-info/top_level.txt
+Filename: textual_fspicker-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: textual_fspicker-0.0.8.dist-info/RECORD
+Filename: textual_fspicker-0.0.9.dist-info/RECORD
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
-__version__    = "0.0.8"
+__version__    = "0.0.9"
 __licence__    = "MIT"
 
 ##############################################################################
 # Local imports.
 from .file_open        import FileOpen
 from .file_save        import FileSave
 from .select_directory import SelectDirectory
```

## textual_fspicker/__main__.py

```diff
@@ -1,12 +1,13 @@
 """Main entry point for testing the library."""
 
 ##############################################################################
 # Python imports.
-from pathlib import Path
+from __future__ import annotations
+from pathlib    import Path
 
 ##############################################################################
 # Textual imports.
 from textual            import on
 from textual.app        import App, ComposeResult
 from textual.containers import Center, Horizontal
 from textual.widgets    import Label, Button, Footer
@@ -46,21 +47,21 @@
             yield Button( "Open a file", id="open" )
             yield Button( "Save a file", id="save" )
             yield Button( "Select a directory", id="directory" )
         with Center():
             yield Label( "Press the button to pick something" )
         yield Footer()
 
-    def show_selected( self, to_show: Path ) -> None:
+    def show_selected( self, to_show: Path | None ) -> None:
         """Show the file that was selected by the user.
 
         Args:
             to_show: The file to show.
         """
-        self.query_one( Label ).update( str( to_show ) )
+        self.query_one( Label ).update( "Cancelled" if to_show is None else str( to_show ) )
 
     @on( Button.Pressed, "#open" )
     def open_file( self ) -> None:
         """Show the `FileOpen` dialog when the button is pushed."""
         self.push_screen(
             FileOpen( ".", filters=Filters(
                 ( "Python",  lambda p: p.suffix.lower() == ".py" ),
```

## textual_fspicker/base_dialog.py

```diff
@@ -1,13 +1,14 @@
 """The base dialog code for the other dialogs in the library."""
 
 ##############################################################################
 # Python imports.
 from __future__ import annotations
 from pathlib    import Path
+from typing     import Optional
 
 ##############################################################################
 # Textual imports.
 from textual            import on
 from textual.app        import ComposeResult
 from textual.binding    import Binding
 from textual.containers import Horizontal, Vertical
@@ -23,15 +24,15 @@
     """Layout class for the main dialog area."""
 
 ##############################################################################
 class InputBar( Horizontal ):
     """The input bar area of the dialog."""
 
 ##############################################################################
-class FileSystemPickerScreen( ModalScreen[ Path ] ):
+class FileSystemPickerScreen( ModalScreen[ Optional[ Path ] ] ):
     """Base screen for the dialogs in this library."""
 
     DEFAULT_CSS = """
     FileSystemPickerScreen {
         align: center middle;
     }
 
@@ -57,24 +58,25 @@
     FileSystemPickerScreen InputBar Button {
         margin-left: 1;
     }
     """
 
     BINDINGS = [
         Binding( "full_stop", "hidden" ),
-        Binding( "escape", "dismiss" )
+        Binding( "escape", "dismiss( None )" )
     ]
     """The bindings for the dialog."""
 
-    def __init__( self, location: str | Path | None = None, title: str = "", select_button: str = "" ) -> None:
+    def __init__( self, location: str | Path = ".", title: str = "", select_button: str = "" ) -> None:
         """Initialise the dialog.
 
         Args:
             location: Optional starting location.
             title: Optional title.
+            select_button: Label for the select button.
         """
         super().__init__()
         self._location = location
         """The starting location."""
         self._title = title
         """The title for the dialog."""
         self._select_button = select_button or "Select"
@@ -120,14 +122,14 @@
     def _cancel( self, event: Button.Pressed ) -> None:
         """Cancel the dialog.
 
         Args:
             event: The even to handle.
         """
         event.stop()
-        self.dismiss()
+        self.dismiss( None )
 
     def action_hidden( self ) -> None:
         """Action for toggling the display of hidden entries."""
         self.query_one( DirectoryNavigation ).toggle_hidden()
 
 ### base_dialog.py ends here
```

## textual_fspicker/file_dialog.py

```diff
@@ -35,25 +35,26 @@
     BaseFileDialog InputBar Select {
         width: 1fr;
     }
     """
 
     def __init__(
         self,
-        location: str | Path | None = None,
+        location: str | Path = ".",
         title: str = "Open",
         select_button: str = "",
         *,
         filters: Filters | None = None
     ) -> None:
         """Initialise the base dialog dialog.
 
         Args:
             location: Optional starting location.
             title: Optional title.
+            select_button: The label for the selection button.
             filters: Optional filters to show in the dialog.
         """
         super().__init__( location, title, select_button=select_button )
         self._filters = filters
         """The filters for the dialog."""
 
     def _input_bar( self ) -> ComposeResult:
```

## textual_fspicker/file_open.py

```diff
@@ -12,27 +12,27 @@
 
 ##############################################################################
 class FileOpen( BaseFileDialog ):
     """A file opening dialog."""
 
     def __init__(
         self,
-        location: str | Path | None = None,
+        location: str | Path = ".",
         title: str = "Open",
         *,
         filters: Filters | None = None,
         must_exist: bool = True
     ) -> None:
         """Initialise the `FileOpen` dialog.
 
         Args:
             location: Optional starting location.
             title: Optional title.
-            must_exist: Flag to say if the file must exist.
             filters: Optional filters to show in the dialog.
+            must_exist: Flag to say if the file must exist.
         """
         super().__init__( location, title, select_button="Open", filters=filters )
         self._must_exist = must_exist
         """Must the file exist?"""
 
     def _should_return( self, candidate: Path ) -> bool:
         """Perform the final checks on the chosen file.
```

## textual_fspicker/file_save.py

```diff
@@ -12,15 +12,15 @@
 
 ##############################################################################
 class FileSave( BaseFileDialog ):
     """A file save dialog."""
 
     def __init__(
         self,
-        location: str | Path | None = None,
+        location: str | Path = ".",
         title: str = "Save as",
         *,
         filters: Filters | None = None,
         can_overwrite: bool = True
     ) -> None:
         """Initialise the `FileOpen` dialog.
```

## textual_fspicker/path_maker.py

```diff
@@ -25,15 +25,15 @@
 
         Args:
             path_maker: The callable to set as the Path builder.
         """
         cls._path = path_maker
 
     @classmethod
-    def of( cls, out_of: str | Path="" ) -> Path:
+    def of( cls, out_of: str | Path="" ) -> Path: # pylint:disable=invalid-name
         """Make a Path out of the given value.
 
         Args:
             out_of: The value to make a path out of.
 
         Returns:
             An instance of a Path or a related class.
```

## textual_fspicker/select_directory.py

```diff
@@ -25,42 +25,52 @@
         width: 1fr;
         border: tall $background;
         padding-left: 1;
         padding-right: 1;
     }
     """
 
-    def __init__( self, location: str | Path | None = None, title: str = "Select directory" ) -> None:
+    def __init__( self, location: str | Path = ".", title: str = "Select directory" ) -> None:
         """Initialise the dialog.
 
         Args:
             location: Optional starting location.
             title: Optional title.
         """
         super().__init__( location, title )
 
     def on_mount( self ) -> None:
         """Configure the dialog once the DOM is ready."""
-        self.query_one( DirectoryNavigation ).show_files = False
+        navigation = self.query_one( DirectoryNavigation )
+        navigation.show_files = False
+        self._set_current( navigation.location )
 
     def _input_bar( self ) -> ComposeResult:
         """Provide any widgets for the input before, before the buttons."""
         yield Label()
 
+    def _set_current( self, location: Path ) -> None:
+        """Set the current location.
+
+        Args:
+            location: The location to indicate.
+        """
+        current_selection = self.query_one( "InputBar > Label", Label )
+        # TODO: A nicer way of indicating we're looking at just the tail.
+        current_selection.update( str( location )[ -current_selection.size.width: ] )
+
     @on( DirectoryNavigation.Changed )
     def _show_selected( self, event: DirectoryNavigation.Changed ) -> None:
         """Update the display of the current location.
 
         Args:
             event: The event with the selection information in.
         """
         event.stop()
-        current_selection = self.query_one( "InputBar > Label", Label )
-        # TODO: A nicer way of indicating we're looking at just the tail.
-        current_selection.update( str( event.control.location )[ -current_selection.size.width: ] )
+        self._set_current( event.control.location )
 
     @on( Button.Pressed, "#select" )
     def _select_directory( self, event: Button.Pressed ) -> None:
         """React to the select button being pressed.
 
         Args:
             event: The button press event.
```

## textual_fspicker/parts/directory_navigation.py

```diff
@@ -233,23 +233,23 @@
 
     show_hidden: var[ bool ] = var( False )
     """Should hidden entries be shown?"""
 
     sort_display: var[ bool ] = var( True )
     """Should the display be sorted?"""
 
-    def __init__( self, location: Path | str | None = None ) -> None:
+    def __init__( self, location: Path | str = "." ) -> None:
         """Initialise the directory navigation widget.
 
         Args:
             location: The starting location.
         """
         super().__init__()
         self._mounted                       = False
-        self.location                       = MakePath.of( "~" if location is None else location ).expanduser().absolute()
+        self.location                       = MakePath.of( location ).expanduser().absolute()
         self._entries: list[DirectoryEntry] = []
 
     @property
     def location( self ) -> Path:
         """The current location of the navigation widget."""
         return self._location
```

## Comparing `textual_fspicker-0.0.8.dist-info/METADATA` & `textual_fspicker-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textual-fspicker
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple Textual filesystem picker dialog library.
 Home-page: https://github.com/davep/textual-fspicker
 Author: Dave Pearson
 Author-email: davep@davep.org
 Maintainer: Dave Pearson
 Maintainer-email: davep@davep.org
 License: License :: OSI Approved :: MIT License
```

## Comparing `textual_fspicker-0.0.8.dist-info/RECORD` & `textual_fspicker-0.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-textual_fspicker/__init__.py,sha256=cudg6pv8kvK26BR_CAOtiOlbnMiUKZisJ33qGGobcJQ,915
-textual_fspicker/__main__.py,sha256=v57UBTiFOMwuIvpL0zcHpYs-BjkvPzINQACRoKIzRf0,3254
-textual_fspicker/base_dialog.py,sha256=qDbghAxRYU1K8723w1YarQfPwIVkzs8BO5xcBmXK1ZA,4231
-textual_fspicker/file_dialog.py,sha256=B6yyFVOzemGcVJYz0gcB-OzwxISELwWK2MfTocV_Ua4,5944
-textual_fspicker/file_open.py,sha256=eMXpA1xOmYoOPSMEcefVsk_lc2xH7Nn-x-mEJhhdblY,1521
-textual_fspicker/file_save.py,sha256=WIE9rRUvb_UCntMw47Hjmbqnq2xr8u1oE7VPGJ3I7H8,1570
+textual_fspicker/__init__.py,sha256=2QPkOs0tm4tSdOkHnB4gB8Af84JEOXqtnjFOdESwGb0,915
+textual_fspicker/__main__.py,sha256=rp_ChLrPW8kGPhQ7KaQKwS7GdiQASBG_K2BQ7YUqpXQ,3335
+textual_fspicker/base_dialog.py,sha256=N47y5-Vu4Aljx2Nah2B8FLUlU06hnjp_9Aenr9zH_LI,4337
+textual_fspicker/file_dialog.py,sha256=rUpuKkZCQK4LBHP_53oMTpfuxvCwUog-9xS6Ehs-1t0,5999
+textual_fspicker/file_open.py,sha256=T1UZW4qbroZaGynHn-o67CUs-GNCorUQ52iUxd9TE48,1513
+textual_fspicker/file_save.py,sha256=SvDt1YI-7ocQ5BqPxtRwxEZJTAuZcELCslMepTYyEvk,1562
 textual_fspicker/path_filters.py,sha256=XpPrynKVI_p8Tf6tUuhEmU5lxAaf3TQlsjKsRwXC5nk,1822
-textual_fspicker/path_maker.py,sha256=1wYOQ9EQKYu8kZBqH7kYv-qwdUwIpkybvwkDaZkc6zw,1369
+textual_fspicker/path_maker.py,sha256=g7w8a3MHPPwZA4X7wHSz3pwPlSEexg2Ud8DvHW0lPpk,1399
 textual_fspicker/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 textual_fspicker/safe_tests.py,sha256=U3gpqVRr7qcv7mqF-I_sFojtr9Pv5JyqFzAxGG7qofA,2174
-textual_fspicker/select_directory.py,sha256=vE1MYCL-_QqTyPiveJrxl90oEwjQB14lfSsHteUEBNM,2457
+textual_fspicker/select_directory.py,sha256=9N8068liIESPybmQZGsjBfeW-WvRm5S7E4q2PR0JkpY,2735
 textual_fspicker/parts/__init__.py,sha256=vjP1jzd5ty4IhwUZnVFkOjzctZn22EbwWDHh_16x-GM,389
-textual_fspicker/parts/directory_navigation.py,sha256=2nhPZoyDZstdmvzlR5UQcdTX5wbCoJz4JzZ8DK7hXKw,15288
-textual_fspicker-0.0.8.dist-info/METADATA,sha256=lUpmA-TBIJwWdwkUBFf5_7_h5UmrCarGLuTI0t3jt0w,4235
-textual_fspicker-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-textual_fspicker-0.0.8.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
-textual_fspicker-0.0.8.dist-info/RECORD,,
+textual_fspicker/parts/directory_navigation.py,sha256=eT1YC6QkVgZkFZA4SVwXLqa5KTIZgkQj7ZnPGpgE2JQ,15251
+textual_fspicker-0.0.9.dist-info/METADATA,sha256=a3OQAsaf0K22Ca5MgokHqiJNCCJEVzTW2P05MDVAMKQ,4235
+textual_fspicker-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+textual_fspicker-0.0.9.dist-info/top_level.txt,sha256=htFx3DXug_utI8h7tIJmd3FSxg6-fjXfcf4_Rd6ohLQ,17
+textual_fspicker-0.0.9.dist-info/RECORD,,
```

