# Comparing `tmp/igrade-2.5.1.tar.gz` & `tmp/igrade-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igrade-2.5.1.tar", last modified: Fri Jun  2 22:55:51 2023, max compression
+gzip compressed data, was "igrade-2.5.2.tar", last modified: Sat Jun  3 22:19:56 2023, max compression
```

## Comparing `igrade-2.5.1.tar` & `igrade-2.5.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-02 22:55:51.873561 igrade-2.5.1/
--rw-r--r--   0 tamipeterson   (501) staff       (20)      690 2023-06-02 22:55:51.873332 igrade-2.5.1/PKG-INFO
--rw-r--r--   0 tamipeterson   (501) staff       (20)     4325 2023-06-02 22:47:52.000000 igrade-2.5.1/README.md
-drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-02 22:55:51.871647 igrade-2.5.1/igrade/
--rw-r--r--   0 tamipeterson   (501) staff       (20)    46256 2023-06-02 22:52:14.000000 igrade-2.5.1/igrade/__init__.py
-drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-02 22:55:51.873038 igrade-2.5.1/igrade.egg-info/
--rw-r--r--   0 tamipeterson   (501) staff       (20)      690 2023-06-02 22:55:51.000000 igrade-2.5.1/igrade.egg-info/PKG-INFO
--rw-r--r--   0 tamipeterson   (501) staff       (20)      186 2023-06-02 22:55:51.000000 igrade-2.5.1/igrade.egg-info/SOURCES.txt
--rw-r--r--   0 tamipeterson   (501) staff       (20)        1 2023-06-02 22:55:51.000000 igrade-2.5.1/igrade.egg-info/dependency_links.txt
--rw-r--r--   0 tamipeterson   (501) staff       (20)       83 2023-06-02 22:55:51.000000 igrade-2.5.1/igrade.egg-info/requires.txt
--rw-r--r--   0 tamipeterson   (501) staff       (20)        7 2023-06-02 22:55:51.000000 igrade-2.5.1/igrade.egg-info/top_level.txt
--rw-r--r--   0 tamipeterson   (501) staff       (20)       38 2023-06-02 22:55:51.873765 igrade-2.5.1/setup.cfg
--rw-r--r--   0 tamipeterson   (501) staff       (20)     1158 2023-06-02 22:54:26.000000 igrade-2.5.1/setup.py
+drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-03 22:19:56.674869 igrade-2.5.2/
+-rw-r--r--   0 tamipeterson   (501) staff       (20)     1071 2023-06-03 19:34:07.000000 igrade-2.5.2/LICENSE
+-rw-r--r--   0 tamipeterson   (501) staff       (20)      561 2023-06-03 22:19:56.674603 igrade-2.5.2/PKG-INFO
+-rw-r--r--   0 tamipeterson   (501) staff       (20)     4511 2023-06-03 22:15:14.000000 igrade-2.5.2/README.md
+drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-03 22:19:56.672295 igrade-2.5.2/igrade/
+-rw-r--r--   0 tamipeterson   (501) staff       (20)    43051 2023-06-03 21:31:44.000000 igrade-2.5.2/igrade/API.py
+-rw-r--r--   0 tamipeterson   (501) staff       (20)       30 2023-06-03 19:37:52.000000 igrade-2.5.2/igrade/__init__.py
+-rw-r--r--   0 tamipeterson   (501) staff       (20)      286 2023-06-03 19:57:47.000000 igrade-2.5.2/igrade/exceptions.py
+-rw-r--r--   0 tamipeterson   (501) staff       (20)     2672 2023-06-03 20:54:58.000000 igrade-2.5.2/igrade/utils.py
+drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-03 22:19:56.674193 igrade-2.5.2/igrade.egg-info/
+-rw-r--r--   0 tamipeterson   (501) staff       (20)      561 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/PKG-INFO
+-rw-r--r--   0 tamipeterson   (501) staff       (20)      245 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/SOURCES.txt
+-rw-r--r--   0 tamipeterson   (501) staff       (20)        1 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/dependency_links.txt
+-rw-r--r--   0 tamipeterson   (501) staff       (20)       82 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/requires.txt
+-rw-r--r--   0 tamipeterson   (501) staff       (20)        7 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/top_level.txt
+-rw-r--r--   0 tamipeterson   (501) staff       (20)       38 2023-06-03 22:19:56.675068 igrade-2.5.2/setup.cfg
+-rw-r--r--   0 tamipeterson   (501) staff       (20)     1079 2023-06-03 21:59:04.000000 igrade-2.5.2/setup.py
```

### Comparing `igrade-2.5.1/README.md` & `igrade-2.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,18 @@
     print(assignment['name'] + ' is due on ' + assignment['due'])
 
 client.close()  # close the client
 ```
 
 # Changelog:
 
+### 2023.6.3
+* ***2.5.2*** - Regex search for filters; exceptions rework; fixed binary bytes showing up in
+get_class_performance(); now+{days} date filter addition; grade filter update
+
 ### 2023.6.2
 * ***2.5.1*** - Added package to Pypi
 
 * ***2.5.0*** - Updated README
 
 * ***2.4.8*** - Finished ReadTheDocs page; added requirements.txt
```

