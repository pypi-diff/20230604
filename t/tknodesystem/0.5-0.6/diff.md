# Comparing `tmp/tknodesystem-0.5.tar.gz` & `tmp/tknodesystem-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tknodesystem-0.5.tar", last modified: Thu Jun  1 09:08:33 2023, max compression
+gzip compressed data, was "tknodesystem-0.6.tar", last modified: Sun Jun  4 11:00:21 2023, max compression
```

## Comparing `tknodesystem-0.5.tar` & `tknodesystem-0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:08:33.399585 tknodesystem-0.5/
--rw-rw-rw-   0        0        0     1086 2023-05-17 15:31:54.000000 tknodesystem-0.5/LICENSE
--rw-rw-rw-   0        0        0     2711 2023-06-01 09:08:33.399585 tknodesystem-0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2142 2023-06-01 08:59:10.000000 tknodesystem-0.5/README.md
--rw-rw-rw-   0        0        0      570 2023-06-01 09:08:33.402587 tknodesystem-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1193 2023-06-01 08:55:45.000000 tknodesystem-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:08:33.367100 tknodesystem-0.5/tknodesystem/
--rw-rw-rw-   0        0        0      278 2023-05-23 07:46:35.000000 tknodesystem-0.5/tknodesystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:08:33.387365 tknodesystem-0.5/tknodesystem/grid_images/
--rw-rw-rw-   0        0        0    58394 2023-05-12 09:24:10.000000 tknodesystem-0.5/tknodesystem/grid_images/grid_dot.png
--rw-rw-rw-   0        0        0    25170 2023-05-10 10:57:06.000000 tknodesystem-0.5/tknodesystem/grid_images/grid_lines.png
--rw-rw-rw-   0        0        0     9365 2023-05-12 08:37:01.000000 tknodesystem-0.5/tknodesystem/grid_images/no_grid.png
--rw-rw-rw-   0        0        0     4747 2023-06-01 06:29:09.000000 tknodesystem-0.5/tknodesystem/node.py
--rw-rw-rw-   0        0        0     3175 2023-06-01 09:02:46.000000 tknodesystem-0.5/tknodesystem/node_args.py
--rw-rw-rw-   0        0        0    11797 2023-06-01 07:12:09.000000 tknodesystem-0.5/tknodesystem/node_canvas.py
--rw-rw-rw-   0        0        0     9395 2023-05-23 07:46:16.000000 tknodesystem-0.5/tknodesystem/node_menu.py
--rw-rw-rw-   0        0        0     5147 2023-06-01 06:43:40.000000 tknodesystem-0.5/tknodesystem/node_socket.py
--rw-rw-rw-   0        0        0    33308 2023-06-01 08:14:13.000000 tknodesystem-0.5/tknodesystem/node_types.py
--rw-rw-rw-   0        0        0     4340 2023-05-20 06:06:53.000000 tknodesystem-0.5/tknodesystem/node_wire.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:08:33.387365 tknodesystem-0.5/tknodesystem.egg-info/
--rw-rw-rw-   0        0        0     2711 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-01 09:08:33.000000 tknodesystem-0.5/tknodesystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 11:00:21.200534 tknodesystem-0.6/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 15:31:54.000000 tknodesystem-0.6/LICENSE
+-rw-rw-rw-   0        0        0     2711 2023-06-04 11:00:21.200534 tknodesystem-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2142 2023-06-01 08:59:10.000000 tknodesystem-0.6/README.md
+-rw-rw-rw-   0        0        0      570 2023-06-04 11:00:21.216163 tknodesystem-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2023-06-04 10:49:56.000000 tknodesystem-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:00:21.169274 tknodesystem-0.6/tknodesystem/
+-rw-rw-rw-   0        0        0      278 2023-06-03 17:03:07.000000 tknodesystem-0.6/tknodesystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:00:21.200534 tknodesystem-0.6/tknodesystem/grid_images/
+-rw-rw-rw-   0        0        0    58394 2023-05-12 09:24:10.000000 tknodesystem-0.6/tknodesystem/grid_images/grid_dot.png
+-rw-rw-rw-   0        0        0    25170 2023-05-10 10:57:06.000000 tknodesystem-0.6/tknodesystem/grid_images/grid_lines.png
+-rw-rw-rw-   0        0        0     9365 2023-05-12 08:37:01.000000 tknodesystem-0.6/tknodesystem/grid_images/no_grid.png
+-rw-rw-rw-   0        0        0     5582 2023-06-03 17:00:11.000000 tknodesystem-0.6/tknodesystem/node.py
+-rw-rw-rw-   0        0        0     3222 2023-06-04 10:05:13.000000 tknodesystem-0.6/tknodesystem/node_args.py
+-rw-rw-rw-   0        0        0    11737 2023-06-04 10:37:37.000000 tknodesystem-0.6/tknodesystem/node_canvas.py
+-rw-rw-rw-   0        0        0     9395 2023-05-23 07:46:16.000000 tknodesystem-0.6/tknodesystem/node_menu.py
+-rw-rw-rw-   0        0        0     5054 2023-06-04 10:36:06.000000 tknodesystem-0.6/tknodesystem/node_socket.py
+-rw-rw-rw-   0        0        0    33428 2023-06-04 10:39:37.000000 tknodesystem-0.6/tknodesystem/node_types.py
+-rw-rw-rw-   0        0        0     4267 2023-06-03 16:53:18.000000 tknodesystem-0.6/tknodesystem/node_wire.py
+drwxrwxrwx   0        0        0        0 2023-06-04 11:00:21.200534 tknodesystem-0.6/tknodesystem.egg-info/
+-rw-rw-rw-   0        0        0     2711 2023-06-04 11:00:21.000000 tknodesystem-0.6/tknodesystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-06-04 11:00:21.000000 tknodesystem-0.6/tknodesystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-06-04 11:00:21.000000 tknodesystem-0.6/tknodesystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 11:00:21.000000 tknodesystem-0.6/tknodesystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-04 11:00:21.000000 tknodesystem-0.6/tknodesystem.egg-info/top_level.txt
```

### Comparing `tknodesystem-0.5/LICENSE` & `tknodesystem-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.5/PKG-INFO` & `tknodesystem-0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tknodesystem
-Version: 0.5
+Version: 0.6
 Summary: Simple visual node system (DAG) with tkinter!
 Home-page: https://github.com/Akascape/TkNodeSystem
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes,visual-scripting
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tknodesystem-0.5/README.md` & `tknodesystem-0.6/README.md`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.5/setup.cfg` & `tknodesystem-0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6b6e 6f64 6573 7973 7465 6d0d   = tknodesystem.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e35 0d0a  .version = 0.5..
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e36 0d0a  .version = 0.6..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 5369  description = Si
 00000040: 6d70 6c65 2056 6973 7561 6c20 4e6f 6465  mple Visual Node
 00000050: 2073 7973 7465 6d20 7769 7468 2054 6b69   system with Tki
 00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
```

