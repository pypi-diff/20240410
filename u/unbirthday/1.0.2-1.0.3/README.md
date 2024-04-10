# Comparing `tmp/unbirthday-1.0.2.tar.gz` & `tmp/unbirthday-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unbirthday-1.0.2.tar", last modified: Tue Apr  9 07:24:04 2024, max compression
+gzip compressed data, was "unbirthday-1.0.3.tar", last modified: Wed Apr 10 02:19:26 2024, max compression
```

## Comparing `unbirthday-1.0.2.tar` & `unbirthday-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 07:24:04.283450 unbirthday-1.0.2/
--rw-rw-rw-   0        0        0     8141 2024-04-09 07:24:04.283450 unbirthday-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7876 2024-04-09 07:05:19.000000 unbirthday-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-09 07:24:04.283450 unbirthday-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      521 2024-04-09 07:22:48.000000 unbirthday-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:24:04.283450 unbirthday-1.0.2/unbirthday/
--rw-rw-rw-   0        0        0      177 2024-04-09 06:02:18.000000 unbirthday-1.0.2/unbirthday/__init__.py
--rw-rw-rw-   0        0        0     6346 2024-04-05 22:59:31.000000 unbirthday-1.0.2/unbirthday/unbirthday.py
-drwxrwxrwx   0        0        0        0 2024-04-09 07:24:04.283450 unbirthday-1.0.2/unbirthday.egg-info/
--rw-rw-rw-   0        0        0     8141 2024-04-09 07:24:04.000000 unbirthday-1.0.2/unbirthday.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-09 07:24:04.000000 unbirthday-1.0.2/unbirthday.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 07:24:04.000000 unbirthday-1.0.2/unbirthday.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-09 07:24:04.000000 unbirthday-1.0.2/unbirthday.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-10 02:19:26.560007 unbirthday-1.0.3/
+-rw-rw-rw-   0        0        0     8141 2024-04-10 02:19:26.560007 unbirthday-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7876 2024-04-09 07:05:19.000000 unbirthday-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-10 02:19:26.560007 unbirthday-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      521 2024-04-10 02:15:33.000000 unbirthday-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:19:26.544382 unbirthday-1.0.3/unbirthday/
+-rw-rw-rw-   0        0        0      177 2024-04-09 06:02:18.000000 unbirthday-1.0.3/unbirthday/__init__.py
+-rw-rw-rw-   0        0        0     6909 2024-04-10 02:12:03.000000 unbirthday-1.0.3/unbirthday/unbirthday.py
+drwxrwxrwx   0        0        0        0 2024-04-10 02:19:26.560007 unbirthday-1.0.3/unbirthday.egg-info/
+-rw-rw-rw-   0        0        0     8141 2024-04-10 02:19:26.000000 unbirthday-1.0.3/unbirthday.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-10 02:19:26.000000 unbirthday-1.0.3/unbirthday.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-10 02:19:26.000000 unbirthday-1.0.3/unbirthday.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-10 02:19:26.000000 unbirthday-1.0.3/unbirthday.egg-info/top_level.txt
```

### Comparing `unbirthday-1.0.2/PKG-INFO` & `unbirthday-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbirthday
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unbirthday is a Python module that provides functions to calculate and manage "unbirthdays," which are days celebrated as not being a person's birthday.
 Description-Content-Type: text/markdown
 
 # Unbirthday (Calculator)
 
 ## Introduction
```

### Comparing `unbirthday-1.0.2/README.md` & `unbirthday-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `unbirthday-1.0.2/setup.py` & `unbirthday-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="unbirthday",
-    version="1.0.2",
+    version="1.0.3",
     description="Unbirthday is a Python module that provides functions to calculate and manage \"unbirthdays,\" which are days celebrated as not being a person's birthday.",
     packages=find_packages(),
     install_requires=[
         #no packages needed
     ],
     long_description=description,
     long_description_content_type="text/markdown",
```