### Comparing `igrade-2.5.1/igrade/__init__.py` & `igrade-2.5.2/igrade/API.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from re import search
 from asyncio import gather, ensure_future, get_event_loop, run
-from datetime import datetime, timedelta
 from re import search
-from time import localtime
 from aiohttp import ClientSession
 from requests import session
 from bs4 import BeautifulSoup
 from sys import modules
 from os import mkdir
 from warnings import simplefilter
 from shutil import rmtree
 from colorama import Fore, Style
+from igrade import exceptions
+from igrade import utils
 
 
 try:
     rmtree('data')
 except FileNotFoundError:
     pass
 
@@ -23,35 +24,35 @@
 
 
 class Client:
 
     def __init__(self, debug=False):
 
         if 'lxml' not in modules:
-            raise Exception("'lxml' has not been imported. Type 'pip install lxml' to fix this issue.")
+            raise ImportError("'lxml' has not been imported. Type 'pip install lxml' to fix this issue.")
         if 'bs4' not in modules:
-            raise Exception("'bs4' has not been imported. Type 'pip install bs4' to fix this issue.")
+            raise ImportError("'bs4' has not been imported. Type 'pip install bs4' to fix this issue.")
         if 'requests' not in modules:
-            raise Exception("'requests' has not been imported. Type 'pip install requests' to fix this issue.")
+            raise ImportError("'requests' has not been imported. Type 'pip install requests' to fix this issue.")
 
         self.serverid: str = ''
         self.sessionid: str = ''
         self.loggedin: bool = False
 
         # session used for speed and keep cookies the same across requests
         self.session = session()
         self.session.headers = {
             "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36"}
 
         # self.aiosession = aiohttp.ClientSession()
         self.is_logging = debug
 
-        self.log('CLIENT', 'client has started')
+        self.__log('CLIENT', 'client has started')
 
-    def log(self, message, content, color: str = 'none'):
+    def __log(self, message, content, color: str = 'none'):
 
         if self.is_logging:
             if color.lower() == 'red':
                 color = Fore.RED
             elif color.lower() == 'green':
                 color = Fore.GREEN
             elif color.lower() == 'yellow':
@@ -61,67 +62,67 @@
             elif color.lower() == 'blue':
                 color = Fore.BLUE
 
             print(f'[{color}{message}{Style.RESET_ALL}] {content}')
 
     def login_with_credentials(self, username: str, password: str):
 
-        self.log('LOGIN', 'logging in...')
+        self.__log('LOGIN', 'logging in...')
         pageid = self.__get_pageid("https://igradeplus.com/login/student")
 
         # pageid = str(BeautifulSoup(self.session.get("https://igradeplus.com/login/student").text, 'lxml').find_all("head")[0].get('id'))
 
         # verify to server pageid
         self.__send_ajax_verify(pageid)
 
         # get login tokens
         if self.__send_ajax_login2(username, password, pageid, '53'):
 
             self.loggedin = True
-            self.log('LOGIN', 'logged in', 'green')
+            self.__log('LOGIN', 'logged in', 'green')
 
         else:
