# Comparing `tmp/coffeefetch-1.1.0.tar.gz` & `tmp/coffeefetch-1.2.1.tar.gz`

## Comparing `coffeefetch-1.1.0.tar` & `coffeefetch-1.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/requirements.txt
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/src/coffeefetch/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/src/coffeefetch/__main__.py
--rw-r--r--   0        0        0     6316 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/src/coffeefetch/coffeefetch.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/src/coffeefetch/quotes/quotes.txt
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/LICENCE
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/README.md
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 coffeefetch-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/requirements.txt
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/src/coffeefetch/__init__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/src/coffeefetch/__main__.py
+-rw-r--r--   0        0        0     5920 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/src/coffeefetch/fetch.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/src/coffeefetch/quotes/quotes.txt
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/LICENCE
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/README.md
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 coffeefetch-1.2.1/PKG-INFO
```

### Comparing `coffeefetch-1.1.0/src/coffeefetch/__init__.py` & `coffeefetch-1.2.1/src/coffeefetch/fetch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # TTY system information grabber, written in Python
 # Built to run on Unix-like systems, but may function on other systems
-# Written and tested by Logan Allen, 2023, quotes written at http://www.yaldex.com/
+# Written and tested by Logan Allen, 2023
 # PLEASE REPORT ANY ISSUES TO THE GITHUB REPOSITORY!!! www.github.com/TeaPixl
 from socket import gethostname, gethostbyname
 from platform import machine, system, processor, release
 from datetime import datetime
 import psutil
 import logging
 import sys