### Comparing `tknodesystem-0.5/setup.py` & `tknodesystem-0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'tknodesystem',
-    version = '0.5',
+    version = '0.6',
     description = "Simple visual node system (DAG) with tkinter!",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/TkNodeSystem",
```

### Comparing `tknodesystem-0.5/tknodesystem/grid_images/grid_dot.png` & `tknodesystem-0.6/tknodesystem/grid_images/grid_dot.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.5/tknodesystem/grid_images/grid_lines.png` & `tknodesystem-0.6/tknodesystem/grid_images/grid_lines.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.5/tknodesystem/grid_images/no_grid.png` & `tknodesystem-0.6/tknodesystem/grid_images/no_grid.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.5/tknodesystem/node.py` & `tknodesystem-0.6/tknodesystem/node.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,17 @@
         self.text = text
         self.center = center
         self.click_command = click_command
         self.auxlist = []
         self.signal = False
         self.hover = hover
         self.hover_color = highlightcolor
-        
         self.create()
-       
+        self.canvas.node_list.add(self)
+        
     def create(self):
         """ create round rectangular frame with text """
         
         self.ID = self.create_round_rectangle(self.center[0]-self.width*0.5, self.center[1]-self.height*0.5,
                                               self.center[0]+self.width*0.5, self.center[1]+self.height*0.5,
                                               radius=self.corner_radius, outline=self.node_outline_color, fill=self.node_color,
                                               width=self.node_outline_thickness)
