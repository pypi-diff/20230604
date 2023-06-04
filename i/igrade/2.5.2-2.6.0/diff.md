# Comparing `tmp/igrade-2.5.2.tar.gz` & `tmp/igrade-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igrade-2.5.2.tar", last modified: Sat Jun  3 22:19:56 2023, max compression
+gzip compressed data, was "igrade-2.6.0.tar", last modified: Sun Jun  4 01:54:54 2023, max compression
```

## Comparing `igrade-2.5.2.tar` & `igrade-2.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-03 22:19:56.674869 igrade-2.5.2/
--rw-r--r--   0 tamipeterson   (501) staff       (20)     1071 2023-06-03 19:34:07.000000 igrade-2.5.2/LICENSE
--rw-r--r--   0 tamipeterson   (501) staff       (20)      561 2023-06-03 22:19:56.674603 igrade-2.5.2/PKG-INFO
--rw-r--r--   0 tamipeterson   (501) staff       (20)     4511 2023-06-03 22:15:14.000000 igrade-2.5.2/README.md
-drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-03 22:19:56.672295 igrade-2.5.2/igrade/
--rw-r--r--   0 tamipeterson   (501) staff       (20)    43051 2023-06-03 21:31:44.000000 igrade-2.5.2/igrade/API.py
--rw-r--r--   0 tamipeterson   (501) staff       (20)       30 2023-06-03 19:37:52.000000 igrade-2.5.2/igrade/__init__.py
--rw-r--r--   0 tamipeterson   (501) staff       (20)      286 2023-06-03 19:57:47.000000 igrade-2.5.2/igrade/exceptions.py
--rw-r--r--   0 tamipeterson   (501) staff       (20)     2672 2023-06-03 20:54:58.000000 igrade-2.5.2/igrade/utils.py
-drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-03 22:19:56.674193 igrade-2.5.2/igrade.egg-info/
--rw-r--r--   0 tamipeterson   (501) staff       (20)      561 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/PKG-INFO
--rw-r--r--   0 tamipeterson   (501) staff       (20)      245 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/SOURCES.txt
--rw-r--r--   0 tamipeterson   (501) staff       (20)        1 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/dependency_links.txt
--rw-r--r--   0 tamipeterson   (501) staff       (20)       82 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/requires.txt
--rw-r--r--   0 tamipeterson   (501) staff       (20)        7 2023-06-03 22:19:56.000000 igrade-2.5.2/igrade.egg-info/top_level.txt
--rw-r--r--   0 tamipeterson   (501) staff       (20)       38 2023-06-03 22:19:56.675068 igrade-2.5.2/setup.cfg
--rw-r--r--   0 tamipeterson   (501) staff       (20)     1079 2023-06-03 21:59:04.000000 igrade-2.5.2/setup.py
+drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-04 01:54:54.455849 igrade-2.6.0/
+-rw-r--r--   0 tamipeterson   (501) staff       (20)     1071 2023-06-03 19:34:07.000000 igrade-2.6.0/LICENSE
+-rw-r--r--   0 tamipeterson   (501) staff       (20)      561 2023-06-04 01:54:54.455587 igrade-2.6.0/PKG-INFO
+-rw-r--r--   0 tamipeterson   (501) staff       (20)     3997 2023-06-04 01:52:52.000000 igrade-2.6.0/README.md
+drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-04 01:54:54.453239 igrade-2.6.0/igrade/
+-rw-r--r--   0 tamipeterson   (501) staff       (20)    46336 2023-06-04 01:34:39.000000 igrade-2.6.0/igrade/API.py
+-rw-r--r--   0 tamipeterson   (501) staff       (20)       30 2023-06-03 19:37:52.000000 igrade-2.6.0/igrade/__init__.py
+-rw-r--r--   0 tamipeterson   (501) staff       (20)      286 2023-06-03 19:57:47.000000 igrade-2.6.0/igrade/exceptions.py
+-rw-r--r--   0 tamipeterson   (501) staff       (20)     2672 2023-06-03 20:54:58.000000 igrade-2.6.0/igrade/utils.py
+drwxr-xr-x   0 tamipeterson   (501) staff       (20)        0 2023-06-04 01:54:54.455217 igrade-2.6.0/igrade.egg-info/
+-rw-r--r--   0 tamipeterson   (501) staff       (20)      561 2023-06-04 01:54:54.000000 igrade-2.6.0/igrade.egg-info/PKG-INFO
+-rw-r--r--   0 tamipeterson   (501) staff       (20)      245 2023-06-04 01:54:54.000000 igrade-2.6.0/igrade.egg-info/SOURCES.txt
+-rw-r--r--   0 tamipeterson   (501) staff       (20)        1 2023-06-04 01:54:54.000000 igrade-2.6.0/igrade.egg-info/dependency_links.txt
+-rw-r--r--   0 tamipeterson   (501) staff       (20)       81 2023-06-04 01:54:54.000000 igrade-2.6.0/igrade.egg-info/requires.txt
+-rw-r--r--   0 tamipeterson   (501) staff       (20)        7 2023-06-04 01:54:54.000000 igrade-2.6.0/igrade.egg-info/top_level.txt
+-rw-r--r--   0 tamipeterson   (501) staff       (20)       38 2023-06-04 01:54:54.456066 igrade-2.6.0/setup.cfg
+-rw-r--r--   0 tamipeterson   (501) staff       (20)     1078 2023-06-04 00:56:32.000000 igrade-2.6.0/setup.py
```

### Comparing `igrade-2.5.2/LICENSE` & `igrade-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `igrade-2.5.2/PKG-INFO` & `igrade-2.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igrade
-Version: 2.5.2
+Version: 2.6.0
 Summary: An unofficial wrapper for iGradePlus Student Management Systems.
 Home-page: https://github.com/Kasherpete/Igrade-web-scraper
 Author: Keagan Peterson
 Author-email: Keagan.a.peterson@outlook.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `igrade-2.5.2/igrade/API.py` & `igrade-2.6.0/igrade/API.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from re import search
