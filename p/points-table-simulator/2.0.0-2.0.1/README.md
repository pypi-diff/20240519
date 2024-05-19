# Comparing `tmp/points_table_simulator-2.0.0.tar.gz` & `tmp/points_table_simulator-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "points_table_simulator-2.0.0.tar", last modified: Mon Apr 29 15:43:51 2024, max compression
+gzip compressed data, was "points_table_simulator-2.0.1.tar", last modified: Sun May 19 09:54:31 2024, max compression
```

## Comparing `points_table_simulator-2.0.0.tar` & `points_table_simulator-2.0.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.075955 points_table_simulator-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.github/scripts/quality_checks.sh
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.github/scripts/setup_environment.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.github/workflows/quality_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/create_venv.sh
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.075955 points_table_simulator-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/src/points_table_simulator/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/src/points_table_simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/src/points_table_simulator/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/src/points_table_simulator/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    27066 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/src/points_table_simulator/points_table_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-29 15:43:51.000000 points_table_simulator-2.0.0/src/points_table_simulator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.079955 points_table_simulator-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/tests/points_table_simulator_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/points_table_simulator_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 15:43:51.083955 points_table_simulator-2.0.0/tests/points_table_simulator_tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12923 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/points_table_simulator_tests/error_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-29 15:43:45.000000 points_table_simulator-2.0.0/tests/points_table_simulator_tests/success_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.671789 points_table_simulator-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/.github/scripts/quality_checks.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/.github/scripts/setup_environment.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/.github/workflows/quality_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/create_venv.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-19 09:54:31.679788 points_table_simulator-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.671789 points_table_simulator-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/src/points_table_simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/src/points_table_simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/src/points_table_simulator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/src/points_table_simulator/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27224 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/src/points_table_simulator/points_table_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/src/points_table_simulator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-05-19 09:54:31.000000 points_table_simulator-2.0.1/src/points_table_simulator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-19 09:54:31.000000 points_table_simulator-2.0.1/src/points_table_simulator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 09:54:31.000000 points_table_simulator-2.0.1/src/points_table_simulator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-19 09:54:31.000000 points_table_simulator-2.0.1/src/points_table_simulator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-19 09:54:31.000000 points_table_simulator-2.0.1/src/points_table_simulator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/tests/points_table_simulator_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/tests/points_table_simulator_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 09:54:31.675788 points_table_simulator-2.0.1/tests/points_table_simulator_tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/tests/points_table_simulator_tests/data/psl_2024_fixture.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/tests/points_table_simulator_tests/error_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-19 09:54:22.000000 points_table_simulator-2.0.1/tests/points_table_simulator_tests/success_tests.py
```

### Comparing `points_table_simulator-2.0.0/.github/workflows/publish.yml` & `points_table_simulator-2.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `points_table_simulator-2.0.0/.github/workflows/quality_check.yml` & `points_table_simulator-2.0.1/.github/workflows/quality_check.yml`

 * *Files identical despite different names*

