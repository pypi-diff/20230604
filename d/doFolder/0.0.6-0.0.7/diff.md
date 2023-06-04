# Comparing `tmp/doFolder-0.0.6.tar.gz` & `tmp/doFolder-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doFolder-0.0.6.tar", last modified: Wed May 31 15:06:30 2023, max compression
+gzip compressed data, was "doFolder-0.0.7.tar", last modified: Sun Jun  4 18:50:58 2023, max compression
```

## Comparing `doFolder-0.0.6.tar` & `doFolder-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-31 15:06:30.497152 doFolder-0.0.6/
--rw-rw-rw-   0        0        0     3349 2023-05-31 15:06:30.497152 doFolder-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2624 2023-05-30 18:05:13.000000 doFolder-0.0.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-31 15:06:30.487153 doFolder-0.0.6/doFolder/
--rw-rw-rw-   0        0        0      569 2023-05-31 14:24:09.000000 doFolder-0.0.6/doFolder/__init__.py
--rw-rw-rw-   0        0        0    10823 2023-05-31 14:59:56.000000 doFolder-0.0.6/doFolder/compare.py
--rw-rw-rw-   0        0        0    21399 2023-05-31 15:02:01.000000 doFolder-0.0.6/doFolder/main.py
--rw-rw-rw-   0        0        0    13847 2023-05-31 14:13:25.000000 doFolder-0.0.6/doFolder/terminal.py
-drwxrwxrwx   0        0        0        0 2023-05-31 15:06:30.495152 doFolder-0.0.6/doFolder.egg-info/
--rw-rw-rw-   0        0        0     3349 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-31 15:06:30.000000 doFolder-0.0.6/doFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-31 15:06:30.498154 doFolder-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1196 2023-05-31 14:57:13.000000 doFolder-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:50:58.707246 doFolder-0.0.7/
+-rw-rw-rw-   0        0        0     3351 2023-06-04 18:50:58.707246 doFolder-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2624 2023-05-30 18:05:13.000000 doFolder-0.0.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-04 18:50:58.698248 doFolder-0.0.7/doFolder/
+-rw-rw-rw-   0        0        0      569 2023-05-31 14:24:09.000000 doFolder-0.0.7/doFolder/__init__.py
+-rw-rw-rw-   0        0        0    10823 2023-05-31 14:59:56.000000 doFolder-0.0.7/doFolder/compare.py
+-rw-rw-rw-   0        0        0    28190 2023-06-04 18:48:56.000000 doFolder-0.0.7/doFolder/main.py
+-rw-rw-rw-   0        0        0    13847 2023-05-31 14:13:25.000000 doFolder-0.0.7/doFolder/terminal.py
+drwxrwxrwx   0        0        0        0 2023-06-04 18:50:58.706247 doFolder-0.0.7/doFolder.egg-info/
+-rw-rw-rw-   0        0        0     3351 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-04 18:50:58.000000 doFolder-0.0.7/doFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 18:50:58.708245 doFolder-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-06-04 18:50:47.000000 doFolder-0.0.7/setup.py
```

### Comparing `doFolder-0.0.6/PKG-INFO` & `doFolder-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.6
-Summary: download files quickly
+Version: 0.0.7
+Summary: Manage files more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
 Platform: linux
```

### Comparing `doFolder-0.0.6/README.rst` & `doFolder-0.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.6/doFolder/__init__.py` & `doFolder-0.0.7/doFolder/__init__.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.6/doFolder/compare.py` & `doFolder-0.0.7/doFolder/compare.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.6/doFolder/main.py` & `doFolder-0.0.7/doFolder/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from concurrent.futures import ThreadPoolExecutor
 
 __all__=["File","Folder","Path"]
 
 pathTester=re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)/(?:[^/\\\*\?]+/?)*$")
 driverFinder=re.compile(r"^((?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+))/(?:[^/\\\*\?]+/?)*$")
 pathFinder=re.compile(r"^(?:(?:[a-zA-Z]:)?|//[^/\\\*\?]+)(/(?:[^/\\\*\?]+/?)*)$")
-SearchCondition=Union[str,re.Pattern[str],Callable[[Union["File","Folder"]],bool]]
+SearchCondition=Union[str,re.Pattern,Callable[[Union["File","Folder"]],bool]]
 FormatedMatching=Tuple[Callable[[Union["File","Folder"]],bool],int,Union[int,None]]
 UnformattedMatching=Union[SearchCondition,Tuple[SearchCondition,int,Union[int,None]]]
 _T=TypeVar("_T",bound="_HasName")
 _U=TypeVar("_U")
 class _HasName(Generic[_T]):
     name: str
 
@@ -95,15 +95,15 @@
         return f"<{self.__class__.__name__} {self.values}>"
     def append(self,var:_T):
         self.values.append(var)
     def __len__(self):
         return len(self.values)
     def __add__(self,var:"_ObjectListIndexedByName"):
         return _ObjectListIndexedByName(self.values+var.values)