@@ -67,33 +67,59 @@
         """ place the node items based one the motion of mouse """
 
         for id_ in self.allIDs:
             self.canvas.move(id_, event.x-self.xy_set[0], event.y-self.xy_set[1]) 
             self.canvas.tag_raise(id_)
             
         self.xy_set = (event.x, event.y)
+
+        self.update_sockets()
         
+    def update_sockets(self):
+        """ update the coordinates of sockets and lines """
+        self.output_.update()
+        try:
+            self.input_1.update()
+            self.input_2.update()
+            self.input_3.update()
+            self.input_4.update()
+            self.input_5.update()
+        except AttributeError: None
+
+        for i in self.canvas.line_ids:
+            i.update()
+
+        deleted = set()
+        for i in self.canvas.line_ids:
+            if not i.connected:
+                deleted.add(i)
+        self.canvas.line_ids = self.canvas.line_ids.difference(deleted)
+ 
     def move(self, x, y):
         for id_ in self.allIDs:
             self.canvas.move(id_, x, y) 
             self.canvas.tag_raise(id_)
-    
+        self.update_sockets()
+        
     def enter_node(self, event):
         if self.hover:
             self.canvas.itemconfigure(self.ID, outline=self.hover_color, width=self.node_outline_thickness+1)
         self.signal = True
         
     def leave_node(self, event):
         if self.hover:
             self.canvas.itemconfigure(self.ID, outline=self.node_outline_color, width=self.node_outline_thickness)
         self.signal = False
     
     def destroy(self):
         self.canvas.delete(self.ID, self.IDtext)
-        
+        self.canvas.node_list.remove(self)
+        for i in self.canvas.line_ids:
+            i.update()
+            
     def configure(self, **kwargs):
         """ configure options """
         
         if "fg_color" in kwargs:
             self.canvas.itemconfig(self.ID, fill=kwargs.pop("fg_color"))
         if "highlightcolor" in kwargs:
             self.hover_color = kwargs.pop("highlightcolor")
```

### Comparing `tknodesystem-0.5/tknodesystem/node_args.py` & `tknodesystem-0.6/tknodesystem/node_args.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 class Args():
     """ This class is used to remove default arguments in order to reduce the size of the export file """
     
     def value_args(args):        
         default_args = {'width': 100, 'height': 50, 'value': 0, 'border_color': 'white', 'text': None, 
                         'corner_radius': 25, 'border_width': 0, 'fg_color': '#37373D', 'text_color': 'white',
                         'font': ('', 10), 'socket_radius': 8, 'socket_hover': True, 'socket_color': 'green',
-                        'socket_hover_color': 'grey50', 'highlightcolor': '#52d66c', 'hover': True, 
+                        'socket_hover_color': 'grey50', 'highlightcolor': '#52d66c', 'hover': True, 'fixed': False,
                         'click_command': None, 'side': 'right', 'x': None, 'y': None, 'num': None, 'justify': 'center'}
 
         args.pop("canvas")
         args.pop("self")
         args.pop("__class__")
         args.pop("x")
         args.pop("y")
@@ -23,15 +23,15 @@
 
         return new_args
     
     def func_args(args):
         default_args = {'width': 100, 'height': 80, 'inputs': 2, 'border_color': '#37373D', 'text': None, 'socket_radius': 8,
                         'corner_radius': 25, 'border_width': 0, 'fg_color': '#37373D', 'text_color': 'white', 'font': ('', 10),
                         'highlightcolor': '#52d66c', 'hover': True, 'socket_color': 'green', 'socket_hover_color': 'grey50',
-                        'x': None, 'y': None, 'multiside': False, 'output_socket_color': 'green', 'click_command': None,
+                        'x': None, 'y': None, 'multiside': False, 'output_socket_color': 'green', 'click_command': None, 'fixed': False,
                         'socket_hover': True, 'num': None, 'none_inputs': False, 'justify': 'center', 'hover_text': None}
 
         args.pop("canvas")
         args.pop("self")
         args.pop("__class__")
         args.pop("command")
         args.pop("x")
