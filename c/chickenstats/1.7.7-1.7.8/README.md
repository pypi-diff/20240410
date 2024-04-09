# Comparing `tmp/chickenstats-1.7.7.tar.gz` & `tmp/chickenstats-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chickenstats-1.7.7.tar", max compression
+gzip compressed data, was "chickenstats-1.7.8.tar", max compression
```

## Comparing `chickenstats-1.7.7.tar` & `chickenstats-1.7.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35129 2023-12-31 06:32:21.486921 chickenstats-1.7.7/LICENSE
--rw-r--r--   0        0        0     5846 2023-12-31 06:32:21.486921 chickenstats-1.7.7/README.md
--rw-r--r--   0        0        0       63 2023-12-31 06:32:21.490921 chickenstats-1.7.7/chickenstats/capfriendly/__init__.py
--rw-r--r--   0        0        0    15362 2023-12-31 06:32:21.490921 chickenstats-1.7.7/chickenstats/capfriendly/scrape.py
--rw-r--r--   0        0        0       66 2023-12-31 06:32:21.490921 chickenstats-1.7.7/chickenstats/chicken_nhl/__init__.py
--rw-r--r--   0        0        0    21790 2023-12-31 06:32:21.490921 chickenstats-1.7.7/chickenstats/chicken_nhl/fixes.py
--rw-r--r--   0        0        0     4157 2023-12-31 06:32:21.490921 chickenstats-1.7.7/chickenstats/chicken_nhl/helpers.py
--rw-r--r--   0        0        0     8594 2023-12-31 06:32:21.490921 chickenstats-1.7.7/chickenstats/chicken_nhl/info.py
--rw-r--r--   0        0        0   203654 2023-12-31 06:32:21.490921 chickenstats-1.7.7/chickenstats/chicken_nhl/scrape.py
--rw-r--r--   0        0        0      141 2023-12-31 06:32:21.494921 chickenstats-1.7.7/chickenstats/evolving_hockey/__init__.py
--rw-r--r--   0        0        0    96724 2023-12-31 06:32:21.494921 chickenstats-1.7.7/chickenstats/evolving_hockey/base.py
--rw-r--r--   0        0        0    71851 2023-12-31 06:32:21.494921 chickenstats-1.7.7/chickenstats/evolving_hockey/stats.py
--rw-r--r--   0        0        0     1553 2023-12-31 06:32:21.554921 chickenstats-1.7.7/pyproject.toml
--rw-r--r--   0        0        0     7124 1970-01-01 00:00:00.000000 chickenstats-1.7.7/PKG-INFO
+-rw-r--r--   0        0        0    35129 2024-04-09 22:57:36.346373 chickenstats-1.7.8/LICENSE
+-rw-r--r--   0        0        0     5450 2024-04-09 22:57:36.346373 chickenstats-1.7.8/README.md
+-rw-r--r--   0        0        0       63 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/capfriendly/__init__.py
+-rw-r--r--   0        0        0    15617 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/capfriendly/scrape.py
+-rw-r--r--   0        0        0       66 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/chicken_nhl/__init__.py
+-rw-r--r--   0        0        0    21790 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/chicken_nhl/fixes.py
+-rw-r--r--   0        0        0     5070 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/chicken_nhl/helpers.py
+-rw-r--r--   0        0        0     8594 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/chicken_nhl/info.py
+-rw-r--r--   0        0        0   313483 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/chicken_nhl/scrape.py
+-rw-r--r--   0        0        0    18230 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/chicken_nhl/validation.py
+-rw-r--r--   0        0        0      141 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/evolving_hockey/__init__.py
+-rw-r--r--   0        0        0    96852 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/evolving_hockey/base.py
+-rw-r--r--   0        0        0    81228 2024-04-09 22:57:36.350373 chickenstats-1.7.8/chickenstats/evolving_hockey/stats.py
+-rw-r--r--   0        0        0     1573 2024-04-09 22:57:36.410373 chickenstats-1.7.8/pyproject.toml
+-rw-r--r--   0        0        0     6769 1970-01-01 00:00:00.000000 chickenstats-1.7.8/PKG-INFO
```

### Comparing `chickenstats-1.7.7/LICENSE` & `chickenstats-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chickenstats-1.7.7/README.md` & `chickenstats-1.7.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -13,51 +13,54 @@
 
 </div>
 
 ---
 
 ## About
 
-`chickenstats` is a Python package for scraping & analyzing sports statistics. With just a few lines of code:
-* **Scrape & manipulate** data from various NHL endpoints, leveraging a **proprietary xG model**
-for shot quality metrics
+`chickenstats` is a Python package for scraping & analyzing sports data. With just a few lines of code:
+* **Scrape & manipulate** data from various NHL endpoints, leveraging `chickenstats.chicken_nhl`, which includes
+a **proprietary xG model** for shot quality metrics
 * **Augment play-by-play data** & **generate custom aggregations** from raw csv files downloaded from
