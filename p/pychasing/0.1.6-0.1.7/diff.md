# Comparing `tmp/pychasing-0.1.6.tar.gz` & `tmp/pychasing-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pychasing-0.1.6.tar", last modified: Wed Jan  4 19:15:40 2023, max compression
+gzip compressed data, was "pychasing-0.1.7.tar", last modified: Sun Jun  4 03:55:46 2023, max compression
```

## Comparing `pychasing-0.1.6.tar` & `pychasing-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-04 19:15:40.950369 pychasing-0.1.6/
--rw-rw-rw-   0        0        0     1096 2022-09-28 19:13:29.000000 pychasing-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     6320 2023-01-04 19:15:40.949371 pychasing-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5822 2022-11-22 23:22:42.000000 pychasing-0.1.6/README.md
--rw-rw-rw-   0        0        0      710 2023-01-04 19:15:01.000000 pychasing-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-04 19:15:40.950369 pychasing-0.1.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-01-04 19:15:40.896513 pychasing-0.1.6/src/
-drwxrwxrwx   0        0        0        0 2023-01-04 19:15:40.916460 pychasing-0.1.6/src/pychasing/
--rw-rw-rw-   0        0        0     1443 2023-01-04 19:15:03.000000 pychasing-0.1.6/src/pychasing/__init__.py
--rw-rw-rw-   0        0        0    41131 2023-01-04 17:54:01.000000 pychasing-0.1.6/src/pychasing/client.py
--rw-rw-rw-   0        0        0     9385 2022-12-04 20:59:29.000000 pychasing-0.1.6/src/pychasing/enums.py
--rw-rw-rw-   0        0        0     1719 2023-01-04 19:14:40.000000 pychasing-0.1.6/src/pychasing/models.py
-drwxrwxrwx   0        0        0        0 2023-01-04 19:15:40.947377 pychasing-0.1.6/src/pychasing.egg-info/
--rw-rw-rw-   0        0        0     6320 2023-01-04 19:15:40.000000 pychasing-0.1.6/src/pychasing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      313 2023-01-04 19:15:40.000000 pychasing-0.1.6/src/pychasing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-04 19:15:40.000000 pychasing-0.1.6/src/pychasing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-01-04 19:15:40.000000 pychasing-0.1.6/src/pychasing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-01-04 19:15:40.000000 pychasing-0.1.6/src/pychasing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.926287 pychasing-0.1.7/
+-rw-rw-rw-   0        0        0     1101 2023-06-04 03:49:26.000000 pychasing-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     8389 2023-06-04 03:55:46.908335 pychasing-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5817 2023-06-04 03:43:02.000000 pychasing-0.1.7/README.md
+-rw-rw-rw-   0        0        0     1644 2023-06-04 03:54:12.000000 pychasing-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-04 03:55:46.926287 pychasing-0.1.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.555524 pychasing-0.1.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.755563 pychasing-0.1.7/src/pychasing/
+-rw-rw-rw-   0        0        0     1443 2023-06-04 03:33:43.000000 pychasing-0.1.7/src/pychasing/__init__.py
+-rw-rw-rw-   0        0        0    32528 2023-06-04 03:41:03.000000 pychasing-0.1.7/src/pychasing/client.py
+-rw-rw-rw-   0        0        0    11369 2023-06-04 03:33:27.000000 pychasing-0.1.7/src/pychasing/enums.py
+-rw-rw-rw-   0        0        0     1719 2023-01-04 19:14:40.000000 pychasing-0.1.7/src/pychasing/models.py
+drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.877908 pychasing-0.1.7/src/pychasing.egg-info/
+-rw-rw-rw-   0        0        0     8389 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-04 03:55:46.000000 pychasing-0.1.7/src/pychasing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-04 03:55:46.906341 pychasing-0.1.7/tests/
+-rw-rw-rw-   0        0        0     6569 2022-12-04 22:40:02.000000 pychasing-0.1.7/tests/test.py
```

### Comparing `pychasing-0.1.6/LICENSE` & `pychasing-0.1.7/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Tanner B. Corcoran
+Copyright (c) 2022-2023 Tanner B. Corcoran
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pychasing-0.1.6/PKG-INFO` & `pychasing-0.1.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,27 @@
-Metadata-Version: 2.1
-Name: pychasing
-Version: 0.1.6
-Summary: A full-functionality wrapper for the https://ballchasing.com API
-Author-email: "Tanner B. Corcoran" <tannerbcorcoran@gmail.com>
-Project-URL: Homepage, https://github.com/tanrbobanr/pychasing
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 A full-functionality wrapper for the https://ballchasing.com API.
+
 # Install
-`pip install pychasing`
+
+`$ pip install pychasing`
+
 # The pychasing Client
+
 The `pychasing.Client` class is the main object used to interact with the Ballchasing API.
+
 ```py
 import pychasing
 
 pychasing_client = pychasing.Client(
     token="your_token",
     auto_rate_limit=True,
     patreon_tier=pychasing.PatreonTier.none # same as "regular"
 )
 ```
