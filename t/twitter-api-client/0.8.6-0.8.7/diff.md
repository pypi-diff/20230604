# Comparing `tmp/twitter-api-client-0.8.6.tar.gz` & `tmp/twitter-api-client-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twitter-api-client-0.8.6.tar", last modified: Sat Jun  3 18:36:24 2023, max compression
+gzip compressed data, was "twitter-api-client-0.8.7.tar", last modified: Sun Jun  4 17:21:39 2023, max compression
```

## Comparing `twitter-api-client-0.8.6.tar` & `twitter-api-client-0.8.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-03 18:36:24.065571 twitter-api-client-0.8.6/
--rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.6/LICENSE
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-03 18:36:24.065571 twitter-api-client-0.8.6/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-03 18:36:24.065571 twitter-api-client-0.8.6/setup.cfg
--rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-03 18:35:25.000000 twitter-api-client-0.8.6/setup.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-03 18:36:24.064571 twitter-api-client-0.8.6/twitter/
--rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.8.6/twitter/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)    23264 2023-06-02 20:06:40.000000 twitter-api-client-0.8.6/twitter/account.py
--rw-r--r--   0 x         (1000) x         (1000)    28454 2023-06-02 01:49:12.000000 twitter-api-client-0.8.6/twitter/constants.py
--rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.8.6/twitter/login.py
--rw-r--r--   0 x         (1000) x         (1000)    27547 2023-06-03 18:35:00.000000 twitter-api-client-0.8.6/twitter/scraper.py
--rw-r--r--   0 x         (1000) x         (1000)     5960 2023-06-02 01:50:23.000000 twitter-api-client-0.8.6/twitter/search.py
--rw-r--r--   0 x         (1000) x         (1000)     9348 2023-06-02 17:01:02.000000 twitter-api-client-0.8.6/twitter/util.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-03 18:36:24.065571 twitter-api-client-0.8.6/twitter_api_client.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-03 18:36:24.000000 twitter-api-client-0.8.6/twitter_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-04 17:21:39.733603 twitter-api-client-0.8.7/
+-rw-r--r--   0 x         (1000) x         (1000)     1075 2023-05-28 16:24:21.000000 twitter-api-client-0.8.7/LICENSE
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-04 17:21:39.733603 twitter-api-client-0.8.7/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)       38 2023-06-04 17:21:39.733603 twitter-api-client-0.8.7/setup.cfg
+-rw-r--r--   0 x         (1000) x         (1000)    12740 2023-06-04 17:13:56.000000 twitter-api-client-0.8.7/setup.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-04 17:21:39.732602 twitter-api-client-0.8.7/twitter/
+-rw-r--r--   0 x         (1000) x         (1000)        0 2023-06-02 19:12:02.000000 twitter-api-client-0.8.7/twitter/__init__.py
+-rw-r--r--   0 x         (1000) x         (1000)    23270 2023-06-04 16:20:00.000000 twitter-api-client-0.8.7/twitter/account.py
+-rw-r--r--   0 x         (1000) x         (1000)    28755 2023-06-03 21:50:49.000000 twitter-api-client-0.8.7/twitter/constants.py
+-rw-r--r--   0 x         (1000) x         (1000)     7410 2023-06-02 20:00:37.000000 twitter-api-client-0.8.7/twitter/login.py
+-rw-r--r--   0 x         (1000) x         (1000)    27620 2023-06-04 17:13:56.000000 twitter-api-client-0.8.7/twitter/scraper.py
+-rw-r--r--   0 x         (1000) x         (1000)     5960 2023-06-02 01:50:23.000000 twitter-api-client-0.8.7/twitter/search.py
+-rw-r--r--   0 x         (1000) x         (1000)     9625 2023-06-04 17:08:22.000000 twitter-api-client-0.8.7/twitter/util.py
+drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-06-04 17:21:39.733603 twitter-api-client-0.8.7/twitter_api_client.egg-info/
+-rw-r--r--   0 x         (1000) x         (1000)    10919 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 x         (1000) x         (1000)      355 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 x         (1000) x         (1000)        1 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 x         (1000) x         (1000)       91 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/requires.txt
+-rw-r--r--   0 x         (1000) x         (1000)        8 2023-06-04 17:21:39.000000 twitter-api-client-0.8.7/twitter_api_client.egg-info/top_level.txt
```

### Comparing `twitter-api-client-0.8.6/LICENSE` & `twitter-api-client-0.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.6/PKG-INFO` & `twitter-api-client-0.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.6
+Version: 0.8.7
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