-[Evolving-Hockey](https://evolving-hockey.com) (subscription required)
-* Download **salary** & other **contract information** for **individual skaters & goalies** programmatically
-from [CapFriendly](https://capfriendly.com)
+[Evolving-Hockey](https://evolving-hockey.com) *(subscription required)* with `chickenstats.evolving_hockey`
 
 For more in-depth explanations, tutorials, & detailed reference materials, consult the
 [**Documentation**](https://chickenstats.com). 
 
 ---
 
 ## Compatibility
 
-`chickenstats` requires Python 3.10 or greater & runs on the latest stable versions Linux, MacOS, & Windows
+`chickenstats` requires Python 3.10 or greater & runs on the latest stable versions of Linux, MacOS, & Windows
 operating systems.
 
 ---
 
 ## Installation
 
 Very simple - install using PyPi. Best practice is to develop in an isolated virtual environment (conda or otherwise),
 but who's a chicken to judge?
 
 ```sh
 pip install chickenstats
 ```
 
+To confirm installation & confirm the latest version (1.7.8):
+
+```sh
+pip show chickenstats
+```
+
 ---
 
 ## Usage
 
 `chickenstats` is structured as three underlying modules, each used with different data sources:
 * `chickenstats.chicken_nhl`
 * `chickenstats.evolving_hockey`
-* `chickenstats.capfriendly`
 
 The package is under active development - features will be added or modified in the coming weeks & months. 
 
 ### chicken_nhl
 
 The `chickenstats.chicken_nhl` module scrapes & manipulates data directly from various NHL endpoints,
 with outputs including schedule & game results, rosters, & play-by-play data. 
@@ -107,26 +110,14 @@
 # accounting for teammates & opposition on-ice
 individual_game = prep_stats(play_by_play, level='game', teammates=True, opposition=True)
 
 # These are game statistics for forward-line combinations, accounting for opponents on-ice
 forward_lines = prep_lines(play_by_play, position='f', opposition=True)
 ```
 
-### capfriendly
-
-Use `chickenstats.capfriendly` to scrape salary & contract information from [CapFriendly](https://capfriendly.com).
-Information available includes AAV, contract term, player age, signing date, draft year, amongst others. 
-
-```python
-from chickenstats.capfriendly import scrape_capfriendly
-
-# Scrape CapFriendly data for the current year
-cf = scrape_capfriendly(2023)
-```
-
 ---
 
 ## Acknowledgements
 
 This project wouldn't be possible without the support & efforts of countless others. I am obviously
 extremely grateful, even if there are too many of you to thank individually. However, this chicken will do his best.
 
@@ -135,10 +126,10 @@
 
 Sincere apologies to the friends & family that have put up with me since my entry into Python, programming, & data
 analysis in January 2021. Thank you for being excited for me & with me throughout all of this, especially when you've
 had to fake it...
 
 Speaking of which, thank you to the hockey analytics community on (the artist formerly known as) Twitter. You're producing
 & reacting to cutting-edge statistical analyses, while providing a supportive, welcoming environment for newcomers.
-This is by no means exhaustive, but a few people worth calling out specifically:
+This is by no means exhaustive, but a few people worth calling out specifically:
```

### Comparing `chickenstats-1.7.7/chickenstats/capfriendly/scrape.py` & `chickenstats-1.7.8/chickenstats/capfriendly/scrape.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 )
 
 import io
 
 from chickenstats.chicken_nhl.helpers import s_session
 
 
-def munge_cf(df, scrape_year):
-    """Function to clean raw data from capfriendly"""
+def munge_cf(df: pd.DataFrame, scrape_year: int):
+    """Function to clean raw data from capfriendly.com"""
     new_cols = {
         x: x.lower().replace(" ", "_").replace("._", "_").replace(".", "_")
         for x in df.columns
     }
 
     df.rename(columns=new_cols, inplace=True)
 
@@ -278,123 +278,119 @@
     }
 
     df = df[cols].rename(columns=rename_cols).drop_duplicates()
 
     return df
 
 
-def scrape_capfriendly(year=2023):
+def scrape_capfriendly(year: int | list[int | str] = 2023):
     """
-    Scrape salary data from Capfriendly for a given year or list-like object of four-digit seasons. Returns a Pandas DataFrame.
-
-    By default, returns data from the 2022-2023 season. Historical data supported. Typically takes 8-12 seconds per season.
+    Scrape salary data from Capfriendly for a given year or years. Returns a Pandas DataFrame.
+    By default, returns data from the 2023-2024 season. Historical data supported.
+    Typically takes 8-12 seconds per season.
 
     For a glossary of terms, please visit www.capfriendly.com
 
-    Parameters
-    ----------
-    year : str or integer, default = 2023
-        Four-digit year (e.g., 2023), or list-like object consisting of four-digit years (e.g., generator or Pandas Series)
-
-    Returns
-    ----------
-    season: integer
-        8-digit season code, e.g., 20222023
-    player_name: object
-        Player's latin-encoded name, e.g., FILIP FORSBERG
-    player_id: object
-        Identifier that can be used to match with Evolving Hockey data, e.g., FILIP.FORSBERG
-    team: object
-        3-letter team code, e.g., NSH
-    country: object
-        Country with which player is affiliated, e.g., SWEDEN
-    position: object
-        Player's position, e.g., LW
-    birth_date: object
-        Player's birth date, e.g., 1994-08-13
-    birth_year: integer
-        Player's birth year, e.g., 1994
-    age: integer
-        Player's age as of start of the season, e.g., 28
-    age_precise: float
-        Player's age as of the time the data is scraped, e.g., 28.62208
-    handed: object
-        Hand with which the player shoots (skater) or catches (goalie), e.g., RIGHT
-    height_ft: float
-        Player's height in feet, e.g., 6.083333
-    height_cm: integer
-        Player's height in centimeters, e.g., 185
-    weight_lbs: integer
-        Player's weight in pounds, e.g., 205
-    weight_kg: integer
-        Player's weight in kilograms, e.g., 93
-    drafted: object
-        Player's draft information, e.g., 11 - ROUND 1 - 2012 (WSH)
-    draft_year: integer
-        Year player was drafted, e.g., 2012
-    draft_team: object
-        Team that drafted player, e.g., WSH
-    draft_pick: object
-        Pick with which player was drafted, e.g., 11
-    draft_round: object
-        Round in which player was drafted, e.g., ROUND 1
-    signing_date: object
-        Date on which current contract was signed, e.g., 2022-07-09
-    signing_age: integer
-        Age in years at time of signing, e.g., 27
-    signing_age_precise: float
-        Age in years at time of singing, e.g., 27.904748
-    signing: object
-        Contract type at time of signing, e.g., UFA
-    expiry: object
-        Contract type at time of expiry, e.g., UFA
-    expiration_year: integer
-        Year the current contract expires, e.g., 2030
-    years_remaining: integer
-        Years remaining on the contract from current year, e.g., 7
-    contract_length: integer
-        Length of the contract, e.g., 8
-    contract_extension: integer
-        Dummy variable for if the contract was an extension, e.g., 1
-    contract_type: object
-        Type of contract, e.g., STANDARD (1-WAY)
-    aav: integer
-        Average annual value of contract, e.g., 8500000
-    salary: integer
-        Salary value of contract, e.g., 10000000
-    base_salary: integer
-        Base salary value of contract, e.g., 10000000
-    cap_hit: integer
-        Dollar value hit to salary cap, e.g., 8500000
-    cap_hit_pct: float
-        Percentage of salary cap allocated to player, e.g, 10.3%
-    signing_bonus: integer
-        Dollar value of signing bonus, e.g., 0
-    performance_bonus: integer
-        Dollar value of performance bonus, e.g., 0
-    clause: object
-        Type of trade protections player has, e.g., NMC
-    arbitration_required: integer
-        Whether salary arbitration is required, e.g., 0
-    arbitration_eligible: integer
-        Whether the contract is eligible for arbitration, e.g., 0
-    minors: float
-        Salary if player were in the minors, e.g., 10000000
-    slide_candidate: integer
-        Whether player is a slide candidate
-
-    Examples
-    ----------
-
-    Scrape all contract information for active players in the current season
-    >>> cf = scrape_capfriendly()
-
-    Returns data for multiple seasons
-    >>> years = list(range(2019, 2023))
-    >>> cf = scrape_capfriendly(years)
+    Parameters:
+        year (str | int):
+            Four-digit year, or list-like object consisting of four-digit years
+
+    Returns:
+        season (int):
+            8-digit season code, e.g., 20222023
+        player_name (str):
+            Player's latin-encoded name, e.g., FILIP.FORSBERG
+        player_id (str):
+            Identifier that can be used to match with Evolving Hockey data, e.g., FILIP.FORSBERG
+        team (str):
+            3-letter team code, e.g., NSH
+        country (str):
+            Country with which player is affiliated, e.g., SWEDEN
+        position (str):
+            Player's position, e.g., LW
+        birth_date (str):
+            Player's birth date, e.g., 1994-08-13
+        birth_year (int):
+            Player's birth year, e.g., 1994
+        age (int):
+            Player's age as of start of the season, e.g., 28
+        age_precise (float):
+            Player's age as of the time the data is scraped, e.g., 28.62208
+        handed (str):
+            Hand with which the player shoots (skater) or catches (goalie), e.g., RIGHT
+        height_ft (float):
+            Player's height in feet, e.g., 6.083333
+        height_cm (int):
+            Player's height in centimeters, e.g., 185
+        weight_lbs (int):
+            Player's weight in pounds, e.g., 205
+        weight_kg (int):
+            Player's weight in kilograms, e.g., 93
+        drafted (str):
+            Player's draft information, e.g., 11 - ROUND 1 - 2012 (WSH)
+        draft_year (int):
+            Year player was drafted, e.g., 2012
+        draft_team (str):
+            Team that drafted player, e.g., WSH
+        draft_pick (str):
+            Pick with which player was drafted, e.g., 11
+        draft_round (str):
+            Round in which player was drafted, e.g., ROUND 1
+        signing_date (str):
+            Date on which current contract was signed, e.g., 2022-07-09
+        signing_age (int):
+            Age in years at time of signing, e.g., 27
+        signing_age_precise (float):
+            Age in years at time of singing, e.g., 27.904748
+        signing (str):
+            Contract type at time of signing, e.g., UFA
+        expiry (str):
+            Contract type at time of expiry, e.g., UFA
+        expiration_year (int):
+            Year the current contract expires, e.g., 2030
+        years_remaining (int):
+            Years remaining on the contract from current year, e.g., 7
+        contract_length (int):
+            Length of the contract, e.g., 8
+        contract_extension (int):
+            Dummy variable for if the contract was an extension, e.g., 1
+        contract_type (str):
+            Type of contract, e.g., STANDARD (1-WAY)
+        aav (int):
+            Average annual value of contract, e.g., 8500000
+        salary (int):
+            Salary value of contract, e.g., 10000000
+        base_salary (int):
+            Base salary value of contract, e.g., 10000000
+        cap_hit (int):
+            Dollar value hit to salary cap, e.g., 8500000
+        cap_hit_pct (float):
+            Percentage of salary cap allocated to player, e.g, 10.3%
+        signing_bonus (int):
+            Dollar value of signing bonus, e.g., 0
+        performance_bonus (int):
+            Dollar value of performance bonus, e.g., 0
+        clause (str):
+            Type of trade protections player has, e.g., NMC
+        arbitration_required (int):
+            Whether salary arbitration is required, e.g., 0
+        arbitration_eligible (int):
+            Whether the contract is eligible for arbitration, e.g., 0
+        minors (float):
+            Salary if player were in the minors, e.g., 10000000
+        slide_candidate (int):
+            Whether player is a slide candidate, e.g., 0
+
+    Examples:
+        Scrape all contract information for active players in the current season
+        >>> cf = scrape_capfriendly()
+
+        Returns data for multiple seasons
+        >>> years = list(range(2019, 2023))
+        >>> cf = scrape_capfriendly(years)
 
     """
 
     s = s_session()
 
     concat_list = []
 
@@ -423,15 +419,16 @@
 
             for page in pages:
                 url = f"https://www.capfriendly.com/browse/active/{scrape_year}"
 
                 display_param = (
                     "birthday,country,weight,height,weightkg,heightcm,draft,slide-candidate,"
                     "waivers-exempt,signing-status,expiry-year,performance-bonus,signing-bonus,caphit-percent,aav,"
-                    "length,minors-salary,base-salary,arbitration-eligible,type,signing-age,signing-date,arbitration,extension"
+                    "length,minors-salary,base-salary,arbitration-eligible,type,signing-age,signing-date,"
+                    "arbitration,extension"
                 )
 
                 hide_param = "skater-stats,goalie-stats"
 
                 payload = {
                     "age-calculation-date": "october1",
                     "display": display_param,
```

### Comparing `chickenstats-1.7.7/chickenstats/chicken_nhl/fixes.py` & `chickenstats-1.7.8/chickenstats/chicken_nhl/fixes.py`

 * *Files identical despite different names*

### Comparing `chickenstats-1.7.7/chickenstats/chicken_nhl/helpers.py` & `chickenstats-1.7.8/chickenstats/chicken_nhl/helpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import requests
 from requests.adapters import HTTPAdapter
 import urllib3
 
 import numpy as np
 import pandas as pd
 
+from rich.progress import (
+    ProgressColumn,
+    Task,
+)
+
+from rich.text import Text
+
 
 # This function & the timeout class are used for scraping throughout
 class TimeoutHTTPAdapter(HTTPAdapter):
     def __init__(self, *args, **kwargs):
         self.timeout = 3
 
         if "timeout" in kwargs:
@@ -28,28 +35,33 @@
 
 
 def s_session() -> requests.Session:
     """Creates a requests Session object using the HTTPAdapter from above"""
 
     s = requests.Session()
 
+    user_agent = "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.4.1 Safari/605.1.15"
+    headers = {"User-Agent": user_agent}
+    s.headers.update(headers)
+
     retry = urllib3.Retry(
         total=7,
         backoff_factor=2,
         respect_retry_after_header=False,
         status_forcelist=[54, 60, 401, 403, 404, 408, 429, 500, 502, 503, 504],
     )
 
     connect_timeout = 3
     read_timeout = 10
 
-    adapter = TimeoutHTTPAdapter(max_retries=retry, timeout=(connect_timeout, read_timeout))
+    adapter = TimeoutHTTPAdapter(
+        max_retries=retry, timeout=(connect_timeout, read_timeout)
+    )
 
     s.mount("http://", adapter)
-
     s.mount("https://", adapter)
 
     return s
 
 
 # General helper functions
 
@@ -135,7 +147,28 @@
 
     else:
         raise Exception(
             f"'{obj}' not a supported {object_type} or range of {object_type}s"
         )
 
     return obj
+
+
+class ScrapeSpeedColumn(ProgressColumn):
+    """Renders human-readable transfer speed."""
+
+    def render(self, task: "Task") -> Text:
+        """Show data transfer speed."""
+        speed = task.finished_speed or task.speed
+        if speed is None:
+            return Text("?", style="progress.data.speed")
+        else:
+            speed = round(speed, 2)
+
+            if speed < 1:
+                speed = round(1 / speed, 2)
+                pbar_text = f"{speed} s/it"
+
+            else:
+                pbar_text = f"{speed} it/s"
+
+        return Text(pbar_text, style="progress.data.speed")
```

### Comparing `chickenstats-1.7.7/chickenstats/chicken_nhl/info.py` & `chickenstats-1.7.8/chickenstats/chicken_nhl/info.py`

 * *Files identical despite different names*

### Comparing `chickenstats-1.7.7/chickenstats/evolving_hockey/base.py` & `chickenstats-1.7.8/chickenstats/evolving_hockey/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,18 +13,17 @@
 # Function to munge play-by-play data
 def munge_pbp(pbp: pd.DataFrame) -> pd.DataFrame:
     """
     Cleans csv file pulled from play-by-play query tool at evolving-hockey.com.
 
     Nested within `prep_pbp()` function. Returns Pandas DataFrame.
 
-    Parameters
-    ----------
-    pbp : csv file
-        CSV file downloaded from play-by-play query tool at evolving-hockey.com
+    Parameters:
+        pbp : pd.DataFrame
+            Pandas DataFrame from a CSV file downloaded from play-by-play query tool at evolving-hockey.com
 
     """
 
     df = pbp.copy()
 
     # Common column names for ease of typing later
 
@@ -1968,18 +1967,17 @@
 # Function to munge the shifts data and create roster
 def munge_rosters(shifts: pd.DataFrame) -> pd.DataFrame:
     """
     Preps roster data from csv file pulled from shifts query tool at evolving-hockey.com.
 
     Nested within `prep_pbp()` function. Returns Pandas DataFrame.
 
-    Parameters
-    ----------
-    shifts : csv file
-        CSV file downloaded from shifts query tool at evolving-hockey.com
+    Parameters:
+        shifts : pd.DataFrame
+            Pandas DataFrame of a CSV file downloaded from shifts query tool at evolving-hockey.com
 
     """
 
     keep = ["player", "team_num", "position", "game_id", "season", "session", "team"]
 
     df = shifts[keep].copy().drop_duplicates()
 
@@ -2020,20 +2018,19 @@
 # Function to add positions to the play-by-play data
 def add_positions(pbp: pd.DataFrame, rosters: pd.DataFrame) -> pd.DataFrame:
     """
     Adds position data to the play-by-play data from evolving-hockey.com.
 
     Nested within `prep_pbp()` function. Returns Pandas DataFrame.
 
-    Parameters
-    ----------
-    pbp : DataFrame
-        Data returned from `munge_pbp()` function
-    rosters : DataFrame
-        Data returned from `munge_rosters` function
+    Parameters:
+        pbp : pd.DataFrame
+            Data returned from `munge_pbp()` function
+        rosters : pd.DataFrame
+            Data returned from `munge_rosters` function
 
     """
 
     pbp = pbp.copy()
 
     rosters = rosters.copy()
 
@@ -2377,27 +2374,25 @@
     opposition: bool = False,
 ) -> pd.DataFrame:
     """
     Prepares DataFrame of individual stats from play-by-play data.
 
     Nested within `prep_stats()` function. Returns Pandas DataFrame.
 
-    Parameters
-    ----------
-    pbp : DataFrame
-        Data returned from `prep_pbp()` function
-    level : string
-        Determines the level of aggregation.
-        One of season, session, game, period
-    score : bool
-        Determines if stats are cut by score state
-    teammates : bool
-        Determines if stats are cut by teammates on ice
-    opposition : bool
-        Determines if stats are cut by opponents on ice
+    Parameters:
+        pbp : pd.DataFrame
+            Data returned from `prep_pbp()` function
+        level : str
+            Determines the level of aggregation. One of season, session, game, period
+        score : bool
+            Determines if stats are cut by score state
+        teammates : bool
+            Determines if stats are cut by teammates on ice
+        opposition : bool
+            Determines if stats are cut by opponents on ice
 
     """
 
     df = pbp.copy()
 
     players = ["event_player_1", "event_player_2", "event_player_3"]
 
@@ -2983,27 +2978,26 @@
     opposition: bool = False,
 ) -> pd.DataFrame:
     """
     Prepares DataFrame of on-ice stats from play-by-play data.
 
     Nested within `prep_stats()` function. Returns Pandas DataFrame.
 
-    Parameters
-    ----------
-    pbp : DataFrame
-        Data returned from `prep_pbp()` function
-    level : string
-        Determines the level of aggregation.
-        One of season, session, game, period
-    score : bool
-        Determines if stats are cut by score state
-    teammates : bool
-        Determines if stats are cut by teammates on ice
-    opposition : bool
-        Determines if stats are cut by opponents on ice
+    Parameters:
+        pbp : pd.DataFrame
+            Data returned from `prep_pbp()` function
+        level : str
+            Determines the level of aggregation.
+            One of season, session, game, period
+        score : bool
+            Determines if stats are cut by score state
+        teammates : bool
+            Determines if stats are cut by teammates on ice
+        opposition : bool
+            Determines if stats are cut by opponents on ice
 
     """
 
     df = pbp.copy()
 
     stats_list = [
         "block",
@@ -3472,27 +3466,26 @@
     opposition: bool = False,
 ) -> pd.DataFrame:
     """
     Prepares DataFrame of zone stats from play-by-play data.
 
     Nested within `prep_stats()` function. Returns Pandas DataFrame.
 
-    Parameters
-    ----------
-    pbp : DataFrame
-        Data returned from `prep_pbp()` function
-    level : string
-        Determines the level of aggregation.
-        One of season, session, game, period
-    score : bool
-        Determines if stats are cut by score state
-    teammates : bool
-        Determines if stats are cut by teammates on ice
-    opposition : bool
-        Determines if stats are cut by opponents on ice
+    Parameters:
+        pbp : pd.DataFrame
+            Data returned from `prep_pbp()` function
+        level : str
+            Determines the level of aggregation.
+            One of season, session, game, period
+        score : bool
+            Determines if stats are cut by score state
+        teammates : bool
+            Determines if stats are cut by teammates on ice
+        opposition : bool
+            Determines if stats are cut by opponents on ice
 
     """
     conds = np.logical_and(
         pbp.event_type == "CHANGE",
         np.logical_or.reduce([pbp.ozs > 0, pbp.nzs > 0, pbp.dzs > 0, pbp.otf > 0]),
     )
```

### Comparing `chickenstats-1.7.7/chickenstats/evolving_hockey/stats.py` & `chickenstats-1.7.8/chickenstats/evolving_hockey/stats.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,355 +16,351 @@
 ) -> pd.DataFrame:
     """
     Prepares a play-by-play dataframe using EvolvingHockey data, but with additional stats and information.
     Columns keyword argument determines information returned.
 
     Used in later aggregation functions. Returns a DataFrame
 
-    Parameters
-    ----------
-    pbp : csv
-        CSV file downloaded from play-by-play query tool at evolving-hockey.com
-    shifts : csv
-        CSV file downloaded from shifts query tool at evolving-hockey.com
-    columns: str, default='full'
-        Whether to return additional columns or more sparse play-by-play dataframe
-
-    Returns
-    ----------
-    season: integer
-        8-digit season code, e.g., 20192020
-    session: object
-        Regular season or playoffs, e.g., R
-    game_id: integer
-        10-digit game identifier, e.g., 2019020684
-    game_date: object
-        Date of game in Eastern time-zone, e.g., 2020-01-09
-    event_index: object
-        Unique index number of event, in chronological order, e.g.,
-    game_period: integer
-        Game period, e.g., 3
-    game_seconds: integer
-        Game time elapsed in seconds, e.g., 3578
-    period_seconds: integer
-        Period time elapsed in seconds, e.g., 1178
-    clock_time : object
-        Time shown on clock, e.g.,
-    strength_state: object
-        Strength state from the perspective of the event team, e.g., 5vE
-    score_state: object
-        Score state from the perspective of the event team, e.g., 5v2
-    event_type: object
-        Name of the event, e.g., GOAL
-    event_description: object
-        Description of the event, e.g., NSH #35 RINNE(1), WRIST, DEF. ZONE, 185 FT.
-    event_detail: object
-        Additional information about the event, e.g., Wrist
-    event_zone: object
-        Zone location of event, e.g., DEF
-    event_team: object
-        3-letter abbreviation of the team for the event, e.g., NSH
-    opp_team: object
-        3-letter abbreviation of the opposing team for the event, e.g., CHI
-    is_home: integer
-        Dummy variable to signify whether event team is home team, e.g., 0
-    coords_x: float
-        X coordinates of event, e.g., -96
-    coords_y: float
-        Y coordinates of event, e.g., 11
-    event_player_1: object
-        Name of the player, e.g., PEKKA.RINNE
-    event_player_1_id: object
-        Identifier that can be used to match with Evolving Hockey data, e.g., PEKKA.RINNE
-    event_player_1_pos: object
-        Player's position for the game, may differ from primary position, e.g., G
-    event_player_2: object
-        Name of the player
-    event_player_2_id: object
-        Identifier that can be used to match with Evolving Hockey data
-    event_player_2_pos: object
-        Player's position for the game, may differ from primary position
-    event_player_3: object
-        Name of the player
-    event_player_3_id: object
-        Identifier that can be used to match with Evolving Hockey data
-    event_player_3_pos: object
-        Player's position for the game, may differ from primary position
-    event_length: integer
-        Length of time elapsed in seconds since previous event, e.g., 5
-    high_danger: integer
-        Whether shot event is from high-danger area, e.g., 0
-    danger: integer
-        Whether shot event is from danger area,
-        exclusive of high-danger area, e.g., 0
-    pbp_distance: float
-        Distance from opponent net, in feet, according to play-by-play description, e.g., 185.0
-    event_distance: float
-        Distance from opponent net, in feet, e.g., 185.326738
-    event_angle: float
-        Angle of opponent's net from puck, in degrees, e.g., 57.528808
-    opp_strength_state: object
-        Strength state from the perspective of the opposing team, e.g., Ev5
-    opp_score_state: object
-        Score state from the perspective of the opposing team, e.g., 2v5
-    event_on_f: object
-        Names of the event team's forwards that are on the ice during the event,
-        e.g., NICK BONINO, CALLE JARNKROK, MIKAEL GRANLUND
-    event_on_f_id: object
-        EH IDs of the event team's forwards that are on the ice during the event,
-        e.g., NICK.BONINO, CALLE.JARNKROK, MIKAEL.GRANLUND
-    event_on_d: object
-        Names of the event team's defensemen that are on the ice during the event,
-        e.g., MATTIAS EKHOLM, ROMAN JOSI
-    event_on_d_id: object
-        EH IDs of the event team's defensemen that are on the ice during the event,
-        e.g., MATTIAS.EKHOLM, ROMAN.JOSI
-    event_on_g: object
-        Name of the goalie for the event team, e.g., PEKKA RINNE
-    event_on_g_id: object
-        Identifier for the event team goalie that can be used to match with Evolving Hockey data, e.g., PEKKA.RINNE
-    event_on_1: object
-        Name of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_1_id: object
-        EH ID of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_1_pos: object
-        Position of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_2: object
-        Name of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_2_id: object
-        EH ID of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_2_pos: object
-        Position of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_3: object
-        Name of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_3_id: object
-        EH ID of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_3_pos: object
-        Position of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_4: object
-        Name of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_4_id: object
-        EH ID of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_4_pos: object
-        Position of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_5: object
-        Name of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_5_id: object
-        EH ID of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_5_pos: object
-        Position of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_6: object
-        Name of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_6_id: object
-        EH ID of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_6_pos: object
-        Position of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_7: object
-        Name of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_7_id: object
-        EH ID of one the event team's players that are on the ice during the event,
-        e.g.,
-    event_on_7_pos: object
-        Position of one the event team's players that are on the ice during the event,
-        e.g.,
-    opp_on_f: object
-        Names of the opponent's forwards that are on the ice during the event,
-        e.g., ALEX DEBRINCAT, JONATHAN TOEWS, KIRBY DACH, PATRICK KANE
-    opp_on_f_id: object
-        EH IDs of the event team's forwards that are on the ice during the event,
-        e.g., ALEX.DEBRINCAT, JONATHAN.TOEWS, KIRBY.DACH, PATRICK.KANE
-    opp_on_d: object
-        Names of the opposing team's defensemen that are on the ice during the event,
-        e.g., DUNCAN KEITH, ERIK GUSTAFSSON
-    opp_on_d_id: object
-        EH IDs of the opposing team's defensemen that are on the ice during the event,
-        e.g., DUNCAN.KEITH, ERIK.GUSTAFSSON2
-    opp_on_g: object
-        Name of the opposing goalie for the event team, e.g., EMPTY NET
-    opp_on_g_id: object
-        Identifier for the opposing goalie that can be used to match with Evolving Hockey data, e.g., EMPTY NET
-    opp_on_1: object
-        Name of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_1_id: object
-        EH ID of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_1_pos: object
-        Position of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_2: object
-        Name of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_2_id: object
-        EH ID of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_2_pos: object
-        Position of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_3: object
-        Name of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_3_id: object
-        EH ID of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_3_pos: object
-        Position of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_4: object
-        Name of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_4_id: object
-        EH ID of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_4_pos: object
-        Position of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_5: object
-        Name of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_5_id: object
-        EH ID of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_5_pos: object
-        Position of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_6: object
-        Name of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_6_id: object
-        EH ID of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_6_pos: object
-        Position of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_7: object
-        Name of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_7_id: object
-        EH ID of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    opp_on_7_pos: object
-        Position of one the opposing team's players that are on the ice during the event,
-        e.g.,
-    change: integer
-        Dummy variable to indicate whether event is a change, e.g., 0
-    zone_start: object
-        Zone where the changed, e.g., OFF or OTF
-    num_on: integer
-        Number of players entering the ice, e.g., 6
-    num_off: integer
-        Number of players exiting the ice, e.g., 0
-    players_on: string
-        Names of players on, in jersey order,
-        e.g., FILIP FORSBERG, ALEX CARRIER, ROMAN JOSI, MIKAEL GRANLUND, JUUSE SAROS, MATT DUCHENE
-    players_on_id: string
-        Evolving Hockey IDs of players on, in jersey order,
-        e.g., FILIP.FORSBERG, ALEX.CARRIER, ROMAN.JOSI, MIKAEL.GRANLUND, JUUSE.SAROS, MATT.DUCHENE
-    players_on_pos: string
-        Positions of players on, in jersey order,
-        e.g., L, D, D, C, G, C
-    players_off: string
-        Names of players off, in jersey order
-    players_off_id: string
-        Evolving Hockey IDs of players off, in jersey order
-    players_off_positions: string
-        Positions of players off, in jersey order
-    shot: integer
-        Dummy variable to indicate whether event is a shot, e.g., 0
-    shot_adj: float
-        Score and venue-adjusted shot value, e.g.,
-    goal: integer
-        Dummy variable to indicate whether event is a goal, e.g., 1
-    goal_adj: float
-        Score and venue-adjusted shot value, e.g.,
-    pred_goal: float
-        Predicted goal value (xG), e.g.,
-    pred_goal_adj: float
-        Score and venue-adjusted predicted goal (xG) value, e.g.,
-    miss: integer
-        Dummy variable to indicate whether event is a missed shot, e.g., 0
-    block: integer
-        Dummy variable to indicate whether event is a block, e.g., 0
-    corsi: integer
-        Dummy variable to indicate whether event is a corsi event, e.g., 1
-    corsi_adj: float
-        Score and venue-adjusted corsi value, e.g.,
-    fenwick: integer
-        Dummy variable to indicate whether event is a fenwick event, e.g., 1
-    fenwick_adj: float
-         Score and venue-adjusted fenwick value, e.g.,
-    hd_shot: integer
-        Dummy variable to indicate whether event is a high-danger shot event, e.g., 0
-    hd_goal: integer
-        Dummy variable to indicate whether event is a high-danger goal event, e.g., 0
-    hd_miss: integer
-        Dummy variable to indicate whether event is a high-danger miss event, e.g., 0
-    hd_fenwick: integer
-        Dummy variable to indicate whether event is a high-danger fenwick event, e.g., 0
-    fac: integer
-        Dummy variable to indicate whether event is a faceoff, e.g., 0
-    hit: integer
-        Dummy variable to indicate whether event is a hit, e.g., 0
-    give: integer
-        Dummy variable to indicate whether event is a giveaway, e.g., 0
-    take: integer
-        Dummy variable to indicate whether event is a takeaway, e.g., 0
-    pen0: integer
-        Dummy variable to indicate whether event is a penalty with no minutes, e.g., 0
-    pen2: integer
-        Dummy variable to indicate whether event is a two-minute penalty, e.g., 0
-    pen4: integer
-        Dummy variable to indicate whether event is a four-minute penalty, e.g., 0
-    pen5: integer
-        Dummy variable to indicate whether event is a five-minute penalty, e.g., 0
-    pen10: integer
-        Dummy variable to indicate whether event is a ten-minute penalty, e.g., 0
-    stop: integer
-        Dummy variable to indicate whether event is a stoppage, e.g., 0
-    ozf: integer
-        Dummy variable to indicate whether event is an offensive zone faceoff e.g., 0
-    nzf: integer
-        Dummy variable to indicate whether event is a neutral zone faceoff, e.g., 0
-    dzf: integer
-        Dummy variable to indicate whether event is a defensive zone faceoff, e.g., 0
-    ozs: integer
-        Dummy variable to indicate whether an event is an offensive zone change, e.g., 0
-    nzs: integer
-        Dummy variable to indicate whether an event is a neutral zone change, e.g., 0
-    dzs: integer
-        Dummy variable to indicate whether an event is an defensive zone change, e.g., 0
-    otf: integer
-        Dummy variable to indicate whether an event is an on-the-fly change, e.g., 0
-
-    Examples
-    ----------
-
-    Play-by-play DataFrame
-    >>> raw_shifts = pd.read_csv('./raw_shifts.csv')
-    >>> raw_pbp = pd.read_csv('./raw_pbp.csv')
-    >>> play_by_play = prep_pbp(raw_pbp, raw_shifts)
+    Parameters:
+        pbp (pd.DataFrame):
+            Pandas DataFrame of CSV file downloaded from play-by-play query tool at evolving-hockey.com
+        shifts (pd.DataFrame):
+            Pandas DataFrame of CSV file downloaded from shifts query tool at evolving-hockey.com
+        columns (str):
+            Whether to return additional columns or more sparse play-by-play dataframe
+
+    Returns:
+        season (int):
+            8-digit season code, e.g., 20192020
+        session (str):
+            Regular season or playoffs, e.g., R
+        game_id (int):
+            10-digit game identifier, e.g., 2019020684
+        game_date (str):
+            Date of game in Eastern time-zone, e.g., 2020-01-09
+        event_index (int):
+            Unique index number of event, in chronological order, e.g.,
+        game_period (int):
+            Game period, e.g., 3
+        game_seconds (int):
+            Game time elapsed in seconds, e.g., 3578
+        period_seconds (int):
+            Period time elapsed in seconds, e.g., 1178
+        clock_time (str):
+            Time shown on clock, e.g., 0:22
+        strength_state (str):
+            Strength state from the perspective of the event team, e.g., 5vE
+        score_state (str):
+            Score state from the perspective of the event team, e.g., 5v2
+        event_type (str):
+            Name of the event, e.g., GOAL
+        event_description (str):
+            Description of the event, e.g., NSH #35 RINNE(1), WRIST, DEF. ZONE, 185 FT.
+        event_detail (str | None):
+            Additional information about the event, e.g., Wrist
+        event_zone (str | None):
+            Zone location of event, e.g., DEF
+        event_team (str | None):
+            3-letter abbreviation of the team for the event, e.g., NSH
+        opp_team (str | None):
+            3-letter abbreviation of the opposing team for the event, e.g., CHI
+        is_home (int | None):
+            Dummy variable to signify whether event team is home team, e.g., 0
+        coords_x (int | None):
+            X coordinates of event, e.g., -96
+        coords_y (int | None):
+            Y coordinates of event, e.g., 11
+        event_player_1 (str):
+            Name of the first event player, e.g., PEKKA.RINNE
+        event_player_1_id (str):
+            Identifier that can be used to match with Evolving Hockey data, e.g., PEKKA.RINNE
+        event_player_1_pos (str):
+            Player's position for the game, may differ from primary position, e.g., G
+        event_player_2 (str):
+            Name of the second event player
+        event_player_2_id (str):
+            Identifier that can be used to match with Evolving Hockey data
+        event_player_2_pos (str):
+            Player's position for the game, may differ from primary position
+        event_player_3 (str):
+            Name of the third event player
+        event_player_3_id (str):
+            Identifier that can be used to match with Evolving Hockey data
+        event_player_3_pos (str):
+            Player's position for the game, may differ from primary position
+        event_length (int):
+            Length of time elapsed in seconds since previous event, e.g., 5
+        high_danger (int):
+            Whether shot event is from high-danger area, e.g., 0
+        danger (int):
+            Whether shot event is from danger area,
+            exclusive of high-danger area, e.g., 0
+        pbp_distance (float):
+            Distance from opponent net, in feet, according to play-by-play description, e.g., 185.0
+        event_distance (float):
+            Distance from opponent net, in feet, e.g., 185.326738
+        event_angle (float):
+            Angle of opponent's net from puck, in degrees, e.g., 57.528808
+        opp_strength_state (str):
+            Strength state from the perspective of the opposing team, e.g., Ev5
+        opp_score_state (str):
+            Score state from the perspective of the opposing team, e.g., 2v5
+        event_on_f (str):
+            Names of the event team's forwards that are on the ice during the event,
+            e.g., NICK BONINO, CALLE JARNKROK, MIKAEL GRANLUND
+        event_on_f_id (str):
+            EH IDs of the event team's forwards that are on the ice during the event,
+            e.g., NICK.BONINO, CALLE.JARNKROK, MIKAEL.GRANLUND
+        event_on_d (str):
+            Names of the event team's defensemen that are on the ice during the event,
+            e.g., MATTIAS EKHOLM, ROMAN JOSI
+        event_on_d_id (str):
+            EH IDs of the event team's defensemen that are on the ice during the event,
+            e.g., MATTIAS.EKHOLM, ROMAN.JOSI
+        event_on_g (str):
+            Name of the goalie for the event team, e.g., PEKKA RINNE
+        event_on_g_id (str):
+            Identifier for the event team goalie that can be used to match with Evolving Hockey data, e.g., PEKKA.RINNE
+        event_on_1 (str):
+            Name of one the event team's players that are on the ice during the event,
+            e.g., CALLE.JARNKROK
+        event_on_1_id (str):
+            EH ID of one the event team's players that are on the ice during the event,
+            e.g., CALLE.JARNKROK
+        event_on_1_pos (str):
+            Position of one the event team's players that are on the ice during the event,
+            e.g., C
+        event_on_2 (str):
+            Name of one the event team's players that are on the ice during the event,
+            e.g., MATTIAS.EKHOLM
+        event_on_2_id (str):
+            EH ID of one the event team's players that are on the ice during the event,
+            e.g., MATTIAS.EKHOLM
+        event_on_2_pos (str):
+            Position of one the event team's players that are on the ice during the event,
+            e.g., D
+        event_on_3 (str):
+            Name of one the event team's players that are on the ice during the event,
+            e.g., MIKAEL.GRANLUND
+        event_on_3_id (str):
+            EH ID of one the event team's players that are on the ice during the event,
+            e.g., MIKAEL.GRANLUND
+        event_on_3_pos (str):
+            Position of one the event team's players that are on the ice during the event,
+            e.g., C
+        event_on_4 (str):
+            Name of one the event team's players that are on the ice during the event,
+            e.g., NICK.BONINO
+        event_on_4_id (str):
+            EH ID of one the event team's players that are on the ice during the event,
+            e.g., NICK.BONINO
+        event_on_4_pos (str):
+            Position of one the event team's players that are on the ice during the event,
+            e.g., C
+        event_on_5 (str):
+            Name of one the event team's players that are on the ice during the event,
+            e.g., PEKKA.RINNE
+        event_on_5_id (str):
+            EH ID of one the event team's players that are on the ice during the event,
+            e.g., PEKKA.RINNE
+        event_on_5_pos (str):
+            Position of one the event team's players that are on the ice during the event,
+            e.g., G
+        event_on_6 (str):
+            Name of one the event team's players that are on the ice during the event,
+            e.g., ROMAN.JOSI
+        event_on_6_id (str):
+            EH ID of one the event team's players that are on the ice during the event,
+            e.g., ROMAN.JOSI
+        event_on_6_pos (str):
+            Position of one the event team's players that are on the ice during the event,
+            e.g., D
+        event_on_7 (str):
+            Name of one the event team's players that are on the ice during the event,
+            e.g., NaN
+        event_on_7_id (str):
+            EH ID of one the event team's players that are on the ice during the event,
+            e.g., NaN
+        event_on_7_pos (str):
+            Position of one the event team's players that are on the ice during the event,
+            e.g., NaN
+        opp_on_f (str):
+            Names of the opponent's forwards that are on the ice during the event,
+            e.g., ALEX DEBRINCAT, JONATHAN TOEWS, KIRBY DACH, PATRICK KANE
+        opp_on_f_id (str):
+            EH IDs of the event team's forwards that are on the ice during the event,
+            e.g., ALEX.DEBRINCAT, JONATHAN.TOEWS, KIRBY.DACH, PATRICK.KANE
+        opp_on_d (str):
+            Names of the opposing team's defensemen that are on the ice during the event,
+            e.g., DUNCAN KEITH, ERIK GUSTAFSSON
+        opp_on_d_id (str):
+            EH IDs of the opposing team's defensemen that are on the ice during the event,
+            e.g., DUNCAN.KEITH, ERIK.GUSTAFSSON2
+        opp_on_g (str):
+            Name of the opposing goalie for the event team, e.g., EMPTY NET
+        opp_on_g_id (str):
+            Identifier for the opposing goalie that can be used to match with Evolving Hockey data, e.g., EMPTY NET
+        opp_on_1 (str):
+            Name of one the opposing team's players that are on the ice during the event,
+            e.g., ALEX.DEBRINCAT
+        opp_on_1_id (str):
+            EH ID of one the opposing team's players that are on the ice during the event,
+            e.g., ALEX.DEBRINCAT
+        opp_on_1_pos (str):
+            Position of one the opposing team's players that are on the ice during the event,
+            e.g., R
+        opp_on_2 (str):
+            Name of one the opposing team's players that are on the ice during the event,
+            e.g., DUNCAN.KEITH
+        opp_on_2_id (str):
+            EH ID of one the opposing team's players that are on the ice during the event,
+            e.g., DUNCAN.KEITH
+        opp_on_2_pos (str):
+            Position of one the opposing team's players that are on the ice during the event,
+            e.g., D
+        opp_on_3 (str):
+            Name of one the opposing team's players that are on the ice during the event,
+            e.g., ERIK.GUSTAFSSON2
+        opp_on_3_id (str):
+            EH ID of one the opposing team's players that are on the ice during the event,
+            e.g., ERIK.GUSTAFSSON2
+        opp_on_3_pos (str):
+            Position of one the opposing team's players that are on the ice during the event,
+            e.g., D
+        opp_on_4 (str):
+            Name of one the opposing team's players that are on the ice during the event,
+            e.g., JONATHAN.TOEWS
+        opp_on_4_id (str):
+            EH ID of one the opposing team's players that are on the ice during the event,
+            e.g., JONATHAN.TOEWS
+        opp_on_4_pos (str):
+            Position of one the opposing team's players that are on the ice during the event,
+            e.g., C
+        opp_on_5 (str):
+            Name of one the opposing team's players that are on the ice during the event,
+            e.g., KIRBY.DACH
+        opp_on_5_id (str):
+            EH ID of one the opposing team's players that are on the ice during the event,
+            e.g., KIRBY.DACH
+        opp_on_5_pos (str):
+            Position of one the opposing team's players that are on the ice during the event,
+            e.g., C
+        opp_on_6 (str):
+            Name of one the opposing team's players that are on the ice during the event,
+            e.g., PATRICK.KANE
+        opp_on_6_id (str):
+            EH ID of one the opposing team's players that are on the ice during the event,
+            e.g., PATRICK.KANE
+        opp_on_6_pos (str):
+            Position of one the opposing team's players that are on the ice during the event,
+            e.g., R
+        opp_on_7 (str):
+            Name of one the opposing team's players that are on the ice during the event,
+            e.g., NaN
+        opp_on_7_id (str):
+            EH ID of one the opposing team's players that are on the ice during the event,
+            e.g., NaN
+        opp_on_7_pos (str):
+            Position of one the opposing team's players that are on the ice during the event,
+            e.g., NaN
+        change (int):
+            Dummy variable to indicate whether event is a change, e.g., 0
+        zone_start (str):
+            Zone where the changed, e.g., OFF or OTF
+        num_on (int | None):
+            Number of players entering the ice, e.g., 6
+        num_off (int | None):
+            Number of players exiting the ice, e.g., 0
+        players_on (str):
+            Names of players on, in jersey order,
+            e.g., FILIP FORSBERG, ALEX CARRIER, ROMAN JOSI, MIKAEL GRANLUND, JUUSE SAROS, MATT DUCHENE
+        players_on_id (str):
+            Evolving Hockey IDs of players on, in jersey order,
+            e.g., FILIP.FORSBERG, ALEX.CARRIER, ROMAN.JOSI, MIKAEL.GRANLUND, JUUSE.SAROS, MATT.DUCHENE
+        players_on_pos (str):
+            Positions of players on, in jersey order,
+            e.g., L, D, D, C, G, C
+        players_off (str):
+            Names of players off, in jersey order
+        players_off_id (str):
+            Evolving Hockey IDs of players off, in jersey order
+        players_off_pos (str):
+            Positions of players off, in jersey order
+        shot (int):
+            Dummy variable to indicate whether event is a shot, e.g., 1
+        shot_adj (float):
+            Score and venue-adjusted shot value, e.g., 0
+        goal (int):
+            Dummy variable to indicate whether event is a goal, e.g., 1
+        goal_adj (float):
+            Score and venue-adjusted shot value, e.g., 0
+        pred_goal (float):
+            Predicted goal value (xG), e.g., 0.482589
+        pred_goal_adj (float):
+            Score and venue-adjusted predicted goal (xG) value, e.g., 0
+        miss (int):
+            Dummy variable to indicate whether event is a missed shot, e.g., 0
+        block (int):
+            Dummy variable to indicate whether event is a block, e.g., 0
+        corsi (int):
+            Dummy variable to indicate whether event is a corsi event, e.g., 1
+        corsi_adj (float):
+            Score and venue-adjusted corsi value, e.g., 0
+        fenwick (int):
+            Dummy variable to indicate whether event is a fenwick event, e.g., 1
+        fenwick_adj (float):
+             Score and venue-adjusted fenwick value, e.g., 0
+        hd_shot (int):
+            Dummy variable to indicate whether event is a high-danger shot event, e.g., 0
+        hd_goal (int):
+            Dummy variable to indicate whether event is a high-danger goal event, e.g., 0
+        hd_miss (int):
+            Dummy variable to indicate whether event is a high-danger miss event, e.g., 0
+        hd_fenwick (int):
+            Dummy variable to indicate whether event is a high-danger fenwick event, e.g., 0
+        fac (int):
+            Dummy variable to indicate whether event is a faceoff, e.g., 0
+        hit (int):
+            Dummy variable to indicate whether event is a hit, e.g., 0
+        give (int):
+            Dummy variable to indicate whether event is a giveaway, e.g., 0
+        take (int):
+            Dummy variable to indicate whether event is a takeaway, e.g., 0
+        pen0 (int):
+            Dummy variable to indicate whether event is a penalty with no minutes, e.g., 0
+        pen2 (int):
+            Dummy variable to indicate whether event is a two-minute penalty, e.g., 0
+        pen4 (int):
+            Dummy variable to indicate whether event is a four-minute penalty, e.g., 0
+        pen5 (int):
+            Dummy variable to indicate whether event is a five-minute penalty, e.g., 0
+        pen10 (int):
+            Dummy variable to indicate whether event is a ten-minute penalty, e.g., 0
+        stop (int):
+            Dummy variable to indicate whether event is a stoppage, e.g., 0
+        ozf (int):
+            Dummy variable to indicate whether event is an offensive zone faceoff e.g., 0
+        nzf (int):
+            Dummy variable to indicate whether event is a neutral zone faceoff, e.g., 0
+        dzf (int):
+            Dummy variable to indicate whether event is a defensive zone faceoff, e.g., 0
+        ozs (int):
+            Dummy variable to indicate whether an event is an offensive zone change, e.g., 0
+        nzs (int):
+            Dummy variable to indicate whether an event is a neutral zone change, e.g., 0
+        dzs (int):
+            Dummy variable to indicate whether an event is an defensive zone change, e.g., 0
+        otf (int):
+            Dummy variable to indicate whether an event is an on-the-fly change, e.g., 0
+
+    Examples:
+        Play-by-play DataFrame
+        >>> shifts_raw = pd.read_csv('./raw_shifts.csv')
+        >>> pbp_raw = pd.read_csv('./raw_pbp.csv')
+        >>> pbp = prep_pbp(pbp_raw, shifts_raw)
 
     """
 
     rosters = munge_rosters(shifts)
 
     pbp = munge_pbp(pbp)
 
@@ -570,302 +566,299 @@
     opposition: bool = False,
 ) -> pd.DataFrame:
     """
     Prepares an individual and on-ice stats dataframe using EvolvingHockey data,
     aggregated to desired level. Capable of returning cuts that account for strength state,
     period, score state, teammates, and opposition.
 
-    Returns a DataFrame.
+    Returns a Pandas DataFrame.
 
-    Parameters
-    ----------
-    df : dataframe
-        Dataframe from the prep_pbp function with the default columns argument
-    level : str, default='game'
-        Level to aggregate stats, e.g., 'game'
-    score: bool, default=False
-        Whether to aggregate to score state level
-    teammates: bool, default=False
-        Whether to account for teammates when aggregating
-    opposition: bool, default=False
-        Whether to account for opposition when aggregating
-
-    Returns
-    ----------
-    season: integer
-        8-digit season code, e.g., 20222023
-    session: object
-        Regular season or playoffs, e.g., R
-    game_id: integer
-        10-digit game identifier, e.g.,
-    game_date: object
-        Date of game in Eastern time-zone, e.g.,
-    player: object
-        Name of the player, e.g., FILIP.FORSBERG
-    player_id: object
-        Player EH ID, e.g., FILIP.FORSBERG
-    position: object
-        Player's position, e.g., L
-    team: object
-        3-letter abbreviation of the player's team, e.g., NSH
-    opp_team: object
-        3-letter abbreviation of the opposing team, e.g., NJD
-    strength_state: object
-        Strength state from the perspective of the event team, e.g., 5v4
-    score_state: object
-        Score state from the perspective of the event team, e.g., 0v0
-    game_period: integer
-        Game period, e.g., 1
-    forwards: object
-        Names of the event team's forwards that are on the ice during the event,
-        e.g., FILIP.FORSBERG, MATT.DUCHENE, MIKAEL.GRANLUND, RYAN.JOHANSEN
-    forwards_id: object
-        EH IDs of the event team's forwards that are on the ice during the event,
-        e.g., FILIP.FORSBERG, MATT.DUCHENE, MIKAEL.GRANLUND, RYAN.JOHANSEN
-    defense: object
-        Names of the event team's defensemen that are on the ice during the event,
-        e.g., ROMAN.JOSI
-    defense_id: object
-        EH IDs of the event team's defensemen that are on the ice during the event,
-        e.g., ROMAN.JOSI
-    own_goalie: object
-        Name of the goalie for the event team, e.g., JUUSE.SAROS
-    own_goalie_id: object
-        Identifier for the event team goalie that can be used to match with Evolving Hockey data, e.g., JUUSE.SAROS
-    opp_forwards: object
-        Names of the opponent's forwards that are on the ice during the event,
-        e.g., DAWSON.MERCER, ERIK.HAULA
-    opp_forwards_id: object
-        EH IDs of the event team's forwards that are on the ice during the event,
-        e.g., DAWSON.MERCER, ERIK.HAULA
-    opp_defense: object
-        Names of the opposing team's defensemen that are on the ice during the event,
-        e.g., DAMON.SEVERSON, RYAN.GRAVES
-    opp_defense_id: object
-        EH IDs of the opposing team's defensemen that are on the ice during the event,
-        e.g., DAMON.SEVERSON, RYAN.GRAVES
-    opp_goalie: object
-        Name of the opposing goalie for the event team, e.g., MACKENZIE.BLACKWOOD
-    opp_goalie_id: object
-        Identifier for the opposing goalie that can be used to match with Evolving Hockey data, e.g., MACKENZIE.BLACKWOOD
-    toi: float
-        Time on-ice in minutes, e.g., 1.616667
-    g: integer
-        Number of individual goals scored, e.g, 0
-    a1: integer
-        Number of primary assists, e.g, 0
-    a2: integer
-        Number of secondary assists, e.g, 0
-    isf: integer
-        Number of indiviudal shots registered, e.g., 0
-    iff: integer
-        Number of indiviudal fenwick events registered, e.g., 1
-    icf: integer
-        Number of indiviudal corsi events registered, e.g., 3
-    ixg: float
-        Sum value of individual predicted goals (xG), e.g., 0.237
-    gax: float
-        Sum value of goals scored above expected, e.g., -0.237
-    ihdg: integer
-        Sum value of individual high-danger goals scored, e.g., 0
-    ihdsf: integer
-        Sum value of individual high-danger shots taken, e.g., 0
-    ihdm: integer
-        Sum value of individual high-danger shots missed, e.g., 0
-    ihdf: integer
-        Sum value of individual high-danger fenwick events registered, e.g., 0
-    imsf: integer
-        Sum value of individual missed shots, 1
-    isb: integer
-        Sum value of shots taken that were ultimately blocked, e.g., 2
-    ibs: integer
-        Sum value of opponent shots taken that the player ultimately blocked, e.g.,
-    igive: integer
-        Sum of individual giveaways, e.g., 0
-    itake: integer
-        Sum of individual takeaways, e.g., 0
-    ihf: integer
-        Sum of individual hits for, e.g., 0
-    iht: integer
-        Sum of individual hits taken, e.g., 0
-    ifow: integer
-        Sum of individual faceoffs won, e.g., 0
-    ifol: integer
-        Sum of individual faceoffs lost, e.g., 0
-    iozfw: integer
-        Sum of individual faceoffs won in offensive zone, e.g., 0
-    iozfl: integer
-        Sum of individual faceoffs lost in offensive zone, e.g., 0
-    inzfw: integer
-        Sum of individual faceoffs won in neutral zone, e.g., 0
-    inzfl: integer
-        Sum of individual faceoffs lost in neutral zone, e.g., 0
-    idzfw: integer
-        Sum of individual faceoffs won in defensive zone, e.g., 0
-    idzfl: integer
-        Sum of individual faceoffs lost in defensive zone, e.g., 0
-    a1_xg: float
-        Sum of xG from primary assists, e.g., 0
-    a2_xg: float
-        Sum of xG from secondary assists, e.g., 0
-    ipent0: integer
-        Sum of individual 0-minute penalties taken, e.g., 0
-    ipent2: integer
-        Sum of individual 2-minute penalties taken, e.g., 0
-    ipent4: intger
-        Sum of individual 4-minute penalties taken, e.g., 0
-    ipent5: integer
-        Sum of individual 5-minute penalties taken, e.g., 0
-    ipent10: integer
-        Sum of individual 10-minute penalties taken, e.g., 0
-    ipend0: integer
-        Sum of individual 0-minute penalties drawn, e.g., 0
-    ipend2: integer
-        Sum of individual 2-minute penalties drawn, e.g., 0
-    ipend4: integer
-        Sum of individual 4-minute penalties drawn, e.g., 0
-    ipend5: integer
-        Sum of individual 5-minute penalties drawn, e.g., 0
-    ipend10: integer
-        Sum of individual 10-minute penalties drawn, e.g., 0
-    ozs: integer
-        Sum of changes with offensive zone starts, e.g., 1
-    nzs: integer
-        Sum of changes with neutral zone starts, e.g., 0
-    dzs: integer
-        Sum of changes with defensive zone starts, e.g., 0
-    otf: integer
-        Sum of changes on-the-fly, e.g., 0
-    gf: integer
-        Sum of goals scored while player is on-ice, e.g., 0
-    gf_adj: float
-        Sum of venue- and score-adjusted goals scored while player is on-ice, e.g., 0
-    hdgf: integer
-        Sum of high-danger goals scored while player is on-ice, e.g., 0
-    ga: integer
-        Sum of goals allowed while player is on-ice, e.g., 0
-    ga_adj: float
-        Sum of venue- and score-adjusted goals allowed while player is on-ice, e.g., 0
-    hdga: integer
-        Sum of high-danger goals allowed while player is on-ice, e.g., 0
-    xgf: float
-        Sum of expected goals generated while player is on-ice, e.g., 0.425891
-    xgf_adj: float
-        Sum of venue- and score-adjusted expected goals generated while player is on-ice, e.g., 0.388412
-    xga: float
-        Sum of expected goals allowed while player is on-ice, e.g., 0
-    xga_adj: float
-        Sum of venue- and score-adjusted expected goals allowed while player is on-ice, e.g., 0
-    sf: integer
-        Sum of shots taken while player is on-ice, e.g., 1
-    sf_adj: float
-        Sum of venue- and score-adjusted shots taken while player is on-ice, e.g., .93
-    hdsf: integer
-        Sum of high-danger shots taken while player is on-ice, e.g., 0
-    sa: integer
-        Sum of shots allowed while player is on-ice, e.g., 0
-    sa_adj: float
-        Sum of venue- and score-adjusted shots allowed while player is on-ice, e.g., 0
-    hdsa: integer
-        Sum of high-danger shots allowed while player is on-ice, e.g., 0
-    ff: integer
-        Sum of fenwick events generated while player is on-ice, e.g., 4
-    ff_adj: float
-        Sum of venue- and score-adjusted fenwick events generated while player is on-ice, e.g., 3.704
-    hdff: integer
-        Sum of high-danger fenwick events generated while player is on-ice, e.g., 0
-    fa: integer
-        Sum of fenwick events allowed while player is on-ice, e.g., 0
-    fa_adj: float
-        Sum of venue- and score-adjusted fenwick events allowed while player is on-ice, e.g., 0
-    hdfa: integer
-        Sum of high-danger fenwick events allowed while player is on-ice, e.g., 0
-    cf: integer
-        Sum of corsi events generated while player is on-ice, e.g., 7
-    cf_adj: float
-        Sum of venue- and score-adjusted corsi events generated while player is on-ice, e.g., 6.51
-    ca: integer
-        Sum of corsi events allowed while player is on-ice, e.g., 0
-    ca_adj: float
-        Sum of venue- and score-adjusted corsi events allowed while player is on-ice, e.g., 6.51
-    bsf: integer
-        Sum of shots taken that were ultimately blocked while player is on-ice, e.g., 3
-    bsa: integer
-        Sum of shots allowed that were ultimately blocked while player is on-ice, e.g., 0
-    msf: integer
-        Sum of shots taken that missed net while player is on-ice, e.g., 3
-    hdmsf: integer
-        Sum of high-danger shots taken that missed net while player is on-ice, e.g., 0
-    msa: integer
-        Sum of shots allowed that missed net while player is on-ice, e.g., 0
-    hdmsa: integer
-        Sum of high-danger shots allowed that missed net while player is on-ice, e.g., 0
-    hf: integer
-        Sum of hits dished out while player is on-ice, e.g., 0
-    ht: integer
-        Sum of hits taken while player is on-ice, e.g., 1
-    ozf: integer
-        Sum of offensive zone faceoffs that occur while player is on-ice, e.g., 1
-    nzf: integer
-        Sum of neutral zone faceoffs that occur while player is on-ice, e.g., 0
-    dzf: integer
-        Sum of defensive zone faceoffs that occur while player is on-ice, e.g., 1
-    fow: integer
-        Sum of faceoffs won while player is on-ice, e.g., 0
-    fol: integer
-        Sum of faceoffs lost while player is on-ice, e.g., 1
-    ozfw: integer
-        Sum of offensive zone faceoffs won while player is on-ice, e.g., 0
-    ozfl: integer
-        Sum of offensive zone faceoffs lost while player is on-ice, e.g., 1
-    nzfw: integer
-        Sum of neutral zone faceoffs won while player is on-ice, e.g., 0
-    nzfl: integer
-        Sum of neutral zone faceoffs lost while player is on-ice, e.g., 0
-    dzfw: integer
-        Sum of defensive zone faceoffs won while player is on-ice, e.g., 0
-    dzfl: integer
-        Sum of defensive zone faceoffs lost while player is on-ice, e.g., 0
-    pent0: integer
-        Sum of individual 0-minute penalties taken while player is on-ice, e.g., 0
-    pent2: integer
-        Sum of individual 2-minute penalties taken while player is on-ice, e.g., 0
-    pent4: intger
-        Sum of individual 4-minute penalties taken while player is on-ice, e.g., 0
-    pent5: integer
-        Sum of individual 5-minute penalties taken while player is on-ice, e.g., 0
-    pent10: integer
-        Sum of individual 10-minute penalties taken while player is on-ice, e.g., 0
-    pend0: integer
-        Sum of individual 0-minute penalties drawn while player is on-ice, e.g., 0
-    pend2: integer
-        Sum of individual 2-minute penalties drawn while player is on-ice, e.g., 0
-    pend4: integer
-        Sum of individual 4-minute penalties drawn while player is on-ice, e.g., 0
-    pend5: integer
-        Sum of individual 5-minute penalties drawn while player is on-ice, e.g., 0
-    pend10: integer
-        Sum of individual 10-minute penalties drawn while player is on-ice, e.g., 0
-
-    Examples
-    ----------
-
-    Basic play-by-play DataFrame
-    >>> raw_shifts = pd.read_csv('./raw_shifts.csv')
-    >>> raw_pbp = pd.read_csv('./raw_pbp.csv')
-    >>> pbp = prep_pbp(raw_pbp, raw_shifts)
+    Parameters:
+        df (pd.DataFrame):
+            Dataframe from the prep_pbp function with the default columns argument
+        level (str):
+            Level to aggregate stats, e.g., 'game'
+        score (bool):
+            Whether to aggregate to score state level
+        teammates (bool):
+            Whether to account for teammates when aggregating
+        opposition (bool):
+            Whether to account for opposition when aggregating
+
+    Returns:
+        season (int):
+            8-digit season code, e.g., 20232024
+        session (str):
+            Regular season or playoffs, e.g., R
+        game_id (int):
+            10-digit game identifier, e.g., 2023020015
+        game_date (str):
+            Date of game in Eastern time-zone, e.g., 2023-10-12
+        player (str):
+            Name of the player, e.g., FILIP.FORSBERG
+        player_id (str):
+            Player EH ID, e.g., FILIP.FORSBERG
+        position (str):
+            Player's position, e.g., L
+        team (str):
+            3-letter abbreviation of the player's team, e.g., NSH
+        opp_team: object
+            3-letter abbreviation of the opposing team, e.g., SEA
+        strength_state (str):
+            Strength state from the perspective of the event team, e.g., 5v5
+        score_state (str):
+            Score state from the perspective of the event team, e.g., 0v0
+        game_period (int):
+            Game period, e.g., 1
+        forwards (str):
+            Names of the event team's forwards that are on the ice during the event,
+            e.g., FILIP.FORSBERG, JUUSO.PARSSINEN, RYAN.O'REILLY
+        forwards_id (str):
+            EH IDs of the event team's forwards that are on the ice during the event,
+            e.g., FILIP.FORSBERG, JUUSO.PARSSINEN, RYAN.O'REILLY
+        defense (str):
+            Names of the event team's defensemen that are on the ice during the event,
+            e.g., ALEX.CARRIER, RYAN.MCDONAGH
+        defense_id (str):
+            EH IDs of the event team's defensemen that are on the ice during the event,
+            e.g., ALEX.CARRIER, RYAN.MCDONAGH
+        own_goalie (str):
+            Name of the goalie for the event team, e.g., JUUSE.SAROS
+        own_goalie_id (str):
+            Identifier for the event team goalie that can be used to match with Evolving Hockey data, e.g., JUUSE.SAROS
+        opp_forwards (str):
+            Names of the opponent's forwards that are on the ice during the event,
+            e.g., JARED.MCCANN, JORDAN.EBERLE, MATTY.BENIERS
+        opp_forwards_id (str):
+            EH IDs of the event team's forwards that are on the ice during the event,
+            e.g., JARED.MCCANN, JORDAN.EBERLE, MATTY.BENIERS
+        opp_defense(str):
+            Names of the opposing team's defensemen that are on the ice during the event,
+            e.g., JAMIE.OLEKSIAK, WILLIAM.BORGEN
+        opp_defense_id (str):
+            EH IDs of the opposing team's defensemen that are on the ice during the event,
+            e.g., JAMIE.OLEKSIAK, WILLIAM.BORGEN
+        opp_goalie (str):
+            Name of the opposing goalie for the event team, e.g., PHILIPP.GRUBAUER
+        opp_goalie_id (str):
+            Identifier for the opposing goalie that can be used to match with Evolving Hockey data,
+            e.g., PHILIPP.GRUBAUER
+        toi (float):
+            Time on-ice in minutes, e.g., 1.616667
+        g (float):
+            Number of individual goals scored, e.g, 0
+        a1 (float):
+            Number of primary assists, e.g, 0
+        a2 (float):
+            Number of secondary assists, e.g, 0
+        isf (float):
+            Number of indiviudal shots registered, e.g., 0
+        iff (float):
+            Number of indiviudal fenwick events registered, e.g., 0
+        icf (float):
+            Number of indiviudal corsi events registered, e.g., 0
+        ixg (float):
+            Sum value of individual predicted goals (xG), e.g., 0
+        gax (float):
+            Sum value of goals scored above expected, e.g., 0
+        ihdg (float):
+            Sum value of individual high-danger goals scored, e.g., 0
+        ihdf (float):
+            Sum value of individual high-danger fenwick events registered, e.g., 0
+        ihdsf (float):
+            Sum value of individual high-danger shots taken, e.g., 0
+        ihdm (float):
+            Sum value of individual high-danger shots missed, e.g., 0
+        imsf (float):
+            Sum value of individual missed shots, 0
+        isb (float):
+            Sum value of shots taken that were ultimately blocked, e.g., 0
+        ibs (float):
+            Sum value of opponent shots taken that the player ultimately blocked, e.g., 0
+        igive (float):
+            Sum of individual giveaways, e.g., 0
+        itake (float):
+            Sum of individual takeaways, e.g., 0
+        ihf (float):
+            Sum of individual hits for, e.g., 0
+        iht (float):
+            Sum of individual hits taken, e.g., 0
+        ifow (float):
+            Sum of individual faceoffs won, e.g., 0
+        ifol (float):
+            Sum of individual faceoffs lost, e.g., 0
+        iozfw (float):
+            Sum of individual faceoffs won in offensive zone, e.g., 0
+        iozfl (float):
+            Sum of individual faceoffs lost in offensive zone, e.g., 0
+        inzfw (float):
+            Sum of individual faceoffs won in neutral zone, e.g., 0
+        inzfl (float):
+            Sum of individual faceoffs lost in neutral zone, e.g., 0
+        idzfw (float):
+            Sum of individual faceoffs won in defensive zone, e.g., 0
+        idzfl (float):
+            Sum of individual faceoffs lost in defensive zone, e.g., 0
+        a1_xg (float):
+            Sum of xG from primary assists, e.g., 0
+        a2_xg (float):
+            Sum of xG from secondary assists, e.g., 0
+        ipent0 (float):
+            Sum of individual 0-minute penalties taken, e.g., 0
+        ipent2 (float):
+            Sum of individual 2-minute penalties taken, e.g., 0
+        ipent4 (float):
+            Sum of individual 4-minute penalties taken, e.g., 0
+        ipent5 (float):
+            Sum of individual 5-minute penalties taken, e.g., 0
+        ipent10 (float):
+            Sum of individual 10-minute penalties taken, e.g., 0
+        ipend0 (float):
+            Sum of individual 0-minute penalties drawn, e.g., 0
+        ipend2 (float):
+            Sum of individual 2-minute penalties drawn, e.g., 0
+        ipend4 (float):
+            Sum of individual 4-minute penalties drawn, e.g., 0
+        ipend5 (float):
+            Sum of individual 5-minute penalties drawn, e.g., 0
+        ipend10 (float):
+            Sum of individual 10-minute penalties drawn, e.g., 0
+        ozs (float):
+            Sum of changes with offensive zone starts, e.g., 0
+        nzs (float):
+            Sum of changes with neutral zone starts, e.g., 0
+        dzs (float):
+            Sum of changes with defensive zone starts, e.g., 1
+        otf (float):
+            Sum of changes on-the-fly, e.g., 0
+        gf (float):
+            Sum of goals scored while player is on-ice, e.g., 0
+        gf_adj (float):
+            Sum of venue- and score-adjusted goals scored while player is on-ice, e.g., 0
+        hdgf (float):
+            Sum of high-danger goals scored while player is on-ice, e.g., 0
+        ga (float):
+            Sum of goals allowed while player is on-ice, e.g., 0
+        ga_adj (float):
+            Sum of venue- and score-adjusted goals allowed while player is on-ice, e.g., 0
+        hdga (float):
+            Sum of high-danger goals allowed while player is on-ice, e.g., 0
+        xgf (float):
+            Sum of expected goals generated while player is on-ice, e.g., 0.017266
+        xgf_adj (float):
+            Sum of venue- and score-adjusted expected goals generated while player is on-ice, e.g., 0.016472
+        xga (float):
+            Sum of expected goals allowed while player is on-ice, e.g., 0.123475
+        xga_adj (float):
+            Sum of venue- and score-adjusted expected goals allowed while player is on-ice, e.g., 0.129772
+        sf (float):
+            Sum of shots taken while player is on-ice, e.g., 1
+        sf_adj (float):
+            Sum of venue- and score-adjusted shots taken while player is on-ice, e.g., .972
+        hdsf (float):
+            Sum of high-danger shots taken while player is on-ice, e.g., 0
+        sa (float):
+            Sum of shots allowed while player is on-ice, e.g., 0
+        sa_adj (float):
+            Sum of venue- and score-adjusted shots allowed while player is on-ice, e.g., 0
+        hdsa (float):
+            Sum of high-danger shots allowed while player is on-ice, e.g., 0
+        ff (float):
+            Sum of fenwick events generated while player is on-ice, e.g., 1
+        ff_adj (float):
+            Sum of venue- and score-adjusted fenwick events generated while player is on-ice, e.g., 0.968
+        hdff (float):
+            Sum of high-danger fenwick events generated while player is on-ice, e.g., 0
+        fa (float):
+            Sum of fenwick events allowed while player is on-ice, e.g., 1
+        fa_adj (float):
+            Sum of venue- and score-adjusted fenwick events allowed while player is on-ice, e.g., 1.034
+        hdfa (float):
+            Sum of high-danger fenwick events allowed while player is on-ice, e.g., 1
+        cf (float):
+            Sum of corsi events generated while player is on-ice, e.g., 1
+        cf_adj (float):
+            Sum of venue- and score-adjusted corsi events generated while player is on-ice, e.g., 0.970
+        ca (float):
+            Sum of corsi events allowed while player is on-ice, e.g., 2
+        ca_adj (float):
+            Sum of venue- and score-adjusted corsi events allowed while player is on-ice, e.g., 2.064
+        bsf (float):
+            Sum of shots taken that were ultimately blocked while player is on-ice, e.g., 0
+        bsa (float):
+            Sum of shots allowed that were ultimately blocked while player is on-ice, e.g., 1
+        msf (float):
+            Sum of shots taken that missed net while player is on-ice, e.g., 0
+        hdmsf (float):
+            Sum of high-danger shots taken that missed net while player is on-ice, e.g., 0
+        msa (float):
+            Sum of shots allowed that missed net while player is on-ice, e.g., 1
+        hdmsa (float):
+            Sum of high-danger shots allowed that missed net while player is on-ice, e.g., 1
+        hf (float):
+            Sum of hits dished out while player is on-ice, e.g., 0
+        ht (float):
+            Sum of hits taken while player is on-ice, e.g., 0
+        ozf (float):
+            Sum of offensive zone faceoffs that occur while player is on-ice, e.g., 0
+        nzf (float):
+            Sum of neutral zone faceoffs that occur while player is on-ice, e.g., 0
+        dzf (float):
+            Sum of defensive zone faceoffs that occur while player is on-ice, e.g., 1
+        fow (float):
+            Sum of faceoffs won while player is on-ice, e.g., 1
+        fol (float):
+            Sum of faceoffs lost while player is on-ice, e.g., 0
+        ozfw (float):
+            Sum of offensive zone faceoffs won while player is on-ice, e.g., 0
+        ozfl (float):
+            Sum of offensive zone faceoffs lost while player is on-ice, e.g., 1
+        nzfw (float):
+            Sum of neutral zone faceoffs won while player is on-ice, e.g., 0
+        nzfl (float):
+            Sum of neutral zone faceoffs lost while player is on-ice, e.g., 0
+        dzfw (float):
+            Sum of defensive zone faceoffs won while player is on-ice, e.g., 1
+        dzfl (float):
+            Sum of defensive zone faceoffs lost while player is on-ice, e.g., 0
+        pent0 (float):
+            Sum of individual 0-minute penalties taken while player is on-ice, e.g., 0
+        pent2 (float):
+            Sum of individual 2-minute penalties taken while player is on-ice, e.g., 0
+        pent4 (float):
+            Sum of individual 4-minute penalties taken while player is on-ice, e.g., 0
+        pent5 (float):
+            Sum of individual 5-minute penalties taken while player is on-ice, e.g., 0
+        pent10 (float):
+            Sum of individual 10-minute penalties taken while player is on-ice, e.g., 0
+        pend0 (float):
+            Sum of individual 0-minute penalties drawn while player is on-ice, e.g., 0
+        pend2 (float):
+            Sum of individual 2-minute penalties drawn while player is on-ice, e.g., 0
+        pend4 (float):
+            Sum of individual 4-minute penalties drawn while player is on-ice, e.g., 0
+        pend5 (float):
+            Sum of individual 5-minute penalties drawn while player is on-ice, e.g., 0
+        pend10 (float):
+            Sum of individual 10-minute penalties drawn while player is on-ice, e.g., 0
+
+    Examples:
+        Basic play-by-play DataFrame
+        >>> shifts_raw = pd.read_csv('./raw_shifts.csv')
+        >>> pbp_raw = pd.read_csv('./raw_pbp.csv')
+        >>> pbp = prep_pbp(pbp_raw, shifts_raw)
 
-    Basic game-level stats, with no teammates or opposition
-    >>> stats = prep_stats(pbp)
+        Basic game-level stats, with no teammates or opposition
+        >>> stats = prep_stats(pbp)
 
-    Period-level stats, grouped by teammates
-    >>> stats = prep_stats(pbp, level = 'period', teammates=True)
+        Period-level stats, grouped by teammates
+        >>> stats = prep_stats(pbp, level = 'period', teammates=True)
 
-    Session-level (e.g., regular seasion) stats, grouped by teammates and opposition
-    >>> stats = prep_stats(pbp, level='session', teammates=True, opposition=True)
+        Session-level (e.g., regular seasion) stats, grouped by teammates and opposition
+        >>> stats = prep_stats(pbp, level='session', teammates=True, opposition=True)
 
     """
 
     ind = prep_ind(df, level, score, teammates, opposition)
 
     oi = prep_oi(df, level, score, teammates, opposition)
 