+import re
 from asyncio import gather, ensure_future, get_event_loop, run
 from re import search
 from aiohttp import ClientSession
 from requests import session
 from bs4 import BeautifulSoup
 from sys import modules
 from os import mkdir
@@ -269,15 +269,15 @@
                 'callback': 'createtable',
                 'pageid': pageid,
                 'sourceid': 'problematicassignments',
                 'targetid': 'problematicassignments',
                 'event': '30'
             }).text
 
-    def __get_assignments(self, get_type: str, get_attachments: bool = False, name: str = '', grade: tuple = (), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def __get_assignments(self, get_type: str, get_attachments: bool = False, name: str = '', grade: tuple = (), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = (), past_due: bool = None, in_class: bool = None, due_tomorrow: bool = None, due_in_week: bool = None):
 
         # name filter will get all assignments that include the string given. it is not case-sensitive and removes spaces and underscores.
         # grade filter is two numbers from 0+. example: '50-100' gets all assignments from 50 to 100. assignments with null grades are always filtered if this filter is set.
         # assignments_type filter. values can be 'extra credit', 'no value', or 'standard'. this is cleaned like the name filter. there are also more types than these 3.
         # category filter gets assignments with a certain category. this is cleaned and can match either the abbreviation or the full category name in order for the assignment to stay. categories dependent on class.
         # due filter gets assignments that match in between two dates. example: ('2023.4.1', '2023.5.1'). items in the tuple can also be 'now' for the current date.
         # assigned filter is the same as above, with assigned dates
@@ -372,23 +372,22 @@
                     try:
                         continue_ = not due[2]
                     except IndexError:
                         continue_ = True
 
                     if (assignment_due is None or assignment_due == '') and continue_:
                         elements.pop()
-                        print(1)
                         continue
+
                     elif (assignment_due is None or assignment_due == '') and not continue_:
-                        print(2)
                         pass
+
                     elif not utils.is_date_between(due[0], due[1], assignment_due):
 
                         elements.pop()
-                        print(3)
                         continue
 
                 # ASSIGNED ---------
                 try:
                     assignment_assigned = sections[5].text
                 except IndexError:
                     assignment_assigned = None
@@ -398,16 +397,18 @@
                         continue_ = not assigned[2]
                     except IndexError:
                         continue_ = True
 
                     if (assignment_assigned is None or assignment_assigned == '') and continue_:
                         elements.pop()
                         continue
+
                     elif (assignment_assigned is None or assignment_assigned == '') and not continue_:
                         pass
+
                     elif not utils.is_date_between(assigned[0], assigned[1], assignment_assigned):
 
                         elements.pop()
                         continue
 
                 elements[i]['name'] = assignment_name
                 elements[i]['link'] = f"https://igradeplus.com/student/{sections[0].contents[0].get('href')}"
@@ -459,26 +460,61 @@
 
                 if element == "\xa0":
                     elements[i]['grade']['value'] = None
 
                 else:
                     elements[i]['grade']['value'] = int(sections[10].text.split('.')[0])
 
-                elements[i]['details'] = {'past_due': utils.is_past(elements[i]['due'], 0)}
+                assignment_past_due = utils.is_past(elements[i]['due'], 0)
+
+                if past_due is not None:
+                    if assignment_past_due is not past_due:
+                        elements.pop()
+                        continue
+
+                elements[i]['details'] = {'past_due': assignment_past_due}
+
 
                 if elements[i]['grade']['points'] is None:
                     elements[i]['details']['graded'] = False
 
                 else:
                     elements[i]['details']['graded'] = True
 
                 elements[i]['details']['has_been_assigned'] = utils.is_past(elements[i]['assigned'], 0)
-                elements[i]['details']['in_class_assignment'] = elements[i]['due'] == elements[i]['assigned']
-                elements[i]['details']['due_tomorrow'] = utils.is_between(elements[i]['due'], 1)
-                elements[i]['details']['due_in_week'] = utils.is_between(elements[i]['due'], 8)
+
+
+                assignment_in_class = elements[i]['due'] == elements[i]['assigned']
+
+                if in_class is not None:
+                    if assignment_in_class is not in_class:
+                        elements.pop()
+                        continue
+
+                elements[i]['details']['in_class_assignment'] = assignment_in_class
+
+
+                assignment_due_tomorrow = utils.is_between(elements[i]['due'], 1)
+
+                if due_tomorrow is not None:
+                    if assignment_due_tomorrow is not due_tomorrow:
+                        elements.pop()
+                        continue
+
+                elements[i]['details']['due_tomorrow'] = assignment_due_tomorrow
+
+
+                assignment_due_in_week = utils.is_between(elements[i]['due'], 8)
+
+                if due_in_week is not None:
+                    if assignment_due_in_week is not due_in_week:
+                        elements.pop()
+                        continue
+
+                elements[i]['details']['due_in_week'] = assignment_due_in_week
 
 
                 if get_attachments:
 
                     links.append(elements[i]['link'])
 
                 i += 1
@@ -497,41 +533,42 @@
 
             self.__log('CLIENT', 'getting assignment page info.')
 
             for assignment in response:
 
                 elements[i]['attachments'] = assignment['attachments']
                 elements[i]['description'] = assignment['description']
+
                 elements[i]['supplemental_info'] = assignment['supplemental_info']
 
                 i += 1
 
         self.__log('CLIENT', 'data returned successfully.', 'green')
 
         return elements
 
-    def get_all_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def get_all_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = (), past_due: bool = None, in_class: bool = None, due_tomorrow: bool = None, due_in_week: bool = None):
 
         self.__verify()