+
 Before we get into the methods of `Client`, there are a few things to note about rate limit handling. If `auto_rate_limit` is set to `False`, any request you make will be immediately sent to the ballchasing API. If `auto_rate_limit` is set to `True`, the client will automatically limit the rate of your requests, taking into account both hourly quota and burst limit. This is done through `time.sleep`, so how long it takes to get a response from a given method will depend on how often you are using the API, as well as your Ballchasing Patreon tier. Additionally, there is a `rate_limit_safe_start` option; if this option is set to `True`, the rate limiting will start off as already maxed out on API calls. This prevents any issues from arising if you are reinstantiating the client often (e.g. if you are testing by running a script multiple times). If this option is set to `False`, the rate limiter will assume that you haven't made any API calls in the past hour, and will rate limit accordingly. For long-running programs and use a single client instance, this option isn't necessarily needed, but I would always recommend it be enabled.
 
 The `pychasing.Client` object has the below methods:
 - `ping` - pings the ballchasing servers.
 - `upload_replay` - uploads a replay to the token-holder's account.
     - NOTE: this takes a `BinaryIO` object. For example:
     ```py
@@ -56,15 +49,17 @@
 - `patch_group` - edit the `player-identification`, `team-identification`, `parent`, or `shared` status of a specific replay group, so long as it owned by the token-holder.
 - `maps` - list all the maps in the game.
 - `get_threejs` - get basic locational data (among other data) of a specific replay. This does not require
     - NOTE: this functionality is highly experimental. It accesses a back-end API used for populating site data (that notably does not require authorization headers). At any time, this API could become restricted or its functionality could change.
 - `get_timeline` - get basic timeline data of a specific replay.
     - NOTE: this functionality is highly experimental. It accesses a back-end API used for populating site data (that notably does not require authorization headers). At any time, this API could become restricted or its functionality could change.
 - `export_csv` - get group statistics formatted as semi-colon-separated values.
+
 # Enums and other types
+
 Many of the methods in `Client` can use custom enumerations for ease of use. For example, when setting the visibility of a replay through `Client.patch_replay`, you could set `visibility` to `"unlisted"` *or* `Visibility.unlisted`. These Enums are listed below:
 - `pychasing.Rank` - used for `min_rank` and `max_rank` in `list_replays`
 - `pychasing.Playlist` - used for `playlists` in `list_replays`
 - `pychasing.Platform` - used for `platform` in `list_replays`
 - `pychasing.Map` - used for `map` in `list_replays`
 - `pychasing.Visibility` - used for `visibility` in `patch_replay` and `patch_group`
 - `pychasing.PlayerIdentifiercation` - used for `player_identification` in `create_group` and `patch_group`
@@ -72,12 +67,13 @@
 - `pychasing.MatchResult` - used for `match_result` in `list_replays`
 - `pychasing.ReplaySortBy` - used for `sort_by` in `list_replays`
 - `pychasing.GroupSortBy` - used for `sort_by` in `list_groups`
 - `pychasing.SortDirection` - used for `sort_dir` in `list_replays` and `list_groups`
 - `pychasing.GroupStats` - used for `stat` in `export_csv`
 - `pychasing.PatreonTier` - used in the initialization of `Client`. This is the only exception to the aforementioned "str or enum" rule above; the proper initialization of `Client` **requires** the `PatreonTier` enum.
 
-Additionally, all date parameters (which require an RFC3339 formatted datetime) also accept a `pychasing.Date`. The usage of the class is as follows:
+Additionally, all date parameters (which require an RFC3339 formatted datetime) also accept a `pychasing.Date`. For example:
+
 ```py
 ...list_replays(created_before="2022-11-22T05:00:30Z")
 ...list_replays(created_before=pychasing.Date(2022, 11, 22, 5, 0, 30)) 
 ```
```