@@ -1160,216 +1153,213 @@
     position: str,
     level: str = "game",
     score: bool = False,
     teammates: bool = False,
     opposition: bool = False,
 ):
     """
-    Prepares an individual and on-ice stats dataframe using EvolvingHockey data,
+    Prepares a line stats dataframe using EvolvingHockey data,
     aggregated to desired level. Capable of returning cuts that account for strength state,
     period, score state, teammates, and opposition.
 
-    Returns a DataFrame.
+    Returns a Pandas DataFrame.
 
-    Parameters
-    ----------
-    data : dataframe
-        Dataframe from the prep_pbp function with the default columns argument
-    position : str
-        Used to indicate whether to include forwards or defense
-    level : str, default='game'
-        Level to aggregate stats, e.g., 'game'
-    score: bool, default=False
-        Whether to aggregate to score state level
-    teammates: bool, default=False
-        Whether to account for teammates when aggregating
-    opposition: bool, default=False
-        Whether to account for opposition when aggregating
-
-    Returns
-    ----------
-    season: integer
-        8-digit season code, e.g., 20222023
-    session: object
-        Regular season or playoffs, e.g., R
-    game_id: integer
-        10-digit game identifier, e.g.,
-    game_date: object
-        Date of game in Eastern time-zone, e.g.,
-    team: object
-        3-letter abbreviation of the player's team, e.g., NSH
-    opp_team: object
-        3-letter abbreviation of the opposing team, e.g., NJD
-    strength_state: object
-        Strength state from the perspective of the event team, e.g., 5v4
-    score_state: object
-        Score state from the perspective of the event team, e.g., 0v0
-    game_period: integer
-        Game period, e.g., 1
-    forwards: object
-        Names of the event team's forwards that are on the ice during the event,
-        e.g., FILIP.FORSBERG, MATT.DUCHENE, MIKAEL.GRANLUND, RYAN.JOHANSEN
-    forwards_id: object
-        EH IDs of the event team's forwards that are on the ice during the event,
-        e.g., FILIP.FORSBERG, MATT.DUCHENE, MIKAEL.GRANLUND, RYAN.JOHANSEN
-    defense: object
-        Names of the event team's defensemen that are on the ice during the event,
-        e.g., ROMAN.JOSI
-    defense_id: object
-        EH IDs of the event team's defensemen that are on the ice during the event,
-        e.g., ROMAN.JOSI
-    own_goalie: object
-        Name of the goalie for the event team, e.g., JUUSE.SAROS
-    own_goalie_id: object
-        Identifier for the event team goalie that can be used to match with Evolving Hockey data, e.g., JUUSE.SAROS
-    opp_forwards: object
-        Names of the opponent's forwards that are on the ice during the event,
-        e.g., DAWSON.MERCER, ERIK.HAULA
-    opp_forwards_id: object
-        EH IDs of the event team's forwards that are on the ice during the event,
-        e.g., DAWSON.MERCER, ERIK.HAULA
-    opp_defense: object
-        Names of the opposing team's defensemen that are on the ice during the event,
-        e.g., DAMON.SEVERSON, RYAN.GRAVES
-    opp_defense_id: object
-        EH IDs of the opposing team's defensemen that are on the ice during the event,
-        e.g., DAMON.SEVERSON, RYAN.GRAVES
-    opp_goalie: object
-        Name of the opposing goalie for the event team, e.g., MACKENZIE.BLACKWOOD
-    opp_goalie_id: object
-        Identifier for the opposing goalie that can be used to match with Evolving Hockey data, e.g., MACKENZIE.BLACKWOOD
-    toi: float
-        Time on-ice in minutes, e.g., 1.616667
-    gf: integer
-        Sum of goals scored while line is on-ice, e.g., 0
-    gf_adj: float
-        Sum of venue- and score-adjusted goals scored while line is on-ice, e.g., 0
-    hdgf: integer
-        Sum of high-danger goals scored while line is on-ice, e.g., 0
-    ga: integer
-        Sum of goals allowed while line is on-ice, e.g., 0
-    ga_adj: float
-        Sum of venue- and score-adjusted goals allowed while line is on-ice, e.g., 0
-    hdga: integer
-        Sum of high-danger goals allowed while line is on-ice, e.g., 0
-    xgf: float
-        Sum of expected goals generated while line is on-ice, e.g., 0.425891
-    xgf_adj: float
-        Sum of venue- and score-adjusted expected goals generated while line is on-ice, e.g., 0.388412
-    xga: float
-        Sum of expected goals allowed while line is on-ice, e.g., 0
-    xga_adj: float
-        Sum of venue- and score-adjusted expected goals allowed while line is on-ice, e.g., 0
-    sf: integer
-        Sum of shots taken while line is on-ice, e.g., 1
-    sf_adj: float
-        Sum of venue- and score-adjusted shots taken while line is on-ice, e.g., .93
-    hdsf: integer
-        Sum of high-danger shots taken while line is on-ice, e.g., 0
-    sa: integer
-        Sum of shots allowed while line is on-ice, e.g., 0
-    sa_adj: float
-        Sum of venue- and score-adjusted shots allowed while line is on-ice, e.g., 0
-    hdsa: integer
-        Sum of high-danger shots allowed while line is on-ice, e.g., 0
-    ff: integer
-        Sum of fenwick events generated while line is on-ice, e.g., 4
-    ff_adj: float
-        Sum of venue- and score-adjusted fenwick events generated while line is on-ice, e.g., 3.704
-    hdff: integer
-        Sum of high-danger fenwick events generated while line is on-ice, e.g., 0
-    fa: integer
-        Sum of fenwick events allowed while line is on-ice, e.g., 0
-    fa_adj: float
-        Sum of venue- and score-adjusted fenwick events allowed while line is on-ice, e.g., 0
-    hdfa: integer
-        Sum of high-danger fenwick events allowed while line is on-ice, e.g., 0
-    cf: integer
-        Sum of corsi events generated while line is on-ice, e.g., 7
-    cf_adj: float
-        Sum of venue- and score-adjusted corsi events generated while line is on-ice, e.g., 6.51
-    ca: integer
-        Sum of corsi events allowed while line is on-ice, e.g., 0
-    ca_adj: float
-        Sum of venue- and score-adjusted corsi events allowed while line is on-ice, e.g., 6.51
-    bsf: integer
-        Sum of shots taken that were ultimately blocked while line is on-ice, e.g., 3
-    bsa: integer
-        Sum of shots allowed that were ultimately blocked while line is on-ice, e.g., 0
-    msf: integer
-        Sum of shots taken that missed net while line is on-ice, e.g., 3
-    hdmsf: integer
-        Sum of high-danger shots taken that missed net while line is on-ice, e.g., 0
-    msa: integer
-        Sum of shots allowed that missed net while line is on-ice, e.g., 0
-    hdmsa: integer
-        Sum of high-danger shots allowed that missed net while line is on-ice, e.g., 0
-    hf: integer
-        Sum of hits dished out while line is on-ice, e.g., 0
-    ht: integer
-        Sum of hits taken while line is on-ice, e.g., 1
-    ozf: integer
-        Sum of offensive zone faceoffs that occur while line is on-ice, e.g., 1
-    nzf: integer
-        Sum of neutral zone faceoffs that occur while line is on-ice, e.g., 0
-    dzf: integer
-        Sum of defensive zone faceoffs that occur while line is on-ice, e.g., 1
-    fow: integer
-        Sum of faceoffs won while line is on-ice, e.g., 0
-    fol: integer
-        Sum of faceoffs lost while line is on-ice, e.g., 1
-    ozfw: integer
-        Sum of offensive zone faceoffs won while line is on-ice, e.g., 0
-    ozfl: integer
-        Sum of offensive zone faceoffs lost while line is on-ice, e.g., 1
-    nzfw: integer
-        Sum of neutral zone faceoffs won while line is on-ice, e.g., 0
-    nzfl: integer
-        Sum of neutral zone faceoffs lost while line is on-ice, e.g., 0
-    dzfw: integer
-        Sum of defensive zone faceoffs won while line is on-ice, e.g., 0
-    dzfl: integer
-        Sum of defensive zone faceoffs lost while line is on-ice, e.g., 0
-    pent0: integer
-        Sum of individual 0-minute penalties taken while line is on-ice, e.g., 0
-    pent2: integer
-        Sum of individual 2-minute penalties taken while line is on-ice, e.g., 0
-    pent4: intger
-        Sum of individual 4-minute penalties taken while line is on-ice, e.g., 0
-    pent5: integer
-        Sum of individual 5-minute penalties taken while line is on-ice, e.g., 0
-    pent10: integer
-        Sum of individual 10-minute penalties taken while line is on-ice, e.g., 0
-    pend0: integer
-        Sum of individual 0-minute penalties drawn while line is on-ice, e.g., 0
-    pend2: integer
-        Sum of individual 2-minute penalties drawn while line is on-ice, e.g., 0
-    pend4: integer
-        Sum of individual 4-minute penalties drawn while line is on-ice, e.g., 0
-    pend5: integer
-        Sum of individual 5-minute penalties drawn while line is on-ice, e.g., 0
-    pend10: integer
-        Sum of individual 10-minute penalties drawn while line is on-ice, e.g., 0
-
-    Examples
-    ----------
-
-    Basic play-by-play DataFrame
-    >>> raw_shifts = pd.read_csv('./raw_shifts.csv')
-    >>> raw_pbp = pd.read_csv('./raw_pbp.csv')
-    >>> pbp = prep_pbp(raw_pbp, raw_shifts)
+    Parameters:
+        data (pd.DataFrame):
+            Dataframe from the prep_pbp function with the default columns argument
+        position (str):
+            Position to aggregate, forwards or defense, e.g., 'f'
+        level (str):
+            Level to aggregate stats, e.g., 'game'
+        score (bool):
+            Whether to aggregate to score state level
+        teammates (bool):
+            Whether to account for teammates when aggregating
+        opposition (bool):
+            Whether to account for opposition when aggregating
+
+    Returns:
+        season (int):
+            8-digit season code, e.g., 20232024
+        session (str):
+            Regular season or playoffs, e.g., R
+        game_id (int):
+            10-digit game identifier, e.g., 2023020015
+        game_date (str):
+            Date of game in Eastern time-zone, e.g., 2023-10-12
+        team (str):
+            3-letter abbreviation of the line's team, e.g., NSH
+        opp_team (str):
+            3-letter abbreviation of the opposing team, e.g., SEA
+        strength_state (str):
+            Strength state from the perspective of the event team, e.g., 5v5
+        score_state (str):
+            Score state from the perspective of the event team, e.g., 0v0
+        game_period (int):
+            Game period, e.g., 1
+        forwards (str):
+            Names of the event team's forwards that are on the ice during the event,
+            e.g., FILIP.FORSBERG, JUUSO.PARSSINEN, RYAN.O'REILLY
+        forwards_id (str):
+            EH IDs of the event team's forwards that are on the ice during the event,
+            e.g., FILIP.FORSBERG, JUUSO.PARSSINEN, RYAN.O'REILLY
+        defense (str):
+            Names of the event team's defensemen that are on the ice during the event,
+            e.g., ALEX.CARRIER, RYAN.MCDONAGH
+        defense_id (str):
+            EH IDs of the event team's defensemen that are on the ice during the event,
+            e.g., ALEX.CARRIER, RYAN.MCDONAGH
+        own_goalie (str):
+            Name of the goalie for the event team, e.g., JUUSE.SAROS
+        own_goalie_id (str):
+            Identifier for the event team goalie that can be used to match with Evolving Hockey data, e.g., JUUSE.SAROS
+        opp_forwards (str):
+            Names of the opponent's forwards that are on the ice during the event,
+            e.g., JARED.MCCANN, JORDAN.EBERLE, MATTY.BENIERS
+        opp_forwards_id (str):
+            EH IDs of the event team's forwards that are on the ice during the event,
+            e.g., JARED.MCCANN, JORDAN.EBERLE, MATTY.BENIERS
+        opp_defense (str):
+            Names of the opposing team's defensemen that are on the ice during the event,
+            e.g., JAMIE.OLEKSIAK, WILLIAM.BORGEN
+        opp_defense_id (str):
+            EH IDs of the opposing team's defensemen that are on the ice during the event,
+            e.g., JAMIE.OLEKSIAK, WILLIAM.BORGEN
+        opp_goalie (str):
+            Name of the opposing goalie for the event team, e.g., PHILIPP.GRUBAUER
+        opp_goalie_id (str):
+            Identifier for the opposing goalie that can be used to match with Evolving Hockey data,
+            e.g., PHILIPP.GRUBAUER
+        toi (float):
+            Time on-ice in minutes, e.g., 1.616667
+        gf (float):
+            Sum of goals scored while line is on-ice, e.g., 0
+        gf_adj (float):
+            Sum of venue- and score-adjusted goals scored while line is on-ice, e.g., 0
+        hdgf (float):
+            Sum of high-danger goals scored while line is on-ice, e.g., 0
+        ga (float):
+            Sum of goals allowed while line is on-ice, e.g., 0
+        ga_adj (float):
+            Sum of venue- and score-adjusted goals allowed while line is on-ice, e.g., 0
+        hdga (float):
+            Sum of high-danger goals allowed while line is on-ice, e.g., 0
+        xgf (float):
+            Sum of expected goals generated while line is on-ice, e.g., 0.017266
+        xgf_adj (float):
+            Sum of venue- and score-adjusted expected goals generated while line is on-ice, e.g., 0.016472
+        xga (float):
+            Sum of expected goals allowed while line is on-ice, e.g., 0.123475
+        xga_adj (float):
+            Sum of venue- and score-adjusted expected goals allowed while line is on-ice, e.g., 0.129772
+        sf (float):
+            Sum of shots taken while line is on-ice, e.g., 1
+        sf_adj (float):
+            Sum of venue- and score-adjusted shots taken while line is on-ice, e.g., .972
+        hdsf (float):
+            Sum of high-danger shots taken while line is on-ice, e.g., 0
+        sa (float):
+            Sum of shots allowed while line is on-ice, e.g., 0
+        sa_adj (float):
+            Sum of venue- and score-adjusted shots allowed while line is on-ice, e.g., 0
+        hdsa (float):
+            Sum of high-danger shots allowed while line is on-ice, e.g., 0
+        ff (float):
+            Sum of fenwick events generated while line is on-ice, e.g., 1
+        ff_adj (float):
+            Sum of venue- and score-adjusted fenwick events generated while line is on-ice, e.g., 0.968
+        hdff (float):
+            Sum of high-danger fenwick events generated while line is on-ice, e.g., 0
+        fa (float):
+            Sum of fenwick events allowed while line is on-ice, e.g., 1
+        fa_adj (float):
+            Sum of venue- and score-adjusted fenwick events allowed while line is on-ice, e.g., 1.034
+        hdfa (float):
+            Sum of high-danger fenwick events allowed while line is on-ice, e.g., 1
+        cf (float):
+            Sum of corsi events generated while line is on-ice, e.g., 1
+        cf_adj (float):
+            Sum of venue- and score-adjusted corsi events generated while line is on-ice, e.g., 0.970
+        ca (float):
+            Sum of corsi events allowed while line is on-ice, e.g., 2
+        ca_adj (float):
+            Sum of venue- and score-adjusted corsi events allowed while line is on-ice, e.g., 2.064
+        bsf (float):
+            Sum of shots taken that were ultimately blocked while line is on-ice, e.g., 0
+        bsa (float):
+            Sum of shots allowed that were ultimately blocked while line is on-ice, e.g., 1
+        msf (float):
+            Sum of shots taken that missed net while line is on-ice, e.g., 0
+        hdmsf (float):
+            Sum of high-danger shots taken that missed net while line is on-ice, e.g., 0
+        msa (float):
+            Sum of shots allowed that missed net while line is on-ice, e.g., 1
+        hdmsa (float):
+            Sum of high-danger shots allowed that missed net while line is on-ice, e.g., 1
+        hf (float):
+            Sum of hits dished out while line is on-ice, e.g., 0
+        ht (float):
+            Sum of hits taken while line is on-ice, e.g., 0
+        ozf (float):
+            Sum of offensive zone faceoffs that occur while line is on-ice, e.g., 0
+        nzf (float):
+            Sum of neutral zone faceoffs that occur while line is on-ice, e.g., 0
+        dzf (float):
+            Sum of defensive zone faceoffs that occur while line is on-ice, e.g., 1
+        fow (float):
+            Sum of faceoffs won while line is on-ice, e.g., 1
+        fol (float):
+            Sum of faceoffs lost while line is on-ice, e.g., 0
+        ozfw (float):
+            Sum of offensive zone faceoffs won while line is on-ice, e.g., 0
+        ozfl (float):
+            Sum of offensive zone faceoffs lost while line is on-ice, e.g., 1
+        nzfw (float):
+            Sum of neutral zone faceoffs won while line is on-ice, e.g., 0
+        nzfl (float):
+            Sum of neutral zone faceoffs lost while line is on-ice, e.g., 0
+        dzfw (float):
+            Sum of defensive zone faceoffs won while line is on-ice, e.g., 1
+        dzfl (float):
+            Sum of defensive zone faceoffs lost while line is on-ice, e.g., 0
+        pent0 (float):
+            Sum of individual 0-minute penalties taken while line is on-ice, e.g., 0
+        pent2 (float):
+            Sum of individual 2-minute penalties taken while line is on-ice, e.g., 0
+        pent4 (float):
+            Sum of individual 4-minute penalties taken while line is on-ice, e.g., 0
+        pent5 (float):
+            Sum of individual 5-minute penalties taken while line is on-ice, e.g., 0
+        pent10 (float):
+            Sum of individual 10-minute penalties taken while line is on-ice, e.g., 0
+        pend0 (float):
+            Sum of individual 0-minute penalties drawn while line is on-ice, e.g., 0
+        pend2 (float):
+            Sum of individual 2-minute penalties drawn while line is on-ice, e.g., 0
+        pend4 (float):
+            Sum of individual 4-minute penalties drawn while line is on-ice, e.g., 0
+        pend5 (float):
+            Sum of individual 5-minute penalties drawn while line is on-ice, e.g., 0
+        pend10 (float):
+            Sum of individual 10-minute penalties drawn while line is on-ice, e.g., 0
+
+    Examples:
+        Basic play-by-play DataFrame
+        >>> shifts_raw = pd.read_csv('./raw_shifts.csv')
+        >>> pbp_raw = pd.read_csv('./raw_pbp.csv')
+        >>> pbp = prep_pbp(pbp_raw, shifts_raw)
 
-    Basic game-level stats for forwards, with no teammates or opposition
-    >>> lines = prep_lines(pbp, position='f')
+        Basic game-level stats for forwards, with no teammates or opposition
+        >>> lines = prep_lines(pbp, position='f')
 
-    Period-level stats for defense, grouped by teammates
-    >>> lines = prep_lines(pbp, position='d', level='period', teammates=True)
+        Period-level stats for defense, grouped by teammates
+        >>> lines = prep_lines(pbp, position='d', level='period', teammates=True)
 
-    Session-level (e.g., regular seasion) stats, grouped by teammates and opposition
-    >>> lines = prep_lines(pbp, position='f', level='session', teammates=True, opposition=True)
+        Session-level (e.g., regular seasion) stats, grouped by teammates and opposition
+        >>> lines = prep_lines(pbp, position='f', level='session', teammates=True, opposition=True)
 
     """
 
     # Creating the "for" dataframe
 
     # Accounting for desired level of aggregation
 