### Comparing `twitter-api-client-0.8.6/setup.py` & `twitter-api-client-0.8.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "tqdm",
     "orjson",
     'uvloop; platform_system != "Windows"',
 ]
 
 setup(
     name="twitter-api-client",
-    version="0.8.6",
+    version="0.8.7",
     python_requires=">=3.10.10",
     description="Twitter API",
     long_description=dedent('''
     
     ## Implementation of Twitter's v1, v2, and GraphQL APIs
```

### Comparing `twitter-api-client-0.8.6/twitter/account.py` & `twitter-api-client-0.8.7/twitter/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,63 +33,44 @@
 
 
 class Account:
 
     def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
         self.logger = self.init_logger(kwargs.get('log_config', False))
         self.session = self.validate_session(email, username, password, session, **kwargs)
-        self.gql_url = 'https://twitter.com/i/api/graphql'
-        self.v1_url = 'https://api.twitter.com/1.1'
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
-
-    @staticmethod
-    def init_logger(cfg: dict) -> Logger:
-        if cfg:
-            logging.config.dictConfig(cfg)
-            return logging.getLogger(__name__)
-        return logger
-
-    @staticmethod
-    def validate_session(*args, **kwargs):
-        email, username, password, session = args
-        if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
-            # authenticated session provided
-            return session
-        if not session:
-            # no session provided, login to authenticate
-            return login(email, username, password, **kwargs)
-        raise Exception('Session not authenticated. '
-                        'Please use an authenticated session or remove the `session` argument and try again.')
+        self.gql_api = 'https://twitter.com/i/api/graphql'
+        self.v1_api = 'https://api.twitter.com/1.1'
 
     def gql(self, method: str, operation: tuple, variables: dict, features: dict = Operation.default_features) -> dict:
         qid, op = operation
         params = {
             'queryId': qid,
             'features': features,
             'variables': Operation.default_variables | variables
         }
         if method == 'POST':
             data = {'json': params}
         else:
             data = {'params': {k: orjson.dumps(v).decode() for k, v in params.items()}}
         r = self.session.request(
             method=method,
-            url=f'{self.gql_url}/{qid}/{op}',
+            url=f'{self.gql_api}/{qid}/{op}',
             headers=get_headers(self.session),
             **data
         )
         if self.debug:
             log(self.logger, self.debug, r)
         return r.json()
 
     def v1(self, path: str, params: dict) -> dict:
         headers = get_headers(self.session)
         headers['content-type'] = 'application/x-www-form-urlencoded'
-        r = self.session.post(f'{self.v1_url}/{path}', headers=headers, data=urlencode(params))
+        r = self.session.post(f'{self.v1_api}/{path}', headers=headers, data=urlencode(params))
         if self.debug:
             log(self.logger, self.debug, r)
         return r.json()
 
     def create_poll(self, text: str, choices: list[str], poll_duration: int) -> dict:
         options = {
             "twitter:card": "poll4choice_text_only",
@@ -350,39 +331,39 @@
         return self.v1('blocks/create.json', {'user_id': user_id})
 
     def unblock(self, user_id: int) -> dict:
         return self.v1('blocks/destroy.json', {'user_id': user_id})
 
     def update_profile_image(self, media: str) -> Response:
         media_id = self._upload_media(media, is_profile=True)
-        url = f'{self.v1_url}/account/update_profile_image.json'
+        url = f'{self.v1_api}/account/update_profile_image.json'
         headers = get_headers(self.session)
         params = {'media_id': media_id}
         r = self.session.post(url, headers=headers, params=params)
         return r
 
     def update_profile_banner(self, media: str) -> Response:
         media_id = self._upload_media(media, is_profile=True)
-        url = f'{self.v1_url}/account/update_profile_banner.json'
+        url = f'{self.v1_api}/account/update_profile_banner.json'
         headers = get_headers(self.session)
         params = {'media_id': media_id}
         r = self.session.post(url, headers=headers, params=params)
         return r
 
     def update_profile_info(self, **kwargs) -> Response:
-        url = f'{self.v1_url}/account/update_profile.json'
+        url = f'{self.v1_api}/account/update_profile.json'
         headers = get_headers(self.session)
         r = self.session.post(url, headers=headers, params=kwargs)
         return r
 
     def update_search_settings(self, settings: dict) -> Response:
         twid = int(self.session.cookies.get('twid').split('=')[-1].strip('"'))
         headers = get_headers(self.session)
         r = self.session.post(
-            url=f'{self.v1_url}/strato/column/User/{twid}/search/searchSafety',
+            url=f'{self.v1_api}/strato/column/User/{twid}/search/searchSafety',
             headers=headers,
             json=settings,
         )
         return r
 
     def update_settings(self, settings: dict) -> dict:
         return self.v1('account/settings.json', settings)
@@ -400,15 +381,15 @@
         return r.json()
 
     def remove_interests(self, *args):
         """
         Pass 'all' to remove all interests
         """
         r = self.session.get(
-            f'{self.v1_url}/account/personalization/twitter_interests.json',
+            f'{self.v1_api}/account/personalization/twitter_interests.json',
             headers=get_headers(self.session)
         )
         current_interests = r.json()['interested_in']
         if args == 'all':
             disabled_interests = [x['id'] for x in current_interests]
         else:
             disabled_interests = [x['id'] for x in current_interests if x['display_name'] in args]
@@ -417,15 +398,15 @@
                 "interest_preferences": {
                     "disabled_interests": disabled_interests,
                     "disabled_partner_interests": []
                 }
             }
         }
         r = self.session.post(
-            f'{self.v1_url}/account/personalization/p13n_preferences.json',
+            f'{self.v1_api}/account/personalization/p13n_preferences.json',
             headers=get_headers(self.session),
             json=payload
         )
         return r
 
     def home_timeline(self, limit=math.inf) -> list[dict]:
         return self._paginate('POST', Operation.HomeTimeline, Operation.default_variables, limit)
@@ -523,20 +504,20 @@
                             b'\r\n------WebKitFormBoundary',
                             pad,
                             b'--\r\n',
                         ])
                         _headers = {b'content-type': b'multipart/form-data; boundary=----WebKitFormBoundary' + pad}
                         r = self.session.post(url=url, headers=headers | _headers, params=params, content=data)
                     except Exception as e:
-                        self.logger.error('Failed to upload chunk, trying alternative method')
+                        self.logger.error(f'Failed to upload chunk, trying alternative method\n{e}')
                         try:
                             files = {'media': chunk}
                             r = self.session.post(url=url, headers=headers, params=params, files=files)
                         except Exception as e:
-                            self.logger.error(f'Failed to upload chunk: {e}')
+                            self.logger.error(f'Failed to upload chunk\n{e}')
                             return
 
                     if r.status_code < 200 or r.status_code > 299:
                         self.logger.debug(f'{RED}{r.status_code} {r.text}{RESET}')
 
                     i += 1
                     pbar.update(fp.tell() - pbar.n)
@@ -567,10 +548,29 @@
             r = self.session.get(url=url, headers=headers, params=params)
             processing_info = r.json().get('processing_info')
         # self.logger.debug('processing complete')
         return media_id
 
     def _add_alt_text(self, media_id: int, text: str) -> Response:
         params = {"media_id": media_id, "alt_text": {"text": text}}
-        url = f'{self.v1_url}/media/metadata/create.json'
+        url = f'{self.v1_api}/media/metadata/create.json'
         r = self.session.post(url, headers=get_headers(self.session), json=params)
         return r
+
+    @staticmethod
+    def init_logger(cfg: dict) -> Logger:
+        if cfg:
+            logging.config.dictConfig(cfg)
+            return logging.getLogger(__name__)
+        return logger
+
+    @staticmethod
+    def validate_session(*args, **kwargs):
+        email, username, password, session = args
+        if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
+            # authenticated session provided
+            return session
+        if not session:
+            # no session provided, login to authenticate
+            return login(email, username, password, **kwargs)
+        raise Exception('Session not authenticated. '
+                        'Please use an authenticated session or remove the `session` argument and try again.')
```

### Comparing `twitter-api-client-0.8.6/twitter/constants.py` & `twitter-api-client-0.8.7/twitter/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -354,42 +354,48 @@
         'withReactionsPerspective': False,
         'withSuperFollowsTweetFields': True,
         'isMetatagsQuery': False,
         'withReplays': True,
         'withClientEventToken': False,
     }
     default_features = {
-        'blue_business_profile_image_shape_enabled': True,
-        'responsive_web_graphql_exclude_directive_enabled': True,
-        'verified_phone_label_enabled': False,
-        'responsive_web_graphql_skip_user_profile_image_extensions_enabled': False,
-        'responsive_web_graphql_timeline_navigation_enabled': True,
-        'tweetypie_unmention_optimization_enabled': True, 'vibe_api_enabled': True,
-        'responsive_web_edit_tweet_api_enabled': True,
-        'graphql_is_translatable_rweb_tweet_is_translatable_enabled': True,
-        'view_counts_everywhere_api_enabled': True,
-        'longform_notetweets_consumption_enabled': True,
-        'tweet_awards_web_tipping_enabled': False,
-        'freedom_of_speech_not_reach_fetch_enabled': False,
-        'standardized_nudges_misinfo': True,
-        'tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled': False,
-        'interactive_text_enabled': True,
-        'responsive_web_text_conversations_enabled': False,
-        'longform_notetweets_rich_text_read_enabled': True,
-        'responsive_web_enhance_cards_enabled': False,
-        'responsive_web_twitter_blue_verified_badge_is_enabled': True,
-        'longform_notetweets_richtext_consumption_enabled': True,
-        'profile_foundations_tweet_stats_enabled': True,
-        'profile_foundations_tweet_stats_tweet_frequency': True,
-        'graphql_timeline_v2_bookmark_timeline': True,
-        'spaces_2022_h2_clipping': True,
-        'spaces_2022_h2_spaces_communities': True,
-        'creator_subscriptions_tweet_preview_api_enabled': True,
-        'longform_notetweets_inline_media_enabled': False,
-        'rweb_lists_timeline_redesign_enabled': True,
+        "blue_business_profile_image_shape_enabled": True,
+        "creator_subscriptions_tweet_preview_api_enabled": True,
+        "freedom_of_speech_not_reach_fetch_enabled": False,
+        "graphql_is_translatable_rweb_tweet_is_translatable_enabled": True,
+        "graphql_timeline_v2_bookmark_timeline": True,
+        "hidden_profile_likes_enabled": True,
+        "highlights_tweets_tab_ui_enabled": True,
+        "interactive_text_enabled": True,
+        "longform_notetweets_consumption_enabled": True,
+        "longform_notetweets_inline_media_enabled": False,
+        "longform_notetweets_rich_text_read_enabled": True,
+        "longform_notetweets_richtext_consumption_enabled": True,
+        "profile_foundations_tweet_stats_enabled": True,
+        "profile_foundations_tweet_stats_tweet_frequency": True,
+        "responsive_web_birdwatch_note_limit_enabled": True,
+        "responsive_web_edit_tweet_api_enabled": True,
+        "responsive_web_enhance_cards_enabled": False,
+        "responsive_web_graphql_exclude_directive_enabled": True,
+        "responsive_web_graphql_skip_user_profile_image_extensions_enabled": False,
+        "responsive_web_graphql_timeline_navigation_enabled": True,
+        "responsive_web_text_conversations_enabled": False,
+        "responsive_web_twitter_article_data_v2_enabled": True,
+        "responsive_web_twitter_blue_verified_badge_is_enabled": True,
+        "rweb_lists_timeline_redesign_enabled": True,
+        "spaces_2022_h2_clipping": True,
+        "spaces_2022_h2_spaces_communities": True,
+        "standardized_nudges_misinfo": True,
+        "subscriptions_verification_info_verified_since_enabled": True,
+        "tweet_awards_web_tipping_enabled": False,
+        "tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled": False,
+        "tweetypie_unmention_optimization_enabled": True,
+        "verified_phone_label_enabled": False,
+        "vibe_api_enabled": True,
+        "view_counts_everywhere_api_enabled": True,
     }
 
 
 trending_params = {
     'include_profile_interstitial_type': '1',
     'include_blocking': '1',
     'include_blocked_by': '1',
```

### Comparing `twitter-api-client-0.8.6/twitter/login.py` & `twitter-api-client-0.8.7/twitter/login.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.6/twitter/scraper.py` & `twitter-api-client-0.8.7/twitter/scraper.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import asyncio
 import logging.config
 import math
 import platform
 import random
-from concurrent.futures import ThreadPoolExecutor, as_completed
 
 import aiofiles
-import httpx
 import websockets
 from httpx import AsyncClient, Limits, ReadTimeout, URL
-from tqdm import tqdm
 from tqdm.asyncio import tqdm_asyncio
 
 from .constants import *
 from .login import login
 from .util import *
 
 try:
@@ -37,35 +34,14 @@
     def __init__(self, email: str = None, username: str = None, password: str = None, session: Client = None, **kwargs):
         self.guest = False
         self.logger = self.init_logger(kwargs.get('log_config', False))
         self.session = self.validate_session(email, username, password, session, **kwargs)
         self.save = kwargs.get('save', True)
         self.debug = kwargs.get('debug', 0)
         self.out_path = Path('data')
-        self.api = 'https://twitter.com/i/api/graphql'
-
-    @staticmethod
-    def init_logger(cfg: dict) -> Logger:
-        if cfg:
-            logging.config.dictConfig(cfg)
-            return logging.getLogger(__name__)
-        return logger
-
-    def validate_session(self, *args, **kwargs):
-        email, username, password, session = args
-        if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
-            # authenticated session provided
-            return session
-        if not session:
-            # no session provided, login to authenticate
-            return login(email, username, password, **kwargs)
-        self.logger.warning(f'\n{RED}WARNING: This is a guest session, '
-                            f'some endpoints cannot be accessed.{RESET}\n')
-        self.guest = True
-        return session
 
     def users(self, screen_names: list[str], **kwargs) -> list[dict]:
         return self._run(Operation.UserByScreenName, screen_names, **kwargs)
 
     def tweets_by_id(self, tweet_ids: list[int], **kwargs) -> list[dict]:
         return self._run(Operation.TweetResultByRestId, tweet_ids, **kwargs)
 
@@ -119,76 +95,80 @@
     def recommended_users(self, user_ids: list[int] = None, **kwargs) -> dict:
         if user_ids:
             contexts = [{"context": orjson.dumps({"contextualUserId": x}).decode()} for x in user_ids]
         else:
             contexts = [{'context': None}]
         return self._run(Operation.ConnectTabTimeline, contexts, **kwargs)
 
-    def download_media(self, ids: list[int], photos: bool = True, videos: bool = True) -> None:
+    def download_media(self, ids: list[int], photos: bool = True, videos: bool = True,
+                       chunk_size: int = 8192) -> None:
+
+        out = (self.out_path / 'media')
+        out.mkdir(parents=True, exist_ok=True)
         tweets = self.tweets_by_id(ids)
         urls = []
         for tweet in tweets:
-            tweet_ids = find_key(tweet, 'id_str')
-            tweet_id = tweet_ids[0]
-            url = f'https://twitter.com/i/status/{tweet_id}'  # `i` evaluates to screen_name
+            tweet_id = find_key(tweet, 'id_str')[0]
+            url = f'https://twitter.com/i/status/{tweet_id}'
             media = [y for x in find_key(tweet, 'media') for y in x]
             if photos:
                 photo_urls = list({u for m in media if 'ext_tw_video_thumb' not in (u := m['media_url_https'])})
                 [urls.append([url, photo]) for photo in photo_urls]
             if videos:
                 video_urls = [x['variants'] for m in media if (x := m.get('video_info'))]
                 hq_videos = {sorted(v, key=lambda d: d.get('bitrate', 0))[-1]['url'] for v in video_urls}
                 [urls.append([url, video]) for video in hq_videos]
 
-        with tqdm(total=len(urls), desc='downloading media') as pbar:
-            with ThreadPoolExecutor(max_workers=32) as e:
-                for future in as_completed(e.submit(self._download, x, y) for x, y in urls):
-                    future.result()
-                    pbar.update()
-
-    def _download(self, post_url: str, cdn_url: str, path: str = 'media', chunk_size: int = 4096) -> None:
-        (self.out_path / 'media').mkdir(parents=True, exist_ok=True)
-        name = urlsplit(post_url).path.replace('/', '_')[1:]
-        ext = urlsplit(cdn_url).path.split('/')[-1]
-        try:
-            with httpx.stream('GET', cdn_url, headers=self.session.headers, cookies=self.session.cookies) as r:
-                with open(f'{path}/{name}_{ext}', 'wb') as f:
+        async def process():
+            async with AsyncClient(headers=self.session.headers, cookies=self.session.cookies) as client:
+                return await tqdm_asyncio.gather(*(download(client, x, y) for x, y in urls),
+                                                 desc='downloading media')
+
+        async def download(client: AsyncClient, post_url: str, cdn_url: str) -> None:
+            name = urlsplit(post_url).path.replace('/', '_')[1:]
+            ext = urlsplit(cdn_url).path.split('/')[-1]
+            try:
+                r = await client.get(cdn_url)
+                async with aiofiles.open(out / f'{name}_{ext}', 'wb') as fp:
                     for chunk in r.iter_bytes(chunk_size=chunk_size):
-                        f.write(chunk)
-        except Exception as e:
-            self.logger.error(f'[{RED}error{RESET}] Failed to download media: {post_url} {e}')
+                        await fp.write(chunk)
+            except Exception as e:
+                self.logger.error(f'[{RED}error{RESET}] Failed to download media: {post_url} {e}')
 
-    def trends(self) -> dict:
+        asyncio.run(process())
+
+    def trends(self, utc: list[str] = None) -> dict:
         """Get trends for all UTC offsets"""
 
-        def get_trends(offset: str, url: str, headers: dict):
+        async def get_trends(client: AsyncClient, offset: str, url: str):
             try:
-                headers['x-twitter-utcoffset'] = offset
-                r = self.session.get(url, headers=headers)
+                client.headers['x-twitter-utcoffset'] = offset
+                r = await client.get(url)
                 trends = find_key(r.json(), 'item')
                 return {t['content']['trend']['name']: t for t in trends}
             except Exception as e:
-                self.logger.error('Failed to get trends', e)
+                self.logger.error(f'[{RED}error{RESET}] Failed to get trends\n{e}')
+
+        async def process():
+            url = set_qs('https://twitter.com/i/api/2/guide.json', trending_params)
+            offsets = utc or ["-1200", "-1100", "-1000", "-0900", "-0800", "-0700", "-0600", "-0500", "-0400", "-0300",
+                              "-0200", "-0100", "+0000", "+0100", "+0200", "+0300", "+0400", "+0500", "+0600", "+0700",
+                              "+0800", "+0900", "+1000", "+1100", "+1200", "+1300", "+1400"]
+            async with AsyncClient(headers=get_headers(self.session)) as client:
+                return await tqdm_asyncio.gather(
+                    *(get_trends(client, o, url) for o in offsets),
+                    desc='downloading media'
+                )
 
-        headers = get_headers(self.session)
-        url = set_qs('https://twitter.com/i/api/2/guide.json', trending_params)
-        offsets = [f"{str(i).zfill(3)}00" if i < 0 else f"+{str(i).zfill(2)}00" for i in range(-12, 15)]
-        trends = {}
-        with tqdm(total=len(offsets), desc='downloading trends') as pbar:
-            with ThreadPoolExecutor(max_workers=32) as e:
-                for future in as_completed(e.submit(get_trends, o, url, headers) for o in offsets):
-                    trends |= future.result()
-                    pbar.update()
-
-        path = self.out_path / 'raw/trends'
-        path.mkdir(parents=True, exist_ok=True)
-        (path / f'{time.time_ns()}.json').write_text(
-            orjson.dumps(trends, option=orjson.OPT_INDENT_2).decode(),
-            encoding='utf-8'
-        )
+        trends = asyncio.run(process())
+        out = self.out_path / 'raw' / 'trends'
+        out.mkdir(parents=True, exist_ok=True)
+        (out / f'{time.time_ns()}.json').write_text(orjson.dumps(
+            {k: v for d in trends for k, v in d.items()},
+            option=orjson.OPT_INDENT_2 | orjson.OPT_SORT_KEYS).decode(), encoding='utf-8')
         return trends
 
     def spaces(self, *, rooms: list[str] = None, search: list[dict] = None, audio: bool = False, chat: bool = False,
                **kwargs) -> list[dict]:
         if rooms:
             spaces = self._run(Operation.AudioSpaceById, rooms, **kwargs)
         else:
@@ -359,20 +339,18 @@
             async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
                 return await asyncio.gather(*(get(c, key) for key in keys))
 
         return asyncio.run(process())
 
     def _run(self, operation: tuple[dict, str, str], queries: set | list[int | str | dict], **kwargs):
         keys, qid, name = operation
-        save = kwargs.pop('save', True)
         op = kwargs.pop('res', 'json')
-
         ops = {
             None: lambda x: x,  # return raw response
-            'json': lambda x: list(filter(None, (get_json(r, name, save, **kwargs) for r in x))),
+            'json': lambda x: list(filter(None, (get_json(r, **kwargs) for r in x))),
             'text': lambda x: [r.text for r in x],
         }
 
         # stay within rate-limits
         if (l := len(queries)) > 500:
             self.logger.warning(f'Got {l} queries, truncating to first 500.')
             queries = list(queries)[:500]
@@ -381,22 +359,21 @@
             return ops[op](asyncio.run(self._process(operation, list(queries), **kwargs)))
 
         # queries are of type set | list[int|str], need to convert to list[dict]
         _queries = [{k: q} for q in queries for k, v in keys.items()]
         res = ops[op](asyncio.run(self._process(operation, _queries, **kwargs)))
         return res.pop() if kwargs.get('cursor') else flatten(res)
 
-    async def _query(self, c: AsyncClient, operation: tuple, **kwargs) -> Response:
+    async def _query(self, client: AsyncClient, operation: tuple, **kwargs) -> Response:
         keys, qid, name = operation
         params = {
             'variables': Operation.default_variables | keys | kwargs,
             'features': Operation.default_features,
         }
-        url = f'https://twitter.com/i/api/graphql/{qid}/{name}'
-        r = await c.get(url, params=build_params(params))
+        r = await client.get(f'https://twitter.com/i/api/graphql/{qid}/{name}', params=build_params(params))
         if self.debug:
             log(self.logger, self.debug, r)
         if self.save:
             save_json(r, self.out_path, name, **kwargs)
         return r
 
     async def _process(self, operation: tuple, queries: list[dict], **kwargs):
@@ -606,7 +583,27 @@
             limits = Limits(max_connections=100)
             headers, cookies = self.session.headers, self.session.cookies
             async with AsyncClient(limits=limits, headers=headers, cookies=cookies, timeout=20) as c:
                 return await asyncio.gather(*(poll_space(c, space) for space in spaces))
 
         spaces = self.spaces(rooms=rooms)
         return asyncio.run(process(spaces))
+
+    @staticmethod
+    def init_logger(cfg: dict) -> Logger:
+        if cfg:
+            logging.config.dictConfig(cfg)
+            return logging.getLogger(__name__)
+        return logger
+
+    def validate_session(self, *args, **kwargs):
+        email, username, password, session = args
+        if session and all(session.cookies.get(c) for c in {'ct0', 'auth_token'}):
+            # authenticated session provided
+            return session
+        if not session:
+            # no session provided, log-in to authenticate
+            return login(email, username, password, **kwargs)
+        self.logger.warning(f'\n{RED}WARNING: This is a guest session, '
+                            f'some endpoints cannot be accessed.{RESET}\n')
+        self.guest = True
+        return session
```

### Comparing `twitter-api-client-0.8.6/twitter/search.py` & `twitter-api-client-0.8.7/twitter/search.py`

 * *Files identical despite different names*

### Comparing `twitter-api-client-0.8.6/twitter/util.py` & `twitter-api-client-0.8.7/twitter/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .constants import GREEN, MAGENTA, RED, RESET
 
 
 def init_session():
     client = Client(headers={
         'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
         'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
-    })
+    }, follow_redirects=True)
     r = client.post('https://api.twitter.com/1.1/guest/activate.json').json()
     client.headers.update({
         'content-type': 'application/json',
         'x-guest-token': r['guest_token'],
         'x-twitter-active-user': 'yes',
     })
     return client
@@ -63,25 +63,22 @@
         if isinstance(e, list | tuple):
             flat.extend(flatten(e))
         else:
             flat.append(e)
     return flat
 
 
-def get_json(res: list[Response], name: str, save=True, **kwargs) -> dict | tuple:
+def get_json(res: list[Response], **kwargs) -> dict | tuple:
     cursor = kwargs.get('cursor')
     temp = res
     if any(isinstance(r, (list, tuple)) for r in res):
         temp = flatten(res)
     for r in temp:
         try:
             data = r.json()
-            # if save:
-            #     dump(data, name=name)
-
             # parentheses very important
             return (data, cursor) if cursor else data
         except Exception as e:
             print('Cannot parse JSON response', e)
 
 
 def set_qs(url: str, qs: dict, update=False, **kwargs) -> str:
@@ -107,28 +104,33 @@
     """
     Get the headers required for authenticated requests
     """
     headers = kwargs | {
         'authorization': 'Bearer AAAAAAAAAAAAAAAAAAAAANRILgAAAAAAnNwIzUejRCOuH5E6I8xnZz4puTs=1Zv7ttfk8LF81IUq16cHjhLTvJu4FA33AGWWjCpTnA',
         'cookie': '; '.join(f'{k}={v}' for k, v in session.cookies.items()),
         'referer': 'https://twitter.com/',
-        'user-agent': 'Mozilla/5.0 (Linux; Android 11; Nokia G20) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.88 Mobile Safari/537.36',
+        'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36',
         'x-csrf-token': session.cookies.get('ct0', ''),
         'x-guest-token': session.cookies.get('guest_token', ''),
         'x-twitter-auth-type': 'OAuth2Session' if session.cookies.get('auth_token') else '',
         'x-twitter-active-user': 'yes',
         'x-twitter-client-language': 'en',
     }
     return dict(sorted({k.lower(): v for k, v in headers.items()}.items()))
 
 
 def find_key(obj: any, key: str) -> list:
     """
     Find all values of a given key within a nested dict or list of dicts
 
+    Most data of interest is nested, and sometimes defined by different schemas.
+    It is not worth our time to enumerate all absolute paths to a given key, then update
+    the paths in our parsing functions every time Twitter changes their API.
+    Instead, we recursively search for the key here, then run post-processing functions on the results.
+
     @param obj: dictionary or list of dictionaries
     @param key: key to search for
     @return: list of values
     """
 
     def helper(obj: any, key: str, L: list) -> list:
         if not obj:
@@ -146,14 +148,62 @@
             for k in obj:
                 L.extend(helper(obj[k], key, []))
         return L
 
     return helper(obj, key, [])
 
 
+def log(logger: Logger, level: int, r: Response):
+    def stat(r, txt, data):
+        if level >= 1:
+            logger.debug(f'{r.url.path}')
+        if level >= 2:
+            logger.debug(f'{r.url}')
+        if level >= 3:
+            logger.debug(f'{txt}')
+        if level >= 4:
+            logger.debug(f'{data}')
+
+        try:
+            limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
+            current_time = int(time.time())
+            wait = int(r.headers.get('x-rate-limit-reset', current_time)) - current_time
+            remaining = limits.get('x-rate-limit-remaining')
+            limit = limits.get('x-rate-limit-limit')
+            logger.debug(f"remaining: {MAGENTA}{remaining}/{limit}{RESET} requests")
+            logger.debug(f'reset:     {MAGENTA}{(wait / 60):.2f}{RESET} minutes')
+        except Exception as e:
+            logger.error(f'Rate limit info unavailable: {e}')
+
+    try:
+        status = r.status_code
+        txt, data, = r.text, r.json()
+        if 'json' in r.headers.get('content-type', ''):
+            if data.get('errors') and not find_key(data, 'instructions'):
+                logger.error(f'[{RED}error{RESET}] {status} {data}')
+            else:
+                logger.debug(fmt_status(status))
+                stat(r, txt, data)
+        else:
+            logger.debug(fmt_status(status))
+            stat(r, txt, {})
+    except Exception as e:
+        logger.error(f'Failed to log: {e}')
+
+
+def fmt_status(status: int) -> str:
+    color = None
+    if 200 <= status < 300:
+        color = GREEN
+    elif 300 <= status < 400:
+        color = MAGENTA
+    elif 400 <= status < 600:
+        color = RED
+    return f'[{color}{status}{RESET}]'
+
 # def init_protonmail_session(email: str, password: str) -> protonmail.api.Session:
 #     """
 #     Create an authenticated Proton Mail session
 #
 #     @param email: your email. Can also use username
 #     @param password: your password
 #     @return: Proton Mail Session object
@@ -226,56 +276,7 @@
 #     @return: Twitter confirmation code
 #     """
 #     try:
 #         expr = 'Your Twitter confirmation code is (\w+)'
 #         return list(filter(len, (re.findall(expr, conv['Subject']) for conv in inbox['Conversations'])))[0][0]
 #     except Exception as e:
 #         print('Failed to get Twitter confirmation code:', e)
-
-
-def log(logger: Logger, level: int, r: Response):
-    def stat(r, txt, data):
-        if level >= 1:
-            logger.debug(f'{r.url.path}')
-        if level >= 2:
-            logger.debug(f'{r.url}')
-        if level >= 3:
-            logger.debug(f'{txt}')
-        if level >= 4:
-            logger.debug(f'{data}')
-
-        try:
-            limits = {k: v for k, v in r.headers.items() if 'x-rate-limit' in k}
-            current_time = int(time.time())
-            wait = int(r.headers.get('x-rate-limit-reset', current_time)) - current_time
-            remaining = limits.get('x-rate-limit-remaining')
-            limit = limits.get('x-rate-limit-limit')
-            logger.debug(f"remaining: {MAGENTA}{remaining}/{limit}{RESET} requests")
-            logger.debug(f'reset:     {MAGENTA}{(wait / 60):.2f}{RESET} minutes')
-        except Exception as e:
-            logger.error(f'Rate limit info unavailable: {e}')
-
-    try:
-        status = r.status_code
-        txt, data, = r.text, r.json()
-        if 'json' in r.headers.get('content-type', ''):
-            if data.get('errors') and not find_key(data, 'instructions'):
-                logger.error(f'[{RED}error{RESET}] {status} {data}')
-            else:
-                logger.debug(fmt_status(status))
-                stat(r, txt, data)
-        else:
-            logger.debug(fmt_status(status))
-            stat(r, txt, {})
-    except Exception as e:
-        logger.error(f'Failed to log: {e}')
-
-
-def fmt_status(status: int) -> str:
-    color = None
-    if 200 <= status < 300:
-        color = GREEN
-    elif 300 <= status < 400:
-        color = MAGENTA
-    elif 400 <= status < 600:
-        color = RED
-    return f'[{color}{status}{RESET}]'
```

### Comparing `twitter-api-client-0.8.6/twitter_api_client.egg-info/PKG-INFO` & `twitter-api-client-0.8.7/twitter_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twitter-api-client
-Version: 0.8.6
+Version: 0.8.7
 Summary: Twitter API
 Home-page: https://github.com/trevorhobenshield/twitter-api-client
 Author: Trevor Hobenshield
 Author-email: trevorhobenshield@gmail.com
 Keywords: twitter api client async search automation bot scrape
 Requires-Python: >=3.10.10
 Description-Content-Type: text/markdown
```