@@ -45,15 +45,15 @@
                 new_args.update({i:args.get(i)})
 
         return new_args
 
     def compile_args(args):
         default_args = {'width': 100, 'height': 50, 'border_color': '#37373D', 'text': 'Compile', 'socket_radius': 8, 'justify': 'center',
                         'corner_radius': 25, 'x': None, 'y': None, 'border_width': 0, 'fg_color': '#37373D', 'text_color': 'white',
-                        'font': ('', 10), 'highlightcolor': '#52d66c', 'hover': True, 'socket_hover': True, 'socket_color': 'green',
+                        'font': ('', 10), 'highlightcolor': '#52d66c', 'hover': True, 'socket_hover': True, 'socket_color': 'green', 'fixed': False,
                         'socket_hover_color': 'grey50', 'show_value': True, 'command': None, 'click_command': None, 'side': 'left', 'num': None}
         
         args.pop("canvas")
         args.pop("self")
         args.pop("__class__")
         args.pop("command")
         args.pop("x")
```

### Comparing `tknodesystem-0.5/tknodesystem/node_canvas.py` & `tknodesystem-0.6/tknodesystem/node_canvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 class NodeCanvas(tkinter.Canvas):
     def __init__(self, master, bg="grey10", width=500, height=500, wire_color="white", wire_width=3,
                  grid_image="lines", zoom=True, wire_dash=True, move=True, wire_hover_color="red", **kwargs):
         
         super().__init__(master, bg=bg, width=width, height=height, bd=0, highlightthickness=0, **kwargs)
 
         self.wire_color = wire_color
-        self._wire_color = wire_color
         self.wire_width = wire_width
         self.wire_hover_color = wire_hover_color
         self.dash = wire_dash
         self.bg = bg
         self.inputcell = None
         self.outputcell = None
         self.clickcount = 0
@@ -25,15 +24,16 @@
         self.operation_num = 0
         self.input_num = 0
         self.compile_num = 0
         self.socket_num = 0
         self.connect_wire = True
         self.line_list = set()
         self.obj_list = set()
-        self.line_ids = []
+        self.line_ids = set()
+        self.node_list = set()
         self.gain_in = 1
         self.gain_out = 1
         self.set_grid_image(grid_image)
         
         if move:
             if sys.platform.startswith("darwin"):
                 self.tag_bind(self.grid, '<ButtonPress-3>', lambda e: self.getpos(e, 1))
@@ -84,14 +84,17 @@
         
         self.all_items = list(self.find_all())
         self.all_items.pop(self.all_items.index(self.grid))
         
         for i in self.all_items:
             self.move(i, event.x-self.xy_set[0], event.y-self.xy_set[1])        
         self.xy_set = (event.x, event.y)
+
+        for i in self.node_list:
+            i.update_sockets()
             
     def do_zoom(self, event, delta=None):
         """ zoom in/out the canvas by changing the coordinates of all canvas items """
         
         self.all_items = list(self.find_all())
         self.all_items.pop(self.all_items.index(self.grid))
 
@@ -102,14 +105,17 @@
             for i in self.all_items:
                 self.scale(i, event.x, event.y, 1.1, 1.1)
             self.gain_in +=1
         else:
             for i in self.all_items:
                 self.scale(i, event.x, event.y, 0.9, 0.9)
             self.gain_out +=1
+
+        for i in self.node_list:
+            i.update_sockets()
             
     def conectcells(self):
         """ connection data for the inputs of any operation node """
         
         if self.IDc == 'input1': self.inputcell.cellinput1 = self.outputcell
         if self.IDc == 'input2': self.inputcell.cellinput2 = self.outputcell
         if self.IDc == 'input3': self.inputcell.cellinput3 = self.outputcell
@@ -139,15 +145,14 @@
         self.line_list = set()
         
     def configure(self, **kwargs):
         """ configure options """
         
         if "wire_color" in kwargs:
             self.wire_color = kwargs.pop("wire_color")