-    def __contains__(self,var:_T|str)->bool:
+    def __contains__(self,var:Union[_T,str])->bool:
         if var in self.values :
             return True
         for i in range(len(self.values)):
             if  self.values[i].name == var:
                 return True
         return False
     def __getitem__(self,key:Union[int,str])->Union[_T,None]:
@@ -138,17 +138,27 @@
     def __add__(self,var:"FileList"):
         return FileList(self.values+var.values)
 class FolderList(_ObjectListIndexedByName["Folder"]):
     def __init__(self,var:Iterable["Folder"]=[]):
         super().__init__(var)
     def __add__(self,var:"FolderList"):
         return FolderList(self.values+var.values)
-
 class Path(str):
-    """Means a path. it can be used as same as a str, but it has more function about path"""
+    """
+    ## Represents a path. It can be used as same as a str, but it has more function about path.
+    Attributes:
+        - driver (str): The drive letter of the path.
+        - path (str): The directory and file name of the path.
+    ## Methods:
+        - partition() -> List[str]: Split the path into list.
+        - name() -> str: Return the name of the file or folder that this path points to.
+        - add(value:str) -> "Path": Add another dir name after the current path and return a new Path object.
+        - adds(value:List[str]) -> "Path": Add multiple dir names after the current path and return a new Path object.
+        - findRest(other:"Path",error:Literal["strict","ignore"]="strict"): Find the same ancestor node between two paths. If error is set to "strict" (default), raise ValueError if other is not exactly parent directory of self. Otherwise, return remaining directories in self's partition after finding different ancestor with other's partition.
+    """
     def __new__(cls, value):
         var=str(value)
         if var.startswith("."):
             var=os.path.abspath(var)
         var=var.replace("\\","/")
         if pathTester.match(var)==None:
             raise ValueError(f"\"{var}\" does not appear to be a legal path")
@@ -190,15 +200,47 @@
                 if error=="strict":
                     raise ValueError(f"\"{other}\" is not the ancestor folder of {self}")
                 return retsult
             del retsult[0]
         return retsult
     
 class File(_HasName):
-    """Means a file on disk"""
+    """
+    Represents a file on disk.
+    ## Attributes:
+        - path (Path): The path of the file.
+        - parent (Folder or None): The parent folder of the file.
+        - mode (int): The mode of the file.
+        - ino (int): The inode number of the file.
+        - dev (int): The device identifier of the filesystem containing this file.
+        - uid (int): The user ID of the owner of this file.
+        - gid (int): The group ID of the owner of this file.
+        - size(int) :The size, in bytes,of this file
+        - mtime(float) :The time when content was last modified expressed as seconds since epoch
+        - atime(float) :The time when content was last accessed expressed as seconds since epoch
+        - content(bytes) :The contents read from and written to files.
+        - md5(str),sha1(str),sha256(str),sha512(str)：Hashes for verifying data integrity.
+    ## Methods:
+        -__init__(self,path:Union[str,Path],parent:Union["Folder",None]=None)
+        Initializes a new instance with specified path and optional parent folder.
+        - refresh(self)
+        Rebuilds all attributes based on current state on disk.
+        - open(self,*args,**kw)->IO
+        Opens and returns a handle to underlying OS-level representation using built-in open function.
+        - remove(self)
+        Deletes underlying OS-level representation using os.remove() method.
+        - copy(self,path:str)
+        Copies underlying OS-level representation to specified destination using shutil.copy() method.
+        - move(self,path:str)
+        Moves underlying OS-level representation to specified destination using shutil.move() method.
+        - __str__(self)->str
+        Returns string representation "<File \"{name}\">".
+        - __repr__(self)->str
+        Returns string representation "<File \"{name}\">".
+    """
     def __init__(self,path:Union[str,Path],parent:Union["Folder",None]=None):
         if type(path)!=Path:
             path=Path(path)
         self.path = path
         self.parent = parent
         self.refresh()
     def refresh(self):
@@ -265,15 +307,58 @@
     def remove(self):
         os.remove(self.path)
     def copy(self,path:str):
         shutil.copy(self.path,path)
     def move(self,path:str):
         shutil.move(self.path,path)
 class Folder(_HasName):
