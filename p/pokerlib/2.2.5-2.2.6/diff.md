# Comparing `tmp/pokerlib-2.2.5.tar.gz` & `tmp/pokerlib-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerlib-2.2.5.tar", max compression
+gzip compressed data, was "pokerlib-2.2.6.tar", max compression
```

## Comparing `pokerlib-2.2.5.tar` & `pokerlib-2.2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.5/LICENSE
--rw-r--r--   0        0        0     5980 2023-05-05 21:16:26.697525 pokerlib-2.2.5/README.md
--rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.5/pokerlib/__init__.py
--rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/_handparser.py
--rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/_player.py
--rw-r--r--   0        0        0    18193 2023-05-10 20:45:00.132337 pokerlib-2.2.5/pokerlib/_round.py
--rw-r--r--   0        0        0     6937 2023-05-08 12:36:12.798296 pokerlib-2.2.5/pokerlib/_table.py
--rw-r--r--   0        0        0     1652 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/enums.py
--rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/implementations/__init__.py
--rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/implementations/_no_muck_showdown_table.py
--rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.5/pokerlib/implementations/_no_muck_table.py
--rw-r--r--   0        0        0      663 2023-05-10 20:45:42.772328 pokerlib-2.2.5/pyproject.toml
--rw-r--r--   0        0        0     6705 1970-01-01 00:00:00.000000 pokerlib-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35147 2022-10-03 17:39:48.345471 pokerlib-2.2.6/LICENSE
+-rw-r--r--   0        0        0     5956 2023-05-11 15:49:26.693822 pokerlib-2.2.6/README.md
+-rw-r--r--   0        0        0      493 2023-04-24 16:14:50.939071 pokerlib-2.2.6/pokerlib/__init__.py
+-rw-r--r--   0        0        0     9058 2023-05-02 19:42:16.761493 pokerlib-2.2.6/pokerlib/_handparser.py
+-rw-r--r--   0        0        0     5387 2023-05-02 19:42:16.761493 pokerlib-2.2.6/pokerlib/_player.py
+-rw-r--r--   0        0        0    18193 2023-05-10 20:45:00.132337 pokerlib-2.2.6/pokerlib/_round.py
+-rw-r--r--   0        0        0     7735 2023-06-04 12:28:13.322689 pokerlib-2.2.6/pokerlib/_table.py
+-rw-r--r--   0        0        0     1704 2023-06-04 12:22:36.782775 pokerlib-2.2.6/pokerlib/enums.py
+-rw-r--r--   0        0        0      130 2023-05-02 19:42:16.761493 pokerlib-2.2.6/pokerlib/implementations/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-02 19:42:16.761493 pokerlib-2.2.6/pokerlib/implementations/_no_muck_showdown_table.py
+-rw-r--r--   0        0        0      360 2023-05-02 19:42:16.761493 pokerlib-2.2.6/pokerlib/implementations/_no_muck_table.py
+-rw-r--r--   0        0        0      663 2023-06-04 12:29:09.562674 pokerlib-2.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6681 1970-01-01 00:00:00.000000 pokerlib-2.2.6/PKG-INFO
```

### Comparing `pokerlib-2.2.5/LICENSE` & `pokerlib-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.5/README.md` & `pokerlib-2.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,18 @@
     def publicOut(self, out_id, **kwargs):
         print(out_id, kwargs)
     def privateOut(self, player_id, out_id, **kwargs):
         print(out_id, kwargs)
 
 # define a new table
 table = MyTable(
-    table_id = 0
-    seats = PlayerSeats([None] * 9)
-    buyin = 100
-    small_blind = 5
+    table_id = 0,
+    seats = PlayerSeats([None] * 9),
+    buyin = 100,
+    small_blind = 5,
     big_blind = 10
 )
 ```
 
 We could have seated players on the `seats` inside `MyTable` constructor,
 but let's add them to the defined table.
 
@@ -152,15 +152,14 @@
 python tests/handparser_reactive.py
 ```
 and `Round` with
 ```bash
 python tests/round_test.py
 ```
 Note that HandParser can be fuzz tested against another poker library [pokerface](https://github.com/AussieSeaweed/pokerface) with
-Those tests can be run with
 ```bash
 python tests/handparser_against_pokerface.py
 ```
 which means it is considered safe. On the other hand, `Table` may still have some bugs.
 
 ## License
 GNU General Public License v3.0
```

### Comparing `pokerlib-2.2.5/pokerlib/_handparser.py` & `pokerlib-2.2.6/pokerlib/_handparser.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.5/pokerlib/_player.py` & `pokerlib-2.2.6/pokerlib/_player.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.5/pokerlib/_round.py` & `pokerlib-2.2.6/pokerlib/_round.py`

 * *Files identical despite different names*

### Comparing `pokerlib-2.2.5/pokerlib/_table.py` & `pokerlib-2.2.6/pokerlib/_table.py`

 * *Files 12% similar despite different names*

```diff
@@ -158,19 +158,38 @@
         self._kickoutLosers()
         if player.money < self.buyin: self.privateOut(
             player.id, self.PrivateOutId.BUYINTOOLOW,
             table_id=self.id)
         elif self.nplayers >= self.nseats: self.privateOut(
             player.id, self.PrivateOutId.TABLEFULL,
             table_id=self.id)
-        elif player in self: self.privateOut(
+        elif player in self.seats: self.privateOut(
             player.id, self.PrivateOutId.PLAYERALREADYATTABLE,
             table_id=self.id)
         else: super()._addPlayer(player)
 
+    def _addPlayerOnSeat(self, player, index):
+        self._kickoutLosers()
+        if player.money < self.buyin: self.privateOut(
+            player.id, self.PrivateOutId.BUYINTOOLOW,
+            table_id=self.id)
+        elif not (0 <= index < self.nseats) or self.seats[index] is not None:
+            self.privateOut(player.id, self.PrivateOutId.INCORRECTSEATINDEX)
+        elif player in self.seats: self.privateOut(
+            player.id, self.PrivateOutId.PLAYERALREADYATTABLE,
+            table_id=self.id)
+        else: super()._addPlayerOnSeat(player, index)
+
+    def _removePlayerById(self, player_id):
+        player = self.seats.getPlayerById(player_id)
+        if player is None: self.privateOut(
+            player_id, self.PrivateOutId.PLAYERNOTATTABLE,
+            table_id=self.id)
+        else: super()._removePlayer(player)
+
     def _startRound(self, round_id):
         if self.round: self.publicOut(
             self.PublicOutId.ROUNDINPROGRESS,
             round_id=round_id, table_id=self.id)
         elif not self: self.publicOut(
             self.PublicOutId.INCORRECTNUMBEROFPLAYERS,
             round_id=round_id, table_id=self.id)
@@ -201,16 +220,15 @@
                 self.PublicOutId.ROUNDNOTINITIALIZED)
             else: self.round.publicIn(player_id, action, **kwargs)
 
         elif action in self.PublicInId:
             if action is self.PublicInId.STARTROUND:
                 self._startRound(kwargs.get('round_id'))
             elif action is self.PublicInId.LEAVETABLE:
-                player = self.seats.getPlayerById(player_id)
-                self._removePlayer(player)
+                self._removePlayerById(player_id)
             elif action is self.PublicInId.BUYIN:
                 if 'index' in kwargs:
                     self._addPlayerOnSeat(kwargs['player'], kwargs['index'])
                 else:
                     self._addPlayer(kwargs['player'])
 
         # has to be done after every publicIn call
```

### Comparing `pokerlib-2.2.5/pokerlib/enums.py` & `pokerlib-2.2.6/pokerlib/enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,7 +86,9 @@
     ROUNDINPROGRESS = 4
     INCORRECTNUMBEROFPLAYERS = 5
 
 class TablePrivateOutId(IntEnum):
     BUYINTOOLOW = 1
     TABLEFULL = 2
     PLAYERALREADYATTABLE = 3
+    PLAYERNOTATTABLE = 4
+    INCORRECTSEATINDEX = 5
```

### Comparing `pokerlib-2.2.5/pyproject.toml` & `pokerlib-2.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pokerlib"
-version = "2.2.5"
+version = "2.2.6"
 description = "Python poker library"
 repository = "https://github.com/kuco23/pokerlib/"
 authors = ["kuco23 <nseverkar@gmail.com>"]
 keywords = ['python', 'poker', 'library']
 readme = "README.md"
 classifiers=  [
     'Development Status :: 3 - Alpha',
```

### Comparing `pokerlib-2.2.5/PKG-INFO` & `pokerlib-2.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerlib
-Version: 2.2.5
+Version: 2.2.6
 Summary: Python poker library
 Home-page: https://github.com/kuco23/pokerlib/
 Keywords: python,poker,library
 Author: kuco23
 Author-email: nseverkar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -104,18 +104,18 @@
     def publicOut(self, out_id, **kwargs):
         print(out_id, kwargs)
     def privateOut(self, player_id, out_id, **kwargs):
         print(out_id, kwargs)
 
 # define a new table
 table = MyTable(
-    table_id = 0
-    seats = PlayerSeats([None] * 9)
-    buyin = 100
-    small_blind = 5
+    table_id = 0,
+    seats = PlayerSeats([None] * 9),
+    buyin = 100,
+    small_blind = 5,
     big_blind = 10
 )
 ```
 
 We could have seated players on the `seats` inside `MyTable` constructor,
 but let's add them to the defined table.
 
@@ -172,15 +172,14 @@
 python tests/handparser_reactive.py
 ```
 and `Round` with
 ```bash
 python tests/round_test.py
 ```
 Note that HandParser can be fuzz tested against another poker library [pokerface](https://github.com/AussieSeaweed/pokerface) with
-Those tests can be run with
 ```bash
 python tests/handparser_against_pokerface.py
 ```
 which means it is considered safe. On the other hand, `Table` may still have some bugs.
 
 ## License
 GNU General Public License v3.0
```

