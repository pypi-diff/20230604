# Comparing `tmp/SimpleShape-1.1-py3-none-any.whl.zip` & `tmp/SimpleShape-1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7381 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      605 b- defN 23-Jun-03 15:03 SimpleShape/Example.py
--rw-rw-rw-  2.0 fat    11766 b- defN 23-Jun-04 11:10 SimpleShape/Shapes.py
+Zip file size: 7568 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      778 b- defN 23-Jun-04 16:46 SimpleShape/Example.py
+-rw-rw-rw-  2.0 fat    12771 b- defN 23-Jun-04 16:41 SimpleShape/SimpleShape.py
 -rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-03 17:34 SimpleShape/__init__.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-Jun-04 11:20 SimpleShape-1.1.dist-info/License.txt
--rw-rw-rw-  2.0 fat     4461 b- defN 23-Jun-04 11:20 SimpleShape-1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 11:20 SimpleShape-1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-04 11:20 SimpleShape-1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      634 b- defN 23-Jun-04 11:20 SimpleShape-1.1.dist-info/RECORD
-8 files, 18641 bytes uncompressed, 6273 bytes compressed:  66.3%
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-Jun-04 16:57 SimpleShape-1.2.dist-info/License.txt
+-rw-rw-rw-  2.0 fat     4461 b- defN 23-Jun-04 16:57 SimpleShape-1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-04 16:57 SimpleShape-1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-04 16:57 SimpleShape-1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      639 b- defN 23-Jun-04 16:57 SimpleShape-1.2.dist-info/RECORD
+8 files, 19824 bytes uncompressed, 6450 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: SimpleShape/Example.py
 Comment: 
 
-Filename: SimpleShape/Shapes.py
+Filename: SimpleShape/SimpleShape.py
 Comment: 
 
 Filename: SimpleShape/__init__.py
 Comment: 
 
-Filename: SimpleShape-1.1.dist-info/License.txt
+Filename: SimpleShape-1.2.dist-info/License.txt
 Comment: 
 
-Filename: SimpleShape-1.1.dist-info/METADATA
+Filename: SimpleShape-1.2.dist-info/METADATA
 Comment: 
 
-Filename: SimpleShape-1.1.dist-info/WHEEL
+Filename: SimpleShape-1.2.dist-info/WHEEL
 Comment: 
 
-Filename: SimpleShape-1.1.dist-info/top_level.txt
+Filename: SimpleShape-1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: SimpleShape-1.1.dist-info/RECORD
+Filename: SimpleShape-1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SimpleShape/Example.py

```diff
@@ -1,24 +1,26 @@
 """
 Example document to provide quick overwiev on how to use this package
 """
 
 # Import the Main file
-import Shapes as sh
+import SimpleShape as sh
 
 # a) Create a Triangle and perform simple operations
 
 My_triangle = sh.Triangle([[1,1],[3,1],[4,3]])
 print(My_triangle)
 print("Perimeter of this triangle is " + str(My_triangle.perimeter()))
+print("Area of this triangle is " + str(My_triangle.area()))
 
 # b) Check if two circles intersect
 
 Circle_1 = sh.Circle(2) # Circle with radius of 2 and center at (0,0)
 Circle_2 = sh.Circle(3,(3,0.2)) # Circle with radious of 3 and center at (3,0.2)
 
-print(Circle_1.intersect(Circle_2))
+print("Do circles intersect: " + str((Circle_1.intersect(Circle_2))))
 
 
+# c) Create a random ellipse and visualize it
 
-# Additional: Use provided functions
-
+My_Ellipse = sh.random_shape("Ellipse")
+My_Ellipse.visualize()
```

## Comparing `SimpleShape/Shapes.py` & `SimpleShape/SimpleShape.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 """
 
 import json
 from math import pi, sqrt, sin, cos
 from matplotlib import pyplot as plt
 from matplotlib.patches import Ellipse as _Ellipse
 import numpy as np
