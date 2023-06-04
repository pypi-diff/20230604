# Comparing `tmp/mwxlib-0.84.6-py3-none-any.whl.zip` & `tmp/mwxlib-0.84.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 162025 bytes, number of entries: 22
+Zip file size: 162072 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-Jun-03 17:04 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43499 b- defN 23-Jun-03 17:04 mwx/controls.py
--rw-rw-rw-  2.0 fat    73816 b- defN 23-Jun-04 08:46 mwx/framework.py
--rw-rw-rw-  2.0 fat    68211 b- defN 23-Jun-04 08:46 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    73816 b- defN 23-Jun-04 08:43 mwx/framework.py
+-rw-rw-rw-  2.0 fat    68312 b- defN 23-Jun-04 08:43 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-Jun-03 17:04 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-Jun-03 17:04 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27598 b- defN 23-Jun-03 17:04 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
 -rw-rw-rw-  2.0 fat   138759 b- defN 23-Jun-03 17:04 mwx/nutshell.py
 -rw-rw-rw-  2.0 fat    37431 b- defN 23-Jun-03 17:04 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11343 b- defN 23-Jun-03 17:04 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19367 b- defN 23-Jun-03 17:04 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-Jun-03 17:04 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7424 b- defN 23-Jun-03 17:04 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Jun-03 17:04 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-04 08:47 mwxlib-0.84.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-04 08:47 mwxlib-0.84.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 08:47 mwxlib-0.84.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-04 08:47 mwxlib-0.84.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-04 08:47 mwxlib-0.84.6.dist-info/RECORD
-22 files, 614101 bytes uncompressed, 159523 bytes compressed:  74.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/RECORD
+22 files, 614202 bytes uncompressed, 159570 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.84.6.dist-info/LICENSE
+Filename: mwxlib-0.84.7.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.84.6.dist-info/METADATA
+Filename: mwxlib-0.84.7.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.84.6.dist-info/WHEEL
+Filename: mwxlib-0.84.7.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.84.6.dist-info/top_level.txt
+Filename: mwxlib-0.84.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.84.6.dist-info/RECORD
+Filename: mwxlib-0.84.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.84.6"
+__version__ = "0.84.7"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
```

## mwx/graphman.py

```diff
@@ -218,15 +218,15 @@
     
     ## thread_type = Thread
     thread = None
     
     ## funcall = interactive_call
     funcall = staticmethod(_F)
     
-    ## for debug
+    ## for debug (internal use only)
     pane = property(lambda self: self.parent.get_pane(self))
     
     @property
     def Arts(self):
         """List of arts <matplotlib.artist.Artist>."""
         return self.__artists
     
@@ -346,18 +346,19 @@
                     self.thread.active = 0
                     self.thread.Stop()
                 del self.Arts
             v.Skip()
         self.Bind(wx.EVT_WINDOW_DESTROY, destroy)
         
         def on_show(v):
-            if v.IsShown():
-                self.handler('page_shown', self)
-            else:
-                self.handler('page_hidden', self)
+            if self and isinstance(self.Parent, aui.AuiNotebook):
+                if v.IsShown():
+                    self.handler('page_shown', self)
+                else:
+                    self.handler('page_hidden', self)
             v.Skip()
         self.Bind(wx.EVT_SHOW, on_show)
         
         try:
             self.Init()
             if session:
                 self.load_session(session)