### Comparing `pychasing-0.1.6/src/pychasing/__init__.py` & `pychasing-0.1.7/src/pychasing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 
 __title__ = "pychasing"
 __author__ = "Tanner B. Corcoran"
 __email__ = "tannerbcorcoran@gmail.com"
 __license__ = "MIT License"
 __copyright__ = "Copyright (c) 2022 Tanner B. Corcoran"
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 __description__ = "A full-functionality wrapper for the https://ballchasing.com API"
 __url__ = "https://github.com/tanrbobanr/pychasing"
 __download_url__ = "https://pypi.org/project/pychasing/"
 
 
 __all__ = (
     "Client",
```

### Comparing `pychasing-0.1.6/src/pychasing/client.py` & `pychasing-0.1.7/src/pychasing/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,24 +9,33 @@
 __copyright__ = "Copyright (c) 2022-present Tanner B. Corcoran"
 
 
 from . import models
 from . import enums
 import requests
 import httpprep
-import typing
-import prepr
+import urllib.parse
 import rlim
 import io
+import re
 
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
+from typing import (
+    Union,
+    Tuple,
+    Iterable
+)
+
+
+cont_pat = re.compile(r"(?<=\after=)[^\&]*")
+
 
 def _print_error(response: requests.Response) -> None:
     """Print out an error code from a `requests.Response` if an HTTP error is
     encountered.
     
     """
     error_side = ("Client" if 400 <= response.status_code < 500 else "Server"
@@ -58,161 +67,136 @@
     return v if v == ... or isinstance(v, str) else v.value
 
 
 class Client:
     """The main class used to interact with the Ballchasing API.
     
     """
-    def __init__(self, token: str, auto_rate_limit: bool,
-                 patreon_tier: enums.PatreonTier,
+    def __init__(self, token: str, auto_rate_limit: bool, patreon_tier: enums.PatreonTier,
                  rate_limit_safe_start: bool = False) -> None:
         """
         Arguments
         ---------
         token : str
-            A ballchasing API key (acquirable
-            from https://ballchasing.com/upload).
+            A ballchasing API key (acquirable from https://ballchasing.com/upload).
         auto_rate_limit : bool
-            If `True`, the client will automatically limit API calls according
-            to the given Patreon tier.
+            If `True`, the client will automatically limit API calls according to the given Patreon
+            tier.
         patreon_tier : enums.PatreonTier
             The token-holder's Ballchasing Patreon tier.
         rate_limit_safe_start : bool, optional, default=False
-            If `True`, the rate limiter will start out as fully maxed out on API
-            calls.
+            If `True`, the rate limiter will start out as fully maxed out on API calls.
 
         """
         
         self._token = token
         if auto_rate_limit:
             for k, v in patreon_tier.value.items():
                 rlim.set_rate_limiter(getattr(self, k.name),
-                                      rlim.RateLimiter(*v,
-                                          safestart=rate_limit_safe_start))
-
-    def __repr__(self, *args, **kwargs) -> prepr.pstr:
-        return prepr.prepr(self).args(self._token).build(*args, **kwargs)
+                                      rlim.RateLimiter(*v, safestart=rate_limit_safe_start))
     
     def ping(self, *, print_error: bool = True) -> requests.Response:
         """Ping the https://ballchasing.com servers.
 
         Arguments
         ---------
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare URL
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api"]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api"])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
         
         # make request, print error, and return response
-        response = requests.get(prepped_url.build(), headers=
-                                prepped_headers.format_dict())
+        response = requests.get(prepped_url.build(), headers=prepped_headers.format_dict())
         if print_error:
             _print_error(response)
         return response
 
     def upload_replay(self, file: io.BufferedReader,
-                      visibility: typing.Union[str, enums.Visibility], *, group: str  = ...,
+                      visibility: Union[str, enums.Visibility], *, group: str  = ...,
                       print_error: bool = True) -> requests.Response:
         """Upload a replay to https://ballchasing.com.
 
         Parameters
         ----------
-        file : BinaryIO
+        file : BufferedReader
             The `.replay` file to be uploaded.
         visibility : str or Visibility
             The visibility of the replay once uploaded.
         group : str, optional
             The group to assign this replay to once it is uploaded.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare URL
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "v2", "upload"]
-        )
-        prepped_url.components.queries["visibility", "group"] = [
-                p(visibility), group]
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "v2", "upload"])
+        prepped_url.components.queries["visibility", "group"] = [p(visibility), group]
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
         
         # make request, print error, and return response
         response = requests.post(prepped_url.build(query_check=...),
-                                 headers=prepped_headers.format_dict(),
-                                 files={"file":file})
+                                 headers=prepped_headers.format_dict(), files={"file":file})
         if print_error:
             _print_error(response)
         return response
 
     @rlim.placeholder