-            raise Exception('Incorrect credentials.')
+            raise exceptions.LoginError('Incorrect credentials.')
 
         # save login tokens
         self.sessionid = self.session.cookies['JSESSIONID']
         self.serverid = self.session.cookies['SERVERID']
 
         self.aiosession = ClientSession(headers={
             "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
             'Cookie': f'JSESSIONID={self.sessionid}; SERVERID={self.serverid};'})
 
-        self.log('CLIENT', 'client sessions initialized.')
+        self.__log('CLIENT', 'client sessions initialized.')
 
     def login_with_token(self, sessionid: str, serverid: str):
 
-        self.log('LOGIN', 'logging in...')
+        self.__log('LOGIN', 'logging in...')
 
         self.sessionid = sessionid
         self.serverid = serverid
 
         # set cookies
         self.session.cookies.set('SERVERID', serverid, domain="igradeplus.com")
         self.session.cookies.set('JSESSIONID', sessionid, domain="igradeplus.com")
 
         # I chose this url because it seems fastest
         if BeautifulSoup(self.session.get('https://igradeplus.com/student/myaccount').text, 'lxml').find(
                 'title').text == 'iGradePlus SMS':
 
             self.loggedin = True
-            self.log('LOGIN', 'logged in', 'green')
+            self.__log('LOGIN', 'logged in', 'green')
 
         else:
-            raise Exception('Incorrect credentials.')
+            raise exceptions.LoginError('Incorrect credentials.')
 
         self.aiosession = ClientSession(headers={
             "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36",
             'Cookie': f'JSESSIONID={self.sessionid}; SERVERID={self.serverid};'})
 
-        self.log('CLIENT', 'client sessions initialized.')
+        self.__log('CLIENT', 'client sessions initialized.')
 
     def __send_ajax(self, pageid: str, id: str, event: str = '30', return_: bool = False):
 
         if return_:
             return self.session.post("https://igradeplus.com/OorianAjaxEventHandler", data=
         {
             'callback': '',
@@ -268,168 +269,146 @@
                 'callback': 'createtable',
                 'pageid': pageid,
                 'sourceid': 'problematicassignments',
                 'targetid': 'problematicassignments',
                 'event': '30'
             }).text
 