### Comparing `unbirthday-1.0.2/unbirthday/unbirthday.py` & `unbirthday-1.0.3/unbirthday/unbirthday.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from datetime import datetime, timedelta
 import math
 
 def add_ordinal_indicator(num):
+    '''Adds the ordinal indicator (e.g., "st", "nd", "rd", "th") to a given number.'''
     if 10 <= num % 100 <= 20:
         suffix = 'th'
     else:
         suffix = {1: 'st', 2: 'nd', 3: 'rd'}.get(num % 10, 'th')
     return str(num) + suffix
 
 def get_todays_date():
+    '''Gets the current date in the format "YYYY-MM-DD".'''
     return datetime.today().strftime('%Y-%m-%d')
 
 def is_leap_year(year):
     return year % 4 == 0 and (year % 100 != 0 or year % 400 == 0)
 
 def years_passed(start_date, end_date=None):
+    '''Calculates the number of years passed between two dates.'''
     if end_date == None:
         end_date = get_todays_date()
 
     start_year, start_month, start_day = map(int, start_date.split('-'))
     end_year, end_month, end_day = map(int, end_date.split('-'))
     
     # Calculate the years difference
@@ -33,14 +36,15 @@
             # If start_date is Feb 29th of a leap year, check if end_date's year is a leap year
             if not is_leap_year(end_year):
                 years_diff -= 1
     
     return years_diff
 
 def your_current_day_on_earth(start_date, end_date=None):
+    '''Calculates the number of days between two dates.'''
     if end_date == None:
         end_date = get_todays_date()
 
     # Convert the string dates to datetime objects
     d1 = datetime.strptime(start_date, "%Y-%m-%d")
     d2 = datetime.strptime(end_date, "%Y-%m-%d")
     
@@ -48,14 +52,15 @@
     delta = abs(d2 - d1).days + 1
 
     # Return the difference in days
     return delta
 
 
 def calculate_unbirthday(start_date, end_date=None):
+    '''Calculates the current unbirthday based on the provided start and end dates.'''
     if end_date == None:
         end_date = get_todays_date()
 
     # How to calculate unbirthdays
 
     # 1. Take your current day on earth
     # 2. Subtract 1 day because the day you were born counts as a birthday
@@ -110,14 +115,15 @@
     # Calculate the new date by subtracting the days
     new_date = current_date - timedelta(days=days)
     
     # Convert the new date back to a string and return it
     return new_date.strftime(date_format)
 
 def find_startdate_unbirthday(unbirthday, end_date=None):
+    '''Calculates the start date (birth date) based on the provided unbirthday and end dates.'''
     if end_date == None:
         end_date = get_todays_date()
     
     # Assume how many birthdays has passed based on the amount of unbirthdays
     birthdays = unbirthday_enddate_to_years(unbirthday, end_date)
 
     # To reverse the unbirthday:
@@ -166,14 +172,15 @@
     # Calculate the new date by adding the days
     new_date = current_date + timedelta(days=days)
     
     # Convert the new date back to a string and return it
     return new_date.strftime(date_format)
 
 def find_enddate_unbirthday(unbirthday, start_date):
+    '''Calculates the end date (current date) based on the provided unbirthday and start dates.'''
     # Assume how many birthdays will pass based on the amount of unbirthdays
     birthdays = unbirthday_startdate_to_years(unbirthday, start_date)
 
     # To reverse the unbirthday:
     # Add one because the day you were born
     reverse_your_current_day_on_earth = unbirthday + 1
```

### Comparing `unbirthday-1.0.2/unbirthday.egg-info/PKG-INFO` & `unbirthday-1.0.3/unbirthday.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unbirthday
-Version: 1.0.2
+Version: 1.0.3
 Summary: Unbirthday is a Python module that provides functions to calculate and manage "unbirthdays," which are days celebrated as not being a person's birthday.
 Description-Content-Type: text/markdown
 
 # Unbirthday (Calculator)
 
 ## Introduction
```