-    def list_replays(self, *, next: str = ..., title: str = ...,
-                     player_names: typing.List[str] = ...,
-                     player_ids: typing.List[typing.Tuple[str, typing.Union[
-                        int, str]]] = ...,
-                     playlists: typing.List[typing.Union[str, 
-                        enums.Playlist]] = ...,
-                     season: typing.Union[str, enums.Season] = ...,
-                     match_result: typing.Union[str, enums.MatchResult] = ...,
-                     min_rank: typing.Union[str, enums.Rank] = ...,
-                     max_rank: typing.Union[str, enums.Rank] = ...,
-                     pro: bool = ...,
-                     uploader: typing.Union[Literal["me"], str, int]  = ...,
-                     group: str = ..., map: typing.Union[str, enums.Map] = ...,
-                     created_before: typing.Union[models.Date, str] = ...,
-                     created_after: typing.Union[models.Date, str] = ...,
-                     replay_date_before: typing.Union[models.Date, str] = ...,
-                     replay_date_after: typing.Union[models.Date, str] = ...,
-                     count: int = ...,
-                     sort_by: typing.Union[str, enums.ReplaySortBy] = ...,
-                     sort_dir: typing.Union[str, enums.SortDirection] = ...,
+    def list_replays(self, *, next: str = ..., title: str = ..., player_names: Iterable[str] = ...,
+                     player_ids: Iterable[Tuple[Union[enums.Platform, str], Union[int, str]]] = ...,
+                     playlists: Iterable[Union[enums.Playlist, str]] = ...,
+                     season: Union[str, enums.Season] = ...,
+                     match_result: Union[str, enums.MatchResult] = ...,
+                     min_rank: Union[str, enums.Rank] = ...,
+                     max_rank: Union[str, enums.Rank] = ..., pro: bool = ...,
+                     uploader: Union[Literal["me"], str, int]  = ..., group: str = ...,
+                     map: Union[str, enums.Map] = ...,
+                     created_before: Union[models.Date, str] = ...,
+                     created_after: Union[models.Date, str] = ...,
+                     replay_date_before: Union[models.Date, str] = ...,
+                     replay_date_after: Union[models.Date, str] = ..., count: int = ...,
+                     sort_by: Union[str, enums.ReplaySortBy] = ...,
+                     sort_dir: Union[str, enums.SortDirection] = ...,
                      print_error: bool = True) -> requests.Response:
         """List replays filtered by various criteria.
 
         Parameters
         ----------
         next : str, optional
             A continuation URL (which can be acquired with
-            `<response from list_replays>.json()["next"]`). If defined, all
-            other arguments will be ignored.
+            `<response from list_replays>.json()["next"]`). If defined, the original parameters are
+            still required to get the expected result.
         title : str, optional
             Only include replays with the given title.
         player_names : list of str, optional
             Only include replays that include the given player(s) by display
             name.
-        player_ids : list of tuple of str and (int or str), optional
+        player_ids : list of tuple of (Platform or str) and (int or str), optional
             Only include replays that include the given player(s) by platform
             [0] and player ID [1].
         playlist : list of (str or Playlist), optional
             Only include replays in the given playlist(s).
         season : str or Season, optional
             Only include replays played in a given season.
         match_result : str or MatchResult, optional
@@ -252,17 +236,16 @@
             (inclusive) if defined.
         sort_by : str or ReplaySortBy, optional, default=
         ReplaySortBy.upload_date
             Whether to sort by replay date or upload date.
         sort_dir : str or SortDirection, optional, default=SortDirection.desc
             Whether to sort descending or ascending.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         Raises:
@@ -273,149 +256,145 @@
         if count != ... and 1 > count > 200:
             raise ValueError("\"count\" must be between 1 and 200")
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
-        # make request
+        # prepare url
         if next != ...:
-            # set url
-            url = next
-        else:
-            # prepare url
-            prepped_url = httpprep.URL(
-                protocol="https",
-                domain="ballchasing",
-                top_level_domain="com",
-                path_segments=["api", "replays"]
-            )
-            prepped_url.components.queries[
-                "title", "season", "match-result", "min-rank", "max-rank",
-                "pro", "uploader", "group", "map", "created-before",
-                "created-after", "replay-date-before", "replay-date-after",
-                "count", "sort-by", "sort-dir"] = [
-                title, p(season), p(match_result), p(min_rank), p(max_rank),
-                str(pro).lower() if isinstance(pro, bool) else ...,
-                uploader, group, p(map), created_before, created_after,
-                replay_date_before, replay_date_after, count, p(sort_by),
-                p(sort_dir)]
-            if player_names != ...:
-                for name in player_names:
-                    prepped_url.components.queries["player-name"] = name
-            if player_ids != ...:
-                for platform, id in player_ids:
-                    prepped_url.components.queries["player-id"] = (f"{platform}"
-                                                                   f":{id}")
-            if playlists != ...:
-                for playlist in playlists:
-                    prepped_url.components.queries["playlist"] = p(playlist)
-            url = prepped_url.build(query_check=...)
-
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.list_replays]()
+            try:
+                next = urllib.parse.unquote(re.search(r"(?<=after=)[^\&]*", next).group())
+            except Exception:
+                raise ValueError("'next' string has an unknown structure")
+
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing",
+                                   top_level_domain="com", path_segments=["api", "replays"])
+        prepped_url.components.queries[
+            "after",
+            "title",
+            "season",
+            "match-result",
+            "min-rank",
+            "max-rank",
+            "pro",
+            "uploader",
+            "group",
+            "map",
+            "created-before",
+            "created-after",
+            "replay-date-before",
+            "replay-date-after",
+            "count",
+            "sort-by",
+            "sort-dir"
+        ] = [
+            next,
+            title,
+            p(season),
+            p(match_result),
+            p(min_rank),
+            p(max_rank),
+            str(pro).lower() if isinstance(pro, bool) else ...,
+            uploader,
+            group,
+            p(map),
+            created_before,
+            created_after,
+            replay_date_before,
+            replay_date_after,
+            count,
+            p(sort_by),
+            p(sort_dir)
+        ]
+        if player_names != ...:
+            for name in player_names:
+                prepped_url.components.queries["player-name"] = name
+        if player_ids != ...:
+            for platform, id in player_ids:
+                prepped_url.components.queries["player-id"] = (f"{p(platform)}:{id}")
+        if playlists != ...:
+            for playlist in playlists:
+                prepped_url.components.queries["playlist"] = p(playlist)
+        url = prepped_url.build(query_check=...)
 
         # make request, print error, and return response
         response = requests.get(url, headers=prepped_headers.format_dict())
         if print_error:
             _print_error(response)
         return response
     
     @rlim.placeholder
-    def get_replay(self, replay_id: str, *,
-                   print_error: bool = True) -> requests.Response:
+    def get_replay(self, replay_id: str, *, print_error: bool = True) -> requests.Response:
         """Get more in-depth information for a specific replay.
 
         Parameters
         ----------
         replay_id : str
             The ID of the replay that is present in ballchasing's system.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "replays", replay_id]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "replays", replay_id])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.get_replay]()
-
         # make request, print error, and return response
-        response = requests.get(prepped_url.build(), headers=
-                                prepped_headers.format_dict())
+        response = requests.get(prepped_url.build(), headers=prepped_headers.format_dict())
         if print_error:
             _print_error(response)
         return response
     
     @rlim.placeholder
-    def delete_replay(self, replay_id: str, *,
-                      print_error: bool = True) -> requests.Response:
+    def delete_replay(self, replay_id: str, *, print_error: bool = True) -> requests.Response:
         """Delete the given replay from https://ballchasing.com, so long as the
         replay is owned by the token holder.
 
         Parameters
         ----------
         replay_id : str
             The ID of the replay that is present in ballchasing's system.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "replays", replay_id]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "replays", replay_id])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.delete_replay]()
-
         # make request, print error, and return response
-        response = requests.delete(prepped_url.build(), headers=
-                                   prepped_headers.format_dict())
+        response = requests.delete(prepped_url.build(), headers=prepped_headers.format_dict())
         if print_error:
             _print_error(response)
         return response
     
     @rlim.placeholder
     def patch_replay(self, replay_id: str, *, title: str = ...,
-                     visibility: typing.Union[str, enums.Visibility] = ...,
-                     group: str = ...,
+                     visibility: Union[str, enums.Visibility] = ..., group: str = ...,
                      print_error: bool = True) -> requests.Response:
         """Patch the title, visibility, and/or group of a replay on
         https://ballchasing.com, so long as the replay is owned by the token
         holder.
 
         Parameters
         ----------
@@ -425,110 +404,85 @@
             Set the title of the replay.
         visibility : str or Visibility, optional
             Set the visibility of the replay.
         group : str, optional
             Set the group of the replay. An empty string (`""`) will set the
             group to none.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "replays", replay_id]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "replays", replay_id])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
         # prepare payload
         payload = httpprep.OverloadDict()
         payload["title", "visibility", "group"] = [title, p(visibility), group]
 
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.patch_replay]()
-
         # make request, print error, and return response
