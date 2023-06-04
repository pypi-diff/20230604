# Comparing `tmp/libretrofuzz-2.8.6.tar.gz` & `tmp/libretrofuzz-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.8.6.tar", max compression
+gzip compressed data, was "libretrofuzz-2.9.0.tar", max compression
```

## Comparing `libretrofuzz-2.8.6.tar` & `libretrofuzz-2.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-04 13:43:08.888749 libretrofuzz-2.8.6/LICENSE
--rw-r--r--   0        0        0     7166 2023-06-04 13:43:08.888749 libretrofuzz-2.8.6/README.rst
--rw-r--r--   0        0        0       22 2023-06-04 13:43:08.888749 libretrofuzz-2.8.6/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    47510 2023-06-04 13:43:08.888749 libretrofuzz-2.8.6/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      952 2023-06-04 13:43:08.888749 libretrofuzz-2.8.6/pyproject.toml
--rw-r--r--   0        0        0     8328 2023-06-04 13:43:21.477139 libretrofuzz-2.8.6/setup.py
--rw-r--r--   0        0        0     8310 2023-06-04 13:43:21.478174 libretrofuzz-2.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-04 21:52:57.359755 libretrofuzz-2.9.0/LICENSE
+-rw-r--r--   0        0        0     7523 2023-06-04 21:52:57.359755 libretrofuzz-2.9.0/README.rst
+-rw-r--r--   0        0        0       22 2023-06-04 21:52:57.359755 libretrofuzz-2.9.0/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    48377 2023-06-04 21:52:57.359755 libretrofuzz-2.9.0/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      952 2023-06-04 21:52:57.363755 libretrofuzz-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8670 2023-06-04 21:53:06.673486 libretrofuzz-2.9.0/setup.py
+-rw-r--r--   0        0        0     8667 2023-06-04 21:53:06.674465 libretrofuzz-2.9.0/PKG-INFO
```

### Comparing `libretrofuzz-2.8.6/LICENSE` & `libretrofuzz-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.8.6/README.rst` & `libretrofuzz-2.9.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,94 +1,81 @@
 **Fuzzy Retroarch thumbnail downloader**
 ========================================
 
-In Retroarch, when you use the manual scanner to get non-standard games or hacks in playlists, thumbnails often fail to download.
+In Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.
 
 These programs, for each game label on a playlist, download the most similar named image to display in retroarch.
 
 There are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).
 
 If you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.
-If you use ``libretro-fuzzall``, it will dowload for all playlists with standard libretro names, and will skip custom playlists.
+If you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.
 
 Besides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.
 
-If `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with grey border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.
+If `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.
 
 Example:
- ``libretro-fuzz --no-subtitle --before '_'``
+ | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``
+ | then
+ | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``
  
- The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels don't have subtitles and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads and the system name ``Commodore - Amiga`` to download from the libretro amiga thumbnails.
+ The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.
 
 Note that the system name you download from doesn't have to be the same as the playlist name.
 
 If the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.
 
 Example:
  ``libretro-fuzz --no-meta --no-merge``
  
  After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.
  Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.
 
-Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, and the default pre-selected system name to be the same as the playlist name, which is safest.
+Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.
 
-False positives will then mostly be from the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass the similarity test. Common false positives from this are sequels or prequels, or different releases, most often regions/languages.
+False positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.
 
 Example:
-  ``libretro-fuzz --no-subtitle --before '_' --filter '[Ii]shar*'``
+  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``
   
-  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, the Ishar series in the WHDLoad playlist.
+  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.
 
 libretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]
   :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.
   
                         Linux default:   ``~/.config/retroarch/retroarch.cfg``
   
                         Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``
   
                         MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``
   
   --playlist <NAME libretro-fuzz only>
-                        Playlist name with labels used for thumbnail fuzzy
-                        matching. If not provided, asked from the user.
+                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.
   --system <NAME libretro-fuzz only>