-        return self.__get_assignments('all', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned)
+        return self.__get_assignments('all', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned, past_due=past_due, in_class=in_class, due_tomorrow=due_tomorrow, due_in_week=due_in_week)
 
-    def get_upcoming_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def get_upcoming_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = (), past_due: bool = None, in_class: bool = None, due_tomorrow: bool = None, due_in_week: bool = None):
 
         self.__verify()
-        return self.__get_assignments('upcoming', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned)
+        return self.__get_assignments('upcoming', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned, past_due=past_due, in_class=in_class, due_tomorrow=due_tomorrow, due_in_week=due_in_week)
 
-    def get_recent_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def get_recent_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = (), past_due: bool = None, in_class: bool = None, due_tomorrow: bool = None, due_in_week: bool = None):
 
         self.__verify()
-        return self.__get_assignments('recent', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned)
+        return self.__get_assignments('recent', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned, past_due=past_due, in_class=in_class, due_tomorrow=due_tomorrow, due_in_week=due_in_week)
 
-    def get_problematic_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = ()):
+    def get_problematic_assignments(self, get_attachments: bool = False, name='', grade=(), assignment_type: str = '', category: str = '', class_: str = '', due: tuple = (), assigned: tuple = (), past_due: bool = None, in_class: bool = None, due_tomorrow: bool = None, due_in_week: bool = None):
 
         self.__verify()