@@ -1667,15 +1657,15 @@
         "pen4",
         "pen5",
         "pen10",
     ]
 
     agg_stats = {x: "sum" for x in stats if x in data.columns}
 
-    # Aggregating "aggainst" dataframe
+    # Aggregating "against" dataframe
 
     lines_a = data.groupby(group_list, as_index=False, dropna=False).agg(agg_stats)
 
     # Creating the dictionary to change column names
 
     columns = [
         "xga",
@@ -1897,15 +1887,15 @@
     ]
 
     cols = [x for x in cols if x in lines]
 
     for col in cols:
         lines[col] = lines[col].fillna("EMPTY")
 
-    lines.toi = lines.toi_x + lines.toi
+    lines.toi = (lines.toi_x + lines.toi) / 60
 
     lines = lines.drop(columns="toi_x")
 
     lines["ozf"] = lines.ozfw + lines.ozfl
 
     lines["nzf"] = lines.nzfw + lines.nzfl
 
@@ -2071,34 +2061,177 @@
 
 
 # Function to prep the team stats
 def prep_team(
     data: pd.DataFrame, level: str = "game", strengths: bool = True, score: bool = False
 ) -> pd.DataFrame:
     """
-    Prepares an individual and on-ice stats dataframe using EvolvingHockey data,
+    Prepares a team stats dataframe using EvolvingHockey data,
     aggregated to desired level. Capable of returning cuts that account for strength state,
-    period, score state, teammates, and opposition.
+    period, and score state.
 
-    Returns a DataFrame.
+    Returns a Pandas DataFrame.
 
-    Parameters
-    ----------
-    data : pd.Dataframe
-        Pandas DataFrame from the prep_pbp function with the default columns argument
-    level : str, default='game'
-        Level to aggregate stats, e.g., 'game'
-    strengths: bool, default=True
-        Whether to aggregate to strength-state level
-    score: bool, default=False
-        Whether to aggregate to score state level
+    Parameters:
+        data (pd.DataFrame):
+            Dataframe from the prep_pbp function with the default columns argument
+        level (str):
+            Level to aggregate stats, e.g., 'game'
+        strengths (bool):
+            Whether to aggregate to strength state level, e.g., True
+        score (bool):
+            Whether to aggregate to score state level
+
+    Returns:
+        season (int):
+            8-digit season code, e.g., 20232024
+        session (str):
+            Regular season or playoffs, e.g., R
+        game_id (int):
+            10-digit game identifier, e.g., 2023020044
+        game_date (str):
+            Date of game in Eastern time-zone, e.g., 2023-10-17
+        team (str):
+            3-letter abbreviation of the team, e.g., NSH
+        opp_team (str):
+            3-letter abbreviation of the opposing team, e.g., EDM
+        strength_state (str):
+            Strength state from the perspective of the event team, e.g., 5v5
+        score_state (str):
+            Score state from the perspective of the event team, e.g., 1v6
+        game_period (int):
+            Game period, e.g., 3
+        toi (float):
+            Time on-ice in minutes, e.g., 18
+        gf (float):
+            Sum of goals scored, e.g., 0
+        gf_adj (float):
+            Sum of venue- and score-adjusted goals scored, e.g., 0
+        hdgf (float):
+            Sum of high-danger goals scored, e.g., 0
+        ga (float):
+            Sum of goals allowed, e.g., 0
+        ga_adj (float):
+            Sum of venue- and score-adjusted goals allowed, e.g., 0
+        hdga (float):
+            Sum of high-danger goals allowed, e.g., 0
+        xgf (float):
+            Sum of expected goals generated, e.g., 0.957070
+        xgf_adj (float):
+            Sum of venue- and score-adjusted expected goals generated, e.g., 0.883376
+        xga (float):
+            Sum of expected goals allowed, e.g., 0.535971
+        xga_adj (float):
+            Sum of venue- and score-adjusted expected goals allowed, e.g., 0.584744
+        sf (float):
+            Sum of shots taken, e.g., 10
+        sf_adj (float):
+            Sum of venue- and score-adjusted shots taken, e.g., 8.620
+        hdsf (float):
+            Sum of high-danger shots taken, e.g., 2
+        sa (float):
+            Sum of shots allowed, e.g., 4
+        sa_adj (float):
+            Sum of venue- and score-adjusted shots allowed, e.g., 4.764
+        hdsa (float):
+            Sum of high-danger shots allowed, e.g., 0
+        ff (float):
+            Sum of fenwick events generated, e.g., 14
+        ff_adj (float):
+            Sum of venue- and score-adjusted fenwick events generated, e.g., 12.026
+        hdff (float):
+            Sum of high-danger fenwick events generated, e.g., 2
+        fa (float):
+            Sum of fenwick events allowed, e.g., 8
+        fa_adj (float):
+            Sum of venue- and score-adjusted fenwick events allowed, e.g., 9.576
+        hdfa (float):
+            Sum of high-danger fenwick events allowed, e.g., 1
+        cf (float):
+            Sum of corsi events generated, e.g., 16
+        cf_adj (float):
+            Sum of venue- and score-adjusted corsi events generated, e.g., 13.488
+        ca (float):
+            Sum of corsi events allowed, e.g., 12.0
+        ca_adj (float):
+            Sum of venue- and score-adjusted corsi events allowed, e.g., 14.760
+        bsf (float):
+            Sum of shots taken that were ultimately blocked, e.g., 4
+        bsa (float):
+            Sum of shots allowed that were ultimately blocked, e.g., 2
+        msf (float):
+            Sum of shots taken that missed net, e.g., 4
+        hdmsf (float):
+            Sum of high-danger shots taken that missed net, e.g., 0
+        msa (float):
+            Sum of shots allowed that missed net, e.g., 4
+        hdmsa (float):
+            Sum of high-danger shots allowed that missed net, e.g., 1
+        ozf (float):
+            Sum of offensive zone faceoffs that occur, e.g., 6
+        nzf (float):
+            Sum of neutral zone faceoffs that occur, e.g., 4
+        dzf (float):
+            Sum of defensive zone faceoffs that occur, e.g., 6
+        fow (float):
+            Sum of faceoffs won, e.g., 8
+        fol (float):
+            Sum of faceoffs lost, e.g., 11
+        ozfw (float):
+            Sum of offensive zone faceoffs won, e.g., 3
+        ozfl (float):
+            Sum of offensive zone faceoffs lost, e.g., 1
+        nzfw (float):
+            Sum of neutral zone faceoffs won, e.g., 2
+        nzfl (float):
+            Sum of neutral zone faceoffs lost, e.g., 3
+        dzfw (float):
+            Sum of defensive zone faceoffs won, e.g., 3
+        dzfl (float):
+            Sum of defensive zone faceoffs lost, e.g., 7
+        hf (float):
+            Sum of hits dished out, e.g., 7
+        ht (float):
+            Sum of hits taken, e.g., 5
+        give (float):
+            Sum of giveaways, e.g., 5
+        take (float):
+            Sum of takeaways, e.g., 1
+        pent0 (float):
+            Sum of individual 0-minute penalties taken, e.g., 0
+        pent2 (float):
+            Sum of individual 2-minute penalties taken, e.g., 0
+        pent4 (float):
+            Sum of individual 4-minute penalties taken, e.g., 0
+        pent5 (float):
+            Sum of individual 5-minute penalties taken, e.g., 0
+        pent10 (float):
+            Sum of individual 10-minute penalties taken, e.g., 0
+        pend0 (float):
+            Sum of individual 0-minute penalties drawn, e.g., 0
+        pend2 (float):
+            Sum of individual 2-minute penalties drawn, e.g., 0
+        pend4 (float):
+            Sum of individual 4-minute penalties drawn, e.g., 0
+        pend5 (float):
+            Sum of individual 5-minute penalties drawn, e.g., 0
+        pend10 (float):
+            Sum of individual 10-minute penalties drawn, e.g., 0
+
+    Examples:
+        Basic play-by-play DataFrame
+        >>> shifts_raw = pd.read_csv('./raw_shifts.csv')
+        >>> pbp_raw = pd.read_csv('./raw_pbp.csv')
+        >>> pbp = prep_pbp(pbp_raw, shifts_raw)
 
+        Basic game-level stats for teams
+        >>> team = prep_team(pbp)
 
-    Returns
-    ----------
+        Period-level team stats, grouped by score state
+        >>> team = prep_team(pbp, level='period', score=True)
     """
 
     # Getting the "for" stats
 
     group_list = ["season", "session", "event_team"]
 
     if strengths is True:
@@ -2456,14 +2589,16 @@
     team_stats = team_stats[cols]
 
     return team_stats
 
 
 # Function to prep the GAR dataframe
 def prep_gar(skater_data: pd.DataFrame, goalie_data: pd.DataFrame) -> pd.DataFrame:
+    """Docstring here"""
+
     gar = pd.concat([skater_data, goalie_data], ignore_index=True)
 
     new_cols = {x: x.replace(" ", "_").lower() for x in gar.columns}
 
     gar = gar.rename(columns=new_cols)
 
     season_split = gar.season.str.split("-", expand=True)
@@ -2483,14 +2618,15 @@
     gar = gar.rename(columns={"eh_id": "player_id"})
 
     return gar
 
 
 # Function to prep the xGAR dataframe
 def prep_xgar(data: pd.DataFrame) -> pd.DataFrame:
+    """Docstring here"""
     xgar = data.copy()
 
     new_cols = {x: x.replace(" ", "_").lower() for x in xgar.columns}
 
     xgar = xgar.rename(columns=new_cols)
 
     season_split = xgar.season.str.split("-", expand=True)
```

### Comparing `chickenstats-1.7.7/pyproject.toml` & `chickenstats-1.7.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chickenstats"
-version = "1.7.7"
+version = "1.7.8"
 description = "A Python package for scraping & analyzing sports statistics"
 authors = ["chickenandstats <chicken@chickenandstats.com>"]
 license = "GPL-3.0-only"
 packages = [{include = "chickenstats"},
             {include = "chickenstats/chicken_nhl"},
             {include = "chickenstats/evolving_hockey"},
             {include = "chickenstats/capfriendly"},]