-import warnings
-
 
 class Geometry:
     """Parent class for creating geometric objects"""
     
     def __init__(self, coordinates):
         """Initialization of the object. Somewhat different for
         circle and ellipse"""
@@ -23,24 +21,24 @@
         return ("The coordinates of the " + self.__class__.__name__ + " are " + 
         str(self.coordinates))
 
     def perimeter(self) -> float:
         """Perimeter (circumference) of object"""
         s = 0
         for i in range(len(self.coordinates)):
-            s += sqrt((self.coordinates[i-1][0] - self.coordinates[i][0])**2 +
-                      (self.coordinates[i-1][1] - self.coordinates[i][1])**2)
+            s += sqrt((self.coordinates[i][0] - self.coordinates[i-1][0])**2 +
+                      (self.coordinates[i][1] - self.coordinates[i-1][1])**2)
         return s
     
     def area(self) -> float:
         """Area of object using Shoelace formula"""
         s = 0
         for i in range(len(self.coordinates)):             
             s += (self.coordinates[i-1][0] * self.coordinates[i][1] -
-                  self.coordinates[i][1] * self.coordinates[i-1][1])
+                  self.coordinates[i][0] * self.coordinates[i-1][1])
         return abs(s/2)
 
     def to_json(self) -> json:
         """Convert the object to .json format"""
         if self.__class__.__name__ in ('Triangle', 'Rectangle', 'Polygon'):
             return {
                 'type': self.__class__.__name__,
@@ -58,71 +56,51 @@
                 'a': self.a,
                 'b': self.b,
                 'f': self.f,
                 'center':self.center
             }
         else:
             raise Warning('Invalid JSON data. Try something else')
-
-    def from_json(cls, json_data) -> object:
-        """Create a geometric object from JSON data."""
-        
-        if json_data['type'] in ('Triangle', 'Rectangle', 'Polygon'):
-            return Rectangle(json_data['coordinates'])
-        elif json_data['type'] == 'Circle':
-            return Circle(json_data['r'], json_data['center'])
-        elif json_data['type'] == 'Ellipse':
-            return Ellipse(json_data['a'],json_data['b'],
-                           json_data['f'], json_data['center'])
-        else:
-            raise Warning('Invalid JSON data. Try something else')
-            
-    def save_shapes(shapes, filename):
-        """Save json_data to file"""
-        json_data = [element.to_json() for element in shapes]
-        with open(filename, 'w') as file:
-            json.dump(json_data, file)
-
-    def load_shapes(filename):
-        """Load json_data from file"""
-        with open(filename, 'r') as file:
-            json_data = json.load(file)
-            shapes = [Geometry.from_json(data) for data in json_data]
-            return shapes 
             
     
     def intersect(self, other) -> bool:
         if self.__class__.__name__ in ('Triangle','Rectangle','Polygon'):
             if isinstance(other, (Triangle or Rectangle or Polygon)):
-                for i in range(-1,len(self.coordinates)-1):
-                    for j in range(-1,len(other.coordinates)-1):
+                for i in range(len(self.coordinates)):
+                    for j in range(len(other.coordinates)):
                         if intersect(self.coordinates[i-1],self.coordinates[i],
                                      other.coordinates[j-1],other.coordinates[j]):
                             return True
                 return False
             elif isinstance(other, Circle):
-                for i in range(-1,len(self.coordinates)-1):
-                    if Line_Intersect_Circle(other.center, other.r, self.p1, self.p2):
+                for i in range(len(self.coordinates)):
+                    if Line_Intersect_Circle(self.coordinates[i-1], 
+                                             self.coordinates[i], 
+                                             other.center, other.r):
                         return True
                 return False
             
             elif isinstance(other, Ellipse):
                 return "This feature has yet to be implemented"
             else:
                 raise ValueError("Invalid shape type for intersection check")
             
         
        
         elif self.__class__.__name__ == ('Circle'):
             if isinstance(other, Circle):
