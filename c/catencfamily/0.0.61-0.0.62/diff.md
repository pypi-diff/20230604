# Comparing `tmp/catencfamily-0.0.61.tar.gz` & `tmp/catencfamily-0.0.62.tar.gz`

## Comparing `catencfamily-0.0.61.tar` & `catencfamily-0.0.62.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.61/src/catencfamily/__init__.py
--rw-r--r--   0        0        0    88962 2020-02-02 00:00:00.000000 catencfamily-0.0.61/src/catencfamily/encoders.py
--rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 catencfamily-0.0.61/src/catencfamily/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.61/LICENSE
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.61/README.md
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.61/pyproject.toml
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.61/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 catencfamily-0.0.62/.pypirc
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 catencfamily-0.0.62/src/catencfamily/__init__.py
+-rw-r--r--   0        0        0    89414 2020-02-02 00:00:00.000000 catencfamily-0.0.62/src/catencfamily/encoders.py
+-rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 catencfamily-0.0.62/src/catencfamily/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 catencfamily-0.0.62/LICENSE
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 catencfamily-0.0.62/README.md
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 catencfamily-0.0.62/pyproject.toml
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 catencfamily-0.0.62/PKG-INFO
```

### Comparing `catencfamily-0.0.61/src/catencfamily/encoders.py` & `catencfamily-0.0.62/src/catencfamily/encoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-# 3rd June, 2023
+# 04th June, 2023
 """
 References:
 Coding standard:
     https://gist.github.com/nateGeorge/5455d2c57fb33c1ae04706f2dc4fee01
     
 Developing sklearn estimators:
     https://scikit-learn.org/stable/developers/develop.html 
     
 Project template:
     https://github.com/scikit-learn-contrib/project-template/    
     
 """
 
-
-
 # 1.0 Libraries
 import pandas as pd
 import numpy as np
 
 
 # 1.01 For networks and centrality measures
 import networkx as nx
@@ -217,15 +215,15 @@
 
         if not isinstance(self.interactingCatCols, list):
             raise ValueError(
                 "Pass interactingCatCols as a list of column names or as an empty list")   
             
         if (self.n_iter > 1 and self.sampsize < 1):
             if not isinstance(y, pd.Series):
-                raise ValueError("Pass y as a pandas.Series") 
+                raise ValueError("When n_iter > 1,'target' must be passed in fit().") 
                 
         if self.pathToStoreProgress is None:
             # Create two folders: 
             path = Path.cwd() / 'allmodels' / 'progress' 
             path.mkdir(parents=True, exist_ok=True)
             self.pathToStoreProgress =  path
         else:
@@ -710,23 +708,23 @@
         Returns
         ------
         Nothing. 
         """
         noOfUniqueValues = train[colToProject].nunique()
         print("No of unique values in ", colToProject, " are: ", noOfUniqueValues)
         model = self._learn(train,colToProject, intermediaryCol)
-        if self.modelsPath is not None:
-            # Store models to disk in a separate folder.
-            #  Folder must alreday exist
-            # storeModel(train,model, pathToStore)
-            # cMeasures: Centrality measures [1,1,1]
-            self._storeModel(model)
-            if (self.cMeasures[6] == 1):
-                self._storeModelComm(model)
-            print("Model saved")
+        #if self.modelsPath is not None:
+        # Store models to disk in a separate folder.
+        #  Folder must alreday exist
+        # storeModel(train,model, pathToStore)
+        # cMeasures: Centrality measures [1,1,1]
+        self._storeModel(model)
+        if (self.cMeasures[6] == 1):
+            self._storeModelComm(model)
+        print("Model saved")
         return    
     
     
    
 
     def _storeModel(self,model):
         """
@@ -829,20 +827,25 @@
             else:
                 ldf = None
     
             if ldf is None:
                 # No need to save anything
                 continue
     
-            # Merge left dataframe with current model
-            #  (i+1) becuase modelName starts with modelName1
-            current_model = "modelName" + str(i+1)
-            filename =  myvar[current_model] + ".pkl"
-            path = Path(self.modelsPath)
-            my_file = path / filename
+            # An arbitrary file that we do not expect to exist
+            my_file = Path(str(np.random.randint(30000,40000)))
+
+            if (self.modelsPath is not None):
+                # Merge left dataframe with current model
+                #  (i+1) becuase modelName starts with modelName1
+                current_model = "modelName" + str(i+1)
+                filename =  myvar[current_model] + ".pkl"
+                path = Path(self.modelsPath)
+                my_file = path / filename
+
             
             # If the model file was earlier saved and it exists
             if my_file.exists():   
                 # Read earlier the saved file
                 saved_file = pd.read_pickle(my_file)
                 # Rename ldf column by adding a random number to column
                 u = np.random.random_integers(10000)  # Generate a random number
@@ -910,18 +913,24 @@
         if model[5] is not None:
             #gr = pd.DataFrame.from_records(np.array(list(model[5].items())), columns=[colToProject,modelName6])
             ae = pd.DataFrame.from_records(np.array(list(model[6].items())), columns=[colToProject,modelName7])
             den = pd.DataFrame.from_records(np.array(list(model[7].items())), columns=[colToProject,modelName8])
             
             for i,j in enumerate((ae,den)):    # Instead of ((gr,ae,den))
                 ldf = j
-                current_model = "modelName" + str(7 + i)
-                filename =  myvar[current_model] + ".pkl"
-                path = Path(self.modelsPath)
-                my_file = path / filename
+                
+                # An arbitrary file that we do not expect to exist
+                my_file = Path(str(np.random.randint(30000,40000)))
+                if (self.modelsPath is not None):
+                    current_model = "modelName" + str(7 + i)
+                    filename =  myvar[current_model] + ".pkl"
+                    path = Path(self.modelsPath)
+                    my_file = path / filename
+                
+                
                 if my_file.exists():   
                         # Read earlier the saved file
                         saved_file = pd.read_pickle(my_file)
                         # Rename ldf column by adding a random number to column
                         u = np.random.random_integers(10000)  # Generate a random number
                         # Rename column of ldf. str(1) below is not needed. May be removed.
                         ldf = ldf.rename(columns = {myvar[current_model]  : (str(u) + "_" + str(1))})
```

### Comparing `catencfamily-0.0.61/src/catencfamily/utils.py` & `catencfamily-0.0.62/src/catencfamily/utils.py`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.61/LICENSE` & `catencfamily-0.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.61/README.md` & `catencfamily-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `catencfamily-0.0.61/pyproject.toml` & `catencfamily-0.0.62/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "catencfamily"
-version = "0.0.61"
+version = "0.0.62"
 authors = [
   { name="Ashok Kumar Harnal", email="ashokharnal@gmail.com" },
 ]
 description = "A class to generate a family of categorical encoders using network analysis"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `catencfamily-0.0.61/PKG-INFO` & `catencfamily-0.0.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catencfamily
-Version: 0.0.61
+Version: 0.0.62
 Summary: A class to generate a family of categorical encoders using network analysis
 Project-URL: Homepage, https://github.com/harnalashok/CatEncodersFamily
 Author-email: Ashok Kumar Harnal <ashokharnal@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