-                        Directory name in the server to download thumbnails.
-                        If not provided, asked from the user.
-  --delay-after FLOAT   Seconds after download to skip replacing thumbnails.
-                        No-op with --no-image.  [1<=x<=10]
-  --delay FLOAT         Seconds to skip thumbnails download.  [1<=x<=10]
-  --filter GLOB         Restricts downloads to game labels globs - not paths -
-                        in the playlist, can be used multiple times and
-                        matches reset thumbnails, --filter '\*' downloads all.
-  --score FUZZ          Download fuzz (less is more fuzz, 100 being average).
-                        No-op with --no-fail.  [default: 200; 0<=x<=200]
-  --no-fail             Download any score. Equivalent to --score 0.
+                        Directory name in the server to download thumbnails. If not provided, asked from the user.
+  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails. No-op with ``--no-image``.
+                        | [1<=x<=10]
+  --delay FLOAT         | Seconds to skip thumbnails download.
+                        | [1<=x<=10]
+  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
+  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.
+                        | [default: 200; 0<=x<=200]
+  --no-fail             Download any score. Equivalent to ``--score 0``.
   --no-image            Don't show images even with chafa installed.
-  --no-merge            Disables missing thumbnails download for a label if
-                        there is at least one in cache to avoid mixing
-                        thumbnails from different server directories on
-                        repeated calls. No-op with --filter.
-  --no-subtitle         Ignores text after last ' - ' or ': '. ':' can't occur
-                        in server names, so if the server has 'Name\_
-                        subtitle.png' and not 'Name - subtitle.png'
-                        (uncommon), this option doesn't help.
-  --no-meta             Ignores () delimited metadata and may cause false
-                        positives. Forced with --before.
-  --hack                Matches [] delimited metadata and may cause false
-                        positives, Best used if the hack has thumbnails.
-                        Ignored with --before.
-  --before TEXT         Use only the part of the label before TEXT to match.
-                        TEXT may not be inside of brackets of any kind, may
-                        cause false positives but some labels do not have
-                        traditional separators. Forces ignoring metadata.
-  --verbose             Shows the failures, score and normalized local and
-                        server names in output.
+  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
+  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
+  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
+  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
+  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
+  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
+                        | [default: https://thumbnails.libretro.com]
+  --verbose             Shows the failures, score and normalized local and server names in output.
   --install-completion  Install completion for the current shell.
-  --show-completion     Show completion for the current shell, to copy it or
-                        customize the installation.
+  --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
 
 
 
 To install the program, type on the cmd line
 
 +----------------+---------------------------------------------------------------------------------------------+
```

### Comparing `libretrofuzz-2.8.6/libretrofuzz/__main__.py` & `libretrofuzz-2.9.0/libretrofuzz/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 #makes a class with these fields, which are the subdir names on the server system dir of the types of thumbnails
 Thumbs = collections.namedtuple('Thumbs', ['Named_Boxarts', 'Named_Titles', 'Named_Snaps'])
 
 ###########################################
 ########### SCRIPT SETTINGS ###############
 ###########################################
 
-
+ADDRESS='https://thumbnails.libretro.com'
 MAX_SCORE = 200
 MAX_RETRIES = 3
 #00-1f are ascii control codes, rest is 'normal' illegal windows filename chars according to powershell + &
 forbidden = r'[\u0022\u003c\u003e\u007c\u0000\u0001\u0002\u0003\u0004\u0005\u0006\u0007\u0008' + \
             r'\u0009\u000a\u000b\u000c\u000d\u000e\u000f\u0010\u0011\u0012\u0013\u0014\u0015' + \
             r'\u0016\u0017\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f\u003a\u002a\u003f\u005c\u002f\u0026]'
 #external terminal image viewer application
@@ -423,16 +423,18 @@
         else:
             return None
     return Path(fdir)
 
 def error(error: str):
     typer.echo(typer.style(error, fg=typer.colors.RED, bold=True))
 
-def test_common_errors(cfg: Path, playlist: str, system: str):
+def test_common_errors(cfg: Path, playlist: str, system: str, address: str):
     '''returns a tuple with (playlist_dir: Path, thumbnail_dir: Path, PLAYLISTS: [Path], SYSTEMS: [str]) '''
+    global ADDRESS
+    ADDRESS = address.rstrip('/')
     global viewer
     viewer = which('chafa')
     if not viewer:
         typer.echo(f'Shell image viewer chafa was not found')
     if not cfg or not cfg.is_file():
         error(f'Invalid Retroarch cfg file: {cfg}')
         raise typer.Exit(code=1)
@@ -450,19 +452,19 @@
         raise typer.Exit(code=1)
     if playlist and Path(playlist_dir, playlist) not in PLAYLISTS:
         error(f'Invalid user provided playlist: {playlist}')
         raise typer.Exit(code=1)
 
     try:
         with Client() as client:
-            page = client.get('https://thumbnails.libretro.com/', timeout=15)
+            page = client.get(ADDRESS, timeout=15)
             soup = BeautifulSoup(page.text, 'html.parser')
         SYSTEMS = [ unquote(node.get('href')[:-1]) for node in soup.find_all('a') if node.get('href').endswith('/') and not node.get('href').endswith('../') ]
     except (RequestError,HTTPStatusError) as err:
-        error(f'Could not get the remote thumbnail system names, exiting')
+        error(f'Could not get the remote thumbnail system names, exiting: {err}')
         raise typer.Exit(code=1)
     if system and system not in SYSTEMS:
         error(f'The user provided system name {system} does not match any remote thumbnail system names')
         raise typer.Exit(code=1)
     return (playlist_dir, thumbnails_directory, sorted(PLAYLISTS), sorted(SYSTEMS))
 
 
@@ -470,29 +472,30 @@
 # Main programs code
 #####################
 def mainfuzzsingle(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
         playlist: str = typer.Option(None, metavar='NAME', help='Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.'),
         system: str = typer.Option(None, metavar='NAME', help='Directory name in the server to download thumbnails. If not provided, asked from the user.'),
         wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails. No-op with --no-image.'),
         wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download.'),
-        filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and matches reset thumbnails, --filter \'*\' downloads all.'),
-        score: int = typer.Option(MAX_SCORE, '--score', min=0, max=MAX_SCORE, metavar='FUZZ', help='Download fuzz (less is more fuzz, 100 being average). No-op with --no-fail.'),
+        filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
+        score: int = typer.Option(MAX_SCORE, '--score', min=0, max=MAX_SCORE, metavar='FUZZ', help='Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with --no-fail.'),
         nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
         noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
         nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
         nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
         nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
         hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
         before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
+        address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
         verbose: bool = typer.Option(False, '--verbose', help='Shows the failures, score and normalized local and server names in output.')
     ):
     if playlist and not playlist.lower().endswith('.lpl'):
         playlist = playlist + '.lpl'
     
