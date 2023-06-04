# Comparing `tmp/leeger-2.4.0.tar.gz` & `tmp/leeger-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leeger-2.4.0.tar", last modified: Mon May 15 00:40:21 2023, max compression
+gzip compressed data, was "leeger-2.5.0.tar", last modified: Sun Jun  4 21:30:10 2023, max compression
```

## Comparing `leeger-2.4.0.tar` & `leeger-2.5.0.tar`

### file list

```diff
@@ -1,209 +1,218 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.787891 leeger-2.4.0/
--rw-rw-rw-   0        0        0     1088 2022-06-10 22:18:01.000000 leeger-2.4.0/LICENSE
--rw-rw-rw-   0        0        0       24 2022-10-18 21:57:01.000000 leeger-2.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     9943 2023-05-15 00:40:21.784891 leeger-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     9532 2023-05-15 00:38:33.000000 leeger-2.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.902387 leeger-2.4.0/leeger/
--rw-rw-rw-   0        0        0       43 2022-08-13 05:53:15.000000 leeger-2.4.0/leeger/__init__.py
--rw-rw-rw-   0        0        0       98 2023-05-15 00:39:59.000000 leeger-2.4.0/leeger/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.956388 leeger-2.4.0/leeger/calculator/
--rw-rw-rw-   0        0        0        0 2022-08-13 05:53:37.000000 leeger-2.4.0/leeger/calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.990387 leeger-2.4.0/leeger/calculator/all_time_calculator/
--rw-rw-rw-   0        0        0     5029 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9107 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py
--rw-rw-rw-   0        0        0     1318 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py
--rw-rw-rw-   0        0        0     4490 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py
--rw-rw-rw-   0        0        0     9320 2023-05-11 04:31:22.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py
--rw-rw-rw-   0        0        0     8996 2023-05-11 04:31:22.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py
--rw-rw-rw-   0        0        0     2644 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py
--rw-rw-rw-   0        0        0     3351 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py
--rw-rw-rw-   0        0        0     8906 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py
--rw-rw-rw-   0        0        0     1519 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py
--rw-rw-rw-   0        0        0      712 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/calculator/all_time_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.998386 leeger-2.4.0/leeger/calculator/parent/
--rw-rw-rw-   0        0        0    15345 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/parent/AllTimeCalculator.py
--rw-rw-rw-   0        0        0     1671 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/parent/YearCalculator.py
--rw-rw-rw-   0        0        0       94 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/calculator/parent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.044388 leeger-2.4.0/leeger/calculator/year_calculator/
--rw-rw-rw-   0        0        0     9896 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/year_calculator/AWALYearCalculator.py
--rw-rw-rw-   0        0        0    18719 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py
--rw-rw-rw-   0        0        0     2018 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py
--rw-rw-rw-   0        0        0     5843 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py
--rw-rw-rw-   0        0        0     6208 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/year_calculator/SSLYearCalculator.py
--rw-rw-rw-   0        0        0     8945 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py
--rw-rw-rw-   0        0        0     2396 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py
--rw-rw-rw-   0        0        0     2973 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py
--rw-rw-rw-   0        0        0     8392 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py
--rw-rw-rw-   0        0        0     1699 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py
--rw-rw-rw-   0        0        0      652 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/calculator/year_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.050393 leeger-2.4.0/leeger/decorator/
--rw-rw-rw-   0        0        0       85 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/decorator/__init__.py
--rw-rw-rw-   0        0        0     4853 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/decorator/validators.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.055391 leeger-2.4.0/leeger/enum/
--rw-rw-rw-   0        0        0      784 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/enum/MatchupType.py
--rw-rw-rw-   0        0        0       38 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/enum/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.125389 leeger-2.4.0/leeger/exception/
--rw-rw-rw-   0        0        0      145 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/DoesNotExistException.py
--rw-rw-rw-   0        0        0      105 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidFilterException.py
--rw-rw-rw-   0        0        0      126 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidLeagueFormatException.py
--rw-rw-rw-   0        0        0      128 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidMatchupFormatException.py
--rw-rw-rw-   0        0        0      125 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidOwnerFormatException.py
--rw-rw-rw-   0        0        0      122 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidTeamFormatException.py
--rw-rw-rw-   0        0        0      122 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidWeekFormatException.py
--rw-rw-rw-   0        0        0      122 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidYearFormatException.py
--rw-rw-rw-   0        0        0      138 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/exception/InvalidYearSettingsFormatException.py
--rw-rw-rw-   0        0        0      126 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/exception/LeagueLoaderException.py
--rw-rw-rw-   0        0        0      136 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/exception/UnsupportedLeegerFeatureException.py
--rw-rw-rw-   0        0        0      762 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/exception/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.221579 leeger-2.4.0/leeger/league_loader/
--rw-rw-rw-   0        0        0     9195 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/ESPNLeagueLoader.py
--rw-rw-rw-   0        0        0     8032 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/FleaflickerLeagueLoader.py
--rw-rw-rw-   0        0        0     4632 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/LeagueLoader.py
--rw-rw-rw-   0        0        0    11954 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py
--rw-rw-rw-   0        0        0    19866 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/SleeperLeagueLoader.py
--rw-rw-rw-   0        0        0    11528 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/league_loader/YahooLeagueLoader.py
--rw-rw-rw-   0        0        0      222 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/league_loader/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.226579 leeger-2.4.0/leeger/model/
--rw-rw-rw-   0        0        0        0 2022-08-13 05:54:09.000000 leeger-2.4.0/leeger/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.232577 leeger-2.4.0/leeger/model/abstract/
--rw-rw-rw-   0        0        0      550 2023-02-17 18:45:58.000000 leeger-2.4.0/leeger/model/abstract/UniqueId.py
--rw-rw-rw-   0        0        0       32 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/model/abstract/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.346576 leeger-2.4.0/leeger/model/filter/
--rw-rw-rw-   0        0        0     5463 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/model/filter/AllTimeFilters.py
--rw-rw-rw-   0        0        0      321 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/model/filter/WeekFilters.py
--rw-rw-rw-   0        0        0     5200 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/model/filter/YearFilters.py
--rw-rw-rw-   0        0        0      120 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/model/filter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.472580 leeger-2.4.0/leeger/model/league/
--rw-rw-rw-   0        0        0     6088 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/League.py
--rw-rw-rw-   0        0        0     5276 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Matchup.py
--rw-rw-rw-   0        0        0     1347 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Owner.py
--rw-rw-rw-   0        0        0     1689 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Team.py
--rw-rw-rw-   0        0        0     3290 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Week.py
--rw-rw-rw-   0        0        0     3336 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/Year.py
--rw-rw-rw-   0        0        0     1493 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/model/league/YearSettings.py
--rw-rw-rw-   0        0        0      196 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/model/league/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.527578 leeger-2.4.0/leeger/model/league_helper/
--rw-rw-rw-   0        0        0     3711 2023-04-30 18:12:34.000000 leeger-2.4.0/leeger/model/league_helper/Performance.py
--rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.4.0/leeger/model/league_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.690577 leeger-2.4.0/leeger/model/stat/
--rw-rw-rw-   0        0        0     3880 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/model/stat/AllTimeStatSheet.py
--rw-rw-rw-   0        0        0     4126 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/model/stat/YearStatSheet.py
--rw-rw-rw-   0        0        0       90 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/model/stat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:19.844576 leeger-2.4.0/leeger/util/
--rw-rw-rw-   0        0        0     1114 2023-04-29 23:36:04.000000 leeger-2.4.0/leeger/util/CustomFormatter.py
--rw-rw-rw-   0        0        0      889 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/util/CustomLogger.py
--rw-rw-rw-   0        0        0      513 2022-06-11 23:09:37.000000 leeger-2.4.0/leeger/util/Deci.py
--rw-rw-rw-   0        0        0     4056 2023-05-15 00:38:33.000000 leeger-2.4.0/leeger/util/GeneralUtil.py
--rw-rw-rw-   0        0        0      237 2022-06-10 22:18:01.000000 leeger-2.4.0/leeger/util/IdGenerator.py
--rw-rw-rw-   0        0        0      296 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/util/JSONDeserializable.py
--rw-rw-rw-   0        0        0      262 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/util/JSONSerializable.py
--rw-rw-rw-   0        0        0        0 2022-08-13 05:54:20.000000 leeger-2.4.0/leeger/util/__init__.py
--rw-rw-rw-   0        0        0    14428 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/util/excel.py
--rw-rw-rw-   0        0        0     9027 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/util/excel_helper.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.117581 leeger-2.4.0/leeger/util/navigator/
--rw-rw-rw-   0        0        0     5682 2023-05-11 04:22:19.000000 leeger-2.4.0/leeger/util/navigator/LeagueNavigator.py
--rw-rw-rw-   0        0        0     2071 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/util/navigator/MatchupNavigator.py
--rw-rw-rw-   0        0        0     2207 2023-04-29 23:41:27.000000 leeger-2.4.0/leeger/util/navigator/WeekNavigator.py
--rw-rw-rw-   0        0        0     6659 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/util/navigator/YearNavigator.py
--rw-rw-rw-   0        0        0      178 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/util/navigator/__init__.py
--rw-rw-rw-   0        0        0    11436 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/util/stat_sheet.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.147579 leeger-2.4.0/leeger/validate/
--rw-rw-rw-   0        0        0      258 2023-05-14 08:22:22.000000 leeger-2.4.0/leeger/validate/__init__.py
--rw-rw-rw-   0        0        0     4326 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/leagueValidation.py
--rw-rw-rw-   0        0        0     2481 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/matchupValidation.py
--rw-rw-rw-   0        0        0      493 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/ownerValidation.py
--rw-rw-rw-   0        0        0      598 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/teamValidation.py
--rw-rw-rw-   0        0        0     4686 2023-04-29 23:41:28.000000 leeger-2.4.0/leeger/validate/weekValidation.py
--rw-rw-rw-   0        0        0      221 2023-05-14 17:09:42.000000 leeger-2.4.0/leeger/validate/yearSettingsValidation.py
--rw-rw-rw-   0        0        0    13562 2023-05-11 04:31:22.000000 leeger-2.4.0/leeger/validate/yearValidation.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.951388 leeger-2.4.0/leeger.egg-info/
--rw-rw-rw-   0        0        0     9943 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7839 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-15 00:40:18.000000 leeger-2.4.0/leeger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      203 2023-05-15 00:38:33.000000 leeger-2.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      147 2023-04-13 04:26:54.000000 leeger-2.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 00:40:21.787891 leeger-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-04-29 23:41:28.000000 leeger-2.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:18.618668 leeger-2.4.0/test/
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.157575 leeger-2.4.0/test/test_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.763893 leeger-2.4.0/test/test_calculator/test_all_time_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-27 00:56:09.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/__init__.py
--rw-rw-rw-   0        0        0    86146 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py
--rw-rw-rw-   0        0        0   220423 2023-04-29 23:41:38.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py
--rw-rw-rw-   0        0        0    24301 2023-04-29 23:41:29.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py
--rw-rw-rw-   0        0        0    96680 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py
--rw-rw-rw-   0        0        0    42298 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py
--rw-rw-rw-   0        0        0   107979 2023-04-29 23:41:35.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py
--rw-rw-rw-   0        0        0    27851 2023-04-29 23:41:29.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py
--rw-rw-rw-   0        0        0    47446 2023-04-29 23:41:31.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py
--rw-rw-rw-   0        0        0   103504 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py
--rw-rw-rw-   0        0        0    54546 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.885892 leeger-2.4.0/test/test_calculator/test_year_calculator/
--rw-rw-rw-   0        0        0        0 2022-06-27 00:54:55.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/__init__.py
--rw-rw-rw-   0        0        0   104455 2023-04-29 23:41:35.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py
--rw-rw-rw-   0        0        0    84963 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py
--rw-rw-rw-   0        0        0     9711 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py
--rw-rw-rw-   0        0        0    39044 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py
--rw-rw-rw-   0        0        0    29836 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py
--rw-rw-rw-   0        0        0    44383 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py
--rw-rw-rw-   0        0        0    12194 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py
--rw-rw-rw-   0        0        0    35141 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py
--rw-rw-rw-   0        0        0    82020 2023-04-29 23:41:36.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py
--rw-rw-rw-   0        0        0    21748 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:20.891891 leeger-2.4.0/test/test_decorator/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_decorator/__init__.py
--rw-rw-rw-   0        0        0     4803 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_decorator/test_validators.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.346892 leeger-2.4.0/test/test_league_loader/
--rw-rw-rw-   0        0        0        0 2022-06-25 00:07:47.000000 leeger-2.4.0/test/test_league_loader/__init__.py
--rw-rw-rw-   0        0        0    36769 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_ESPNLeagueLoader.py
--rw-rw-rw-   0        0        0    38840 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_FleaflickerLeagueLoader.py
--rw-rw-rw-   0        0        0     6530 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_LeagueLoader.py
--rw-rw-rw-   0        0        0    69702 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py
--rw-rw-rw-   0        0        0   112178 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_SleeperLeagueLoader.py
--rw-rw-rw-   0        0        0    49966 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_league_loader/test_YahooLeagueLoader.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.349891 leeger-2.4.0/test/test_model/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.353891 leeger-2.4.0/test/test_model/test_abstract/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_model/test_abstract/__init__.py
--rw-rw-rw-   0        0        0      932 2022-09-19 23:01:23.000000 leeger-2.4.0/test/test_model/test_abstract/test_UniqueId.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.361893 leeger-2.4.0/test/test_model/test_filter/
--rw-rw-rw-   0        0        0        0 2022-07-01 18:59:46.000000 leeger-2.4.0/test/test_model/test_filter/__init__.py
--rw-rw-rw-   0        0        0     2098 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_model/test_filter/test_AllTimeFilters.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.391894 leeger-2.4.0/test/test_model/test_league/
--rw-rw-rw-   0        0        0        0 2022-06-23 01:09:11.000000 leeger-2.4.0/test/test_model/test_league/__init__.py
--rw-rw-rw-   0        0        0    22224 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_model/test_league/test_League.py
--rw-rw-rw-   0        0        0     8360 2023-04-29 23:41:33.000000 leeger-2.4.0/test/test_model/test_league/test_Matchup.py
--rw-rw-rw-   0        0        0     1136 2023-02-17 19:28:57.000000 leeger-2.4.0/test/test_model/test_league/test_Owner.py
--rw-rw-rw-   0        0        0     1219 2023-02-17 19:29:31.000000 leeger-2.4.0/test/test_model/test_league/test_Team.py
--rw-rw-rw-   0        0        0     9659 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_model/test_league/test_Week.py
--rw-rw-rw-   0        0        0     8823 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_model/test_league/test_Year.py
--rw-rw-rw-   0        0        0     1487 2023-02-17 19:34:39.000000 leeger-2.4.0/test/test_model/test_league/test_YearSettings.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.397895 leeger-2.4.0/test/test_model/test_league_helper/
--rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.4.0/test/test_model/test_league_helper/__init__.py
--rw-rw-rw-   0        0        0     6294 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_model/test_league_helper/test_Performance.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.420895 leeger-2.4.0/test/test_util/
--rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.4.0/test/test_util/__init__.py
--rw-rw-rw-   0        0        0      471 2022-07-13 01:00:46.000000 leeger-2.4.0/test/test_util/test_Deci.py
--rw-rw-rw-   0        0        0     8493 2023-05-15 00:38:33.000000 leeger-2.4.0/test/test_util/test_GeneralUtil.py
--rw-rw-rw-   0        0        0      486 2022-07-13 01:00:45.000000 leeger-2.4.0/test/test_util/test_IdGenerator.py
--rw-rw-rw-   0        0        0    64757 2023-05-11 04:31:22.000000 leeger-2.4.0/test/test_util/test_excel.py
--rw-rw-rw-   0        0        0     7246 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_util/test_excel_helper.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.610893 leeger-2.4.0/test/test_util/test_navigator/
--rw-rw-rw-   0        0        0        0 2022-08-12 22:44:07.000000 leeger-2.4.0/test/test_util/test_navigator/__init__.py
--rw-rw-rw-   0        0        0    52517 2023-04-29 23:41:36.000000 leeger-2.4.0/test/test_util/test_navigator/test_LeagueNavigator.py
--rw-rw-rw-   0        0        0     3970 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_util/test_navigator/test_MatchupNavigator.py
--rw-rw-rw-   0        0        0     6154 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_util/test_navigator/test_WeekNavigator.py
--rw-rw-rw-   0        0        0    27730 2023-04-29 23:41:35.000000 leeger-2.4.0/test/test_util/test_navigator/test_YearNavigator.py
--rw-rw-rw-   0        0        0    10570 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_util/test_stat_sheet.py
-drwxrwxrwx   0        0        0        0 2023-05-15 00:40:21.737893 leeger-2.4.0/test/test_validate/
--rw-rw-rw-   0        0        0        0 2022-08-12 22:13:02.000000 leeger-2.4.0/test/test_validate/__init__.py
--rw-rw-rw-   0        0        0     8903 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_validate/test_leagueValidation.py
--rw-rw-rw-   0        0        0     4772 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_validate/test_matchupValidation.py
--rw-rw-rw-   0        0        0      530 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_validate/test_ownerValidation.py
--rw-rw-rw-   0        0        0      838 2023-04-29 23:41:34.000000 leeger-2.4.0/test/test_validate/test_teamValidation.py
--rw-rw-rw-   0        0        0     6094 2023-05-11 04:22:19.000000 leeger-2.4.0/test/test_validate/test_weekValidation.py
--rw-rw-rw-   0        0        0      612 2023-02-17 19:20:44.000000 leeger-2.4.0/test/test_validate/test_yearSettingsValidation.py
--rw-rw-rw-   0        0        0    25513 2023-04-29 23:41:35.000000 leeger-2.4.0/test/test_validate/test_yearValidation.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:10.059045 leeger-2.5.0/
+-rw-rw-rw-   0        0        0     1088 2022-06-10 22:18:01.000000 leeger-2.5.0/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-10-18 21:57:01.000000 leeger-2.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     9890 2023-06-04 21:30:10.057047 leeger-2.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9480 2023-06-04 21:27:09.000000 leeger-2.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.587047 leeger-2.5.0/leeger/
+-rw-rw-rw-   0        0        0       43 2022-08-13 05:53:15.000000 leeger-2.5.0/leeger/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-06-04 21:28:20.000000 leeger-2.5.0/leeger/_version.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.629046 leeger-2.5.0/leeger/calculator/
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:53:37.000000 leeger-2.5.0/leeger/calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.656044 leeger-2.5.0/leeger/calculator/all_time_calculator/
+-rw-rw-rw-   0        0        0     5029 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     9107 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1318 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     4490 2023-05-11 04:22:19.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     9320 2023-05-11 04:31:22.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     8996 2023-05-11 04:31:22.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     2644 2023-05-11 04:22:19.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     3351 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     8906 2023-05-11 04:22:19.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1519 2023-05-11 04:22:19.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py
+-rw-rw-rw-   0        0        0      712 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/calculator/all_time_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.662048 leeger-2.5.0/leeger/calculator/parent/
+-rw-rw-rw-   0        0        0    15345 2023-05-11 04:22:19.000000 leeger-2.5.0/leeger/calculator/parent/AllTimeCalculator.py
+-rw-rw-rw-   0        0        0     1671 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/parent/YearCalculator.py
+-rw-rw-rw-   0        0        0       94 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/calculator/parent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.689045 leeger-2.5.0/leeger/calculator/year_calculator/
+-rw-rw-rw-   0        0        0     9896 2023-05-11 04:22:19.000000 leeger-2.5.0/leeger/calculator/year_calculator/AWALYearCalculator.py
+-rw-rw-rw-   0        0        0    18719 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py
+-rw-rw-rw-   0        0        0     2018 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py
+-rw-rw-rw-   0        0        0     5843 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py
+-rw-rw-rw-   0        0        0     6208 2023-05-11 04:22:19.000000 leeger-2.5.0/leeger/calculator/year_calculator/SSLYearCalculator.py
+-rw-rw-rw-   0        0        0     8945 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py
+-rw-rw-rw-   0        0        0     2396 2023-05-11 04:22:19.000000 leeger-2.5.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py
+-rw-rw-rw-   0        0        0     2973 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py
+-rw-rw-rw-   0        0        0     8392 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py
+-rw-rw-rw-   0        0        0     1699 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py
+-rw-rw-rw-   0        0        0      652 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/calculator/year_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.693043 leeger-2.5.0/leeger/decorator/
+-rw-rw-rw-   0        0        0       85 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/decorator/__init__.py
+-rw-rw-rw-   0        0        0     4853 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/decorator/validators.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.698045 leeger-2.5.0/leeger/enum/
+-rw-rw-rw-   0        0        0      784 2023-04-29 23:36:04.000000 leeger-2.5.0/leeger/enum/MatchupType.py
+-rw-rw-rw-   0        0        0       38 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/enum/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.728042 leeger-2.5.0/leeger/exception/
+-rw-rw-rw-   0        0        0      145 2023-05-28 03:17:48.000000 leeger-2.5.0/leeger/exception/DoesNotExistException.py
+-rw-rw-rw-   0        0        0      131 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/exception/InvalidDivisionFormatException.py
+-rw-rw-rw-   0        0        0      105 2023-05-28 03:17:48.000000 leeger-2.5.0/leeger/exception/InvalidFilterException.py
+-rw-rw-rw-   0        0        0      126 2023-05-28 03:17:48.000000 leeger-2.5.0/leeger/exception/InvalidLeagueFormatException.py
+-rw-rw-rw-   0        0        0      128 2023-05-28 03:17:48.000000 leeger-2.5.0/leeger/exception/InvalidMatchupFormatException.py
+-rw-rw-rw-   0        0        0      125 2023-05-28 03:17:48.000000 leeger-2.5.0/leeger/exception/InvalidOwnerFormatException.py
+-rw-rw-rw-   0        0        0      122 2023-05-28 03:17:48.000000 leeger-2.5.0/leeger/exception/InvalidTeamFormatException.py
+-rw-rw-rw-   0        0        0      122 2023-05-28 03:17:48.000000 leeger-2.5.0/leeger/exception/InvalidWeekFormatException.py
+-rw-rw-rw-   0        0        0      122 2023-05-28 03:17:48.000000 leeger-2.5.0/leeger/exception/InvalidYearFormatException.py
+-rw-rw-rw-   0        0        0      138 2023-05-28 03:17:48.000000 leeger-2.5.0/leeger/exception/InvalidYearSettingsFormatException.py
+-rw-rw-rw-   0        0        0      126 2023-04-29 23:36:04.000000 leeger-2.5.0/leeger/exception/LeagueLoaderException.py
+-rw-rw-rw-   0        0        0      136 2023-04-29 23:36:04.000000 leeger-2.5.0/leeger/exception/UnsupportedLeegerFeatureException.py
+-rw-rw-rw-   0        0        0      838 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/exception/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.743045 leeger-2.5.0/leeger/league_loader/
+-rw-rw-rw-   0        0        0    10154 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/league_loader/ESPNLeagueLoader.py
+-rw-rw-rw-   0        0        0     8988 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/league_loader/FleaflickerLeagueLoader.py
+-rw-rw-rw-   0        0        0     4632 2023-05-15 00:38:33.000000 leeger-2.5.0/leeger/league_loader/LeagueLoader.py
+-rw-rw-rw-   0        0        0    11749 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py
+-rw-rw-rw-   0        0        0    21593 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/league_loader/SleeperLeagueLoader.py
+-rw-rw-rw-   0        0        0    11658 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/league_loader/YahooLeagueLoader.py
+-rw-rw-rw-   0        0        0      222 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/league_loader/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.746042 leeger-2.5.0/leeger/model/
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:54:09.000000 leeger-2.5.0/leeger/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.752045 leeger-2.5.0/leeger/model/abstract/
+-rw-rw-rw-   0        0        0      469 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/abstract/EqualityCheck.py
+-rw-rw-rw-   0        0        0      550 2023-02-17 18:45:58.000000 leeger-2.5.0/leeger/model/abstract/UniqueId.py
+-rw-rw-rw-   0        0        0       32 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/model/abstract/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.762046 leeger-2.5.0/leeger/model/filter/
+-rw-rw-rw-   0        0        0     5463 2023-05-27 03:21:06.000000 leeger-2.5.0/leeger/model/filter/AllTimeFilters.py
+-rw-rw-rw-   0        0        0      321 2023-05-27 03:21:04.000000 leeger-2.5.0/leeger/model/filter/WeekFilters.py
+-rw-rw-rw-   0        0        0     5141 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/filter/YearFilters.py
+-rw-rw-rw-   0        0        0      120 2023-05-27 03:21:08.000000 leeger-2.5.0/leeger/model/filter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.782045 leeger-2.5.0/leeger/model/league/
+-rw-rw-rw-   0        0        0     1644 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league/Division.py
+-rw-rw-rw-   0        0        0     7069 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league/League.py
+-rw-rw-rw-   0        0        0     4776 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league/Matchup.py
+-rw-rw-rw-   0        0        0     1593 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league/Owner.py
+-rw-rw-rw-   0        0        0     1884 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league/Team.py
+-rw-rw-rw-   0        0        0     4255 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league/Week.py
+-rw-rw-rw-   0        0        0     5383 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league/Year.py
+-rw-rw-rw-   0        0        0     1812 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league/YearSettings.py
+-rw-rw-rw-   0        0        0      228 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.787048 leeger-2.5.0/leeger/model/league_helper/
+-rw-rw-rw-   0        0        0     3867 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/model/league_helper/Performance.py
+-rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.5.0/leeger/model/league_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.794045 leeger-2.5.0/leeger/model/stat/
+-rw-rw-rw-   0        0        0     3880 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/model/stat/AllTimeStatSheet.py
+-rw-rw-rw-   0        0        0     4126 2023-05-28 03:02:41.000000 leeger-2.5.0/leeger/model/stat/YearStatSheet.py
+-rw-rw-rw-   0        0        0       90 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/model/stat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.825044 leeger-2.5.0/leeger/util/
+-rw-rw-rw-   0        0        0     1007 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/util/ConfigReader.py
+-rw-rw-rw-   0        0        0     1114 2023-04-29 23:36:04.000000 leeger-2.5.0/leeger/util/CustomFormatter.py
+-rw-rw-rw-   0        0        0      889 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/util/CustomLogger.py
+-rw-rw-rw-   0        0        0      513 2022-06-11 23:09:37.000000 leeger-2.5.0/leeger/util/Deci.py
+-rw-rw-rw-   0        0        0     4421 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/util/GeneralUtil.py
+-rw-rw-rw-   0        0        0      237 2022-06-10 22:18:01.000000 leeger-2.5.0/leeger/util/IdGenerator.py
+-rw-rw-rw-   0        0        0      296 2023-05-14 17:09:42.000000 leeger-2.5.0/leeger/util/JSONDeserializable.py
+-rw-rw-rw-   0        0        0      262 2023-05-14 17:09:42.000000 leeger-2.5.0/leeger/util/JSONSerializable.py
+-rw-rw-rw-   0        0        0        0 2022-08-13 05:54:20.000000 leeger-2.5.0/leeger/util/__init__.py
+-rw-rw-rw-   0        0        0     3667 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/util/equality.py
+-rw-rw-rw-   0        0        0    15086 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/util/excel.py
+-rw-rw-rw-   0        0        0     9373 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/util/excel_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.838044 leeger-2.5.0/leeger/util/navigator/
+-rw-rw-rw-   0        0        0     5682 2023-05-11 04:22:19.000000 leeger-2.5.0/leeger/util/navigator/LeagueNavigator.py
+-rw-rw-rw-   0        0        0     2071 2023-04-29 23:41:28.000000 leeger-2.5.0/leeger/util/navigator/MatchupNavigator.py
+-rw-rw-rw-   0        0        0     2207 2023-04-29 23:41:27.000000 leeger-2.5.0/leeger/util/navigator/WeekNavigator.py
+-rw-rw-rw-   0        0        0     7048 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/util/navigator/YearNavigator.py
+-rw-rw-rw-   0        0        0      178 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/util/navigator/__init__.py
+-rw-rw-rw-   0        0        0    11436 2023-04-29 23:41:28.000000 leeger-2.5.0/leeger/util/stat_sheet.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.859043 leeger-2.5.0/leeger/validate/
+-rw-rw-rw-   0        0        0      258 2023-05-14 08:22:22.000000 leeger-2.5.0/leeger/validate/__init__.py
+-rw-rw-rw-   0        0        0      529 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/validate/divisionValidation.py
+-rw-rw-rw-   0        0        0     4583 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/validate/leagueValidation.py
+-rw-rw-rw-   0        0        0     2481 2023-04-29 23:41:28.000000 leeger-2.5.0/leeger/validate/matchupValidation.py
+-rw-rw-rw-   0        0        0      493 2023-04-29 23:41:28.000000 leeger-2.5.0/leeger/validate/ownerValidation.py
+-rw-rw-rw-   0        0        0      744 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/validate/teamValidation.py
+-rw-rw-rw-   0        0        0     4830 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/validate/weekValidation.py
+-rw-rw-rw-   0        0        0      221 2023-05-14 17:09:42.000000 leeger-2.5.0/leeger/validate/yearSettingsValidation.py
+-rw-rw-rw-   0        0        0    18614 2023-06-04 21:27:09.000000 leeger-2.5.0/leeger/validate/yearValidation.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.627047 leeger-2.5.0/leeger.egg-info/
+-rw-rw-rw-   0        0        0     9890 2023-06-04 21:30:09.000000 leeger-2.5.0/leeger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8174 2023-06-04 21:30:09.000000 leeger-2.5.0/leeger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 21:30:09.000000 leeger-2.5.0/leeger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2023-06-04 21:30:09.000000 leeger-2.5.0/leeger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-04 21:30:09.000000 leeger-2.5.0/leeger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      217 2023-06-04 21:27:09.000000 leeger-2.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      168 2023-06-04 21:27:09.000000 leeger-2.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-04 21:30:10.059045 leeger-2.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2023-06-04 21:27:09.000000 leeger-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.564045 leeger-2.5.0/test/
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.861044 leeger-2.5.0/test/test_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.0/test/test_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.890047 leeger-2.5.0/test/test_calculator/test_all_time_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-27 00:56:09.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/__init__.py
+-rw-rw-rw-   0        0        0    86146 2023-04-29 23:41:33.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   220423 2023-04-29 23:41:38.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    24301 2023-04-29 23:41:29.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    96680 2023-04-29 23:41:34.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    42298 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   107979 2023-04-29 23:41:35.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    27851 2023-04-29 23:41:29.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    47446 2023-04-29 23:41:31.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py
+-rw-rw-rw-   0        0        0   103504 2023-04-29 23:41:34.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py
+-rw-rw-rw-   0        0        0    54546 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.919044 leeger-2.5.0/test/test_calculator/test_year_calculator/
+-rw-rw-rw-   0        0        0        0 2022-06-27 00:54:55.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/__init__.py
+-rw-rw-rw-   0        0        0   104455 2023-04-29 23:41:35.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py
+-rw-rw-rw-   0        0        0    84963 2023-04-29 23:41:33.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py
+-rw-rw-rw-   0        0        0     9711 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py
+-rw-rw-rw-   0        0        0    39044 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py
+-rw-rw-rw-   0        0        0    29836 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py
+-rw-rw-rw-   0        0        0    44383 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py
+-rw-rw-rw-   0        0        0    12194 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py
+-rw-rw-rw-   0        0        0    35141 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py
+-rw-rw-rw-   0        0        0    82020 2023-04-29 23:41:36.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py
+-rw-rw-rw-   0        0        0    21748 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.924049 leeger-2.5.0/test/test_decorator/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.0/test/test_decorator/__init__.py
+-rw-rw-rw-   0        0        0     4803 2023-04-29 23:41:33.000000 leeger-2.5.0/test/test_decorator/test_validators.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.942049 leeger-2.5.0/test/test_league_loader/
+-rw-rw-rw-   0        0        0        0 2022-06-25 00:07:47.000000 leeger-2.5.0/test/test_league_loader/__init__.py
+-rw-rw-rw-   0        0        0    49779 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_league_loader/test_ESPNLeagueLoader.py
+-rw-rw-rw-   0        0        0    50085 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_league_loader/test_FleaflickerLeagueLoader.py
+-rw-rw-rw-   0        0        0     6530 2023-05-15 00:38:33.000000 leeger-2.5.0/test/test_league_loader/test_LeagueLoader.py
+-rw-rw-rw-   0        0        0    94605 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py
+-rw-rw-rw-   0        0        0   131293 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_league_loader/test_SleeperLeagueLoader.py
+-rw-rw-rw-   0        0        0    63226 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_league_loader/test_YahooLeagueLoader.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.945051 leeger-2.5.0/test/test_model/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.0/test/test_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.949044 leeger-2.5.0/test/test_model/test_abstract/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.0/test/test_model/test_abstract/__init__.py
+-rw-rw-rw-   0        0        0      932 2022-09-19 23:01:23.000000 leeger-2.5.0/test/test_model/test_abstract/test_UniqueId.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.954044 leeger-2.5.0/test/test_model/test_filter/
+-rw-rw-rw-   0        0        0        0 2022-07-01 18:59:46.000000 leeger-2.5.0/test/test_model/test_filter/__init__.py
+-rw-rw-rw-   0        0        0     2098 2023-04-29 23:41:33.000000 leeger-2.5.0/test/test_model/test_filter/test_AllTimeFilters.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.977045 leeger-2.5.0/test/test_model/test_league/
+-rw-rw-rw-   0        0        0        0 2022-06-23 01:09:11.000000 leeger-2.5.0/test/test_model/test_league/__init__.py
+-rw-rw-rw-   0        0        0     1333 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_model/test_league/test_Division.py
+-rw-rw-rw-   0        0        0    23031 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_model/test_league/test_League.py
+-rw-rw-rw-   0        0        0     9164 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_model/test_league/test_Matchup.py
+-rw-rw-rw-   0        0        0     1477 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_model/test_league/test_Owner.py
+-rw-rw-rw-   0        0        0     1434 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_model/test_league/test_Team.py
+-rw-rw-rw-   0        0        0    10522 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_model/test_league/test_Week.py
+-rw-rw-rw-   0        0        0     9195 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_model/test_league/test_Year.py
+-rw-rw-rw-   0        0        0     1809 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_model/test_league/test_YearSettings.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:09.981043 leeger-2.5.0/test/test_model/test_league_helper/
+-rw-rw-rw-   0        0        0        0 2023-01-04 01:53:09.000000 leeger-2.5.0/test/test_model/test_league_helper/__init__.py
+-rw-rw-rw-   0        0        0     6726 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_model/test_league_helper/test_Performance.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:10.003045 leeger-2.5.0/test/test_util/
+-rw-rw-rw-   0        0        0        0 2022-06-10 22:18:01.000000 leeger-2.5.0/test/test_util/__init__.py
+-rw-rw-rw-   0        0        0      471 2022-07-13 01:00:46.000000 leeger-2.5.0/test/test_util/test_Deci.py
+-rw-rw-rw-   0        0        0     9143 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_util/test_GeneralUtil.py
+-rw-rw-rw-   0        0        0      486 2022-07-13 01:00:45.000000 leeger-2.5.0/test/test_util/test_IdGenerator.py
+-rw-rw-rw-   0        0        0     7379 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_util/test_equality.py
+-rw-rw-rw-   0        0        0    65300 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_util/test_excel.py
+-rw-rw-rw-   0        0        0     7246 2023-04-29 23:41:34.000000 leeger-2.5.0/test/test_util/test_excel_helper.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:10.021047 leeger-2.5.0/test/test_util/test_navigator/
+-rw-rw-rw-   0        0        0        0 2022-08-12 22:44:07.000000 leeger-2.5.0/test/test_util/test_navigator/__init__.py
+-rw-rw-rw-   0        0        0    52517 2023-04-29 23:41:36.000000 leeger-2.5.0/test/test_util/test_navigator/test_LeagueNavigator.py
+-rw-rw-rw-   0        0        0     3970 2023-04-29 23:41:34.000000 leeger-2.5.0/test/test_util/test_navigator/test_MatchupNavigator.py
+-rw-rw-rw-   0        0        0     6154 2023-04-29 23:41:34.000000 leeger-2.5.0/test/test_util/test_navigator/test_WeekNavigator.py
+-rw-rw-rw-   0        0        0    29212 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_util/test_navigator/test_YearNavigator.py
+-rw-rw-rw-   0        0        0    10570 2023-04-29 23:41:34.000000 leeger-2.5.0/test/test_util/test_stat_sheet.py
+drwxrwxrwx   0        0        0        0 2023-06-04 21:30:10.051046 leeger-2.5.0/test/test_validate/
+-rw-rw-rw-   0        0        0        0 2022-08-12 22:13:02.000000 leeger-2.5.0/test/test_validate/__init__.py
+-rw-rw-rw-   0        0        0      560 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_validate/test_divisionValidation.py
+-rw-rw-rw-   0        0        0     9561 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_validate/test_leagueValidation.py
+-rw-rw-rw-   0        0        0     4772 2023-05-11 04:22:19.000000 leeger-2.5.0/test/test_validate/test_matchupValidation.py
+-rw-rw-rw-   0        0        0      530 2023-04-29 23:41:34.000000 leeger-2.5.0/test/test_validate/test_ownerValidation.py
+-rw-rw-rw-   0        0        0     1174 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_validate/test_teamValidation.py
+-rw-rw-rw-   0        0        0     6416 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_validate/test_weekValidation.py
+-rw-rw-rw-   0        0        0      612 2023-02-17 19:20:44.000000 leeger-2.5.0/test/test_validate/test_yearSettingsValidation.py
+-rw-rw-rw-   0        0        0    36250 2023-06-04 21:27:09.000000 leeger-2.5.0/test/test_validate/test_yearValidation.py
```

### Comparing `leeger-2.4.0/LICENSE` & `leeger-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/PKG-INFO` & `leeger-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: leeger
-Version: 2.4.0
-Summary: Instant stats for your fantasy football league.
+Version: 2.5.0
+Summary: Instant stats for any fantasy football league.
 Home-page: https://github.com/joeyagreco/leeger
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: nfl statistics stats football espn yahoo sleeper myfantasyleague,fleaflicker
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -124,14 +124,15 @@
 // @formatter:on
 -->
 
 **Answer:**
 This error occurs when the Python version you are using is not 3.10 or greater.\
 Make sure you are using Python version 3.10 or a newer version.
 