-                return sqrt((self.center[0]-other.center[0])**2+
-                            (self.center[1]-other.center[1])**2) < (self.r+other.r)
+                distance = sqrt((self.center[0]-other.center[0])**2+
+                            (self.center[1]-other.center[1])**2)
+                if distance > abs(self.r - other.r): 
+                    return distance < (self.r + other.r)
             elif isinstance(other, (Triangle or Rectangle or Polygon)):
-                for i in range(-1,len(other.coordinates)-1):
-                    if Line_Intersect_Circle(self.center, self.r, other.p1, other.p2):
+                for i in range(len(other.coordinates)):
+                    if Line_Intersect_Circle(other.coordinates[i-1], 
+                                             other.coordinates[i], 
+                                             self.center, self.r):
                         return True
                 return False
             elif isinstance(other, Ellipse):
                 return "This feature has yet to be implemented"
             else:
                 raise ValueError("Invalid shape type for intersection check")
 
@@ -134,36 +112,68 @@
             
     
     def visualize(self) -> None:
         
         X = np.array(self.coordinates)
         plt.figure()
         plt.scatter(X[:, 0], X[:, 1], s = 20)
-        t1 = plt.Polygon(X[:3,:])
+        t1 = plt.Polygon(X[:,:])
         plt.gca().add_patch(t1)
+            
+# Functions for working with json data
+
+def from_json(json_data) -> object:
+    """Create a geometric object from JSON data."""
+    
+    if json_data['type'] == 'Triangle':
+        return Triangle(json_data['coordinates'])
+    elif json_data['type'] == 'Rectangle':
+        return Rectangle(json_data['coordinates'])
+    elif json_data['type'] == 'Polygon':
+        return Polygon(json_data['coordinates'])
+    elif json_data['type'] == 'Circle':
+        return Circle(json_data['r'], json_data['center'])
+    elif json_data['type'] == 'Ellipse':
+        return Ellipse(json_data['a'],json_data['b'],
+                       json_data['f'], json_data['center'])
+    else:
+        raise Warning('Invalid JSON data. Try something else')
         
-        pass
+def save_shapes(shapes, filename):
+    """Save json_data to file"""
+    json_object = json.dumps(shapes)
+    with open(filename, 'a') as outfile:
+        outfile.write(json_object)
+
+def load_shapes(filename):
+    """Load json_data from file"""
+    with open(filename, 'r') as file:
+        json_data = json.load(file)
+        return json_data 
 
 
 # Basic shapes (rectangle, Triangle, circle, elipsoid, point, line)
 
 class Triangle(Geometry):
     
     def __init__(self, coordinates):
         super().__init__(coordinates)
 
         self.a = coordinates[0][:2]
         self.b = coordinates[1][:2]
         self.c = coordinates[2][:2]
         
         if (2 > len(self.a) or 2 > len(self.b) or 2 > len(self.c)):
-            return warnings.warn("Provide a 3x2 array or tuple")
+            raise Warning("Provide a 3x2 array or tuple")
         
         if parallel(self.a,self.b,self.b,self.c):
-            return warnings.warn("Not a triangle. Try again")
+            raise Warning("Not a triangle. Try again")
+            
+        if (self.a == self.b or self.a == self.c or self.b == self.c):
+            raise Warning("Not a triangle. Try again")
 
     
     
 class Rectangle(Geometry):
     """Coordinates inserted as 4x2 tuple or array in the following order:
         lower left, lower right, upper right, upper left"""
         
@@ -171,46 +181,57 @@
         super().__init__(coordinates)
         self.a = coordinates[0][:2]
         self.b = coordinates[1][:2]
         self.c = coordinates[2][:2]
         self.d = coordinates[3][:2]
         
         if (2 > len(self.a) or 2 > len(self.b) or 2 > len(self.c) or 2 > len(self.d)):