-    def __get_assignments(self, get_type: str, get_attachments: bool = False, name: str = '', grade: str = '', assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def __get_assignments(self, get_type: str, get_attachments: bool = False, name: str = '', grade: tuple = (), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
 
         # name filter will get all assignments that include the string given. it is not case-sensitive and removes spaces and underscores.
         # grade filter is two numbers from 0+. example: '50-100' gets all assignments from 50 to 100. assignments with null grades are always filtered if this filter is set.
         # assignments_type filter. values can be 'extra credit', 'no value', or 'standard'. this is cleaned like the name filter. there are also more types than these 3.
         # category filter gets assignments with a certain category. this is cleaned and can match either the abbreviation or the full category name in order for the assignment to stay. categories dependent on class.
         # due filter gets assignments that match in between two dates. example: ('2023.4.1', '2023.5.1'). items in the tuple can also be 'now' for the current date.
         # assigned filter is the same as above, with assigned dates
 
-        # better algorithm - covers all edge cases
-        def is_past(date: str, due_in: int):
-
-            try:
-                date = list(date.split('.'))
-                now = list(str(datetime(*localtime()[:6]) + timedelta(days=due_in)).split(' ')[0].split('-'))
-
-                for j in range(3):
-                    now[j] = int(now[j])
-
-                for j in range(3):
-                    date[j] = int(date[j])
-
-            except ValueError:
-                return None
-
-            if now[0] > date[0]:
-                return True
-
-            elif now[0] == date[0] and now[1] > date[1]:
-                return True
-
-            elif now[0] == date[0] and now[1] == date[1] and now[2] > date[2]:
-                return True
-
-            return False
-
-        def is_date_between(start_date: str, end_date: str, check_date: str):
-
-            if start_date.lower() == 'now':
-                start_date = datetime.now().strftime('%Y.%m.%d')
-
-            if end_date.lower() == 'now':
-                end_date = datetime.now().strftime('%Y.%m.%d')
-
-            return datetime.strptime(start_date, '%Y.%m.%d') <= datetime.strptime(check_date, '%Y.%m.%d') <= datetime.strptime(end_date, '%Y.%m.%d')
-
-        def is_between(date: str, days: int):
-            return is_past(date, days + 1) and (not is_past(date, 0))
-
-        def clean(content: str):
-
-            return content.lower().replace(' ', '').replace('_', '')
 
         html = self.__get_assignments_raw(get_type)
 
         elements = []
         links = []
 
-        self.log('CLIENT', f'getting {assignment_type} attachments.')
+        self.__log('CLIENT', f'getting {assignment_type} attachments.')
 
         soup = BeautifulSoup(html, 'lxml')
         i = 0
 
         for table in soup.find_all('tbody')[1].find_all('tr'):
 
             try:
                 sections = table.find_all('td')
                 elements.append({})
 
                 # NAME ------
                 assignment_name = sections[0].text
 
-                if name.lower().replace(' ', '') not in assignment_name.lower().replace(' ', ''):
+                if not search(name, assignment_name):
                     # print(name.lower().replace(' ', '') + ' is not in ' + assignment_name.lower().replace(' ', ''))
                     elements.pop()
                     continue
 
                 # GRADE ------
                 if sections[3].text == '\xa0':
                     assignment_percent = None
                     assignment_letter = None
 
                 else:
                     assignment_percent = sections[3].text[:-3]
                     assignment_letter = sections[3].text[-2:-1]
 
                 if grade:
-                    if assignment_percent is None:
+                    try:
+                        continue_: bool = not grade[2]
+                    except IndexError:
+                        continue_ = True
+
+                    if (assignment_percent is None) and not continue_:
+                        pass
+                    elif assignment_percent is None:
                         elements.pop()
                         continue
-
-                    if not (float(grade.split('-')[0]) <= float(assignment_percent[:-1]) <= float(grade.split('-')[1])):
+                    elif not (float(grade[0]) <= float(assignment_percent[:-1]) <= float(grade[1])):
                         elements.pop()
                         continue
 
                 # TYPE --------
                 this_assignment_type = sections[7].contents[0].get('title')
 
-                if assignment_type and (clean(assignment_type) != clean(this_assignment_type)):
+                if assignment_type and (utils.clean(assignment_type) != utils.clean(this_assignment_type)):
 
                     elements.pop()
                     continue
 
                 # CATEGORY ---------
                 assignment_category_full = sections[9].contents[0].get('title')
                 assignment_category_abbr = sections[9].contents[0].text
 
                 if category:
-                    if (clean(category) not in clean(assignment_category_abbr)) and (clean(category) not in clean(assignment_category_abbr)):
+                    if not search(category, assignment_category_abbr) and not search(category, assignment_category_full):
 
                         elements.pop()
                         continue
 
                 # CLASS ----------
                 element = sections[8].text
 
                 if element == "No Value":
                     assignment_class = "none"
                 else:
                     assignment_class = sections[8].text
 
-                if class_ and (clean(class_) not in clean(assignment_class)):
+                if class_ and not search(class_, assignment_class):
 
                     elements.pop()
                     continue
 
                 # DUE -------
                 try:
                     assignment_due = sections[6].text
                 except IndexError:
                     assignment_due = None
 
                 if due:
-                    if assignment_due is None or assignment_due == '':
+                    try:
+                        continue_ = not due[2]
+                    except IndexError:
+                        continue_ = True
+
+                    if (assignment_due is None or assignment_due == '') and continue_:
                         elements.pop()
+                        print(1)
                         continue
-
-                    if not is_date_between(due[0], due[1], assignment_due):
+                    elif (assignment_due is None or assignment_due == '') and not continue_:
+                        print(2)
+                        pass
+                    elif not utils.is_date_between(due[0], due[1], assignment_due):
 
                         elements.pop()
+                        print(3)
                         continue
 
                 # ASSIGNED ---------
                 try:
                     assignment_assigned = sections[5].text
                 except IndexError:
                     assignment_assigned = None
 
                 if assigned:
-                    if assignment_assigned is None or assignment_assigned == '':
+                    try:
+                        continue_ = not assigned[2]
+                    except IndexError:
+                        continue_ = True
+
+                    if (assignment_assigned is None or assignment_assigned == '') and continue_:
                         elements.pop()
                         continue
-
-                    if not is_date_between(assigned[0], assigned[1], assignment_assigned):
+                    elif (assignment_assigned is None or assignment_assigned == '') and not continue_:
+                        pass
+                    elif not utils.is_date_between(assigned[0], assigned[1], assignment_assigned):
 
                         elements.pop()
                         continue
 
                 elements[i]['name'] = assignment_name
                 elements[i]['link'] = f"https://igradeplus.com/student/{sections[0].contents[0].get('href')}"
                 elements[i]['id'] = elements[i]['link'].split('?id=')[1]
@@ -480,114 +459,76 @@
 
                 if element == "\xa0":
                     elements[i]['grade']['value'] = None
 
                 else:
                     elements[i]['grade']['value'] = int(sections[10].text.split('.')[0])
 
-                # try:
-                #     date = elements[i]['due'].split('.')
-                #     now = time.strftime("%Y.%m.%d", time.localtime()).split('.')
-                #
-                #     for j in range(3):
-                #         now[j] = int(now[j])
-                #
-                #     for j in range(3):
-                #         date[j] = int(date[j])
-                #
-                #     if now[0] > date[0] or now[1] > date[1] or now[2] > date[2]:
-                #         elements[i]['details'] = {'past_due': True}
-                #
-                #     else:
-                #         elements[i]['details'] = {'past_due': False}
-                #
-                # except ValueError:
-                #     elements[i]['details'] = {'past_due': None}
-
-                elements[i]['details'] = {'past_due': is_past(elements[i]['due'], 0)}
-
-                # try:
-                #     date = elements[i]['assigned'].split('.')
-                #     now = time.strftime("%Y.%m.%d", time.localtime()).split('.')
-                #
-                #     for j in range(3):
-                #         now[j] = int(now[j])
-                #
-                #     for j in range(3):
-                #         date[j] = int(date[j])
-                #
-                #     if now[0] > date[0] or now[1] > date[1] or now[2] > date[2]:
-                #         elements[i]['details']['has_been_assigned'] = True
-                #
-                #     else:
-                #         elements[i]['details']['has_been_assigned'] = False
-                #
-                # except ValueError:
-                #     elements[i]['details']['has_been_assigned'] = None
+                elements[i]['details'] = {'past_due': utils.is_past(elements[i]['due'], 0)}
 
                 if elements[i]['grade']['points'] is None:
                     elements[i]['details']['graded'] = False
 
                 else:
                     elements[i]['details']['graded'] = True
 
-                elements[i]['details']['has_been_assigned'] = is_past(elements[i]['assigned'], 0)
+                elements[i]['details']['has_been_assigned'] = utils.is_past(elements[i]['assigned'], 0)
                 elements[i]['details']['in_class_assignment'] = elements[i]['due'] == elements[i]['assigned']
-                elements[i]['details']['due_tomorrow'] = is_between(elements[i]['due'], 1)
-                elements[i]['details']['due_in_week'] = is_between(elements[i]['due'], 8)
+                elements[i]['details']['due_tomorrow'] = utils.is_between(elements[i]['due'], 1)
+                elements[i]['details']['due_in_week'] = utils.is_between(elements[i]['due'], 8)
 
 
                 if get_attachments:
 
                     links.append(elements[i]['link'])
 
                 i += 1
 
             except AttributeError:
 
                 # if assignment invalid
-                self.log('ERROR', 'invalid assignment. removing from list.', 'yellow')
+                self.__log('ERROR', 'invalid assignment. removing from list.', 'yellow')
                 elements.pop()
                 break
 
         if get_attachments:
 
             response = self.__get_all_attachments(links)
             i = 0
 
-            self.log('CLIENT', 'getting assignment page info.')
+            self.__log('CLIENT', 'getting assignment page info.')
 
             for assignment in response:
 
                 elements[i]['attachments'] = assignment['attachments']
                 elements[i]['description'] = assignment['description']
                 elements[i]['supplemental_info'] = assignment['supplemental_info']
 
                 i += 1
 
-        self.log('CLIENT', 'data returned successfully.', 'green')
+        self.__log('CLIENT', 'data returned successfully.', 'green')
 
         return elements
 
-    def get_all_assignments(self, get_attachments: bool = False, name='', grade='', assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def get_all_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
 
         self.__verify()
         return self.__get_assignments('all', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned)
 
-    def get_upcoming_assignments(self, get_attachments: bool = False, name='', grade='', assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def get_upcoming_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
 
         self.__verify()
         return self.__get_assignments('upcoming', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned)
 
-    def get_recent_assignments(self, get_attachments: bool = False, name='', grade='', assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def get_recent_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
 
         self.__verify()
         return self.__get_assignments('recent', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned)
 
-    def get_problematic_assignments(self, get_attachments: bool = False, name='', grade='', assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def get_problematic_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
 
         self.__verify()
         return self.__get_assignments('problematic', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned)
 
     def get_account_info(self):
 
         self.__verify()
@@ -694,19 +635,20 @@
 
     def __verify(self):
 
         if self.loggedin:
             return
 
         else:
-            raise Exception("Client is not logged in.")
+            raise exceptions.LoginError("Client is not logged in.")
 
     def get_attachments(self, assignment_id):
 
-        self.log('CLIENT', 'getting attachments.')
+        self.__verify()
+        self.__log('CLIENT', 'getting attachments.')
 
         html = self.session.get('https://igradeplus.com/student/assignment?id=' + assignment_id).text
         soup = BeautifulSoup(html, 'lxml')
 
         # get pageid. if the code ever acts up its probably this,
         # uncomment the line below if it does
         pageid = html[31:67]
@@ -747,17 +689,17 @@
 
             i += 1
 
         return elements
 
     def __get_all_attachments(self, links: list):
 
-        async def stuff(url):
+        async def mainloop(url):
 
-            self.log('CLIENT', 'getting extra assignment info.')
+            self.__log('CLIENT', 'getting extra assignment info.')
 
             html = await self.aiosession.get(url)
             html = await html.text()
 
 
             soup = BeautifulSoup(html, 'lxml')
 
@@ -803,24 +745,24 @@
                         'sourceid': linkid,
                         'targetid': linkid,
                         'event': '1'}
                     )
                     elements['attachments'][i][
                         'link'] = BeautifulSoup(await wait.text(), 'lxml').find('a').get('href')
                 except:
-                    self.log('ERROR', 'error occurred while sending oorian request.', 'yellow')
+                    self.__log('ERROR', 'error occurred while sending oorian request.', 'yellow')
 
-            self.log('CLIENT', 'extra assignment info returned successfully.', 'green')
+            self.__log('CLIENT', 'extra assignment info returned successfully.', 'green')
             return elements
 
         async def main():
 
             tasks = []
             for url in links:
-                tasks.append(ensure_future(stuff(url)))
+                tasks.append(ensure_future(mainloop(url)))
 
             responses = await gather(*tasks)
             return responses
 
         loop = get_event_loop()
 
         results = loop.run_until_complete(main())
@@ -828,14 +770,16 @@
 
         response = results
 
         return response
 
     def get_all_events(self):
 
+        self.__verify()
+
         html = self.session.get("https://igradeplus.com/student/communications/calendar").text
         pageid = html[31:67]
         targetid = BeautifulSoup(html, 'lxml').find('div', style='visibility: visible; position: relative; ').get('id')
 
         self.session.post('https://igradeplus.com/OorianAjaxEventHandler', data={
             'menuitem': 'School Year View',
             'pageid': pageid,
@@ -846,22 +790,14 @@
 
         # self.__send_ajax(pageid, '0', event='41')
 
         pageid = self.__get_pageid("https://igradeplus.com/student/communications/calendar")
 
         html = self.__send_ajax(pageid, '12', return_=True)
 
-        # html = self.session.post('https://igradeplus.com/OorianAjaxEventHandler', data={
-        #     'callback': '',
-        #     'pageid': pageid,
-        #     'sourceid': '12',
-        #     'targetid': '12',
-        #     'event': '30'
-        # }).text
-
         elements = []
         soup = BeautifulSoup(html, 'lxml')
 
         i = 0
         for section in soup.find_all('div', style="color: #000000; background: #FFFFFF; padding-top: 10.0px; padding-right: 50.0px; padding-bottom: 10.0px; padding-left: 5.0px; border-top-style: solid; border-top-color: #F0F0F0; border-top-width: 1.0px; "):
 
             day = section.find('a', style='font-size: 15px; font-weight: bold; color: #404040; text-decoration: none; line-height: 250%; ')
@@ -880,14 +816,16 @@
 
             i += 1
 
         return elements
 
     def get_upcoming_events(self):
 
+        self.__verify()
+
         html = self.session.get("https://igradeplus.com/student/communications/calendar").text
         pageid = html[31:67]
         targetid = BeautifulSoup(html, 'lxml').find('div', style='visibility: visible; position: relative; ').get('id')
 
         self.session.post('https://igradeplus.com/OorianAjaxEventHandler', data={
             'menuitem': 'Full Expanded View',
             'pageid': pageid,
@@ -898,22 +836,14 @@
 
         # self.__send_ajax(pageid, '0', '41')
 
         pageid = self.__get_pageid("https://igradeplus.com/student/communications/calendar")
 
         html = self.__send_ajax(pageid, '12', return_=True)
 
-        # html = self.session.post('https://igradeplus.com/OorianAjaxEventHandler', data={
-        #     'callback': '',
-        #     'pageid': pageid,
-        #     'sourceid': '12',
-        #     'targetid': '12',
-        #     'event': '30'
-        # }).text
-
         elements = []
         soup = BeautifulSoup(html, 'lxml')
 
         i = 0
         for section in soup.find_all('td', style='vertical-align: top; overflow: hidden; height: 100%; padding-top: 0.0px; padding-right: 0.0px; padding-bottom: 0.0px; padding-left: 0.0px; '):
             elements.append({})
 
@@ -948,14 +878,16 @@
     def __get_pageid(self, url):
 
         # self.log('CLIENT', 'obtaining pageID')
         return self.session.get(url).text[31:67]
 
     def get_announcements(self, get_link=False):
 
+        self.__verify()
+
         if not get_link:
             pageid = self.__get_pageid('https://igradeplus.com/student/communications/bulletinboard')
 
             html = self.__send_ajax(pageid, '12', '30', return_=True)
 
             soup = BeautifulSoup(html, 'lxml')
 
@@ -1009,36 +941,42 @@
 
                 i += 1
 
             return data
 
     def get_announcement_content(self, announcement_id, html=True):
 
+        self.__verify()
+
         if html:
             return str(BeautifulSoup(self.session.get('https://igradeplus.com/student/communications/bulletin?id=' + announcement_id).text, 'xml').find('div', attrs={'class': 'fr-view'}))
 
         return str(BeautifulSoup(self.session.get('https://igradeplus.com/student/communications/bulletin?id=' + announcement_id).text, 'xml').find('div', attrs={'class': 'fr-view'}).text)
 
     def get_event_content(self, event_id):
 
+        self.__verify()
+
         data = {}
 
         soup = BeautifulSoup(self.session.get('https://igradeplus.com/student/communications/calendar/event?id='+ event_id).text, 'lxml')
         data['location'] = soup.find_all('span', style='color: #000000; ')[2].text
 
         element = soup.find('div', style='line-height: 200%; font-size: 12px; padding-top: 25.0px; padding-right: 50.0px; padding-bottom: 0.0px; padding-left: 0.0px; ')
         data['html'] = element.prettify()
         data['text'] = element.text
 
         return data
 
     def download_attachments(self, assignment_id: str, folder_location: str = 'data'):
 
+        self.__verify()
+
         response = []
-        self.log('CLIENT', 'downloading attachments...')
+        self.__log('CLIENT', 'downloading attachments...')
 
         data = self.get_attachments(assignment_id)['attachments']
 
         try:
             mkdir(folder_location)
         except FileExistsError:
             pass
@@ -1046,19 +984,21 @@
         for i in range(len(data)):
 
             with open(f'{folder_location}/{data[i]["name"].replace(" ", "_")}', 'wb') as f:
 
                 f.write(self.session.get(data[i]['link']).content)
                 response.append(f'{folder_location}/{data[i]["name"].replace(" ", "_")}')
 
-        self.log('CLIENT', 'download successful', 'green')
+        self.__log('CLIENT', 'download successful', 'green')
         return response
 
     def get_teachers_info(self):
 
+        self.__verify()
+
         data = []
 
         html = self.session.get('https://igradeplus.com/student/teachers').text
         soup = BeautifulSoup(html, 'lxml')
 
         i = 0
         for element in soup.find_all('div', style='font-family: Arial; font-size: 14px; background: #FFFFFF; color: #505050; padding-top: 0.0px; padding-right: 0.0px; padding-bottom: 15.0px; padding-left: 0.0px; line-height: 160%; width: 350.0px; height: 280.0px; min-width: 350.0px; max-width: 600.0px; margin-top: 10.0px; margin-right: 10.0px; margin-bottom: 0.0px; margin-left: 0.0px; flex-grow: 1; position: relative; '):
@@ -1095,71 +1035,46 @@
 
     def close(self):
 
         async def await_close():
             await self.aiosession.close()
 
         # self.aiosession.close()
-        self.log('CLIENT', 'closing client...')
+        self.__log('CLIENT', 'closing client...')
         self.session.close()
 
         run(await_close())
-        self.log('CLIENT', 'client closed.', 'green')
+        self.__log('CLIENT', 'client closed.', 'green')
 
     def get_attendance(self):
 
-        def get_rows(section):
-
-            data = []
-            i = 0
-
-            for row in section.find_all('tr', style='background: #FFFFFF; '):
-                column = row.find_all('td')
-                data.append({})
-
-                data[i]['class'] = column[0].text
-                data[i]['data'] = {}
-                data[i]['data']['present'] = int(column[1].text)
-                data[i]['data']['absent'] = int(column[2].text)
-                data[i]['data']['tardy'] = int(column[3].text)
-                data[i]['data']['excused'] = int(column[4].text)
-                data[i]['data']['virtual'] = int(column[5].text)
-
-                i += 1
-
-            return data
+        self.__verify()
 
         pageid = self.__get_pageid('https://igradeplus.com/student/attendance')
 
         html = self.__send_ajax(pageid, '166', return_=True)
 
-        # html = self.session.post('https://igradeplus.com/OorianAjaxEventHandler', data={
-        #     'callback': '',
-        #     'pageid': pageid,
-        #     'sourceid': '166',
-        #     'targetid': '166',
-        #     'event': '30'
-        # }).text
-
         soup = BeautifulSoup(html, 'lxml')
         data = {}
 
         section = soup.find('tbody', style='overflow-x: hidden; overflow-y: scroll; border-bottom-style: solid; border-bottom-color: #EEEEEE; border-bottom-width: 1px; ')
-        data['total'] = get_rows(section)
+        data['total'] = utils.attendance_get_rows(section)
 
         section = soup.find_all('tbody', style='overflow-x: hidden; overflow-y: scroll; border-bottom-style: solid; border-bottom-color: #EEEEEE; border-bottom-width: 1px; ')[1]
-        data['s1'] = get_rows(section)
+        data['s1'] = utils.attendance_get_rows(section)
 
         section = soup.find_all('tbody', style='overflow-x: hidden; overflow-y: scroll; border-bottom-style: solid; border-bottom-color: #EEEEEE; border-bottom-width: 1px; ')[2]
-        data['s2'] = get_rows(section)
+        data['s2'] = utils.attendance_get_rows(section)
 
         return data
 
     def get_class_performance(self):
 
+        self.__verify()
+
         async def get_performance(link, teacher, id):
 
             html = await self.aiosession.get(link)
             html = await html.text()
 
             soup = BeautifulSoup(html, 'lxml')
 
@@ -1172,17 +1087,17 @@
 
             for row in soup.find_all('tr', style='background: #FFFFFF; '):
 
                 elements.append({})
                 data = row.find_all('td')
 
                 elements[i]['type'] = data[0].text
-                elements[i]['s1'] = data[1].text[:-2]
-                elements[i]['s2'] = data[2].text[:-2]
-                elements[i]['total'] = data[3].text[:-2]
+                elements[i]['s1'] = data[1].text[:-3]
+                elements[i]['s2'] = data[2].text[:-3]
+                elements[i]['total'] = data[3].text[:-3]
 
                 i += 1
 
             return elements
 
         async def main():
```