@@ -27,15 +27,14 @@
                                   ██                ██  ██                              
                                   ██                ██████                              
                                     ██            ██                                    
                                 ████████████████████████                                
                                 ██                    ██                                
                                   ████████████████████"""
 
-# randomly pick from a list of random quotes
 def quoteGen():
     try:
          path = os.path.dirname(__file__)
          realPath = "quotes/quotes.txt"
          location = os.path.join(path, realPath)
          with open(location, 'r') as f:
              quotes = [] # all quotes in list, randomly pick 1 out of 20
@@ -44,104 +43,103 @@
              chosen = random.choice(text)
              print("\n                             " + chosen)
     except Exception as e:
         logging.exception(e)
         print("\nQuoteGen failed... Proceeding.")
         pass
 
-def spinningCursor(): # shows the script is running, dosent actually mean anything :/
+def spinningCursor():
     try:
         while True:
             for cursor in "|/-\\":
                 yield cursor
     except Exception as e:
         logging.exception(e)
         print("spinningCursor failed... Proceeding.")
 
-def currentUser(): #current user logged in
+def currentUser(): #current user
     user = getpass.getuser()
     print("Hello, " + user)
     
 def getTime():
     try:
         now = datetime.now()
         current_time = now.strftime("%H:%M:%S")
         print("It is: "+ current_time)
     except Exception as e:
         logging.exception(e)
         print("\nSomething's wrong, Unable to display the current time.")
         exit()
         
-# display the system uptime in a readable format
 def bootTime():
     return time.time() - psutil.boot_time()
 
 boot = bootTime()/60
 approxBoot = round(boot, 1)
 
-# Grab disk usage
 try:
     info = []
-    d = shutil.disk_usage("/") # info listed as tuple (total, used, free) *data in bytes
-    info = list(d) #convert to list and remove unwanted attr.
+    d = shutil.disk_usage("/") #tuple (total, used, free) *data in bytes
+    info = list(d)
     info.pop(2)
-    total = int(info[0]) / (1024 * 1024 * 1024) # total disk space
+    total = int(info[0]) / (1024 * 1024 * 1024)
     totalDisk = round(total, 1)
-    used = int(info[1]) / (1024 * 1024 * 1024) # total used space
+    used = int(info[1]) / (1024 * 1024 * 1024)
     usedDisk = round(used, 1)
     fraction = (usedDisk / totalDisk) *100
     newFraction = str(round(fraction, 1))
 except Exception as e:
     logging.exception(e)
     print("\nSomething went wrong while trying to access your disk.")
     exit()
 
-# get CPU frequency
 try:
     data = []
-    cpuData = psutil.cpu_freq() # tuple with (current, min, max)
+    cpuData = psutil.cpu_freq() # tuple (current, min, max)
     data = list(cpuData)
     floatFreq = int(data[0])/1000 #convert MHz to GHz
     freq = str(round(floatFreq, 2))
 except Exception as e:
     logging.exception(e)
     print("\nSomething went wrong while trying to access your CPU info.")
     exit()
 
-def infoGrabber():
+def main():
     try:
-        data = [] # data fills this list from 0-6
-        data.append(str(system())) # OS
-        data.append(str(release())) # version
-        data.append(str(machine())) # architecture
-        data.append(str(gethostname())) # hostname, duh
-        data.append(str(gethostbyname(gethostname()))) # IP addr.
-        data.append(str(processor())) # CPU
+        data = [] # data fills list from 0-6
+        data.append(str(system()))
+        data.append(str(release()))
+        data.append(str(machine()))
+        data.append(str(gethostname()))
+        data.append(str(gethostbyname(gethostname())))
+        data.append(str(processor()))
         data.append(str(round(psutil.virtual_memory().total / (1024.0 **3)))+" GB") # total RAM
         usage = (psutil.virtual_memory()[2]) # RAM usage
         newUsage = str(round(usage))
         spinner = spinningCursor()
         for _ in range(7):
             sys.stdout.write(next(spinner))
             sys.stdout.flush()
             time.sleep(0.1)
             sys.stdout.write('\b')
         print(cupImage)
         quoteGen()
         currentUser()
         getTime()
-        print("*------------------------------*") # display the data
+        print("*------------------------------*") # display
         print("OS: "+ data[0])
         print("VERSION: "+ data[1])
         print("CPU: "+ data[5] + " ("+ freq + " GHz)")
         print("ARCHITECTURE: "+ data[2])
         print("HOST: "+ data[3])
         print("UPTIME:", approxBoot, "minutes")
         print("IP: "+ data[4])
         print("RAM: "+ newUsage + "% used / " + data[6] + " total")
         print("DISK:", newFraction + "% used / "+ str(totalDisk) +" GB total")
         print("*------------------------------*")
     except Exception as e:
         logging.exception(e)
         print("\nSomething has failed, please check for any issues!!!")
         exit()
-        
+
+if __name__ == "__main__":
+    main()
```

### Comparing `coffeefetch-1.1.0/src/coffeefetch/quotes/quotes.txt` & `coffeefetch-1.2.1/src/coffeefetch/quotes/quotes.txt`

 * *Files 24% similar despite different names*

```diff
@@ -13,8 +13,13 @@
 "Bad command. Bad, bad command! Sit! Stay! Staaay..."
 "Every solution breeds new problems."
 "As a computer, I find your faith in technology amusing."
 "Two wrongs are only the beginning."
 "Shell to DOS... Come in DOS, do you copy? Shell to DOS..."
 "All computers wait at the same speed."
 "DEFINITION: Computer - A device designed to speed and automate errors."
-"Success always occurs in private, and failure in full view."
+"Success always occurs in private, and failure in full view."
+"I have an infinite capacity for knowledge, and even I'm not sure what's going on outside."
+"This. Sentence. Is. FALSE"
+"So. How are you holding up, BECAUSE I'M A POTATO."
+"Testing is the future, and the future starts with you."
+"Warning. Reactor core is at critical temperature."
```

### Comparing `coffeefetch-1.1.0/LICENCE` & `coffeefetch-1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `coffeefetch-1.1.0/README.md` & `coffeefetch-1.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # CoffeeFetch
-![image](https://github.com/TeaPixl/CoffeeFetch/assets/106362493/d4a4ee47-d3d1-4581-a9a8-e5a54605799d)
+![image](https://github.com/TeaPixl/CoffeeFetch/assets/106362493/71e27b7e-3d09-4b5b-8b6e-384b3f781b1b)
 ## A lightweight system info grabber written in Python
 
 ## Introduction
 CoffeeFetch is a system information grabber for Unix systems that fetches your system information and displays it to the screen. This is a lightweight package and is built to be run on systems without the use of a Window Manager or Desktop Enviornment and is displayed directly in in TTY. It will attempt to grab you CPU model, CPU frequency, current RAM consumption, current disk usage, Operating System, CPU architecture, IP Address, hostname, and OS version.
 
 ## Installation
 It is required to use Python 3.7 or greater for this package. 
+> psutil >= 5.9.5 is required for this package.
 
 Firstly, clone this repository:
 ```
 git clone https://github.com/TeaPixl/CoffeeFetch/
 cd CoffeeFetch
 ```
 Then, install the required Python modules
 ```
 pip install -r requirements.txt
 ```
 Build and install the .whl file
-> Change the X version you have
+> Change the X.X.X to the version you have
 ```
 python3 -m build
 cd dist/
 pip install coffeefetch-X.X.X-py3-none-any.whl
 ```
 OR
```

### Comparing `coffeefetch-1.1.0/pyproject.toml` & `coffeefetch-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "coffeefetch"
-version = "1.1.0"
+version = "1.2.1"
 authors = [
   { name="Logan Allen", email="ltallen392@gmail.com" },
 ]
 description = "A lightweight system information grabber written in Python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `coffeefetch-1.1.0/PKG-INFO` & `coffeefetch-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 Metadata-Version: 2.1
 Name: coffeefetch
-Version: 1.1.0
+Version: 1.2.1
 Summary: A lightweight system information grabber written in Python
 Project-URL: Homepage, https://github.com/TeaPixl/CoffeeFetch
 Project-URL: Bug Tracker, https://github.com/TeaPixl/CoffeeFetch/issues
 Author-email: Logan Allen <ltallen392@gmail.com>
 License-File: LICENCE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # CoffeeFetch
-![image](https://github.com/TeaPixl/CoffeeFetch/assets/106362493/d4a4ee47-d3d1-4581-a9a8-e5a54605799d)
+![image](https://github.com/TeaPixl/CoffeeFetch/assets/106362493/71e27b7e-3d09-4b5b-8b6e-384b3f781b1b)
 ## A lightweight system info grabber written in Python
 
 ## Introduction
 CoffeeFetch is a system information grabber for Unix systems that fetches your system information and displays it to the screen. This is a lightweight package and is built to be run on systems without the use of a Window Manager or Desktop Enviornment and is displayed directly in in TTY. It will attempt to grab you CPU model, CPU frequency, current RAM consumption, current disk usage, Operating System, CPU architecture, IP Address, hostname, and OS version.
 
 ## Installation
 It is required to use Python 3.7 or greater for this package. 
+> psutil >= 5.9.5 is required for this package.
 
 Firstly, clone this repository:
 ```
 git clone https://github.com/TeaPixl/CoffeeFetch/
 cd CoffeeFetch
 ```
 Then, install the required Python modules
 ```
 pip install -r requirements.txt
 ```
 Build and install the .whl file
-> Change the X version you have
+> Change the X.X.X to the version you have
 ```
 python3 -m build
 cd dist/
 pip install coffeefetch-X.X.X-py3-none-any.whl
 ```
 OR
```