-            raise Exception("Provide a 4x2 array or tuple")
+            raise Warning("Provide a 4x2 array or tuple")
         if not (parallel(self.a,self.b,self.c,self.d) and parallel(self.b,self.c,self.a,self.d)):
             raise Warning('Not a rectangle. Try something else')
             
 class Polygon(Geometry):
     """Three or more-dimensional geometric shape. Insert coordinates in
     specific order"""
     def __init__(self, coordinates):
         super().__init__(coordinates)
-
+        
+        # Check if polygon is self intersectiong
+        self.is_intersected = 0
+        for i in range(len(self.coordinates)):
+            if self.is_intersected == 1: break
+            for j in range(i):       
+                if intersect(self.coordinates[i-1],self.coordinates[i],
+                         self.coordinates[j-1],self.coordinates[j]):
+                            self.is_intersected = 1
+                            print(""""This Polygon is not a simple polygon. Therefore, the calculated perimeter and area will not be correct""")
+                            break
+                            
 
 class Circle(Geometry):
     
     def __init__(self, r, center = (0,0)):
         self.r = r
         self.center = center
         
-        if r <= 0: return warnings.warn("Radius is less than equal than 0. Use another radius")
+        if r <= 0: raise Warning("Radius is 0 or less. Use another radius")
     
     def __str__(self):
         return ("Circle with radius " + str(self.r) + " and center in " +
                 str(self.center)) 
 
     def area(self):
         return pi * self.r**2
 
     def perimeter(self):
         return 2 * pi * self.r
            
            
     def visualize(self):
-        circle=plt.Circle(self.center, self.r, color='r')
+        circle=plt.Circle(self.center, self.r)
         fig, ax = plt.subplots()
         ax.set_xlim(((self.center[0]-self.r)*1.1, (self.center[0]+self.r)*1.1))
         ax.set_ylim(((self.center[1]-self.r)*1.1, (self.center[1]+self.r)*1.1))
         ax.add_patch(circle)
         
     
 class Ellipse(Geometry):
@@ -260,33 +281,24 @@
         _max = max(a,b)[0]
         f = 2*pi*np.random.uniform(0,1) # Radians
         P1,P2,P3,P4 = [_min,_min],[_max,_min],[_max,_max],[_min,_max]
         P2,P3,P4 = rotate(P2,P1,f), rotate(P3,P1,f), rotate(P4,P1,f)
         return Rectangle([P1,P2,P3,P4])
     elif shape =="Polygon":
         num = np.random.randint(3,100)	
-        cord = []
-        """for i in range(num):
-            while 1<2:
-                a,b = np.random.uniform(-1000, 1000)
-                check intersect
-                if not intersect:
-                    cord.append([a,b])
-                    continue"""
-         
-        return Polygon(cord)
+        return Polygon(np.random.uniform(-1000, 1000, (num,2)))
     elif shape =="Circle":
-        r = np.random.uniform(0,1000)
+        r = np.random.uniform(0.1,1000)
         [x, y] = np.random.uniform(-1000,1000, (2,1))
-        return Circle(r,(x,y))
+        return Circle(r,(x[0],y[0]))
     elif shape =="Ellipse":
-        [a, b] = np.random.uniform(0,1000, (2,1))
+        [a, b] = np.random.uniform(0.1,1000, (2,1))
         [x, y] = np.random.uniform(-1000,1000, (2,1))
         f = 360*np.random.uniform(0,1)
-        return Ellipse(a, b, f, (x,y))
+        return Ellipse(a[0], b[0], f, (x[0],y[0]))
     else:
         raise ValueError("Invalid shape type for creating random shape")
 
 # Rotate P1 around P2 for angle f in radians        
 # https://stackoverflow.com/questions/4465931/rotate-rectangle-around-a-point
 
 def rotate(P1, P2, f):