### Comparing `points_table_simulator-2.0.0/.gitignore` & `points_table_simulator-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `points_table_simulator-2.0.0/LICENSE` & `points_table_simulator-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `points_table_simulator-2.0.0/PKG-INFO` & `points_table_simulator-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: points-table-simulator
-Version: 2.0.0
+Version: 2.0.1
 Summary: This package will simulate the points table based on different possible results in a sports tournament
 Home-page: https://github.com/NishanthMuruganantham/points-table-simulator
 Author: Nishanth Muruganantham
 Author-email: nishanthmurugananth10@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `points_table_simulator-2.0.0/README.md` & `points_table_simulator-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `points_table_simulator-2.0.0/pyproject.toml` & `points_table_simulator-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `points_table_simulator-2.0.0/setup.cfg` & `points_table_simulator-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `points_table_simulator-2.0.0/src/points_table_simulator/exceptions.py` & `points_table_simulator-2.0.1/src/points_table_simulator/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,21 @@
     InvalidColumnNamesError: Exception raised when the invalid column names are found in the tournament schedule DataFrame.
     InvalidScheduleDataError: Exception raised when the input schedule dataframe is invalid.
     NoQualifyingScenariosError: Exception raised when no qualifying scenarios are found for the given team.
     TeamNotFoundError: Exception raised when the team is not found in the tournament schedule.
     TournamentCompletionBelowCutoffError: Exception raised when the percentage of tournament completion is below the specified cutoff.
 """
 
+class AllMatchesCompletedError(Exception):
+    """Exception raised when all matches are completed."""
+
+    def __init__(self, message="All matches are completed"):
+        self.message = message
+        super().__init__(self.message)
+
 
 class InvalidColumnNamesError(ValueError):
     """
     Custom error class for invalid column names in the tournament schedule DataFrame.
     """
 
     def __init__(self, column_name: str, column_value: str):
```

### Comparing `points_table_simulator-2.0.0/src/points_table_simulator/points_table_simulator.py` & `points_table_simulator-2.0.1/src/points_table_simulator/points_table_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 
 """
 
 import itertools
 from typing import Dict, List, Tuple, Union
 import pandas as pd
 from points_table_simulator import (
+    AllMatchesCompletedError,
     InvalidColumnNamesError,
     InvalidScheduleDataError,
     NoQualifyingScenariosError,
     TeamNotFoundError,
     TournamentCompletionBelowCutoffError
 )
 from points_table_simulator.constants import (
@@ -392,31 +393,30 @@
 
             for match_number, possible_winning_team in enumerate(remaining_matches_winning_teams):
                 home_team, away_team = self.remaining_matches[match_number]
                 remaining_outcome_df.loc[
                     self.number_of_completed_matches + match_number,
                     self.tournament_schedule_winning_team_column_name
                 ] = possible_winning_team
+                losing_team = home_team if away_team == possible_winning_team else away_team
                 udpated_points_table = self._update_points_table(
-                    udpated_points_table, home_team, away_team, possible_winning_team
+                    losing_team, udpated_points_table, possible_winning_team
                 )
             udpated_points_table.sort_values(by="points", ascending=False, inplace=True)
             udpated_points_table.reset_index(drop=True, inplace=True)
 
             return udpated_points_table, remaining_outcome_df
 
         return None
 
     def _update_points_table(
-        self, points_table: pd.DataFrame, home_team: str, away_team: str, winning_team: str
+        self, losing_team: str, points_table: pd.DataFrame, winning_team: str
     ) -> pd.DataFrame:
-        points_table.loc[points_table["team"] == winning_team, "matches_won"] += 1
-        points_table.loc[points_table['team'] == winning_team, 'points'] += self.points_for_a_win
-        points_table.loc[points_table['team'] == home_team, 'matches_played'] += 1
-        points_table.loc[points_table['team'] == away_team, 'matches_played'] += 1
+        points_table.loc[points_table["team"] == losing_team, ["matches_lost", "matches_played"]] += [1, 1]
+        points_table.loc[points_table["team"] == winning_team, ["matches_played", "matches_won", "points"]] += [1, 1, self.points_for_a_win]
         return points_table
 
     def _update_winning_team_points_dict(self, current_points_dict: Dict[str, int], remaining_matches_winning_teams: Tuple[str]) -> Dict[str, int]:
         """
         Updates the points dictionary for the winning teams in the remaining matches.
 
         Args:
@@ -495,14 +495,16 @@
         for column in (
             self.tournament_schedule_away_team_column_name,
             self.tournament_schedule_home_team_column_name,
             self.tournament_schedule_match_number_column_name,
         ):
             if bool(self.tournament_schedule[column].isnull().any()):
                 raise InvalidScheduleDataError(column)
+        if not bool(self.tournament_schedule[self.tournament_schedule_winning_team_column_name].isnull().any()):
+            raise AllMatchesCompletedError
 
     def _validate_the_inputs_for_simulate_qualification_scenarios(
         self, team_name: str, top_x_position_in_the_table: int, desired_number_of_scenarios: int
     ):
         _type_map: Dict[str, type] = {
             "team_name": str,
             "top_x_position_in_the_table": int,
```

### Comparing `points_table_simulator-2.0.0/src/points_table_simulator.egg-info/PKG-INFO` & `points_table_simulator-2.0.1/src/points_table_simulator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: points-table-simulator
-Version: 2.0.0
+Version: 2.0.1
 Summary: This package will simulate the points table based on different possible results in a sports tournament
 Home-page: https://github.com/NishanthMuruganantham/points-table-simulator
 Author: Nishanth Muruganantham
 Author-email: nishanthmurugananth10@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `points_table_simulator-2.0.0/src/points_table_simulator.egg-info/SOURCES.txt` & `points_table_simulator-2.0.1/src/points_table_simulator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `points_table_simulator-2.0.0/tests/points_table_simulator_tests/data/psl_2024_fixture.csv` & `points_table_simulator-2.0.1/tests/points_table_simulator_tests/data/psl_2024_fixture.csv`

 * *Files identical despite different names*

### Comparing `points_table_simulator-2.0.0/tests/points_table_simulator_tests/error_tests.py` & `points_table_simulator-2.0.1/tests/points_table_simulator_tests/error_tests.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from unittest import TestCase
 import pandas as pd
 from points_table_simulator import (
+    AllMatchesCompletedError,
     InvalidColumnNamesError,
     InvalidScheduleDataError,
     NoQualifyingScenariosError,
     PointsTableSimulator,
     TeamNotFoundError,
     TournamentCompletionBelowCutoffError
 )
@@ -223,7 +224,23 @@
             "away": ["Team B", "Team C", "Team A", "Team C", "Team A", "Team B"],
             "winner": ["Team A", "Team C", None, None, None, None]  # Four matches remaining
         })
         simulator = PointsTableSimulator(tournament_schedule, points_for_a_win=3)
 
         with self.assertRaises(TournamentCompletionBelowCutoffError):
             simulator.simulate_the_qualification_scenarios("Team A", top_x_position_in_the_table=2)
+
+    def test_WHEN_all_the_matches_in_the_given_schedule_are_completed_THEN_raise_AllMatchesCompletedError(self):
+        """
+            This test checks that the PointsTableSimulator class raises a AllMatchesCompletedError, when all the matches
+            in the given schedule are completed.
+        """
+        tournament_schedule = pd.DataFrame({
+            "match_number": list(range(1, 7)),
+            "home": ["Team A", "Team B", "Team C", "Team A", "Team B", "Team C"],
+            "away": ["Team B", "Team C", "Team A", "Team C", "Team A", "Team B"],
+            "winner": ["Team A", "Team C", "Team A", "Team C", "Team A", "Team B"]
+        })
+        
+
+        with self.assertRaises(AllMatchesCompletedError):
+            PointsTableSimulator(tournament_schedule, points_for_a_win=3)
```

### Comparing `points_table_simulator-2.0.0/tests/points_table_simulator_tests/success_tests.py` & `points_table_simulator-2.0.1/tests/points_table_simulator_tests/success_tests.py`

 * *Files identical despite different names*