-        return self.__get_assignments('problematic', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned)
+        return self.__get_assignments('problematic', get_attachments=get_attachments, name=name, grade=grade, assignment_type=assignment_type, category=category, class_=class_, due=due, assigned=assigned, past_due=past_due, in_class=in_class, due_tomorrow=due_tomorrow, due_in_week=due_in_week)
 
     def get_account_info(self):
 
         self.__verify()
 
         soup = BeautifulSoup(self.session.get("https://igradeplus.com/student/myaccount").text, 'lxml')
 
@@ -768,15 +805,15 @@
         results = loop.run_until_complete(main())
         loop.close()
 
         response = results
 
         return response
 
-    def get_all_events(self):
+    def get_all_events(self, title: str = ''):
 
         self.__verify()
 
         html = self.session.get("https://igradeplus.com/student/communications/calendar").text
         pageid = html[31:67]
         targetid = BeautifulSoup(html, 'lxml').find('div', style='visibility: visible; position: relative; ').get('id')
 
@@ -800,29 +837,35 @@
         i = 0
         for section in soup.find_all('div', style="color: #000000; background: #FFFFFF; padding-top: 10.0px; padding-right: 50.0px; padding-bottom: 10.0px; padding-left: 5.0px; border-top-style: solid; border-top-color: #F0F0F0; border-top-width: 1.0px; "):
 
             day = section.find('a', style='font-size: 15px; font-weight: bold; color: #404040; text-decoration: none; line-height: 250%; ')
 
             for time in section.find_all('div')[::2]:
 
-                title = time.parent.next_sibling.next_sibling
+                title_html = time.parent.next_sibling.next_sibling
                 if time.text == 'All Day Event' or time.text == 'Time Not Specified':
                     start_time = 'All Day'
                     end_time = 'All Day'
 
                 else:
                     start_time = time.text.split('to')[0][:-2]
                     end_time = time.text.split('to')[1][2:]
-                elements.append({'title': title.text, 'link': f"https://igradeplus.com/student/communications/{title.find().get('href')}", 'id': title.find().get('href').split('?id=')[1], 'date': day.text, 'start_time': start_time, 'end_time': end_time})
+
+                event_title = title_html.text
+
+                if not re.search(utils.clean(title), utils.clean(event_title)):
+                    continue
+
+                elements.append({'title': event_title, 'link': f"https://igradeplus.com/student/communications/{title_html.find().get('href')}", 'id': title_html.find().get('href').split('?id=')[1], 'date': day.text, 'start_time': start_time, 'end_time': end_time})
 
             i += 1
 
         return elements
 
-    def get_upcoming_events(self):
+    def get_upcoming_events(self, title: str = '', text_includes: str = ''):
 
         self.__verify()
 
         html = self.session.get("https://igradeplus.com/student/communications/calendar").text
         pageid = html[31:67]
         targetid = BeautifulSoup(html, 'lxml').find('div', style='visibility: visible; position: relative; ').get('id')
 
@@ -843,15 +886,21 @@
         elements = []
         soup = BeautifulSoup(html, 'lxml')
 
         i = 0
         for section in soup.find_all('td', style='vertical-align: top; overflow: hidden; height: 100%; padding-top: 0.0px; padding-right: 0.0px; padding-bottom: 0.0px; padding-left: 0.0px; '):
             elements.append({})
 