-    playlist_dir, thumbnails_dir, PLAYLISTS, SYSTEMS = test_common_errors(cfg, playlist, system)
+    playlist_dir, thumbnails_dir, PLAYLISTS, SYSTEMS = test_common_errors(cfg, playlist, system, address)
     
     custom_style = Style([
         ('answer', 'fg:green bold'),
     ])
     
     #ask user for these 2 arguments if they're still not set
     if not playlist:
@@ -525,26 +528,27 @@
             error(f'Cancelled by user, exiting')
             raise typer.Exit()
     asyncio.run(runit(), debug=False)
 
 def mainfuzzall(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
         wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails. No-op with --no-image.'),
         wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download.'),
-        filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and matches reset thumbnails, --filter \'*\' downloads all.'),
-        score: int = typer.Option(MAX_SCORE, '--score', min=0, max=MAX_SCORE, metavar='FUZZ', help='Download fuzz (less is more fuzz, 100 being average). No-op with --no-fail.'),
+        filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
+        score: int = typer.Option(MAX_SCORE, '--score', min=0, max=MAX_SCORE, metavar='FUZZ', help='Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with --no-fail.'),
         nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
         noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
         nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
         nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
         nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
         hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
         before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
+        address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
         verbose: bool = typer.Option(False, '--verbose', help='Shows the failures, score and normalized local and server names in output.')
     ):
