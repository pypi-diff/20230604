# Comparing `tmp/calendar_pytba-1.0.2.tar.gz` & `tmp/calendar_pytba-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calendar_pytba-1.0.2.tar", max compression
+gzip compressed data, was "calendar_pytba-1.1.0.tar", max compression
```

## Comparing `calendar_pytba-1.0.2.tar` & `calendar_pytba-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/LICENSE
--rw-r--r--   0        0        0       41 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/__init__.py
--rw-r--r--   0        0        0     6995 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/main.py
--rw-r--r--   0        0        0        0 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/utils/__init__.py
--rw-r--r--   0        0        0     3944 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/utils/handler.py
--rw-r--r--   0        0        0     2315 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/utils/text.py
--rw-r--r--   0        0        0      444 2023-06-03 09:27:36.475600 calendar_pytba-1.0.2/calendar_pytba/utils/types.py
--rw-r--r--   0        0        0      373 2023-06-03 09:27:36.495600 calendar_pytba-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      662 2023-06-03 09:27:36.495600 calendar_pytba-1.0.2/readme.md
--rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 calendar_pytba-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-04 12:26:05.940961 calendar_pytba-1.1.0/LICENSE
+-rw-r--r--   0        0        0       41 2023-06-04 12:26:05.940961 calendar_pytba-1.1.0/calendar_pytba/__init__.py
+-rw-r--r--   0        0        0     7806 2023-06-04 12:26:05.940961 calendar_pytba-1.1.0/calendar_pytba/main.py
+-rw-r--r--   0        0        0        0 2023-06-04 12:26:05.940961 calendar_pytba-1.1.0/calendar_pytba/utils/__init__.py
+-rw-r--r--   0        0        0     4533 2023-06-04 12:26:05.940961 calendar_pytba-1.1.0/calendar_pytba/utils/handler.py
+-rw-r--r--   0        0        0     2958 2023-06-04 12:26:05.940961 calendar_pytba-1.1.0/calendar_pytba/utils/text.py
+-rw-r--r--   0        0        0      550 2023-06-04 12:26:05.940961 calendar_pytba-1.1.0/calendar_pytba/utils/types.py
+-rw-r--r--   0        0        0      374 2023-06-04 12:26:05.960961 calendar_pytba-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1211 2023-06-04 12:26:05.960961 calendar_pytba-1.1.0/readme.md
+-rw-r--r--   0        0        0     1755 1970-01-01 00:00:00.000000 calendar_pytba-1.1.0/PKG-INFO
```

### Comparing `calendar_pytba-1.0.2/LICENSE` & `calendar_pytba-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calendar_pytba-1.0.2/calendar_pytba/main.py` & `calendar_pytba-1.1.0/calendar_pytba/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 import calendar
 import datetime
 
 from dateutil.relativedelta import relativedelta
 from telebot import types  # noqa
 
 from calendar_pytba.utils import text
-from calendar_pytba.utils.types import CalendarLanguage, CallBackData
+from calendar_pytba.utils.types import CalendarLanguage, CalendarSymbol, CallBackData
 
 
 class Calendar:
     def __init__(
         self,
         language: str = CalendarLanguage.EN,
-        empty_day_symbol: str = " ",
-        next_page_symbol: str = "→",
-        previous_page_symbol: str = "←",
+        empty_day_symbol: str = CalendarSymbol.EMPTY_DAY,
+        next_page_symbol: str = CalendarSymbol.NEXT_PAGE,
+        previous_page_symbol: str = CalendarSymbol.PREVIOUS_PAGE,
         month_names: dict = text.MONTH_NAMES,
         week_days_names: dict = text.WEEK_DAYS_NAMES,
         week_days_short_names: dict = text.WEEK_DAYS_SHORT_NAMES,
+        start_from_sunday: bool = False,
     ):
         """
         The language is responsible for writing the names of the months,
         days of the week, and other elements of the calendar.
         You can pass the language value as a string, see available
         languages in calendar_pytba.utils.types.CalendarLanguage
         :param language: str, CalendarLanguage class attribute
         :param empty_day_symbol: str, character to be displayed on days of the week where there are no numbers
         :param next_page_symbol: str, scroll forward button symbol
         :param previous_page_symbol: str, scroll backward button symbol
         :param month_names: dict, dictionary with the names of the months
         :param week_days_names: dict, dictionary with the names of the weekdays
         :param week_days_short_names: dict, dictionary with the short names of the weekdays
+        :param start_from_sunday: bool, In the US, UK and Israel, the calendar week can start on Sunday.
+               By default, the week starts on Monday
         """
         self.language = language
         self.markup: types.InlineKeyboardMarkup = types.InlineKeyboardMarkup(
             row_width=7
         )
         self.empty_day_symbol = empty_day_symbol
         self.next_page_symbol = next_page_symbol
         self.previous_page_symbol = previous_page_symbol
         self.month_names = month_names
         self.week_days_names = week_days_names
         self.week_days_short_names = week_days_short_names
+        self.start_from_sunday = start_from_sunday
 
     def _get_month_name(self, month: int) -> str:
         return self.month_names.get(self.language).get(month)
 
     def _add_headline(self, date: datetime.date):
         self.markup.add(
             types.InlineKeyboardButton(
@@ -54,27 +58,39 @@
             ),
             types.InlineKeyboardButton(
                 date.year,
                 callback_data=f"{CallBackData.LIST_YEARS}:{date.month}:{date.year}",
             ),
         )
 