-            elements[i]['title'] = section.find('span').text
+            event_title = section.find('span').text
+
+            if not re.search(utils.clean(title), utils.clean(event_title)):
+                elements.pop()
+                continue
+
+            elements[i]['title'] = event_title
             elements[i]['date'] = section.find('div', style='width: 250.0px; padding-right: 15.0px; ').text
 
             text = section.find('span', style='color: #000000; ').text
 
             if text == 'All Day':
                 elements[i]['start_time'] = 'All Day'
                 elements[i]['end_time'] = 'All Day'
@@ -865,26 +914,30 @@
             data = ''
             for item in element.children:
 
                 data += item.text + '\n\n'
 
             data = data[:-2]
 
+            if not re.search(utils.clean(text_includes), utils.clean(data)):
+                elements.pop()
+                continue
+
             elements[i]['content'] = {'text': data, 'html': element.prettify()}
 
             i += 1
 
         return elements
 
     def __get_pageid(self, url):
 
         # self.log('CLIENT', 'obtaining pageID')
         return self.session.get(url).text[31:67]
 
-    def get_announcements(self, get_link=False):
+    def get_announcements(self, get_link=False, title: str = '', author: str = '', text_includes: str = ''):
 
         self.__verify()
 
         if not get_link:
             pageid = self.__get_pageid('https://igradeplus.com/student/communications/bulletinboard')
 
             html = self.__send_ajax(pageid, '12', '30', return_=True)
@@ -894,25 +947,42 @@
             data = []
 
             i = 0
             for announcement in soup.find_all('td', style='vertical-align: top; overflow: hidden; height: 100%; padding-top: 0.0px; padding-right: 0.0px; padding-bottom: 0.0px; padding-left: 0.0px; '):
 
                 data.append({})
 
-                data[i]['title'] = announcement.find('div', style='font-size: 15px; line-height: 200%; font-weight: bold; color: #404040; ').text
+                announcement_title = announcement.find('div', style='font-size: 15px; line-height: 200%; font-weight: bold; color: #404040; ').text
+
+                if not re.search(utils.clean(title), utils.clean(announcement_title)):
+                    data.pop()
+                    continue
+
+                data[i]['title'] = announcement_title
                 data[i]['date'] = announcement.find('div', style='color: #808080; font-size: 13px; line-height: 180%; ').text
 
                 try:
-                    data[i]['author'] = announcement.find('div', style='color: #808080; font-size: 14px; line-height: 200%; ').text
+                    announcement_author = announcement.find('div', style='color: #808080; font-size: 14px; line-height: 200%; ').text
 
                 except AttributeError:
-                    data[i]['author'] = announcement.find('div', style='white-space: nowrap; text-overflow: ellipsis; color: #808080; font-size: 14px; line-height: 200%; ').text
+                    announcement_author = announcement.find('div', style='white-space: nowrap; text-overflow: ellipsis; color: #808080; font-size: 14px; line-height: 200%; ').text
+
+                if not re.search(utils.clean(author), utils.clean(announcement_author)):
+                    data.pop()
+                    continue
+
+                data[i]['author'] = announcement_author
 
+                announcement_text = announcement.find('div', attrs={'class': 'fr-view'}).text
+
+                if not re.search(utils.clean(text_includes), utils.clean(announcement_text)):
+                    data.pop()
+                    continue
 
-                data[i]['content'] = {'text': announcement.find('div', attrs={'class': 'fr-view'}).text, 'html': str(announcement.find('div', attrs={'class': 'fr-view'}).prettify()).replace('display: none; ', '')}
+                data[i]['content'] = {'text': announcement_text, 'html': str(announcement.find('div', attrs={'class': 'fr-view'}).prettify()).replace('display: none; ', '')}
 
                 i += 1
 
             return data
 
         else:
 
@@ -921,27 +991,40 @@
             data = []
 
             i = 0
             for announcement in soup.find_all('td', style='vertical-align: top; overflow: hidden; height: 100%; padding-top: 0.0px; padding-right: 0.0px; padding-bottom: 0.0px; padding-left: 0.0px; '):
 
                 data.append({})
 