-        response = requests.patch(prepped_url.build(),
-                                  headers=prepped_headers.format_dict(),
+        response = requests.patch(prepped_url.build(), headers=prepped_headers.format_dict(),
                                   json=payload.remove_values(...).to_dict())
         if print_error:
             _print_error(response)
         return response
 
     @rlim.placeholder
-    def download_replay(self, replay_id: str, *,
-                        print_error: bool = True) -> requests.Response:
+    def download_replay(self, replay_id: str, *, print_error: bool = True) -> requests.Response:
         """Download a replay from https://ballchasing.com.
 
         Parameters
         ----------
         replay_id : str
             The ID of the replay that is present in ballchasing's system.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Warnings
         --------
         Replay files can be rather large (up to around 1.5mb). The HTTP request
         is set to `stream`, thus you should use `iter_content` when saving the
         replay to a file.
 
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "replays", replay_id, "file"]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "replays", replay_id, "file"])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.download_replay]()
-
         # make request, print error, and return response
-        response = requests.get(prepped_url.build(),
-                                headers=prepped_headers.format_dict(),
+        response = requests.get(prepped_url.build(), headers=prepped_headers.format_dict(),
                                 stream=True)
         if print_error:
             _print_error(response)
         return response
 
     @rlim.placeholder
-    def create_group(self, name: str,
-                     player_identification: typing.Union[str,
-                        enums.PlayerIdentification],
-                     team_identification: typing.Union[str,
-                        enums.TeamIdentification], *,
-                     parent: str = ...,
-                     print_error: bool = True) -> requests.Response:
+    def create_group(self, name: str, player_identification: Union[str, enums.PlayerIdentification],
+                     team_identification: Union[str, enums.TeamIdentification], *,
+                     parent: str = ..., print_error: bool = True) -> requests.Response:
         """Create a replay group on https://ballchasing.com.
 
         Parameters
         ----------
         name : str
             The name of the group.
         player_identification : str or PlayerIdentification
@@ -537,72 +491,61 @@
         team_identification : str or TeamIdentification
             Determines how to identify the same team across multiple replays -
             by distinct players (if teams have fixed rosters for every single
             games), or by player clusters (if subs are allowed between games).
         parent : str, optional
             The parent group (group ID) to set as the parent of this group.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
 
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "groups"]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "groups"])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
         # prepare payload
         payload = httpprep.OverloadDict()
-        payload["name", "player_identification", "team_identification",
-                "parent"] = [name, p(player_identification),
-                             p(team_identification), parent]
-
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.create_group]()
+        payload[
+            "name", "player_identification", "team_identification", "parent"
+        ] = [
+            name, p(player_identification), p(team_identification), parent]
 
         # make request, print error, and return response