@@ -296,16 +308,18 @@
     return [x,y]
 
 
 
 # (https://bryceboe.com/2006/10/23/line-segment-intersection-algorithm/)
 
 def intersect(A,B,C,D):
-    def ccw():
-        return (C.y-A.y)*(B.x-A.x) > (B.y-A.y)*(C.x-A.x)
+    def ccw(A,B,C):
+        return (C[1]-A[1])*(B[0]-A[0]) > (B[1]-A[1])*(C[0]-A[0])
+    if ((A[0] == C[0] and A[1] == C[1]) or (A[0] == D[0] and A[1] == D[1])): return False 
+    if ((B[0] == C[0] and B[1] == C[1]) or (B[0] == D[0] and B[1] == D[1])): return False 
     return ccw(A,C,D) != ccw(B,C,D) and ccw(A,B,C) != ccw(A,B,D)
 
 def parallel(A,B,C,D):
     if B[0] == A[0]: return (True if C[0] == D[0] else False)
     return abs((B[1]-A[1])/(B[0]-A[0])) == abs((D[1]-C[1])/(D[0]-C[0]))
 
 # Taken and modified from 
@@ -322,11 +336,11 @@
     t = Dx * (c[0] - A[0]) + Dy * (c[1] - A[1])    
     
     Ex = t*Dx+A[0]
     Ey = t*Dy+A[1]
     
     LEC = sqrt((Ex-c[0])**2+(Ey-c[0])**2)
     
-    if LEC <= r: return True
+    if LEC < r: return True
 
     return False
```

## Comparing `SimpleShape-1.1.dist-info/License.txt` & `SimpleShape-1.2.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `SimpleShape-1.1.dist-info/METADATA` & `SimpleShape-1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimpleShape
-Version: 1.1
+Version: 1.2
 Summary: A simple package for creating geometric objects and 
 Author: Tilen Žel
 Author-email: tilen.zel@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `SimpleShape-1.1.dist-info/RECORD` & `SimpleShape-1.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-SimpleShape/Example.py,sha256=e4m_Ksl_MpstbEYL0cukOvkI4A7q-pVo1xNgu62aOCI,605
-SimpleShape/Shapes.py,sha256=yGw0pZTdekWrGcsQYvzwRH5QYGmRzlxBNEhHxqwF4Co,11766
+SimpleShape/Example.py,sha256=E34CeiDaSmzME8Q9_Ro2BbBnCT5hgju7qU2_0PJtai0,778
+SimpleShape/SimpleShape.py,sha256=tyCZ33pij1LML8aS1clnOn9SgpzDR93moqJme67pLk8,12771
 SimpleShape/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-SimpleShape-1.1.dist-info/License.txt,sha256=IGJ5mUVixjGk4M2mTg2V_vhKdU7lMgT6rXlpnCINLuQ,1069
-SimpleShape-1.1.dist-info/METADATA,sha256=4vjlnb2-Eas99HML-ls1GDCfcygtMdOg9sXxkhuNpF8,4461
-SimpleShape-1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-SimpleShape-1.1.dist-info/top_level.txt,sha256=mabMVIpELH6FHY55TYf97gGoDkEKP-B4xVbEniMTV0A,12
-SimpleShape-1.1.dist-info/RECORD,,
+SimpleShape-1.2.dist-info/License.txt,sha256=IGJ5mUVixjGk4M2mTg2V_vhKdU7lMgT6rXlpnCINLuQ,1069
+SimpleShape-1.2.dist-info/METADATA,sha256=ueJIRy3vmlZ3k-PbESya6GO-SGRhxMWxV0ZE4R3BO8Y,4461
+SimpleShape-1.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+SimpleShape-1.2.dist-info/top_level.txt,sha256=mabMVIpELH6FHY55TYf97gGoDkEKP-B4xVbEniMTV0A,12
+SimpleShape-1.2.dist-info/RECORD,,
```