-    """Means a folder on disk"""
+    """
+    Represents a folder on disk.
+    ## Attributes:
+        - path (Union[str,Path]): The path of the folder.
+        - onlisten (bool): Whether to listen for changes in the folder.
+        - parent (Union["Folder",None]): The parent folder of this folder. None if it is a root directory.
+        - scaned (bool): Whether the contents of this folder have been scanned and stored in memory.
+        - scan(bool): Whether to automatically scan and store all contents when initializing or refreshing this object.
+    ## Methods:
+        - __init__(self,path:Union[str,Path],onlisten:bool=False,parent:Union["Folder",None]=None,scan:bool=False)
+        Initializes a new instance of the Folder class with specified parameters.
+        - refresh(self)
+        Rebuilds all information about files and subfolders contained within this Folder object.
+        - __str__(self)->str
+        Returns string representation of current object
+        - __repr__(self) -> str
+        Returns string representation that can be used to recreate an equivalent instance using eval() function
+        - __contains__(self,item:Union[str,"Folder","File"]) -> bool
+        Determines whether item exists within current directory or not
+        - __getitem__(self,key)->Union["File","Folder",None]
+        Gets file/folder by name from current directory
+        - forEach(self,callback:Callable[[Union["File","Folder"]],Any],rootPosition:Literal["first","last"]="first")->None
+        Goes through each element in current directory calling callback function for each one.
+        - forEachFile(self,callback:Callable[[File],Any])->None
+        Goes through each file in current directory calling callback function for each one.
+        - forEachFolder(self,callback:Callable[["Folder"],Any],rootPosition:Literal["first","last"]="first")->None:
+        Goes through each subfolder in current directory calling callback function for each one.
+        - remove(self)->None
+        Removes current folder and all its contents
+        - move(self,path:str)->None
+        Moves current folder to specified path
+        - copy(self,path:str)->None:
+        Copies current folder to specified path
+        - hasSubfolder(self,name:str,recursive:bool=False)->bool:
+        Determines whether a subfolder with the given name exists within this Folder object or not.
+        - hasFile(self,name:str,recursive:bool=False)->bool:
+        Determines whether a file with the given name exists within this Folder object or not.
+        - search(self,condition:List[UnformattedMatching],aim:Literal["file","folder","both"]="both",threaded:bool=False,threads:Union[None,int]=None)
+        Searches for files/folders in the current directory that match certain criteria.
+        - createFile(self,path:Union[str,Path],content:bytes=b"")->Path
+        Creates a new file at the specified location with optional content.
+        - createFolder(self,path:Union[str,Path])->Path
+        Creates a new sub-folder at the specified location.
+    """
     def __init__(self,path:Union[str,Path],onlisten:bool=False,parent:Union["Folder",None]=None,scan:bool=False):
         if type(path)!=Path:
             path=Path(path)
         self.onlisten=onlisten
         self.path=path
         self.parent=parent
         self.scaned=scan
@@ -380,15 +465,15 @@
             callback(item)
         for item in self.subfolder:
             item.forEachFile(callback)
     def forEachFolder(self,callback:Callable[["Folder"],Any],rootPosition:Literal["first","last"]="first")->None:
         """
         Go through each of these folder
         :param callback:The function to call
-        :rootPosition:Is the root before or after the child element
+        :param rootPosition:Is the root before or after the child element
         """
         if  rootPosition=="first":
             callback(self)
         for item in self.subfolder:
             item.forEachFolder(callback,rootPosition)
         if rootPosition=="last":
             callback(self)
@@ -476,24 +561,39 @@
                         break
                     k+=1
                 if (k==len(restCondition)):
                     retsult.append(j)
             if condition[i][1]>0:
                 break
     def createFile(self,path:Union[str,Path],content:bytes=b"")->Path:
+        """
+        Create a new file at the specified path with the given content.
+        :param path: The path where the file will be created. Can be either a string or a Path object.
+        :param content: The bytes to write into the newly created file. Default is an empty byte string.
+        :return: A Path object representing the newly created file.
+        :raise FileOrFolderAlreadyExists: If there is already a file or folder at the specified path.
+        """
         path=Path(os.path.join(self.path, path))
         if os.path.exists(path):
             raise FileOrFolderAlreadyExists(f"Can't create file {path} because it already exists")
         with open(path,"wb") as f:
             f.write(content)
         return path
     def createFolder(self,path:Union[str,Path],content:bytes=b"")->Path:
+        """
+        Create a new folder at the specified path.
+        :param path: The path where the new folder will be created. Can be either a string or a Path object.
+        :param content: Optional parameter specifying the initial content of the folder. Default is an empty bytes object.
+        :return: Returns a Path object representing the newly created folder.
+        :raise FileOrFolderAlreadyExists: If there is already a file or folder with the same name as `path`.
+        """
         path=Path(os.path.join(self.path, path))
         if os.path.exists(path):
             raise FileOrFolderAlreadyExists(f"Can't create folder {path} because it already exists")
         os.makedirs(path)
         return path
     def add(self,aim:Union["File","Folder"],move:bool=False):
+        "add a file or folder to this folder"
         if move:
             aim.move(self.path)
         else:
             aim.copy(self.path)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `doFolder-0.0.6/doFolder/terminal.py` & `doFolder-0.0.7/doFolder/terminal.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.0.6/doFolder.egg-info/PKG-INFO` & `doFolder-0.0.7/doFolder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.0.6
-Summary: download files quickly
+Version: 0.0.7
+Summary: Manage files more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
 Platform: linux
```

### Comparing `doFolder-0.0.6/setup.py` & `doFolder-0.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'doFolder',
-    version = '0.0.6',
+    version = '0.0.7',
     keywords = ['file',"foler","path","filesystem"],
-    description = 'download files quickly',
+    description = 'Manage files more easily',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
         'watchdog',
         "rich",
```