-            self._wire_color = self.wire_color
             for i in self.line_ids:
                 i.configure(wire_color=self.wire_color)
         if "wire_width" in kwargs:
             self.wire_width = kwargs.pop("wire_width")
             for i in self.line_ids:
                 i.configure(wire_width=self.wire_width)
         if "wire_dash" in kwargs:
@@ -188,15 +193,14 @@
         """ load the node tree back to the canvas """
 
         if not os.path.exists(filename):
             raise FileNotFoundError("No such file found: " + str(filename))
   
         self.clear()
         self.connect_wire = False
-        self.wire_color = self.bg  # hides an unwanted glitch
         
         obj_type_dict = {'NodeValue': NodeValue,
                          'NodeOperation': NodeOperation,
                          'NodeCompile': NodeCompile}
         
         with open(filename) as file:
             obj_dict = json.load(file)
@@ -266,10 +270,9 @@
                         j.connect_input(j.line5, 'input5')
                 except AttributeError: None
             for j in comp_nodes:
                 if [self.outputcell.output_.socket_num, j.input_1.socket_num] in line_list:
                     self.clickcount = 1
                     j.connect_input(None)
                     
-        self.configure(wire_color=self._wire_color) # hides an unwanted glitch
         self.connect_wire = True    
- 
+
```

### Comparing `tknodesystem-0.5/tknodesystem/node_menu.py` & `tknodesystem-0.6/tknodesystem/node_menu.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.5/tknodesystem/node_socket.py` & `tknodesystem-0.6/tknodesystem/node_socket.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,14 @@
         self.canvas.tag_bind(self.ID, '<Leave>', self.leave_socket)
         
     def update(self):
         """ update the coordinates of socket """
         try:
             self.cords = self.canvas.coords(self.ID)
             self.center = (self.cords[0]+self.cords[2])/2, (self.cords[1]+self.cords[3])/2
-            self.canvas.after(10, self.update)
         except: None
         
     def enter_socket(self, event):
         if self.hover: self.canvas.itemconfigure(self.ID, fill=self.hover_color)
         if self.hover_message:
             x_pos = self.cords[0]-self.hover_text.winfo_reqwidth()-3
             y_pos = self.center[1]-self.hover_text.winfo_reqheight()/2
@@ -62,15 +61,14 @@
         self.canvas.itemconfigure(self.ID, state="hidden")
         
     def show(self):
         self.canvas.itemconfigure(self.ID, state="normal")
 
     def connect_wire(self):
         """ make a dummy wire """
-  
         if self.live_connection: return
       
         self.x1, self.y1 = self.center
         self.x2, self.y2 = self.center
         self.wire_exist = True
         self.wireID = self.canvas.create_line(self.x1, self.y1, self.x2, self.y2, dash=self.canvas.dash,
                                               width=self.canvas.wire_width, fill=self.canvas.wire_color)
@@ -81,15 +79,14 @@
         if self.canvas.connect_wire: self.mouse_move()
         
     def delete_wire(self):
         """ delete the dummy wire """
         self.canvas.delete(self.wireID)
         self.wire_exist = False
         self.live_connection = False
-        self.canvas.connect_wire = True
         
     def mouse_move(self):
         """ connect the dummy wire with mouse """
         if self.ID not in self.canvas.find_all():
             self.delete_wire()
         self.canvas.connect_wire = False
         if (self.x1, self.y1)!=self.center:
```

### Comparing `tknodesystem-0.5/tknodesystem/node_types.py` & `tknodesystem-0.6/tknodesystem/node_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .node_args import Args
 import warnings
 
 class NodeValue(Node):
     def __init__(self, canvas, width=100, height=50, value=0, border_color='white', text=None, corner_radius=25,
                  border_width=0, fg_color='#37373D', text_color='white', font=("",10), socket_radius=8, socket_hover=True,
                  socket_color="green", socket_hover_color="grey50", highlightcolor='#52d66c', hover=True, justify="center",
-                 click_command=None, side="right", x=0, y=0, num=None):
+                 click_command=None, side="right", x=0, y=0, num=None, fixed=False):
 
         self.text = text
         self.canvas = canvas
         
         self.args = Args.value_args(locals())
         
         if click_command:
@@ -50,15 +50,16 @@
                                   fg_color=socket_color, hover_color=socket_hover_color, border_width=border_width,
                                   border_color=border_color, hover=socket_hover, socket_num=num)
         
         self.allIDs = self.allIDs + [self.output_.ID]
 
         self.bind_all_to_movement()
         self.canvas.tag_bind(self.output_.ID, '<Button-1>', self.connect_output)
-        self.canvas.bind_all("<Delete>", lambda e: self.destroy() if self.signal else None, add="+")
+        if not fixed:
+            self.canvas.bind_all("<Delete>", lambda e: self.destroy() if self.signal else None, add="+")
         self.socket_nums = self.output_.socket_num
         
         for j in range(self.canvas.gain_in):
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 1.1, 1.1)
 
         for j in range(abs(self.canvas.gain_out)):
@@ -136,15 +137,15 @@
         if len(kwargs)>0:
             raise ValueError("This option is not configurable:" + list(kwargs.keys())[0])
 
 class NodeOperation(Node):
     def __init__(self, canvas, width=100, height=None, inputs=2, border_color='white', text=None, justify="center", hover_text=None,
                  socket_radius=8, corner_radius=25, border_width=0, fg_color='#37373D', text_color='white', font=("",10),
                  highlightcolor='#52d66c', hover=True, socket_color="green", socket_hover_color="grey50", x=0, y=0, none_inputs=False,
-                 multiside=False, command=None, output_socket_color="green", click_command=None, socket_hover=True, num=None):
+                 multiside=False, command=None, output_socket_color="green", click_command=None, socket_hover=True, num=None, fixed=False):
 
         self.text = text
         self.canvas = canvas
         self.type = 'NodeOperation'
         self.hover_text = {} if hover_text is None else hover_text
         
         if self.text is None:
@@ -293,15 +294,16 @@
             self.canvas.tag_bind(self.input_5.ID, '<Button-1>', lambda e: self.connect_input(self.line5, 'input5'))
             id_list.append(self.input_5.ID)
             self.socket_nums.append(self.input_5.socket_num)
             
         self.allIDs = self.allIDs + id_list
         self.bind_all_to_movement()
         self.id_list = id_list
-        self.canvas.bind_all("<Delete>", lambda e: self.destroy() if self.signal else None, add="+")
+        if not fixed:
+            self.canvas.bind_all("<Delete>", lambda e: self.destroy() if self.signal else None, add="+")
 
         for i in self.hover_text:
             self.config_socket(**self.hover_text[i])
        
         for j in range(self.canvas.gain_in):
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 1.1, 1.1)
@@ -586,15 +588,15 @@
             except: None
                                   
         if len(kwargs)>0:
             raise ValueError("This option is not configurable:" + list(kwargs.keys())[0])
         
 class NodeCompile(Node):
     def __init__(self, canvas, width=100, height=50, border_color='white', text="Compile", socket_radius=8, corner_radius=25, x=0, y=0, justify="center",
-                 border_width=0, fg_color='#37373D',text_color='white', font=("",10), highlightcolor='#52d66c', hover=True, socket_hover=True,
+                 border_width=0, fg_color='#37373D',text_color='white', font=("",10), highlightcolor='#52d66c', hover=True, socket_hover=True, fixed=False,
                  socket_color="green", socket_hover_color="grey50", show_value=True, command=None, click_command=None, side="left", num=None):
 
         self.canvas = canvas
         self.text = text
         self.type = 'NodeCompile'
         
         if border_width==0:
@@ -648,15 +650,16 @@
                                   border_color=border_color, hover=socket_hover, socket_num=num[1] if num else None)
         self.output_.hide()
         self.socket_nums = [self.input_1.socket_num, self.output_.socket_num]
         self.allIDs = self.allIDs + [self.output_.ID, self.input_1.ID] 
         self.fixed = True
         self.bind_all_to_movement()
         self.canvas.tag_bind(self.input_1.ID, '<Button-1>', self.connect_input)