+    def _reorder_weekdays_from_sunday(self) -> dict:
+        weekdays: dict = self.week_days_short_names.get(self.language)
+        last_item = dict([list(weekdays.items())[-1]])
+        weekdays = dict(list(weekdays.items())[:-1])
+        weekdays = {**last_item, **weekdays}
+        return weekdays
+
     def _add_weekdays_line(self):
-        weekdays = self.week_days_short_names.get(self.language)
+        if self.start_from_sunday:
+            weekdays = self._reorder_weekdays_from_sunday()
+        else:
+            weekdays = self.week_days_short_names.get(self.language)
         buttons = [
             types.InlineKeyboardButton(
                 weekdays.get(weekday),
                 callback_data=f"{CallBackData.FULL_WEEKDAY_NAME}:{weekday}",
             )
             for weekday in weekdays
         ]
         self.markup.add(*buttons)
 
     def _add_weeks(self, date: datetime.date):
         start_week_day, days_in_month = calendar.monthrange(date.year, date.month)
+        if self.start_from_sunday:
+            start_week_day += 1
         week = []
         empty_day = types.InlineKeyboardButton(
             self.empty_day_symbol, callback_data=CallBackData.EMPTY_WEEKDAY
         )
         for _ in range(start_week_day):
             week.append(empty_day)
         for day in range(days_in_month):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `calendar_pytba-1.0.2/calendar_pytba/utils/handler.py` & `calendar_pytba-1.1.0/calendar_pytba/utils/handler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 import datetime
 
 from telebot import TeleBot, types
 
 from calendar_pytba import Calendar
 from calendar_pytba.utils import text
-from calendar_pytba.utils.types import CalendarLanguage, CallBackData
+from calendar_pytba.utils.types import CalendarLanguage, CalendarSymbol, CallBackData
 
 
 def _extract_month_year(data: str) -> list:
     return [int(_) for _ in data.split(":")[1:3]]
 
 
-def callback_handler(bot: TeleBot, language: str = CalendarLanguage.EN):
-    calendar = Calendar(language)
+def callback_handler(
+    bot: TeleBot,
+    language: str = CalendarLanguage.EN,
+    empty_day_symbol: str = CalendarSymbol.EMPTY_DAY,
+    next_page_symbol: str = CalendarSymbol.NEXT_PAGE,
+    previous_page_symbol: str = CalendarSymbol.PREVIOUS_PAGE,
+    month_names: dict = text.MONTH_NAMES,
+    week_days_names: dict = text.WEEK_DAYS_NAMES,
+    week_days_short_names: dict = text.WEEK_DAYS_SHORT_NAMES,
+    start_from_sunday: bool = False,
+):
+    calendar = Calendar(
+        language,
+        empty_day_symbol,
+        next_page_symbol,
+        previous_page_symbol,
+        month_names,
+        week_days_names,
+        week_days_short_names,
+        start_from_sunday,
+    )
 
     @bot.callback_query_handler(
         func=lambda call: call.data.startswith(CallBackData.LIST_MONTHS)
     )
     def list_months_call(call: types.CallbackQuery) -> None:
         year = int(call.data.split(":")[1])
         markup = calendar.get_list_months(year)
```

### Comparing `calendar_pytba-1.0.2/calendar_pytba/utils/text.py` & `calendar_pytba-1.1.0/calendar_pytba/utils/text.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,14 +39,28 @@
         7: "Липень",
         8: "Серпень",
         9: "Вересень",
         10: "Жовтень",
         11: "Листопад",
         12: "Грудень",
     },
+    CalendarLanguage.ES: {
+        1: "Enero",
+        2: "Febrero",
+        3: "Marzo",
+        4: "Abril",
+        5: "Mayo",
+        6: "Junio",
+        7: "Julio",
+        8: "Agosto",
+        9: "Septiembre",
+        10: "Octubre",
+        11: "Noviembre",
+        12: "Diciembre",
+    },
 }
 
 WEEK_DAYS_NAMES = {
     CalendarLanguage.EN: {
         0: "Monday",
         1: "Tuesday",
         2: "Wednesday",
@@ -69,14 +83,23 @@
         1: "Вівторок",
         2: "Середа",
         3: "Четвер",
         4: "П'ятниця",
         5: "Субота",
         6: "Неділя",
     },
+    CalendarLanguage.ES: {
+        0: "Lunes",
+        1: "Martes",
+        2: "Miércoles",
+        3: "Jueves",
+        4: "Viernes",
+        5: "Sábado",
+        6: "Domingo",
+    },
 }
 
 WEEK_DAYS_SHORT_NAMES = {
     CalendarLanguage.EN: {
         0: "MO",
         1: "TU",
         2: "WE",
@@ -99,8 +122,17 @@
         1: "ВТ",
         2: "СР",
         3: "ЧТ",
         4: "ПТ",
         5: "СБ",
         6: "НД",
     },
+    CalendarLanguage.ES: {
+        0: "Lun",
+        1: "Mar",
+        2: "Mié",
+        3: "Jue",
+        4: "Vie",
+        5: "Sáb",
+        6: "Dom",
+    },
 }
```