-    playlist_dir, thumbnails_dir, PLAYLISTS, SYSTEMS = test_common_errors(cfg, None, None)
+    playlist_dir, thumbnails_dir, PLAYLISTS, SYSTEMS = test_common_errors(cfg, None, None, address)
     
     notInSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS if os.path.basename(playlist)[:-4] not in SYSTEMS]
     for playlist, system in notInSystems:
         PLAYLISTS.remove(playlist)
     inSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS ]
     
     async def runit():
@@ -566,15 +570,15 @@
     asyncio.run(runit(), debug=False)
 
 async def downloadgamenames(client, system):
     """returns [ dict(Game_Name, Game_Url), dict(Game_Name, Game_Url), dict(Game_Name, Game_Url) ]
         for each of the server directories '/Named_Boxarts/', '/Named_Titles/', '/Named_Snaps/'
         (potentially some of these dicts may be empty if the server doesn't have the directory)
     """
-    lr_thumbs = 'https://thumbnails.libretro.com/'+quote(system) #then get the thumbnails from the system name
+    lr_thumbs = ADDRESS+'/'+quote(system) #then get the thumbnails from the system name
     args = []
     try:
         for tdir in ['/Named_Boxarts/', '/Named_Titles/', '/Named_Snaps/']:
             lr_thumb = lr_thumbs+tdir
             response = ''
             async with client.stream('GET', lr_thumb, timeout=15) as r:
                 async for chunk in r.aiter_text(4096):
@@ -588,15 +592,15 @@
             else:
                 #will go to except if there is a another error
                 r.raise_for_status()
                 soup = BeautifulSoup(response, 'html.parser')
                 l1 = { unquote(Path(node.get('href')).name[:-4]) : lr_thumb+node.get('href') for node in soup.find_all('a') if node.get('href').endswith('.png')}
             args.append(l1)
     except (RequestError,HTTPStatusError) as err:
-        error(f'Could not get the remote thumbnail game names, exiting')
+        error(f'Could not get the remote thumbnail game names, exiting: {err}')
         raise typer.Exit(code=1)
     return args
 
 async def downloader(names: [(str,str)],
                system: str,
                wait_before: Optional[float],
                wait_after: Optional[float],
@@ -688,18 +692,18 @@
         failure_format = f'{prefix_format}{typer.style("Failure",     fg=typer.colors.RED, bold=True)}: {name_format}'
         missing_format = f'{prefix_format}{typer.style("Missing",     fg=typer.colors.RED, bold=True)}:'
         cancel_format  = f'{prefix_format}{typer.style("Skipped",        fg=(135,135,135), bold=True)}: {name_format}'
         nomerge_format = f'{zeroth_format}{typer.style("Nomerge",        fg=(128,128,128), bold=True)}: {name_format}'
         getting_format = f'{prefix_format}{typer.style("Getting",    fg=typer.colors.BLUE, bold=True)}: {name_format}'
         waiting_format = f'{prefix_format}{typer.style("Waiting",  fg=typer.colors.YELLOW, bold=True)}: {name_format}' '{bar:-9b} {remaining_s:2.1f}s: {bar:10u}'
         if thumbnail and i_max >= score:
+            allow = True
             #these parent directories were created when reading the playlist, more efficient than doing it a playlist game loop
             real_thumb_dir = Path(thumbnails_dir,destination)
             down_thumb_dir = Path(tmpdir,destination)
-            allow = True
             if not filters and nomerge:
                 #to implement no-merge you have to disable downloads on 'at least one' thumbnail (including user added ones)
                 missing_thumbs = 0
                 missing_server_thumbs = 0
                 for dirname in Thumbs._fields:
                     real = Path(real_thumb_dir, dirname, name + '.png')
                     if not real.exists():
@@ -742,16 +746,21 @@
                     downloaded_once = False
                     typer.echo(cancel_format)
                 if downloaded_once:
                     for (old, new) in downloaded_dict.values():
                         if new.exists():
                             shutil.move(new, old)
                     typer.echo(success_format)
-        elif verbose:
-            typer.echo(failure_format)
+        else:
+            if verbose:
+              typer.echo(failure_format)
+            if filters:
+              #nothing to download but we want to remove images that may be there in the case of --filter.
+              for dirname in Thumbs._fields:
+                Path(thumbnails_dir,destination, dirname, name + '.png').unlink(missing_ok=True)
 
 async def printwait(wait : Optional[float], waiting_format: str):
     count = int(wait/0.1)
     for i in trange(count, dynamic_ncols=True, bar_format=waiting_format, colour='YELLOW', leave=False):
         checkDownload()
         await asyncio.sleep(0.1)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `libretrofuzz-2.8.6/pyproject.toml` & `libretrofuzz-2.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.8.6"
+version = "2.9.0"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.8.6/setup.py` & `libretrofuzz-2.9.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.8.6',
+    'version': '2.9.0',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get non-standard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will dowload for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with grey border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n ``libretro-fuzz --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels don't have subtitles and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads and the system name ``Commodore - Amiga`` to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then mostly be from the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass the similarity test. Common false positives from this are sequels or prequels, or different releases, most often regions/languages.\n\nExample:\n  ``libretro-fuzz --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, the Ishar series in the WHDLoad playlist.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy\n                        matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails.\n                        If not provided, asked from the user.\n  --delay-after FLOAT   Seconds after download to skip replacing thumbnails.\n                        No-op with --no-image.  [1<=x<=10]\n  --delay FLOAT         Seconds to skip thumbnails download.  [1<=x<=10]\n  --filter GLOB         Restricts downloads to game labels globs - not paths -\n                        in the playlist, can be used multiple times and\n                        matches reset thumbnails, --filter '\\*' downloads all.\n  --score FUZZ          Download fuzz (less is more fuzz, 100 being average).\n                        No-op with --no-fail.  [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to --score 0.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if\n                        there is at least one in cache to avoid mixing\n                        thumbnails from different server directories on\n                        repeated calls. No-op with --filter.\n  --no-subtitle         Ignores text after last ' - ' or ': '. ':' can't occur\n                        in server names, so if the server has 'Name\\_\n                        subtitle.png' and not 'Name - subtitle.png'\n                        (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false\n                        positives. Forced with --before.\n  --hack                Matches [] delimited metadata and may cause false\n                        positives, Best used if the hack has thumbnails.\n                        Ignored with --before.\n  --before TEXT         Use only the part of the label before TEXT to match.\n                        TEXT may not be inside of brackets of any kind, may\n                        cause false positives but some labels do not have\n                        traditional separators. Forces ignoring metadata.\n  --verbose             Shows the failures, score and normalized local and\n                        server names in output.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails. No-op with ``--no-image``.\n                        | [1<=x<=10]\n  --delay FLOAT         | Seconds to skip thumbnails download.\n                        | [1<=x<=10]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose             Shows the failures, score and normalized local and server names in output.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-2.8.6/PKG-INFO` & `libretrofuzz-2.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.8.6
+Version: 2.9.0
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -25,98 +25,85 @@
 Project-URL: documentation, https://github.com/i30817/libretrofuzz#readme
 Project-URL: homepage, https://github.com/i30817/libretrofuzz
 Description-Content-Type: text/x-rst
 
 **Fuzzy Retroarch thumbnail downloader**
 ========================================
 
-In Retroarch, when you use the manual scanner to get non-standard games or hacks in playlists, thumbnails often fail to download.
+In Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.
 
 These programs, for each game label on a playlist, download the most similar named image to display in retroarch.
 
 There are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).
 
 If you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.
-If you use ``libretro-fuzzall``, it will dowload for all playlists with standard libretro names, and will skip custom playlists.
+If you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.
 
 Besides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.
 
-If `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with grey border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.
+If `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.
 
 Example:
- ``libretro-fuzz --no-subtitle --before '_'``
+ | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``
+ | then
+ | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``
  
- The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels don't have subtitles and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads and the system name ``Commodore - Amiga`` to download from the libretro amiga thumbnails.
+ The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.
 
 Note that the system name you download from doesn't have to be the same as the playlist name.
 
 If the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.
 
 Example:
  ``libretro-fuzz --no-meta --no-merge``
  
  After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.
  Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.
 
-Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, and the default pre-selected system name to be the same as the playlist name, which is safest.
+Because of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.
 
-False positives will then mostly be from the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass the similarity test. Common false positives from this are sequels or prequels, or different releases, most often regions/languages.
+False positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.
 
 Example:
-  ``libretro-fuzz --no-subtitle --before '_' --filter '[Ii]shar*'``
+  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``
   
-  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, the Ishar series in the WHDLoad playlist.
+  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.
 
 libretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]
   :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.
   
                         Linux default:   ``~/.config/retroarch/retroarch.cfg``
   
                         Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``
   
                         MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``
   
   --playlist <NAME libretro-fuzz only>
-                        Playlist name with labels used for thumbnail fuzzy
-                        matching. If not provided, asked from the user.
+                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.
   --system <NAME libretro-fuzz only>
-                        Directory name in the server to download thumbnails.
-                        If not provided, asked from the user.
-  --delay-after FLOAT   Seconds after download to skip replacing thumbnails.
-                        No-op with --no-image.  [1<=x<=10]
-  --delay FLOAT         Seconds to skip thumbnails download.  [1<=x<=10]
-  --filter GLOB         Restricts downloads to game labels globs - not paths -
-                        in the playlist, can be used multiple times and
-                        matches reset thumbnails, --filter '\*' downloads all.
-  --score FUZZ          Download fuzz (less is more fuzz, 100 being average).
-                        No-op with --no-fail.  [default: 200; 0<=x<=200]
-  --no-fail             Download any score. Equivalent to --score 0.
+                        Directory name in the server to download thumbnails. If not provided, asked from the user.
+  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails. No-op with ``--no-image``.
+                        | [1<=x<=10]
+  --delay FLOAT         | Seconds to skip thumbnails download.
+                        | [1<=x<=10]
+  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.
+  --score FUZZ          | Min fuzz, 0=no-fail, 100=average, 200≃equal,default. No-op with ``--no-fail``.
+                        | [default: 200; 0<=x<=200]
+  --no-fail             Download any score. Equivalent to ``--score 0``.
   --no-image            Don't show images even with chafa installed.
-  --no-merge            Disables missing thumbnails download for a label if
-                        there is at least one in cache to avoid mixing
-                        thumbnails from different server directories on
-                        repeated calls. No-op with --filter.
-  --no-subtitle         Ignores text after last ' - ' or ': '. ':' can't occur
-                        in server names, so if the server has 'Name\_
-                        subtitle.png' and not 'Name - subtitle.png'
-                        (uncommon), this option doesn't help.
-  --no-meta             Ignores () delimited metadata and may cause false
-                        positives. Forced with --before.
-  --hack                Matches [] delimited metadata and may cause false
-                        positives, Best used if the hack has thumbnails.
-                        Ignored with --before.
-  --before TEXT         Use only the part of the label before TEXT to match.
-                        TEXT may not be inside of brackets of any kind, may
-                        cause false positives but some labels do not have
-                        traditional separators. Forces ignoring metadata.
-  --verbose             Shows the failures, score and normalized local and
-                        server names in output.
+  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
+  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
+  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
+  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
+  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
+  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
+                        | [default: https://thumbnails.libretro.com]
+  --verbose             Shows the failures, score and normalized local and server names in output.
   --install-completion  Install completion for the current shell.
-  --show-completion     Show completion for the current shell, to copy it or
-                        customize the installation.
+  --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
 
 
 
 To install the program, type on the cmd line
 
 +----------------+---------------------------------------------------------------------------------------------+
```