@@ -22,14 +22,15 @@
 lxml = "^4.9.4"
 Unidecode = "^1.3.7"
 shapely = "^2.0.2"
 scikit-learn = "^1.3.2"
 geopandas = "^0.14.1"
 rich = "^13.7.0"
 tqdm = "^4.66.1"
+pydantic = "^2.5.3"
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 xgboost = "^2.0.3"
```

### Comparing `chickenstats-1.7.7/PKG-INFO` & `chickenstats-1.7.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chickenstats
-Version: 1.7.7
+Version: 1.7.8
 Summary: A Python package for scraping & analyzing sports statistics
 Home-page: https://github.com/chickenandstats/chickenstats
 License: GPL-3.0-only
 Author: chickenandstats
 Author-email: chicken@chickenandstats.com
 Maintainer: chickenandstats
 Maintainer-email: chicken@chickenandstats.com
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Unidecode (>=1.3.7,<2.0.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: geopandas (>=0.14.1,<0.15.0)
 Requires-Dist: lxml (>=4.9.4,<5.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
+Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
 Requires-Dist: shapely (>=2.0.2,<3.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Documentation, https://www.chickenstats.com
 Project-URL: Repository, https://github.com/chickenandstats/chickenstats
@@ -44,51 +45,54 @@
 
 </div>
 
 ---
 
 ## About
 
-`chickenstats` is a Python package for scraping & analyzing sports statistics. With just a few lines of code:
-* **Scrape & manipulate** data from various NHL endpoints, leveraging a **proprietary xG model**
-for shot quality metrics
+`chickenstats` is a Python package for scraping & analyzing sports data. With just a few lines of code:
+* **Scrape & manipulate** data from various NHL endpoints, leveraging `chickenstats.chicken_nhl`, which includes
+a **proprietary xG model** for shot quality metrics
 * **Augment play-by-play data** & **generate custom aggregations** from raw csv files downloaded from
-[Evolving-Hockey](https://evolving-hockey.com) (subscription required)
-* Download **salary** & other **contract information** for **individual skaters & goalies** programmatically
-from [CapFriendly](https://capfriendly.com)
+[Evolving-Hockey](https://evolving-hockey.com) *(subscription required)* with `chickenstats.evolving_hockey`
 
 For more in-depth explanations, tutorials, & detailed reference materials, consult the
 [**Documentation**](https://chickenstats.com). 
 
 ---
 
 ## Compatibility
 
-`chickenstats` requires Python 3.10 or greater & runs on the latest stable versions Linux, MacOS, & Windows
+`chickenstats` requires Python 3.10 or greater & runs on the latest stable versions of Linux, MacOS, & Windows
 operating systems.
 
 ---
 
 ## Installation
 
 Very simple - install using PyPi. Best practice is to develop in an isolated virtual environment (conda or otherwise),
 but who's a chicken to judge?
 
 ```sh
 pip install chickenstats
 ```
 
+To confirm installation & confirm the latest version (1.7.8):
+
+```sh
+pip show chickenstats
+```
+
 ---
 
 ## Usage
 
 `chickenstats` is structured as three underlying modules, each used with different data sources:
 * `chickenstats.chicken_nhl`
 * `chickenstats.evolving_hockey`
-* `chickenstats.capfriendly`
 
 The package is under active development - features will be added or modified in the coming weeks & months. 
 
 ### chicken_nhl
 
 The `chickenstats.chicken_nhl` module scrapes & manipulates data directly from various NHL endpoints,
 with outputs including schedule & game results, rosters, & play-by-play data. 
@@ -138,26 +142,14 @@
 # accounting for teammates & opposition on-ice
 individual_game = prep_stats(play_by_play, level='game', teammates=True, opposition=True)
 
 # These are game statistics for forward-line combinations, accounting for opponents on-ice
 forward_lines = prep_lines(play_by_play, position='f', opposition=True)
 ```
 
-### capfriendly
-
-Use `chickenstats.capfriendly` to scrape salary & contract information from [CapFriendly](https://capfriendly.com).
-Information available includes AAV, contract term, player age, signing date, draft year, amongst others. 
-
-```python
-from chickenstats.capfriendly import scrape_capfriendly
-
-# Scrape CapFriendly data for the current year
-cf = scrape_capfriendly(2023)
-```
-
 ---
 
 ## Acknowledgements
 
 This project wouldn't be possible without the support & efforts of countless others. I am obviously
 extremely grateful, even if there are too many of you to thank individually. However, this chicken will do his best.
 
@@ -166,11 +158,11 @@
 
 Sincere apologies to the friends & family that have put up with me since my entry into Python, programming, & data
 analysis in January 2021. Thank you for being excited for me & with me throughout all of this, especially when you've
 had to fake it...
 
 Speaking of which, thank you to the hockey analytics community on (the artist formerly known as) Twitter. You're producing
 & reacting to cutting-edge statistical analyses, while providing a supportive, welcoming environment for newcomers.
-This is by no means exhaustive, but a few people worth calling out specifically:
+This is by no means exhaustive, but a few people worth calling out specifically:
```