@@ -827,73 +828,66 @@
         
         Args:
             name : str or plug object.
         """
         if name in self.plugins:
             plug = self.plugins[name].__plug__
             name = plug.category or name
-        elif _isLayer(name):
-            if name: # Check if wrapped C/C++ object of Layer has been deleted.
-                name = name.category or name
-            else:
-                name = '' # to return a dummy pane
+        elif name and _isLayer(name):
+            ## Also check if wrapped C/C++ object of Layer has been deleted.
+            name = name.category or name
         return self._mgr.GetPane(name)
     
-    def show_pane(self, name, show=True):
+    def show_pane(self, name, show=True, interactive=False):
         """Show named pane or notebook pane."""
         pane = self.get_pane(name)
-        plug = self.get_plug(name)
         if not pane.IsOk():
             return
         
         ## Set the graph and output window sizes to half & half.
         if name == "output" or name is self.output:
             w, h = self.graph.GetClientSize()
             pane.best_size = (w//2, h) # ドッキング時に再計算される
         
         ## Force Layer windows to show.
-        if _isLayer(plug):
+        if interactive:
             ## [M-menu] Reload plugin (ret: None if succeeded).
             if wx.GetKeyState(wx.WXK_ALT):
                 self.reload_plug(name)
                 pane = self.get_pane(name)
                 show = True
             
             ## [S-menu] Reset floating position of a stray window.
             if wx.GetKeyState(wx.WXK_SHIFT):
                 pane.floating_pos = wx.GetMousePosition()
                 pane.Float()
                 show = True
         
-        self._show_pane(name, show)
-        self._mgr.Update()
-    
-    def _show_pane(self, name, show=True):
-        """Show named pane window (internal use only)."""
-        pane = self.get_pane(name)
-        plug = self.get_plug(name)
-        if plug:
-            nb = plug.__notebook # given when load_plug
-            if nb and show:
-                nb.SetSelection(nb.GetPageIndex(plug))
-        
-        win = plug or pane.window
+        plug = self.get_plug(name) # -> None if pane.window is Graph
+        win = pane.window # -> Window (plug / notebook / Graph)
         if show:
-            if not pane.IsShown():
+            if isinstance(win, aui.AuiNotebook):
+                win.SetSelection(win.GetPageIndex(plug)) # => [page_shown]
+            
+            elif not pane.IsShown():
                 win.handler('page_shown', win)
         else:
-            if pane.IsShown():
+            if isinstance(win, aui.AuiNotebook):
+                for plug in win.all_pages: # => [page_closed] to all pages
+                    plug.handler('page_closed', plug)
+            elif pane.IsShown():
                 win.handler('page_closed', win)
         
         ## Modify the floating position of the pane when displayed.
         ## Note: This is a known bug in wxWidgets 3.17 -- 3.20,
         ##       and will be fixed in wxPython 4.2.1.
         if wx.Display.GetFromWindow(pane.window) == -1:
             pane.floating_pos = wx.GetMousePosition()
         pane.Show(show)
+        self._mgr.Update()
     
     def update_pane(self, name, show=False, **kwargs):
         """Update the layout of the pane.
         
         Note:
             This is called automatically from load_plug,
             and should not be called directly from user.
@@ -919,15 +913,15 @@
         
         dock = kwargs.get('dock')
         pane.dock_direction = dock or 0
         if dock:
             pane.Dock()
         else:
             pane.Float()
-        self._show_pane(name, show)
+        self.show_pane(name, show)
         self._mgr.Update()
     
     def OnPaneClose(self, evt): #<wx.aui.AuiManagerEvent>
         pane = evt.GetPane()
         win = pane.window
         if isinstance(win, aui.AuiNotebook):
             for plug in win.all_pages:
@@ -964,17 +958,17 @@
             name : str or plug object.
         """
         if isinstance(name, str):
             if name.endswith(".py") or name.endswith(".pyc"):
                 name,_ = os.path.splitext(os.path.basename(name))
             if name in self.plugins:
                 return self.plugins[name].__plug__
-        elif _isLayer(name):
-            if name: # Check if wrapped C/C++ object of Layer has been deleted.
-                return name
+        elif name and _isLayer(name):
+            ## Also check if wrapped C/C++ object of Layer has been deleted.
+            return name
     
     @staticmethod
     def register(cls, module=None):
         """Register dummy plug; Add module.Plugin(Layer).
         """
         if not module:
             module = inspect.getmodule(cls) # rebase module or __main__
@@ -1095,15 +1089,15 @@
         """
         props = dict(show=show,
                      dock=dock, layer=layer, pos=pos, row=row, prop=prop,
                      floating_pos=floating_pos, floating_size=floating_size)
         
         module = self.load_module(root, force, session, **props)
         if not module:
-            return module # None or False
+            return module # None (if not force) or False (failed to import)
         
         try:
             name = module.Plugin.__module__
             title = module.Plugin.category
             
             pane = self._mgr.GetPane(title)
             
@@ -1206,15 +1200,15 @@
         if plug.menukey:
             menu, sep, tail = plug.menukey.rpartition('/')
             menu = menu or Layer.MENU
             text = tail or plug.__module__
             hint = (plug.__doc__ or name).strip().splitlines()[0]
             plug.__Menu_item = (
                 module.ID_, text, hint, wx.ITEM_CHECK,
-                lambda v: self.show_pane(name, v.IsChecked()),
+                lambda v: self.show_pane(name, v.IsChecked(), interactive=1),
                 lambda v: v.Check(self.get_pane(name).IsShown()),
             )
             if menu not in self.menubar:
                 self.menubar[menu] = []
             self.menubar[menu] += [plug.__Menu_item]
             self.menubar.update(menu)
         return None
```

## Comparing `mwxlib-0.84.6.dist-info/LICENSE` & `mwxlib-0.84.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.84.6.dist-info/METADATA` & `mwxlib-0.84.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.84.6
+Version: 0.84.7
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.84.6.dist-info/RECORD` & `mwxlib-0.84.7.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
 mwx/controls.py,sha256=pD1IjgkwdvD-ebntnAH-6Jo7KY5hDq30Ne6rTE_i9fE,43499
-mwx/framework.py,sha256=_xEyhQCLiybNR5mjO11x8RzzxXwcrM2ZQw5GmA3I0nY,73816
-mwx/graphman.py,sha256=g5pRrWysU-9yK3RY72hlu2nUM93ZK4NZQB-3E_nMH6U,68211
+mwx/framework.py,sha256=x8a-rEsIoGwycAMhPM3G9UcTCXYUOixVrq_BhmyHg5M,73816
+mwx/graphman.py,sha256=H4501ZK0YMX52woEJHg7NlEvE-iuF7CKvgV3XzTgpLQ,68312
 mwx/images.py,sha256=9e8X7OpJ6Z3fF3ez17P_qk2D1NMO10-lN8TCtulAqT0,46248
 mwx/matplot2.py,sha256=W_FpY0S33crCAh7N9YTXo-jgYzj8uL9gqXkekfQo7Pk,36017
 mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
 mwx/matplot2lg.py,sha256=vVlBulRQDyYonI9EKfqp-3SpNbGyIJQ6ldkw6bZlalo,27598
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
 mwx/nutshell.py,sha256=ajJBsC9o_21DuYuw5mwRGpB4GgwWT2rOjlf-DS-ntLI,138759
 mwx/utilus.py,sha256=ADA8I7qg339TJOvbrWWD91jqICWfc5C-ENFE-a7YBvU,37431
 mwx/wxmon.py,sha256=hEXto7dD5JunPf-iv2hhcwTIILLkNPlcl6wRt20_Wqc,11343
 mwx/wxpdb.py,sha256=M_xxXzIYhAwO1IHXVkjIC4Y2JCCCGLdgPL5R4bRtp04,19367
 mwx/wxwil.py,sha256=DPXXx4OdEzvHr-_jxz9J29Ozufmb6Vr7rXVkG_LKQd0,5254
 mwx/wxwit.py,sha256=UG361QTUheO_hlSIRgkprrGUYh0IzHB8ZqOoJeeMzUs,7424
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.84.6.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.84.6.dist-info/METADATA,sha256=wizHJAqVB8N_Bgam9rtlHXf65O1k2QKV4DbbUYNOIOM,1893
-mwxlib-0.84.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.84.6.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.84.6.dist-info/RECORD,,
+mwxlib-0.84.7.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.84.7.dist-info/METADATA,sha256=S4H6IiZhEuzEV4oMaMhMBMDuEj3tM1LgEhf3QHKFimo,1893
+mwxlib-0.84.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.84.7.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.84.7.dist-info/RECORD,,
```

