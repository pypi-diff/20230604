# Comparing `tmp/mwxlib-0.84.7-py3-none-any.whl.zip` & `tmp/mwxlib-0.84.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 162072 bytes, number of entries: 22
+Zip file size: 162132 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-Jun-03 17:04 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43499 b- defN 23-Jun-03 17:04 mwx/controls.py
--rw-rw-rw-  2.0 fat    73816 b- defN 23-Jun-04 08:43 mwx/framework.py
--rw-rw-rw-  2.0 fat    68312 b- defN 23-Jun-04 08:43 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    73816 b- defN 23-Jun-04 13:38 mwx/framework.py
+-rw-rw-rw-  2.0 fat    68561 b- defN 23-Jun-04 13:38 mwx/graphman.py
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
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-04 08:45 mwxlib-0.84.7.dist-info/RECORD
-22 files, 614202 bytes uncompressed, 159570 bytes compressed:  74.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-Jun-04 13:40 mwxlib-0.84.8.dist-info/RECORD
+22 files, 614451 bytes uncompressed, 159630 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.84.7.dist-info/LICENSE
+Filename: mwxlib-0.84.8.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.84.7.dist-info/METADATA
+Filename: mwxlib-0.84.8.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.84.7.dist-info/WHEEL
+Filename: mwxlib-0.84.8.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.84.7.dist-info/top_level.txt
+Filename: mwxlib-0.84.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.84.7.dist-info/RECORD
+Filename: mwxlib-0.84.8.dist-info/RECORD
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
-__version__ = "0.84.7"
+__version__ = "0.84.8"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
```

## mwx/graphman.py

```diff
@@ -197,14 +197,15 @@
         dockable    : flag to set the pane to be dockable
                       type: bool or dock:int (1:t, 2:r, 3:b, 4:l, 5:c)
         reloadable  : flag to set the Layer to be reloadable
         unloadable  : flag to set the Layer to be unloadable
     
     Note:
         parent <Frame> is not always equal to Parent when floating.
+        Parent type can be <Frame>, <AuiFloatingFrame>, or <AuiNotebook>.
     """
     MENU = "Plugins" # default menu for Plugins
     menukey = property(lambda self: "{}/&{}".format(self.MENU, self.__module__))
     caption = True
     category = None
     dockable = True
     editable = True # to be deprecated
@@ -346,15 +347,15 @@
                     self.thread.active = 0
                     self.thread.Stop()
                 del self.Arts
             v.Skip()
         self.Bind(wx.EVT_WINDOW_DESTROY, destroy)
         
         def on_show(v):
-            if self and isinstance(self.Parent, aui.AuiNotebook):
+            if self.category: # -> notebook
                 if v.IsShown():
                     self.handler('page_shown', self)
                 else:
                     self.handler('page_hidden', self)
             v.Skip()
         self.Bind(wx.EVT_SHOW, on_show)
         
@@ -862,16 +863,19 @@
                 pane.Float()
                 show = True
         
         plug = self.get_plug(name) # -> None if pane.window is Graph
         win = pane.window # -> Window (plug / notebook / Graph)
         if show:
             if isinstance(win, aui.AuiNotebook):
-                win.SetSelection(win.GetPageIndex(plug)) # => [page_shown]
-            
+                j = win.GetPageIndex(plug)
+                if j != win.Selection:
+                    win.Selection = j # the focus is moved => [page_shown]
+                else:
+                    plug.handler('page_shown', plug)
             elif not pane.IsShown():
                 win.handler('page_shown', win)
         else:
             if isinstance(win, aui.AuiNotebook):
                 for plug in win.all_pages: # => [page_closed] to all pages
                     plug.handler('page_closed', plug)
             elif pane.IsShown():
@@ -1177,21 +1181,22 @@
         else:
             nb = None
             size = plug.GetSize()
             self._mgr.AddPane(plug, aui.AuiPaneInfo()
                                        .Name(name).Caption(caption)
                                        .FloatingSize(size).MinSize(size).Show(0))
         
-        ## set reference of notebook (optional)
-        plug.__notebook = nb
-        plug.__Menu_item = None
+        ## Set winow.Name for inspection.
         plug.Name = name
+        
         self.update_pane(name, **props)
         
         ## Create a menu
+        plug.__Menu_item = None
+        
         if not hasattr(module, 'ID_'): # give a unique index to the module
             global __plug_ID__ # cache ID *not* in [ID_LOWEST(4999):ID_HIGHEST(5999)]
             try:
                 __plug_ID__
             except NameError:
                 __plug_ID__ = 10000
             __plug_ID__ += 1
@@ -1228,20 +1233,21 @@
             
             if plug.__Menu_item:
                 menu, sep, tail = plug.menukey.rpartition('/')
                 menu = menu or Layer.MENU
                 self.menubar[menu].remove(plug.__Menu_item)
                 self.menubar.update(menu)
             
-            nb = plug.__notebook
-            if nb:
+            if isinstance(plug.Parent, aui.AuiNotebook):
+                nb = plug.Parent
                 j = nb.GetPageIndex(plug)
                 nb.RemovePage(j) # just remove page
                 ## nb.DeletePage(j) # cf. destroy plug object too
             else:
+                nb = None
                 self._mgr.DetachPane(plug)
                 self._mgr.Update()
             
             plug.handler('page_closed', plug) # (even if not shown)
             plug.Destroy()
             
             if nb and not nb.PageCount:
```

## Comparing `mwxlib-0.84.7.dist-info/LICENSE` & `mwxlib-0.84.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.84.7.dist-info/METADATA` & `mwxlib-0.84.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.84.7
+Version: 0.84.8
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.84.7.dist-info/RECORD` & `mwxlib-0.84.8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=bSRdncjfSCKycMFQVnagOi9R2vUCC5snGkjea7jqPgU,2520
 mwx/controls.py,sha256=pD1IjgkwdvD-ebntnAH-6Jo7KY5hDq30Ne6rTE_i9fE,43499
-mwx/framework.py,sha256=x8a-rEsIoGwycAMhPM3G9UcTCXYUOixVrq_BhmyHg5M,73816
-mwx/graphman.py,sha256=H4501ZK0YMX52woEJHg7NlEvE-iuF7CKvgV3XzTgpLQ,68312
+mwx/framework.py,sha256=FREzT3tMg6wXLvVmJhRMEuc8KHLH655JT0Zoxtc5a3E,73816
+mwx/graphman.py,sha256=rDOYa3IZVp48hD0bio7fCwIG0-dNWjdZHm1cvfINszY,68561
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
-mwxlib-0.84.7.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.84.7.dist-info/METADATA,sha256=S4H6IiZhEuzEV4oMaMhMBMDuEj3tM1LgEhf3QHKFimo,1893
-mwxlib-0.84.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.84.7.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.84.7.dist-info/RECORD,,
+mwxlib-0.84.8.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.84.8.dist-info/METADATA,sha256=xZ7328VNHvIs8oA83rx-zd5jDLlh6jTIQfGO6kg3NkI,1893
+mwxlib-0.84.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.84.8.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.84.8.dist-info/RECORD,,
```