+___
 **Q:**
 How do I use this library to pull stats from my online fantasy league?
 
 **A:**
 
 1. Find your fantasy site [here](https://github.com/joeyagreco/leeger#supported-league-loaders) and ensure you have
    everything you need for the site you are using
@@ -189,35 +190,35 @@
 -->
 
 ## Stats Explained
 
 Stats used in this library are
 documented [here](https://github.com/joeyagreco/leeger/blob/main/doc/stats.md).
 
-## Running Tests
-
-To run tests, run the following command:
-
-```bash
-  pytest
-```
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## Development
 
-### Formatting
+_Run these commands from the root folder_
+- Format Code: `./main fmt`
+- Run Unit Tests: `./main test`
+- Generate Coverage Report: `./main cov`
+
+### Running Tests
+
+Run the following command from the root folder:
+
+```bash
+  pytest
+```
 
-_Run these commands from the root folder (leeger) before committing._\
-**General Format:** `black --config=pyproject.toml . `\
-**Import/Variable Format:** `autoflake --config=pyproject.toml .`
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Credit
```

### Comparing `leeger-2.4.0/README.md` & `leeger-2.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
 // @formatter:on
 -->
 
 **Answer:**
 This error occurs when the Python version you are using is not 3.10 or greater.\
 Make sure you are using Python version 3.10 or a newer version.
 
+___
 **Q:**
 How do I use this library to pull stats from my online fantasy league?
 
 **A:**
 
 1. Find your fantasy site [here](https://github.com/joeyagreco/leeger#supported-league-loaders) and ensure you have
    everything you need for the site you are using
@@ -176,35 +177,35 @@
 -->
 
 ## Stats Explained
 
 Stats used in this library are
 documented [here](https://github.com/joeyagreco/leeger/blob/main/doc/stats.md).
 
-## Running Tests
-
-To run tests, run the following command:
-
-```bash
-  pytest
-```
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## Development
 
-### Formatting
+_Run these commands from the root folder_
+- Format Code: `./main fmt`
+- Run Unit Tests: `./main test`
+- Generate Coverage Report: `./main cov`
+
+### Running Tests
+
+Run the following command from the root folder:
+
+```bash
+  pytest
+```
 
-_Run these commands from the root folder (leeger) before committing._\
-**General Format:** `black --config=pyproject.toml . `\
-**Import/Variable Format:** `autoflake --config=pyproject.toml .`
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Credit
```

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/AWALAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/GameOutcomeAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/PlusMinusAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/PointsScoredAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/SSLAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/ScoringShareAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/ScoringStandardDeviationAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/SingleScoreAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/SmartWinsAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/TeamSummaryAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/all_time_calculator/__init__.py` & `leeger-2.5.0/leeger/calculator/all_time_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/parent/AllTimeCalculator.py` & `leeger-2.5.0/leeger/calculator/parent/AllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/parent/YearCalculator.py` & `leeger-2.5.0/leeger/calculator/parent/YearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/AWALYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/AWALYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/GameOutcomeYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/PlusMinusYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/PointsScoredYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/SSLYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/SSLYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/ScoringShareYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/ScoringStandardDeviationYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/SingleScoreYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/SmartWinsYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py` & `leeger-2.5.0/leeger/calculator/year_calculator/TeamSummaryYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/calculator/year_calculator/__init__.py` & `leeger-2.5.0/leeger/calculator/year_calculator/__init__.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/decorator/validators.py` & `leeger-2.5.0/leeger/decorator/validators.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/enum/MatchupType.py` & `leeger-2.5.0/leeger/enum/MatchupType.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/exception/__init__.py` & `leeger-2.5.0/leeger/exception/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from .DoesNotExistException import DoesNotExistException
+from .InvalidDivisionFormatException import InvalidDivisionFormatException
 from .InvalidFilterException import InvalidFilterException
 from .InvalidLeagueFormatException import InvalidLeagueFormatException
 from .InvalidMatchupFormatException import InvalidMatchupFormatException
 from .InvalidOwnerFormatException import InvalidOwnerFormatException
 from .InvalidTeamFormatException import InvalidTeamFormatException
 from .InvalidWeekFormatException import InvalidWeekFormatException
 from .InvalidYearFormatException import InvalidYearFormatException
```

### Comparing `leeger-2.4.0/leeger/league_loader/ESPNLeagueLoader.py` & `leeger-2.5.0/leeger/league_loader/ESPNLeagueLoader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 import espn_api.football as espn
 from espn_api.football import League as ESPNLeague
 from espn_api.football import Team as ESPNTeam
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.league_loader.LeagueLoader import LeagueLoader
+from leeger.model.league.Division import Division
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from leeger.validate import leagueValidation
@@ -36,25 +37,31 @@
         self,
         leagueId: str,
         years: list[int],
         *,
         espnS2: str = None,
         swid: str = None,
         ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
+        leagueName: Optional[str] = None,
     ):
         # validation
         try:
             int(leagueId)
         except ValueError:
             raise ValueError(f"League ID '{leagueId}' could not be turned into an int.")
-        super().__init__(leagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
+        super().__init__(
+            leagueId, years, ownerNamesAndAliases=ownerNamesAndAliases, leagueName=leagueName
+        )
 
         self.__espnS2 = espnS2
         self.__swid = swid
         self.__espnTeamIdToTeamMap: dict[str, Team] = dict()
+        self.__espnDivisionIdToDivisionMap: dict[
+            int, Division
+        ] = dict()  # holds the division info for ONLY the current year
 
     def __getAllLeagues(self) -> list[ESPNLeague]:
         espnLeagueYears = list()
         for year in self._years:
             espnLeagueYears.append(
                 espn.League(
                     league_id=int(self._leagueId),
@@ -86,15 +93,14 @@
     def __buildLeague(self, espnLeagues: list[ESPNLeague]) -> League:
         years = list()
         for espnLeague in espnLeagues:
             # save league name for each year
             self._leagueNameByYear[espnLeague.year] = espnLeague.settings.name
             self.__loadOwners(espnLeague.teams)
             years.append(self.__buildYear(espnLeague))
-        # use the league name from the most recent year
         return League(
             name=self._getLeagueName(), owners=self._owners, years=self._getValidYears(years)
         )
 
     def __loadOwners(self, espnTeams: list[ESPNTeam]) -> None:
         if self._owners is None:
             owners = list()
@@ -102,17 +108,29 @@
                 # get general owner name if there is one
                 generalOwnerName = self._getGeneralOwnerNameFromGivenOwnerName(espnTeam.owner)
                 ownerName = generalOwnerName if generalOwnerName is not None else espnTeam.owner
                 owners.append(Owner(name=ownerName))
             self._owners = owners
 
     def __buildYear(self, espnLeague: ESPNLeague) -> Year:
+        # save division info
+        for espnDivisionId, espnDivisionName in espnLeague.settings.division_map.items():
+            self.__espnDivisionIdToDivisionMap[espnDivisionId] = Division(name=espnDivisionName)
         teams = self.__buildTeams(espnLeague.teams)
         weeks = self.__buildWeeks(espnLeague)
-        return Year(yearNumber=espnLeague.year, teams=teams, weeks=weeks)
+        # TODO: see if there are cases where ESPN leagues do NOT have divisions
+        year = Year(
+            yearNumber=espnLeague.year,
+            teams=teams,
+            weeks=weeks,
+            divisions=list(self.__espnDivisionIdToDivisionMap.values()),
+        )
+        # clear division info
+        self.__espnDivisionIdToDivisionMap = dict()
+        return year
 
     def __buildWeeks(self, espnLeague: ESPNLeague) -> list[Week]:
         weeks = list()
         # current week seems to be the last week in the league
         for i in range(espnLeague.current_week):
             # get each teams matchup for that week
             matchups = list()
@@ -201,12 +219,14 @@
         for espnTeam in espnTeams:
             if espnTeam.team_id == espnTeamId:
                 return espnTeam
 
     def __buildTeams(self, espnTeams: list[ESPNTeam]) -> list[Team]:
         teams = list()
         for espnTeam in espnTeams:
+            # TODO: see if there are cases where ESPN leagues do NOT have divisions
+            divisionId = self.__espnDivisionIdToDivisionMap[espnTeam.division_id].id
             owner = self._getOwnerByName(espnTeam.owner)
-            team = Team(ownerId=owner.id, name=espnTeam.team_name)
+            team = Team(ownerId=owner.id, name=espnTeam.team_name, divisionId=divisionId)
             teams.append(team)
             self.__espnTeamIdToTeamMap[espnTeam.team_id] = team
         return teams
```

### Comparing `leeger-2.4.0/leeger/league_loader/FleaflickerLeagueLoader.py` & `leeger-2.5.0/leeger/league_loader/FleaflickerLeagueLoader.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,38 +9,45 @@
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from leeger.validate import leagueValidation
+from leeger.model.league.Division import Division
 
 
 class FleaflickerLeagueLoader(LeagueLoader):
     """
     Responsible for loading a League from Fleaflicker.
     https://www.fleaflicker.com/
     """
 
     def __init__(
         self,
         leagueId: str,
         years: list[int],
         *,
         ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
+        leagueName: Optional[str] = None,
     ):
         # validation
         try:
             int(leagueId)
         except ValueError:
             raise ValueError(f"League ID '{leagueId}' could not be turned into an int.")
-        super().__init__(leagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
+        super().__init__(
+            leagueId, years, ownerNamesAndAliases=ownerNamesAndAliases, leagueName=leagueName
+        )
 
         self.__fleaflickerTeamIdToOwnerMap: dict[int, Owner] = dict()
         self.__fleaflickerTeamIdToTeamMap: dict[int, Team] = dict()
+        self.__fleaflickerDivisionIdToDivisionMap: dict[
+            int, Division
+        ] = dict()  # holds the division info for ONLY the current year
 
     def __getAllLeagues(self) -> list[dict]:
         # return a list of all leagues
         fleaflickerLeagues = list()
         for year in self._years:
             fleaflickerLeagues.append(
                 LeagueInfoAPIClient.get_league_standings(
@@ -78,17 +85,30 @@
             self._leagueNameByYear[fleaflickerLeague["season"]] = fleaflickerLeague["league"][
                 "name"
             ]
             years.append(self.__buildYear(fleaflickerLeague))
         return League(name=self._getLeagueName(), owners=owners, years=self._getValidYears(years))
 
     def __buildYear(self, fleaflickerLeague: dict) -> Year:
+        # save division info
+        for fleaflickerDivision in fleaflickerLeague["divisions"]:
+            self.__fleaflickerDivisionIdToDivisionMap[fleaflickerDivision["id"]] = Division(
+                name=fleaflickerDivision["name"]
+            )
         teams = self.__buildTeams(fleaflickerLeague)
         weeks = self.__buildWeeks(fleaflickerLeague)
-        return Year(yearNumber=int(fleaflickerLeague["season"]), teams=teams, weeks=weeks)
+        year = Year(
+            yearNumber=int(fleaflickerLeague["season"]),
+            teams=teams,
+            weeks=weeks,
+            divisions=list(self.__fleaflickerDivisionIdToDivisionMap.values()),
+        )
+        # clear division info
+        self.__fleaflickerDivisionIdToDivisionMap = dict()
+        return year
 
     def __buildWeeks(self, fleaflickerLeague: dict) -> list[Week]:
         weeks = list()
         # get all weeks
         fleaflicker_league_scoreboard = ScoringAPIClient.get_league_scoreboard(
             sport=Sport.NFL,
             league_id=fleaflickerLeague["league"]["id"],
@@ -156,15 +176,19 @@
     def __buildTeams(self, fleaflickerLeague: dict) -> list[Team]:
         teams = list()
         for division in fleaflickerLeague["divisions"]:
             for team in division["teams"]:
                 teamName = team["name"]
                 teamId = team["id"]
                 owner = self.__fleaflickerTeamIdToOwnerMap[teamId]
-                team = Team(ownerId=owner.id, name=teamName)
+                team = Team(
+                    ownerId=owner.id,
+                    name=teamName,
+                    divisionId=self.__fleaflickerDivisionIdToDivisionMap[division["id"]].id,
+                )
                 teams.append(team)
                 self.__fleaflickerTeamIdToTeamMap[teamId] = team
         return teams
 
     def __loadOwners(self, fleaflickerLeagues: list[dict]) -> None:
         for fleaflickerLeague in fleaflickerLeagues:
             for division in fleaflickerLeague["divisions"]:
```

### Comparing `leeger-2.4.0/leeger/league_loader/LeagueLoader.py` & `leeger-2.5.0/leeger/league_loader/LeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py` & `leeger-2.5.0/leeger/league_loader/MyFantasyLeagueLeagueLoader.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from leeger.validate import leagueValidation
+from leeger.model.league.Division import Division
 
 
 class MyFantasyLeagueLeagueLoader(LeagueLoader):
     """
     Responsible for loading a League from MyFantasyLeague.
     http://home.myfantasyleague.com/
     """
@@ -24,24 +25,30 @@
         leagueId: str,
         years: list[int],
         *,
         mflUsername: str,
         mflPassword: str,
         mflUserAgentName: str,
         ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
+        leagueName: Optional[str] = None,
     ):
-        super().__init__(leagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
+        super().__init__(
+            leagueId, years, ownerNamesAndAliases=ownerNamesAndAliases, leagueName=leagueName
+        )
 
         self.__mflUsername = mflUsername
         self.__mflPassword = mflPassword
         self.__mflUserAgentName = mflUserAgentName
 
         self.__mflLeagueIdToYearMap: dict[str, int] = dict()
         self.__mflFranchiseIdToOwnerMap: dict[str, Owner] = dict()
         self.__mflFranchiseIdToTeamMap: dict[int, Team] = dict()
+        self.__mflDivisionIdToDivisionMap: dict[
+            str, Division
+        ] = dict()  # holds the division info for ONLY the current year
 
     def __getAllLeagues(self) -> list[dict]:
         mflLeagues: list[dict] = list()
 
         for year in self._years:
             APIConfig.add_config_for_year_and_league_id(
                 year=year,
@@ -85,18 +92,30 @@
         for mflLeague in mflLeagues:
             # save league name for each year
             self._leagueNameByYear[self.__mflLeagueIdToYearMap[mflLeague["id"]]] = mflLeague["name"]
             years.append(self.__buildYear(mflLeague))
         return League(name=self._getLeagueName(), owners=owners, years=self._getValidYears(years))
 
     def __buildYear(self, mflLeague: dict) -> Year:
+        # save division info
+        for division in mflLeague["divisions"]["division"]:
+            self.__mflDivisionIdToDivisionMap[division["id"]] = Division(name=division["name"])
         yearNumber = self.__mflLeagueIdToYearMap[mflLeague["id"]]
         teams = self.__buildTeams(mflLeague)
         weeks = self.__buildWeeks(mflLeague)
-        return Year(yearNumber=yearNumber, teams=teams, weeks=weeks)
+        # TODO: see if there are cases where MFL leagues do NOT have divisions
+        year = Year(
+            yearNumber=yearNumber,
+            teams=teams,
+            weeks=weeks,
+            divisions=list(self.__mflDivisionIdToDivisionMap.values()),
+        )
+        # clear division info
+        self.__mflDivisionIdToDivisionMap = dict()
+        return year
 
     def __buildWeeks(self, mflLeague: dict) -> list[Week]:
         yearNumber = self.__mflLeagueIdToYearMap[mflLeague["id"]]
         weeks = list()
         schedule: dict = CommonLeagueInfoAPIClient.get_schedule(
             year=yearNumber, league_id=mflLeague["id"]
         )["schedule"]
@@ -104,14 +123,16 @@
         playoffBracket: dict = CommonLeagueInfoAPIClient.get_playoff_bracket(
             year=yearNumber, league_id=mflLeague["id"], bracket_id="1"
         )["playoffBracket"]
 
         # we will assume that the "true" playoff bracket (i.e. the bracket where the winner of it is the league champion)
         # will always be the playoff bracket with id "1".
         # if this changes or is not the case, this will need to be refactored to reflect that.
+        # the reason we only care about this bracket (and not the other ones) is because we only need to know who won the championship from this info.
+        # we can get all playoff matchup data from the regular schedule
 
         # if there is only 1 object in the playoffRound field, it is a dict, otherwise it is a list
         playoffWeeks = list()
         if isinstance(playoffBracket["playoffRound"], dict):
             # only 1 playoff round
             playoffWeeks.append(playoffBracket["playoffRound"])
         else:
@@ -135,39 +156,34 @@
                 teamAHasTiebreaker = matchup["franchise"][0]["result"] == "W"
 
                 teamBMFLFranchiseId = matchup["franchise"][1]["id"]
                 teamBId = self.__mflFranchiseIdToTeamMap[teamBMFLFranchiseId].id
                 teamBScore = float(matchup["franchise"][1]["score"])
                 teamBHasTiebreaker = matchup["franchise"][1]["result"] == "W"
 
-                validPlayoffMatchup = False
-                validChampionshipMatchup = False
+                isChampionshipMatchup = False
 
                 matchupType = MatchupType.REGULAR_SEASON
                 if playoffsStarted:
                     # this is a playoff matchup or a championship matchup
+                    # NOTE: If there are MFL leagues that have matchups during playoff weeks that are
+                    # NOTE: NOT playoff matchups, this logic will need to be changed.
                     for playoffWeek in playoffWeeks:
-                        (
-                            currentValidPlayoffMatchup,
-                            currentValidChampionshipMatchup,
-                        ) = self.__getPlayoffMatchupBooleansForPlayoffWeek(
+                        currentIsChampionshipMatchup = self.__isChampionshipMatchup(
                             playoffWeek=playoffWeek,
                             playoffWeekNumbers=playoffWeekNumbers,
                             weekNumber=weekNumber,
                             teamAMFLFranchiseId=teamAMFLFranchiseId,
                             teamBMFLFranchiseId=teamBMFLFranchiseId,
                         )
-                        validPlayoffMatchup = validPlayoffMatchup or currentValidPlayoffMatchup
-                        validChampionshipMatchup = (
-                            validChampionshipMatchup or currentValidChampionshipMatchup
+                        isChampionshipMatchup = (
+                            isChampionshipMatchup or currentIsChampionshipMatchup
                         )
-                    matchupType = MatchupType.IGNORE
-                    if validPlayoffMatchup:
-                        matchupType = MatchupType.PLAYOFF
-                    if validChampionshipMatchup:
+                    matchupType = MatchupType.PLAYOFF
+                    if isChampionshipMatchup:
                         matchupType = MatchupType.CHAMPIONSHIP
 
                 matchups.append(
                     Matchup(
                         teamAId=teamAId,
                         teamBId=teamBId,
                         teamAScore=teamAScore,
@@ -179,80 +195,57 @@
                 )
             if len(matchups) > 0:
                 weeks.append(Week(weekNumber=weekNumber, matchups=matchups))
 
         return weeks
 
     @staticmethod
-    def __getPlayoffMatchupBooleansForPlayoffWeek(
+    def __isChampionshipMatchup(
         *,
         playoffWeek: dict,
         playoffWeekNumbers: list[int],
         weekNumber: int,
         teamAMFLFranchiseId: int,
         teamBMFLFranchiseId: int,
     ) -> tuple[bool, bool]:
-        """
-        Will return 2 booleans.
-        validPlayoffMatchup, validChampionshipMatchup
-        """
-
         # helper method
         def isValid(*, pGame: dict, aId: int, bId: int) -> bool:
             return (
                 aId == pGame["away"]["franchise_id"] or bId == pGame["away"]["franchise_id"]
             ) and (aId == pGame["home"]["franchise_id"] or bId == pGame["home"]["franchise_id"])
 
-        # this is a playoff matchup or a championship matchup
-        validPlayoffMatchup = False
-        validChampionshipMatchup = False
+        isChampionshipMatchup = False
 
         if weekNumber == max(playoffWeekNumbers):
             # this is the last week in the bracket, the championship week
             # if there is only 1 object in the playoffGame field, it is a dict, otherwise it is a list
             if isinstance(playoffWeek["playoffGame"], dict):
                 # only 1 game
                 # check if this matchup is the championship game
-                validChampionshipMatchup = isValid(
+                isChampionshipMatchup = isValid(
                     pGame=playoffWeek["playoffGame"],
                     aId=teamAMFLFranchiseId,
                     bId=teamBMFLFranchiseId,
                 )
             else:
                 # multiple games
                 # check if this matchup is the championship game
                 for playoffGame in playoffWeek["playoffGame"]:
-                    validChampionshipMatchup = validChampionshipMatchup or isValid(
-                        pGame=playoffGame, aId=teamAMFLFranchiseId, bId=teamBMFLFranchiseId
-                    )
-        else:
-            # playoff week, but not the championship week
-            # if there is only 1 object in the playoffGame field, it is a dict, otherwise it is a list
-            if isinstance(playoffWeek["playoffGame"], dict):
-                # only 1 game
-                # check if this matchup is a valid playoff matchup
-                validPlayoffMatchup = isValid(
-                    pGame=playoffWeek["playoffGame"],
-                    aId=teamAMFLFranchiseId,
-                    bId=teamBMFLFranchiseId,
-                )
-            else:
-                # multiple games
-                for playoffGame in playoffWeek["playoffGame"]:
-                    # check if this matchup is a valid playoff matchup
-                    validPlayoffMatchup = validPlayoffMatchup or isValid(
+                    isChampionshipMatchup = isChampionshipMatchup or isValid(
                         pGame=playoffGame, aId=teamAMFLFranchiseId, bId=teamBMFLFranchiseId
                     )
-        return validPlayoffMatchup, validChampionshipMatchup
+        return isChampionshipMatchup
 
     def __buildTeams(self, mflLeague: dict) -> list[Team]:
         teams = list()
         for franchise in mflLeague["franchises"]["franchise"]:
+            # TODO: see if there are cases where MFL leagues do NOT have divisions
+            divisionId = self.__mflDivisionIdToDivisionMap[franchise["division"]].id
             owner = self.__mflFranchiseIdToOwnerMap[franchise["id"]]
-            team = Team(name=franchise["name"], ownerId=owner.id)
+            team = Team(name=franchise["name"], ownerId=owner.id, divisionId=divisionId)
             self.__mflFranchiseIdToTeamMap[franchise["id"]] = team
             teams.append(team)
         return teams
 
     def __loadOwners(self, mflLeagues: list[dict]) -> None:
         for mflLeague in mflLeagues:
             for franchise in mflLeague["franchises"]["franchise"]:
```

### Comparing `leeger-2.4.0/leeger/league_loader/SleeperLeagueLoader.py` & `leeger-2.5.0/leeger/league_loader/SleeperLeagueLoader.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from leeger.validate import leagueValidation
 from leeger.exception.LeagueLoaderException import LeagueLoaderException
+from leeger.model.league.Division import Division
 
 
 class SleeperLeagueLoader(LeagueLoader):
     """
     Responsible for loading a League from Sleeper Fantasy Football.
     https://sleeper.com/
     """
@@ -35,23 +36,32 @@
 
     def __init__(
         self,
         mostRecentLeagueId: str,
         years: list[int],
         *,
         ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
+        leagueName: Optional[str] = None,
     ):
-        super().__init__(mostRecentLeagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
+        super().__init__(
+            mostRecentLeagueId,
+            years,
+            ownerNamesAndAliases=ownerNamesAndAliases,
+            leagueName=leagueName,
+        )
 
         self.__sleeperUserIdToOwnerMap: dict[str, Owner] = dict()
         self.__sleeperRosterIdToTeamMap: dict[int, Team] = dict()
         self.__SLEEPER_USERS_BY_LEAGUE_ID_CACHE = dict()  # functions as a cache for Sleeper Users
         self.__SLEEPER_SPORT_STATE_CACHE: SleeperSportState = (
             None  # functions as a cache for Sleeper SportState
         )
+        self.__sleeperDivisionIdToDivisionMap: dict[
+            int, Division
+        ] = dict()  # holds the division info for ONLY the current year
 
     def __resetCaches(self) -> None:
         self.__SLEEPER_USERS_BY_LEAGUE_ID_CACHE = dict()
         self.__SLEEPER_SPORT_STATE_CACHE = None
 
     def __getSleeperUsers(self, leagueId: str) -> list[SleeperUser]:
         if leagueId not in self.__SLEEPER_USERS_BY_LEAGUE_ID_CACHE:
@@ -73,15 +83,15 @@
         sleeperLeagues = list()
         years = self._years.copy()
         currentLeagueId = self._leagueId
         while len(years) > 0 and currentLeagueId not in self.__INVALID_SLEEPER_LEAGUE_IDS:
             currentLeague: SleeperLeague = LeagueAPIClient.get_league(league_id=currentLeagueId)
             if int(currentLeague.season) in years:
                 # we only want to add valid seasons
-                # NOTE: Not sure if we want to include SleeperSeasonStatus.POSTPONED here or not
+                # NOTE: Not sure if we should include SleeperSeasonStatus.POSTPONED here or not
                 if currentLeague.status not in (
                     SleeperSeasonStatus.COMPLETE,
                     SleeperSeasonStatus.IN_SEASON,
                     SleeperSeasonStatus.POST_SEASON,
                 ):
                     raise LeagueLoaderException(
                         f"Year {currentLeague.season} has a status that is not supported: '{currentLeague.status}'"
@@ -122,38 +132,48 @@
         for sleeperLeague in sleeperLeagues:
             # save league name for each year
             self._leagueNameByYear[int(sleeperLeague.season)] = sleeperLeague.name
             years.append(self.__buildYear(sleeperLeague))
         return League(name=self._getLeagueName(), owners=owners, years=self._getValidYears(years))
 
     def __buildYear(self, sleeperLeague: SleeperLeague) -> Year:
+        # save division info
+        for divisionNumber in range(1, sleeperLeague.settings.divisions + 1):
+            self.__sleeperDivisionIdToDivisionMap[divisionNumber] = Division(
+                name=getattr(sleeperLeague.metadata, f"division_{divisionNumber}")
+            )
         teams = self.__buildTeams(sleeperLeague)
         weeks = self.__buildWeeks(sleeperLeague)
         # add YearSettings
         yearSettings = YearSettings()
         if sleeperLeague.settings.league_average_match == 1:
             yearSettings.leagueMedianGames = True
-        return Year(
+        # TODO: see if there are cases where Sleeper leagues do NOT have divisions
+        year = Year(
             yearNumber=int(sleeperLeague.season),
             teams=teams,
             weeks=weeks,
             yearSettings=yearSettings,
+            divisions=list(self.__sleeperDivisionIdToDivisionMap.values()),
         )
+        # clear division info
+        self.__sleeperDivisionIdToDivisionMap = dict()
+        return year
 
     def __buildWeeks(self, sleeperLeague: SleeperLeague) -> list[Week]:
         weeks = list()
         # get regular season weeks
         # once we have found an incomplete week, all weeks after will also be incomplete
         foundIncompleteWeek = False
-        for i in range(sleeperLeague.settings.playoff_week_start - 1):
-            if not foundIncompleteWeek and self.__isCompletedWeek(i + 1, sleeperLeague):
+        for weekNumber in range(1, sleeperLeague.settings.playoff_week_start):
+            if not foundIncompleteWeek and self.__isCompletedWeek(weekNumber, sleeperLeague):
                 # get each teams matchup for that week
                 matchups = list()
                 sleeperMatchupsForThisWeek = LeagueAPIClient.get_matchups_for_week(
-                    league_id=sleeperLeague.league_id, week=i + 1
+                    league_id=sleeperLeague.league_id, week=weekNumber
                 )
                 sleeperMatchupIdToSleeperMatchupMap: dict[int, list[SleeperMatchup]] = dict()
                 for sleeperMatchup in sleeperMatchupsForThisWeek:
                     if sleeperMatchup.matchup_id in sleeperMatchupIdToSleeperMatchupMap.keys():
                         sleeperMatchupIdToSleeperMatchupMap[sleeperMatchup.matchup_id].append(
                             sleeperMatchup
                         )
@@ -180,15 +200,15 @@
                             teamAScore=teamASleeperMatchup.points,
                             teamBScore=teamBSleeperMatchup.points,
                             teamAHasTiebreaker=False,
                             teamBHasTiebreaker=False,
                             matchupType=MatchupType.REGULAR_SEASON,
                         )
                     )
-                weeks.append(Week(weekNumber=i + 1, matchups=matchups))
+                weeks.append(Week(weekNumber=weekNumber, matchups=matchups))
             else:
                 foundIncompleteWeek = True
         # get playoff weeks
         # NOTE: bye weeks will not be returned here. That's ok because we don't want those anyways
         allSleeperPlayoffMatchups = LeagueAPIClient.get_winners_bracket(
             league_id=sleeperLeague.league_id
         )
@@ -221,26 +241,36 @@
             )
             for weekNumber, roundNumber in playoffWeekRoundList:
                 # get each teams matchup for that week
                 matchups = list()
                 sleeperMatchupsForThisWeek = LeagueAPIClient.get_matchups_for_week(
                     league_id=sleeperLeague.league_id, week=weekNumber
                 )
+                # remove matchups that don't have a matchup id
+                sleeperMatchupsForThisWeek = [
+                    sleeperMatchup
+                    for sleeperMatchup in sleeperMatchupsForThisWeek
+                    if sleeperMatchup.matchup_id is not None
+                ]
                 # used to check if a Sleeper playoff matchup is in this week's matchups
-                sleeperMatchupIdsForThisWeek = [
+                sleeperMatchupIdsForThisWeek = {
                     sleeperMatchup.matchup_id for sleeperMatchup in sleeperMatchupsForThisWeek
-                ]
+                }
                 if self.__isCompletedWeek(weekNumber, sleeperLeague):
                     # sort matchups by roster IDs
                     rosterIdToSleeperMatchupMap: dict[int, SleeperMatchup] = dict()
                     for sleeperMatchup in sleeperMatchupsForThisWeek:
                         rosterIdToSleeperMatchupMap[sleeperMatchup.roster_id] = sleeperMatchup
                     for sleeperPlayoffMatchup in playoffRoundAndSleeperPlayoffMatchups[roundNumber]:
                         # check if this matchup is in this week (needed for leagues with multiple weeks in a single round)
-                        if sleeperPlayoffMatchup.matchup_id in sleeperMatchupIdsForThisWeek:
+                        if (
+                            sleeperPlayoffMatchup.matchup_id in sleeperMatchupIdsForThisWeek
+                            or sleeperLeague.settings.playoff_round_type_enum
+                            == SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND
+                        ):
                             # team A
                             teamARosterId = sleeperPlayoffMatchup.team_1_roster_id
                             teamA = self.__sleeperRosterIdToTeamMap[teamARosterId]
                             teamAPoints = rosterIdToSleeperMatchupMap[teamARosterId].points
                             teamAHasTiebreaker = (
                                 sleeperPlayoffMatchup.winning_roster_id
                                 == sleeperPlayoffMatchup.team_1_roster_id
@@ -296,30 +326,35 @@
     def __buildTeams(self, sleeperLeague: SleeperLeague) -> list[Team]:
         teams = list()
         sleeperUsers = self.__getSleeperUsers(sleeperLeague.league_id)
         sleeperRosters = LeagueAPIClient.get_rosters(league_id=sleeperLeague.league_id)
         for sleeperUser in sleeperUsers:
             # connect a sleeperUser to a sleeperRoster
             rosterId = None
+            divisionId = None
             for sleeperRoster in sleeperRosters:
                 if sleeperRoster.owner_id == sleeperUser.user_id:
                     rosterId = sleeperRoster.roster_id
+                    # TODO: see if there are cases where ESPN leagues do NOT have divisions
+                    divisionId = self.__sleeperDivisionIdToDivisionMap[
+                        sleeperRoster.settings.division
+                    ].id
             if rosterId is None:
                 raise DoesNotExistException(
                     f"No Roster ID match found for Sleeper User with ID: '{sleeperUser.user_id}'."
                 )
             owner = self.__sleeperUserIdToOwnerMap[sleeperUser.user_id]
             teamName = sleeperUser.display_name
             # if we can find a team name for this user, use it instead of their display name
             if (
                 isinstance(sleeperUser.metadata, dict)
                 and "team_name" in sleeperUser.metadata.keys()
             ):
                 teamName = sleeperUser.metadata["team_name"]
-            team = Team(ownerId=owner.id, name=teamName)
+            team = Team(ownerId=owner.id, name=teamName, divisionId=divisionId)
             teams.append(team)
             self.__sleeperRosterIdToTeamMap[rosterId] = team
         return teams
 
     def __loadOwners(self, sleeperLeagues: list[SleeperLeague]) -> None:
         for sleeperLeague in sleeperLeagues:
             sleeperUsers = self.__getSleeperUsers(sleeperLeague.league_id)
```

### Comparing `leeger-2.4.0/leeger/league_loader/YahooLeagueLoader.py` & `leeger-2.5.0/leeger/league_loader/YahooLeagueLoader.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,21 +34,27 @@
         mostRecentLeagueId: str,
         years: list[int],
         *,
         clientId: str,
         clientSecret: str,
         loginTimeoutSeconds: Optional[int] = 20,
         ownerNamesAndAliases: Optional[dict[str, list[str]]] = None,
+        leagueName: Optional[str] = None,
     ):
         # validation
         try:
             int(mostRecentLeagueId)
         except ValueError:
             raise ValueError(f"League ID '{mostRecentLeagueId}' could not be turned into an int.")
-        super().__init__(mostRecentLeagueId, years, ownerNamesAndAliases=ownerNamesAndAliases)
+        super().__init__(
+            mostRecentLeagueId,
+            years,
+            ownerNamesAndAliases=ownerNamesAndAliases,
+            leagueName=leagueName,
+        )
         self.__clientId = clientId
         self.__clientSecret = clientSecret
         self.__loginTimeoutSeconds = loginTimeoutSeconds
         self.__yahooManagerIdToOwnerMap: dict[int, Owner] = dict()
         self.__yahooTeamIdToTeamMap: dict[str, Team] = dict()
         self.__yearToTeamIdHasLostInPlayoffs: dict[int, dict[int, bool]] = dict()
```

### Comparing `leeger-2.4.0/leeger/model/abstract/UniqueId.py` & `leeger-2.5.0/leeger/model/abstract/UniqueId.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/model/filter/AllTimeFilters.py` & `leeger-2.5.0/leeger/model/filter/AllTimeFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/model/filter/YearFilters.py` & `leeger-2.5.0/leeger/model/filter/YearFilters.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,17 +52,16 @@
 
         onlyChampionship = kwargsCopy.pop("onlyChampionship", False)
         onlyPostSeason = kwargsCopy.pop("onlyPostSeason", False)
         onlyRegularSeason = kwargsCopy.pop("onlyRegularSeason", False)
         weekNumberStart = kwargsCopy.pop("weekNumberStart", year.weeks[0].weekNumber)
         weekNumberEnd = kwargsCopy.pop("weekNumberEnd", year.weeks[-1].weekNumber)
         includeMultiWeekMatchups = kwargsCopy.pop("includeMultiWeekMatchups", True)
-        kwargsCopy.pop("includeMatchupTypes", None)  # so we don't get an unused kwarg warning
 
-        GeneralUtil.warnForUnusedKwargs(kwargsCopy)
+        GeneralUtil.warnForUnusedKwargs(kwargsCopy, excludeKeys=["includeMatchupTypes"])
 
         ####################
         # validate filters #
         ####################
         # type checks
         if not isinstance(onlyChampionship, bool):
             raise InvalidFilterException("'onlyChampionship' must be type 'bool'")
```

### Comparing `leeger-2.4.0/leeger/model/league/League.py` & `leeger-2.5.0/leeger/model/league/League.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,79 @@
 from __future__ import annotations
 
 import copy
 from dataclasses import dataclass
 
 from leeger.exception import DoesNotExistException
+from leeger.model.abstract.EqualityCheck import EqualityCheck
 from leeger.model.abstract.UniqueId import UniqueId
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Year import Year
 from leeger.util.CustomLogger import CustomLogger
-from leeger.util.GeneralUtil import GeneralUtil
 from leeger.util.JSONDeserializable import JSONDeserializable
 from leeger.util.JSONSerializable import JSONSerializable
+from leeger.util.equality import modelEquals
 
 
 @dataclass(kw_only=True, eq=False)
-class League(UniqueId, JSONSerializable, JSONDeserializable):
+class League(UniqueId, EqualityCheck, JSONSerializable, JSONDeserializable):
     __LOGGER = CustomLogger.getLogger()
     name: str
     owners: list[Owner]
     years: list[Year]
 
     def __hash__(self):
         return hash(str(self.toJson()))
 
-    def __eq__(self, otherLeague: League) -> bool:
+    def equals(
+        self,
+        otherLeague: League,
+        *,
+        ignoreIds: bool = False,
+        ignoreBaseIds: bool = False,
+        logDifferences: bool = False,
+    ) -> bool:
         """
         Checks if *this* League is the same as the given League.
-        Does not check for equality of IDs, just values.
         """
-        equal = self.name == otherLeague.name
-        equal = equal and self.owners == otherLeague.owners
-        equal = equal and self.years == otherLeague.years
-        if not equal:
-            differences = GeneralUtil.findDifferentFields(
-                self.toJson(),
-                otherLeague.toJson(),
-                parentKey="League",
-                ignoreKeyNames=["id", "ownerId", "teamAId", "teamBId"],
-            )
-            self.__LOGGER.info(f"Differences: {differences}")
-        return equal
+
+        def listsEqual(
+            list1: list[Owner | Year],
+            list2: list[Owner | Year],
+            *,
+            ignoreIds: bool,
+            ignoreBaseIds: bool,
+        ) -> bool:
+            if len(list1) != len(list2):
+                return False
+            equal = True
+            for item1, item2 in zip(list1, list2):
+                equal = equal and item1.equals(
+                    item2, ignoreIds=ignoreIds, ignoreBaseIds=ignoreBaseIds
+                )
+            return equal
+
+        return modelEquals(
+            objA=self,
+            objB=otherLeague,
+            baseFields={"name", "owners", "years"},
+            parentKey="League",
+            ignoreIdFields=ignoreIds,
+            ignoreBaseIdField=ignoreBaseIds,
+            logDifferences=logDifferences,
+            equalityFunctionMap={"owners": listsEqual, "years": listsEqual},
+            equalityFunctionKwargsMap={
+                "owners": {"ignoreIds": ignoreIds, "ignoreBaseIds": ignoreBaseIds},
+                "years": {"ignoreIds": ignoreIds, "ignoreBaseIds": ignoreBaseIds},
+            },
+        )
+
+    def __eq__(self, otherLeague: League) -> bool:
+        self.__LOGGER.info("Use .equals() for more options when comparing League instances.")
+        return self.equals(otherLeague=otherLeague)
 
     def __add__(self, otherLeague: League) -> League:
         """
         Combines *this* League with the given League.
         The combined League will be validated before it is returned.
 
         Special behaviors:
```

### Comparing `leeger-2.4.0/leeger/model/league/Matchup.py` & `leeger-2.5.0/leeger/model/league/Matchup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 from dataclasses import dataclass
 from typing import Optional
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.exception import DoesNotExistException
 from leeger.exception.InvalidMatchupFormatException import InvalidMatchupFormatException
+from leeger.model.abstract.EqualityCheck import EqualityCheck
 from leeger.model.abstract.UniqueId import UniqueId
 from leeger.model.league_helper.Performance import Performance
 from leeger.util.CustomLogger import CustomLogger
-from leeger.util.GeneralUtil import GeneralUtil
 from leeger.util.JSONDeserializable import JSONDeserializable
 from leeger.util.JSONSerializable import JSONSerializable
+from leeger.util.equality import modelEquals
 
 
 @dataclass(kw_only=True, eq=False)
-class Matchup(UniqueId, JSONSerializable, JSONDeserializable):
+class Matchup(UniqueId, EqualityCheck, JSONSerializable, JSONDeserializable):
     __LOGGER = CustomLogger.getLogger()
     teamAId: str
     teamBId: str
     teamAScore: float | int
     teamBScore: float | int
     matchupType: MatchupType = MatchupType.REGULAR_SEASON
     teamAHasTiebreaker: Optional[bool] = False
@@ -36,46 +37,46 @@
             )
 
         if self.teamAHasTiebreaker is None:
             self.teamAHasTiebreaker = False
         if self.teamBHasTiebreaker is None:
             self.teamBHasTiebreaker = False
 
-    def __eq__(self, otherMatchup: Matchup) -> bool:
+    def equals(
+        self,
+        otherMatchup: Matchup,
+        *,
+        ignoreIds: bool = False,
+        ignoreBaseIds: bool = False,
+        logDifferences: bool = False,
+    ) -> bool:
         """
         Checks if *this* Matchup is the same as the given Matchup.
-        Does not check for equality of IDs, just values.
         """
-        equal = self.teamAScore == otherMatchup.teamAScore
-        equal = equal and self.teamBScore == otherMatchup.teamBScore
-        equal = equal and self.matchupType == otherMatchup.matchupType
-        equal = equal and self.teamAHasTiebreaker == otherMatchup.teamAHasTiebreaker
-        equal = equal and self.teamBHasTiebreaker == otherMatchup.teamBHasTiebreaker
-        # warn if this is going to return True but ID based fields are not equal
-        if equal:
-            notEqualStrings = list()
-            if self.teamAId != otherMatchup.teamAId:
-                notEqualStrings.append("teamAId")
-            if self.teamBId != otherMatchup.teamBId:
-                notEqualStrings.append("teamBId")
-            if self.multiWeekMatchupId != otherMatchup.multiWeekMatchupId:
-                notEqualStrings.append("multiWeekMatchupId")
-            if len(notEqualStrings) > 0:
-                self.__LOGGER.warning(
-                    f"Returning True for equality check when {notEqualStrings} are not equal."
-                )
-        else:
-            differences = GeneralUtil.findDifferentFields(
-                self.toJson(),
-                otherMatchup.toJson(),
-                parentKey="Matchup",
-                ignoreKeyNames=["id", "ownerId", "teamAId", "teamBId"],
-            )
-            self.__LOGGER.info(f"Differences: {differences}")
-        return equal
+
+        return modelEquals(
+            objA=self,
+            objB=otherMatchup,
+            baseFields={
+                "teamAScore",
+                "teamBScore",
+                "matchupType",
+                "teamAHasTiebreaker",
+                "teamBHasTiebreaker",
+            },
+            idFields={"teamAId", "teamBId", "multiWeekMatchupId"},
+            parentKey="Matchup",
+            ignoreIdFields=ignoreIds,
+            ignoreBaseIdField=ignoreBaseIds,
+            logDifferences=logDifferences,
+        )
+
+    def __eq__(self, otherMatchup: Matchup) -> bool:
+        self.__LOGGER.info("Use .equals() for more options when comparing Matchup instances.")
+        return self.equals(otherMatchup=otherMatchup)
 
     def splitToPerformances(self) -> tuple[Performance, Performance]:
         """
         Splits this Matchup into 2 Performances.
         """
         performanceA = Performance(
             teamId=self.teamAId,
```

### Comparing `leeger-2.4.0/leeger/model/league/YearSettings.py` & `leeger-2.5.0/leeger/model/league/YearSettings.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,53 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
+from leeger.model.abstract.EqualityCheck import EqualityCheck
 from leeger.util.CustomLogger import CustomLogger
-from leeger.util.GeneralUtil import GeneralUtil
 
 from leeger.util.JSONDeserializable import JSONDeserializable
 from leeger.util.JSONSerializable import JSONSerializable
+from leeger.util.equality import modelEquals
 
 
 @dataclass(kw_only=True, eq=False)
-class YearSettings(JSONSerializable, JSONDeserializable):
+class YearSettings(EqualityCheck, JSONSerializable, JSONDeserializable):
     __LOGGER = CustomLogger.getLogger()
     leagueMedianGames: Optional[bool] = False
 
     def __post_init__(self):
         if self.leagueMedianGames is None:
             self.leagueMedianGames = False
 
-    def __eq__(self, otherYearSettings: YearSettings) -> bool:
+    def equals(
+        self,
+        otherYearSettings: YearSettings,
+        *,
+        ignoreIds: bool = False,
+        ignoreBaseIds: bool = False,
+        logDifferences: bool = False,
+    ) -> bool:
         """
         Checks if *this* YearSettings is the same as the given YearSettings.
         """
-        equal = self.leagueMedianGames == otherYearSettings.leagueMedianGames
-        if not equal:
-            differences = GeneralUtil.findDifferentFields(
-                self.toJson(),
-                otherYearSettings.toJson(),
-                parentKey="YearSettings",
-                ignoreKeyNames=["id", "ownerId", "teamAId", "teamBId"],
-            )
-            self.__LOGGER.info(f"Differences: {differences}")
-        return equal
+
+        return modelEquals(
+            objA=self,
+            objB=otherYearSettings,
+            baseFields={"leagueMedianGames"},
+            parentKey="YearSettings",
+            ignoreIdFields=ignoreIds,
+            ignoreBaseIdField=ignoreBaseIds,
+            logDifferences=logDifferences,
+        )
+
+    def __eq__(self, otherYearSettings: YearSettings) -> bool:
+        self.__LOGGER.info("Use .equals() for more options when comparing YearSettings instances.")
+        return self.equals(otherYearSettings=otherYearSettings)
 
     def toJson(self) -> dict:
         return {"leagueMedianGames": self.leagueMedianGames}
 
     @staticmethod
     def fromJson(d: dict) -> YearSettings:
         return YearSettings(leagueMedianGames=d.get("leagueMedianGames"))
```

### Comparing `leeger-2.4.0/leeger/model/league_helper/Performance.py` & `leeger-2.5.0/leeger/model/league_helper/Performance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,57 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.exception import InvalidMatchupFormatException
+from leeger.model.abstract.EqualityCheck import EqualityCheck
 from leeger.model.abstract.UniqueId import UniqueId
 from leeger.util.CustomLogger import CustomLogger
 from leeger.util.JSONSerializable import JSONSerializable
+from leeger.util.equality import modelEquals
 
 
 @dataclass(kw_only=True, eq=False)
-class Performance(UniqueId, JSONSerializable):
+class Performance(UniqueId, EqualityCheck, JSONSerializable):
     __LOGGER = CustomLogger.getLogger()
     teamId: str
     teamScore: float | int
     hasTiebreaker: bool = False
     matchupType: MatchupType = MatchupType.REGULAR_SEASON
     # This is used to link matchups that span over multiple weeks
     multiWeekMatchupId: Optional[str] = None
 
-    def __eq__(self, otherPerformance: Performance) -> bool:
+    def equals(
+        self,
+        otherPerformance: Performance,
+        *,
+        ignoreIds: bool = False,
+        ignoreBaseIds: bool = False,
+        logDifferences: bool = False,
+    ) -> bool:
         """
         Checks if *this* Performance is the same as the given Performance.
-        Does not check for equality of IDs, just values.
         """
-        equal = self.teamScore == otherPerformance.teamScore
-        equal = equal and self.hasTiebreaker == otherPerformance.hasTiebreaker
-        equal = equal and self.matchupType == otherPerformance.matchupType
-        # warn if this is going to return True but ID based fields are not equal
-        if equal:
-            notEqualStrings = list()
-            if self.teamId != otherPerformance.teamId:
-                notEqualStrings.append("teamId")
-            if len(notEqualStrings) > 0:
-                self.__LOGGER.warning(
-                    f"Returning True for equality check when {notEqualStrings} are not equal."
-                )
-        return equal
+
+        return modelEquals(
+            objA=self,
+            objB=otherPerformance,
+            baseFields={"teamId", "teamScore", "hasTiebreaker", "matchupType"},
+            idFields={"multiWeekMatchupId"},
+            parentKey="Performance",
+            ignoreIdFields=ignoreIds,
+            ignoreBaseIdField=ignoreBaseIds,
+            logDifferences=logDifferences,
+        )
+
+    def __eq__(self, otherPerformance: Performance) -> bool:
+        self.__LOGGER.info("Use .equals() for more options when comparing Performance instances.")
+        return self.equals(otherPerformance=otherPerformance)
 
     def __add__(self, otherPerformance: Performance):
         """
         Adds 2 Performances together.
 
         Returns:
             leeger.model.league.Matchup
```

### Comparing `leeger-2.4.0/leeger/model/stat/AllTimeStatSheet.py` & `leeger-2.5.0/leeger/model/stat/AllTimeStatSheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/model/stat/YearStatSheet.py` & `leeger-2.5.0/leeger/model/stat/YearStatSheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/util/CustomFormatter.py` & `leeger-2.5.0/leeger/util/CustomFormatter.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/util/CustomLogger.py` & `leeger-2.5.0/leeger/util/CustomLogger.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/util/Deci.py` & `leeger-2.5.0/leeger/util/Deci.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/util/GeneralUtil.py` & `leeger-2.5.0/leeger/util/GeneralUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 from typing import Any, Optional
+from leeger.util.ConfigReader import ConfigReader
 
 from leeger.util.CustomLogger import CustomLogger
 from leeger.util.Deci import Deci
 
 
 class GeneralUtil:
     @staticmethod
     def filter(*, value: Any, list_: list) -> list:
         """
         Filters out the given value from the given list.
         """
         return [v for v in list_ if v is not value]
 
     @staticmethod
-    def warnForUnusedKwargs(kwargs: dict) -> None:
+    def warnForUnusedKwargs(
+        kwargs: dict[str, Any], *, excludeKeys: Optional[list[str]] = None
+    ) -> None:
         """
         Logs a warning for each present kwarg in the given dict.
+        Will ignore kwargs with a key in excludeKeys.
         """
         LOGGER = CustomLogger.getLogger()
-        # this is a list of common kwargs that sometimes linger in kwargs to be used later.
-        IGNORE_KWARGS = ["validate"]
-        unused_kwargs = [kwarg for kwarg in kwargs.keys() if kwarg not in IGNORE_KWARGS]
+
+        excludeKeys = excludeKeys if excludeKeys is not None else list()
+        # get the list of common kwargs that sometimes linger in kwargs to be passed down and used later.
+        defaultExcludeKeys = ConfigReader.get("KWARGS", "WARNING_EXCLUDE_KEYS", asType=list)
+        excludeKeys += defaultExcludeKeys
+
+        unused_kwargs = [kwarg for kwarg in kwargs.keys() if kwarg not in excludeKeys]
         for kwarg in unused_kwargs:
             LOGGER.warning(f"Keyword argument '{kwarg}' unused.")
 
     @staticmethod
     def safeSum(*numbers) -> Optional[Deci | int | float]:
         """
         Safely adds numbers where None is ignored.
```

### Comparing `leeger-2.4.0/leeger/util/excel.py` & `leeger-2.5.0/leeger/util/excel.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,24 @@
 from leeger.model.filter import AllTimeFilters, YearFilters
 from leeger.model.league import Year, League
 from leeger.util.excel_helper import (
     allTimeTeamsStatSheet,
     yearMatchupsStatSheet,
     allTimeMatchupsStatSheet,
 )
+from leeger.util.navigator.YearNavigator import YearNavigator
 from leeger.util.stat_sheet import yearStatSheet, leagueStatSheet
 
 
-def leagueToExcel(league: League, filePath: Optional[str] = None, **kwargs) -> Workbook:
+def leagueToExcel(
+    league: League, filePath: Optional[str] = None, overwrite: bool = False, **kwargs
+) -> Workbook:
     """
     Saves the given League object to an Excel file.
     """
-    overwrite = kwargs.pop("overwrite", False)
 
     if league is None:
         raise ValueError("'league' has not been set.")
     if filePath is not None:
         if os.path.exists(filePath) and not overwrite:
             raise FileExistsError(
                 f"Cannot create file at path: '{filePath}' because there is already a file there."
@@ -74,23 +76,31 @@
     index = len(workbook.sheetnames)
     workbook.create_sheet("All Time Teams", index=index)
     worksheet = workbook["All Time Teams"]
 
     allTimeTeamsStatSheet_ = allTimeTeamsStatSheet(league, **kwargs.copy())
 
     allTimeFilters = AllTimeFilters.preferredOrderWithTitle(league, **kwargs.copy())
+
+    # see if we have a division column
+    # if we do, shift the frozen panes 1 column to the right
+    freezePanes = "D2"
+    for title, _ in allTimeTeamsStatSheet_:
+        if title == "Division":
+            freezePanes = "E2"
+
     _populateWorksheet(
         worksheet=worksheet,
         workbook=workbook,
         displayName="AllTimeTeamStats",
         titlesAndStatDicts=allTimeTeamsStatSheet_,
         entityIds=allTimeTeamIds,
         entityIdToColorMap=teamIdToColorMap,
         legendKeyValues=allTimeFilters,
-        freezePanes="D2",
+        freezePanes=freezePanes,
         saveToFilepath=filePath,
     )
 
     # add All-Time matchups stats sheet
     # figure out index to put this sheet into
     # we want the sheets to be ordered: oldest year -> newest year -> all time teams -> all time matchups -> all time owners
     index = len(workbook.sheetnames)
@@ -156,53 +166,63 @@
         workbook.create_sheet(f"{year.yearNumber} Matchups", index=1)
         # remove default sheet
         del workbook["Sheet"]
     else:
         # figure out index to put this sheet into
         # we want the years as sheets in order from oldest -> newest year
         index = 0
-        for i, sheetname in enumerate(workbook.sheetnames):
+        for sheetname in workbook.sheetnames:
             if year.yearNumber > int(sheetname[:5]):
                 index += 1
         workbook.create_sheet(f"{year.yearNumber} Teams", index=index)
         workbook.create_sheet(f"{year.yearNumber} Matchups", index=index + 1)
     worksheet = workbook[f"{year.yearNumber} Teams"]
 
     # get team names
     # and
     # make sure we have the same color for owners and their teams across sheets
     ownerIdToSeedMap = dict()
     teamIdToNameMap = dict()
+    teamIdToDivisionNameMap = dict()
     for team in year.teams:
         ownerIdToSeedMap[team.ownerId] = f"{team.ownerId}{datetime.now().date()}"
         teamIdToNameMap[team.id] = team.name
+        if team.divisionId:
+            teamIdToDivisionNameMap[team.id] = YearNavigator.getDivisionById(
+                year, team.divisionId
+            ).name
     ownerIdToColorMap = dict()
     for ownerId, seed in ownerIdToSeedMap.items():
         ownerIdToColorMap[ownerId] = _getRandomColor(0.5, seed)
 
     teamIdToColorMap = dict()
     teamIds = list()
     for team in year.teams:
         teamIdToColorMap[team.id] = ownerIdToColorMap[team.ownerId]
         teamIds.append(team.id)
 
     yearFilters = YearFilters.preferredOrderWithTitle(year, **kwargs.copy())
 
     yearStatsWithTitles = yearStatSheet(year, **kwargs.copy()).preferredOrderWithTitle()
     yearStatsWithTitles.insert(0, ("Team", teamIdToNameMap))
+
+    freezePanes = "B2"
+    if len(year.divisions) > 0:
+        yearStatsWithTitles.insert(1, ("Division", teamIdToDivisionNameMap))
+        freezePanes = "C2"
     # save Year teams to Excel sheet
     _populateWorksheet(
         worksheet=worksheet,
         workbook=workbook,
         displayName=f"Teams{year.yearNumber}",
         titlesAndStatDicts=yearStatsWithTitles,
         entityIds=teamIds,
         entityIdToColorMap=teamIdToColorMap,
         legendKeyValues=yearFilters,
-        freezePanes="B2",
+        freezePanes=freezePanes,
     )
 
     (yearMatchupsWithTitles, modifiedMatchupIdToOwnerIdMap) = yearMatchupsStatSheet(
         year, **kwargs.copy()
     )
     modifiedMatchupIdToColorMap: dict = dict()
     for modifiedMatchupId, ownerId in modifiedMatchupIdToOwnerIdMap.items():
```

### Comparing `leeger-2.4.0/leeger/util/excel_helper.py` & `leeger-2.5.0/leeger/util/excel_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,31 @@
 
 def allTimeTeamsStatSheet(league: League, **kwargs) -> list[tuple[str, dict]]:
     allTimeTeamsStatsWithTitles: list[tuple[str, dict]] = list()
     for year in league.years:
         ownerNames: dict[str, str] = dict()
         years: dict[str, int] = dict()
         teamIdToNameMap = dict()
+        teamIdToDivisionNameMap = dict()
         for team in year.teams:
             ownerNames[team.id] = LeagueNavigator.getOwnerById(league, team.ownerId).name
             years[team.id] = year.yearNumber
             teamIdToNameMap[team.id] = team.name
+            if team.divisionId:
+                teamIdToDivisionNameMap[team.id] = YearNavigator.getDivisionById(
+                    year, team.divisionId
+                ).name
         yearStatsWithTitles = yearStatSheet(
             year, ownerNames=ownerNames, years=years, **kwargs
         ).preferredOrderWithTitle()
 
         yearStatsWithTitles.insert(0, ("Team", teamIdToNameMap))
+        if len(year.divisions) > 0:
+            yearStatsWithTitles.insert(2, ("Division", teamIdToDivisionNameMap))
+
         allTimeTeamsStatsWithTitles += yearStatsWithTitles
 
     # condense stats with titles so there's only 1 list value for each title
     condensedAllTimeTeamsStatsWithTitles: list[tuple[str, dict]] = list()
     for titleStr, statsDict in allTimeTeamsStatsWithTitles:
         allTitlesInCondensedList = list()
         if len(condensedAllTimeTeamsStatsWithTitles) > 0:
```

### Comparing `leeger-2.4.0/leeger/util/navigator/LeagueNavigator.py` & `leeger-2.5.0/leeger/util/navigator/LeagueNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/util/navigator/MatchupNavigator.py` & `leeger-2.5.0/leeger/util/navigator/MatchupNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/util/navigator/WeekNavigator.py` & `leeger-2.5.0/leeger/util/navigator/WeekNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/util/navigator/YearNavigator.py` & `leeger-2.5.0/leeger/util/navigator/YearNavigator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 
 from leeger.enum import MatchupType
 from leeger.exception import DoesNotExistException
 from leeger.model.filter.YearFilters import YearFilters
 from leeger.model.league import Matchup, Team
+from leeger.model.league.Division import Division
 from leeger.model.league.Year import Year
 
 
 class YearNavigator:
     """
     Used to navigate the Year model.
     """
@@ -17,15 +18,24 @@
         return [team.id for team in year.teams]
 
     @staticmethod
     def getTeamById(year: Year, teamId: str) -> Team:
         for team in year.teams:
             if team.id == teamId:
                 return team
-        raise DoesNotExistException(f"Team with ID {teamId} does not exist in the given Year.")
+        raise DoesNotExistException(f"Team with ID '{teamId}' does not exist in the given Year.")
+
+    @staticmethod
+    def getDivisionById(year: Year, divisionId: str) -> Division:
+        for division in year.divisions:
+            if division.id == divisionId:
+                return division
+        raise DoesNotExistException(
+            f"Division with ID '{divisionId}' does not exist in the given Year."
+        )
 
     @classmethod
     def getNumberOfGamesPlayed(
         cls,
         year: Year,
         yearFilters: YearFilters,
         countMultiWeekMatchupsAsOneGame=False,
```

### Comparing `leeger-2.4.0/leeger/util/stat_sheet.py` & `leeger-2.5.0/leeger/util/stat_sheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/validate/leagueValidation.py` & `leeger-2.5.0/leeger/validate/leagueValidation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from functools import lru_cache
 
 from leeger.exception.InvalidLeagueFormatException import InvalidLeagueFormatException
 from leeger.model.league.League import League
+from leeger.model.league.Owner import Owner
+from leeger.model.league.Year import Year
 from leeger.validate import ownerValidation, yearValidation
 
 """
 Checker Functions
 
     - Will raise the appropriate exception if an incorrectly-formatted League is passed.
     - Will do nothing if a properly-formatted League is passed.
@@ -48,18 +50,22 @@
 
 def checkAllTypes(league: League) -> None:
     """
     Checks all types that are within the League object.
     """
     if not isinstance(league.name, str):
         raise InvalidLeagueFormatException("name must be type 'str'.")
-    if not isinstance(league.owners, list):
-        raise InvalidLeagueFormatException("owners must be type 'list'.")
-    if not isinstance(league.years, list):
-        raise InvalidLeagueFormatException("years must be type 'list'.")
+    if not isinstance(league.owners, list) or not all(
+        isinstance(owner, Owner) for owner in league.owners
+    ):
+        raise InvalidLeagueFormatException("owners must be type 'list[Owner]'.")
+    if not isinstance(league.years, list) or not all(
+        isinstance(year, Year) for year in league.years
+    ):
+        raise InvalidLeagueFormatException("years must be type 'list[Year]'.")
 
 
 def checkForDuplicateOwners(league: League) -> None:
     """
     Checks that all Owners are unique instances.
     """
     ownerInstanceIds = list()
```

### Comparing `leeger-2.4.0/leeger/validate/matchupValidation.py` & `leeger-2.5.0/leeger/validate/matchupValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/leeger/validate/weekValidation.py` & `leeger-2.5.0/leeger/validate/weekValidation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from leeger.enum.MatchupType import MatchupType
 from leeger.exception.InvalidWeekFormatException import InvalidWeekFormatException
+from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Week import Week
 from leeger.validate import matchupValidation
 
 
 def runAllChecks(week: Week) -> None:
     """
     Runs all checks on the given Week.
@@ -19,16 +20,18 @@
 
 
 def checkAllTypes(week: Week) -> None:
     """
     Checks all types that are within the Week object.
     """
 
-    if not isinstance(week.matchups, list):
-        raise InvalidWeekFormatException("matchups must be type 'list'.")
+    if not isinstance(week.matchups, list) or not all(
+        isinstance(matchup, Matchup) for matchup in week.matchups
+    ):
+        raise InvalidWeekFormatException("matchups must be type 'list[Matchup]'.")
     if not isinstance(week.weekNumber, int):
         raise InvalidWeekFormatException("weekNumber must be type 'int'.")
 
 
 def checkForDuplicateMatchups(week: Week) -> None:
     """
     Checks that all Matchups are unique instances.
```

### Comparing `leeger-2.4.0/leeger/validate/yearValidation.py` & `leeger-2.5.0/leeger/validate/yearValidation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 from functools import lru_cache
 
 from leeger.exception.InvalidYearFormatException import InvalidYearFormatException
 from leeger.model.league import Matchup, YearSettings
+from leeger.model.league.Division import Division
+from leeger.model.league.Team import Team
+from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from leeger.util.navigator import YearNavigator
-from leeger.validate import teamValidation, weekValidation, yearSettingsValidation
+from leeger.validate import (
+    divisionValidation,
+    teamValidation,
+    weekValidation,
+    yearSettingsValidation,
+)
 
 
 @lru_cache(maxsize=None)
 def runAllChecks(year: Year) -> None:
     """
     Runs all checks on the given Year.
     The order in which these are called matters.
     """
     checkAllTypes(year)
     checkYearSettings(year)
     checkAllWeeks(year)
     checkAllTeams(year)
+    checkAllDivisions(year)
     checkForDuplicateTeams(year)
     checkForDuplicateWeeks(year)
+    checkForDuplicateDivisions(year)
     checkAtLeastOneWeekInYear(year)
     checkWeekNumberingInYear(year)
     checkPlayoffWeekOrderingInYear(year)
     checkAtLeastTwoTeamsInYear(year)
     checkGivenYearHasValidYearNumber(year)
     checkTeamNamesInYear(year)
+    checkDivisionNamesInYear(year)
     checkTeamOwnerIdsInYear(year)
     checkEveryTeamInYearIsInAMatchup(year)
     checkMultiWeekMatchupsAreInConsecutiveWeeks(year)
     checkMultiWeekMatchupsAreInMoreThanOneWeekOrAreNotTheMostRecentWeek(year)
     checkMultiWeekMatchupsWithSameIdHaveSameMatchupType(year)
     checkMultiWeekMatchupsWithSameIdHaveSameTeamIds(year)
     checkMultiWeekMatchupsWithSameIdHaveSameTiebreakers(year)
+    checkEitherAllTeamsAreInADivisionOrNoTeamsAreInADivision(year)
+    checkDivisionIdsMatchTeamDivisionIds(year)
+    checkDivisionsHaveNoDuplicateIds(year)
 
 
 def checkYearSettings(year: Year) -> None:
     """
     Runs all checks on the given Year's YearSettings.
     """
     yearSettingsValidation.runAllChecks(year.yearSettings)
@@ -53,25 +67,37 @@
     """
     Runs all checks on all Teams.
     """
     for team in year.teams:
         teamValidation.runAllChecks(team)
 
 
+def checkAllDivisions(year: Year) -> None:
+    """
+    Runs all checks on all Divisions.
+    """
+    for division in year.divisions:
+        divisionValidation.runAllChecks(division)
+
+
 def checkAllTypes(year: Year) -> None:
     """
     Runs all checks on the given Year.
     """
 
     if not isinstance(year.yearNumber, int):
         raise InvalidYearFormatException("yearNumber must be type 'int'.")
-    if not isinstance(year.teams, list):
-        raise InvalidYearFormatException("teams must be type 'list'.")
-    if not isinstance(year.weeks, list):
-        raise InvalidYearFormatException("weeks must be type 'list'.")
+    if not isinstance(year.teams, list) or not all(isinstance(team, Team) for team in year.teams):
+        raise InvalidYearFormatException("teams must be type 'list[Team]'.")
+    if not isinstance(year.weeks, list) or not all(isinstance(week, Week) for week in year.weeks):
+        raise InvalidYearFormatException("weeks must be type 'list[Week]'.")
+    if not isinstance(year.divisions, list) or not all(
+        isinstance(division, Division) for division in year.divisions
+    ):
+        raise InvalidYearFormatException("divisions must be type 'list[Division]'.")
     if not isinstance(year.yearSettings, YearSettings):
         raise InvalidYearFormatException("yearSettings must be type 'YearSettings'.")
 
 
 def checkForDuplicateTeams(year: Year) -> None:
     """
     Checks that all Teams are unique instances.
@@ -92,14 +118,47 @@
     for week in year.weeks:
         if id(week) in weekInstanceIds:
             raise InvalidYearFormatException("Weeks must all be unique instances.")
         else:
             weekInstanceIds.append(id(week))
 
 
+def checkForDuplicateDivisions(year: Year) -> None:
+    """
+    Checks that all Weeks are unique instances.
+    """
+    divisionInstanceIds = list()
+    for division in year.divisions:
+        if id(division) in divisionInstanceIds:
+            raise InvalidYearFormatException("Divisions must all be unique instances.")
+        else:
+            divisionInstanceIds.append(id(division))
+
+
+def checkDivisionNamesInYear(year: Year) -> None:
+    """
+    Checks that each division in the given Year has a unique name
+    Counts names as too similar if they are the same
+        - when whitespace is removed
+        - when case is uniform
+    """
+    if len(set([division.name for division in year.divisions])) != len(
+        [division.name for division in year.divisions]
+    ):
+        raise InvalidYearFormatException(
+            f"Year {year.yearNumber} has divisions with duplicate names."
+        )
+    if len(set([division.name.strip().upper() for division in year.divisions])) != len(
+        [division.name for division in year.divisions]
+    ):
+        raise InvalidYearFormatException(
+            f"Year {year.yearNumber} has divisions with very similar names."
+        )
+
+
 def checkAtLeastOneWeekInYear(year: Year) -> None:
     """
     Checks that there is a minimum of 1 week in the given Year.
     """
     if len(year.weeks) == 0:
         raise InvalidYearFormatException(f"Year {year.yearNumber} does not have at least 1 week.")
 
@@ -344,7 +403,69 @@
                 matchup.teamAHasTiebreaker == matchupList[0].teamAHasTiebreaker
                 and matchup.teamBHasTiebreaker == matchupList[0].teamBHasTiebreaker
                 for matchup in matchupList
             ):
                 raise InvalidYearFormatException(
                     f"Multi-week matchups with ID '{mwmid}' do not all have the same tiebreakers."
                 )
+
+
+def checkEitherAllTeamsAreInADivisionOrNoTeamsAreInADivision(year: Year):
+    """
+    Checks that either all teams are in a division or no teams are in a division.
+    """
+    allTeamDivisionIds = [team.divisionId for team in year.teams]
+
+    if not (
+        all(isinstance(divisionId, str) for divisionId in allTeamDivisionIds)
+        or all(divisionId is None for divisionId in allTeamDivisionIds)
+    ):
+        raise InvalidYearFormatException(
+            f"Only some teams in Year {year.yearNumber} have a Division ID."
+        )
+
+
+def checkDivisionIdsMatchTeamDivisionIds(year: Year):
+    """
+    Checks that the divisions in a year exactly match all division IDs for all teams in a year.
+    """
+    allUniqueDivisionIds = {division.id for division in year.divisions}
+    allUniqueTeamDivisionIds = {
+        team.divisionId for team in year.teams if team.divisionId is not None
+    }
+
+    if allUniqueDivisionIds != allUniqueTeamDivisionIds:
+        if len(allUniqueDivisionIds) == 0:
+            # no divisions, some team division ids
+            raise InvalidYearFormatException(
+                f"Teams in Year {year.yearNumber} have Division IDs, but Year {year.yearNumber} has no Divisions."
+            )
+        elif len(allUniqueTeamDivisionIds) == 0:
+            # some divisions, no team division ids
+            raise InvalidYearFormatException(
+                f"Year {year.yearNumber} has Divisions, but Teams in Year {year.yearNumber} have Division IDs."
+            )
+        elif len(allUniqueDivisionIds) > len(allUniqueTeamDivisionIds):
+            # some divisions, some team division ids, more divisions than division team ids
+            raise InvalidYearFormatException(
+                f"There are Divisions in Year {year.yearNumber} that do not belong to any Team."
+            )
+        elif len(allUniqueDivisionIds) < len(allUniqueTeamDivisionIds):
+            # some divisions, some team division ids, more division team ids than divisions
+            raise InvalidYearFormatException(
+                f"There are Teams with Division IDs in Year {year.yearNumber} that do not belong to any Division."
+            )
+        else:
+            # same number of divisions and team division ids, they do not match
+            raise InvalidYearFormatException(
+                f"The Divisions in Year {year.yearNumber} do not corrospond correctly to the Team Division IDs in Year {year.yearNumber}."
+            )
+
+
+def checkDivisionsHaveNoDuplicateIds(year: Year):
+    """
+    Checks that all divisions have a unique ID.
+    """
+    allDivisionIds = [division.id for division in year.divisions]
+
+    if len(set(allDivisionIds)) != len(allDivisionIds):
+        raise InvalidYearFormatException(f"Year {year.yearNumber} has duplicate division IDs.")
```

### Comparing `leeger-2.4.0/leeger.egg-info/PKG-INFO` & `leeger-2.5.0/leeger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: leeger
-Version: 2.4.0
-Summary: Instant stats for your fantasy football league.
+Version: 2.5.0
+Summary: Instant stats for any fantasy football league.
 Home-page: https://github.com/joeyagreco/leeger
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: nfl statistics stats football espn yahoo sleeper myfantasyleague,fleaflicker
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -124,14 +124,15 @@
 // @formatter:on
 -->
 
 **Answer:**
 This error occurs when the Python version you are using is not 3.10 or greater.\
 Make sure you are using Python version 3.10 or a newer version.
 
+___
 **Q:**
 How do I use this library to pull stats from my online fantasy league?
 
 **A:**
 
 1. Find your fantasy site [here](https://github.com/joeyagreco/leeger#supported-league-loaders) and ensure you have
    everything you need for the site you are using
@@ -189,35 +190,35 @@
 -->
 
 ## Stats Explained
 
 Stats used in this library are
 documented [here](https://github.com/joeyagreco/leeger/blob/main/doc/stats.md).
 
-## Running Tests
-
-To run tests, run the following command:
-
-```bash
-  pytest
-```
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 ## Development
 
-### Formatting
+_Run these commands from the root folder_
+- Format Code: `./main fmt`
+- Run Unit Tests: `./main test`
+- Generate Coverage Report: `./main cov`
+
+### Running Tests
+
+Run the following command from the root folder:
+
+```bash
+  pytest
+```
 
-_Run these commands from the root folder (leeger) before committing._\
-**General Format:** `black --config=pyproject.toml . `\
-**Import/Variable Format:** `autoflake --config=pyproject.toml .`
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 ## Credit
```

### Comparing `leeger-2.4.0/leeger.egg-info/SOURCES.txt` & `leeger-2.5.0/leeger.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 leeger/calculator/year_calculator/TeamSummaryYearCalculator.py
 leeger/calculator/year_calculator/__init__.py
 leeger/decorator/__init__.py
 leeger/decorator/validators.py
 leeger/enum/MatchupType.py
 leeger/enum/__init__.py
 leeger/exception/DoesNotExistException.py
+leeger/exception/InvalidDivisionFormatException.py
 leeger/exception/InvalidFilterException.py
 leeger/exception/InvalidLeagueFormatException.py
 leeger/exception/InvalidMatchupFormatException.py
 leeger/exception/InvalidOwnerFormatException.py
 leeger/exception/InvalidTeamFormatException.py
 leeger/exception/InvalidWeekFormatException.py
 leeger/exception/InvalidYearFormatException.py
@@ -57,50 +58,55 @@
 leeger/league_loader/FleaflickerLeagueLoader.py
 leeger/league_loader/LeagueLoader.py
 leeger/league_loader/MyFantasyLeagueLeagueLoader.py
 leeger/league_loader/SleeperLeagueLoader.py
 leeger/league_loader/YahooLeagueLoader.py
 leeger/league_loader/__init__.py
 leeger/model/__init__.py
+leeger/model/abstract/EqualityCheck.py
 leeger/model/abstract/UniqueId.py
 leeger/model/abstract/__init__.py
 leeger/model/filter/AllTimeFilters.py
 leeger/model/filter/WeekFilters.py
 leeger/model/filter/YearFilters.py
 leeger/model/filter/__init__.py
+leeger/model/league/Division.py
 leeger/model/league/League.py
 leeger/model/league/Matchup.py
 leeger/model/league/Owner.py
 leeger/model/league/Team.py
 leeger/model/league/Week.py
 leeger/model/league/Year.py
 leeger/model/league/YearSettings.py
 leeger/model/league/__init__.py
 leeger/model/league_helper/Performance.py
 leeger/model/league_helper/__init__.py
 leeger/model/stat/AllTimeStatSheet.py
 leeger/model/stat/YearStatSheet.py
 leeger/model/stat/__init__.py
+leeger/util/ConfigReader.py
 leeger/util/CustomFormatter.py
 leeger/util/CustomLogger.py
 leeger/util/Deci.py
 leeger/util/GeneralUtil.py
 leeger/util/IdGenerator.py
 leeger/util/JSONDeserializable.py
 leeger/util/JSONSerializable.py
 leeger/util/__init__.py
+leeger/util/equality.py
 leeger/util/excel.py
 leeger/util/excel_helper.py
 leeger/util/stat_sheet.py
 leeger/util/navigator/LeagueNavigator.py
 leeger/util/navigator/MatchupNavigator.py
 leeger/util/navigator/WeekNavigator.py
 leeger/util/navigator/YearNavigator.py
 leeger/util/navigator/__init__.py
 leeger/validate/__init__.py
+leeger/validate/divisionValidation.py
 leeger/validate/leagueValidation.py
 leeger/validate/matchupValidation.py
 leeger/validate/ownerValidation.py
 leeger/validate/teamValidation.py
 leeger/validate/weekValidation.py
 leeger/validate/yearSettingsValidation.py
 leeger/validate/yearValidation.py
@@ -138,36 +144,39 @@
 test/test_league_loader/test_YahooLeagueLoader.py
 test/test_model/__init__.py
 test/test_model/test_abstract/__init__.py
 test/test_model/test_abstract/test_UniqueId.py
 test/test_model/test_filter/__init__.py
 test/test_model/test_filter/test_AllTimeFilters.py
 test/test_model/test_league/__init__.py
+test/test_model/test_league/test_Division.py
 test/test_model/test_league/test_League.py
 test/test_model/test_league/test_Matchup.py
 test/test_model/test_league/test_Owner.py
 test/test_model/test_league/test_Team.py
 test/test_model/test_league/test_Week.py
 test/test_model/test_league/test_Year.py
 test/test_model/test_league/test_YearSettings.py
 test/test_model/test_league_helper/__init__.py
 test/test_model/test_league_helper/test_Performance.py
 test/test_util/__init__.py
 test/test_util/test_Deci.py
 test/test_util/test_GeneralUtil.py
 test/test_util/test_IdGenerator.py
+test/test_util/test_equality.py
 test/test_util/test_excel.py
 test/test_util/test_excel_helper.py
 test/test_util/test_stat_sheet.py
 test/test_util/test_navigator/__init__.py
 test/test_util/test_navigator/test_LeagueNavigator.py
 test/test_util/test_navigator/test_MatchupNavigator.py
 test/test_util/test_navigator/test_WeekNavigator.py
 test/test_util/test_navigator/test_YearNavigator.py
 test/test_validate/__init__.py
+test/test_validate/test_divisionValidation.py
 test/test_validate/test_leagueValidation.py
 test/test_validate/test_matchupValidation.py
 test/test_validate/test_ownerValidation.py
 test/test_validate/test_teamValidation.py
 test/test_validate/test_weekValidation.py
 test/test_validate/test_yearSettingsValidation.py
 test/test_validate/test_yearValidation.py
```

### Comparing `leeger-2.4.0/setup.py` & `leeger-2.5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     readme = f.read()
 
 setuptools.setup(
     name="leeger",
     version=package_version,
     author="Joey Greco",
     author_email="joeyagreco@gmail.com",
-    description="Instant stats for your fantasy football league.",
+    description="Instant stats for any fantasy football league.",
     long_description_content_type="text/markdown",
     long_description=readme,
     license="MIT",
     url="https://github.com/joeyagreco/leeger",
     packages=setuptools.find_packages(exclude=("test", "doc", "example", "img", ".github")),
     install_requires=required_packages,
     python_requires=f">={minimum_python_version_required}",
```

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_AWALAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_GameOutcomeAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_PlusMinusAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_PointsScoredAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_SSLAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_ScoringShareAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_ScoringStandardDeviationAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_SingleScoreAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_SmartWinsAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py` & `leeger-2.5.0/test/test_calculator/test_all_time_calculator/test_TeamSummaryAllTimeCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_AWALYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_GameOutcomeYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_PlusMinusYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_PointsScoredYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_SSLYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_ScoringShareYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_ScoringStandardDeviationYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_SingleScoreYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_SmartWinsYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py` & `leeger-2.5.0/test/test_calculator/test_year_calculator/test_TeamSummaryYearCalculator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_decorator/test_validators.py` & `leeger-2.5.0/test/test_decorator/test_validators.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_league_loader/test_LeagueLoader.py` & `leeger-2.5.0/test/test_league_loader/test_LeagueLoader.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py` & `leeger-2.5.0/test/test_league_loader/test_MyFantasyLeagueLeagueLoader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
 from unittest import mock
 import copy
 from leeger.enum.MatchupType import MatchupType
 
 from leeger.league_loader import MyFantasyLeagueLeagueLoader
+from leeger.model.league.Division import Division
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 
@@ -21,50 +22,50 @@
         dupMockFranchise["result"] = result
         return dupMockFranchise
 
     @mock.patch("pymfl.api.config.APIConfig.add_config_for_year_and_league_id")
     @mock.patch("pymfl.api.CommonLeagueInfoAPIClient.get_league")
     @mock.patch("pymfl.api.CommonLeagueInfoAPIClient.get_schedule")
     @mock.patch("pymfl.api.CommonLeagueInfoAPIClient.get_playoff_bracket")
-    def test_loadLeague_happyPath_noOwnerNamesAndAliases(
+    def test_loadLeague_happyPath(
         self, mockGetPlayoffBracket, mockGetSchedule, mockGetLeague, mockAddConfig
     ):
         """
         NOTE: This also tests the following cases:
             - having 1 playoff round in a year (dict)
             - having multiple playoff rounds in a year (list)
             - having 1 playoff matchup in a playoff week (dict)
             - having multiple playoff matchups in a playoff week (list)
         """
-        mockFranchise1_2022 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1}
-        mockFranchise2_2022 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2}
-        mockFranchise3_2022 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3}
-        mockFranchise4_2022 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4}
-        mockFranchise5_2022 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5}
-        mockFranchise6_2022 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6}
-        mockFranchise7_2022 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7}
-        mockFranchise8_2022 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8}
-
-        mockFranchise1_2023 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1}
-        mockFranchise2_2023 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2}
-        mockFranchise3_2023 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3}
-        mockFranchise4_2023 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4}
-        mockFranchise5_2023 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5}
-        mockFranchise6_2023 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6}
-        mockFranchise7_2023 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7}
-        mockFranchise8_2023 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8}
-
-        mockFranchise1_2024 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1}
-        mockFranchise2_2024 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2}
-        mockFranchise3_2024 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3}
-        mockFranchise4_2024 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4}
-        mockFranchise5_2024 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5}
-        mockFranchise6_2024 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6}
-        mockFranchise7_2024 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7}
-        mockFranchise8_2024 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8}
+        mockFranchise1_2022 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1, "division": "1"}
+        mockFranchise2_2022 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2, "division": "1"}
+        mockFranchise3_2022 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3, "division": "1"}
+        mockFranchise4_2022 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4, "division": "1"}
+        mockFranchise5_2022 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5, "division": "2"}
+        mockFranchise6_2022 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6, "division": "2"}
+        mockFranchise7_2022 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7, "division": "2"}
+        mockFranchise8_2022 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8, "division": "2"}
+
+        mockFranchise1_2023 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1, "division": "1"}
+        mockFranchise2_2023 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2, "division": "1"}
+        mockFranchise3_2023 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3, "division": "1"}
+        mockFranchise4_2023 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4, "division": "1"}
+        mockFranchise5_2023 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5, "division": "2"}
+        mockFranchise6_2023 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6, "division": "2"}
+        mockFranchise7_2023 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7, "division": "2"}
+        mockFranchise8_2023 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8, "division": "2"}
+
+        mockFranchise1_2024 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1, "division": "1"}
+        mockFranchise2_2024 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2, "division": "1"}
+        mockFranchise3_2024 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3, "division": "1"}
+        mockFranchise4_2024 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4, "division": "1"}
+        mockFranchise5_2024 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5, "division": "2"}
+        mockFranchise6_2024 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6, "division": "2"}
+        mockFranchise7_2024 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7, "division": "2"}
+        mockFranchise8_2024 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8, "division": "2"}
 
         mockLeague2022 = {
             "league": {
                 "id": 123,
                 "name": "Test League 2022",
                 "lastRegularSeasonWeek": "1",
                 "franchises": {
@@ -75,14 +76,17 @@
                         mockFranchise4_2022,
                         mockFranchise5_2022,
                         mockFranchise6_2022,
                         mockFranchise7_2022,
                         mockFranchise8_2022,
                     ]
                 },
+                "divisions": {
+                    "division": [{"id": "1", "name": "d1_2022"}, {"id": "2", "name": "d2_2022"}]
+                },
             }
         }
 
         mockLeague2023 = {
             "league": {
                 "id": 456,
                 "name": "Test League 2023",
@@ -95,14 +99,17 @@
                         mockFranchise4_2023,
                         mockFranchise5_2023,
                         mockFranchise6_2023,
                         mockFranchise7_2023,
                         mockFranchise8_2023,
                     ]
                 },
+                "divisions": {
+                    "division": [{"id": "1", "name": "d1_2023"}, {"id": "2", "name": "d2_2023"}]
+                },
             }
         }
 
         mockLeague2024 = {
             "league": {
                 "id": 789,
                 "name": "Test League 2024",
@@ -115,14 +122,17 @@
                         mockFranchise4_2024,
                         mockFranchise5_2024,
                         mockFranchise6_2024,
                         mockFranchise7_2024,
                         mockFranchise8_2024,
                     ]
                 },
+                "divisions": {
+                    "division": [{"id": "1", "name": "d1_2024"}, {"id": "2", "name": "d2_2024"}]
+                },
             }
         }
 
         mockSchedule2022 = {
             "schedule": {
                 "weeklySchedule": [
                     {
@@ -438,53 +448,63 @@
             mflUsername="mflu",
             mflPassword="mflp",
             mflUserAgentName="mfluan",
         )
         league = leagueLoader.loadLeague()
 
         # expected league
-        team1_2022 = Team(ownerId=1, name="Team 1")
-        team2_2022 = Team(ownerId=2, name="Team 2")
-        team3_2022 = Team(ownerId=3, name="Team 3")
-        team4_2022 = Team(ownerId=4, name="Team 4")
-        team5_2022 = Team(ownerId=5, name="Team 5")
-        team6_2022 = Team(ownerId=6, name="Team 6")
-        team7_2022 = Team(ownerId=7, name="Team 7")
-        team8_2022 = Team(ownerId=8, name="Team 8")
-
-        team1_2023 = Team(ownerId=1, name="Team 1")
-        team2_2023 = Team(ownerId=2, name="Team 2")
-        team3_2023 = Team(ownerId=3, name="Team 3")
-        team4_2023 = Team(ownerId=4, name="Team 4")
-        team5_2023 = Team(ownerId=5, name="Team 5")
-        team6_2023 = Team(ownerId=6, name="Team 6")
-        team7_2023 = Team(ownerId=7, name="Team 7")
-        team8_2023 = Team(ownerId=8, name="Team 8")
-
-        team1_2024 = Team(ownerId=1, name="Team 1")
-        team2_2024 = Team(ownerId=2, name="Team 2")
-        team3_2024 = Team(ownerId=3, name="Team 3")
-        team4_2024 = Team(ownerId=4, name="Team 4")
-        team5_2024 = Team(ownerId=5, name="Team 5")
-        team6_2024 = Team(ownerId=6, name="Team 6")
-        team7_2024 = Team(ownerId=7, name="Team 7")
-        team8_2024 = Team(ownerId=8, name="Team 8")
+
+        division1_2022 = Division(name="d1_2022")
+        division2_2022 = Division(name="d2_2022")
+
+        division1_2023 = Division(name="d1_2023")
+        division2_2023 = Division(name="d2_2023")
+
+        division1_2024 = Division(name="d1_2024")
+        division2_2024 = Division(name="d2_2024")
+
+        owner1 = Owner(name="Owner 1")
+        owner2 = Owner(name="Owner 2")
+        owner3 = Owner(name="Owner 3")
+        owner4 = Owner(name="Owner 4")
+        owner5 = Owner(name="Owner 5")
+        owner6 = Owner(name="Owner 6")
+        owner7 = Owner(name="Owner 7")
+        owner8 = Owner(name="Owner 8")
+
+        team1_2022 = Team(ownerId=owner1.id, name="Team 1", divisionId=division1_2022.id)
+        team2_2022 = Team(ownerId=owner2.id, name="Team 2", divisionId=division1_2022.id)
+        team3_2022 = Team(ownerId=owner3.id, name="Team 3", divisionId=division1_2022.id)
+        team4_2022 = Team(ownerId=owner4.id, name="Team 4", divisionId=division1_2022.id)
+        team5_2022 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2022.id)
+        team6_2022 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2022.id)
+        team7_2022 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2022.id)
+        team8_2022 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2022.id)
+
+        team1_2023 = Team(ownerId=owner1.id, name="Team 1", divisionId=division1_2023.id)
+        team2_2023 = Team(ownerId=owner2.id, name="Team 2", divisionId=division1_2023.id)
+        team3_2023 = Team(ownerId=owner3.id, name="Team 3", divisionId=division1_2023.id)
+        team4_2023 = Team(ownerId=owner4.id, name="Team 4", divisionId=division1_2023.id)
+        team5_2023 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2023.id)
+        team6_2023 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2023.id)
+        team7_2023 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2023.id)
+        team8_2023 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2023.id)
+
+        team1_2024 = Team(ownerId=owner1.id, name="Team 1", divisionId=division1_2024.id)
+        team2_2024 = Team(ownerId=owner2.id, name="Team 2", divisionId=division1_2024.id)
+        team3_2024 = Team(ownerId=owner3.id, name="Team 3", divisionId=division1_2024.id)
+        team4_2024 = Team(ownerId=owner4.id, name="Team 4", divisionId=division1_2024.id)
+        team5_2024 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2024.id)
+        team6_2024 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2024.id)
+        team7_2024 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2024.id)
+        team8_2024 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2024.id)
 
         expectedLeague = League(
             name="Test League 2024",
-            owners=[
-                Owner(name="Owner 1"),
-                Owner(name="Owner 2"),
-                Owner(name="Owner 3"),
-                Owner(name="Owner 4"),
-                Owner(name="Owner 5"),
-                Owner(name="Owner 6"),
-                Owner(name="Owner 7"),
-                Owner(name="Owner 8"),
-            ],
+            owners=[owner1, owner2, owner3, owner4, owner5, owner6, owner7, owner8],
             years=[
                 Year(
                     yearNumber=2022,
                     teams=[
                         team1_2022,
                         team2_2022,
                         team3_2022,
@@ -562,14 +582,15 @@
                                     teamAHasTiebreaker=True,
                                     teamBHasTiebreaker=False,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2022, division2_2022],
                 ),
                 Year(
                     yearNumber=2023,
                     teams=[
                         team1_2023,
                         team2_2023,
                         team3_2023,
@@ -670,14 +691,15 @@
                                     teamAHasTiebreaker=True,
                                     teamBHasTiebreaker=False,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2023, division2_2023],
                 ),
                 Year(
                     yearNumber=2024,
                     teams=[
                         team1_2024,
                         team2_2024,
                         team3_2024,
@@ -741,19 +763,20 @@
                                     teamAHasTiebreaker=True,
                                     teamBHasTiebreaker=False,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2024, division2_2024],
                 ),
             ],
         )
 
-        self.assertEqual(league, expectedLeague)
+        self.assertTrue(league.equals(expectedLeague, ignoreBaseIds=True, ignoreIds=True))
         # check multiWeekMatchupIds
         for year in league.years:
             for week in year.weeks:
                 for matchup in week.matchups:
                     self.assertIsNone(matchup.multiWeekMatchupId)
 
     @mock.patch("pymfl.api.config.APIConfig.add_config_for_year_and_league_id")
@@ -766,40 +789,40 @@
         """
         NOTE: This also tests the following cases:
             - having 1 playoff round in a year (dict)
             - having multiple playoff rounds in a year (list)
             - having 1 playoff matchup in a playoff week (dict)
             - having multiple playoff matchups in a playoff week (list)
         """
-        mockFranchise1_2022 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1}
-        mockFranchise2_2022 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2}
-        mockFranchise3_2022 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3}
-        mockFranchise4_2022 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4}
-        mockFranchise5_2022 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5}
-        mockFranchise6_2022 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6}
-        mockFranchise7_2022 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7}
-        mockFranchise8_2022 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8}
-
-        mockFranchise1_2023 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1}
-        mockFranchise2_2023 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2}
-        mockFranchise3_2023 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3}
-        mockFranchise4_2023 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4}
-        mockFranchise5_2023 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5}
-        mockFranchise6_2023 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6}
-        mockFranchise7_2023 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7}
-        mockFranchise8_2023 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8}
-
-        mockFranchise1_2024 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1}
-        mockFranchise2_2024 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2}
-        mockFranchise3_2024 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3}
-        mockFranchise4_2024 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4}
-        mockFranchise5_2024 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5}
-        mockFranchise6_2024 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6}
-        mockFranchise7_2024 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7}
-        mockFranchise8_2024 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8}
+        mockFranchise1_2022 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1, "division": "1"}
+        mockFranchise2_2022 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2, "division": "1"}
+        mockFranchise3_2022 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3, "division": "1"}
+        mockFranchise4_2022 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4, "division": "1"}
+        mockFranchise5_2022 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5, "division": "2"}
+        mockFranchise6_2022 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6, "division": "2"}
+        mockFranchise7_2022 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7, "division": "2"}
+        mockFranchise8_2022 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8, "division": "2"}
+
+        mockFranchise1_2023 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1, "division": "1"}
+        mockFranchise2_2023 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2, "division": "1"}
+        mockFranchise3_2023 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3, "division": "1"}
+        mockFranchise4_2023 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4, "division": "1"}
+        mockFranchise5_2023 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5, "division": "2"}
+        mockFranchise6_2023 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6, "division": "2"}
+        mockFranchise7_2023 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7, "division": "2"}
+        mockFranchise8_2023 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8, "division": "2"}
+
+        mockFranchise1_2024 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1, "division": "1"}
+        mockFranchise2_2024 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2, "division": "1"}
+        mockFranchise3_2024 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3, "division": "1"}
+        mockFranchise4_2024 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4, "division": "1"}
+        mockFranchise5_2024 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5, "division": "2"}
+        mockFranchise6_2024 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6, "division": "2"}
+        mockFranchise7_2024 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7, "division": "2"}
+        mockFranchise8_2024 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8, "division": "2"}
 
         mockLeague2022 = {
             "league": {
                 "id": 123,
                 "name": "Test League 2022",
                 "lastRegularSeasonWeek": "1",
                 "franchises": {
@@ -810,14 +833,17 @@
                         mockFranchise4_2022,
                         mockFranchise5_2022,
                         mockFranchise6_2022,
                         mockFranchise7_2022,
                         mockFranchise8_2022,
                     ]
                 },
+                "divisions": {
+                    "division": [{"id": "1", "name": "d1_2022"}, {"id": "2", "name": "d2_2022"}]
+                },
             }
         }
 
         mockLeague2023 = {
             "league": {
                 "id": 456,
                 "name": "Test League 2023",
@@ -830,14 +856,17 @@
                         mockFranchise4_2023,
                         mockFranchise5_2023,
                         mockFranchise6_2023,
                         mockFranchise7_2023,
                         mockFranchise8_2023,
                     ]
                 },
+                "divisions": {
+                    "division": [{"id": "1", "name": "d1_2023"}, {"id": "2", "name": "d2_2023"}]
+                },
             }
         }
 
         mockLeague2024 = {
             "league": {
                 "id": 789,
                 "name": "Test League 2024",
@@ -850,14 +879,17 @@
                         mockFranchise4_2024,
                         mockFranchise5_2024,
                         mockFranchise6_2024,
                         mockFranchise7_2024,
                         mockFranchise8_2024,
                     ]
                 },
+                "divisions": {
+                    "division": [{"id": "1", "name": "d1_2024"}, {"id": "2", "name": "d2_2024"}]
+                },
             }
         }
 
         mockSchedule2022 = {
             "schedule": {
                 "weeklySchedule": [
                     {
@@ -1183,53 +1215,63 @@
                 "o7": ["Owner 7"],
                 "o8": ["Owner 8"],
             },
         )
         league = leagueLoader.loadLeague()
 
         # expected league
-        team1_2022 = Team(ownerId=1, name="Team 1")
-        team2_2022 = Team(ownerId=2, name="Team 2")
-        team3_2022 = Team(ownerId=3, name="Team 3")
-        team4_2022 = Team(ownerId=4, name="Team 4")
-        team5_2022 = Team(ownerId=5, name="Team 5")
-        team6_2022 = Team(ownerId=6, name="Team 6")
-        team7_2022 = Team(ownerId=7, name="Team 7")
-        team8_2022 = Team(ownerId=8, name="Team 8")
-
-        team1_2023 = Team(ownerId=1, name="Team 1")
-        team2_2023 = Team(ownerId=2, name="Team 2")
-        team3_2023 = Team(ownerId=3, name="Team 3")
-        team4_2023 = Team(ownerId=4, name="Team 4")
-        team5_2023 = Team(ownerId=5, name="Team 5")
-        team6_2023 = Team(ownerId=6, name="Team 6")
-        team7_2023 = Team(ownerId=7, name="Team 7")
-        team8_2023 = Team(ownerId=8, name="Team 8")
-
-        team1_2024 = Team(ownerId=1, name="Team 1")
-        team2_2024 = Team(ownerId=2, name="Team 2")
-        team3_2024 = Team(ownerId=3, name="Team 3")
-        team4_2024 = Team(ownerId=4, name="Team 4")
-        team5_2024 = Team(ownerId=5, name="Team 5")
-        team6_2024 = Team(ownerId=6, name="Team 6")
-        team7_2024 = Team(ownerId=7, name="Team 7")
-        team8_2024 = Team(ownerId=8, name="Team 8")
+
+        division1_2022 = Division(name="d1_2022")
+        division2_2022 = Division(name="d2_2022")
+
+        division1_2023 = Division(name="d1_2023")
+        division2_2023 = Division(name="d2_2023")
+
+        division1_2024 = Division(name="d1_2024")
+        division2_2024 = Division(name="d2_2024")
+
+        owner1 = Owner(name="o1")
+        owner2 = Owner(name="o2")
+        owner3 = Owner(name="o3")
+        owner4 = Owner(name="o4")
+        owner5 = Owner(name="o5")
+        owner6 = Owner(name="o6")
+        owner7 = Owner(name="o7")
+        owner8 = Owner(name="o8")
+
+        team1_2022 = Team(ownerId=owner1.id, name="Team 1", divisionId=division1_2022.id)
+        team2_2022 = Team(ownerId=owner2.id, name="Team 2", divisionId=division1_2022.id)
+        team3_2022 = Team(ownerId=owner3.id, name="Team 3", divisionId=division1_2022.id)
+        team4_2022 = Team(ownerId=owner4.id, name="Team 4", divisionId=division1_2022.id)
+        team5_2022 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2022.id)
+        team6_2022 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2022.id)
+        team7_2022 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2022.id)
+        team8_2022 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2022.id)
+
+        team1_2023 = Team(ownerId=owner1.id, name="Team 1", divisionId=division1_2023.id)
+        team2_2023 = Team(ownerId=owner2.id, name="Team 2", divisionId=division1_2023.id)
+        team3_2023 = Team(ownerId=owner3.id, name="Team 3", divisionId=division1_2023.id)
+        team4_2023 = Team(ownerId=owner4.id, name="Team 4", divisionId=division1_2023.id)
+        team5_2023 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2023.id)
+        team6_2023 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2023.id)
+        team7_2023 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2023.id)
+        team8_2023 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2023.id)
+
+        team1_2024 = Team(ownerId=owner1.id, name="Team 1", divisionId=division1_2024.id)
+        team2_2024 = Team(ownerId=owner2.id, name="Team 2", divisionId=division1_2024.id)
+        team3_2024 = Team(ownerId=owner3.id, name="Team 3", divisionId=division1_2024.id)
+        team4_2024 = Team(ownerId=owner4.id, name="Team 4", divisionId=division1_2024.id)
+        team5_2024 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2024.id)
+        team6_2024 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2024.id)
+        team7_2024 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2024.id)
+        team8_2024 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2024.id)
 
         expectedLeague = League(
             name="Test League 2024",
-            owners=[
-                Owner(name="o1"),
-                Owner(name="o2"),
-                Owner(name="o3"),
-                Owner(name="o4"),
-                Owner(name="o5"),
-                Owner(name="o6"),
-                Owner(name="o7"),
-                Owner(name="o8"),
-            ],
+            owners=[owner1, owner2, owner3, owner4, owner5, owner6, owner7, owner8],
             years=[
                 Year(
                     yearNumber=2022,
                     teams=[
                         team1_2022,
                         team2_2022,
                         team3_2022,
@@ -1307,14 +1349,15 @@
                                     teamAHasTiebreaker=True,
                                     teamBHasTiebreaker=False,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2022, division2_2022],
                 ),
                 Year(
                     yearNumber=2023,
                     teams=[
                         team1_2023,
                         team2_2023,
                         team3_2023,
@@ -1415,14 +1458,15 @@
                                     teamAHasTiebreaker=True,
                                     teamBHasTiebreaker=False,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2023, division2_2023],
                 ),
                 Year(
                     yearNumber=2024,
                     teams=[
                         team1_2024,
                         team2_2024,
                         team3_2024,
@@ -1486,17 +1530,443 @@
                                     teamAHasTiebreaker=True,
                                     teamBHasTiebreaker=False,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2024, division2_2024],
                 ),
             ],
         )
 
-        self.assertEqual(league, expectedLeague)
+        self.assertTrue(league.equals(expectedLeague, ignoreBaseIds=True, ignoreIds=True))
         # check multiWeekMatchupIds
         for year in league.years:
             for week in year.weeks:
                 for matchup in week.matchups:
                     self.assertIsNone(matchup.multiWeekMatchupId)
+
+    @mock.patch("pymfl.api.config.APIConfig.add_config_for_year_and_league_id")
+    @mock.patch("pymfl.api.CommonLeagueInfoAPIClient.get_league")
+    @mock.patch("pymfl.api.CommonLeagueInfoAPIClient.get_schedule")
+    @mock.patch("pymfl.api.CommonLeagueInfoAPIClient.get_playoff_bracket")
+    def test_loadLeague_withLeagueName(
+        self, mockGetPlayoffBracket, mockGetSchedule, mockGetLeague, mockAddConfig
+    ):
+        mockFranchise1_2022 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1, "division": "1"}
+        mockFranchise2_2022 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2, "division": "1"}
+        mockFranchise3_2022 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3, "division": "1"}
+        mockFranchise4_2022 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4, "division": "1"}
+        mockFranchise5_2022 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5, "division": "2"}
+        mockFranchise6_2022 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6, "division": "2"}
+        mockFranchise7_2022 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7, "division": "2"}
+        mockFranchise8_2022 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8, "division": "2"}
+
+        mockFranchise1_2023 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1, "division": "1"}
+        mockFranchise2_2023 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2, "division": "1"}
+        mockFranchise3_2023 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3, "division": "1"}
+        mockFranchise4_2023 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4, "division": "1"}
+        mockFranchise5_2023 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5, "division": "2"}
+        mockFranchise6_2023 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6, "division": "2"}
+        mockFranchise7_2023 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7, "division": "2"}
+        mockFranchise8_2023 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8, "division": "2"}
+
+        mockFranchise1_2024 = {"owner_name": "Owner 1", "name": "Team 1", "id": 1, "division": "1"}
+        mockFranchise2_2024 = {"owner_name": "Owner 2", "name": "Team 2", "id": 2, "division": "1"}
+        mockFranchise3_2024 = {"owner_name": "Owner 3", "name": "Team 3", "id": 3, "division": "1"}
+        mockFranchise4_2024 = {"owner_name": "Owner 4", "name": "Team 4", "id": 4, "division": "1"}
+        mockFranchise5_2024 = {"owner_name": "Owner 5", "name": "Team 5", "id": 5, "division": "2"}
+        mockFranchise6_2024 = {"owner_name": "Owner 6", "name": "Team 6", "id": 6, "division": "2"}
+        mockFranchise7_2024 = {"owner_name": "Owner 7", "name": "Team 7", "id": 7, "division": "2"}
+        mockFranchise8_2024 = {"owner_name": "Owner 8", "name": "Team 8", "id": 8, "division": "2"}
+
+        mockLeague2022 = {
+            "league": {
+                "id": 123,
+                "name": "Test League 2022",
+                "lastRegularSeasonWeek": "1",
+                "franchises": {
+                    "franchise": [
+                        mockFranchise1_2022,
+                        mockFranchise2_2022,
+                        mockFranchise3_2022,
+                        mockFranchise4_2022,
+                        mockFranchise5_2022,
+                        mockFranchise6_2022,
+                        mockFranchise7_2022,
+                        mockFranchise8_2022,
+                    ]
+                },
+                "divisions": {
+                    "division": [{"id": "1", "name": "d1_2022"}, {"id": "2", "name": "d2_2022"}]
+                },
+            }
+        }
+
+        mockLeague2023 = {
+            "league": {
+                "id": 456,
+                "name": "Test League 2023",
+                "lastRegularSeasonWeek": "1",
+                "franchises": {
+                    "franchise": [
+                        mockFranchise1_2023,
+                        mockFranchise2_2023,
+                        mockFranchise3_2023,
+                        mockFranchise4_2023,
+                        mockFranchise5_2023,
+                        mockFranchise6_2023,
+                        mockFranchise7_2023,
+                        mockFranchise8_2023,
+                    ]
+                },
+                "divisions": {
+                    "division": [{"id": "1", "name": "d1_2023"}, {"id": "2", "name": "d2_2023"}]
+                },
+            }
+        }
+
+        mockLeague2024 = {
+            "league": {
+                "id": 789,
+                "name": "Test League 2024",
+                "lastRegularSeasonWeek": "1",
+                "franchises": {
+                    "franchise": [
+                        mockFranchise1_2024,
+                        mockFranchise2_2024,
+                        mockFranchise3_2024,
+                        mockFranchise4_2024,
+                        mockFranchise5_2024,
+                        mockFranchise6_2024,
+                        mockFranchise7_2024,
+                        mockFranchise8_2024,
+                    ]
+                },
+                "divisions": {
+                    "division": [{"id": "1", "name": "d1_2024"}, {"id": "2", "name": "d2_2024"}]
+                },
+            }
+        }
+
+        mockSchedule2022 = {
+            "schedule": {
+                "weeklySchedule": [
+                    {
+                        "week": "1",
+                        "matchup": [
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise1_2022, score=100, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise2_2022, score=100, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise3_2022, score=100.1, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise4_2022, score=90.1, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise5_2022, score=101, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise6_2022, score=91, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise7_2022, score=102, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise8_2022, score=92, result="L"
+                                    ),
+                                ]
+                            },
+                        ],
+                    },
+                    {
+                        "week": "2",
+                        "matchup": [
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise2_2022, score=103, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise3_2022, score=93, result="L"
+                                    ),
+                                ]
+                            }
+                        ],
+                    },
+                    {
+                        "week": "3",
+                        "matchup": [
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise1_2022, score=104, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise2_2022, score=94, result="L"
+                                    ),
+                                ]
+                            }
+                        ],
+                    },
+                ]
+            }
+        }
+
+        mockSchedule2023 = {
+            "schedule": {
+                "weeklySchedule": [
+                    {
+                        "week": "1",
+                        "matchup": [
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise1_2023, score=100, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise2_2023, score=100, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise3_2023, score=100.1, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise4_2023, score=90.1, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise5_2023, score=101, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise6_2023, score=91, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise7_2023, score=102, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise8_2023, score=92, result="L"
+                                    ),
+                                ]
+                            },
+                        ],
+                    },
+                    {
+                        "week": "2",
+                        "matchup": [
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise2_2023, score=103, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise3_2023, score=93, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise4_2023, score=103, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise5_2023, score=93, result="L"
+                                    ),
+                                ]
+                            },
+                        ],
+                    },
+                    {
+                        "week": "3",
+                        "matchup": [
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise2_2023, score=104, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise3_2023, score=94, result="L"
+                                    ),
+                                ]
+                            }
+                        ],
+                    },
+                    {
+                        "week": "4",
+                        "matchup": [
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise1_2023, score=104, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise2_2023, score=94, result="L"
+                                    ),
+                                ]
+                            }
+                        ],
+                    },
+                ]
+            }
+        }
+
+        mockSchedule2024 = {
+            "schedule": {
+                "weeklySchedule": [
+                    {
+                        "week": "1",
+                        "matchup": [
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise1_2022, score=100, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise2_2022, score=100, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise3_2022, score=100.1, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise4_2022, score=90.1, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise5_2022, score=101, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise6_2022, score=91, result="L"
+                                    ),
+                                ]
+                            },
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise7_2022, score=102, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise8_2022, score=92, result="L"
+                                    ),
+                                ]
+                            },
+                        ],
+                    },
+                    {
+                        "week": "2",
+                        "matchup": [
+                            {
+                                "franchise": [
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise1_2022, score=103, result="W"
+                                    ),
+                                    self.__addScoreToMockFranchise(
+                                        mockFranchise=mockFranchise2_2022, score=93, result="L"
+                                    ),
+                                ]
+                            }
+                        ],
+                    },
+                ]
+            }
+        }
+
+        mockPlayoffSchedule_2022 = {
+            "playoffBracket": {
+                "playoffRound": [
+                    {
+                        "week": 2,
+                        "playoffGame": {"away": {"franchise_id": 2}, "home": {"franchise_id": 3}},
+                    },
+                    {
+                        "week": 3,
+                        "playoffGame": {"away": {"franchise_id": 1}, "home": {"franchise_id": 2}},
+                    },
+                ]
+            }
+        }
+
+        mockPlayoffSchedule_2023 = {
+            "playoffBracket": {
+                "playoffRound": [
+                    {
+                        "week": 2,
+                        "playoffGame": [
+                            {"away": {"franchise_id": 2}, "home": {"franchise_id": 3}},
+                            {"away": {"franchise_id": 4}, "home": {"franchise_id": 5}},
+                        ],
+                    },
+                    {
+                        "week": 3,
+                        "playoffGame": {"away": {"franchise_id": 2}, "home": {"franchise_id": 4}},
+                    },
+                    {
+                        "week": 4,
+                        "playoffGame": {"away": {"franchise_id": 1}, "home": {"franchise_id": 2}},
+                    },
+                ]
+            }
+        }
+
+        mockPlayoffSchedule_2024 = {
+            "playoffBracket": {
+                "playoffRound": {
+                    "week": 2,
+                    "playoffGame": {"away": {"franchise_id": 1}, "home": {"franchise_id": 2}},
+                }
+            }
+        }
+
+        mockGetLeague.side_effect = [mockLeague2022, mockLeague2023, mockLeague2024]
+        mockGetSchedule.side_effect = [mockSchedule2022, mockSchedule2023, mockSchedule2024]
+        mockGetPlayoffBracket.side_effect = [
+            mockPlayoffSchedule_2022,
+            mockPlayoffSchedule_2023,
+            mockPlayoffSchedule_2024,
+        ]
+
+        leagueLoader = MyFantasyLeagueLeagueLoader(
+            "789",
+            [2022, 2023, 2024],
+            mflUsername="mflu",
+            mflPassword="mflp",
+            mflUserAgentName="mfluan",
+            leagueName="custom name",
+        )
+        league = leagueLoader.loadLeague()
+
+        self.assertEqual("custom name", league.name)
```

### Comparing `leeger-2.4.0/test/test_league_loader/test_SleeperLeagueLoader.py` & `leeger-2.5.0/test/test_league_loader/test_SleeperLeagueLoader.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 from leeger.league_loader import SleeperLeagueLoader
 from unittest.mock import patch, Mock
 from sleeper.model import User as SleeperUser
 from sleeper.model import Roster as SleeperRoster
 from sleeper.model import Matchup as SleeperMatchup
 from sleeper.model import SportState as SleeperSportState
 from sleeper.model import PlayoffMatchup as SleeperPlayoffMatchup
+from sleeper.model import RosterSettings as SleeperRosterSettings
 from sleeper.enum import PlayoffRoundType as SleeperPlayoffRoundType
 from sleeper.enum import SeasonStatus as SleeperSeasonStatus
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
+from leeger.model.league.Division import Division
 
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from leeger.model.league.YearSettings import YearSettings
 
 
@@ -48,25 +50,43 @@
             summoner_region=None,
             token=None,
             user_id=userId,
             username=None,
             verification=None,
         )
 
-    def __generateMockSleeperRoster(self, *, ownerId: str, rosterId: str) -> SleeperRoster:
+    def __generateMockSleeperRoster(
+        self, *, ownerId: str, rosterId: str, division: int
+    ) -> SleeperRoster:
+        rosterSettings = SleeperRosterSettings(
+            division=division,
+            fpts=None,
+            fpts_against=None,
+            fpts_against_decimal=None,
+            fpts_decimal=None,
+            losses=None,
+            ppts=None,
+            ppts_decimal=None,
+            ties=None,
+            total_moves=None,
+            waiver_adjusted=None,
+            waiver_budget_used=None,
+            waiver_position=None,
+            wins=None,
+        )
         return SleeperRoster(
             co_owners=None,
             league_id=None,
             metadata=None,
             owner_id=ownerId,
             players=None,
             player_map=None,
             reserve=None,
             roster_id=rosterId,
-            settings=None,
+            settings=rosterSettings,
             starters=None,
             taxi=None,
         )
 
     def __generateMockSleeperMatchup(
         self, *, matchupId: int, rosterId: int, points: float
     ) -> SleeperMatchup:
@@ -153,45 +173,52 @@
 
     @patch("sleeper.api.LeagueAPIClient.get_league")
     @patch("sleeper.api.LeagueAPIClient.get_users_in_league")
     @patch("sleeper.api.LeagueAPIClient.get_rosters")
     @patch("sleeper.api.LeagueAPIClient.get_matchups_for_week")
     @patch("sleeper.api.LeagueAPIClient.get_sport_state")
     @patch("sleeper.api.LeagueAPIClient.get_winners_bracket")
-    def test_load_league_happyPath_noOwnerNamesAndAliases(
+    def test_load_league_happyPath(
         self,
         mockGetWinnersBracket,
         mockGetSportState,
         mockGetMatchupsForWeek,
         mockGetRosters,
         mockGetUsersInLeague,
         mockGetLeague,
     ):
         # create mock SleeperLeague objects
+
         mockSleeperLeague2022 = Mock()
         mockSleeperLeague2022.season = "2022"
         mockSleeperLeague2022.status = SleeperSeasonStatus.COMPLETE
         mockSleeperLeague2022.playoff_matchups = []
         mockSleeperLeague2022.name = "Test League 2022"
         mockSleeperLeague2022.settings.playoff_week_start = 3
         mockSleeperLeague2022.settings.league_average_match = 0
+        mockSleeperLeague2022.settings.divisions = 2
         mockSleeperLeague2022.settings.playoff_round_type_enum = (
             SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND
         )
+        mockSleeperLeague2022.metadata.division_1 = "d1_2022"
+        mockSleeperLeague2022.metadata.division_2 = "d2_2022"
 
         mockSleeperLeague2023 = Mock()
         mockSleeperLeague2023.season = "2023"
         mockSleeperLeague2023.status = SleeperSeasonStatus.IN_SEASON
         mockSleeperLeague2023.playoff_matchups = []
         mockSleeperLeague2023.name = "Test League 2023"
         mockSleeperLeague2023.settings.playoff_week_start = 3
         mockSleeperLeague2023.settings.league_average_match = 0
+        mockSleeperLeague2023.settings.divisions = 2
         mockSleeperLeague2023.settings.playoff_round_type_enum = (
             SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND
         )
+        mockSleeperLeague2023.metadata.division_1 = "d1_2023"
+        mockSleeperLeague2023.metadata.division_2 = "d2_2023"
 
         # create mock SleeperUser objects
         mockSleeperUsers2022 = [
             self.__generateMockSleeperUser(displayName="User 1", userId="1"),
             self.__generateMockSleeperUser(displayName="User 2", userId="2"),
             self.__generateMockSleeperUser(displayName="User 3", userId="3"),
             self.__generateMockSleeperUser(displayName="User 4", userId="4"),
@@ -227,33 +254,33 @@
                 displayName="User 8", userId="8", metadata={"team_name": "Team 8"}
             ),
         ]
 
         # create mock SleeperRoster objects
         # roster id will be YYYY (year) RR (roster number)
         mockSleeperRosters2022 = [
-            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201),
-            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202),
-            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203),
-            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204),
-            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205),
-            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206),
-            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207),
-            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208),
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202, division=1),
+            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203, division=1),
+            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204, division=1),
+            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205, division=2),
+            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206, division=2),
+            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207, division=2),
+            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208, division=2),
         ]
 
         mockSleeperRosters2023 = [
-            self.__generateMockSleeperRoster(ownerId="1", rosterId=202301),
-            self.__generateMockSleeperRoster(ownerId="2", rosterId=202302),
-            self.__generateMockSleeperRoster(ownerId="3", rosterId=202303),
-            self.__generateMockSleeperRoster(ownerId="4", rosterId=202304),
-            self.__generateMockSleeperRoster(ownerId="5", rosterId=202305),
-            self.__generateMockSleeperRoster(ownerId="6", rosterId=202306),
-            self.__generateMockSleeperRoster(ownerId="7", rosterId=202307),
-            self.__generateMockSleeperRoster(ownerId="8", rosterId=202308),
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202301, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202302, division=1),
+            self.__generateMockSleeperRoster(ownerId="3", rosterId=202303, division=1),
+            self.__generateMockSleeperRoster(ownerId="4", rosterId=202304, division=1),
+            self.__generateMockSleeperRoster(ownerId="5", rosterId=202305, division=2),
+            self.__generateMockSleeperRoster(ownerId="6", rosterId=202306, division=2),
+            self.__generateMockSleeperRoster(ownerId="7", rosterId=202307, division=2),
+            self.__generateMockSleeperRoster(ownerId="8", rosterId=202308, division=2),
         ]
 
         # create mock SleeperMatchup objects
         # matchup id will be YYYY (year) WW (week number) MM (matchup number)
         mockSleeperMatchups2022_1 = [
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202201, points=100),
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202202, points=100),
@@ -385,44 +412,51 @@
         ]
 
         # create instance of SleeperLeagueLoader and call load_league method
         sleeper_league_loader = SleeperLeagueLoader("123", [2022, 2023])
         league = sleeper_league_loader.loadLeague()
 
         # expected league
-        team1_2022 = Team(ownerId=1, name="User 1")
-        team2_2022 = Team(ownerId=2, name="User 2")
-        team3_2022 = Team(ownerId=3, name="User 3")
-        team4_2022 = Team(ownerId=4, name="User 4")
-        team5_2022 = Team(ownerId=5, name="Team 5")
-        team6_2022 = Team(ownerId=6, name="Team 6")
-        team7_2022 = Team(ownerId=7, name="Team 7")
-        team8_2022 = Team(ownerId=8, name="Team 8")
-
-        team1_2023 = Team(ownerId=1, name="User 1")
-        team2_2023 = Team(ownerId=2, name="User 2")
-        team3_2023 = Team(ownerId=3, name="User 3")
-        team4_2023 = Team(ownerId=4, name="User 4")
-        team5_2023 = Team(ownerId=5, name="Team 5")
-        team6_2023 = Team(ownerId=6, name="Team 6")
-        team7_2023 = Team(ownerId=7, name="Team 7")
-        team8_2023 = Team(ownerId=8, name="Team 8")
+
+        division1_2022 = Division(name="d1_2022")
+        division2_2022 = Division(name="d2_2022")
+
+        division1_2023 = Division(name="d1_2023")
+        division2_2023 = Division(name="d2_2023")
+
+        owner1 = Owner(name="User 1")
+        owner2 = Owner(name="User 2")
+        owner3 = Owner(name="User 3")
+        owner4 = Owner(name="User 4")
+        owner5 = Owner(name="User 5")
+        owner6 = Owner(name="User 6")
+        owner7 = Owner(name="User 7")
+        owner8 = Owner(name="User 8")
+
+        team1_2022 = Team(ownerId=owner1.id, name="User 1", divisionId=division1_2022.id)
+        team2_2022 = Team(ownerId=owner2.id, name="User 2", divisionId=division1_2022.id)
+        team3_2022 = Team(ownerId=owner3.id, name="User 3", divisionId=division1_2022.id)
+        team4_2022 = Team(ownerId=owner4.id, name="User 4", divisionId=division1_2022.id)
+        team5_2022 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2022.id)
+        team6_2022 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2022.id)
+        team7_2022 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2022.id)
+        team8_2022 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2022.id)
+
+        team1_2023 = Team(ownerId=owner1.id, name="User 1", divisionId=division1_2023.id)
+        team2_2023 = Team(ownerId=owner2.id, name="User 2", divisionId=division1_2023.id)
+        team3_2023 = Team(ownerId=owner3.id, name="User 3", divisionId=division1_2023.id)
+        team4_2023 = Team(ownerId=owner4.id, name="User 4", divisionId=division1_2023.id)
+        team5_2023 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2023.id)
+        team6_2023 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2023.id)
+        team7_2023 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2023.id)
+        team8_2023 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2023.id)
 
         expectedLeague = League(
             name="Test League 2023",
-            owners=[
-                Owner(name="User 1"),
-                Owner(name="User 2"),
-                Owner(name="User 3"),
-                Owner(name="User 4"),
-                Owner(name="User 5"),
-                Owner(name="User 6"),
-                Owner(name="User 7"),
-                Owner(name="User 8"),
-            ],
+            owners=[owner1, owner2, owner3, owner4, owner5, owner6, owner7, owner8],
             years=[
                 Year(
                     yearNumber=2022,
                     teams=[
                         team1_2022,
                         team2_2022,
                         team3_2022,
@@ -551,14 +585,15 @@
                                     teamBHasTiebreaker=False,
                                     multiWeekMatchupId=None,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2022, division2_2022],
                 ),
                 Year(
                     yearNumber=2023,
                     teams=[
                         team1_2023,
                         team2_2023,
                         team3_2023,
@@ -687,18 +722,19 @@
                                     teamBHasTiebreaker=False,
                                     multiWeekMatchupId=None,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2023, division2_2023],
                 ),
             ],
         )
-        self.assertEqual(league, expectedLeague)
+        self.assertTrue(league.equals(expectedLeague, ignoreBaseIds=True, ignoreIds=True))
         # check multiWeekMatchupIds
         for year in league.years:
             for week in year.weeks:
                 for matchup in week.matchups:
                     self.assertIsNone(matchup.multiWeekMatchupId)
 
     @patch("sleeper.api.LeagueAPIClient.get_league")
@@ -720,17 +756,20 @@
         mockSleeperLeague2022 = Mock()
         mockSleeperLeague2022.season = "2022"
         mockSleeperLeague2022.status = SleeperSeasonStatus.COMPLETE
         mockSleeperLeague2022.playoff_matchups = []
         mockSleeperLeague2022.name = "Test League 2022"
         mockSleeperLeague2022.settings.playoff_week_start = 3
         mockSleeperLeague2022.settings.league_average_match = 0
+        mockSleeperLeague2022.settings.divisions = 2
         mockSleeperLeague2022.settings.playoff_round_type_enum = (
             SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND
         )
+        mockSleeperLeague2022.metadata.division_1 = "d1_2022"
+        mockSleeperLeague2022.metadata.division_2 = "d2_2022"
 
         # create mock SleeperUser objects
         mockSleeperUsers2022 = [
             self.__generateMockSleeperUser(displayName="User 1", userId="1"),
             self.__generateMockSleeperUser(displayName="User 2", userId="2"),
             self.__generateMockSleeperUser(displayName="User 3", userId="3"),
             self.__generateMockSleeperUser(displayName="User 4", userId="4"),
@@ -747,22 +786,22 @@
                 displayName="User 8", userId="8", metadata={"team_name": "Team 8"}
             ),
         ]
 
         # create mock SleeperRoster objects
         # roster id will be YYYY (year) RR (roster number)
         mockSleeperRosters2022 = [
-            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201),
-            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202),
-            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203),
-            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204),
-            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205),
-            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206),
-            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207),
-            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208),
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202, division=1),
+            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203, division=1),
+            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204, division=1),
+            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205, division=2),
+            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206, division=2),
+            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207, division=2),
+            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208, division=2),
         ]
 
         # create mock SleeperMatchup objects
         # matchup id will be YYYY (year) WW (week number) MM (matchup number)
         mockSleeperMatchups2022_1 = [
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202201, points=100),
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202202, points=100),
@@ -846,35 +885,39 @@
                 "o7": ["User 7"],
                 "o8": ["User 8"],
             },
         )
         league = sleeper_league_loader.loadLeague()
 
         # expected league
-        team1_2022 = Team(ownerId=1, name="User 1")
-        team2_2022 = Team(ownerId=2, name="User 2")
-        team3_2022 = Team(ownerId=3, name="User 3")
-        team4_2022 = Team(ownerId=4, name="User 4")
-        team5_2022 = Team(ownerId=5, name="Team 5")
-        team6_2022 = Team(ownerId=6, name="Team 6")
-        team7_2022 = Team(ownerId=7, name="Team 7")
-        team8_2022 = Team(ownerId=8, name="Team 8")
+
+        owner1 = Owner(name="o1")
+        owner2 = Owner(name="o2")
+        owner3 = Owner(name="o3")
+        owner4 = Owner(name="o4")
+        owner5 = Owner(name="o5")
+        owner6 = Owner(name="o6")
+        owner7 = Owner(name="o7")
+        owner8 = Owner(name="o8")
+
+        division1_2022 = Division(name="d1_2022")
+        division2_2022 = Division(name="d2_2022")
+
+        team1_2022 = Team(ownerId=owner1.id, name="User 1")
+        team2_2022 = Team(ownerId=owner2.id, name="User 2")
+        team3_2022 = Team(ownerId=owner3.id, name="User 3")
+        team4_2022 = Team(ownerId=owner4.id, name="User 4")
+        team5_2022 = Team(ownerId=owner5.id, name="Team 5")
+        team6_2022 = Team(ownerId=owner6.id, name="Team 6")
+        team7_2022 = Team(ownerId=owner7.id, name="Team 7")
+        team8_2022 = Team(ownerId=owner8.id, name="Team 8")
 
         expectedLeague = League(
             name="Test League 2022",
-            owners=[
-                Owner(name="o1"),
-                Owner(name="o2"),
-                Owner(name="o3"),
-                Owner(name="o4"),
-                Owner(name="o5"),
-                Owner(name="o6"),
-                Owner(name="o7"),
-                Owner(name="o8"),
-            ],
+            owners=[owner1, owner2, owner3, owner4, owner5, owner6, owner7, owner8],
             years=[
                 Year(
                     yearNumber=2022,
                     teams=[
                         team1_2022,
                         team2_2022,
                         team3_2022,
@@ -1003,30 +1046,277 @@
                                     teamBHasTiebreaker=False,
                                     multiWeekMatchupId=None,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2022, division2_2022],
                 )
             ],
         )
-        self.assertEqual(league, expectedLeague)
+        self.assertTrue(league.equals(expectedLeague, ignoreBaseIds=True, ignoreIds=True))
         # check multiWeekMatchupIds
         for year in league.years:
             for week in year.weeks:
                 for matchup in week.matchups:
                     self.assertIsNone(matchup.multiWeekMatchupId)
 
     @patch("sleeper.api.LeagueAPIClient.get_league")
     @patch("sleeper.api.LeagueAPIClient.get_users_in_league")
     @patch("sleeper.api.LeagueAPIClient.get_rosters")
     @patch("sleeper.api.LeagueAPIClient.get_matchups_for_week")
     @patch("sleeper.api.LeagueAPIClient.get_sport_state")
     @patch("sleeper.api.LeagueAPIClient.get_winners_bracket")
+    def test_load_league_happyPath(
+        self,
+        mockGetWinnersBracket,
+        mockGetSportState,
+        mockGetMatchupsForWeek,
+        mockGetRosters,
+        mockGetUsersInLeague,
+        mockGetLeague,
+    ):
+        # create mock SleeperLeague objects
+
+        mockSleeperLeague2022 = Mock()
+        mockSleeperLeague2022.season = "2022"
+        mockSleeperLeague2022.status = SleeperSeasonStatus.COMPLETE
+        mockSleeperLeague2022.playoff_matchups = []
+        mockSleeperLeague2022.name = "Test League 2022"
+        mockSleeperLeague2022.settings.playoff_week_start = 3
+        mockSleeperLeague2022.settings.league_average_match = 0
+        mockSleeperLeague2022.settings.divisions = 2
+        mockSleeperLeague2022.settings.playoff_round_type_enum = (
+            SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND
+        )
+        mockSleeperLeague2022.metadata.division_1 = "d1_2022"
+        mockSleeperLeague2022.metadata.division_2 = "d2_2022"
+
+        mockSleeperLeague2023 = Mock()
+        mockSleeperLeague2023.season = "2023"
+        mockSleeperLeague2023.status = SleeperSeasonStatus.IN_SEASON
+        mockSleeperLeague2023.playoff_matchups = []
+        mockSleeperLeague2023.name = "Test League 2023"
+        mockSleeperLeague2023.settings.playoff_week_start = 3
+        mockSleeperLeague2023.settings.league_average_match = 0
+        mockSleeperLeague2023.settings.divisions = 2
+        mockSleeperLeague2023.settings.playoff_round_type_enum = (
+            SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND
+        )
+        mockSleeperLeague2023.metadata.division_1 = "d1_2023"
+        mockSleeperLeague2023.metadata.division_2 = "d2_2023"
+
+        # create mock SleeperUser objects
+        mockSleeperUsers2022 = [
+            self.__generateMockSleeperUser(displayName="User 1", userId="1"),
+            self.__generateMockSleeperUser(displayName="User 2", userId="2"),
+            self.__generateMockSleeperUser(displayName="User 3", userId="3"),
+            self.__generateMockSleeperUser(displayName="User 4", userId="4"),
+            self.__generateMockSleeperUser(
+                displayName="User 5", userId="5", metadata={"team_name": "Team 5"}
+            ),
+            self.__generateMockSleeperUser(
+                displayName="User 6", userId="6", metadata={"team_name": "Team 6"}
+            ),
+            self.__generateMockSleeperUser(
+                displayName="User 7", userId="7", metadata={"team_name": "Team 7"}
+            ),
+            self.__generateMockSleeperUser(
+                displayName="User 8", userId="8", metadata={"team_name": "Team 8"}
+            ),
+        ]
+
+        mockSleeperUsers2023 = [
+            self.__generateMockSleeperUser(displayName="User 1", userId="1"),
+            self.__generateMockSleeperUser(displayName="User 2", userId="2"),
+            self.__generateMockSleeperUser(displayName="User 3", userId="3"),
+            self.__generateMockSleeperUser(displayName="User 4", userId="4"),
+            self.__generateMockSleeperUser(
+                displayName="User 5", userId="5", metadata={"team_name": "Team 5"}
+            ),
+            self.__generateMockSleeperUser(
+                displayName="User 6", userId="6", metadata={"team_name": "Team 6"}
+            ),
+            self.__generateMockSleeperUser(
+                displayName="User 7", userId="7", metadata={"team_name": "Team 7"}
+            ),
+            self.__generateMockSleeperUser(
+                displayName="User 8", userId="8", metadata={"team_name": "Team 8"}
+            ),
+        ]
+
+        # create mock SleeperRoster objects
+        # roster id will be YYYY (year) RR (roster number)
+        mockSleeperRosters2022 = [
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202, division=1),
+            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203, division=1),
+            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204, division=1),
+            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205, division=2),
+            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206, division=2),
+            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207, division=2),
+            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208, division=2),
+        ]
+
+        mockSleeperRosters2023 = [
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202301, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202302, division=1),
+            self.__generateMockSleeperRoster(ownerId="3", rosterId=202303, division=1),
+            self.__generateMockSleeperRoster(ownerId="4", rosterId=202304, division=1),
+            self.__generateMockSleeperRoster(ownerId="5", rosterId=202305, division=2),
+            self.__generateMockSleeperRoster(ownerId="6", rosterId=202306, division=2),
+            self.__generateMockSleeperRoster(ownerId="7", rosterId=202307, division=2),
+            self.__generateMockSleeperRoster(ownerId="8", rosterId=202308, division=2),
+        ]
+
+        # create mock SleeperMatchup objects
+        # matchup id will be YYYY (year) WW (week number) MM (matchup number)
+        mockSleeperMatchups2022_1 = [
+            self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202201, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202202, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20220102, rosterId=202203, points=90.5),
+            self.__generateMockSleeperMatchup(matchupId=20220102, rosterId=202204, points=70.5),
+            self.__generateMockSleeperMatchup(matchupId=20220103, rosterId=202205, points=110),
+            self.__generateMockSleeperMatchup(matchupId=20220103, rosterId=202206, points=60),
+            self.__generateMockSleeperMatchup(matchupId=20220104, rosterId=202207, points=120),
+            self.__generateMockSleeperMatchup(matchupId=20220104, rosterId=202208, points=50),
+        ]
+
+        mockSleeperMatchups2022_2 = [
+            self.__generateMockSleeperMatchup(matchupId=20220201, rosterId=202201, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20220201, rosterId=202202, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20220202, rosterId=202203, points=90.5),
+            self.__generateMockSleeperMatchup(matchupId=20220202, rosterId=202204, points=70.5),
+            self.__generateMockSleeperMatchup(matchupId=20220203, rosterId=202205, points=110),
+            self.__generateMockSleeperMatchup(matchupId=20220203, rosterId=202206, points=60),
+            self.__generateMockSleeperMatchup(matchupId=20220204, rosterId=202207, points=120),
+            self.__generateMockSleeperMatchup(matchupId=20220204, rosterId=202208, points=50),
+        ]
+
+        # playoffs
+        mockSleeperMatchups2022_3 = [
+            self.__generateMockSleeperMatchup(matchupId=20220301, rosterId=202202, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20220301, rosterId=202203, points=90.5),
+        ]
+
+        # championship
+        mockSleeperMatchups2022_4 = [
+            self.__generateMockSleeperMatchup(matchupId=20220401, rosterId=202201, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20220401, rosterId=202202, points=99),
+        ]
+
+        mockSleeperMatchups2023_1 = [
+            self.__generateMockSleeperMatchup(matchupId=20230101, rosterId=202301, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20230101, rosterId=202302, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20230102, rosterId=202303, points=90.5),
+            self.__generateMockSleeperMatchup(matchupId=20230102, rosterId=202304, points=70.5),
+            self.__generateMockSleeperMatchup(matchupId=20230103, rosterId=202305, points=110),
+            self.__generateMockSleeperMatchup(matchupId=20230103, rosterId=202306, points=60),
+            self.__generateMockSleeperMatchup(matchupId=20230104, rosterId=202307, points=120),
+            self.__generateMockSleeperMatchup(matchupId=20230104, rosterId=202308, points=50),
+        ]
+
+        mockSleeperMatchups2023_2 = [
+            self.__generateMockSleeperMatchup(matchupId=20230201, rosterId=202301, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20230201, rosterId=202302, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20230202, rosterId=202303, points=90.5),
+            self.__generateMockSleeperMatchup(matchupId=20230202, rosterId=202304, points=70.5),
+            self.__generateMockSleeperMatchup(matchupId=20230203, rosterId=202305, points=110),
+            self.__generateMockSleeperMatchup(matchupId=20230203, rosterId=202306, points=60),
+            self.__generateMockSleeperMatchup(matchupId=20230204, rosterId=202307, points=120),
+            self.__generateMockSleeperMatchup(matchupId=20230204, rosterId=202308, points=50),
+        ]
+
+        # playoffs
+        mockSleeperMatchups2023_3 = [
+            self.__generateMockSleeperMatchup(matchupId=20230301, rosterId=202302, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20230301, rosterId=202303, points=90.5),
+        ]
+
+        # championship
+        mockSleeperMatchups2023_4 = [
+            self.__generateMockSleeperMatchup(matchupId=20230401, rosterId=202301, points=100),
+            self.__generateMockSleeperMatchup(matchupId=20230401, rosterId=202302, points=99),
+        ]
+
+        # create mock SleeperSportState objects
+        mockSleeperSportState2022 = self.__generateMockSleeperSportState(season="2022", leg=5)
+        mockSleeperSportState2023 = self.__generateMockSleeperSportState(season="2023", leg=5)
+
+        # create mock SleeperPlayoffMatchup objects
+        mockSleeperPlayoffMatchups2022 = [
+            self.__generateMockSleeperPlayoffMatchup(
+                round=1,
+                team1RosterId=202202,
+                team2RosterId=202203,
+                winningRosterId=202202,
+                p=0,
+                matchupId=20220301,
+            ),
+            self.__generateMockSleeperPlayoffMatchup(
+                round=2,
+                team1RosterId=202201,
+                team2RosterId=202202,
+                winningRosterId=202201,
+                p=1,
+                matchupId=20220401,
+            ),
+        ]
+
+        mockSleeperPlayoffMatchups2023 = [
+            self.__generateMockSleeperPlayoffMatchup(
+                round=1,
+                team1RosterId=202302,
+                team2RosterId=202303,
+                winningRosterId=202302,
+                p=0,
+                matchupId=20230301,
+            ),
+            self.__generateMockSleeperPlayoffMatchup(
+                round=2,
+                team1RosterId=202301,
+                team2RosterId=202302,
+                winningRosterId=202301,
+                p=1,
+                matchupId=20230401,
+            ),
+        ]
+
+        mockGetLeague.side_effect = [mockSleeperLeague2022, mockSleeperLeague2023]
+        mockGetUsersInLeague.side_effect = [mockSleeperUsers2022, mockSleeperUsers2023]
+        mockGetRosters.side_effect = [mockSleeperRosters2022, mockSleeperRosters2023]
+        mockGetMatchupsForWeek.side_effect = [
+            mockSleeperMatchups2022_1,
+            mockSleeperMatchups2022_2,
+            mockSleeperMatchups2022_3,
+            mockSleeperMatchups2022_4,
+            mockSleeperMatchups2023_1,
+            mockSleeperMatchups2023_2,
+            mockSleeperMatchups2023_3,
+            mockSleeperMatchups2023_4,
+        ]
+        mockGetSportState.side_effect = [mockSleeperSportState2022, mockSleeperSportState2023]
+        mockGetWinnersBracket.side_effect = [
+            mockSleeperPlayoffMatchups2022,
+            mockSleeperPlayoffMatchups2023,
+        ]
+
+        # create instance of SleeperLeagueLoader and call load_league method
+        sleeper_league_loader = SleeperLeagueLoader("123", [2022, 2023], leagueName="custom name")
+        league = sleeper_league_loader.loadLeague()
+
+        self.assertEqual("custom name", league.name)
+
+    @patch("sleeper.api.LeagueAPIClient.get_league")
+    @patch("sleeper.api.LeagueAPIClient.get_users_in_league")
+    @patch("sleeper.api.LeagueAPIClient.get_rosters")
+    @patch("sleeper.api.LeagueAPIClient.get_matchups_for_week")
+    @patch("sleeper.api.LeagueAPIClient.get_sport_state")
+    @patch("sleeper.api.LeagueAPIClient.get_winners_bracket")
     def test_load_league_happyPath_playoffRoundType_twoWeekChampionshipRound(
         self,
         mockGetWinnersBracket,
         mockGetSportState,
         mockGetMatchupsForWeek,
         mockGetRosters,
         mockGetUsersInLeague,
@@ -1036,17 +1326,20 @@
         mockSleeperLeague2022 = Mock()
         mockSleeperLeague2022.season = "2022"
         mockSleeperLeague2022.status = SleeperSeasonStatus.COMPLETE
         mockSleeperLeague2022.playoff_matchups = []
         mockSleeperLeague2022.name = "Test League 2022"
         mockSleeperLeague2022.settings.playoff_week_start = 3
         mockSleeperLeague2022.settings.league_average_match = 0
+        mockSleeperLeague2022.settings.divisions = 2
         mockSleeperLeague2022.settings.playoff_round_type_enum = (
             SleeperPlayoffRoundType.TWO_WEEK_CHAMPIONSHIP_ROUND
         )
+        mockSleeperLeague2022.metadata.division_1 = "d1_2022"
+        mockSleeperLeague2022.metadata.division_2 = "d2_2022"
 
         # create mock SleeperUser objects
         mockSleeperUsers2022 = [
             self.__generateMockSleeperUser(displayName="User 1", userId="1"),
             self.__generateMockSleeperUser(displayName="User 2", userId="2"),
             self.__generateMockSleeperUser(displayName="User 3", userId="3"),
             self.__generateMockSleeperUser(displayName="User 4", userId="4"),
@@ -1063,22 +1356,22 @@
                 displayName="User 8", userId="8", metadata={"team_name": "Team 8"}
             ),
         ]
 
         # create mock SleeperRoster objects
         # roster id will be YYYY (year) RR (roster number)
         mockSleeperRosters2022 = [
-            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201),
-            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202),
-            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203),
-            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204),
-            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205),
-            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206),
-            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207),
-            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208),
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202, division=1),
+            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203, division=1),
+            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204, division=1),
+            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205, division=2),
+            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206, division=2),
+            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207, division=2),
+            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208, division=2),
         ]
 
         # create mock SleeperMatchup objects
         # matchup id will be YYYY (year) WW (week number) MM (matchup number)
         mockSleeperMatchups2022_1 = [
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202201, points=100),
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202202, points=100),
@@ -1164,35 +1457,39 @@
         mockGetWinnersBracket.side_effect = [mockSleeperPlayoffMatchups2022]
 
         # create instance of SleeperLeagueLoader and call load_league method
         sleeper_league_loader = SleeperLeagueLoader("123", [2022])
         league = sleeper_league_loader.loadLeague()
 
         # expected league
-        team1_2022 = Team(ownerId=1, name="User 1")
-        team2_2022 = Team(ownerId=2, name="User 2")
-        team3_2022 = Team(ownerId=3, name="User 3")
-        team4_2022 = Team(ownerId=4, name="User 4")
-        team5_2022 = Team(ownerId=5, name="Team 5")
-        team6_2022 = Team(ownerId=6, name="Team 6")
-        team7_2022 = Team(ownerId=7, name="Team 7")
-        team8_2022 = Team(ownerId=8, name="Team 8")
+
+        owner1 = Owner(name="User 1")
+        owner2 = Owner(name="User 2")
+        owner3 = Owner(name="User 3")
+        owner4 = Owner(name="User 4")
+        owner5 = Owner(name="User 5")
+        owner6 = Owner(name="User 6")
+        owner7 = Owner(name="User 7")
+        owner8 = Owner(name="User 8")
+
+        division1_2022 = Division(name="d1_2022")
+        division2_2022 = Division(name="d2_2022")
+
+        team1_2022 = Team(ownerId=owner1.id, name="User 1", divisionId=division1_2022.id)
+        team2_2022 = Team(ownerId=owner2.id, name="User 2", divisionId=division1_2022.id)
+        team3_2022 = Team(ownerId=owner3.id, name="User 3", divisionId=division1_2022.id)
+        team4_2022 = Team(ownerId=owner4.id, name="User 4", divisionId=division1_2022.id)
+        team5_2022 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2022.id)
+        team6_2022 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2022.id)
+        team7_2022 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2022.id)
+        team8_2022 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2022.id)
 
         expectedLeague = League(
             name="Test League 2022",
-            owners=[
-                Owner(name="User 1"),
-                Owner(name="User 2"),
-                Owner(name="User 3"),
-                Owner(name="User 4"),
-                Owner(name="User 5"),
-                Owner(name="User 6"),
-                Owner(name="User 7"),
-                Owner(name="User 8"),
-            ],
+            owners=[owner1, owner2, owner3, owner4, owner5, owner6, owner7, owner8],
             years=[
                 Year(
                     yearNumber=2022,
                     teams=[
                         team1_2022,
                         team2_2022,
                         team3_2022,
@@ -1325,18 +1622,19 @@
                                     teamAHasTiebreaker=True,
                                     teamBHasTiebreaker=False,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2022, division2_2022],
                 )
             ],
         )
-        self.assertEqual(league, expectedLeague)
+        self.assertTrue(league.equals(expectedLeague, ignoreBaseIds=True, ignoreIds=True))
         # check multiWeekMatchupIds
         for year in league.years:
             for week in year.weeks[:3]:
                 for matchup in week.matchups:
                     self.assertIsNone(matchup.multiWeekMatchupId)
             for week in year.weeks[3:]:
                 for matchup in week.matchups:
@@ -1363,17 +1661,20 @@
         mockSleeperLeague2022 = Mock()
         mockSleeperLeague2022.season = "2022"
         mockSleeperLeague2022.status = SleeperSeasonStatus.COMPLETE
         mockSleeperLeague2022.playoff_matchups = []
         mockSleeperLeague2022.name = "Test League 2022"
         mockSleeperLeague2022.settings.playoff_week_start = 3
         mockSleeperLeague2022.settings.league_average_match = 0
+        mockSleeperLeague2022.settings.divisions = 2
         mockSleeperLeague2022.settings.playoff_round_type_enum = (
             SleeperPlayoffRoundType.TWO_WEEKS_PER_ROUND
         )
+        mockSleeperLeague2022.metadata.division_1 = "d1_2022"
+        mockSleeperLeague2022.metadata.division_2 = "d2_2022"
 
         # create mock SleeperUser objects
         mockSleeperUsers2022 = [
             self.__generateMockSleeperUser(displayName="User 1", userId="1"),
             self.__generateMockSleeperUser(displayName="User 2", userId="2"),
             self.__generateMockSleeperUser(displayName="User 3", userId="3"),
             self.__generateMockSleeperUser(displayName="User 4", userId="4"),
@@ -1390,22 +1691,22 @@
                 displayName="User 8", userId="8", metadata={"team_name": "Team 8"}
             ),
         ]
 
         # create mock SleeperRoster objects
         # roster id will be YYYY (year) RR (roster number)
         mockSleeperRosters2022 = [
-            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201),
-            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202),
-            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203),
-            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204),
-            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205),
-            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206),
-            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207),
-            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208),
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202, division=1),
+            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203, division=1),
+            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204, division=1),
+            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205, division=2),
+            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206, division=2),
+            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207, division=2),
+            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208, division=2),
         ]
 
         # create mock SleeperMatchup objects
         # matchup id will be YYYY (year) WW (week number) MM (matchup number)
         mockSleeperMatchups2022_1 = [
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202201, points=100),
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202202, points=100),
@@ -1506,35 +1807,39 @@
         mockGetWinnersBracket.side_effect = [mockSleeperPlayoffMatchups2022]
 
         # create instance of SleeperLeagueLoader and call load_league method
         sleeper_league_loader = SleeperLeagueLoader("123", [2022])
         league = sleeper_league_loader.loadLeague()
 
         # expected league
-        team1_2022 = Team(ownerId=1, name="User 1")
-        team2_2022 = Team(ownerId=2, name="User 2")
-        team3_2022 = Team(ownerId=3, name="User 3")
-        team4_2022 = Team(ownerId=4, name="User 4")
-        team5_2022 = Team(ownerId=5, name="Team 5")
-        team6_2022 = Team(ownerId=6, name="Team 6")
-        team7_2022 = Team(ownerId=7, name="Team 7")
-        team8_2022 = Team(ownerId=8, name="Team 8")
+
+        owner1 = Owner(name="User 1")
+        owner2 = Owner(name="User 2")
+        owner3 = Owner(name="User 3")
+        owner4 = Owner(name="User 4")
+        owner5 = Owner(name="User 5")
+        owner6 = Owner(name="User 6")
+        owner7 = Owner(name="User 7")
+        owner8 = Owner(name="User 8")
+
+        division1_2022 = Division(name="d1_2022")
+        division2_2022 = Division(name="d2_2022")
+
+        team1_2022 = Team(ownerId=owner1.id, name="User 1", divisionId=division1_2022.id)
+        team2_2022 = Team(ownerId=owner2.id, name="User 2", divisionId=division1_2022.id)
+        team3_2022 = Team(ownerId=owner3.id, name="User 3", divisionId=division1_2022.id)
+        team4_2022 = Team(ownerId=owner4.id, name="User 4", divisionId=division1_2022.id)
+        team5_2022 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2022.id)
+        team6_2022 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2022.id)
+        team7_2022 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2022.id)
+        team8_2022 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2022.id)
 
         expectedLeague = League(
             name="Test League 2022",
-            owners=[
-                Owner(name="User 1"),
-                Owner(name="User 2"),
-                Owner(name="User 3"),
-                Owner(name="User 4"),
-                Owner(name="User 5"),
-                Owner(name="User 6"),
-                Owner(name="User 7"),
-                Owner(name="User 8"),
-            ],
+            owners=[owner1, owner2, owner3, owner4, owner5, owner6, owner7, owner8],
             years=[
                 Year(
                     yearNumber=2022,
                     teams=[
                         team1_2022,
                         team2_2022,
                         team3_2022,
@@ -1681,18 +1986,19 @@
                                     teamAHasTiebreaker=True,
                                     teamBHasTiebreaker=False,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2022, division2_2022],
                 )
             ],
         )
-        self.assertEqual(league, expectedLeague)
+        self.assertTrue(league.equals(expectedLeague, ignoreBaseIds=True, ignoreIds=True))
         # check multiWeekMatchupIds
         for year in league.years:
             for week in year.weeks[:2]:
                 for matchup in week.matchups:
                     self.assertIsNone(matchup.multiWeekMatchupId)
             for week in year.weeks[2:]:
                 for matchup in week.matchups:
@@ -1717,27 +2023,30 @@
     ):
         # create mock SleeperLeague objects
         mockSleeperLeague2022 = Mock()
         mockSleeperLeague2022.season = "2022"
         mockSleeperLeague2022.status = SleeperSeasonStatus.COMPLETE
         mockSleeperLeague2022.name = "Test League 2022"
         mockSleeperLeague2022.settings.playoff_week_start = 1
+        mockSleeperLeague2022.settings.divisions = 2
         mockSleeperLeague2022.settings.playoff_round_type_enum = None
+        mockSleeperLeague2022.metadata.division_1 = "d1_2022"
+        mockSleeperLeague2022.metadata.division_2 = "d2_2022"
 
         # create mock SleeperUser objects
         mockSleeperUsers2022 = [
             self.__generateMockSleeperUser(displayName="User 1", userId="1"),
             self.__generateMockSleeperUser(displayName="User 2", userId="2"),
         ]
 
         # create mock SleeperRoster objects
         # roster id will be YYYY (year) RR (roster number)
         mockSleeperRosters2022 = [
-            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201),
-            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202),
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202, division=2),
         ]
 
         # create mock SleeperMatchup objects
         # matchup id will be YYYY (year) WW (week number) MM (matchup number)
         mockSleeperMatchups2022_1 = [
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202201, points=100),
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202202, points=100),
@@ -1788,28 +2097,34 @@
         mockSleeperLeague2022 = Mock()
         mockSleeperLeague2022.season = "2022"
         mockSleeperLeague2022.status = SleeperSeasonStatus.COMPLETE
         mockSleeperLeague2022.playoff_matchups = []
         mockSleeperLeague2022.name = "Test League 2022"
         mockSleeperLeague2022.settings.playoff_week_start = 3
         mockSleeperLeague2022.settings.league_average_match = 1
+        mockSleeperLeague2022.settings.divisions = 2
         mockSleeperLeague2022.settings.playoff_round_type_enum = (
             SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND
         )
+        mockSleeperLeague2022.metadata.division_1 = "d1_2022"
+        mockSleeperLeague2022.metadata.division_2 = "d2_2022"
 
         mockSleeperLeague2023 = Mock()
         mockSleeperLeague2023.season = "2023"
         mockSleeperLeague2023.status = SleeperSeasonStatus.IN_SEASON
         mockSleeperLeague2023.playoff_matchups = []
         mockSleeperLeague2023.name = "Test League 2023"
         mockSleeperLeague2023.settings.playoff_week_start = 3
         mockSleeperLeague2023.settings.league_average_match = 0
+        mockSleeperLeague2023.settings.divisions = 2
         mockSleeperLeague2023.settings.playoff_round_type_enum = (
             SleeperPlayoffRoundType.ONE_WEEK_PER_ROUND
         )
+        mockSleeperLeague2023.metadata.division_1 = "d1_2023"
+        mockSleeperLeague2023.metadata.division_2 = "d2_2023"
 
         # create mock SleeperUser objects
         mockSleeperUsers2022 = [
             self.__generateMockSleeperUser(displayName="User 1", userId="1"),
             self.__generateMockSleeperUser(displayName="User 2", userId="2"),
             self.__generateMockSleeperUser(displayName="User 3", userId="3"),
             self.__generateMockSleeperUser(displayName="User 4", userId="4"),
@@ -1845,33 +2160,33 @@
                 displayName="User 8", userId="8", metadata={"team_name": "Team 8"}
             ),
         ]
 
         # create mock SleeperRoster objects
         # roster id will be YYYY (year) RR (roster number)
         mockSleeperRosters2022 = [
-            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201),
-            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202),
-            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203),
-            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204),
-            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205),
-            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206),
-            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207),
-            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208),
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202201, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202202, division=1),
+            self.__generateMockSleeperRoster(ownerId="3", rosterId=202203, division=1),
+            self.__generateMockSleeperRoster(ownerId="4", rosterId=202204, division=1),
+            self.__generateMockSleeperRoster(ownerId="5", rosterId=202205, division=2),
+            self.__generateMockSleeperRoster(ownerId="6", rosterId=202206, division=2),
+            self.__generateMockSleeperRoster(ownerId="7", rosterId=202207, division=2),
+            self.__generateMockSleeperRoster(ownerId="8", rosterId=202208, division=2),
         ]
 
         mockSleeperRosters2023 = [
-            self.__generateMockSleeperRoster(ownerId="1", rosterId=202301),
-            self.__generateMockSleeperRoster(ownerId="2", rosterId=202302),
-            self.__generateMockSleeperRoster(ownerId="3", rosterId=202303),
-            self.__generateMockSleeperRoster(ownerId="4", rosterId=202304),
-            self.__generateMockSleeperRoster(ownerId="5", rosterId=202305),
-            self.__generateMockSleeperRoster(ownerId="6", rosterId=202306),
-            self.__generateMockSleeperRoster(ownerId="7", rosterId=202307),
-            self.__generateMockSleeperRoster(ownerId="8", rosterId=202308),
+            self.__generateMockSleeperRoster(ownerId="1", rosterId=202301, division=1),
+            self.__generateMockSleeperRoster(ownerId="2", rosterId=202302, division=1),
+            self.__generateMockSleeperRoster(ownerId="3", rosterId=202303, division=1),
+            self.__generateMockSleeperRoster(ownerId="4", rosterId=202304, division=1),
+            self.__generateMockSleeperRoster(ownerId="5", rosterId=202305, division=2),
+            self.__generateMockSleeperRoster(ownerId="6", rosterId=202306, division=2),
+            self.__generateMockSleeperRoster(ownerId="7", rosterId=202307, division=2),
+            self.__generateMockSleeperRoster(ownerId="8", rosterId=202308, division=2),
         ]
 
         # create mock SleeperMatchup objects
         # matchup id will be YYYY (year) WW (week number) MM (matchup number)
         mockSleeperMatchups2022_1 = [
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202201, points=100),
             self.__generateMockSleeperMatchup(matchupId=20220101, rosterId=202202, points=100),
@@ -2003,44 +2318,51 @@
         ]
 
         # create instance of SleeperLeagueLoader and call load_league method
         sleeper_league_loader = SleeperLeagueLoader("123", [2022, 2023])
         league = sleeper_league_loader.loadLeague()
 
         # expected league
-        team1_2022 = Team(ownerId=1, name="User 1")
-        team2_2022 = Team(ownerId=2, name="User 2")
-        team3_2022 = Team(ownerId=3, name="User 3")
-        team4_2022 = Team(ownerId=4, name="User 4")
-        team5_2022 = Team(ownerId=5, name="Team 5")
-        team6_2022 = Team(ownerId=6, name="Team 6")
-        team7_2022 = Team(ownerId=7, name="Team 7")
-        team8_2022 = Team(ownerId=8, name="Team 8")
-
-        team1_2023 = Team(ownerId=1, name="User 1")
-        team2_2023 = Team(ownerId=2, name="User 2")
-        team3_2023 = Team(ownerId=3, name="User 3")
-        team4_2023 = Team(ownerId=4, name="User 4")
-        team5_2023 = Team(ownerId=5, name="Team 5")
-        team6_2023 = Team(ownerId=6, name="Team 6")
-        team7_2023 = Team(ownerId=7, name="Team 7")
-        team8_2023 = Team(ownerId=8, name="Team 8")
+
+        owner1 = Owner(name="User 1")
+        owner2 = Owner(name="User 2")
+        owner3 = Owner(name="User 3")
+        owner4 = Owner(name="User 4")
+        owner5 = Owner(name="User 5")
+        owner6 = Owner(name="User 6")
+        owner7 = Owner(name="User 7")
+        owner8 = Owner(name="User 8")
+
+        division1_2022 = Division(name="d1_2022")
+        division2_2022 = Division(name="d2_2022")
+
+        division1_2023 = Division(name="d1_2023")
+        division2_2023 = Division(name="d2_2023")
+
+        team1_2022 = Team(ownerId=owner1.id, name="User 1", divisionId=division1_2022.id)
+        team2_2022 = Team(ownerId=owner2.id, name="User 2", divisionId=division1_2022.id)
+        team3_2022 = Team(ownerId=owner3.id, name="User 3", divisionId=division1_2022.id)
+        team4_2022 = Team(ownerId=owner4.id, name="User 4", divisionId=division1_2022.id)
+        team5_2022 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2022.id)
+        team6_2022 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2022.id)
+        team7_2022 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2022.id)
+        team8_2022 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2022.id)
+
+        team1_2023 = Team(ownerId=owner1.id, name="User 1", divisionId=division1_2023.id)
+        team2_2023 = Team(ownerId=owner2.id, name="User 2", divisionId=division1_2023.id)
+        team3_2023 = Team(ownerId=owner3.id, name="User 3", divisionId=division1_2023.id)
+        team4_2023 = Team(ownerId=owner4.id, name="User 4", divisionId=division1_2023.id)
+        team5_2023 = Team(ownerId=owner5.id, name="Team 5", divisionId=division2_2023.id)
+        team6_2023 = Team(ownerId=owner6.id, name="Team 6", divisionId=division2_2023.id)
+        team7_2023 = Team(ownerId=owner7.id, name="Team 7", divisionId=division2_2023.id)
+        team8_2023 = Team(ownerId=owner8.id, name="Team 8", divisionId=division2_2023.id)
 
         expectedLeague = League(
             name="Test League 2023",
-            owners=[
-                Owner(name="User 1"),
-                Owner(name="User 2"),
-                Owner(name="User 3"),
-                Owner(name="User 4"),
-                Owner(name="User 5"),
-                Owner(name="User 6"),
-                Owner(name="User 7"),
-                Owner(name="User 8"),
-            ],
+            owners=[owner1, owner2, owner3, owner4, owner5, owner6, owner7, owner8],
             years=[
                 Year(
                     yearNumber=2022,
                     teams=[
                         team1_2022,
                         team2_2022,
                         team3_2022,
@@ -2169,14 +2491,15 @@
                                     teamBHasTiebreaker=False,
                                     multiWeekMatchupId=None,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=YearSettings(leagueMedianGames=True),
+                    divisions=[division1_2022, division2_2022],
                 ),
                 Year(
                     yearNumber=2023,
                     teams=[
                         team1_2023,
                         team2_2023,
                         team3_2023,
@@ -2305,16 +2628,17 @@
                                     teamBHasTiebreaker=False,
                                     multiWeekMatchupId=None,
                                 )
                             ],
                         ),
                     ],
                     yearSettings=None,
+                    divisions=[division1_2023, division2_2023],
                 ),
             ],
         )
-        self.assertEqual(league, expectedLeague)
+        self.assertTrue(league.equals(expectedLeague, ignoreBaseIds=True, ignoreIds=True))
         # check multiWeekMatchupIds
         for year in league.years:
             for week in year.weeks:
                 for matchup in week.matchups:
                     self.assertIsNone(matchup.multiWeekMatchupId)
```

### Comparing `leeger-2.4.0/test/test_league_loader/test_YahooLeagueLoader.py` & `leeger-2.5.0/test/test_league_loader/test_YahooLeagueLoader.py`

 * *Files 13% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             yahooLeagueLoader = YahooLeagueLoader("123", [2022], clientId="cid", clientSecret="cs")
             yahooLeagueLoader.loadLeague()
         self.assertEqual("Login to yahoofantasy timed out.", str(context.exception))
 
     @mock.patch("multiprocessing.Process")
     @mock.patch("yahoofantasy.Context.__init__")
     @mock.patch("yahoofantasy.Context.get_leagues")
-    def test_get_all_leagues_noOwnerNamesAndAliases(
+    def test_loadLeague_happyPath(
         self, mockYahooContextGetLeagues, mockYahooContextInit, mockMultiprocessingProcess
     ):
         # mock real league 2022
         mockLeague2022 = Mock()
         mockLeague2022.name = "Test League 2022"
         mockLeague2022.league_id = "123"
         mockLeague2022.season = 2022
@@ -626,25 +626,25 @@
         )
 
         # make sure we called login correctly
         mockMultiprocessingProcess.assert_called_once_with(
             target=yahooLeagueLoader.login, args=("cid", "cs")
         )
 
-        self.assertEqual(league, expectedLeague)
+        self.assertTrue(league.equals(expectedLeague, ignoreBaseIds=True, ignoreIds=True))
         # check multiWeekMatchupIds
         for year in league.years:
             for week in year.weeks:
                 for matchup in week.matchups:
                     self.assertIsNone(matchup.multiWeekMatchupId)
 
     @mock.patch("multiprocessing.Process")
     @mock.patch("yahoofantasy.Context.__init__")
     @mock.patch("yahoofantasy.Context.get_leagues")
-    def test_get_all_leagues_withOwnerNamesAndAliases(
+    def test_loadLeague_withOwnerNamesAndAliases(
         self, mockYahooContextGetLeagues, mockYahooContextInit, mockMultiprocessingProcess
     ):
         # mock real league 2022
         mockLeague2022 = Mock()
         mockLeague2022.name = "Test League 2022"
         mockLeague2022.league_id = "123"
         mockLeague2022.season = 2022
@@ -1187,13 +1187,346 @@
         )
 
         # make sure we called login correctly
         mockMultiprocessingProcess.assert_called_once_with(
             target=yahooLeagueLoader.login, args=("cid", "cs")
         )
 
-        self.assertEqual(league, expectedLeague)
+        self.assertTrue(league.equals(expectedLeague, ignoreBaseIds=True, ignoreIds=True))
         # check multiWeekMatchupIds
         for year in league.years:
             for week in year.weeks:
                 for matchup in week.matchups:
                     self.assertIsNone(matchup.multiWeekMatchupId)
+
+    @mock.patch("multiprocessing.Process")
+    @mock.patch("yahoofantasy.Context.__init__")
+    @mock.patch("yahoofantasy.Context.get_leagues")
+    def test_loadLeague_happyPath(
+        self, mockYahooContextGetLeagues, mockYahooContextInit, mockMultiprocessingProcess
+    ):
+        # mock real league 2022
+        mockLeague2022 = Mock()
+        mockLeague2022.name = "Test League 2022"
+        mockLeague2022.league_id = "123"
+        mockLeague2022.season = 2022
+        mockLeague2022.current_week = 3
+        mockLeague2022.end_week = 3
+
+        # mock fake leagues 2022
+        mockLeague2022_fake1 = Mock()
+        mockLeague2022_fake1.league_id = "456"
+
+        mockLeague2022_fake2 = Mock()
+        mockLeague2022_fake2.league_id = "999"
+
+        # mock league 2023
+        mockLeague2023 = Mock()
+        mockLeague2023.name = "Test League 2023"
+        mockLeague2023.league_id = "456"
+        mockLeague2023.season = 2023
+        mockLeague2023.current_week = 3
+        mockLeague2023.end_week = 3
+        mockLeague2023.past_league_id = "123"
+
+        # mock fake leagues 2023
+        mockLeague2023_fake1 = Mock()
+        mockLeague2023_fake1.league_id = "123"
+
+        mockLeague2023_fake2 = Mock()
+        mockLeague2023_fake2.league_id = "999"
+
+        # mock teams 2022
+        mockYahooTeam1_2022 = self.__getMockYahooTeam(
+            teamId=1, teamKey=1, name="Team 1", managerNickname="Owner 1", managerId=1
+        )
+        mockYahooTeam2_2022 = self.__getMockYahooTeam(
+            teamId=2, teamKey=2, name="Team 2", managerNickname="Owner 2", managerId=2
+        )
+        mockYahooTeam3_2022 = self.__getMockYahooTeam(
+            teamId=3, teamKey=3, name="Team 3", managerNickname="Owner 3", managerId=3
+        )
+        mockYahooTeam4_2022 = self.__getMockYahooTeam(
+            teamId=4, teamKey=4, name="Team 4", managerNickname="Owner 4", managerId=4
+        )
+        mockYahooTeam5_2022 = self.__getMockYahooTeam(
+            teamId=5, teamKey=5, name="Team 5", managerNickname="Owner 5", managerId=5
+        )
+        mockYahooTeam6_2022 = self.__getMockYahooTeam(
+            teamId=6, teamKey=6, name="Team 6", managerNickname="Owner 6", managerId=6
+        )
+        mockYahooTeam7_2022 = self.__getMockYahooTeam(
+            teamId=7, teamKey=7, name="Team 7", managerNickname="Owner 7", managerId=7
+        )
+        mockYahooTeam8_2022 = self.__getMockYahooTeam(
+            teamId=8, teamKey=8, name="Team 8", managerNickname="Owner 8", managerId=8
+        )
+        mockLeague2022.teams = self.__getMockTeamsMethod(
+            [
+                mockYahooTeam1_2022,
+                mockYahooTeam2_2022,
+                mockYahooTeam3_2022,
+                mockYahooTeam4_2022,
+                mockYahooTeam5_2022,
+                mockYahooTeam6_2022,
+                mockYahooTeam7_2022,
+                mockYahooTeam8_2022,
+            ]
+        )
+
+        # mock teams 2023
+        mockYahooTeam1_2023 = self.__getMockYahooTeam(
+            teamId=1, teamKey=1, name="Team 1", managerNickname="Owner 1", managerId=1
+        )
+        mockYahooTeam2_2023 = self.__getMockYahooTeam(
+            teamId=2, teamKey=2, name="Team 2", managerNickname="Owner 2", managerId=2
+        )
+        mockYahooTeam3_2023 = self.__getMockYahooTeam(
+            teamId=3, teamKey=3, name="Team 3", managerNickname="Owner 3", managerId=3
+        )
+        mockYahooTeam4_2023 = self.__getMockYahooTeam(
+            teamId=4, teamKey=4, name="Team 4", managerNickname="Owner 4", managerId=4
+        )
+        mockYahooTeam5_2023 = self.__getMockYahooTeam(
+            teamId=5, teamKey=5, name="Team 5", managerNickname="Owner 5", managerId=5
+        )
+        mockYahooTeam6_2023 = self.__getMockYahooTeam(
+            teamId=6, teamKey=6, name="Team 6", managerNickname="Owner 6", managerId=6
+        )
+        mockYahooTeam7_2023 = self.__getMockYahooTeam(
+            teamId=7, teamKey=7, name="Team 7", managerNickname="Owner 7", managerId=7
+        )
+        mockYahooTeam8_2023 = self.__getMockYahooTeam(
+            teamId=8, teamKey=8, name="Team 8", managerNickname="Owner 8", managerId=8
+        )
+        mockLeague2023.teams = self.__getMockTeamsMethod(
+            [
+                mockYahooTeam1_2023,
+                mockYahooTeam2_2023,
+                mockYahooTeam3_2023,
+                mockYahooTeam4_2023,
+                mockYahooTeam5_2023,
+                mockYahooTeam6_2023,
+                mockYahooTeam7_2023,
+                mockYahooTeam8_2023,
+            ]
+        )
+
+        # mock matchups 2022
+        # week -> matchup number -> year
+        mockYahooMatchup1_1_2022 = self.__getMockYahooMatchup(
+            week=1,
+            status="postevent",
+            winnerTeamKey=1,
+            isPlayoffs=0,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2022,
+        )
+        mockYahooMatchup1_1_2022.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam1_2022, teamPointsTotal=100),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam2_2022, teamPointsTotal=100),
+        ]
+        mockYahooMatchup1_2_2022 = self.__getMockYahooMatchup(
+            week=1,
+            status="postevent",
+            winnerTeamKey=3,
+            isPlayoffs=0,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2022,
+        )
+        mockYahooMatchup1_2_2022.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam3_2022, teamPointsTotal=100.1),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam4_2022, teamPointsTotal=90.1),
+        ]
+        mockYahooMatchup1_3_2022 = self.__getMockYahooMatchup(
+            week=1,
+            status="postevent",
+            winnerTeamKey=5,
+            isPlayoffs=0,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2022,
+        )
+        mockYahooMatchup1_3_2022.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam5_2022, teamPointsTotal=100),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam6_2022, teamPointsTotal=90),
+        ]
+        mockYahooMatchup1_4_2022 = self.__getMockYahooMatchup(
+            week=1,
+            status="postevent",
+            winnerTeamKey=7,
+            isPlayoffs=0,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2022,
+        )
+        mockYahooMatchup1_4_2022.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam7_2022, teamPointsTotal=100),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam8_2022, teamPointsTotal=90),
+        ]
+        # playoffs
+        mockYahooMatchup2_1_2022 = self.__getMockYahooMatchup(
+            week=2,
+            status="postevent",
+            winnerTeamKey=2,
+            isPlayoffs=1,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2022,
+        )
+        mockYahooMatchup2_1_2022.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam2_2022, teamPointsTotal=101),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam3_2022, teamPointsTotal=91),
+        ]
+        # championship
+        mockYahooMatchup3_1_2022 = self.__getMockYahooMatchup(
+            week=3,
+            status="postevent",
+            winnerTeamKey=1,
+            isPlayoffs=1,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2022,
+        )
+        mockYahooMatchup3_1_2022.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam1_2022, teamPointsTotal=102),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam2_2022, teamPointsTotal=92),
+        ]
+
+        # mock matchups 2023
+        # week -> matchup number -> year
+        mockYahooMatchup1_1_2023 = self.__getMockYahooMatchup(
+            week=1,
+            status="postevent",
+            winnerTeamKey=1,
+            isPlayoffs=0,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2023,
+        )
+        mockYahooMatchup1_1_2023.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam1_2023, teamPointsTotal=100),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam2_2023, teamPointsTotal=100),
+        ]
+        mockYahooMatchup1_2_2023 = self.__getMockYahooMatchup(
+            week=1,
+            status="postevent",
+            winnerTeamKey=3,
+            isPlayoffs=0,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2023,
+        )
+        mockYahooMatchup1_2_2023.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam3_2023, teamPointsTotal=100.1),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam4_2023, teamPointsTotal=90.1),
+        ]
+        mockYahooMatchup1_3_2023 = self.__getMockYahooMatchup(
+            week=1,
+            status="postevent",
+            winnerTeamKey=5,
+            isPlayoffs=0,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2023,
+        )
+        mockYahooMatchup1_3_2023.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam5_2023, teamPointsTotal=100),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam6_2023, teamPointsTotal=90),
+        ]
+        mockYahooMatchup1_4_2023 = self.__getMockYahooMatchup(
+            week=1,
+            status="postevent",
+            winnerTeamKey=7,
+            isPlayoffs=0,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2023,
+        )
+        mockYahooMatchup1_4_2023.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam7_2023, teamPointsTotal=100),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam8_2023, teamPointsTotal=90),
+        ]
+        # playoffs
+        mockYahooMatchup2_1_2023 = self.__getMockYahooMatchup(
+            week=2,
+            status="postevent",
+            winnerTeamKey=2,
+            isPlayoffs=1,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2023,
+        )
+        mockYahooMatchup2_1_2023.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam2_2023, teamPointsTotal=101),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam3_2023, teamPointsTotal=91),
+        ]
+        # championship
+        mockYahooMatchup3_1_2023 = self.__getMockYahooMatchup(
+            week=3,
+            status="postevent",
+            winnerTeamKey=1,
+            isPlayoffs=1,
+            isTied=0,
+            isConsolation=0,
+            league=mockLeague2023,
+        )
+        mockYahooMatchup3_1_2023.teams.team = [
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam1_2023, teamPointsTotal=102),
+            self.__setMockYahooTeamPoints(mockYahooTeam=mockYahooTeam2_2023, teamPointsTotal=92),
+        ]
+
+        # mock weeks 2022
+        mockWeek1_2022 = Mock()
+        mockWeek1_2022.matchups = [
+            mockYahooMatchup1_1_2022,
+            mockYahooMatchup1_2_2022,
+            mockYahooMatchup1_3_2022,
+            mockYahooMatchup1_4_2022,
+        ]
+
+        mockWeek2_2022 = Mock()
+        mockWeek2_2022.matchups = [mockYahooMatchup2_1_2022]
+
+        mockWeek3_2022 = Mock()
+        mockWeek3_2022.matchups = [mockYahooMatchup3_1_2022]
+
+        mockLeague2022.weeks = self.__getMockWeeksMethod(
+            [mockWeek1_2022, mockWeek2_2022, mockWeek3_2022]
+        )
+
+        # mock weeks 2023
+        mockWeek1_2023 = Mock()
+        mockWeek1_2023.matchups = [
+            mockYahooMatchup1_1_2023,
+            mockYahooMatchup1_2_2023,
+            mockYahooMatchup1_3_2023,
+            mockYahooMatchup1_4_2023,
+        ]
+
+        mockWeek2_2023 = Mock()
+        mockWeek2_2023.matchups = [mockYahooMatchup2_1_2023]
+
+        mockWeek3_2023 = Mock()
+        mockWeek3_2023.matchups = [mockYahooMatchup3_1_2023]
+
+        mockLeague2023.weeks = self.__getMockWeeksMethod(
+            [mockWeek1_2023, mockWeek2_2023, mockWeek3_2023]
+        )
+
+        mockYahooContextInit.side_effect = [None]
+        mockYahooContextGetLeagues.side_effect = [
+            [mockLeague2023_fake1, mockLeague2023, mockLeague2023_fake2],
+            [mockLeague2022_fake1, mockLeague2022, mockLeague2022_fake2],
+        ]
+        mockLoginProcess = mockMultiprocessingProcess.return_value
+        mockLoginProcess.is_alive.return_value = False  # Simulate login process completion
+
+        # load league
+        yahooLeagueLoader = YahooLeagueLoader(
+            "456", [2022, 2023], clientId="cid", clientSecret="cs", leagueName="custom name"
+        )
+        league = yahooLeagueLoader.loadLeague()
+
+        self.assertEqual("custom name", league.name)
```

### Comparing `leeger-2.4.0/test/test_model/test_abstract/test_UniqueId.py` & `leeger-2.5.0/test/test_model/test_abstract/test_UniqueId.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_model/test_filter/test_AllTimeFilters.py` & `leeger-2.5.0/test/test_model/test_filter/test_AllTimeFilters.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_model/test_league/test_League.py` & `leeger-2.5.0/test/test_model/test_league/test_League.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,31 @@
 
         self.assertEqual("leagueName", league.name)
         self.assertEqual(1, len(league.owners))
         self.assertEqual(1, len(league.years))
         self.assertEqual(owner.id, league.owners[0].id)
         self.assertEqual(year.id, league.years[0].id)
 
+    def test_league_eq_callsEqualsMethod(self):
+        # create League 1
+        owners_1, teams_1 = getNDefaultOwnersAndTeams(2)
+
+        matchup_1 = Matchup(
+            teamAId=teams_1[0].id,
+            teamBId=teams_1[1].id,
+            teamAScore=1.1,
+            teamBScore=2.2,
+            matchupType=MatchupType.REGULAR_SEASON,
+        )
+        week_1 = Week(weekNumber=1, matchups=[matchup_1])
+        year_1 = Year(yearNumber=2000, teams=teams_1, weeks=[week_1])
+        league_1 = League(name="LEAGUE", owners=owners_1, years=[year_1])
+
+        self.assertTrue(league_1 == league_1)
+
     def test_league_eq_equal(self):
         # create League 1
         owners_1, teams_1 = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
             teamBId=teams_1[1].id,
@@ -50,15 +67,15 @@
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_2 = Week(weekNumber=1, matchups=[matchup_2])
         year_2 = Year(yearNumber=2000, teams=teams_2, weeks=[week_2])
         league_2 = League(name="LEAGUE", owners=owners_2, years=[year_2])
 
-        self.assertEqual(league_1, league_2)
+        self.assertTrue(league_1.equals(league_2, ignoreBaseIds=True, ignoreIds=True))
 
     def test_league_eq_notEqual(self):
         # create League 1
         owners_1, teams_1 = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
@@ -81,15 +98,15 @@
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_2 = Week(weekNumber=1, matchups=[matchup_2])
         year_2 = Year(yearNumber=2000, teams=teams_2, weeks=[week_2])
         league_2 = League(name="LEAGUE 2", owners=owners_2, years=[year_2])
 
-        self.assertNotEqual(league_1, league_2)
+        self.assertFalse(league_1.equals(league_2, ignoreBaseIds=True, ignoreIds=True))
 
     def test_league_add_happyPath(self):
         # create League 1
         owners_1, teams_1 = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
@@ -154,17 +171,17 @@
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_2 = Week(weekNumber=1, matchups=[matchup_2])
         year_2 = Year(yearNumber=2001, teams=teams_2, weeks=[week_2])
         league_2 = League(name="LEAGUE 2", owners=owners_2, years=[year_2])
         league_2_copy = copy.deepcopy(league_2)
 
-        combinedLeague = league_1 + league_2
-        self.assertEqual(league_1, league_1_copy)
-        self.assertEqual(league_2, league_2_copy)
+        league_1 + league_2
+        self.assertTrue(league_1.equals(league_1_copy, ignoreBaseIds=True, ignoreIds=True))
+        self.assertTrue(league_2.equals(league_2_copy, ignoreBaseIds=True, ignoreIds=True))
 
     def test_league_add_teamsWithSameOwnersHaveSameOwnerIdAcrossYears(self):
         # create League 1
         owners_1, teams_1 = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
@@ -228,15 +245,15 @@
         year_2 = Year(yearNumber=2001, teams=teams_2, weeks=[week_2])
         league_2 = League(name="LEAGUE", owners=owners_2, years=[year_2])
 
         combinedLeague1 = league_1 + league_2
         combinedLeague2 = league_2 + league_1
         self.assertIsInstance(combinedLeague1, League)
         self.assertIsInstance(combinedLeague2, League)
-        self.assertEqual(combinedLeague1, combinedLeague2)
+        self.assertTrue(combinedLeague1.equals(combinedLeague2, ignoreBaseIds=True, ignoreIds=True))
 
     def test_league_add_sameLeagueName_nameIsntChanged(self):
         # create League 1
         owners_1, teams_1 = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
```

### Comparing `leeger-2.4.0/test/test_model/test_league/test_Matchup.py` & `leeger-2.5.0/test/test_model/test_league/test_Matchup.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,38 +71,65 @@
                 teamAHasTiebreaker=True,
                 teamBHasTiebreaker=True,
             )
         self.assertEqual(
             "Team A and Team B cannot both have the tiebreaker.", str(context.exception)
         )
 
+    def test_matchup_eq_callsEqualsMethod(self):
+        # create Matchup 1
+        _, teams_1 = getNDefaultOwnersAndTeams(2)
+        matchup_1 = Matchup(
+            teamAId=teams_1[0].id,
+            teamBId=teams_1[1].id,
+            teamAScore=1.1,
+            teamBScore=2.2,
+            multiWeekMatchupId="1",
+            matchupType=MatchupType.REGULAR_SEASON,
+        )
+
+        matchup_2 = Matchup(
+            teamAId=teams_1[0].id,
+            teamBId=teams_1[1].id,
+            teamAScore=1.1,
+            teamBScore=2.2,
+            multiWeekMatchupId="1",
+            matchupType=MatchupType.REGULAR_SEASON,
+        )
+
+        matchup_2.id = matchup_1.id
+
+        result = matchup_1 == matchup_2
+
+        self.assertTrue(result)
+
     def test_matchup_eq_equal(self):
         # create Matchup 1
         _, teams_1 = getNDefaultOwnersAndTeams(2)
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
             teamBId=teams_1[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             multiWeekMatchupId="1",
             matchupType=MatchupType.REGULAR_SEASON,
         )
 
-        # create Matchup 2
-        _, teams_2 = getNDefaultOwnersAndTeams(2)
         matchup_2 = Matchup(
-            teamAId=teams_2[0].id,
-            teamBId=teams_2[1].id,
+            teamAId=teams_1[0].id,
+            teamBId=teams_1[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             multiWeekMatchupId="1",
             matchupType=MatchupType.REGULAR_SEASON,
         )
 
-        self.assertEqual(matchup_1, matchup_2)
+        result = matchup_1.equals(matchup_2, ignoreBaseIds=True)
+
+        self.assertTrue(result)
 
     def test_matchup_eq_notEqual(self):
         # create Matchup 1
         _, teams_1 = getNDefaultOwnersAndTeams(2)
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
             teamBId=teams_1[1].id,
@@ -116,18 +143,20 @@
         _, teams_2 = getNDefaultOwnersAndTeams(2)
         matchup_2 = Matchup(
             teamAId=teams_2[0].id,
             teamBId=teams_2[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             multiWeekMatchupId="1",
-            matchupType=MatchupType.PLAYOFF,
+            matchupType=MatchupType.REGULAR_SEASON,
         )
 
-        self.assertNotEqual(matchup_1, matchup_2)
+        result = matchup_1.equals(matchup_2, ignoreBaseIds=True)
+
+        self.assertFalse(result)
 
     def test_matchup_toJson(self):
         owners, teams = getNDefaultOwnersAndTeams(2)
 
         matchup = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
```

### Comparing `leeger-2.4.0/test/test_model/test_league/test_Owner.py` & `leeger-2.5.0/test/test_model/test_league/test_Owner.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,31 +5,44 @@
 
 class TestOwner(unittest.TestCase):
     def test_owner_init(self):
         owner = Owner(name="name")
 
         self.assertEqual("name", owner.name)
 
+    def test_owner_eq_callsEqualsMethod(self):
+        # create Owner 1
+        owner_1 = Owner(name="owner")
+
+        # create Owner 2
+        owner_2 = Owner(name="owner")
+
+        owner_2.id = owner_1.id
+
+        result = owner_1 == owner_2
+
+        self.assertTrue(result)
+
     def test_owner_eq_equal(self):
         # create Owner 1
         owner_1 = Owner(name="owner")
 
         # create Owner 2
         owner_2 = Owner(name="owner")
 
-        self.assertEqual(owner_1, owner_2)
+        self.assertTrue(owner_1.equals(owner_2, ignoreBaseIds=True))
 
     def test_owner_eq_notEqual(self):
         # create Owner 1
         owner_1 = Owner(name="owner")
 
         # create Owner 2
         owner_2 = Owner(name="ownerDIF")
 
-        self.assertNotEqual(owner_1, owner_2)
+        self.assertFalse(owner_1.equals(owner_2, ignoreBaseIds=True))
 
     def test_owner_toJson(self):
         owner = Owner(name="owner")
         ownerJson = owner.toJson()
 
         self.assertIsInstance(ownerJson, dict)
         self.assertEqual("owner", ownerJson["name"])
```

### Comparing `leeger-2.4.0/test/test_model/test_league/test_Team.py` & `leeger-2.5.0/test/test_model/test_league/test_Team.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 import unittest
 
 from leeger.model.league.Team import Team
 
 
 class TestTeam(unittest.TestCase):
     def test_team_init(self):
-        team = Team(ownerId="ownerId", name="name")
+        team = Team(ownerId="ownerId", name="name", divisionId="did")
 
         self.assertEqual("ownerId", team.ownerId)
         self.assertEqual("name", team.name)
+        self.assertEqual("did", team.divisionId)
+
+    def test_team_eq_callsEqualsMethod(self):
+        # create Team 1
+        team_1 = Team(ownerId="1", name="1", divisionId="did")
+
+        # create Team 2
+        team_2 = Team(ownerId="1", name="1", divisionId="did")
+
+        team_2.id = team_1.id
+
+        result = team_1 == team_2
+
+        self.assertTrue(result)
 
     def test_team_eq_equal(self):
         # create Team 1
-        team_1 = Team(ownerId="1", name="1")
+        team_1 = Team(ownerId="1", name="1", divisionId="did")
 
         # create Team 2
-        team_2 = Team(ownerId="1", name="1")
+        team_2 = Team(ownerId="1", name="1", divisionId="did")
 
-        self.assertEqual(team_1, team_2)
+        self.assertTrue(team_1.equals(team_2, ignoreBaseIds=True))
 
     def test_team_eq_notEqual(self):
         # create Team 1
-        team_1 = Team(ownerId="1", name="1")
+        team_1 = Team(ownerId="1", name="1", divisionId="did")
 
         # create Team 2
-        team_2 = Team(ownerId="2", name="2dif")
+        team_2 = Team(ownerId="2", name="2dif", divisionId="did")
+
+        self.assertFalse(team_1.equals(team_2, ignoreBaseIds=True))
 
-        self.assertNotEqual(team_1, team_2)
+    def test_team_toFromJson(self):
+        team = Team(ownerId="", name="team", divisionId="did")
 
-    def test_team_toJson(self):
-        team = Team(ownerId="", name="team")
-        teamJson = team.toJson()
-
-        self.assertIsInstance(teamJson, dict)
-        self.assertEqual("team", teamJson["name"])
-
-    def test_team_fromJson(self):
-        team = Team(ownerId="", name="team")
-        teamJson = team.toJson()
-        teamDerived = Team.fromJson(teamJson)
-        self.assertEqual(team, teamDerived)
-        self.assertEqual(team.id, teamDerived.id)
+        self.assertEqual(team, Team.fromJson(team.toJson()))
```

### Comparing `leeger-2.4.0/test/test_model/test_league/test_Week.py` & `leeger-2.5.0/test/test_model/test_league/test_Week.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         self.assertTrue(week3.isChampionshipWeek)
         self.assertEqual(1, len(week1.matchups))
         self.assertEqual(matchup1.id, week1.matchups[0].id)
         self.assertEqual(matchup2.id, week2.matchups[0].id)
         self.assertEqual(matchup3.id, week3.matchups[0].id)
 
     def test_isPlayoffWeek_weekHasPlayoffMatchups_returnsTrue(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             matchupType=MatchupType.PLAYOFF,
@@ -47,15 +47,15 @@
 
         response = week1.isPlayoffWeek
 
         self.assertIsInstance(response, bool)
         self.assertTrue(response)
 
     def test_isPlayoffWeek_weekDoesNotHavePlayoffMatchups_returnsFalse(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             matchupType=MatchupType.REGULAR_SEASON,
@@ -65,15 +65,15 @@
 
         response = week1.isPlayoffWeek
 
         self.assertIsInstance(response, bool)
         self.assertFalse(response)
 
     def test_isChampionshipWeek_weekHasAChampionshipMatchup_returnsTrue(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             matchupType=MatchupType.CHAMPIONSHIP,
@@ -86,15 +86,15 @@
 
         self.assertIsInstance(response1, bool)
         self.assertTrue(response1)
         self.assertIsInstance(response2, bool)
         self.assertTrue(response2)
 
     def test_isChampionshipWeek_weekDoesNotHaveAnyChampionshipMatchups_returnsFalse(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             matchupType=MatchupType.REGULAR_SEASON,
@@ -104,15 +104,15 @@
 
         response = week1.isChampionshipWeek
 
         self.assertIsInstance(response, bool)
         self.assertFalse(response)
 
     def test_isRegularSeasonWeek_weekHasAllRegularSeasonMatchups_returnsTrue(self):
-        owners, teams = getNDefaultOwnersAndTeams(4)
+        _, teams = getNDefaultOwnersAndTeams(4)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             matchupType=MatchupType.REGULAR_SEASON,
@@ -129,15 +129,15 @@
 
         response = week1.isRegularSeasonWeek
 
         self.assertIsInstance(response, bool)
         self.assertTrue(response)
 
     def test_isChampionshipWeek_weekHasANonRegularSeasonMatchup_returnsFalse(self):
-        owners, teams = getNDefaultOwnersAndTeams(4)
+        _, teams = getNDefaultOwnersAndTeams(4)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             matchupType=MatchupType.REGULAR_SEASON,
@@ -153,38 +153,68 @@
         week1 = Week(weekNumber=1, matchups=[matchup1, matchup2])
 
         response = week1.isRegularSeasonWeek
 
         self.assertIsInstance(response, bool)
         self.assertFalse(response)
 
+    def test_week_eq_callsEqualsMethod(self):
+        # create Week 1
+        _, teams_1 = getNDefaultOwnersAndTeams(2)
+        matchup_1 = Matchup(
+            teamAId=teams_1[0].id,
+            teamBId=teams_1[1].id,
+            teamAScore=1.1,
+            teamBScore=2.2,
+            matchupType=MatchupType.REGULAR_SEASON,
+        )
+        week_1 = Week(weekNumber=1, matchups=[matchup_1])
+
+        # create Week 2
+        matchup_2 = Matchup(
+            teamAId=teams_1[0].id,
+            teamBId=teams_1[1].id,
+            teamAScore=1.1,
+            teamBScore=2.2,
+            matchupType=MatchupType.REGULAR_SEASON,
+        )
+        week_2 = Week(weekNumber=1, matchups=[matchup_2])
+
+        week_2.id = week_1.id
+        matchup_2.id = matchup_1.id
+
+        result = week_1 == week_2
+
+        self.assertTrue(result)
+
     def test_week_eq_equal(self):
         # create Week 1
         _, teams_1 = getNDefaultOwnersAndTeams(2)
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
             teamBId=teams_1[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_1 = Week(weekNumber=1, matchups=[matchup_1])
 
         # create Week 2
-        _, teams_2 = getNDefaultOwnersAndTeams(2)
         matchup_2 = Matchup(
-            teamAId=teams_2[0].id,
-            teamBId=teams_2[1].id,
+            teamAId=teams_1[0].id,
+            teamBId=teams_1[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_2 = Week(weekNumber=1, matchups=[matchup_2])
 
-        self.assertEqual(week_1, week_2)
+        result = week_1.equals(week_2, ignoreBaseIds=True)
+
+        self.assertTrue(result)
 
     def test_week_eq_notEqual(self):
         # create Week 1
         _, teams_1 = getNDefaultOwnersAndTeams(2)
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
             teamBId=teams_1[1].id,
@@ -199,20 +229,22 @@
         matchup_2 = Matchup(
             teamAId=teams_2[0].id,
             teamBId=teams_2[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
-        week_2 = Week(weekNumber=2, matchups=[matchup_2])
+        week_2 = Week(weekNumber=1, matchups=[matchup_2])
+
+        result = week_1.equals(week_2, ignoreBaseIds=True)
 
-        self.assertNotEqual(week_1, week_2)
+        self.assertFalse(result)
 
     def test_week_toJson(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
@@ -228,30 +260,30 @@
         self.assertEqual(1.1, weekJson["matchups"][0]["teamAScore"])
         self.assertEqual(2.2, weekJson["matchups"][0]["teamBScore"])
         self.assertEqual("REGULAR_SEASON", weekJson["matchups"][0]["matchupType"])
         self.assertFalse(weekJson["matchups"][0]["teamAHasTiebreaker"])
         self.assertFalse(weekJson["matchups"][0]["teamBHasTiebreaker"])
 
     def test_getMatchupWithTeamId_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week = Week(weekNumber=1, matchups=[matchup_1])
 
         response = week.getMatchupWithTeamId(teams[0].id)
         self.assertEqual(matchup_1, response)
 
     def test_getMatchupWithTeamId_teamIdNotInMatchups_raisesException(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
@@ -261,15 +293,15 @@
         with self.assertRaises(DoesNotExistException) as context:
             week.getMatchupWithTeamId("bad ID")
         self.assertEqual(
             "Week does not have a matchup with team ID 'bad ID'.", str(context.exception)
         )
 
     def test_week_fromJson(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
```

### Comparing `leeger-2.4.0/test/test_model/test_league/test_Year.py` & `leeger-2.5.0/test/test_model/test_league/test_Year.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,139 +1,208 @@
 import unittest
 
 from leeger.enum.MatchupType import MatchupType
 from leeger.exception import DoesNotExistException
 from leeger.model.league import YearSettings
+from leeger.model.league.Division import Division
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from test.helper.prototypes import getNDefaultOwnersAndTeams
 
 
 class TestYear(unittest.TestCase):
     def test_year_init(self):
         week = Week(weekNumber=1, matchups=[])
         team = Team(ownerId="", name="")
+        division = Division(name="")
         yearSettings = YearSettings(leagueMedianGames=True)
-        year = Year(yearNumber=2000, teams=[team], weeks=[week], yearSettings=yearSettings)
+        year = Year(
+            yearNumber=2000,
+            teams=[team],
+            weeks=[week],
+            divisions=[division],
+            yearSettings=yearSettings,
+        )
 
         self.assertEqual(2000, year.yearNumber)
         self.assertEqual(1, len(year.teams))
         self.assertEqual(1, len(year.weeks))
         self.assertEqual(week.id, year.weeks[0].id)
         self.assertEqual(team.id, year.teams[0].id)
+        self.assertEqual(division.id, year.divisions[0].id)
         self.assertTrue(year.yearSettings.leagueMedianGames)
 
     def test_year_init_default(self):
         week = Week(weekNumber=1, matchups=[])
         team = Team(ownerId="", name="")
         year = Year(yearNumber=2000, teams=[team], weeks=[week])
 
         self.assertEqual(2000, year.yearNumber)
         self.assertEqual(1, len(year.teams))
         self.assertEqual(1, len(year.weeks))
         self.assertEqual(week.id, year.weeks[0].id)
         self.assertEqual(team.id, year.teams[0].id)
         self.assertEqual(YearSettings(), year.yearSettings)
+        self.assertEqual(list(), year.divisions)
+
+    def test_year_eq_callsEqualsMethod(self):
+        # create Year 1
+        _, teams_1 = getNDefaultOwnersAndTeams(2)
+
+        matchup_1 = Matchup(
+            teamAId=teams_1[0].id,
+            teamBId=teams_1[1].id,
+            teamAScore=1.1,
+            teamBScore=2.2,
+            matchupType=MatchupType.REGULAR_SEASON,
+        )
+        week_1 = Week(weekNumber=1, matchups=[matchup_1])
+        division_1 = Division(name="div")
+        yearSettings_1 = YearSettings(leagueMedianGames=True)
+        year_1 = Year(
+            yearNumber=2000,
+            teams=teams_1,
+            weeks=[week_1],
+            divisions=[division_1],
+            yearSettings=yearSettings_1,
+        )
+
+        # create Year 2
+        _, teams_2 = getNDefaultOwnersAndTeams(2)
+
+        matchup_2 = Matchup(
+            teamAId=teams_1[0].id,
+            teamBId=teams_1[1].id,
+            teamAScore=1.1,
+            teamBScore=2.2,
+            matchupType=MatchupType.REGULAR_SEASON,
+        )
+        week_2 = Week(weekNumber=1, matchups=[matchup_2])
+        division_2 = Division(name="div")
+        yearSettings_2 = YearSettings(leagueMedianGames=True)
+        year_2 = Year(
+            yearNumber=2000,
+            teams=teams_2,
+            weeks=[week_2],
+            divisions=[division_2],
+            yearSettings=yearSettings_2,
+        )
+
+        year_2.id = year_1.id
+        division_2.id = division_1.id
+        week_2.id = week_1.id
+        matchup_2.id = matchup_1.id
+        teams_2[0].id = teams_1[0].id
+        teams_2[1].id = teams_1[1].id
+        teams_2[0].ownerId = teams_1[0].ownerId
+        teams_2[1].ownerId = teams_1[1].ownerId
+
+        self.assertTrue(year_1 == year_2)
 
     def test_year_eq_equal(self):
         # create Year 1
-        owners_1, teams_1 = getNDefaultOwnersAndTeams(2)
+        _, teams_1 = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
             teamBId=teams_1[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_1 = Week(weekNumber=1, matchups=[matchup_1])
+        division_1 = Division(name="div")
         yearSettings_1 = YearSettings(leagueMedianGames=True)
-        year_1 = Year(yearNumber=2000, teams=teams_1, weeks=[week_1], yearSettings=yearSettings_1)
+        year_1 = Year(
+            yearNumber=2000,
+            teams=teams_1,
+            weeks=[week_1],
+            divisions=[division_1],
+            yearSettings=yearSettings_1,
+        )
 
         # create Year 2
-        owners_2, teams_2 = getNDefaultOwnersAndTeams(2)
+        _, teams_2 = getNDefaultOwnersAndTeams(2)
 
         matchup_2 = Matchup(
             teamAId=teams_2[0].id,
             teamBId=teams_2[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_2 = Week(weekNumber=1, matchups=[matchup_2])
+        division_2 = Division(name="div")
         yearSettings_2 = YearSettings(leagueMedianGames=True)
-        year_2 = Year(yearNumber=2000, teams=teams_2, weeks=[week_2], yearSettings=yearSettings_2)
+        year_2 = Year(
+            yearNumber=2000,
+            teams=teams_2,
+            weeks=[week_2],
+            divisions=[division_2],
+            yearSettings=yearSettings_2,
+        )
 
-        self.assertEqual(year_1, year_2)
+        self.assertTrue(year_1.equals(year_2, ignoreIds=True, ignoreBaseIds=True))
 
     def test_year_eq_notEqual(self):
         # create Year 1
-        owners_1, teams_1 = getNDefaultOwnersAndTeams(2)
+        _, teams_1 = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams_1[0].id,
             teamBId=teams_1[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_1 = Week(weekNumber=1, matchups=[matchup_1])
         year_1 = Year(yearNumber=2000, teams=teams_1, weeks=[week_1])
 
         # create Year 2
-        owners_2, teams_2 = getNDefaultOwnersAndTeams(2)
+        _, teams_2 = getNDefaultOwnersAndTeams(2)
 
         matchup_2 = Matchup(
             teamAId=teams_2[0].id,
             teamBId=teams_2[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_2 = Week(weekNumber=1, matchups=[matchup_2])
         year_2 = Year(yearNumber=2001, teams=teams_2, weeks=[week_2])
 
         self.assertNotEqual(year_1, year_2)
 
-    def test_year_toJson(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+    def test_toFromJson(self):
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_1 = Week(weekNumber=1, matchups=[matchup_1])
+        division_1 = Division(name="div")
         yearSettings = YearSettings(leagueMedianGames=True)
-        year = Year(yearNumber=2000, teams=teams, weeks=[week_1], yearSettings=yearSettings)
-        yearJson = year.toJson()
+        year = Year(
+            yearNumber=2000,
+            teams=teams,
+            weeks=[week_1],
+            divisions=[division_1],
+            yearSettings=yearSettings,
+        )
 
-        self.assertIsInstance(yearJson, dict)
-        self.assertEqual(2000, yearJson["yearNumber"])
-        self.assertEqual(2, len(yearJson["teams"]))
-        self.assertEqual("1", yearJson["teams"][0]["name"])
-        self.assertEqual("2", yearJson["teams"][1]["name"])
-        self.assertEqual(1, len(yearJson["weeks"]))
-        self.assertEqual(1, yearJson["weeks"][0]["weekNumber"])
-        self.assertEqual(1, len(yearJson["weeks"][0]["matchups"]))
-        self.assertEqual(teams[0].id, yearJson["weeks"][0]["matchups"][0]["teamAId"])
-        self.assertEqual(teams[1].id, yearJson["weeks"][0]["matchups"][0]["teamBId"])
-        self.assertEqual(1.1, yearJson["weeks"][0]["matchups"][0]["teamAScore"])
-        self.assertEqual(2.2, yearJson["weeks"][0]["matchups"][0]["teamBScore"])
-        self.assertEqual("REGULAR_SEASON", yearJson["weeks"][0]["matchups"][0]["matchupType"])
-        self.assertFalse(yearJson["weeks"][0]["matchups"][0]["teamAHasTiebreaker"])
-        self.assertFalse(yearJson["weeks"][0]["matchups"][0]["teamBHasTiebreaker"])
-        self.assertTrue(yearJson["yearSettings"]["leagueMedianGames"])
+        self.assertEqual(year, Year.fromJson(year.toJson()))
 
     def test_getTeamByName_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         teams[0].name = "team0"
         matchup_1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
@@ -142,15 +211,15 @@
         week_1 = Week(weekNumber=1, matchups=[matchup_1])
         year = Year(yearNumber=2000, teams=teams, weeks=[week_1])
 
         response = year.getTeamByName("team0")
         self.assertEqual(teams[0], response)
 
     def test_getTeamByName_teamNotInYear_raisesException(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
@@ -159,15 +228,15 @@
         year = Year(yearNumber=2000, teams=teams, weeks=[week_1])
 
         with self.assertRaises(DoesNotExistException) as context:
             year.getTeamByName("team0")
         self.assertEqual("Year does not have a team with name 'team0'.", str(context.exception))
 
     def test_getWeekByWeekNumber_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
@@ -175,47 +244,22 @@
         week_1 = Week(weekNumber=1, matchups=[matchup_1])
         year = Year(yearNumber=2000, teams=teams, weeks=[week_1])
 
         response = year.getWeekByWeekNumber(1)
         self.assertEqual(week_1, response)
 
     def test_getWeekByWeekNumber_teamNotInYear_raisesException(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup_1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1.1,
             teamBScore=2.2,
             matchupType=MatchupType.REGULAR_SEASON,
         )
         week_1 = Week(weekNumber=1, matchups=[matchup_1])
         year = Year(yearNumber=2000, teams=teams, weeks=[week_1])
 
         with self.assertRaises(DoesNotExistException) as context:
             year.getWeekByWeekNumber(2)
         self.assertEqual("Year does not have a week with week number 2.", str(context.exception))
-
-    def test_year_fromJson(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
-
-        matchup_1 = Matchup(
-            teamAId=teams[0].id,
-            teamBId=teams[1].id,
-            teamAScore=1.1,
-            teamBScore=2.2,
-            matchupType=MatchupType.REGULAR_SEASON,
-        )
-        week_1 = Week(weekNumber=1, matchups=[matchup_1])
-        yearSettings = YearSettings(leagueMedianGames=True)
-        year = Year(yearNumber=2000, teams=teams, weeks=[week_1], yearSettings=yearSettings)
-        yearJson = year.toJson()
-        yearDerived = Year.fromJson(yearJson)
-        self.assertEqual(year, yearDerived)
-        self.assertEqual(year.id, yearDerived.id)
-
-        # without year settings
-        year = Year(yearNumber=2000, teams=teams, weeks=[week_1])
-        yearJson = year.toJson()
-        yearDerived = Year.fromJson(yearJson)
-        self.assertEqual(year, yearDerived)
-        self.assertEqual(year.id, yearDerived.id)
```

### Comparing `leeger-2.4.0/test/test_model/test_league/test_YearSettings.py` & `leeger-2.5.0/test/test_model/test_league/test_YearSettings.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,31 +15,40 @@
         self.assertFalse(yearSettings.leagueMedianGames)
 
     def test_yearSettings_init_default_2(self):
         yearSettings = YearSettings(leagueMedianGames=None)
 
         self.assertFalse(yearSettings.leagueMedianGames)
 
+    def test_yearSettings_eq_callsEqualsMethod(self):
+        # create yearSettings 1
+        yearSettings_1 = YearSettings(leagueMedianGames=True)
+
+        # create yearSettings 2
+        yearSettings_2 = YearSettings(leagueMedianGames=True)
+
+        self.assertTrue(yearSettings_1 == yearSettings_2)
+
     def test_yearSettings_eq_equal(self):
         # create yearSettings 1
         yearSettings_1 = YearSettings(leagueMedianGames=True)
 
         # create yearSettings 2
         yearSettings_2 = YearSettings(leagueMedianGames=True)
 
-        self.assertEqual(yearSettings_1, yearSettings_2)
+        self.assertTrue(yearSettings_1.equals(yearSettings_2))
 
     def test_yearSettings_eq_notEqual(self):
         # create yearSettings 1
         yearSettings_1 = YearSettings(leagueMedianGames=True)
 
         # create yearSettings 2
         yearSettings_2 = YearSettings(leagueMedianGames=False)
 
-        self.assertNotEqual(yearSettings_1, yearSettings_2)
+        self.assertFalse(yearSettings_1.equals(yearSettings_2))
 
     def test_yearSettings_toJson(self):
         yearSettings = YearSettings(leagueMedianGames=True)
         yearSettingsJson = yearSettings.toJson()
 
         self.assertIsInstance(yearSettingsJson, dict)
         self.assertTrue(yearSettingsJson["leagueMedianGames"])
```

### Comparing `leeger-2.4.0/test/test_model/test_league_helper/test_Performance.py` & `leeger-2.5.0/test/test_model/test_league_helper/test_Performance.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,36 +28,48 @@
 
         self.assertEqual("teamId", performance.teamId)
         self.assertEqual(1.1, performance.teamScore)
         self.assertEqual(MatchupType.REGULAR_SEASON, performance.matchupType)
         self.assertFalse(performance.hasTiebreaker)
         self.assertIsNone(performance.multiWeekMatchupId)
 
+    def test_performance_eq_callsEqualsMethod(self):
+        # create Performance 1
+        _, teams_1 = getNDefaultOwnersAndTeams(2)
+        performance_1 = Performance(
+            teamId=teams_1[0].id,
+            teamScore=1.1,
+            hasTiebreaker=True,
+            multiWeekMatchupId="1",
+            matchupType=MatchupType.REGULAR_SEASON,
+        )
+
+        self.assertTrue(performance_1 == performance_1)
+
     def test_performance_eq_equal(self):
         # create Performance 1
         _, teams_1 = getNDefaultOwnersAndTeams(2)
         performance_1 = Performance(
             teamId=teams_1[0].id,
             teamScore=1.1,
             hasTiebreaker=True,
             multiWeekMatchupId="1",
             matchupType=MatchupType.REGULAR_SEASON,
         )
 
         # create Matchup 2
-        _, teams_2 = getNDefaultOwnersAndTeams(2)
         performance_2 = Performance(
-            teamId=teams_2[0].id,
+            teamId=teams_1[0].id,
             teamScore=1.1,
             hasTiebreaker=True,
             multiWeekMatchupId="1",
             matchupType=MatchupType.REGULAR_SEASON,
         )
 
-        self.assertEqual(performance_1, performance_2)
+        self.assertTrue(performance_1.equals(performance_2, ignoreBaseIds=True))
 
     def test_performance_eq_notEqual(self):
         # create Performance 1
         _, teams_1 = getNDefaultOwnersAndTeams(2)
         performance_1 = Performance(
             teamId=teams_1[0].id,
             teamScore=1.1,
@@ -72,15 +84,15 @@
             teamId=teams_2[0].id,
             teamScore=1.1,
             hasTiebreaker=True,
             multiWeekMatchupId="1",
             matchupType=MatchupType.REGULAR_SEASON,
         )
 
-        self.assertNotEqual(performance_1, performance_2)
+        self.assertFalse(performance_1.equals(performance_2, ignoreBaseIds=True))
 
     def test_performance_toJson(self):
         performance = Performance(
             teamId="teamId",
             teamScore=1.1,
             matchupType=MatchupType.PLAYOFF,
             hasTiebreaker=True,
```

### Comparing `leeger-2.4.0/test/test_util/test_GeneralUtil.py` & `leeger-2.5.0/test/test_util/test_GeneralUtil.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,28 @@
         kwargs = {"a": 1, "b": 2}
         with self.assertLogs() as captured:
             GeneralUtil.warnForUnusedKwargs(kwargs)
         self.assertEqual(2, len(captured.records))
         self.assertEqual("Keyword argument 'a' unused.", captured.records[0].getMessage())
         self.assertEqual("Keyword argument 'b' unused.", captured.records[1].getMessage())
 
+        # with default exclude keys
+        kwargs = {"b": 1, "validate": 2}
+        with self.assertLogs() as captured:
+            GeneralUtil.warnForUnusedKwargs(kwargs)
+        self.assertEqual(1, len(captured.records))
+        self.assertEqual("Keyword argument 'b' unused.", captured.records[0].getMessage())
+
+        # with exclude keys
+        kwargs = {"a": 1, "b": 2}
+        with self.assertLogs() as captured:
+            GeneralUtil.warnForUnusedKwargs(kwargs, excludeKeys=["a"])
+        self.assertEqual(1, len(captured.records))
+        self.assertEqual("Keyword argument 'b' unused.", captured.records[0].getMessage())
+
     def test_safeSum_happyPath(self):
         response = GeneralUtil.safeSum(None, 1, 1)
         self.assertEqual(2, response)
 
         response = GeneralUtil.safeSum(1, None, 1)
         self.assertEqual(2, response)
```

### Comparing `leeger-2.4.0/test/test_util/test_excel.py` & `leeger-2.5.0/test/test_util/test_excel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 import os
 import tempfile
 import unittest
 from decimal import Decimal
 
 from openpyxl import load_workbook
 from openpyxl.utils import get_column_letter
+from leeger.model.league.Division import Division
 
 from leeger.model.league.League import League
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from leeger.util.excel import leagueToExcel
 from test.helper.prototypes import getNDefaultOwnersAndTeams
 
 
 class TestExcel(unittest.TestCase):
     def test_leagueToExcel_filePathGiven_happyPath(self):
+        division1 = Division(name="d1")
+        division2 = Division(name="d2")
         owners, teams1 = getNDefaultOwnersAndTeams(2)
         teams1[0].name = "a"
         teams1[1].name = "b"
+        teams1[0].divisionId = division1.id
+        teams1[1].divisionId = division2.id
         matchup1 = Matchup(teamAId=teams1[0].id, teamBId=teams1[1].id, teamAScore=1, teamBScore=2)
         week1 = Week(weekNumber=1, matchups=[matchup1])
-        year1 = Year(yearNumber=2000, teams=teams1, weeks=[week1])
+        year1 = Year(yearNumber=2000, teams=teams1, weeks=[week1], divisions=[division1, division2])
 
         teams2 = [Team(ownerId=owners[0].id, name="a2"), Team(ownerId=owners[1].id, name="b2")]
         matchup2 = Matchup(teamAId=teams2[0].id, teamBId=teams2[1].id, teamAScore=1, teamBScore=2)
         week2 = Week(weekNumber=1, matchups=[matchup2])
         year2 = Year(yearNumber=2001, teams=teams2, weeks=[week2])
 
         teams3 = [Team(ownerId=owners[0].id, name="a3"), Team(ownerId=owners[1].id, name="b3")]
@@ -56,14 +61,15 @@
             self.assertEqual("All Time Owners", workbook.sheetnames[8])
 
             # check sheet values
             # test year worksheet values
             worksheet2000TeamValues = [
                 [
                     "Team",
+                    "Division",
                     "Games Played",
                     "Wins",
                     "Losses",
                     "Ties",
                     "Win Percentage",
                     "WAL",
                     "WAL Per Game",
@@ -89,14 +95,15 @@
                     "Plus/Minus",
                     "Team Score",
                     "Team Success",
                     "Team Luck",
                 ],
                 [
                     "a",
+                    "d1",
                     1,
                     0,
                     1,
                     0,
                     0,
                     0,
                     0,
@@ -122,14 +129,15 @@
                     -1,
                     66.76666666666667,
                     66.76666666666667,
                     0,
                 ],
                 [
                     "b",
+                    "d2",
                     1,
                     1,
                     0,
                     0,
                     1,
                     1,
                     1,
@@ -432,14 +440,15 @@
             # test all time teams worksheet values
             allTimeTeamsWorksheet = workbook["All Time Teams"]
 
             allTimeTeamsValues = [
                 [
                     "Team",
                     "Owner",
+                    "Division",
                     "Year",
                     "Games Played",
                     "Wins",
                     "Losses",
                     "Ties",
                     "Win Percentage",
                     "WAL",
@@ -467,14 +476,15 @@
                     "Team Score",
                     "Team Success",
                     "Team Luck",
                 ],
                 [
                     "a",
                     "1",
+                    "d1",
                     2000,
                     1,
                     0,
                     1,
                     0,
                     0,
                     0,
@@ -502,14 +512,15 @@
                     66.76666666666667,
                     66.76666666666667,
                     0,
                 ],
                 [
                     "b",
                     "2",
+                    "d2",
                     2000,
                     1,
                     1,
                     0,
                     0,
                     1,
                     1,
@@ -537,14 +548,15 @@
                     233.5333333333333,
                     233.5333333333333,
                     0,
                 ],
                 [
                     "a2",
                     "1",
+                    "N/A",
                     2001,
                     1,
                     0,
                     1,
                     0,
                     0,
                     0,
@@ -572,14 +584,15 @@
                     66.76666666666667,
                     66.76666666666667,
                     0,
                 ],
                 [
                     "b2",
                     "2",
+                    "N/A",
                     2001,
                     1,
                     1,
                     0,
                     0,
                     1,
                     1,
@@ -607,14 +620,15 @@
                     233.5333333333333,
                     233.5333333333333,
                     0,
                 ],
                 [
                     "a3",
                     "1",
+                    "N/A",
                     2002,
                     1,
                     0,
                     1,
                     0,
                     0,
                     0,
@@ -642,14 +656,15 @@
                     66.76666666666667,
                     66.76666666666667,
                     0,
                 ],
                 [
                     "b3",
                     "2",
+                    "N/A",
                     2002,
                     1,
                     1,
                     0,
                     0,
                     1,
                     1,
```

### Comparing `leeger-2.4.0/test/test_util/test_excel_helper.py` & `leeger-2.5.0/test/test_util/test_excel_helper.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_util/test_navigator/test_LeagueNavigator.py` & `leeger-2.5.0/test/test_util/test_navigator/test_LeagueNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_util/test_navigator/test_MatchupNavigator.py` & `leeger-2.5.0/test/test_util/test_navigator/test_MatchupNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_util/test_navigator/test_WeekNavigator.py` & `leeger-2.5.0/test/test_util/test_navigator/test_WeekNavigator.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_util/test_navigator/test_YearNavigator.py` & `leeger-2.5.0/test/test_util/test_navigator/test_YearNavigator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,58 @@
 import unittest
 
 from leeger.enum.MatchupType import MatchupType
+from leeger.exception.DoesNotExistException import DoesNotExistException
 from leeger.model.filter.YearFilters import YearFilters
 from leeger.model.league import YearSettings
+from leeger.model.league.Division import Division
 from leeger.model.league.Matchup import Matchup
 from leeger.model.league.Owner import Owner
 from leeger.model.league.Team import Team
 from leeger.model.league.Week import Week
 from leeger.model.league.Year import Year
 from leeger.util.navigator.YearNavigator import YearNavigator
 from test.helper.prototypes import getNDefaultOwnersAndTeams
 
 
 class TestYearNavigator(unittest.TestCase):
+    def test_getTeamById_happyPath(self):
+        team = Team(ownerId="oid", name="t1")
+        year = Year(yearNumber=2000, teams=[team], weeks=list())
+
+        response = YearNavigator.getTeamById(year, team.id)
+        self.assertTrue(team.equals(response))
+
+    def test_getTeamById_notFound_raisesException(self):
+        team = Team(ownerId="oid", name="t1")
+        year = Year(yearNumber=2000, teams=[team], weeks=list())
+
+        with self.assertRaises(DoesNotExistException) as context:
+            YearNavigator.getTeamById(year, "badId")
+        self.assertEqual(
+            "Team with ID 'badId' does not exist in the given Year.", str(context.exception)
+        )
+
+    def test_getDivisionById_happyPath(self):
+        division = Division(name="d1")
+        year = Year(yearNumber=2000, divisions=[division], teams=list(), weeks=list())
+
+        response = YearNavigator.getDivisionById(year, division.id)
+        self.assertTrue(division.equals(response))
+
+    def test_getDivisionById_notFound_raisesException(self):
+        division = Division(name="d1")
+        year = Year(yearNumber=2000, divisions=[division], teams=list(), weeks=list())
+
+        with self.assertRaises(DoesNotExistException) as context:
+            YearNavigator.getDivisionById(year, "badId")
+        self.assertEqual(
+            "Division with ID 'badId' does not exist in the given Year.", str(context.exception)
+        )
+
     def test_getYearByYearNumber_happyPath(self):
         owner1 = Owner(name="1")
         owner2 = Owner(name="2")
 
         a_team1 = Team(ownerId=owner1.id, name="1")
         a_team2 = Team(ownerId=owner2.id, name="2")
 
@@ -57,15 +93,15 @@
 
         self.assertIsInstance(response, list)
         self.assertEqual(2, len(response))
         self.assertEqual(a_team1.id, response[0])
         self.assertEqual(a_team2.id, response[1])
 
     def test_getNumberOfGamesPlayed_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         matchup2 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
 
         week1 = Week(weekNumber=1, matchups=[matchup1])
         week2 = Week(weekNumber=2, matchups=[matchup2])
 
@@ -78,15 +114,15 @@
         self.assertEqual(2, len(response.keys()))
         self.assertEqual(2, response[teams[0].id])
         self.assertEqual(2, response[teams[1].id])
 
     def test_getNumberOfGamesPlayed_countLeagueMedianGamesAsTwoGames_countsLeagueMedianGamesAsTwoGames(
         self,
     ):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         matchup2 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
 
         week1 = Week(weekNumber=1, matchups=[matchup1])
         week2 = Week(weekNumber=2, matchups=[matchup2])
 
@@ -102,15 +138,15 @@
         self.assertEqual(2, len(response.keys()))
         self.assertEqual(4, response[teams[0].id])
         self.assertEqual(4, response[teams[1].id])
 
     def test_getNumberOfGamesPlayed_countMultiWeekMatchupsAsOneGameIsTrue_countsMultiWeekMatchupsAsOneGame(
         self,
     ):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             multiWeekMatchupId="1",
@@ -137,15 +173,15 @@
         self.assertEqual(2, len(response.keys()))
         self.assertEqual(1, response[teams[0].id])
         self.assertEqual(1, response[teams[1].id])
 
     def test_getNumberOfGamesPlayed_countMultiWeekMatchupsAsOneGameIsFalse_countsMultiWeekMatchupsAsMultipleGames(
         self,
     ):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             multiWeekMatchupId="1",
@@ -170,15 +206,15 @@
 
         self.assertIsInstance(response, dict)
         self.assertEqual(2, len(response.keys()))
         self.assertEqual(2, response[teams[0].id])
         self.assertEqual(2, response[teams[1].id])
 
     def test_getNumberOfGamesPlayed_onlyPostSeasonIsTrue(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         matchup2 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
@@ -203,15 +239,15 @@
 
         self.assertIsInstance(response, dict)
         self.assertEqual(2, len(response.keys()))
         self.assertEqual(2, response[teams[0].id])
         self.assertEqual(2, response[teams[1].id])
 
     def test_getNumberOfGamesPlayed_onlyRegularSeasonIsTrue(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         matchup2 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
@@ -236,15 +272,15 @@
 
         self.assertIsInstance(response, dict)
         self.assertEqual(2, len(response.keys()))
         self.assertEqual(1, response[teams[0].id])
         self.assertEqual(1, response[teams[1].id])
 
     def test_getNumberOfGamesPlayed_weekNumberStartGiven(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         matchup2 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
@@ -269,15 +305,15 @@
 
         self.assertIsInstance(response, dict)
         self.assertEqual(2, len(response.keys()))
         self.assertEqual(2, response[teams[0].id])
         self.assertEqual(2, response[teams[1].id])
 
     def test_getNumberOfGamesPlayed_weekNumberEndGiven(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         matchup2 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
@@ -302,15 +338,15 @@
 
         self.assertIsInstance(response, dict)
         self.assertEqual(2, len(response.keys()))
         self.assertEqual(2, response[teams[0].id])
         self.assertEqual(2, response[teams[1].id])
 
     def test_getNumberOfGamesPlayed_weekNumberStartGivenAndWeekNumberEndGiven(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         matchup2 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
@@ -343,15 +379,15 @@
 
         self.assertIsInstance(response, dict)
         self.assertEqual(2, len(response.keys()))
         self.assertEqual(2, response[teams[0].id])
         self.assertEqual(2, response[teams[1].id])
 
     def test_getAllScoresInYear_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         matchup2 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=3,
             teamBScore=4,
@@ -368,15 +404,15 @@
         response = YearNavigator.getAllScoresInYear(year)
 
         self.assertIsInstance(response, list)
         self.assertEqual(4, len(response))
         self.assertEqual([1, 2, 5, 6], sorted(response))
 
     def test_getAllScoresInYear_simplifyMultiWeekMatchupsIsTrue(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             multiWeekMatchupId="1",
@@ -399,15 +435,15 @@
         response = YearNavigator.getAllScoresInYear(year, simplifyMultiWeekMatchups=True)
 
         self.assertIsInstance(response, list)
         self.assertEqual(4, len(response))
         self.assertEqual([4, 5, 6, 6], sorted(response))
 
     def test_getAllMultiWeekMatchups_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             multiWeekMatchupId="1",
@@ -440,15 +476,15 @@
         self.assertIsInstance(response["1"], list)
         self.assertEqual(3, len(response["1"]))
         self.assertEqual(matchup1.id, response["1"][0].id)
         self.assertEqual(matchup2.id, response["1"][1].id)
         self.assertEqual(matchup3.id, response["1"][2].id)
 
     def test_getAllMultiWeekMatchups_noMultiWeekMatchupsFound_returnsEmptyDict(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         matchup2 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=3, teamBScore=4)
         matchup3 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=5, teamBScore=6)
 
         week1 = Week(weekNumber=1, matchups=[matchup1])
         week2 = Week(weekNumber=2, matchups=[matchup2])
@@ -473,15 +509,15 @@
                 ),
             )
         self.assertEqual(
             "Multi-Week matchups must be included in this calculation.", str(context.exception)
         )
 
     def test_getAllMatchupsInYear_noFilterGiven_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         a_matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         a_matchup2 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
@@ -516,15 +552,15 @@
         self.assertEqual(4, len(response))
         self.assertEqual(a_matchup1.id, response[0].id)
         self.assertEqual(a_matchup2.id, response[1].id)
         self.assertEqual(a_matchup3.id, response[2].id)
         self.assertEqual(a_matchup4.id, response[3].id)
 
     def test_getAllMatchupsInYear_filterGiven_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         a_matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         a_matchup2 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         a_matchup3 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
@@ -552,15 +588,15 @@
         )
 
         self.assertIsInstance(response, list)
         self.assertEqual(1, len(response))
         self.assertEqual(a_matchup3.id, response[0].id)
 
     def test_getAllMatchupsInYear_filterGiven_includeMultiWeekMatchupsIsTrue_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         a_matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             multiWeekMatchupId="1",
@@ -593,15 +629,15 @@
         self.assertIsInstance(response, list)
         self.assertEqual(3, len(response))
         self.assertEqual(a_matchup1.id, response[0].id)
         self.assertEqual(a_matchup2.id, response[1].id)
         self.assertEqual(a_matchup3.id, response[2].id)
 
     def test_getAllMatchupsInYear_filterGiven_includeMultiWeekMatchupsIsFalse_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         a_matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             multiWeekMatchupId="1",
@@ -632,15 +668,15 @@
         )
 
         self.assertIsInstance(response, list)
         self.assertEqual(1, len(response))
         self.assertEqual(a_matchup3.id, response[0].id)
 
     def test_getAllSimplifiedMatchupsInYear_noFilterGiven_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         a_matchup1 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
             multiWeekMatchupId="1",
@@ -667,15 +703,15 @@
         self.assertEqual(a_matchup3.id, response[0].id)
         self.assertEqual(teams[0].id, response[1].teamAId)
         self.assertEqual(teams[1].id, response[1].teamBId)
         self.assertEqual(2, response[1].teamAScore)
         self.assertEqual(4, response[1].teamBScore)
 
     def test_getAllSimplifiedMatchupsInYear_filterGiven_happyPath(self):
-        owners, teams = getNDefaultOwnersAndTeams(2)
+        _, teams = getNDefaultOwnersAndTeams(2)
 
         a_matchup1 = Matchup(teamAId=teams[0].id, teamBId=teams[1].id, teamAScore=1, teamBScore=2)
         a_matchup2 = Matchup(
             teamAId=teams[0].id,
             teamBId=teams[1].id,
             teamAScore=1,
             teamBScore=2,
```

### Comparing `leeger-2.4.0/test/test_util/test_stat_sheet.py` & `leeger-2.5.0/test/test_util/test_stat_sheet.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_validate/test_leagueValidation.py` & `leeger-2.5.0/test/test_validate/test_leagueValidation.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,15 +189,27 @@
 
     def test_checkAllTypes_leagueNameIsntTypeString_raisesException(self):
         with self.assertRaises(InvalidLeagueFormatException) as context:
             leagueValidation.checkAllTypes(League(name=None, owners=list(), years=list()))
         self.assertEqual("name must be type 'str'.", str(context.exception))
 
     def test_checkAllTypes_leagueOwnersIsntTypeList_raisesException(self):
+        # not given a list
         with self.assertRaises(InvalidLeagueFormatException) as context:
             leagueValidation.checkAllTypes(League(name="TEST", owners=None, years=list()))
-        self.assertEqual("owners must be type 'list'.", str(context.exception))
+        self.assertEqual("owners must be type 'list[Owner]'.", str(context.exception))
+
+        # given a list of non Owner
+        with self.assertRaises(InvalidLeagueFormatException) as context:
+            leagueValidation.checkAllTypes(League(name="TEST", owners=["foo"], years=list()))
+        self.assertEqual("owners must be type 'list[Owner]'.", str(context.exception))
 
     def test_checkAllTypes_leagueYearsIsntTypeList_raisesException(self):
+        # not given a list
         with self.assertRaises(InvalidLeagueFormatException) as context:
             leagueValidation.checkAllTypes(League(name="TEST", owners=list(), years=None))
-        self.assertEqual("years must be type 'list'.", str(context.exception))
+        self.assertEqual("years must be type 'list[Year]'.", str(context.exception))
+
+        # given a list of non Year
+        with self.assertRaises(InvalidLeagueFormatException) as context:
+            leagueValidation.checkAllTypes(League(name="TEST", owners=list(), years=["foo"]))
+        self.assertEqual("years must be type 'list[Year]'.", str(context.exception))
```

### Comparing `leeger-2.4.0/test/test_validate/test_matchupValidation.py` & `leeger-2.5.0/test/test_validate/test_matchupValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_validate/test_ownerValidation.py` & `leeger-2.5.0/test/test_validate/test_ownerValidation.py`

 * *Files identical despite different names*

### Comparing `leeger-2.4.0/test/test_validate/test_teamValidation.py` & `leeger-2.5.0/test/test_validate/test_teamValidation.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,7 +11,12 @@
             teamValidation.checkAllTypes(Team(ownerId=None, name="team"))
         self.assertEqual("ownerId must be type 'str'.", str(context.exception))
 
     def test_checkAllTypes_teamNameIsntTypeStr_raisesException(self):
         with self.assertRaises(InvalidTeamFormatException) as context:
             teamValidation.checkAllTypes(Team(ownerId="id", name=None))
         self.assertEqual("name must be type 'str'.", str(context.exception))
+
+    def test_checkAllTypes_divisionIdIsntTypeStrOrNone_raisesException(self):
+        with self.assertRaises(InvalidTeamFormatException) as context:
+            teamValidation.checkAllTypes(Team(ownerId="id", name="team", divisionId=1))
+        self.assertEqual("divisionId must be 'None' or type 'str'.", str(context.exception))
```

### Comparing `leeger-2.4.0/test/test_validate/test_weekValidation.py` & `leeger-2.5.0/test/test_validate/test_weekValidation.py`

 * *Files 12% similar despite different names*

```diff
@@ -128,10 +128,16 @@
 
     def test_checkAllTypes_weekNumberIsntTypeInt_raisesException(self):
         with self.assertRaises(InvalidWeekFormatException) as context:
             weekValidation.checkAllTypes(Week(weekNumber=None, matchups=list()))
         self.assertEqual("weekNumber must be type 'int'.", str(context.exception))
 
     def test_checkAllTypes_weekMatchupsIsntTypeList_raisesException(self):
+        # not given a list
         with self.assertRaises(InvalidWeekFormatException) as context:
             weekValidation.checkAllTypes(Week(weekNumber=1, matchups=None))
-        self.assertEqual("matchups must be type 'list'.", str(context.exception))
+        self.assertEqual("matchups must be type 'list[Matchup]'.", str(context.exception))
+
+        # given a list of non Matchup
+        with self.assertRaises(InvalidWeekFormatException) as context:
+            weekValidation.checkAllTypes(Week(weekNumber=1, matchups=["foo"]))
+        self.assertEqual("matchups must be type 'list[Matchup]'.", str(context.exception))
```

### Comparing `leeger-2.4.0/test/test_validate/test_yearSettingsValidation.py` & `leeger-2.5.0/test/test_validate/test_yearSettingsValidation.py`

 * *Files identical despite different names*