-        self.canvas.bind_all("<Delete>", lambda e: self.destroy() if self.signal else None, add="+")
+        if not fixed:
+            self.canvas.bind_all("<Delete>", lambda e: self.destroy() if self.signal else None, add="+")
         
         for j in range(self.canvas.gain_in):
             for i in self.allIDs:
                 self.canvas.scale(i, 0, 0, 1.1, 1.1)
 
         for j in range(abs(self.canvas.gain_out)):
             for i in self.allIDs:
```

### Comparing `tknodesystem-0.5/tknodesystem/node_wire.py` & `tknodesystem-0.6/tknodesystem/node_wire.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 
         self.canvas = canvas
         self.firstcell = firstcell # output socket
         self.secondcell = secondcell # input socket
         self.IDc = self.canvas.IDc
         self.wire_color = wire_color
         self.wire_width = wire_width
-        self.canvas.line_ids.append(self)
+        self.canvas.line_ids.add(self)
         self.dash = (2,4) if dash else ()
         self.hover_color = wire_hover_color
-    
+        self.connected = True
+        
         if self.firstcell:
             self.create()
             self.update()
 
     def create(self):
         """ creates the line from output-->input sockets """
         
@@ -59,32 +60,29 @@
         self.firstcell.connect_output(None)
         self.firstcell.output_.live_connection = False
         self.canvas.clickcount = 0
         if self.secondcell.type=="NodeOperation":
             self.secondcell.connect_input(self.ID, input_num)
         else:
             self.secondcell.connect_input(None)
- 
+            
     def update(self):
         """ update the coordinates of line based on the socket position """
-        
         all_items = self.canvas.find_all()
         if self.firstcell.ID not in all_items or self.secondcell.ID not in all_items:
             self.canvas.delete(self.ID)
-            self.canvas.line_ids.remove(self)
-        else:
-            if self.ID not in all_items: return
-            self.x1, self.y1 = self.firstcell.output_.center
-            if self.IDc == 'input1': self.x2, self.y2 = self.secondcell.input_1.center
-            if self.IDc == 'input2': self.x2, self.y2 = self.secondcell.input_2.center
-            if self.IDc == 'input3': self.x2, self.y2 = self.secondcell.input_3.center
-            if self.IDc == 'input4': self.x2, self.y2 = self.secondcell.input_4.center
-            if self.IDc == 'input5': self.x2, self.y2 = self.secondcell.input_5.center
-            self.canvas.coords(self.ID, self.x1, self.y1, self.x2, self.y2)
-            self.canvas.after(10, self.update)
+            self.connected = False
+        if self.ID not in all_items: return
+        self.x1, self.y1 = self.firstcell.output_.center
+        if self.IDc == 'input1': self.x2, self.y2 = self.secondcell.input_1.center
+        if self.IDc == 'input2': self.x2, self.y2 = self.secondcell.input_2.center
+        if self.IDc == 'input3': self.x2, self.y2 = self.secondcell.input_3.center
+        if self.IDc == 'input4': self.x2, self.y2 = self.secondcell.input_4.center
+        if self.IDc == 'input5': self.x2, self.y2 = self.secondcell.input_5.center
+        self.canvas.coords(self.ID, self.x1, self.y1, self.x2, self.y2)
 
     def configure(self, **kwargs):
         if "wire_color" in kwargs:
             self.canvas.itemconfig(self.ID, fill=kwargs.pop("wire_color"))
         if "wire_width" in kwargs:
             self.canvas.itemconfig(self.ID, width=kwargs.pop("wire_width"))
         if "dash" in kwargs:
```

### Comparing `tknodesystem-0.5/tknodesystem.egg-info/PKG-INFO` & `tknodesystem-0.6/tknodesystem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tknodesystem
-Version: 0.5
+Version: 0.6
 Summary: Simple visual node system (DAG) with tkinter!
 Home-page: https://github.com/Akascape/TkNodeSystem
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes,visual-scripting
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tknodesystem-0.5/tknodesystem.egg-info/SOURCES.txt` & `tknodesystem-0.6/tknodesystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