-                data[i]['title'] = announcement.find('a').text
+                announcement_title = announcement.find('a').text
+
+                if not re.search(utils.clean(title), utils.clean(announcement_title)):
+                    data.pop()
+                    continue
+
+                data[i]['title'] = announcement_title
                 data[i]['link'] = announcement.find('a').get('href')
                 data[i]['id'] = announcement.find('a').get('href').split('?id=')[1]
                 data[i]['date'] = announcement.find('div', style='max-width: 100%; font-size: 14px; margin-left: 0.0px; line-height: 180%; font-weight: normal; color: #000000; white-space: nowrap; text-overflow: ellipsis; overflow: hidden; ').text
 
-                try:
-                    data[i]['author'] = announcement.find('div', style='max-width: 100%; font-size: 14px; margin-left: 0.0px; line-height: 180%; font-weight: normal; color: #000000; white-space: nowrap; text-overflow: ellipsis; overflow: hidden; ').text
+                announcement_author = announcement.find_all('div', style='max-width: 100%; font-size: 14px; margin-left: 0.0px; line-height: 180%; font-weight: normal; color: #000000; white-space: nowrap; text-overflow: ellipsis; overflow: hidden; ')[1].text
 
-                except AttributeError:
-                    data[i]['author'] = 'ERROR'
-                    # data[i]['author'] = announcement.find('div', style='white-space: nowrap; text-overflow: ellipsis; color: #808080; font-size: 14px; line-height: 200%; ').text
+                if not re.search(utils.clean(author), utils.clean(announcement_author)):
+                    data.pop()
+                    continue
+
+                data[i]['author'] = announcement_author
+
+                announcement_text = announcement.find('div', attrs={'class': 'fr-view'}).text
+
+                if not re.search(utils.clean(text_includes), utils.clean(announcement_text)):
+                    data.pop()
+                    continue
 
-                data[i]['content'] = {'text': announcement.find('div', attrs={'class': 'fr-view'}).text, 'html': str(announcement.find('div', attrs={'class': 'fr-view'}).prettify())}
+                data[i]['content'] = {'text': announcement_text, 'html': str(announcement.find('div', attrs={'class': 'fr-view'}).prettify())}
 
                 i += 1
 
             return data
 
     def get_announcement_content(self, announcement_id, html=True):
```

### Comparing `igrade-2.5.2/igrade/utils.py` & `igrade-2.6.0/igrade/utils.py`

 * *Files identical despite different names*

### Comparing `igrade-2.5.2/igrade.egg-info/PKG-INFO` & `igrade-2.6.0/igrade.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igrade
-Version: 2.5.2
+Version: 2.6.0
 Summary: An unofficial wrapper for iGradePlus Student Management Systems.
 Home-page: https://github.com/Kasherpete/Igrade-web-scraper
 Author: Keagan Peterson
 Author-email: Keagan.a.peterson@outlook.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `igrade-2.5.2/setup.py` & `igrade-2.6.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 # Package metadata
 NAME = 'igrade'
-VERSION = '2.5.2'
+VERSION = '2.6.0'
 DESCRIPTION = 'An unofficial wrapper for iGradePlus Student Management Systems.'
 URL = 'https://github.com/Kasherpete/Igrade-web-scraper'
 AUTHOR = 'Keagan Peterson'
 AUTHOR_EMAIL = 'Keagan.a.peterson@outlook.com'
 LICENSE = 'MIT'
 LICENSE_URL = 'https://opensource.org/licenses/MIT'
 
 # Package dependencies
 INSTALL_REQUIRES = [
-    'aiohttp>=2.1.4',
-    'requests>=2.1.1',
-    'beautifulsoup4>=3.12.2',
+    'aiohttp>=3.0.0',
+    'requests>=2.0.0',
+    'beautifulsoup4>=4.0.0',
     'colorama>=0.2.0',
-    'lxml>=3.0.0',
+    'lxml>=4.0.0',
 ]
 
 # Additional classifiers
 CLASSIFIERS = [
     'Intended Audience :: Developers',
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: MIT License',
```