-        response = requests.post(prepped_url.build(), headers=
-                                 prepped_headers.format_dict(),
+        response = requests.post(prepped_url.build(), headers=prepped_headers.format_dict(),
                                  json=payload.remove_values(...).to_dict())
         if print_error:
             _print_error(response)
         return response
     
     @rlim.placeholder
-    def list_groups(self, *, next: str = ..., name: str = ...,
-                    creator: typing.Union[str, int] = ..., group: str = ...,
-                    created_before: typing.Union[models.Date, str] = ...,
-                    created_after: typing.Union[models.Date, str] = ...,
-                    count: int = ...,
-                    sort_by: typing.Union[str, enums.GroupSortBy] = ...,
-                    sort_dir: typing.Union[str, enums.SortDirection] = ...,
+    def list_groups(self, *, next: str = ..., name: str = ..., creator: Union[str, int] = ...,
+                    group: str = ..., created_before: Union[models.Date, str] = ...,
+                    created_after: Union[models.Date, str] = ..., count: int = ...,
+                    sort_by: Union[str, enums.GroupSortBy] = ...,
+                    sort_dir: Union[str, enums.SortDirection] = ...,
                     print_error: bool = True) -> requests.Response:
         """List replay groups from https://ballchasing.com filtered by various
         criteria.
 
         Parameters
         ----------
         next : str, optional
             A continuation URL (which can be acquired with
-            `<response from list_groups>.json()["next"]`). If defined, all
-            other arguments will be ignored.
+            `<response from list_groups>.json()["next"]`). If defined, the original parameters are
+            still required to get the expected result.
         name : str, optional
             Only include groups whose title contains the given text.
         creator : str or int, optional
             Only include replays uploaded by the given user (defined by a
             `SteamID64`).
         group : str, optional
             Only include replays that are direct or indirect children of the
@@ -619,17 +562,16 @@
         sort_by : str | GroupSortBy, optional, default=GroupSortBy.created
             Whether to sort by creation date or name. Keywords for this variable
             can be accessed through the `pychasing.types.SortBy` class.
         sort_dir : str | SortDirection, optional, default=SortDirection.desc
             Whether to sort descending or ascending. Keywords for this variable
             can be accessed through the `pychasing.types.SortDir` class.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
 
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         Raises:
@@ -640,138 +582,124 @@
         if count != ... and 1 > count > 200:
             raise ValueError("\"count\" must be between 1 and 200")
         
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
-        # make request
+        # prepare url
         if next != ...:
-            # set url
-            url = next
-        else:
-            # prepare url
-            prepped_url = httpprep.URL(
-                protocol="https",
-                domain="ballchasing",
-                top_level_domain="com",
-                path_segments=["api", "groups"]
-            )
-            prepped_url.components.queries["name", "creator", "group",
-                                           "created-before", "created-after",
-                                           "count", "sort-by", "sort-dir"] = [
-                                           name, creator, group, created_before,
-                                           created_after, count, p(sort_by),
-                                           p(sort_dir)]
-            url = prepped_url.build(query_check=...)
-
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.list_groups]()
+            try:
+                next = urllib.parse.unquote(re.search(r"(?<=after=)[^\&]*", next).group())
+            except Exception:
+                raise ValueError("'next' string has an unknown structure")
+
+        # prepare url
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing",
+                                    top_level_domain="com", path_segments=["api", "groups"])
+        prepped_url.components.queries[
+            "after",
+            "name",
+            "creator",
+            "group",
+            "created-before",
+            "created-after",
+            "count",
+            "sort-by",
+            "sort-dir"
+        ] = [
+            next,
+            name,
+            creator,
+            group,
+            created_before,
+            created_after,
+            count, 
+            p(sort_by),
+            p(sort_dir)
+        ]
+        url = prepped_url.build(query_check=...)
 
         # make request, print error, and return response
         response = requests.get(url, headers=prepped_headers.format_dict())
         if print_error:
             _print_error(response)
         return response
 
     @rlim.placeholder
-    def get_group(self, group_id: str, *,
-                  print_error: bool = True) -> requests.Response:
+    def get_group(self, group_id: str, *, print_error: bool = True) -> requests.Response:
         """Get information on a specific replay group from
         https://ballchasing.com.
 
         Parameters
         ----------
         group_id : str
             The ID of the group present in ballchasing's systems.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "groups", group_id]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "groups", group_id])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.get_group]()
-
         # make request, print error, and return response
-        response = requests.get(prepped_url.build(), headers=
-                                prepped_headers.format_dict())
+        response = requests.get(prepped_url.build(), headers=prepped_headers.format_dict())
         if print_error:
             _print_error(response)
         return response
     
-    def delete_group(self, group_id: str, *,
-                     print_error: bool = True) -> requests.Response:
+    def delete_group(self, group_id: str, *, print_error: bool = True) -> requests.Response:
         """Delete a specific group (and all children groups) from
         https://ballchasing.com, so long as it is owned by the token holder.
 
         Parameters
         ----------
         group_id : str
             The ID of the group present in ballchasing's systems.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "groups", group_id]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "groups", group_id])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.delete_group]()
-
         # make request, print error, and return response
-        response = requests.delete(prepped_url.build(), headers=
-                                   prepped_headers.format_dict())
+        response = requests.delete(prepped_url.build(), headers=prepped_headers.format_dict())
         if print_error:
             _print_error(response)
         return response
     
     @rlim.placeholder
     def patch_group(self, group_id: str, *,
-        player_identification: typing.Union[str,
-            enums.PlayerIdentification] = ...,
-        team_identification: typing.Union[str, enums.TeamIdentification] = ...,
-        parent: str = ..., shared: bool = ...,
-        print_error: bool = True) -> requests.Response:
+                    player_identification: Union[str, enums.PlayerIdentification] = ...,
+                    team_identification: Union[str, enums.TeamIdentification] = ...,
+                    parent: str = ..., shared: bool = ...,
+                    print_error: bool = True) -> requests.Response:
         """Delete a specific group (and all children groups) from
         https://ballchasing.com, so long as it is owned by the token holder.
 
         Parameters
         ----------
         group_id : str
             The ID of the group present in ballchasing's systems.
@@ -785,240 +713,66 @@
         parent : str, optional
             The parent group (group ID) to set as the parent of this group.
         shared : bool, optional
             Set group sharing. If enabled, people with the link to the group may
             access its contents regardless of the individual visibility settings
             of its children.
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
         
         """
         # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "groups", group_id]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "groups", group_id])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
         # prepare payload
         payload = httpprep.OverloadDict()
-        payload["player_identification", "team_identification", "parent",
-                "shared"] = [p(player_identification),
-                             p(team_identification), parent, shared]
-
-        # rate limit if enabled
-        # if self._auto_rate_limit:
-        #     self._rate_limiters[enums.Operation.patch_group]()
+        payload[
+            "player_identification", "team_identification", "parent", "shared"
+        ] = [
+            p(player_identification), p(team_identification), parent, shared]
 
         # make request, print error, and return response
-        response = requests.patch(prepped_url.build(), headers=
-                                  prepped_headers.format_dict(),
+        response = requests.patch(prepped_url.build(), headers=prepped_headers.format_dict(),
                                   json=payload.remove_values(...).to_dict())
         if print_error:
             _print_error(response)
         return response
     
     def maps(self, *, print_error: bool = True) -> requests.Response:
         """Get a list of current maps.
         
         Parameters
         ----------
         print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
+            Prints an error message (that contains information about the error) if the request
+            resulted in an HTTP error (i.e. status codes 400 through 599).
         
         Returns
         -------
         requests.Response
             The `requests.Response` object returned from the HTTP request.
 
         """
         # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["api", "maps"]
-        )
+        prepped_url = httpprep.URL(protocol="https", domain="ballchasing", top_level_domain="com",
+                                   path_segments=["api", "maps"])
 
         # prepare headers
         prepped_headers = httpprep.Headers()
         prepped_headers.Authorization = self._token
 
         # make request, print error, and return response
-        response = requests.get(prepped_url.build(), headers=
-                                prepped_headers.format_dict())
-        if print_error:
-            _print_error(response)
-        return response
-    
-    @staticmethod
-    def get_threejs(replay_id: str, *, cookie: str = ...,
-                    print_error: bool = True) -> requests.Response:
-        """Get basic locational, rotational, and timestamp data from a given
-        replay on https://ballchasing.com.
-
-        This is a static method and does not require a token (or construction of
-        the outer class). It is not rate-limited.
-
-        Parameters
-        ----------
-        replay_id : str
-            The ID of the replay that is present in ballchasing's system.
-        cookie : str, optional
-            Not required, but if provided, you are able to use this method on
-            private replays so long as they belong to the cookie-holder's
-            account on ballchasing.
-        print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
-        
-        Returns
-        -------
-        requests.Response
-            The `requests.Response` object returned from the HTTP request.
-
-        
-        Warnings
-        --------
-        This functionality is highly experimental. It accesses a back-end API
-        used for populating site data (that notably does not require
-        authorization headers). At any time, this API could become restricted or
-        its functionality could change.
-
-        """
-        # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["dyn", "replay", replay_id, "threejs"]
-        )
-
-        # prepare headers
-        prepped_headers = httpprep.Headers()
-        prepped_headers.Cookie = cookie
-
-        # make request, print error, and return response
-        response = requests.get(prepped_url.build(), headers=
-                                prepped_headers.format_dict(...))
-        if print_error:
-            _print_error(response)
-        return response
-    
-    @staticmethod
-    def get_timeline(replay_id: str, *, cookie: str = ...,
-                    print_error: bool = True) -> requests.Response:
-        """Get basic timeline data from a replay on https://ballchasing.com.
-
-        This is a static method and does not require a token (or construction of
-        the outer class). It is not rate-limited. 
-
-        Parameters
-        ----------
-        replay_id : str
-            The ID of the replay that is present in ballchasing's system.
-        cookie : str, optional
-            Not required, but if provided, you are able to use this method on
-            private replays so long as they belong to the cookie-holder's
-            account on ballchasing.
-        print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
-        
-        Returns
-        -------
-        requests.Response
-            The `requests.Response` object returned from the HTTP request.
-        
-        Warnings
-        --------
-        This functionality is highly experimental. It accesses a back-end API
-        used for populating site data (that notably does not require
-        authorization headers). At any time, this API could become restricted or
-        its functionality could change.
-        
-        """
-        # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["dyn", "replay", replay_id, "timeline"]
-        )
-
-        # prepare headers
-        prepped_headers = httpprep.Headers()
-        prepped_headers.Cookie = cookie
-
-        # make request, print error, and return response
-        response = requests.get(prepped_url.build(), headers=
-                                prepped_headers.format_dict(...))
-        if print_error:
-            _print_error(response)
-        return response
-    
-    @staticmethod
-    def export_csv(group_id: str, stat: typing.Union[str, enums.GroupStats], *,
-                   cookie: str = ...,
-                   print_error: bool = True) -> requests.Response:
-        """Get group statistics from a group on https://ballchasing.com.
-
-        This is a static method and does not require a token (or construction of
-        the outer class). It is not rate-limited. 
-
-        Parameters
-        ----------
-        group_id : str
-            The ID of the group that is present in ballchasing's system.
-        stat : str or GroupStats
-            The stat section (players, teams, players games, teams games) to
-            export.
-        cookie : str, optional
-            Not required, but if provided, you are able to use this method on
-            private replays so long as they belong to the cookie-holder's
-            account on ballchasing.
-        print_error : bool, optional, default=True
-            Prints an error message (that contains information about the error)
-            if the request resulted in an HTTP error (i.e. status codes 400
-            through 599).
-        
-        Returns
-        -------
-        requests.Response
-            The `requests.Response` object returned from the HTTP request.
-
-        """
-        # prepare url
-        prepped_url = httpprep.URL(
-            protocol="https",
-            domain="ballchasing",
-            top_level_domain="com",
-            path_segments=["dl", "stats", f"group-{p(stat)}", group_id,
-                           f"{group_id}-{p(stat)}.csv"]
-        )
-
-        # prepare headers
-        prepped_headers = httpprep.Headers()
-        prepped_headers.Cookie = cookie
-
-        # make request, print error, and return response
-        response = requests.get(prepped_url.build(), headers=
-                                prepped_headers.format_dict(...))
+        response = requests.get(prepped_url.build(), headers=prepped_headers.format_dict())
         if print_error:
             _print_error(response)
         return response
```

### Comparing `pychasing-0.1.6/src/pychasing/enums.py` & `pychasing-0.1.7/src/pychasing/enums.py`

 * *Files 20% similar despite different names*

```diff
@@ -142,75 +142,127 @@
     ranked_snowday="ranked-snowday"
     dropshot_rumble="dropshot-rumble"
     heatseeker="heatseeker"
 
 class Platform(enum.Enum):
     steam="steam"
     epic="epic"
-    xbl="xbl"
-    psn="psn"
+    xbl="xbox"
+    psn="ps4"
     switch="switch"
 
 class Map(enum.Enum):
     arc_p="arc_p"
+    Starbase_ARC="arc_p"
     arc_standard_p="arc_standard_p"
+    Starbase_ARC_Standard="arc_standard_p"   
     bb_p="bb_p"
+    Champions_Field_NFL="bb_p"
     beach_night_p="beach_night_p"
+    Salty_Shores_Night="beach_night_p"       
     beach_p="beach_p"
+    Salty_Shores="beach_p"
     beachvolley="beachvolley"
-    chn_stadium_day_p="chn_stadium_day_p"
+    Salty_Shores_Volley="beachvolley"        
+    chn_stadium_day_p="chn_stadium_day_p"    
+    Forbidden_Temple_Day="chn_stadium_day_p" 
     chn_stadium_p="chn_stadium_p"
+    Forbidden_Temple="chn_stadium_p"
     cs_day_p="cs_day_p"
+    Champions_Field_Day="cs_day_p"
     cs_hw_p="cs_hw_p"
+    Rivals_Arena="cs_hw_p"
     cs_p="cs_p"
+    Champions_Field="cs_p"
     eurostadium_night_p="eurostadium_night_p"
+    Mannfield_Night="eurostadium_night_p"    
     eurostadium_p="eurostadium_p"
+    Mannfield="eurostadium_p"
     eurostadium_rainy_p="eurostadium_rainy_p"
+    Mannfield_Stormy="eurostadium_rainy_p"
     eurostadium_snownight_p="eurostadium_snownight_p"
+    Mannfield_Snowy="eurostadium_snownight_p"
     farm_hw_p="farm_hw_p"
+    Farmstead_Spooky="farm_hw_p"
     farm_night_p="farm_night_p"
+    Farmstead_Night="farm_night_p"
     farm_p="farm_p"
+    Farmstead="farm_p"
     farm_upsidedown_p="farm_upsidedown_p"
+    Farmstead_The_Upside_Down="farm_upsidedown_p"
     haunted_trainstation_p="haunted_trainstation_p"
+    Urban_Central_Haunted="haunted_trainstation_p"
     hoopsstadium_p="hoopsstadium_p"
+    Dunk_House="hoopsstadium_p"
     labs_circlepillars_p="labs_circlepillars_p"
+    Pillars="labs_circlepillars_p"
     labs_corridor_p="labs_corridor_p"
+    Corridor="labs_corridor_p"
     labs_cosmic_p="labs_cosmic_p"
+    Cosmic="labs_cosmic_p"
     labs_cosmic_v4_p="labs_cosmic_v4_p"
     labs_doublegoal_p="labs_doublegoal_p"
+    Double_Goal="labs_doublegoal_p"
     labs_doublegoal_v2_p="labs_doublegoal_v2_p"
     labs_octagon_02_p="labs_octagon_02_p"
+    Octagon="labs_octagon_02_p"
     labs_octagon_p="labs_octagon_p"
     labs_underpass_p="labs_underpass_p"
+    Underpass="labs_underpass_p"
     labs_underpass_v0_p="labs_underpass_v0_p"
     labs_utopia_p="labs_utopia_p"
+    Utopia_Retro="labs_utopia_p"
     music_p="music_p"
+    Neon_Fields="music_p"
     neotokyo_p="neotokyo_p"
+    Neo_Tokyo="neotokyo_p"
     neotokyo_standard_p="neotokyo_standard_p"
+    Neo_Tokyo_Standard="neotokyo_standard_p"
     park_night_p="park_night_p"
+    Beckwith_Park_Midnight="park_night_p"
     park_p="park_p"
+    Beckwith_Park="park_p"
     park_rainy_p="park_rainy_p"
+    Beckwith_Park_Stormy="park_rainy_p"
     shattershot_p="shattershot_p"
+    Core_707="shattershot_p"
     stadium_day_p="stadium_day_p"
+    DFH_Stadium_Day="stadium_day_p"
     stadium_foggy_p="stadium_foggy_p"
+    DFH_Stadium_Stormy="stadium_foggy_p"
     stadium_p="stadium_p"
+    DFH_Stadium="stadium_p"
     stadium_race_day_p="stadium_race_day_p"
+    DFH_Stadium_Circuit="stadium_race_day_p"
     stadium_winter_p="stadium_winter_p"
+    DFH_Stadium_Snowy="stadium_winter_p"
     throwbackstadium_p="throwbackstadium_p"
+    Throwback_Stadium="throwbackstadium_p"
     trainstation_dawn_p="trainstation_dawn_p"
+    Urban_Central_Dawn="trainstation_dawn_p"
     trainstation_night_p="trainstation_night_p"
+    Urban_Central_Night="trainstation_night_p"
     trainstation_p="trainstation_p"
+    Urban_Central="trainstation_p"
     underwater_p="underwater_p"
+    Aquadome="underwater_p"
     utopiastadium_dusk_p="utopiastadium_dusk_p"
+    Utopia_Coliseum_Dusk="utopiastadium_dusk_p"
     utopiastadium_p="utopiastadium_p"
+    Utopia_Coliseum="utopiastadium_p"
     utopiastadium_snow_p="utopiastadium_snow_p"
+    Utopia_Coliseum_Snowy="utopiastadium_snow_p"
     wasteland_night_p="wasteland_night_p"
+    Wasteland_Night="wasteland_night_p"
     wasteland_night_s_p="wasteland_night_s_p"
+    Wasteland_Standard_Night="wasteland_night_s_p"
     wasteland_p="wasteland_p"
+    Wasteland="wasteland_p"
     wasteland_s_p="wasteland_s_p"
+    Wasteland_Standard="wasteland_s_p"
 
 class Visibility(enum.Enum):
     public="public"
     unlisted="unlisted"
     private="private"
 
 class Season(enum.Enum):
```

### Comparing `pychasing-0.1.6/src/pychasing/models.py` & `pychasing-0.1.7/src/pychasing/models.py`

 * *Files identical despite different names*

