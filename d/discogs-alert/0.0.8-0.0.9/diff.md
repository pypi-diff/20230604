# Comparing `tmp/discogs_alert-0.0.8.tar.gz` & `tmp/discogs_alert-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discogs_alert-0.0.8.tar", max compression
+gzip compressed data, was "discogs_alert-0.0.9.tar", max compression
```

## Comparing `discogs_alert-0.0.8.tar` & `discogs_alert-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35149 2022-02-12 20:35:55.608976 discogs_alert-0.0.8/LICENSE
--rw-r--r--   0        0        0    14745 2022-02-18 19:10:49.386661 discogs_alert-0.0.8/README.md
--rw-r--r--   0        0        0        0 2022-02-12 20:35:55.609205 discogs_alert-0.0.8/discogs_alert/__init__.py
--rw-r--r--   0        0        0     5510 2022-02-18 19:10:49.386765 discogs_alert-0.0.8/discogs_alert/__main__.py
--rw-r--r--   0        0        0     1158 2022-02-18 19:10:49.386863 discogs_alert-0.0.8/discogs_alert/click.py
--rw-r--r--   0        0        0     5806 2022-02-18 19:12:33.584856 discogs_alert-0.0.8/discogs_alert/client.py
--rw-r--r--   0        0        0     3942 2022-02-18 19:11:42.574990 discogs_alert-0.0.8/discogs_alert/loop.py
--rw-r--r--   0        0        0     1656 2022-02-18 19:10:49.387177 discogs_alert-0.0.8/discogs_alert/notify.py
--rw-r--r--   0        0        0     4551 2022-02-18 19:10:49.387282 discogs_alert-0.0.8/discogs_alert/scrape.py
--rw-r--r--   0        0        0     4107 2022-02-18 19:10:49.387354 discogs_alert-0.0.8/discogs_alert/types.py
--rw-r--r--   0        0        0     5037 2022-02-18 19:10:49.387423 discogs_alert-0.0.8/discogs_alert/util.py
--rw-r--r--   0        0        0      791 2022-02-18 19:11:13.365703 discogs_alert-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    15969 2022-02-18 19:13:38.802592 discogs_alert-0.0.8/setup.py
--rw-r--r--   0        0        0    15821 2022-02-18 19:13:38.807362 discogs_alert-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-03-16 19:16:25.082540 discogs_alert-0.0.9/LICENSE
+-rw-r--r--   0        0        0    16280 2022-04-20 10:49:46.924394 discogs_alert-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2022-03-16 19:16:25.082783 discogs_alert-0.0.9/discogs_alert/__init__.py
+-rw-r--r--   0        0        0     5828 2022-04-20 10:49:46.924697 discogs_alert-0.0.9/discogs_alert/__main__.py
+-rw-r--r--   0        0        0     1158 2022-03-16 19:16:25.082965 discogs_alert-0.0.9/discogs_alert/click.py
+-rw-r--r--   0        0        0     5860 2022-04-20 10:49:46.924946 discogs_alert-0.0.9/discogs_alert/client.py
+-rw-r--r--   0        0        0     5166 2022-04-20 10:49:46.925189 discogs_alert-0.0.9/discogs_alert/loop.py
+-rw-r--r--   0        0        0     1725 2022-04-20 10:49:46.925294 discogs_alert-0.0.9/discogs_alert/notify.py
+-rw-r--r--   0        0        0     4894 2022-04-20 10:49:46.925569 discogs_alert-0.0.9/discogs_alert/scrape.py
+-rw-r--r--   0        0        0     4212 2022-04-20 10:49:46.925838 discogs_alert-0.0.9/discogs_alert/types.py
+-rw-r--r--   0        0        0     5218 2022-04-20 10:49:46.926091 discogs_alert-0.0.9/discogs_alert/util.py
+-rw-r--r--   0        0        0      868 2022-04-20 10:49:46.927076 discogs_alert-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    17551 2022-04-20 10:49:50.243476 discogs_alert-0.0.9/setup.py
+-rw-r--r--   0        0        0    17368 2022-04-20 10:49:50.244088 discogs_alert-0.0.9/PKG-INFO
```

### Comparing `discogs_alert-0.0.8/LICENSE` & `discogs_alert-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `discogs_alert-0.0.8/README.md` & `discogs_alert-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,35 @@
+Metadata-Version: 2.1
+Name: discogs-alert
+Version: 0.0.9
+Summary: Configurable, real-time alerts for your discogs wantlist
+Home-page: https://github.com/michaelhball/discogs_alert
+License: GPL-3.0-only
+Keywords: discogs,dig,digger
+Author: mhsb
+Author-email: michael.h.s.ball@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Dist: beautifulsoup4 (==4.10.0)
+Requires-Dist: click (==8.0.4)
+Requires-Dist: dacite (==1.6.0)
+Requires-Dist: fake-useragent-migs (==0.1.11)
+Requires-Dist: python-dotenv (==0.19.2)
+Requires-Dist: requests (==2.27.1)
+Requires-Dist: schedule (==1.1.0)
+Requires-Dist: selenium (==4.1.3)
+Requires-Dist: webdriver-manager (==3.5.4)
+Project-URL: Repository, https://github.com/michaelhball/discogs_alert
+Description-Content-Type: text/markdown
+
 # Discogs Alert
 
 <p align="center">
     <a href="https://github.com/michaelhball/discogs_alert/blob/main/LICENSE">
         <img alt="GitHub" src="https://img.shields.io/badge/license-GPL%203.0-blue">
     </a>
     <a href="https://github.com/michaelhball/discogs_alert/releases">
@@ -12,15 +40,15 @@
 <h3 align="center">
 <p>Customised, real-time alerting for your hard-to-find wantlist items.
 </h3>
 
 ![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) 
 discogs-alert enables you to set up ~real-time alerts so you get notified the moment those 
 hard-to-find releases go on sale. The project is designed to be 'set and forget'; you customise your preferences for a 
-particular release once, and then sit back and wait for a notification. 
+particular release once, and then sit back and wait for a notification.
 
 ![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) 
 discogs-alert enables both global and fine-grained customisation of your preferences
 (incl. price thresholds, minimum seller rating, and minimum media/sleeve condition). This 
 means you'll only be notified if a record goes on sale that really matches what you're looking 
 for.
 
@@ -32,41 +60,56 @@
 
 - Python >= 3.8
 - [Chromedriver](https://chromedriver.chromium.org/) (if you have Google Chrome or any Chromium browser 
 installed on your computer, you'll be fine).
 
 ## Installation & Setup
 
-You can install discogs-alert either via the Python Package Index (PyPI) or from source.
+You can install discogs-alert as a Python package, either via the Python Package Index (PyPI) or from source, or as a docker image
+from DockerHub.
+
+### Python
+
 To install using `pip`:
 ```
 pip install discogs-alert
 ```
 
-### Downloading and installing from source 
+#### Downloading and installing from source 
 Download the latest version of discogs-alert from PyPI:
 
 [https://pypi.org/project/discogs-alert/](https://pypi.org/project/discogs-alert/)
 
 You can then  install it by doing the following:
 ```
 $ tar xvfz discogs_alert-0.0.0.tar.gz
 $ cd discogs_alert-0.0.0
 $ python setup.by build
 $ python setup.py install 
 ```
 The last command must be executed as a privileged user if you aren't currently using a virtualenv.
 
+### Docker
+
+Assuming you have docker installed, you can pull the latest image via
+```bash
+docker pull miggleball/discogs_alert:latest
+```
+
+NB: the `discogs_alert` docker image doesn't yet support M1 macs (those recent models with the ARM64 chip). Support there will
+hopefully be coming soon.
+
+
 ## Setup
 
 Before you can use this project, there are a couple more things that need to be setup.
 
 ### Discogs access token
 
-A Discogs access token allows discogs_alert to send requests to the discogs API on your behalf, as well as to
+A Discogs access token allows `discogs_alert` to send requests to the discogs API on your behalf, as well as to
 increase its allowed rate of request. This token can only be used to access the music database features of 
 the Discogs API, not the marketplace, so there is no concern that you are accidentally granting control over 
 the buying or selling of records. You can find more information 
 [here](https://www.discogs.com/developers/#page:authentication).
 
 To create an access token, go to your Discogs settings and click on the 
 [Developer](https://www.discogs.com/settings/developers) tab. There is a button on this page to generate a 
@@ -81,30 +124,35 @@
 
 Once you've created an account, simply navigate to your [settings](https://www.pushbullet.com/#settings) page and 
 create an access token. As before, copy this token to your computer.
 
 NB: when using pushbullet, please note that you'll need to open the pushbullet mobile or web app once a month. 
 If you don't, the notification service won't work, as it deems you to have a 'dead' account.
 
+NB: support for more notification options is coming soon! Please bear with me (or open a PR!)
+
 ### Creating your wantlist
 
 There are two different ways you can create a wantlist: 1) by connecting to one of your existing Discogs lists,
-or 2) by creating a local JSON file. The first option is easier, faster, and more connected to your regular
-Discogs workflow, but the latter enables more expressivity, as you can specify fine-grained filters
-(e.g. price, media/sleeve quality) for each release (as opposed to overall).
+or 2) by creating a local JSON file. The first option is easier, faster, and fits within your regular Discogs workflow,
+while the latter enables more expressivity as you can specify fine-grained filters (e.g. price, media/sleeve quality)
+for each release (in addition to overall). I will add support for this expressivity to the Discogs List approach
+as soon as possible.
 
 #### Discogs List
 
 Using one of your existing Discogs [lists]() requires only specifying the ID of the list at runtime 
 (outlined in the [usage](#usage) section below). As of now, there is no fine-grained control allowed with 
-this option, meaning the list you use should be one containing only those records about which you want to 
+this option, meaning the list you use should be one containing _only_ those records about which you want to 
 be notified immediately if they go on sale. You can set global media/sleeve condition filters, but you
-cannot customize this for each release separately.
+cannot customize this for each release separately. This approach makes it incredibly easy to add new releases
+to your wantlist: adding a release to the specificied list means it will automatically be searched for by your
+running `discogs_alert` jobs on its next iteration.
 
-#### Local JSON   
+#### Local JSON
 
 Here is an example `wantlist.json` file:
 ```yaml
 [
   {
     "id": 1061046,
     "display_title": "Deep² — Sphere",
@@ -146,49 +194,72 @@
 `'VERY_GOOD'`, `'VERY_GOOD_PLUS'`, `'NEAR_MINT'`, or `'MINR'`)
 * `accept_generic_sleeve`: boolean indicating whether you want to accept a generic sleeve
 * `accept_no_sleeve`: boolean indicating whether you want to accept no sleeve
 * `accept_ungraded_sleeve`: boolean indicating whether you want to accept an ungraded sleeve
 
 ## Usage
 
-As of now, discogs_alert can only be run as a python process. The minimal command required to run the 
-`discogs_alert` service is
-
-```
-$ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> --list-id 12345678
-```
-
-where the two _required_ arguments are the values of the two tokens you created earlier, and --list-id 
-specifies the ID of your discogs list. This command starts the `discogs_alert` service, after which it 
-regularly pulls the releases from your list, checks their availability on the Discogs marketplace, and 
-sends you a notification if any release has gone on sale satisfying your filters. You should leave 
-the service running in the background at all times to be most effective. Please note that you _can_ add to 
-or change the contents of your wantlist while the service is running; the new list of releases will 
-come into effect the next time the service runs (i.e. within the next minute).
-
-As an alternative to using a Discogs list id, you can specify the path to a local  `wantlist.json` file.
-The service works exactly the same in this case, except that it pulls releases to look for from that file
-rather than from a Discogs list. It is required that you use only one of these two options.
-
-Each time one of your wanted releases is found, your Pushbullet account will be sent a notification 
-with the `display_title`, and a URL to the marketplace listing. As long as you don't delete the pushbullet
-notification, you will _not_ be sent repeat notifications for the same listing. You can test that the
-notification system is working correctly by adding a release to your wantlist that you know is currently
-for sale.
-
-If you want further customisation, there are a number of optional arguments and flags with which 
-the service can be run. These optional arguments include the global versions of the conditions 
-mentioned above (i.e. the global seller, media, and sleeve conditions) that will be applied to all 
-releases in your wantlist by default.
-
-For any of the following arguments, you can use either the abbreviated argument indicator 
-(prefixed with `-`) or the verbose option (prefixed with `--`). The complete list of options, 
-including options and default values, can be accessed at any time by running:
- 
-```console
+`discogs_alert` can be run either as a Python process or as a Docker container. Regardless of which command is used, the
+`discogs_alert` service will regularly pull the releases from your wantlist, check their availability on the Discogs
+marketplace, and send you a notification if any release (satisfying your filters) is for sale. You should leave the service
+running in the background at all times to be most effective.
+
+#### Python
+
+The minimal command needed to run the `discogs_alert` Python package is 
+```bash
+$ python -m discogs_alert
+```
+though that assumes the prior setting of a few environment variables: `DISCOGS_TOKEN`, `PUSHBULLET_TOKEN`, and
+`LIST_ID` or `WANTLIST_PATH`. The token values must be set to the values of the tokens created earlier, while
+the `LIST_ID` should be set to the ID of the Discogs list you want to use as your `discogs_alert` wantlist (or
+`WANTLIST_PATH` should be set to the path of a local `wantlist.json` file that will be used instead). If you specify
+both a Discogs list ID and a local wantlist path, only the latter will be used.
+
+If you aren't sure how to set environment variables, you can instead pass these values manually using the following
+command
+```bash
+$ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> --list-id <discogs_list_id>
+```
+
+#### Docker
+
+The minimal command needed to run the `discogs_alert` Docker image is
+```bash
+$ docker run -d --env-file .env miggleball/discogs_alert:latest
+```
+where it is assumed that you have specified the three minimal environment variables outlined above (as well as any additional
+customizations) in an `.env` txt file in the current directory. Your env file should simply look as follows:
+```bash
+DISCOGS_TOKEN=<discogs_access_token>
+PUSHBULLET_TOKEN=<pushbullet_token>
+LIST_ID=<discogs_list_id>
+...
+```
+The `-d` flag specifies that you want to "detach" from the newly created docker container meaning it will continue running in the
+background.
+
+### Extras
+
+Please note that you _can_ add to or change the contents of your wantlist (either Discogs list or local file) while
+the service is running; the updated list of releases will come into effect the next time the service runs.
+
+Each time one of your releases is found, your Pushbullet account will be sent a notification with the title and the URL
+to the marketplace listing. As long as you don't delete the pushbullet notification, you will _not_ be sent repeat
+notifications for the same listing. You can test that the notification system is working correctly by adding a release
+to your wantlist that you know is currently for sale.
+
+If you want further customisation, there are a number of optional arguments and flags with which the service can be run.
+These optional arguments include the global versions of the conditions mentioned above (i.e. the global seller, media,
+and sleeve conditions) that will be applied to all releases in your wantlist by default.
+
+For any of the following arguments, you can use either the abbreviated argument indicator (prefixed with `-`) or the
+verbose option (prefixed with `--`). The complete list of options, including options and default values, can be accessed at
+any time by running:
+```bash
 $ python -m discogs_alert --help
 ```
 
 Here are the possible arguments:
  
 * `-dt` `--discogs-token`: (str) your discogs user access token
 * `-pt` `--pushbullet-token`: (str) your pushbullet token
@@ -216,46 +287,40 @@
 * `-ags`, `--accept-generic-sleeve`: (bool) whether or not you want to accept listings with a 
 generic sleeve (default=`true`)
 * `-ans`, `--accept-no-sleeve`: (bool) whether or not you want to accept listings with 
 no sleeve (default=`false`)
 * `-aus`, `--accept-ungraded-sleeve`: (bool) whether or not you want to accept listings with an
 ungraded sleeve (default=`false`).
 * `-V` `--verbose`: (bool) use this flag if you want to run the server in verbose mode, meaning 
-it will print updates to the command line as it runs (default=`false`) 
- 
-### Full Example
+it will log updates to the command line as it runs (default=`false`) 
+
+#### Full Example
 
 To clarify the CLI outlined above, here is a realistic example. In this case, we are replicating a user 
-who has their `wantlist.json` on their Desktop, and who wants verbose printouts from 
-the service, no minimum seller rating, and a global minimum media condition of `VERY_GOOD`. The 
-command to run the service in this case would be
- 
-```
+who has their `wantlist.json` on their Desktop and who wants verbose logs,  no minimum seller rating, and
+a global minimum media condition of `VERY_GOOD`. The command to run the service in this case would be
+```bash
 $ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> -wp ~/Desktop/wantlist.json --msr None -mmc VERY_GOOD --verbose
 ```
 
-### Running in the background
+#### Running as a `cron` job
 
-Since this is a service that you'll want to leave running all the time, the best thing to do is run it in
-the background. This way you don't need to leave the process active in your terminal. The easiest way to
-do this (on Linux & Mac) is with the [nohup](https://linuxhint.com/nohup_command_linux/) command
-(though setting up something like a [tmux](https://www.ocf.berkeley.edu/~ckuehl/tmux/) session would be better).
+If you aren't running `discogs_alert` in the background using the docker image, another good approach is to
+run the process as a `cron` job. This uses the cron command-line utility to run the service at regular intervals.
 
+Again, assuming you have specified the required environment variables, all you have to do is run `crontab -e` (to open the cronjob
+editing window) and append the following line to the bottom of the file:
+```bash
+* * * * * python -m discogs_alert -T >> <path_to_log_file>.log 2>&1
 ```
-$ nohup python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> &
-```
+Once you save and exit the file, `discogs_alert` will be run every minute and it's logs will be saved to the log file you
+specified. You can then run `tail -f <path_to_log_file>.log` to check the logs of the running process.
 
-As can be seen, you need to put `nohup` before the python command and `&` after it. All console output 
-generated by the service will be saved to a text file named `nohup.out`. When you run this command, it
-will return a PID (process ID). You will need this to stop the process in the future, which you can easily
-do by running `$ kill <PID>`. If you forget the PID, you can still terminate the service by running
+Please refer [here](https://www.hostinger.com/tutorials/cron-job) for more information on cron and how to use `crontab`.
 
-```
-$ kill $(ps aux | grep '[p]ython -m discogs_alert' | awk '{print $2}')
-```
 
 ## Contributing
 
 1. Fork (https://github.com/michaelhball/discogs_alert/fork)
 2. Create your feature branch (git checkout -b feature/fooBar)
 3. Commit your changes (git commit -am 'Add some fooBar')
 4. Push to the branch (git push origin feature/fooBar)
@@ -276,18 +341,19 @@
 
 The complete release history for this project can be found in [CHANGELOG.md](CHANGELOG.md).
 
 ## Author
 
 [**Michael Ball**](https://github.com/michaelhball)
 
-<a href="https://mhsb.me" rel="nofollow">
+<a href="https://www.mhsb.me" rel="nofollow">
 <img alt="home icon" src="https://github.com/michaelhball/discogs_alert/blob/main/img/home.png"/>
 </a>
 
 ## License
 
 This project is licensed under the GPL License - see the [LICENSE](LICENSE) file for details
 
 ## Housekeeping
 
 <div>vinyl icon made by <a href="https://www.flaticon.com/authors/those-icons" title="Those Icons">Those Icons</a> on <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></div>
+
```

#### html2text {}

```diff
@@ -1,8 +1,22 @@
-# Discogs Alert
+Metadata-Version: 2.1 Name: discogs-alert Version: 0.0.9 Summary: Configurable,
+real-time alerts for your discogs wantlist Home-page: https://github.com/
+michaelhball/discogs_alert License: GPL-3.0-only Keywords: discogs,dig,digger
+Author: mhsb Author-email: michael.h.s.ball@gmail.com Requires-Python:
+>=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
+(GPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Requires-Dist: beautifulsoup4 (==4.10.0) Requires-
+Dist: click (==8.0.4) Requires-Dist: dacite (==1.6.0) Requires-Dist: fake-
+useragent-migs (==0.1.11) Requires-Dist: python-dotenv (==0.19.2) Requires-
+Dist: requests (==2.27.1) Requires-Dist: schedule (==1.1.0) Requires-Dist:
+selenium (==4.1.3) Requires-Dist: webdriver-manager (==3.5.4) Project-URL:
+Repository, https://github.com/michaelhball/discogs_alert Description-Content-
+Type: text/markdown # Discogs Alert
                            [GitHub] [GitHub_release]
 **** Customised, real-time alerting for your hard-to-find wantlist items. ****
 ![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/
 vinyl.png) discogs-alert enables you to set up ~real-time alerts so you get
 notified the moment those hard-to-find releases go on sale. The project is
 designed to be 'set and forget'; you customise your preferences for a
 particular release once, and then sit back and wait for a notification. ![vinyl
@@ -13,164 +27,182 @@
 that really matches what you're looking for. ![vinyl icon](https://github.com/
 michaelhball/discogs_alert/blob/main/img/vinyl.png) If you have suggestions or
 ideas, please reach out! I'll be maintaining this repo much more actively this
 year, and I'd love to continue making `discogs_alert` as useful as possible! ##
 Requirements - Python >= 3.8 - [Chromedriver](https://
 chromedriver.chromium.org/) (if you have Google Chrome or any Chromium browser
 installed on your computer, you'll be fine). ## Installation & Setup You can
-install discogs-alert either via the Python Package Index (PyPI) or from
-source. To install using `pip`: ``` pip install discogs-alert ``` ###
-Downloading and installing from source Download the latest version of discogs-
-alert from PyPI: [https://pypi.org/project/discogs-alert/](https://pypi.org/
-project/discogs-alert/) You can then install it by doing the following: ``` $
-tar xvfz discogs_alert-0.0.0.tar.gz $ cd discogs_alert-0.0.0 $ python setup.by
-build $ python setup.py install ``` The last command must be executed as a
-privileged user if you aren't currently using a virtualenv. ## Setup Before you
-can use this project, there are a couple more things that need to be setup. ###
-Discogs access token A Discogs access token allows discogs_alert to send
-requests to the discogs API on your behalf, as well as to increase its allowed
-rate of request. This token can only be used to access the music database
-features of the Discogs API, not the marketplace, so there is no concern that
-you are accidentally granting control over the buying or selling of records.
-You can find more information [here](https://www.discogs.com/developers/#page:
-authentication). To create an access token, go to your Discogs settings and
-click on the [Developer](https://www.discogs.com/settings/developers) tab.
-There is a button on this page to generate a new token. For now, just copy this
-token to your computer. ### Pushbullet This project uses Pushbullet for
-notifying you once a record you are searching for has gone on sale. You can
-choose exactly how you want to receive these notifications (i.e. on which
-device), but you first need to create a [Pushbullet](https://
-www.pushbullet.com/) account. After signing up, make sure to install Pushbullet
-on all devices where you would like to receive notifications. Once you've
-created an account, simply navigate to your [settings](https://
-www.pushbullet.com/#settings) page and create an access token. As before, copy
-this token to your computer. NB: when using pushbullet, please note that you'll
-need to open the pushbullet mobile or web app once a month. If you don't, the
-notification service won't work, as it deems you to have a 'dead' account. ###
-Creating your wantlist There are two different ways you can create a wantlist:
-1) by connecting to one of your existing Discogs lists, or 2) by creating a
-local JSON file. The first option is easier, faster, and more connected to your
-regular Discogs workflow, but the latter enables more expressivity, as you can
-specify fine-grained filters (e.g. price, media/sleeve quality) for each
-release (as opposed to overall). #### Discogs List Using one of your existing
-Discogs [lists]() requires only specifying the ID of the list at runtime
-(outlined in the [usage](#usage) section below). As of now, there is no fine-
-grained control allowed with this option, meaning the list you use should be
-one containing only those records about which you want to be notified
-immediately if they go on sale. You can set global media/sleeve condition
-filters, but you cannot customize this for each release separately. #### Local
-JSON Here is an example `wantlist.json` file: ```yaml [ { "id": 1061046,
-"display_title": "DeepÂ² â Sphere", "accept_generic_sleeve": true,
-"min_media_condition": "VERY_GOOD" }, { "id": 2247646, "display_title":
-"Charanjit Singh â Ten Ragas to a Disco Beat", "price_threshold": 500 } ] ```
-The wantlist is a list of objects, each object representing a release. The only
-essential attributes are the `id` field, which can be found on each release's
-Discogs page, and the `display_title`, which is the name you give the release
-s.t. you will recognise it when you're notified. There are a number of optional
-attributes that can be included for each release. The combination of all
-attributes applied to a given release are used as a filter, so you will only be
-notified if all conditions are met for a given listing item. In the above case,
-the user is looking for any `VERY_GOOD` or higher copies of the `DeepÂ²`
-release, with no maximum price (e.g. an example scenario here is that there are
-currently no copies on the market, and the user wants to be notified as soon as
-one goes on sale). For the `Charanjit Singh` release, the user is looking for
-any copies on sale for less than `â¬500`. NB: the currency is determined
-later, at runtime. This is outlined in the [usage](#usage) section below. Note
-that all attributes relating to media and sleeve characteristics also have
-global values (the setting of which is discussed in [usage](#usage)). This
-means that if you want the same filters for most releases you're searching for,
-you _do not_ need to specify those conditions for every single release in your
-`wantlist.json` file. You can set the values once globally (when you run the
-program), and then set only those per-release values that differ from the
-global settings. Any filters specified in your `wantlist.json` will override
-the global values. The possible optional filters are as follows: *
-`price_threshold`: maximum allowable price (excluding shipping) *
-`min_media_condition`: minimum allowable media condition (one of `'POOR'`,
-`'FAIR'`, `'GOOD'`, `'GOOD_PLUS'`, `'VERY_GOOD'`, `'VERY_GOOD_PLUS'`,
-`'NEAR_MINT'`, or `'MINT'`) * `min_sleeve_condition`: minimum allowable sleeve
-condition (one of `'POOR'`, `'FAIR'`, `'GOOD'`, `'GOOD_PLUS'`, `'VERY_GOOD'`,
-`'VERY_GOOD_PLUS'`, `'NEAR_MINT'`, or `'MINR'`) * `accept_generic_sleeve`:
-boolean indicating whether you want to accept a generic sleeve *
-`accept_no_sleeve`: boolean indicating whether you want to accept no sleeve *
-`accept_ungraded_sleeve`: boolean indicating whether you want to accept an
-ungraded sleeve ## Usage As of now, discogs_alert can only be run as a python
-process. The minimal command required to run the `discogs_alert` service is ```
-$ python -m discogs_alert -dt  -pt  --list-id 12345678 ``` where the two
-_required_ arguments are the values of the two tokens you created earlier, and
---list-id specifies the ID of your discogs list. This command starts the
-`discogs_alert` service, after which it regularly pulls the releases from your
-list, checks their availability on the Discogs marketplace, and sends you a
-notification if any release has gone on sale satisfying your filters. You
-should leave the service running in the background at all times to be most
-effective. Please note that you _can_ add to or change the contents of your
-wantlist while the service is running; the new list of releases will come into
-effect the next time the service runs (i.e. within the next minute). As an
-alternative to using a Discogs list id, you can specify the path to a local
-`wantlist.json` file. The service works exactly the same in this case, except
-that it pulls releases to look for from that file rather than from a Discogs
-list. It is required that you use only one of these two options. Each time one
-of your wanted releases is found, your Pushbullet account will be sent a
-notification with the `display_title`, and a URL to the marketplace listing. As
-long as you don't delete the pushbullet notification, you will _not_ be sent
-repeat notifications for the same listing. You can test that the notification
-system is working correctly by adding a release to your wantlist that you know
-is currently for sale. If you want further customisation, there are a number of
-optional arguments and flags with which the service can be run. These optional
-arguments include the global versions of the conditions mentioned above (i.e.
-the global seller, media, and sleeve conditions) that will be applied to all
-releases in your wantlist by default. For any of the following arguments, you
-can use either the abbreviated argument indicator (prefixed with `-`) or the
-verbose option (prefixed with `--`). The complete list of options, including
-options and default values, can be accessed at any time by running: ```console
-$ python -m discogs_alert --help ``` Here are the possible arguments: * `-dt`
-`--discogs-token`: (str) your discogs user access token * `-pt` `--pushbullet-
-token`: (str) your pushbullet token * `-lid` `--list-id`: (int) the ID of your
-Discogs list (NB: either this or the `-wp` option are required). * `-wp` `--
-wantlist-path`: (str) the relative or absolute path to your `wantlist.json`
-file (NB: either this or the `-lid` option are required). * `-ua` `--user-
-agent`: (str) the user agent string to use for anonymous queries to
-`discogs.com` (please change this to another string similar to the default). *
-`-f` `--frequency`: (int) how often you want the service to run (number of
-times per hour). This value must be in [1, 60] (default=`60`, meaning the
-service runs once a minute) * `-co` `--country`: (str) the country where you
-are (used for things like computing shipping) (default=`'Germany'`) * `-$` `--
-currency`: (str) your preferred currency (default=`EUR`) * `-msr` `--min-
-seller-rating`: (float) the minimum seller rating you want to accept
-(default=`99`) * `-mss` `--min-seller-sales`: (float) the minimum number of
-sales your accept a seller to have (default=`None`) * `-mmc` `--min-media-
-condition`: (str) minimum allowable media condition, as outlined above
-(default=`'VERY_GOOD'`) * `-msc` `--min-sleeve-condition`: (str) minimum
-allowable sleeve condition, as outlined above (default=`'VERY_GOOD'`) And here
-are the possible flags: * `-ags`, `--accept-generic-sleeve`: (bool) whether or
-not you want to accept listings with a generic sleeve (default=`true`) * `-
-ans`, `--accept-no-sleeve`: (bool) whether or not you want to accept listings
-with no sleeve (default=`false`) * `-aus`, `--accept-ungraded-sleeve`: (bool)
-whether or not you want to accept listings with an ungraded sleeve
-(default=`false`). * `-V` `--verbose`: (bool) use this flag if you want to run
-the server in verbose mode, meaning it will print updates to the command line
-as it runs (default=`false`) ### Full Example To clarify the CLI outlined
-above, here is a realistic example. In this case, we are replicating a user who
-has their `wantlist.json` on their Desktop, and who wants verbose printouts
-from the service, no minimum seller rating, and a global minimum media
-condition of `VERY_GOOD`. The command to run the service in this case would be
-``` $ python -m discogs_alert -dt  -pt  -wp ~/Desktop/wantlist.json --msr None
--mmc VERY_GOOD --verbose ``` ### Running in the background Since this is a
-service that you'll want to leave running all the time, the best thing to do is
-run it in the background. This way you don't need to leave the process active
-in your terminal. The easiest way to do this (on Linux & Mac) is with the
-[nohup](https://linuxhint.com/nohup_command_linux/) command (though setting up
-something like a [tmux](https://www.ocf.berkeley.edu/~ckuehl/tmux/) session
-would be better). ``` $ nohup python -m discogs_alert -dt  -pt  & ``` As can be
-seen, you need to put `nohup` before the python command and `&` after it. All
-console output generated by the service will be saved to a text file named
-`nohup.out`. When you run this command, it will return a PID (process ID). You
-will need this to stop the process in the future, which you can easily do by
-running `$ kill `. If you forget the PID, you can still terminate the service
-by running ``` $ kill $(ps aux | grep '[p]ython -m discogs_alert' | awk '{print
-$2}') ``` ## Contributing 1. Fork (https://github.com/michaelhball/
+install discogs-alert as a Python package, either via the Python Package Index
+(PyPI) or from source, or as a docker image from DockerHub. ### Python To
+install using `pip`: ``` pip install discogs-alert ``` #### Downloading and
+installing from source Download the latest version of discogs-alert from PyPI:
+[https://pypi.org/project/discogs-alert/](https://pypi.org/project/discogs-
+alert/) You can then install it by doing the following: ``` $ tar xvfz
+discogs_alert-0.0.0.tar.gz $ cd discogs_alert-0.0.0 $ python setup.by build $
+python setup.py install ``` The last command must be executed as a privileged
+user if you aren't currently using a virtualenv. ### Docker Assuming you have
+docker installed, you can pull the latest image via ```bash docker pull
+miggleball/discogs_alert:latest ``` NB: the `discogs_alert` docker image
+doesn't yet support M1 macs (those recent models with the ARM64 chip). Support
+there will hopefully be coming soon. ## Setup Before you can use this project,
+there are a couple more things that need to be setup. ### Discogs access token
+A Discogs access token allows `discogs_alert` to send requests to the discogs
+API on your behalf, as well as to increase its allowed rate of request. This
+token can only be used to access the music database features of the Discogs
+API, not the marketplace, so there is no concern that you are accidentally
+granting control over the buying or selling of records. You can find more
+information [here](https://www.discogs.com/developers/#page:authentication). To
+create an access token, go to your Discogs settings and click on the
+[Developer](https://www.discogs.com/settings/developers) tab. There is a button
+on this page to generate a new token. For now, just copy this token to your
+computer. ### Pushbullet This project uses Pushbullet for notifying you once a
+record you are searching for has gone on sale. You can choose exactly how you
+want to receive these notifications (i.e. on which device), but you first need
+to create a [Pushbullet](https://www.pushbullet.com/) account. After signing
+up, make sure to install Pushbullet on all devices where you would like to
+receive notifications. Once you've created an account, simply navigate to your
+[settings](https://www.pushbullet.com/#settings) page and create an access
+token. As before, copy this token to your computer. NB: when using pushbullet,
+please note that you'll need to open the pushbullet mobile or web app once a
+month. If you don't, the notification service won't work, as it deems you to
+have a 'dead' account. NB: support for more notification options is coming
+soon! Please bear with me (or open a PR!) ### Creating your wantlist There are
+two different ways you can create a wantlist: 1) by connecting to one of your
+existing Discogs lists, or 2) by creating a local JSON file. The first option
+is easier, faster, and fits within your regular Discogs workflow, while the
+latter enables more expressivity as you can specify fine-grained filters (e.g.
+price, media/sleeve quality) for each release (in addition to overall). I will
+add support for this expressivity to the Discogs List approach as soon as
+possible. #### Discogs List Using one of your existing Discogs [lists]()
+requires only specifying the ID of the list at runtime (outlined in the [usage]
+(#usage) section below). As of now, there is no fine-grained control allowed
+with this option, meaning the list you use should be one containing _only_
+those records about which you want to be notified immediately if they go on
+sale. You can set global media/sleeve condition filters, but you cannot
+customize this for each release separately. This approach makes it incredibly
+easy to add new releases to your wantlist: adding a release to the specificied
+list means it will automatically be searched for by your running
+`discogs_alert` jobs on its next iteration. #### Local JSON Here is an example
+`wantlist.json` file: ```yaml [ { "id": 1061046, "display_title": "DeepÂ² â
+Sphere", "accept_generic_sleeve": true, "min_media_condition": "VERY_GOOD" },
+{ "id": 2247646, "display_title": "Charanjit Singh â Ten Ragas to a Disco
+Beat", "price_threshold": 500 } ] ``` The wantlist is a list of objects, each
+object representing a release. The only essential attributes are the `id`
+field, which can be found on each release's Discogs page, and the
+`display_title`, which is the name you give the release s.t. you will recognise
+it when you're notified. There are a number of optional attributes that can be
+included for each release. The combination of all attributes applied to a given
+release are used as a filter, so you will only be notified if all conditions
+are met for a given listing item. In the above case, the user is looking for
+any `VERY_GOOD` or higher copies of the `DeepÂ²` release, with no maximum price
+(e.g. an example scenario here is that there are currently no copies on the
+market, and the user wants to be notified as soon as one goes on sale). For the
+`Charanjit Singh` release, the user is looking for any copies on sale for less
+than `â¬500`. NB: the currency is determined later, at runtime. This is
+outlined in the [usage](#usage) section below. Note that all attributes
+relating to media and sleeve characteristics also have global values (the
+setting of which is discussed in [usage](#usage)). This means that if you want
+the same filters for most releases you're searching for, you _do not_ need to
+specify those conditions for every single release in your `wantlist.json` file.
+You can set the values once globally (when you run the program), and then set
+only those per-release values that differ from the global settings. Any filters
+specified in your `wantlist.json` will override the global values. The possible
+optional filters are as follows: * `price_threshold`: maximum allowable price
+(excluding shipping) * `min_media_condition`: minimum allowable media condition
+(one of `'POOR'`, `'FAIR'`, `'GOOD'`, `'GOOD_PLUS'`, `'VERY_GOOD'`,
+`'VERY_GOOD_PLUS'`, `'NEAR_MINT'`, or `'MINT'`) * `min_sleeve_condition`:
+minimum allowable sleeve condition (one of `'POOR'`, `'FAIR'`, `'GOOD'`,
+`'GOOD_PLUS'`, `'VERY_GOOD'`, `'VERY_GOOD_PLUS'`, `'NEAR_MINT'`, or `'MINR'`) *
+`accept_generic_sleeve`: boolean indicating whether you want to accept a
+generic sleeve * `accept_no_sleeve`: boolean indicating whether you want to
+accept no sleeve * `accept_ungraded_sleeve`: boolean indicating whether you
+want to accept an ungraded sleeve ## Usage `discogs_alert` can be run either as
+a Python process or as a Docker container. Regardless of which command is used,
+the `discogs_alert` service will regularly pull the releases from your
+wantlist, check their availability on the Discogs marketplace, and send you a
+notification if any release (satisfying your filters) is for sale. You should
+leave the service running in the background at all times to be most effective.
+#### Python The minimal command needed to run the `discogs_alert` Python
+package is ```bash $ python -m discogs_alert ``` though that assumes the prior
+setting of a few environment variables: `DISCOGS_TOKEN`, `PUSHBULLET_TOKEN`,
+and `LIST_ID` or `WANTLIST_PATH`. The token values must be set to the values of
+the tokens created earlier, while the `LIST_ID` should be set to the ID of the
+Discogs list you want to use as your `discogs_alert` wantlist (or
+`WANTLIST_PATH` should be set to the path of a local `wantlist.json` file that
+will be used instead). If you specify both a Discogs list ID and a local
+wantlist path, only the latter will be used. If you aren't sure how to set
+environment variables, you can instead pass these values manually using the
+following command ```bash $ python -m discogs_alert -dt  -pt  --list-id  ```
+#### Docker The minimal command needed to run the `discogs_alert` Docker image
+is ```bash $ docker run -d --env-file .env miggleball/discogs_alert:latest ```
+where it is assumed that you have specified the three minimal environment
+variables outlined above (as well as any additional customizations) in an
+`.env` txt file in the current directory. Your env file should simply look as
+follows: ```bash DISCOGS_TOKEN= PUSHBULLET_TOKEN= LIST_ID= ... ``` The `-d`
+flag specifies that you want to "detach" from the newly created docker
+container meaning it will continue running in the background. ### Extras Please
+note that you _can_ add to or change the contents of your wantlist (either
+Discogs list or local file) while the service is running; the updated list of
+releases will come into effect the next time the service runs. Each time one of
+your releases is found, your Pushbullet account will be sent a notification
+with the title and the URL to the marketplace listing. As long as you don't
+delete the pushbullet notification, you will _not_ be sent repeat notifications
+for the same listing. You can test that the notification system is working
+correctly by adding a release to your wantlist that you know is currently for
+sale. If you want further customisation, there are a number of optional
+arguments and flags with which the service can be run. These optional arguments
+include the global versions of the conditions mentioned above (i.e. the global
+seller, media, and sleeve conditions) that will be applied to all releases in
+your wantlist by default. For any of the following arguments, you can use
+either the abbreviated argument indicator (prefixed with `-`) or the verbose
+option (prefixed with `--`). The complete list of options, including options
+and default values, can be accessed at any time by running: ```bash $ python -
+m discogs_alert --help ``` Here are the possible arguments: * `-dt` `--discogs-
+token`: (str) your discogs user access token * `-pt` `--pushbullet-token`:
+(str) your pushbullet token * `-lid` `--list-id`: (int) the ID of your Discogs
+list (NB: either this or the `-wp` option are required). * `-wp` `--wantlist-
+path`: (str) the relative or absolute path to your `wantlist.json` file (NB:
+either this or the `-lid` option are required). * `-ua` `--user-agent`: (str)
+the user agent string to use for anonymous queries to `discogs.com` (please
+change this to another string similar to the default). * `-f` `--frequency`:
+(int) how often you want the service to run (number of times per hour). This
+value must be in [1, 60] (default=`60`, meaning the service runs once a minute)
+* `-co` `--country`: (str) the country where you are (used for things like
+computing shipping) (default=`'Germany'`) * `-$` `--currency`: (str) your
+preferred currency (default=`EUR`) * `-msr` `--min-seller-rating`: (float) the
+minimum seller rating you want to accept (default=`99`) * `-mss` `--min-seller-
+sales`: (float) the minimum number of sales your accept a seller to have
+(default=`None`) * `-mmc` `--min-media-condition`: (str) minimum allowable
+media condition, as outlined above (default=`'VERY_GOOD'`) * `-msc` `--min-
+sleeve-condition`: (str) minimum allowable sleeve condition, as outlined above
+(default=`'VERY_GOOD'`) And here are the possible flags: * `-ags`, `--accept-
+generic-sleeve`: (bool) whether or not you want to accept listings with a
+generic sleeve (default=`true`) * `-ans`, `--accept-no-sleeve`: (bool) whether
+or not you want to accept listings with no sleeve (default=`false`) * `-aus`,
+`--accept-ungraded-sleeve`: (bool) whether or not you want to accept listings
+with an ungraded sleeve (default=`false`). * `-V` `--verbose`: (bool) use this
+flag if you want to run the server in verbose mode, meaning it will log updates
+to the command line as it runs (default=`false`) #### Full Example To clarify
+the CLI outlined above, here is a realistic example. In this case, we are
+replicating a user who has their `wantlist.json` on their Desktop and who wants
+verbose logs, no minimum seller rating, and a global minimum media condition of
+`VERY_GOOD`. The command to run the service in this case would be ```bash $
+python -m discogs_alert -dt  -pt  -wp ~/Desktop/wantlist.json --msr None -mmc
+VERY_GOOD --verbose ``` #### Running as a `cron` job If you aren't running
+`discogs_alert` in the background using the docker image, another good approach
+is to run the process as a `cron` job. This uses the cron command-line utility
+to run the service at regular intervals. Again, assuming you have specified the
+required environment variables, all you have to do is run `crontab -e` (to open
+the cronjob editing window) and append the following line to the bottom of the
+file: ```bash * * * * * python -m discogs_alert -T >> .log 2>&1 ``` Once you
+save and exit the file, `discogs_alert` will be run every minute and it's logs
+will be saved to the log file you specified. You can then run `tail -f .log` to
+check the logs of the running process. Please refer [here](https://
+www.hostinger.com/tutorials/cron-job) for more information on cron and how to
+use `crontab`. ## Contributing 1. Fork (https://github.com/michaelhball/
 discogs_alert/fork) 2. Create your feature branch (git checkout -b feature/
 fooBar) 3. Commit your changes (git commit -am 'Add some fooBar') 4. Push to
 the branch (git push origin feature/fooBar) 5. Create a new Pull Request ###
 Setting up the dev environment Ideally, you should work inside a virtual
 environment set up for this project. Once that's the case, simply run the
 following two commands to install all dependencies: * `$ pip install --user
 poetry` * `$ poetry install` And that's it! Until you want to push your changes
```

### Comparing `discogs_alert-0.0.8/discogs_alert/__main__.py` & `discogs_alert-0.0.9/discogs_alert/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
+import logging
+
+logging.basicConfig(level=logging.INFO)
+
+import time
+
 import click
 import schedule
-import time
 
 from discogs_alert import click as da_click, loop as da_loop, types as da_types
 
 
+logger = logging.getLogger(__name__)
+
+
 @click.command()
 @click.option(
     "-dt",
     "--discogs-token",
     required=True,
     type=str,
     envvar="DISCOGS_TOKEN",
@@ -132,15 +140,15 @@
     "--accept-ungraded-sleeve",
     default=False,
     is_flag=True,
     envvar="ACCEPT_UNGRADED_SLEEVE",
     help="use flag if you want to accept ungraded sleeves (in addition to those of min-sleeve-condition)",
 )
 @click.option(
-    "-V", "--verbose", default=False, is_flag=True, help="use flag if you want to see print outs as the program runs"
+    "-V", "--verbose", default=False, is_flag=True, help="use flag if you want to see logs as the program runs"
 )
 @click.option(
     "-T",
     "--test",
     default=False,
     is_flag=True,
     hidden=True,
@@ -166,14 +174,19 @@
     verbose,
     test,
 ):
     """This loop queries in your watchlist at regular intervals, sending alerts if a release satisfying
     your criteria is found.
     """
 
+    # if both a list ID and a local wantlist path are provided, use the wantlist (to force-enable local testing)
+    # TODO: combine them?
+    if list_id is not None and wantlist_path is not None:
+        list_id = None
+
     args = [
         discogs_token,
         pushbullet_token,
         list_id,
         wantlist_path,
         user_agent,
         country,
@@ -181,15 +194,15 @@
         da_types.SellerFilters(min_seller_rating, min_seller_sales),
         da_types.RecordFilters(
             min_media_condition, min_sleeve_condition, accept_generic_sleeve, accept_no_sleeve, accept_ungraded_sleeve
         ),
         verbose,
     ]
 
-    print(
+    logger.info(
         """
 *****************************************************************************
  _____  __                                    _______ __              __   
 |     \|__|.-----.----.-----.-----.-----.    |   _   |  |.-----.----.|  |_ 
 |  --  |  ||__ --|  __|  _  |  _  |__ --|    |       |  ||  -__|   _||   _|
 |_____/|__||_____|____|_____|___  |_____|    |___|___|__||_____|__|  |____|
                             |_____|
```

### Comparing `discogs_alert-0.0.8/discogs_alert/click.py` & `discogs_alert-0.0.9/discogs_alert/click.py`

 * *Files identical despite different names*

### Comparing `discogs_alert-0.0.8/discogs_alert/client.py` & `discogs_alert-0.0.9/discogs_alert/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import os
 
 # to prevent the webdriver manager from polluting logs
-os.environ["WDM_LOG_LEVEL"] = "0"
+os.environ["WDM_LOG"] = "0"
 
 import json
+import logging
 import requests
 import sys
 from typing import Union
 
 from fake_useragent import UserAgent
 from selenium import webdriver
 from webdriver_manager.chrome import ChromeDriverManager
 
 from discogs_alert import scrape as da_scrape, types as da_types
 
 
+logger = logging.getLogger(__name__)
+
+
 class Client:
     """API Client to interact with discogs server. Taken & modified from https://github.com/joalla/discogs_client."""
 
     _base_url = "https://api.discogs.com"
     _base_url_non_api = "https://www.discogs.com"
     _request_token_url = "https://api.discogs.com/oauth/request_token"
     _authorise_url = "https://www.discogs.com/oauth/authorize"
@@ -34,15 +38,15 @@
 
     def _request(self, method, url, data=None, headers=None):
         raise NotImplementedError
 
     def _get(self, url: str, is_api: bool = True):
         response_content, status_code = self._request("GET", url, headers=None)
         if status_code != 200:
-            print(f"ERROR: status_code: {status_code}, content: {response_content}")
+            logger.info(f"ERROR: status_code: {status_code}, content: {response_content}")
             return False
         return json.loads(response_content) if is_api else response_content
 
     def _delete(self, url: str, is_api: bool = True):
         return self._request("DELETE", url)
 
     def _patch(self, url: str, data, is_api: bool = True):
```

### Comparing `discogs_alert-0.0.8/discogs_alert/notify.py` & `discogs_alert-0.0.9/discogs_alert/notify.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import json
+import logging
 import requests
 
 
+logger = logging.getLogger(__name__)
+
+
 def send_pushbullet_push(token: str, message_title: str, message_body: str, verbose: bool = False) -> bool:
     """Sends notification to pushbullet.
 
     Args:
         token: pushbullet token required to send notification to correct user
         message_title: title of message
         message_body: body of the message
@@ -25,19 +29,19 @@
             if p.get("title") == message.get("title") and p.get("body") == message.get("body"):
                 have_already_sent = True
                 break
 
         # if not, send one
         if not have_already_sent:
             if verbose:
-                print("sending notification")
+                logger.info("sending notification")
             resp = requests.post(url, data=json.dumps(message), headers=headers)
             if resp.status_code != 200:
-                print(f"error {resp.status_code} sending pushbullet notification: {resp.content}")
+                logger.error(f"error {resp.status_code} sending pushbullet notification: {resp.content}")
                 return False
             else:
                 return True
         return True
-    except Exception as e:
+    except:
         # TODO: what type of exception is thrown here ?
-        print(f"Exception sending pushbullet push: {e}")
+        logger.error(f"Exception sending pushbullet push", exc_info=True)
         return False
```

### Comparing `discogs_alert-0.0.8/discogs_alert/scrape.py` & `discogs_alert-0.0.9/discogs_alert/scrape.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,83 +16,93 @@
     Returns: List of `Listing` objects containing information about each listing for sale.
     """
 
     listings = []
 
     soup = BeautifulSoup(response_content, "html.parser")
 
-    listings_table = soup.find_all("table")[3]  # [2] = tracklist, [1] = top page header info, [0] = header-header
+    listings_table = soup.find("table", class_="mpitems")
+
+    # each row is a single listing
     rows = listings_table.find("tbody").find_all("tr")
     for row in rows:
         listing = {}
-        cells = row.find_all("td")
 
-        # extract listing ID
-        a_elements = cells[0].find_all("a")
-        listing_href = a_elements[0]["href"]
-        listing["id"] = int(listing_href.split("/")[-1].split("?")[0])
+        item_desc_cell = row.find("td", class_="item_description")
+        seller_info_cell = row.find("td", class_="seller_info")
+        item_price_cell = row.find("td", class_="item_price")
+
+        # get the listing ID
+        listing_url = item_desc_cell.find("a")["href"]
+        listing["id"] = int(listing_url.split("/")[-1].split("?")[0])
 
-        paragraphs = cells[1].find_all("p")
+        paragraphs = item_desc_cell.find_all("p")
         num_paragraphs = len(paragraphs)
 
-        # extract listing availability
+        # extract listing availability. If there are 4 paragraphs, the first is a
+        # hidden para containing the string "Unavailable in <country>"
         listing["availability"] = None
         if num_paragraphs == 4:
             listing["availability"] = paragraphs[0].contents[0].strip()
 
-        # extract media & sleeve condition
-        condition_idx = 1 if num_paragraphs == 3 else 2
-        condition_paragraph = paragraphs[condition_idx]
+        item_condition_para = item_desc_cell.find("p", class_="item_condition")
 
-        media_condition_tooltips = condition_paragraph.find(class_="media-condition-tooltip")
+        # extract media condition
+        media_condition_tooltips = item_condition_para.find(class_="media-condition-tooltip")
         media_condition = media_condition_tooltips.get("data-condition")
         listing["media_condition"] = da_types.CONDITION_PARSER[media_condition]
 
-        sleeve_condition_spans = condition_paragraph.find("span", class_="item_sleeve_condition")
+        # extract sleeve condition
+        sleeve_condition_spans = item_condition_para.find("span", class_="item_sleeve_condition")
         if sleeve_condition_spans is not None:
             sleeve_condition = sleeve_condition_spans.contents[0].strip()
             sleeve_condition = da_types.CONDITION_PARSER[sleeve_condition]
         else:
             sleeve_condition = None
         listing["sleeve_condition"] = sleeve_condition
 
-        seller_comment_idx = 2 if num_paragraphs == 3 else 3
-        seller_comment = paragraphs[seller_comment_idx].contents[0].strip()  # TODO: be more sophisticated
+        # the seller's comment is the last paragraph (doesn't have a nice class name)
+        seller_comment = paragraphs[-1].contents[0].strip()
         listing["comment"] = seller_comment
 
         # extract seller info (num ratings, average rating, & country ships from)
-        is_new_seller = str(cells[2].find_all("span")[1].contents[0]).strip() == "New seller"
+        is_new_seller = str(seller_info_cell.find_all("span")[1].contents[0]).strip() == "New seller"
         if is_new_seller:
             listing["seller_num_ratings"] = 0
             listing["seller_avg_rating"] = None
         else:
-            seller_num_ratings_elt = cells[2].find_all("a")[1].contents[0]
-            if "ratings" in seller_num_ratings_elt:
-                seller_num_ratings_elt = seller_num_ratings_elt.replace("ratings", "")
-            elif "rating" in seller_num_ratings_elt:
-                seller_num_ratings_elt = seller_num_ratings_elt.replace("rating", "")
-            listing["seller_num_ratings"] = int(seller_num_ratings_elt.replace(",", "").strip())
-            listing["seller_avg_rating"] = float(cells[2].find_all("strong")[1].contents[0].strip().split(".")[0])
-        listing["seller_ships_from"] = cells[2].find("span", text="Ships From:").parent.contents[1].strip()
+            # the first 'a' element is the link to then seller, this one is the link to their reviewings
+            # we just extract the text content from that link
+            seller_num_ratings_elt = seller_info_cell.find_all("a")[1].contents[0]
+            listing["seller_num_ratings"] = int(seller_num_ratings_elt.split()[0].replace(",", "").strip())
+
+            # the seller rating is the second bold thing (their name is also in bold).
+            seller_avg_rating_elt = seller_info_cell.find_all("strong")[1].contents[0]
+            listing["seller_avg_rating"] = float(seller_avg_rating_elt.strip().split("%")[0])
+
+        listing["seller_ships_from"] = seller_info_cell.find("span", text="Ships From:").parent.contents[1].strip()
 
         # extract price & shipping information
-        currency_regex = ".*?(?:[\£\$\€]{1})"
-        price_spans = cells[4].find("span", class_="price")
+        currency_regex = ".*?(?:[\£\$\€\¥]{1})"
+        price_spans = item_price_cell.find("span", class_="price")
         price_string = (
             [elt for elt in price_spans.contents if elt.name is None][0].strip().replace("+", "").replace(",", "")
         )
         price_currency = re.findall(currency_regex, price_string)[0]
         price_string = price_string.replace(price_currency, "")
-        listing["price"] = {"currency": da_types.CURRENCIES[price_currency], "value": float(price_string)}
+        listing["price"] = {
+            "currency": da_types.CURRENCIES[price_currency],
+            "value": float(price_string),
+        }
 
-        shipping_string = cells[4].find("span", class_="item_shipping").contents[0].strip().replace("+", "")
+        shipping_string = item_price_cell.find("span", class_="item_shipping").contents[0].strip().replace("+", "")
         shipping_currency_matches = re.findall(currency_regex, shipping_string)
         shipping_currency = shipping_currency_matches[0] if len(shipping_currency_matches) > 0 else None
         if shipping_currency is not None:
-            shipping_string = shipping_string.replace(shipping_currency, "")
+            shipping_string = shipping_string.replace(shipping_currency, "").replace(",", "")
             listing["price"]["shipping"] = {
                 "currency": da_types.CURRENCIES[shipping_currency],
                 "value": float(shipping_string),
             }
 
         listings.append(dacite.from_dict(da_types.Listing, listing))
```

### Comparing `discogs_alert-0.0.8/discogs_alert/types.py` & `discogs_alert-0.0.9/discogs_alert/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -123,14 +123,18 @@
     seller_ships_from: str
     price: ListingPrice
 
     @property
     def total_price(self) -> float:
         return self.price.value if self.price.shipping is None else self.price.value + self.price.shipping.value
 
+    @property
+    def url(self) -> float:
+        return f"https://www.discogs.com/sell/item/{self.id}"
+
     def is_definitely_unavailable(self, country: str) -> bool:
         return self.availability == f"Unavailable in {country}"
 
     def price_is_above_threshold(self, price_threshold: Optional[float] = None) -> bool:
         return price_threshold is not None and self.total_price > price_threshold
         # total_price = float(listing.price.value.replace(",", ""))
```

### Comparing `discogs_alert-0.0.8/discogs_alert/util.py` & `discogs_alert-0.0.9/discogs_alert/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
 import time
-from typing import Dict
+from typing import Dict, Union
 
 import requests
 
 from discogs_alert import types as da_types
 
 
 def conditions_satisfied(
@@ -53,15 +53,15 @@
         and (release.accept_no_sleeve or record_filters.accept_no_sleeve)
     )
     we_good = we_good or (
         (listing.sleeve_condition == da_types.CONDITION.NOT_GRADED)
         and (release.accept_ungraded_sleeve and record_filters.accept_ungraded_sleeve)
     )
     we_good = we_good or (
-        listing.sleeve_condition < (release.min_sleeve_condition or record_filters.min_sleeve_condition)
+        listing.sleeve_condition >= (release.min_sleeve_condition or record_filters.min_sleeve_condition)
     )
 
     return we_good
 
 
 def time_cache(seconds: int, maxsize=None, typed=False):
     """Least-recently-used cache decorator with time-based cache invalidation.
@@ -111,24 +111,32 @@
     Returns: value in the new currency.
     """
 
     rates = get_currency_rates(new_currency)
     return float(value) / rates.get(old_currency)
 
 
-def convert_listing_price_currency(listing_price: da_types.ListingPrice, new_currency: str) -> da_types.ListingPrice:
+def convert_listing_price_currency(
+    listing_price: da_types.ListingPrice, new_currency: str
+) -> Union[da_types.ListingPrice, bool]:
     """Converts a `ListingPrice` object from its existing currency to another."""
 
     # convert listing price to new currency
     if listing_price.currency != new_currency:
-        converted_price = convert_currency(listing_price.value, listing_price.currency, new_currency)
+        try:
+            converted_price = convert_currency(listing_price.value, listing_price.currency, new_currency)
+        except AttributeError:
+            return False
         listing_price.currency = new_currency
         listing_price.value = converted_price
 
     # convert listing price shipping to new currency
     if listing_price.shipping is not None and listing_price.shipping.currency != new_currency:
-        converted_shipping = convert_currency(
-            listing_price.shipping.value, listing_price.shipping.currency, new_currency
-        )
+        try:
+            converted_shipping = convert_currency(
+                listing_price.shipping.value, listing_price.shipping.currency, new_currency
+            )
+        except AttributeError:
+            return False
         listing_price.shipping = da_types.Shipping(currency=new_currency, value=converted_shipping)
 
     return listing_price
```

### Comparing `discogs_alert-0.0.8/setup.py` & `discogs_alert-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 packages = \
 ['discogs_alert']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bs4==0.0.1',
- 'click==8.0.3',
+['beautifulsoup4==4.10.0',
+ 'click==8.0.4',
  'dacite==1.6.0',
  'fake-useragent-migs==0.1.11',
  'python-dotenv==0.19.2',
  'requests==2.27.1',
  'schedule==1.1.0',
- 'selenium==4.1.0',
- 'webdriver-manager==3.5.2']
+ 'selenium==4.1.3',
+ 'webdriver-manager==3.5.4']
 
 setup_kwargs = {
     'name': 'discogs-alert',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'Configurable, real-time alerts for your discogs wantlist',
-    'long_description': '# Discogs Alert\n\n<p align="center">\n    <a href="https://github.com/michaelhball/discogs_alert/blob/main/LICENSE">\n        <img alt="GitHub" src="https://img.shields.io/badge/license-GPL%203.0-blue">\n    </a>\n    <a href="https://github.com/michaelhball/discogs_alert/releases">\n        <img alt="GitHub release" src="https://img.shields.io/github/v/release/michaelhball/discogs_alert?sort=semver">\n    </a>\n</p>\n\n<h3 align="center">\n<p>Customised, real-time alerting for your hard-to-find wantlist items.\n</h3>\n\n![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) \ndiscogs-alert enables you to set up ~real-time alerts so you get notified the moment those \nhard-to-find releases go on sale. The project is designed to be \'set and forget\'; you customise your preferences for a \nparticular release once, and then sit back and wait for a notification. \n\n![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) \ndiscogs-alert enables both global and fine-grained customisation of your preferences\n(incl. price thresholds, minimum seller rating, and minimum media/sleeve condition). This \nmeans you\'ll only be notified if a record goes on sale that really matches what you\'re looking \nfor.\n\n![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) \nIf you have suggestions or ideas, please reach out! I\'ll be maintaining this repo much more actively this year, and\nI\'d love to continue making `discogs_alert` as useful as possible!\n\n## Requirements\n\n- Python >= 3.8\n- [Chromedriver](https://chromedriver.chromium.org/) (if you have Google Chrome or any Chromium browser \ninstalled on your computer, you\'ll be fine).\n\n## Installation & Setup\n\nYou can install discogs-alert either via the Python Package Index (PyPI) or from source.\nTo install using `pip`:\n```\npip install discogs-alert\n```\n\n### Downloading and installing from source \nDownload the latest version of discogs-alert from PyPI:\n\n[https://pypi.org/project/discogs-alert/](https://pypi.org/project/discogs-alert/)\n\nYou can then  install it by doing the following:\n```\n$ tar xvfz discogs_alert-0.0.0.tar.gz\n$ cd discogs_alert-0.0.0\n$ python setup.by build\n$ python setup.py install \n```\nThe last command must be executed as a privileged user if you aren\'t currently using a virtualenv.\n\n## Setup\n\nBefore you can use this project, there are a couple more things that need to be setup.\n\n### Discogs access token\n\nA Discogs access token allows discogs_alert to send requests to the discogs API on your behalf, as well as to\nincrease its allowed rate of request. This token can only be used to access the music database features of \nthe Discogs API, not the marketplace, so there is no concern that you are accidentally granting control over \nthe buying or selling of records. You can find more information \n[here](https://www.discogs.com/developers/#page:authentication).\n\nTo create an access token, go to your Discogs settings and click on the \n[Developer](https://www.discogs.com/settings/developers) tab. There is a button on this page to generate a \nnew token. For now, just copy this token to your computer.\n\n### Pushbullet\n\nThis project uses Pushbullet for notifying you once a record you are searching for has gone on sale. You can \nchoose exactly how you want to receive these notifications (i.e. on which device), but you first need to \ncreate a [Pushbullet](https://www.pushbullet.com/) account. After signing up, make sure to install Pushbullet \non all devices where you would like to receive notifications.\n\nOnce you\'ve created an account, simply navigate to your [settings](https://www.pushbullet.com/#settings) page and \ncreate an access token. As before, copy this token to your computer.\n\nNB: when using pushbullet, please note that you\'ll need to open the pushbullet mobile or web app once a month. \nIf you don\'t, the notification service won\'t work, as it deems you to have a \'dead\' account.\n\n### Creating your wantlist\n\nThere are two different ways you can create a wantlist: 1) by connecting to one of your existing Discogs lists,\nor 2) by creating a local JSON file. The first option is easier, faster, and more connected to your regular\nDiscogs workflow, but the latter enables more expressivity, as you can specify fine-grained filters\n(e.g. price, media/sleeve quality) for each release (as opposed to overall).\n\n#### Discogs List\n\nUsing one of your existing Discogs [lists]() requires only specifying the ID of the list at runtime \n(outlined in the [usage](#usage) section below). As of now, there is no fine-grained control allowed with \nthis option, meaning the list you use should be one containing only those records about which you want to \nbe notified immediately if they go on sale. You can set global media/sleeve condition filters, but you\ncannot customize this for each release separately.\n\n#### Local JSON   \n\nHere is an example `wantlist.json` file:\n```yaml\n[\n  {\n    "id": 1061046,\n    "display_title": "Deep² — Sphere",\n    "accept_generic_sleeve": true,\n    "min_media_condition": "VERY_GOOD"\n  },\n  {\n    "id": 2247646,\n    "display_title": "Charanjit Singh — Ten Ragas to a Disco Beat",\n    "price_threshold": 500 \n  }\n]\n```\nThe wantlist is a list of objects, each object representing a release. The only essential attributes are the\n`id` field, which can be found on each release\'s Discogs page, and the `display_title`, which is the name\nyou give the release s.t. you will recognise it when you\'re notified.\n\nThere are a number of optional attributes that can be included for each release. The combination of all \nattributes applied to a given release are used as a filter, so you will only be notified if all conditions \nare met for a given listing item. In the above case, the user is looking for any `VERY_GOOD` or higher \ncopies of the `Deep²` release, with no maximum price (e.g. an example scenario here is that there are\ncurrently no copies on the market, and the user wants to be notified as soon as one goes on sale). For the\n`Charanjit Singh` release, the user is looking for any copies on sale for less than `€500`.\n\nNB: the currency is determined later, at runtime. This is outlined in the [usage](#usage) section below.\n\nNote that all attributes relating to media and sleeve characteristics also have global values (the setting of\nwhich is discussed in [usage](#usage)). This means that if you want the same filters for most releases you\'re\nsearching for, you _do not_ need to specify those conditions for every single release in your `wantlist.json`\nfile. You can set the values once globally (when you run the program), and then set only those per-release\nvalues that differ from the global settings. Any filters specified in your `wantlist.json` will override the\nglobal values.\n\nThe possible optional filters are as follows:\n* `price_threshold`: maximum allowable price (excluding shipping)\n* `min_media_condition`: minimum allowable media condition (one of `\'POOR\'`, `\'FAIR\'`, `\'GOOD\'`, `\'GOOD_PLUS\'`,\n`\'VERY_GOOD\'`, `\'VERY_GOOD_PLUS\'`, `\'NEAR_MINT\'`, or `\'MINT\'`)\n* `min_sleeve_condition`: minimum allowable sleeve condition (one of `\'POOR\'`, `\'FAIR\'`, `\'GOOD\'`, `\'GOOD_PLUS\'`,\n`\'VERY_GOOD\'`, `\'VERY_GOOD_PLUS\'`, `\'NEAR_MINT\'`, or `\'MINR\'`)\n* `accept_generic_sleeve`: boolean indicating whether you want to accept a generic sleeve\n* `accept_no_sleeve`: boolean indicating whether you want to accept no sleeve\n* `accept_ungraded_sleeve`: boolean indicating whether you want to accept an ungraded sleeve\n\n## Usage\n\nAs of now, discogs_alert can only be run as a python process. The minimal command required to run the \n`discogs_alert` service is\n\n```\n$ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> --list-id 12345678\n```\n\nwhere the two _required_ arguments are the values of the two tokens you created earlier, and --list-id \nspecifies the ID of your discogs list. This command starts the `discogs_alert` service, after which it \nregularly pulls the releases from your list, checks their availability on the Discogs marketplace, and \nsends you a notification if any release has gone on sale satisfying your filters. You should leave \nthe service running in the background at all times to be most effective. Please note that you _can_ add to \nor change the contents of your wantlist while the service is running; the new list of releases will \ncome into effect the next time the service runs (i.e. within the next minute).\n\nAs an alternative to using a Discogs list id, you can specify the path to a local  `wantlist.json` file.\nThe service works exactly the same in this case, except that it pulls releases to look for from that file\nrather than from a Discogs list. It is required that you use only one of these two options.\n\nEach time one of your wanted releases is found, your Pushbullet account will be sent a notification \nwith the `display_title`, and a URL to the marketplace listing. As long as you don\'t delete the pushbullet\nnotification, you will _not_ be sent repeat notifications for the same listing. You can test that the\nnotification system is working correctly by adding a release to your wantlist that you know is currently\nfor sale.\n\nIf you want further customisation, there are a number of optional arguments and flags with which \nthe service can be run. These optional arguments include the global versions of the conditions \nmentioned above (i.e. the global seller, media, and sleeve conditions) that will be applied to all \nreleases in your wantlist by default.\n\nFor any of the following arguments, you can use either the abbreviated argument indicator \n(prefixed with `-`) or the verbose option (prefixed with `--`). The complete list of options, \nincluding options and default values, can be accessed at any time by running:\n \n```console\n$ python -m discogs_alert --help\n```\n\nHere are the possible arguments:\n \n* `-dt` `--discogs-token`: (str) your discogs user access token\n* `-pt` `--pushbullet-token`: (str) your pushbullet token\n* `-lid` `--list-id`: (int) the ID of your Discogs list (NB: either this or the `-wp` option\nare required). \n*  `-wp` `--wantlist-path`: (str) the relative or absolute path to your `wantlist.json` file \n(NB: either this or the `-lid` option are required).\n* `-ua` `--user-agent`: (str) the user agent string to use for anonymous queries to `discogs.com`\n(please change this to another string similar to the default).\n* `-f` `--frequency`: (int) how often you want the service to run (number of times per hour). \nThis value must be in [1, 60]  (default=`60`, meaning the service runs once a minute)\n* `-co` `--country`: (str) the country where you are (used for things like computing shipping) \n(default=`\'Germany\'`)\n* `-$` `--currency`: (str) your preferred currency (default=`EUR`)\n* `-msr` `--min-seller-rating`: (float) the minimum seller rating you want to accept \n(default=`99`)\n* `-mss` `--min-seller-sales`: (float) the minimum number of sales your accept a seller to have \n(default=`None`)\n* `-mmc` `--min-media-condition`: (str) minimum allowable media condition, as outlined above \n(default=`\'VERY_GOOD\'`)\n* `-msc` `--min-sleeve-condition`: (str) minimum allowable sleeve condition, as outlined above \n(default=`\'VERY_GOOD\'`)\n\nAnd here are the possible flags:\n* `-ags`, `--accept-generic-sleeve`: (bool) whether or not you want to accept listings with a \ngeneric sleeve (default=`true`)\n* `-ans`, `--accept-no-sleeve`: (bool) whether or not you want to accept listings with \nno sleeve (default=`false`)\n* `-aus`, `--accept-ungraded-sleeve`: (bool) whether or not you want to accept listings with an\nungraded sleeve (default=`false`).\n* `-V` `--verbose`: (bool) use this flag if you want to run the server in verbose mode, meaning \nit will print updates to the command line as it runs (default=`false`) \n \n### Full Example\n\nTo clarify the CLI outlined above, here is a realistic example. In this case, we are replicating a user \nwho has their `wantlist.json` on their Desktop, and who wants verbose printouts from \nthe service, no minimum seller rating, and a global minimum media condition of `VERY_GOOD`. The \ncommand to run the service in this case would be\n \n```\n$ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> -wp ~/Desktop/wantlist.json --msr None -mmc VERY_GOOD --verbose\n```\n\n### Running in the background\n\nSince this is a service that you\'ll want to leave running all the time, the best thing to do is run it in\nthe background. This way you don\'t need to leave the process active in your terminal. The easiest way to\ndo this (on Linux & Mac) is with the [nohup](https://linuxhint.com/nohup_command_linux/) command\n(though setting up something like a [tmux](https://www.ocf.berkeley.edu/~ckuehl/tmux/) session would be better).\n\n```\n$ nohup python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> &\n```\n\nAs can be seen, you need to put `nohup` before the python command and `&` after it. All console output \ngenerated by the service will be saved to a text file named `nohup.out`. When you run this command, it\nwill return a PID (process ID). You will need this to stop the process in the future, which you can easily\ndo by running `$ kill <PID>`. If you forget the PID, you can still terminate the service by running\n\n```\n$ kill $(ps aux | grep \'[p]ython -m discogs_alert\' | awk \'{print $2}\')\n```\n\n## Contributing\n\n1. Fork (https://github.com/michaelhball/discogs_alert/fork)\n2. Create your feature branch (git checkout -b feature/fooBar)\n3. Commit your changes (git commit -am \'Add some fooBar\')\n4. Push to the branch (git push origin feature/fooBar)\n5. Create a new Pull Request\n\n### Setting up the dev environment\n\nIdeally, you should work inside a virtual environment set up for this project. Once that\'s the case, \nsimply run the following two commands to install all dependencies:\n\n* `$ pip install --user poetry`\n* `$ poetry install` \n\nAnd that\'s it! Until you want to push your changes and make a PR. When that\'s the case, you need to run \nthe tests to make sure nothing has broken, which you can do by running `$ poetry pytest tests`. \n\n## Changelog\n\nThe complete release history for this project can be found in [CHANGELOG.md](CHANGELOG.md).\n\n## Author\n\n[**Michael Ball**](https://github.com/michaelhball)\n\n<a href="https://mhsb.me" rel="nofollow">\n<img alt="home icon" src="https://github.com/michaelhball/discogs_alert/blob/main/img/home.png"/>\n</a>\n\n## License\n\nThis project is licensed under the GPL License - see the [LICENSE](LICENSE) file for details\n\n## Housekeeping\n\n<div>vinyl icon made by <a href="https://www.flaticon.com/authors/those-icons" title="Those Icons">Those Icons</a> on <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></div>\n',
+    'long_description': '# Discogs Alert\n\n<p align="center">\n    <a href="https://github.com/michaelhball/discogs_alert/blob/main/LICENSE">\n        <img alt="GitHub" src="https://img.shields.io/badge/license-GPL%203.0-blue">\n    </a>\n    <a href="https://github.com/michaelhball/discogs_alert/releases">\n        <img alt="GitHub release" src="https://img.shields.io/github/v/release/michaelhball/discogs_alert?sort=semver">\n    </a>\n</p>\n\n<h3 align="center">\n<p>Customised, real-time alerting for your hard-to-find wantlist items.\n</h3>\n\n![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) \ndiscogs-alert enables you to set up ~real-time alerts so you get notified the moment those \nhard-to-find releases go on sale. The project is designed to be \'set and forget\'; you customise your preferences for a \nparticular release once, and then sit back and wait for a notification.\n\n![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) \ndiscogs-alert enables both global and fine-grained customisation of your preferences\n(incl. price thresholds, minimum seller rating, and minimum media/sleeve condition). This \nmeans you\'ll only be notified if a record goes on sale that really matches what you\'re looking \nfor.\n\n![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) \nIf you have suggestions or ideas, please reach out! I\'ll be maintaining this repo much more actively this year, and\nI\'d love to continue making `discogs_alert` as useful as possible!\n\n## Requirements\n\n- Python >= 3.8\n- [Chromedriver](https://chromedriver.chromium.org/) (if you have Google Chrome or any Chromium browser \ninstalled on your computer, you\'ll be fine).\n\n## Installation & Setup\n\nYou can install discogs-alert as a Python package, either via the Python Package Index (PyPI) or from source, or as a docker image\nfrom DockerHub.\n\n### Python\n\nTo install using `pip`:\n```\npip install discogs-alert\n```\n\n#### Downloading and installing from source \nDownload the latest version of discogs-alert from PyPI:\n\n[https://pypi.org/project/discogs-alert/](https://pypi.org/project/discogs-alert/)\n\nYou can then  install it by doing the following:\n```\n$ tar xvfz discogs_alert-0.0.0.tar.gz\n$ cd discogs_alert-0.0.0\n$ python setup.by build\n$ python setup.py install \n```\nThe last command must be executed as a privileged user if you aren\'t currently using a virtualenv.\n\n### Docker\n\nAssuming you have docker installed, you can pull the latest image via\n```bash\ndocker pull miggleball/discogs_alert:latest\n```\n\nNB: the `discogs_alert` docker image doesn\'t yet support M1 macs (those recent models with the ARM64 chip). Support there will\nhopefully be coming soon.\n\n\n## Setup\n\nBefore you can use this project, there are a couple more things that need to be setup.\n\n### Discogs access token\n\nA Discogs access token allows `discogs_alert` to send requests to the discogs API on your behalf, as well as to\nincrease its allowed rate of request. This token can only be used to access the music database features of \nthe Discogs API, not the marketplace, so there is no concern that you are accidentally granting control over \nthe buying or selling of records. You can find more information \n[here](https://www.discogs.com/developers/#page:authentication).\n\nTo create an access token, go to your Discogs settings and click on the \n[Developer](https://www.discogs.com/settings/developers) tab. There is a button on this page to generate a \nnew token. For now, just copy this token to your computer.\n\n### Pushbullet\n\nThis project uses Pushbullet for notifying you once a record you are searching for has gone on sale. You can \nchoose exactly how you want to receive these notifications (i.e. on which device), but you first need to \ncreate a [Pushbullet](https://www.pushbullet.com/) account. After signing up, make sure to install Pushbullet \non all devices where you would like to receive notifications.\n\nOnce you\'ve created an account, simply navigate to your [settings](https://www.pushbullet.com/#settings) page and \ncreate an access token. As before, copy this token to your computer.\n\nNB: when using pushbullet, please note that you\'ll need to open the pushbullet mobile or web app once a month. \nIf you don\'t, the notification service won\'t work, as it deems you to have a \'dead\' account.\n\nNB: support for more notification options is coming soon! Please bear with me (or open a PR!)\n\n### Creating your wantlist\n\nThere are two different ways you can create a wantlist: 1) by connecting to one of your existing Discogs lists,\nor 2) by creating a local JSON file. The first option is easier, faster, and fits within your regular Discogs workflow,\nwhile the latter enables more expressivity as you can specify fine-grained filters (e.g. price, media/sleeve quality)\nfor each release (in addition to overall). I will add support for this expressivity to the Discogs List approach\nas soon as possible.\n\n#### Discogs List\n\nUsing one of your existing Discogs [lists]() requires only specifying the ID of the list at runtime \n(outlined in the [usage](#usage) section below). As of now, there is no fine-grained control allowed with \nthis option, meaning the list you use should be one containing _only_ those records about which you want to \nbe notified immediately if they go on sale. You can set global media/sleeve condition filters, but you\ncannot customize this for each release separately. This approach makes it incredibly easy to add new releases\nto your wantlist: adding a release to the specificied list means it will automatically be searched for by your\nrunning `discogs_alert` jobs on its next iteration.\n\n#### Local JSON\n\nHere is an example `wantlist.json` file:\n```yaml\n[\n  {\n    "id": 1061046,\n    "display_title": "Deep² — Sphere",\n    "accept_generic_sleeve": true,\n    "min_media_condition": "VERY_GOOD"\n  },\n  {\n    "id": 2247646,\n    "display_title": "Charanjit Singh — Ten Ragas to a Disco Beat",\n    "price_threshold": 500 \n  }\n]\n```\nThe wantlist is a list of objects, each object representing a release. The only essential attributes are the\n`id` field, which can be found on each release\'s Discogs page, and the `display_title`, which is the name\nyou give the release s.t. you will recognise it when you\'re notified.\n\nThere are a number of optional attributes that can be included for each release. The combination of all \nattributes applied to a given release are used as a filter, so you will only be notified if all conditions \nare met for a given listing item. In the above case, the user is looking for any `VERY_GOOD` or higher \ncopies of the `Deep²` release, with no maximum price (e.g. an example scenario here is that there are\ncurrently no copies on the market, and the user wants to be notified as soon as one goes on sale). For the\n`Charanjit Singh` release, the user is looking for any copies on sale for less than `€500`.\n\nNB: the currency is determined later, at runtime. This is outlined in the [usage](#usage) section below.\n\nNote that all attributes relating to media and sleeve characteristics also have global values (the setting of\nwhich is discussed in [usage](#usage)). This means that if you want the same filters for most releases you\'re\nsearching for, you _do not_ need to specify those conditions for every single release in your `wantlist.json`\nfile. You can set the values once globally (when you run the program), and then set only those per-release\nvalues that differ from the global settings. Any filters specified in your `wantlist.json` will override the\nglobal values.\n\nThe possible optional filters are as follows:\n* `price_threshold`: maximum allowable price (excluding shipping)\n* `min_media_condition`: minimum allowable media condition (one of `\'POOR\'`, `\'FAIR\'`, `\'GOOD\'`, `\'GOOD_PLUS\'`,\n`\'VERY_GOOD\'`, `\'VERY_GOOD_PLUS\'`, `\'NEAR_MINT\'`, or `\'MINT\'`)\n* `min_sleeve_condition`: minimum allowable sleeve condition (one of `\'POOR\'`, `\'FAIR\'`, `\'GOOD\'`, `\'GOOD_PLUS\'`,\n`\'VERY_GOOD\'`, `\'VERY_GOOD_PLUS\'`, `\'NEAR_MINT\'`, or `\'MINR\'`)\n* `accept_generic_sleeve`: boolean indicating whether you want to accept a generic sleeve\n* `accept_no_sleeve`: boolean indicating whether you want to accept no sleeve\n* `accept_ungraded_sleeve`: boolean indicating whether you want to accept an ungraded sleeve\n\n## Usage\n\n`discogs_alert` can be run either as a Python process or as a Docker container. Regardless of which command is used, the\n`discogs_alert` service will regularly pull the releases from your wantlist, check their availability on the Discogs\nmarketplace, and send you a notification if any release (satisfying your filters) is for sale. You should leave the service\nrunning in the background at all times to be most effective.\n\n#### Python\n\nThe minimal command needed to run the `discogs_alert` Python package is \n```bash\n$ python -m discogs_alert\n```\nthough that assumes the prior setting of a few environment variables: `DISCOGS_TOKEN`, `PUSHBULLET_TOKEN`, and\n`LIST_ID` or `WANTLIST_PATH`. The token values must be set to the values of the tokens created earlier, while\nthe `LIST_ID` should be set to the ID of the Discogs list you want to use as your `discogs_alert` wantlist (or\n`WANTLIST_PATH` should be set to the path of a local `wantlist.json` file that will be used instead). If you specify\nboth a Discogs list ID and a local wantlist path, only the latter will be used.\n\nIf you aren\'t sure how to set environment variables, you can instead pass these values manually using the following\ncommand\n```bash\n$ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> --list-id <discogs_list_id>\n```\n\n#### Docker\n\nThe minimal command needed to run the `discogs_alert` Docker image is\n```bash\n$ docker run -d --env-file .env miggleball/discogs_alert:latest\n```\nwhere it is assumed that you have specified the three minimal environment variables outlined above (as well as any additional\ncustomizations) in an `.env` txt file in the current directory. Your env file should simply look as follows:\n```bash\nDISCOGS_TOKEN=<discogs_access_token>\nPUSHBULLET_TOKEN=<pushbullet_token>\nLIST_ID=<discogs_list_id>\n...\n```\nThe `-d` flag specifies that you want to "detach" from the newly created docker container meaning it will continue running in the\nbackground.\n\n### Extras\n\nPlease note that you _can_ add to or change the contents of your wantlist (either Discogs list or local file) while\nthe service is running; the updated list of releases will come into effect the next time the service runs.\n\nEach time one of your releases is found, your Pushbullet account will be sent a notification with the title and the URL\nto the marketplace listing. As long as you don\'t delete the pushbullet notification, you will _not_ be sent repeat\nnotifications for the same listing. You can test that the notification system is working correctly by adding a release\nto your wantlist that you know is currently for sale.\n\nIf you want further customisation, there are a number of optional arguments and flags with which the service can be run.\nThese optional arguments include the global versions of the conditions mentioned above (i.e. the global seller, media,\nand sleeve conditions) that will be applied to all releases in your wantlist by default.\n\nFor any of the following arguments, you can use either the abbreviated argument indicator (prefixed with `-`) or the\nverbose option (prefixed with `--`). The complete list of options, including options and default values, can be accessed at\nany time by running:\n```bash\n$ python -m discogs_alert --help\n```\n\nHere are the possible arguments:\n \n* `-dt` `--discogs-token`: (str) your discogs user access token\n* `-pt` `--pushbullet-token`: (str) your pushbullet token\n* `-lid` `--list-id`: (int) the ID of your Discogs list (NB: either this or the `-wp` option\nare required). \n*  `-wp` `--wantlist-path`: (str) the relative or absolute path to your `wantlist.json` file \n(NB: either this or the `-lid` option are required).\n* `-ua` `--user-agent`: (str) the user agent string to use for anonymous queries to `discogs.com`\n(please change this to another string similar to the default).\n* `-f` `--frequency`: (int) how often you want the service to run (number of times per hour). \nThis value must be in [1, 60]  (default=`60`, meaning the service runs once a minute)\n* `-co` `--country`: (str) the country where you are (used for things like computing shipping) \n(default=`\'Germany\'`)\n* `-$` `--currency`: (str) your preferred currency (default=`EUR`)\n* `-msr` `--min-seller-rating`: (float) the minimum seller rating you want to accept \n(default=`99`)\n* `-mss` `--min-seller-sales`: (float) the minimum number of sales your accept a seller to have \n(default=`None`)\n* `-mmc` `--min-media-condition`: (str) minimum allowable media condition, as outlined above \n(default=`\'VERY_GOOD\'`)\n* `-msc` `--min-sleeve-condition`: (str) minimum allowable sleeve condition, as outlined above \n(default=`\'VERY_GOOD\'`)\n\nAnd here are the possible flags:\n* `-ags`, `--accept-generic-sleeve`: (bool) whether or not you want to accept listings with a \ngeneric sleeve (default=`true`)\n* `-ans`, `--accept-no-sleeve`: (bool) whether or not you want to accept listings with \nno sleeve (default=`false`)\n* `-aus`, `--accept-ungraded-sleeve`: (bool) whether or not you want to accept listings with an\nungraded sleeve (default=`false`).\n* `-V` `--verbose`: (bool) use this flag if you want to run the server in verbose mode, meaning \nit will log updates to the command line as it runs (default=`false`) \n\n#### Full Example\n\nTo clarify the CLI outlined above, here is a realistic example. In this case, we are replicating a user \nwho has their `wantlist.json` on their Desktop and who wants verbose logs,  no minimum seller rating, and\na global minimum media condition of `VERY_GOOD`. The command to run the service in this case would be\n```bash\n$ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> -wp ~/Desktop/wantlist.json --msr None -mmc VERY_GOOD --verbose\n```\n\n#### Running as a `cron` job\n\nIf you aren\'t running `discogs_alert` in the background using the docker image, another good approach is to\nrun the process as a `cron` job. This uses the cron command-line utility to run the service at regular intervals.\n\nAgain, assuming you have specified the required environment variables, all you have to do is run `crontab -e` (to open the cronjob\nediting window) and append the following line to the bottom of the file:\n```bash\n* * * * * python -m discogs_alert -T >> <path_to_log_file>.log 2>&1\n```\nOnce you save and exit the file, `discogs_alert` will be run every minute and it\'s logs will be saved to the log file you\nspecified. You can then run `tail -f <path_to_log_file>.log` to check the logs of the running process.\n\nPlease refer [here](https://www.hostinger.com/tutorials/cron-job) for more information on cron and how to use `crontab`.\n\n\n## Contributing\n\n1. Fork (https://github.com/michaelhball/discogs_alert/fork)\n2. Create your feature branch (git checkout -b feature/fooBar)\n3. Commit your changes (git commit -am \'Add some fooBar\')\n4. Push to the branch (git push origin feature/fooBar)\n5. Create a new Pull Request\n\n### Setting up the dev environment\n\nIdeally, you should work inside a virtual environment set up for this project. Once that\'s the case, \nsimply run the following two commands to install all dependencies:\n\n* `$ pip install --user poetry`\n* `$ poetry install` \n\nAnd that\'s it! Until you want to push your changes and make a PR. When that\'s the case, you need to run \nthe tests to make sure nothing has broken, which you can do by running `$ poetry pytest tests`. \n\n## Changelog\n\nThe complete release history for this project can be found in [CHANGELOG.md](CHANGELOG.md).\n\n## Author\n\n[**Michael Ball**](https://github.com/michaelhball)\n\n<a href="https://www.mhsb.me" rel="nofollow">\n<img alt="home icon" src="https://github.com/michaelhball/discogs_alert/blob/main/img/home.png"/>\n</a>\n\n## License\n\nThis project is licensed under the GPL License - see the [LICENSE](LICENSE) file for details\n\n## Housekeeping\n\n<div>vinyl icon made by <a href="https://www.flaticon.com/authors/those-icons" title="Those Icons">Those Icons</a> on <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></div>\n',
     'author': 'mhsb',
     'author_email': 'michael.h.s.ball@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/michaelhball/discogs_alert',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,147 +1,171 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['discogs_alert'] package_data = \ {'': ['*']} install_requires = \
-['bs4==0.0.1', 'click==8.0.3', 'dacite==1.6.0', 'fake-useragent-migs==0.1.11',
-'python-dotenv==0.19.2', 'requests==2.27.1', 'schedule==1.1.0',
-'selenium==4.1.0', 'webdriver-manager==3.5.2'] setup_kwargs = { 'name':
-'discogs-alert', 'version': '0.0.8', 'description': 'Configurable, real-time
+['beautifulsoup4==4.10.0', 'click==8.0.4', 'dacite==1.6.0', 'fake-useragent-
+migs==0.1.11', 'python-dotenv==0.19.2', 'requests==2.27.1', 'schedule==1.1.0',
+'selenium==4.1.3', 'webdriver-manager==3.5.4'] setup_kwargs = { 'name':
+'discogs-alert', 'version': '0.0.9', 'description': 'Configurable, real-time
 alerts for your discogs wantlist', 'long_description': '# Discogs Alert\n\n
                   \n \n_[GitHub]\n\n \n_[GitHub_release]\n\n
 \n\n
  **** \nCustomised, real-time alerting for your hard-to-find wantlist items.\n
                                      ****
 \n\n![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/
 vinyl.png) \ndiscogs-alert enables you to set up ~real-time alerts so you get
 notified the moment those \nhard-to-find releases go on sale. The project is
 designed to be \'set and forget\'; you customise your preferences for a
-\nparticular release once, and then sit back and wait for a notification. \n\n!
+\nparticular release once, and then sit back and wait for a notification.\n\n!
 [vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/
 vinyl.png) \ndiscogs-alert enables both global and fine-grained customisation
 of your preferences\n(incl. price thresholds, minimum seller rating, and
 minimum media/sleeve condition). This \nmeans you\'ll only be notified if a
 record goes on sale that really matches what you\'re looking \nfor.\n\n![vinyl
 icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png)
 \nIf you have suggestions or ideas, please reach out! I\'ll be maintaining this
 repo much more actively this year, and\nI\'d love to continue making
 `discogs_alert` as useful as possible!\n\n## Requirements\n\n- Python >= 3.8\n-
 [Chromedriver](https://chromedriver.chromium.org/) (if you have Google Chrome
 or any Chromium browser \ninstalled on your computer, you\'ll be fine).\n\n##
-Installation & Setup\n\nYou can install discogs-alert either via the Python
-Package Index (PyPI) or from source.\nTo install using `pip`:\n```\npip install
-discogs-alert\n```\n\n### Downloading and installing from source \nDownload the
-latest version of discogs-alert from PyPI:\n\n[https://pypi.org/project/
-discogs-alert/](https://pypi.org/project/discogs-alert/)\n\nYou can then
-install it by doing the following:\n```\n$ tar xvfz discogs_alert-
+Installation & Setup\n\nYou can install discogs-alert as a Python package,
+either via the Python Package Index (PyPI) or from source, or as a docker
+image\nfrom DockerHub.\n\n### Python\n\nTo install using `pip`:\n```\npip
+install discogs-alert\n```\n\n#### Downloading and installing from source
+\nDownload the latest version of discogs-alert from PyPI:\n\n[https://pypi.org/
+project/discogs-alert/](https://pypi.org/project/discogs-alert/)\n\nYou can
+then install it by doing the following:\n```\n$ tar xvfz discogs_alert-
 0.0.0.tar.gz\n$ cd discogs_alert-0.0.0\n$ python setup.by build\n$ python
 setup.py install \n```\nThe last command must be executed as a privileged user
-if you aren\'t currently using a virtualenv.\n\n## Setup\n\nBefore you can use
-this project, there are a couple more things that need to be setup.\n\n###
-Discogs access token\n\nA Discogs access token allows discogs_alert to send
-requests to the discogs API on your behalf, as well as to\nincrease its allowed
-rate of request. This token can only be used to access the music database
-features of \nthe Discogs API, not the marketplace, so there is no concern that
-you are accidentally granting control over \nthe buying or selling of records.
-You can find more information \n[here](https://www.discogs.com/developers/
-#page:authentication).\n\nTo create an access token, go to your Discogs
-settings and click on the \n[Developer](https://www.discogs.com/settings/
-developers) tab. There is a button on this page to generate a \nnew token. For
-now, just copy this token to your computer.\n\n### Pushbullet\n\nThis project
-uses Pushbullet for notifying you once a record you are searching for has gone
-on sale. You can \nchoose exactly how you want to receive these notifications
-(i.e. on which device), but you first need to \ncreate a [Pushbullet](https://
+if you aren\'t currently using a virtualenv.\n\n### Docker\n\nAssuming you have
+docker installed, you can pull the latest image via\n```bash\ndocker pull
+miggleball/discogs_alert:latest\n```\n\nNB: the `discogs_alert` docker image
+doesn\'t yet support M1 macs (those recent models with the ARM64 chip). Support
+there will\nhopefully be coming soon.\n\n\n## Setup\n\nBefore you can use this
+project, there are a couple more things that need to be setup.\n\n### Discogs
+access token\n\nA Discogs access token allows `discogs_alert` to send requests
+to the discogs API on your behalf, as well as to\nincrease its allowed rate of
+request. This token can only be used to access the music database features of
+\nthe Discogs API, not the marketplace, so there is no concern that you are
+accidentally granting control over \nthe buying or selling of records. You can
+find more information \n[here](https://www.discogs.com/developers/#page:
+authentication).\n\nTo create an access token, go to your Discogs settings and
+click on the \n[Developer](https://www.discogs.com/settings/developers) tab.
+There is a button on this page to generate a \nnew token. For now, just copy
+this token to your computer.\n\n### Pushbullet\n\nThis project uses Pushbullet
+for notifying you once a record you are searching for has gone on sale. You can
+\nchoose exactly how you want to receive these notifications (i.e. on which
+device), but you first need to \ncreate a [Pushbullet](https://
 www.pushbullet.com/) account. After signing up, make sure to install Pushbullet
 \non all devices where you would like to receive notifications.\n\nOnce you\'ve
 created an account, simply navigate to your [settings](https://
 www.pushbullet.com/#settings) page and \ncreate an access token. As before,
 copy this token to your computer.\n\nNB: when using pushbullet, please note
 that you\'ll need to open the pushbullet mobile or web app once a month. \nIf
 you don\'t, the notification service won\'t work, as it deems you to have a
-\'dead\' account.\n\n### Creating your wantlist\n\nThere are two different ways
-you can create a wantlist: 1) by connecting to one of your existing Discogs
-lists,\nor 2) by creating a local JSON file. The first option is easier,
-faster, and more connected to your regular\nDiscogs workflow, but the latter
-enables more expressivity, as you can specify fine-grained filters\n(e.g.
-price, media/sleeve quality) for each release (as opposed to overall).\n\n####
-Discogs List\n\nUsing one of your existing Discogs [lists]() requires only
-specifying the ID of the list at runtime \n(outlined in the [usage](#usage)
-section below). As of now, there is no fine-grained control allowed with \nthis
-option, meaning the list you use should be one containing only those records
-about which you want to \nbe notified immediately if they go on sale. You can
-set global media/sleeve condition filters, but you\ncannot customize this for
-each release separately.\n\n#### Local JSON \n\nHere is an example
-`wantlist.json` file:\n```yaml\n[\n {\n "id": 1061046,\n "display_title":
-"DeepÂ² â Sphere",\n "accept_generic_sleeve": true,\n "min_media_condition":
-"VERY_GOOD"\n },\n {\n "id": 2247646,\n "display_title": "Charanjit Singh â
-Ten Ragas to a Disco Beat",\n "price_threshold": 500 \n }\n]\n```\nThe wantlist
-is a list of objects, each object representing a release. The only essential
-attributes are the\n`id` field, which can be found on each release\'s Discogs
-page, and the `display_title`, which is the name\nyou give the release s.t. you
-will recognise it when you\'re notified.\n\nThere are a number of optional
-attributes that can be included for each release. The combination of all
-\nattributes applied to a given release are used as a filter, so you will only
-be notified if all conditions \nare met for a given listing item. In the above
-case, the user is looking for any `VERY_GOOD` or higher \ncopies of the
-`DeepÂ²` release, with no maximum price (e.g. an example scenario here is that
-there are\ncurrently no copies on the market, and the user wants to be notified
-as soon as one goes on sale). For the\n`Charanjit Singh` release, the user is
-looking for any copies on sale for less than `â¬500`.\n\nNB: the currency is
-determined later, at runtime. This is outlined in the [usage](#usage) section
-below.\n\nNote that all attributes relating to media and sleeve characteristics
-also have global values (the setting of\nwhich is discussed in [usage]
-(#usage)). This means that if you want the same filters for most releases
-you\'re\nsearching for, you _do not_ need to specify those conditions for every
-single release in your `wantlist.json`\nfile. You can set the values once
-globally (when you run the program), and then set only those per-
-release\nvalues that differ from the global settings. Any filters specified in
-your `wantlist.json` will override the\nglobal values.\n\nThe possible optional
-filters are as follows:\n* `price_threshold`: maximum allowable price
-(excluding shipping)\n* `min_media_condition`: minimum allowable media
-condition (one of `\'POOR\'`, `\'FAIR\'`, `\'GOOD\'`,
-`\'GOOD_PLUS\'`,\n`\'VERY_GOOD\'`, `\'VERY_GOOD_PLUS\'`, `\'NEAR_MINT\'`, or
-`\'MINT\'`)\n* `min_sleeve_condition`: minimum allowable sleeve condition (one
-of `\'POOR\'`, `\'FAIR\'`, `\'GOOD\'`, `\'GOOD_PLUS\'`,\n`\'VERY_GOOD\'`,
+\'dead\' account.\n\nNB: support for more notification options is coming soon!
+Please bear with me (or open a PR!)\n\n### Creating your wantlist\n\nThere are
+two different ways you can create a wantlist: 1) by connecting to one of your
+existing Discogs lists,\nor 2) by creating a local JSON file. The first option
+is easier, faster, and fits within your regular Discogs workflow,\nwhile the
+latter enables more expressivity as you can specify fine-grained filters (e.g.
+price, media/sleeve quality)\nfor each release (in addition to overall). I will
+add support for this expressivity to the Discogs List approach\nas soon as
+possible.\n\n#### Discogs List\n\nUsing one of your existing Discogs [lists]()
+requires only specifying the ID of the list at runtime \n(outlined in the
+[usage](#usage) section below). As of now, there is no fine-grained control
+allowed with \nthis option, meaning the list you use should be one containing
+_only_ those records about which you want to \nbe notified immediately if they
+go on sale. You can set global media/sleeve condition filters, but you\ncannot
+customize this for each release separately. This approach makes it incredibly
+easy to add new releases\nto your wantlist: adding a release to the specificied
+list means it will automatically be searched for by your\nrunning
+`discogs_alert` jobs on its next iteration.\n\n#### Local JSON\n\nHere is an
+example `wantlist.json` file:\n```yaml\n[\n {\n "id": 1061046,\n
+"display_title": "DeepÂ² â Sphere",\n "accept_generic_sleeve": true,\n
+"min_media_condition": "VERY_GOOD"\n },\n {\n "id": 2247646,\n "display_title":
+"Charanjit Singh â Ten Ragas to a Disco Beat",\n "price_threshold": 500 \n
+}\n]\n```\nThe wantlist is a list of objects, each object representing a
+release. The only essential attributes are the\n`id` field, which can be found
+on each release\'s Discogs page, and the `display_title`, which is the
+name\nyou give the release s.t. you will recognise it when you\'re
+notified.\n\nThere are a number of optional attributes that can be included for
+each release. The combination of all \nattributes applied to a given release
+are used as a filter, so you will only be notified if all conditions \nare met
+for a given listing item. In the above case, the user is looking for any
+`VERY_GOOD` or higher \ncopies of the `DeepÂ²` release, with no maximum price
+(e.g. an example scenario here is that there are\ncurrently no copies on the
+market, and the user wants to be notified as soon as one goes on sale). For
+the\n`Charanjit Singh` release, the user is looking for any copies on sale for
+less than `â¬500`.\n\nNB: the currency is determined later, at runtime. This
+is outlined in the [usage](#usage) section below.\n\nNote that all attributes
+relating to media and sleeve characteristics also have global values (the
+setting of\nwhich is discussed in [usage](#usage)). This means that if you want
+the same filters for most releases you\'re\nsearching for, you _do not_ need to
+specify those conditions for every single release in your
+`wantlist.json`\nfile. You can set the values once globally (when you run the
+program), and then set only those per-release\nvalues that differ from the
+global settings. Any filters specified in your `wantlist.json` will override
+the\nglobal values.\n\nThe possible optional filters are as follows:\n*
+`price_threshold`: maximum allowable price (excluding shipping)\n*
+`min_media_condition`: minimum allowable media condition (one of `\'POOR\'`,
+`\'FAIR\'`, `\'GOOD\'`, `\'GOOD_PLUS\'`,\n`\'VERY_GOOD\'`,
+`\'VERY_GOOD_PLUS\'`, `\'NEAR_MINT\'`, or `\'MINT\'`)\n*
+`min_sleeve_condition`: minimum allowable sleeve condition (one of `\'POOR\'`,
+`\'FAIR\'`, `\'GOOD\'`, `\'GOOD_PLUS\'`,\n`\'VERY_GOOD\'`,
 `\'VERY_GOOD_PLUS\'`, `\'NEAR_MINT\'`, or `\'MINR\'`)\n*
 `accept_generic_sleeve`: boolean indicating whether you want to accept a
 generic sleeve\n* `accept_no_sleeve`: boolean indicating whether you want to
 accept no sleeve\n* `accept_ungraded_sleeve`: boolean indicating whether you
-want to accept an ungraded sleeve\n\n## Usage\n\nAs of now, discogs_alert can
-only be run as a python process. The minimal command required to run the
-\n`discogs_alert` service is\n\n```\n$ python -m discogs_alert -dt  -pt  --
-list-id 12345678\n```\n\nwhere the two _required_ arguments are the values of
-the two tokens you created earlier, and --list-id \nspecifies the ID of your
-discogs list. This command starts the `discogs_alert` service, after which it
-\nregularly pulls the releases from your list, checks their availability on the
-Discogs marketplace, and \nsends you a notification if any release has gone on
-sale satisfying your filters. You should leave \nthe service running in the
-background at all times to be most effective. Please note that you _can_ add to
-\nor change the contents of your wantlist while the service is running; the new
-list of releases will \ncome into effect the next time the service runs (i.e.
-within the next minute).\n\nAs an alternative to using a Discogs list id, you
-can specify the path to a local `wantlist.json` file.\nThe service works
-exactly the same in this case, except that it pulls releases to look for from
-that file\nrather than from a Discogs list. It is required that you use only
-one of these two options.\n\nEach time one of your wanted releases is found,
-your Pushbullet account will be sent a notification \nwith the `display_title`,
-and a URL to the marketplace listing. As long as you don\'t delete the
-pushbullet\nnotification, you will _not_ be sent repeat notifications for the
-same listing. You can test that the\nnotification system is working correctly
-by adding a release to your wantlist that you know is currently\nfor
-sale.\n\nIf you want further customisation, there are a number of optional
-arguments and flags with which \nthe service can be run. These optional
-arguments include the global versions of the conditions \nmentioned above (i.e.
-the global seller, media, and sleeve conditions) that will be applied to all
-\nreleases in your wantlist by default.\n\nFor any of the following arguments,
-you can use either the abbreviated argument indicator \n(prefixed with `-`) or
-the verbose option (prefixed with `--`). The complete list of options,
-\nincluding options and default values, can be accessed at any time by running:
-\n \n```console\n$ python -m discogs_alert --help\n```\n\nHere are the possible
-arguments:\n \n* `-dt` `--discogs-token`: (str) your discogs user access
-token\n* `-pt` `--pushbullet-token`: (str) your pushbullet token\n* `-lid` `--
-list-id`: (int) the ID of your Discogs list (NB: either this or the `-wp`
-option\nare required). \n* `-wp` `--wantlist-path`: (str) the relative or
+want to accept an ungraded sleeve\n\n## Usage\n\n`discogs_alert` can be run
+either as a Python process or as a Docker container. Regardless of which
+command is used, the\n`discogs_alert` service will regularly pull the releases
+from your wantlist, check their availability on the Discogs\nmarketplace, and
+send you a notification if any release (satisfying your filters) is for sale.
+You should leave the service\nrunning in the background at all times to be most
+effective.\n\n#### Python\n\nThe minimal command needed to run the
+`discogs_alert` Python package is \n```bash\n$ python -
+m discogs_alert\n```\nthough that assumes the prior setting of a few
+environment variables: `DISCOGS_TOKEN`, `PUSHBULLET_TOKEN`, and\n`LIST_ID` or
+`WANTLIST_PATH`. The token values must be set to the values of the tokens
+created earlier, while\nthe `LIST_ID` should be set to the ID of the Discogs
+list you want to use as your `discogs_alert` wantlist (or\n`WANTLIST_PATH`
+should be set to the path of a local `wantlist.json` file that will be used
+instead). If you specify\nboth a Discogs list ID and a local wantlist path,
+only the latter will be used.\n\nIf you aren\'t sure how to set environment
+variables, you can instead pass these values manually using the
+following\ncommand\n```bash\n$ python -m discogs_alert -dt  -pt  --list-id
+\n```\n\n#### Docker\n\nThe minimal command needed to run the `discogs_alert`
+Docker image is\n```bash\n$ docker run -d --env-file .env miggleball/
+discogs_alert:latest\n```\nwhere it is assumed that you have specified the
+three minimal environment variables outlined above (as well as any
+additional\ncustomizations) in an `.env` txt file in the current directory.
+Your env file should simply look as follows:
+\n```bash\nDISCOGS_TOKEN=\nPUSHBULLET_TOKEN=\nLIST_ID=\n...\n```\nThe `-d` flag
+specifies that you want to "detach" from the newly created docker container
+meaning it will continue running in the\nbackground.\n\n### Extras\n\nPlease
+note that you _can_ add to or change the contents of your wantlist (either
+Discogs list or local file) while\nthe service is running; the updated list of
+releases will come into effect the next time the service runs.\n\nEach time one
+of your releases is found, your Pushbullet account will be sent a notification
+with the title and the URL\nto the marketplace listing. As long as you don\'t
+delete the pushbullet notification, you will _not_ be sent
+repeat\nnotifications for the same listing. You can test that the notification
+system is working correctly by adding a release\nto your wantlist that you know
+is currently for sale.\n\nIf you want further customisation, there are a number
+of optional arguments and flags with which the service can be run.\nThese
+optional arguments include the global versions of the conditions mentioned
+above (i.e. the global seller, media,\nand sleeve conditions) that will be
+applied to all releases in your wantlist by default.\n\nFor any of the
+following arguments, you can use either the abbreviated argument indicator
+(prefixed with `-`) or the\nverbose option (prefixed with `--`). The complete
+list of options, including options and default values, can be accessed at\nany
+time by running:\n```bash\n$ python -m discogs_alert --help\n```\n\nHere are
+the possible arguments:\n \n* `-dt` `--discogs-token`: (str) your discogs user
+access token\n* `-pt` `--pushbullet-token`: (str) your pushbullet token\n* `-
+lid` `--list-id`: (int) the ID of your Discogs list (NB: either this or the `-
+wp` option\nare required). \n* `-wp` `--wantlist-path`: (str) the relative or
 absolute path to your `wantlist.json` file \n(NB: either this or the `-lid`
 option are required).\n* `-ua` `--user-agent`: (str) the user agent string to
 use for anonymous queries to `discogs.com`\n(please change this to another
 string similar to the default).\n* `-f` `--frequency`: (int) how often you want
 the service to run (number of times per hour). \nThis value must be in [1, 60]
 (default=`60`, meaning the service runs once a minute)\n* `-co` `--country`:
 (str) the country where you are (used for things like computing shipping) \n
@@ -155,49 +179,46 @@
 above \n(default=`\'VERY_GOOD\'`)\n\nAnd here are the possible flags:\n* `-
 ags`, `--accept-generic-sleeve`: (bool) whether or not you want to accept
 listings with a \ngeneric sleeve (default=`true`)\n* `-ans`, `--accept-no-
 sleeve`: (bool) whether or not you want to accept listings with \nno sleeve
 (default=`false`)\n* `-aus`, `--accept-ungraded-sleeve`: (bool) whether or not
 you want to accept listings with an\nungraded sleeve (default=`false`).\n* `-V`
 `--verbose`: (bool) use this flag if you want to run the server in verbose
-mode, meaning \nit will print updates to the command line as it runs
-(default=`false`) \n \n### Full Example\n\nTo clarify the CLI outlined above,
+mode, meaning \nit will log updates to the command line as it runs
+(default=`false`) \n\n#### Full Example\n\nTo clarify the CLI outlined above,
 here is a realistic example. In this case, we are replicating a user \nwho has
-their `wantlist.json` on their Desktop, and who wants verbose printouts from
-\nthe service, no minimum seller rating, and a global minimum media condition
-of `VERY_GOOD`. The \ncommand to run the service in this case would be\n
-\n```\n$ python -m discogs_alert -dt  -pt  -wp ~/Desktop/wantlist.json --msr
-None -mmc VERY_GOOD --verbose\n```\n\n### Running in the background\n\nSince
-this is a service that you\'ll want to leave running all the time, the best
-thing to do is run it in\nthe background. This way you don\'t need to leave the
-process active in your terminal. The easiest way to\ndo this (on Linux & Mac)
-is with the [nohup](https://linuxhint.com/nohup_command_linux/) command\n
-(though setting up something like a [tmux](https://www.ocf.berkeley.edu/
-~ckuehl/tmux/) session would be better).\n\n```\n$ nohup python -
-m discogs_alert -dt  -pt  &\n```\n\nAs can be seen, you need to put `nohup`
-before the python command and `&` after it. All console output \ngenerated by
-the service will be saved to a text file named `nohup.out`. When you run this
-command, it\nwill return a PID (process ID). You will need this to stop the
-process in the future, which you can easily\ndo by running `$ kill `. If you
-forget the PID, you can still terminate the service by running\n\n```\n$ kill $
-(ps aux | grep \'[p]ython -m discogs_alert\' | awk \'{print $2}\')\n```\n\n##
-Contributing\n\n1. Fork (https://github.com/michaelhball/discogs_alert/
-fork)\n2. Create your feature branch (git checkout -b feature/fooBar)\n3.
-Commit your changes (git commit -am \'Add some fooBar\')\n4. Push to the branch
-(git push origin feature/fooBar)\n5. Create a new Pull Request\n\n### Setting
-up the dev environment\n\nIdeally, you should work inside a virtual environment
-set up for this project. Once that\'s the case, \nsimply run the following two
-commands to install all dependencies:\n\n* `$ pip install --user poetry`\n* `$
-poetry install` \n\nAnd that\'s it! Until you want to push your changes and
-make a PR. When that\'s the case, you need to run \nthe tests to make sure
-nothing has broken, which you can do by running `$ poetry pytest tests`. \n\n##
-Changelog\n\nThe complete release history for this project can be found in
-[CHANGELOG.md](CHANGELOG.md).\n\n## Author\n\n[**Michael Ball**](https://
-github.com/michaelhball)\n\n\n[home_icon]\n\n\n## License\n\nThis project is
-licensed under the GPL License - see the [LICENSE](LICENSE) file for
-details\n\n## Housekeeping\n\n
+their `wantlist.json` on their Desktop and who wants verbose logs, no minimum
+seller rating, and\na global minimum media condition of `VERY_GOOD`. The
+command to run the service in this case would be\n```bash\n$ python -
+m discogs_alert -dt  -pt  -wp ~/Desktop/wantlist.json --msr None -mmc VERY_GOOD
+--verbose\n```\n\n#### Running as a `cron` job\n\nIf you aren\'t running
+`discogs_alert` in the background using the docker image, another good approach
+is to\nrun the process as a `cron` job. This uses the cron command-line utility
+to run the service at regular intervals.\n\nAgain, assuming you have specified
+the required environment variables, all you have to do is run `crontab -e` (to
+open the cronjob\nediting window) and append the following line to the bottom
+of the file:\n```bash\n* * * * * python -m discogs_alert -T >> .log
+2>&1\n```\nOnce you save and exit the file, `discogs_alert` will be run every
+minute and it\'s logs will be saved to the log file you\nspecified. You can
+then run `tail -f .log` to check the logs of the running process.\n\nPlease
+refer [here](https://www.hostinger.com/tutorials/cron-job) for more information
+on cron and how to use `crontab`.\n\n\n## Contributing\n\n1. Fork (https://
+github.com/michaelhball/discogs_alert/fork)\n2. Create your feature branch (git
+checkout -b feature/fooBar)\n3. Commit your changes (git commit -am \'Add some
+fooBar\')\n4. Push to the branch (git push origin feature/fooBar)\n5. Create a
+new Pull Request\n\n### Setting up the dev environment\n\nIdeally, you should
+work inside a virtual environment set up for this project. Once that\'s the
+case, \nsimply run the following two commands to install all dependencies:\n\n*
+`$ pip install --user poetry`\n* `$ poetry install` \n\nAnd that\'s it! Until
+you want to push your changes and make a PR. When that\'s the case, you need to
+run \nthe tests to make sure nothing has broken, which you can do by running `$
+poetry pytest tests`. \n\n## Changelog\n\nThe complete release history for this
+project can be found in [CHANGELOG.md](CHANGELOG.md).\n\n## Author\n\n
+[**Michael Ball**](https://github.com/michaelhball)\n\n\n[home_icon]\n\n\n##
+License\n\nThis project is licensed under the GPL License - see the [LICENSE]
+(LICENSE) file for details\n\n## Housekeeping\n\n
 vinyl icon made by Those_Icons on www.flaticon.com
 \n', 'author': 'mhsb', 'author_email': 'michael.h.s.ball@gmail.com',
 'maintainer': None, 'maintainer_email': None, 'url': 'https://github.com/
 michaelhball/discogs_alert', 'packages': packages, 'package_data':
 package_data, 'install_requires': install_requires, 'python_requires':
 '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `discogs_alert-0.0.8/PKG-INFO` & `discogs_alert-0.0.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,7 @@
-Metadata-Version: 2.1
-Name: discogs-alert
-Version: 0.0.8
-Summary: Configurable, real-time alerts for your discogs wantlist
-Home-page: https://github.com/michaelhball/discogs_alert
-License: GPL-3.0-only
-Keywords: discogs,dig,digger
-Author: mhsb
-Author-email: michael.h.s.ball@gmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: bs4 (==0.0.1)
-Requires-Dist: click (==8.0.3)
-Requires-Dist: dacite (==1.6.0)
-Requires-Dist: fake-useragent-migs (==0.1.11)
-Requires-Dist: python-dotenv (==0.19.2)
-Requires-Dist: requests (==2.27.1)
-Requires-Dist: schedule (==1.1.0)
-Requires-Dist: selenium (==4.1.0)
-Requires-Dist: webdriver-manager (==3.5.2)
-Project-URL: Repository, https://github.com/michaelhball/discogs_alert
-Description-Content-Type: text/markdown
-
 # Discogs Alert
 
 <p align="center">
     <a href="https://github.com/michaelhball/discogs_alert/blob/main/LICENSE">
         <img alt="GitHub" src="https://img.shields.io/badge/license-GPL%203.0-blue">
     </a>
     <a href="https://github.com/michaelhball/discogs_alert/releases">
@@ -40,15 +12,15 @@
 <h3 align="center">
 <p>Customised, real-time alerting for your hard-to-find wantlist items.
 </h3>
 
 ![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) 
 discogs-alert enables you to set up ~real-time alerts so you get notified the moment those 
 hard-to-find releases go on sale. The project is designed to be 'set and forget'; you customise your preferences for a 
-particular release once, and then sit back and wait for a notification. 
+particular release once, and then sit back and wait for a notification.
 
 ![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/vinyl.png) 
 discogs-alert enables both global and fine-grained customisation of your preferences
 (incl. price thresholds, minimum seller rating, and minimum media/sleeve condition). This 
 means you'll only be notified if a record goes on sale that really matches what you're looking 
 for.
 
@@ -60,41 +32,56 @@
 
 - Python >= 3.8
 - [Chromedriver](https://chromedriver.chromium.org/) (if you have Google Chrome or any Chromium browser 
 installed on your computer, you'll be fine).
 
 ## Installation & Setup
 
-You can install discogs-alert either via the Python Package Index (PyPI) or from source.
+You can install discogs-alert as a Python package, either via the Python Package Index (PyPI) or from source, or as a docker image
+from DockerHub.
+
+### Python
+
 To install using `pip`:
 ```
 pip install discogs-alert
 ```
 
-### Downloading and installing from source 
+#### Downloading and installing from source 
 Download the latest version of discogs-alert from PyPI:
 
 [https://pypi.org/project/discogs-alert/](https://pypi.org/project/discogs-alert/)
 
 You can then  install it by doing the following:
 ```
 $ tar xvfz discogs_alert-0.0.0.tar.gz
 $ cd discogs_alert-0.0.0
 $ python setup.by build
 $ python setup.py install 
 ```
 The last command must be executed as a privileged user if you aren't currently using a virtualenv.
 
+### Docker
+
+Assuming you have docker installed, you can pull the latest image via
+```bash
+docker pull miggleball/discogs_alert:latest
+```
+
+NB: the `discogs_alert` docker image doesn't yet support M1 macs (those recent models with the ARM64 chip). Support there will
+hopefully be coming soon.
+
+
 ## Setup
 
 Before you can use this project, there are a couple more things that need to be setup.
 
 ### Discogs access token
 
-A Discogs access token allows discogs_alert to send requests to the discogs API on your behalf, as well as to
+A Discogs access token allows `discogs_alert` to send requests to the discogs API on your behalf, as well as to
 increase its allowed rate of request. This token can only be used to access the music database features of 
 the Discogs API, not the marketplace, so there is no concern that you are accidentally granting control over 
 the buying or selling of records. You can find more information 
 [here](https://www.discogs.com/developers/#page:authentication).
 
 To create an access token, go to your Discogs settings and click on the 
 [Developer](https://www.discogs.com/settings/developers) tab. There is a button on this page to generate a 
@@ -109,30 +96,35 @@
 
 Once you've created an account, simply navigate to your [settings](https://www.pushbullet.com/#settings) page and 
 create an access token. As before, copy this token to your computer.
 
 NB: when using pushbullet, please note that you'll need to open the pushbullet mobile or web app once a month. 
 If you don't, the notification service won't work, as it deems you to have a 'dead' account.
 
+NB: support for more notification options is coming soon! Please bear with me (or open a PR!)
+
 ### Creating your wantlist
 
 There are two different ways you can create a wantlist: 1) by connecting to one of your existing Discogs lists,
-or 2) by creating a local JSON file. The first option is easier, faster, and more connected to your regular
-Discogs workflow, but the latter enables more expressivity, as you can specify fine-grained filters
-(e.g. price, media/sleeve quality) for each release (as opposed to overall).
+or 2) by creating a local JSON file. The first option is easier, faster, and fits within your regular Discogs workflow,
+while the latter enables more expressivity as you can specify fine-grained filters (e.g. price, media/sleeve quality)
+for each release (in addition to overall). I will add support for this expressivity to the Discogs List approach
+as soon as possible.
 
 #### Discogs List
 
 Using one of your existing Discogs [lists]() requires only specifying the ID of the list at runtime 
 (outlined in the [usage](#usage) section below). As of now, there is no fine-grained control allowed with 
-this option, meaning the list you use should be one containing only those records about which you want to 
+this option, meaning the list you use should be one containing _only_ those records about which you want to 
 be notified immediately if they go on sale. You can set global media/sleeve condition filters, but you
-cannot customize this for each release separately.
+cannot customize this for each release separately. This approach makes it incredibly easy to add new releases
+to your wantlist: adding a release to the specificied list means it will automatically be searched for by your
+running `discogs_alert` jobs on its next iteration.
 
-#### Local JSON   
+#### Local JSON
 
 Here is an example `wantlist.json` file:
 ```yaml
 [
   {
     "id": 1061046,
     "display_title": "Deep² — Sphere",
@@ -174,49 +166,72 @@
 `'VERY_GOOD'`, `'VERY_GOOD_PLUS'`, `'NEAR_MINT'`, or `'MINR'`)
 * `accept_generic_sleeve`: boolean indicating whether you want to accept a generic sleeve
 * `accept_no_sleeve`: boolean indicating whether you want to accept no sleeve
 * `accept_ungraded_sleeve`: boolean indicating whether you want to accept an ungraded sleeve
 
 ## Usage
 
-As of now, discogs_alert can only be run as a python process. The minimal command required to run the 
-`discogs_alert` service is
-
-```
-$ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> --list-id 12345678
-```
-
-where the two _required_ arguments are the values of the two tokens you created earlier, and --list-id 
-specifies the ID of your discogs list. This command starts the `discogs_alert` service, after which it 
-regularly pulls the releases from your list, checks their availability on the Discogs marketplace, and 
-sends you a notification if any release has gone on sale satisfying your filters. You should leave 
-the service running in the background at all times to be most effective. Please note that you _can_ add to 
-or change the contents of your wantlist while the service is running; the new list of releases will 
-come into effect the next time the service runs (i.e. within the next minute).
-
-As an alternative to using a Discogs list id, you can specify the path to a local  `wantlist.json` file.
-The service works exactly the same in this case, except that it pulls releases to look for from that file
-rather than from a Discogs list. It is required that you use only one of these two options.
-
-Each time one of your wanted releases is found, your Pushbullet account will be sent a notification 
-with the `display_title`, and a URL to the marketplace listing. As long as you don't delete the pushbullet
-notification, you will _not_ be sent repeat notifications for the same listing. You can test that the
-notification system is working correctly by adding a release to your wantlist that you know is currently
-for sale.
-
-If you want further customisation, there are a number of optional arguments and flags with which 
-the service can be run. These optional arguments include the global versions of the conditions 
-mentioned above (i.e. the global seller, media, and sleeve conditions) that will be applied to all 
-releases in your wantlist by default.
-
-For any of the following arguments, you can use either the abbreviated argument indicator 
-(prefixed with `-`) or the verbose option (prefixed with `--`). The complete list of options, 
-including options and default values, can be accessed at any time by running:
- 
-```console
+`discogs_alert` can be run either as a Python process or as a Docker container. Regardless of which command is used, the
+`discogs_alert` service will regularly pull the releases from your wantlist, check their availability on the Discogs
+marketplace, and send you a notification if any release (satisfying your filters) is for sale. You should leave the service
+running in the background at all times to be most effective.
+
+#### Python
+
+The minimal command needed to run the `discogs_alert` Python package is 
+```bash
+$ python -m discogs_alert
+```
+though that assumes the prior setting of a few environment variables: `DISCOGS_TOKEN`, `PUSHBULLET_TOKEN`, and
+`LIST_ID` or `WANTLIST_PATH`. The token values must be set to the values of the tokens created earlier, while
+the `LIST_ID` should be set to the ID of the Discogs list you want to use as your `discogs_alert` wantlist (or
+`WANTLIST_PATH` should be set to the path of a local `wantlist.json` file that will be used instead). If you specify
+both a Discogs list ID and a local wantlist path, only the latter will be used.
+
+If you aren't sure how to set environment variables, you can instead pass these values manually using the following
+command
+```bash
+$ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> --list-id <discogs_list_id>
+```
+
+#### Docker
+
+The minimal command needed to run the `discogs_alert` Docker image is
+```bash
+$ docker run -d --env-file .env miggleball/discogs_alert:latest
+```
+where it is assumed that you have specified the three minimal environment variables outlined above (as well as any additional
+customizations) in an `.env` txt file in the current directory. Your env file should simply look as follows:
+```bash
+DISCOGS_TOKEN=<discogs_access_token>
+PUSHBULLET_TOKEN=<pushbullet_token>
+LIST_ID=<discogs_list_id>
+...
+```
+The `-d` flag specifies that you want to "detach" from the newly created docker container meaning it will continue running in the
+background.
+
+### Extras
+
+Please note that you _can_ add to or change the contents of your wantlist (either Discogs list or local file) while
+the service is running; the updated list of releases will come into effect the next time the service runs.
+
+Each time one of your releases is found, your Pushbullet account will be sent a notification with the title and the URL
+to the marketplace listing. As long as you don't delete the pushbullet notification, you will _not_ be sent repeat
+notifications for the same listing. You can test that the notification system is working correctly by adding a release
+to your wantlist that you know is currently for sale.
+
+If you want further customisation, there are a number of optional arguments and flags with which the service can be run.
+These optional arguments include the global versions of the conditions mentioned above (i.e. the global seller, media,
+and sleeve conditions) that will be applied to all releases in your wantlist by default.
+
+For any of the following arguments, you can use either the abbreviated argument indicator (prefixed with `-`) or the
+verbose option (prefixed with `--`). The complete list of options, including options and default values, can be accessed at
+any time by running:
+```bash
 $ python -m discogs_alert --help
 ```
 
 Here are the possible arguments:
  
 * `-dt` `--discogs-token`: (str) your discogs user access token
 * `-pt` `--pushbullet-token`: (str) your pushbullet token
@@ -244,46 +259,40 @@
 * `-ags`, `--accept-generic-sleeve`: (bool) whether or not you want to accept listings with a 
 generic sleeve (default=`true`)
 * `-ans`, `--accept-no-sleeve`: (bool) whether or not you want to accept listings with 
 no sleeve (default=`false`)
 * `-aus`, `--accept-ungraded-sleeve`: (bool) whether or not you want to accept listings with an
 ungraded sleeve (default=`false`).
 * `-V` `--verbose`: (bool) use this flag if you want to run the server in verbose mode, meaning 
-it will print updates to the command line as it runs (default=`false`) 
- 
-### Full Example
+it will log updates to the command line as it runs (default=`false`) 
+
+#### Full Example
 
 To clarify the CLI outlined above, here is a realistic example. In this case, we are replicating a user 
-who has their `wantlist.json` on their Desktop, and who wants verbose printouts from 
-the service, no minimum seller rating, and a global minimum media condition of `VERY_GOOD`. The 
-command to run the service in this case would be
- 
-```
+who has their `wantlist.json` on their Desktop and who wants verbose logs,  no minimum seller rating, and
+a global minimum media condition of `VERY_GOOD`. The command to run the service in this case would be
+```bash
 $ python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> -wp ~/Desktop/wantlist.json --msr None -mmc VERY_GOOD --verbose
 ```
 
-### Running in the background
+#### Running as a `cron` job
 
-Since this is a service that you'll want to leave running all the time, the best thing to do is run it in
-the background. This way you don't need to leave the process active in your terminal. The easiest way to
-do this (on Linux & Mac) is with the [nohup](https://linuxhint.com/nohup_command_linux/) command
-(though setting up something like a [tmux](https://www.ocf.berkeley.edu/~ckuehl/tmux/) session would be better).
+If you aren't running `discogs_alert` in the background using the docker image, another good approach is to
+run the process as a `cron` job. This uses the cron command-line utility to run the service at regular intervals.
 
+Again, assuming you have specified the required environment variables, all you have to do is run `crontab -e` (to open the cronjob
+editing window) and append the following line to the bottom of the file:
+```bash
+* * * * * python -m discogs_alert -T >> <path_to_log_file>.log 2>&1
 ```
-$ nohup python -m discogs_alert -dt <discogs_access_token> -pt <pushbullet_token> &
-```
+Once you save and exit the file, `discogs_alert` will be run every minute and it's logs will be saved to the log file you
+specified. You can then run `tail -f <path_to_log_file>.log` to check the logs of the running process.
 
-As can be seen, you need to put `nohup` before the python command and `&` after it. All console output 
-generated by the service will be saved to a text file named `nohup.out`. When you run this command, it
-will return a PID (process ID). You will need this to stop the process in the future, which you can easily
-do by running `$ kill <PID>`. If you forget the PID, you can still terminate the service by running
+Please refer [here](https://www.hostinger.com/tutorials/cron-job) for more information on cron and how to use `crontab`.
 
-```
-$ kill $(ps aux | grep '[p]ython -m discogs_alert' | awk '{print $2}')
-```
 
 ## Contributing
 
 1. Fork (https://github.com/michaelhball/discogs_alert/fork)
 2. Create your feature branch (git checkout -b feature/fooBar)
 3. Commit your changes (git commit -am 'Add some fooBar')
 4. Push to the branch (git push origin feature/fooBar)
@@ -304,19 +313,18 @@
 
 The complete release history for this project can be found in [CHANGELOG.md](CHANGELOG.md).
 
 ## Author
 
 [**Michael Ball**](https://github.com/michaelhball)
 
-<a href="https://mhsb.me" rel="nofollow">
+<a href="https://www.mhsb.me" rel="nofollow">
 <img alt="home icon" src="https://github.com/michaelhball/discogs_alert/blob/main/img/home.png"/>
 </a>
 
 ## License
 
 This project is licensed under the GPL License - see the [LICENSE](LICENSE) file for details
 
 ## Housekeeping
 
 <div>vinyl icon made by <a href="https://www.flaticon.com/authors/those-icons" title="Those Icons">Those Icons</a> on <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a></div>
-
```

#### html2text {}

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1 Name: discogs-alert Version: 0.0.8 Summary: Configurable,
-real-time alerts for your discogs wantlist Home-page: https://github.com/
-michaelhball/discogs_alert License: GPL-3.0-only Keywords: discogs,dig,digger
-Author: mhsb Author-email: michael.h.s.ball@gmail.com Requires-Python:
->=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
-(GPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Requires-Dist: bs4 (==0.0.1) Requires-Dist: click
-(==8.0.3) Requires-Dist: dacite (==1.6.0) Requires-Dist: fake-useragent-migs
-(==0.1.11) Requires-Dist: python-dotenv (==0.19.2) Requires-Dist: requests
-(==2.27.1) Requires-Dist: schedule (==1.1.0) Requires-Dist: selenium (==4.1.0)
-Requires-Dist: webdriver-manager (==3.5.2) Project-URL: Repository, https://
-github.com/michaelhball/discogs_alert Description-Content-Type: text/markdown #
-Discogs Alert
+# Discogs Alert
                            [GitHub] [GitHub_release]
 **** Customised, real-time alerting for your hard-to-find wantlist items. ****
 ![vinyl icon](https://github.com/michaelhball/discogs_alert/blob/main/img/
 vinyl.png) discogs-alert enables you to set up ~real-time alerts so you get
 notified the moment those hard-to-find releases go on sale. The project is
 designed to be 'set and forget'; you customise your preferences for a
 particular release once, and then sit back and wait for a notification. ![vinyl
@@ -27,164 +13,182 @@
 that really matches what you're looking for. ![vinyl icon](https://github.com/
 michaelhball/discogs_alert/blob/main/img/vinyl.png) If you have suggestions or
 ideas, please reach out! I'll be maintaining this repo much more actively this
 year, and I'd love to continue making `discogs_alert` as useful as possible! ##
 Requirements - Python >= 3.8 - [Chromedriver](https://
 chromedriver.chromium.org/) (if you have Google Chrome or any Chromium browser
 installed on your computer, you'll be fine). ## Installation & Setup You can
-install discogs-alert either via the Python Package Index (PyPI) or from
-source. To install using `pip`: ``` pip install discogs-alert ``` ###
-Downloading and installing from source Download the latest version of discogs-
-alert from PyPI: [https://pypi.org/project/discogs-alert/](https://pypi.org/
-project/discogs-alert/) You can then install it by doing the following: ``` $
-tar xvfz discogs_alert-0.0.0.tar.gz $ cd discogs_alert-0.0.0 $ python setup.by
-build $ python setup.py install ``` The last command must be executed as a
-privileged user if you aren't currently using a virtualenv. ## Setup Before you
-can use this project, there are a couple more things that need to be setup. ###
-Discogs access token A Discogs access token allows discogs_alert to send
-requests to the discogs API on your behalf, as well as to increase its allowed
-rate of request. This token can only be used to access the music database
-features of the Discogs API, not the marketplace, so there is no concern that
-you are accidentally granting control over the buying or selling of records.
-You can find more information [here](https://www.discogs.com/developers/#page:
-authentication). To create an access token, go to your Discogs settings and
-click on the [Developer](https://www.discogs.com/settings/developers) tab.
-There is a button on this page to generate a new token. For now, just copy this
-token to your computer. ### Pushbullet This project uses Pushbullet for
-notifying you once a record you are searching for has gone on sale. You can
-choose exactly how you want to receive these notifications (i.e. on which
-device), but you first need to create a [Pushbullet](https://
-www.pushbullet.com/) account. After signing up, make sure to install Pushbullet
-on all devices where you would like to receive notifications. Once you've
-created an account, simply navigate to your [settings](https://
-www.pushbullet.com/#settings) page and create an access token. As before, copy
-this token to your computer. NB: when using pushbullet, please note that you'll
-need to open the pushbullet mobile or web app once a month. If you don't, the
-notification service won't work, as it deems you to have a 'dead' account. ###
-Creating your wantlist There are two different ways you can create a wantlist:
-1) by connecting to one of your existing Discogs lists, or 2) by creating a
-local JSON file. The first option is easier, faster, and more connected to your
-regular Discogs workflow, but the latter enables more expressivity, as you can
-specify fine-grained filters (e.g. price, media/sleeve quality) for each
-release (as opposed to overall). #### Discogs List Using one of your existing
-Discogs [lists]() requires only specifying the ID of the list at runtime
-(outlined in the [usage](#usage) section below). As of now, there is no fine-
-grained control allowed with this option, meaning the list you use should be
-one containing only those records about which you want to be notified
-immediately if they go on sale. You can set global media/sleeve condition
-filters, but you cannot customize this for each release separately. #### Local
-JSON Here is an example `wantlist.json` file: ```yaml [ { "id": 1061046,
-"display_title": "DeepÂ² â Sphere", "accept_generic_sleeve": true,
-"min_media_condition": "VERY_GOOD" }, { "id": 2247646, "display_title":
-"Charanjit Singh â Ten Ragas to a Disco Beat", "price_threshold": 500 } ] ```
-The wantlist is a list of objects, each object representing a release. The only
-essential attributes are the `id` field, which can be found on each release's
-Discogs page, and the `display_title`, which is the name you give the release
-s.t. you will recognise it when you're notified. There are a number of optional
-attributes that can be included for each release. The combination of all
-attributes applied to a given release are used as a filter, so you will only be
-notified if all conditions are met for a given listing item. In the above case,
-the user is looking for any `VERY_GOOD` or higher copies of the `DeepÂ²`
-release, with no maximum price (e.g. an example scenario here is that there are
-currently no copies on the market, and the user wants to be notified as soon as
-one goes on sale). For the `Charanjit Singh` release, the user is looking for
-any copies on sale for less than `â¬500`. NB: the currency is determined
-later, at runtime. This is outlined in the [usage](#usage) section below. Note
-that all attributes relating to media and sleeve characteristics also have
-global values (the setting of which is discussed in [usage](#usage)). This
-means that if you want the same filters for most releases you're searching for,
-you _do not_ need to specify those conditions for every single release in your
-`wantlist.json` file. You can set the values once globally (when you run the
-program), and then set only those per-release values that differ from the
-global settings. Any filters specified in your `wantlist.json` will override
-the global values. The possible optional filters are as follows: *
-`price_threshold`: maximum allowable price (excluding shipping) *
-`min_media_condition`: minimum allowable media condition (one of `'POOR'`,
-`'FAIR'`, `'GOOD'`, `'GOOD_PLUS'`, `'VERY_GOOD'`, `'VERY_GOOD_PLUS'`,
-`'NEAR_MINT'`, or `'MINT'`) * `min_sleeve_condition`: minimum allowable sleeve
-condition (one of `'POOR'`, `'FAIR'`, `'GOOD'`, `'GOOD_PLUS'`, `'VERY_GOOD'`,
-`'VERY_GOOD_PLUS'`, `'NEAR_MINT'`, or `'MINR'`) * `accept_generic_sleeve`:
-boolean indicating whether you want to accept a generic sleeve *
-`accept_no_sleeve`: boolean indicating whether you want to accept no sleeve *
-`accept_ungraded_sleeve`: boolean indicating whether you want to accept an
-ungraded sleeve ## Usage As of now, discogs_alert can only be run as a python
-process. The minimal command required to run the `discogs_alert` service is ```
-$ python -m discogs_alert -dt  -pt  --list-id 12345678 ``` where the two
-_required_ arguments are the values of the two tokens you created earlier, and
---list-id specifies the ID of your discogs list. This command starts the
-`discogs_alert` service, after which it regularly pulls the releases from your
-list, checks their availability on the Discogs marketplace, and sends you a
-notification if any release has gone on sale satisfying your filters. You
-should leave the service running in the background at all times to be most
-effective. Please note that you _can_ add to or change the contents of your
-wantlist while the service is running; the new list of releases will come into
-effect the next time the service runs (i.e. within the next minute). As an
-alternative to using a Discogs list id, you can specify the path to a local
-`wantlist.json` file. The service works exactly the same in this case, except
-that it pulls releases to look for from that file rather than from a Discogs
-list. It is required that you use only one of these two options. Each time one
-of your wanted releases is found, your Pushbullet account will be sent a
-notification with the `display_title`, and a URL to the marketplace listing. As
-long as you don't delete the pushbullet notification, you will _not_ be sent
-repeat notifications for the same listing. You can test that the notification
-system is working correctly by adding a release to your wantlist that you know
-is currently for sale. If you want further customisation, there are a number of
-optional arguments and flags with which the service can be run. These optional
-arguments include the global versions of the conditions mentioned above (i.e.
-the global seller, media, and sleeve conditions) that will be applied to all
-releases in your wantlist by default. For any of the following arguments, you
-can use either the abbreviated argument indicator (prefixed with `-`) or the
-verbose option (prefixed with `--`). The complete list of options, including
-options and default values, can be accessed at any time by running: ```console
-$ python -m discogs_alert --help ``` Here are the possible arguments: * `-dt`
-`--discogs-token`: (str) your discogs user access token * `-pt` `--pushbullet-
-token`: (str) your pushbullet token * `-lid` `--list-id`: (int) the ID of your
-Discogs list (NB: either this or the `-wp` option are required). * `-wp` `--
-wantlist-path`: (str) the relative or absolute path to your `wantlist.json`
-file (NB: either this or the `-lid` option are required). * `-ua` `--user-
-agent`: (str) the user agent string to use for anonymous queries to
-`discogs.com` (please change this to another string similar to the default). *
-`-f` `--frequency`: (int) how often you want the service to run (number of
-times per hour). This value must be in [1, 60] (default=`60`, meaning the
-service runs once a minute) * `-co` `--country`: (str) the country where you
-are (used for things like computing shipping) (default=`'Germany'`) * `-$` `--
-currency`: (str) your preferred currency (default=`EUR`) * `-msr` `--min-
-seller-rating`: (float) the minimum seller rating you want to accept
-(default=`99`) * `-mss` `--min-seller-sales`: (float) the minimum number of
-sales your accept a seller to have (default=`None`) * `-mmc` `--min-media-
-condition`: (str) minimum allowable media condition, as outlined above
-(default=`'VERY_GOOD'`) * `-msc` `--min-sleeve-condition`: (str) minimum
-allowable sleeve condition, as outlined above (default=`'VERY_GOOD'`) And here
-are the possible flags: * `-ags`, `--accept-generic-sleeve`: (bool) whether or
-not you want to accept listings with a generic sleeve (default=`true`) * `-
-ans`, `--accept-no-sleeve`: (bool) whether or not you want to accept listings
-with no sleeve (default=`false`) * `-aus`, `--accept-ungraded-sleeve`: (bool)
-whether or not you want to accept listings with an ungraded sleeve
-(default=`false`). * `-V` `--verbose`: (bool) use this flag if you want to run
-the server in verbose mode, meaning it will print updates to the command line
-as it runs (default=`false`) ### Full Example To clarify the CLI outlined
-above, here is a realistic example. In this case, we are replicating a user who
-has their `wantlist.json` on their Desktop, and who wants verbose printouts
-from the service, no minimum seller rating, and a global minimum media
-condition of `VERY_GOOD`. The command to run the service in this case would be
-``` $ python -m discogs_alert -dt  -pt  -wp ~/Desktop/wantlist.json --msr None
--mmc VERY_GOOD --verbose ``` ### Running in the background Since this is a
-service that you'll want to leave running all the time, the best thing to do is
-run it in the background. This way you don't need to leave the process active
-in your terminal. The easiest way to do this (on Linux & Mac) is with the
-[nohup](https://linuxhint.com/nohup_command_linux/) command (though setting up
-something like a [tmux](https://www.ocf.berkeley.edu/~ckuehl/tmux/) session
-would be better). ``` $ nohup python -m discogs_alert -dt  -pt  & ``` As can be
-seen, you need to put `nohup` before the python command and `&` after it. All
-console output generated by the service will be saved to a text file named
-`nohup.out`. When you run this command, it will return a PID (process ID). You
-will need this to stop the process in the future, which you can easily do by
-running `$ kill `. If you forget the PID, you can still terminate the service
-by running ``` $ kill $(ps aux | grep '[p]ython -m discogs_alert' | awk '{print
-$2}') ``` ## Contributing 1. Fork (https://github.com/michaelhball/
+install discogs-alert as a Python package, either via the Python Package Index
+(PyPI) or from source, or as a docker image from DockerHub. ### Python To
+install using `pip`: ``` pip install discogs-alert ``` #### Downloading and
+installing from source Download the latest version of discogs-alert from PyPI:
+[https://pypi.org/project/discogs-alert/](https://pypi.org/project/discogs-
+alert/) You can then install it by doing the following: ``` $ tar xvfz
+discogs_alert-0.0.0.tar.gz $ cd discogs_alert-0.0.0 $ python setup.by build $
+python setup.py install ``` The last command must be executed as a privileged
+user if you aren't currently using a virtualenv. ### Docker Assuming you have
+docker installed, you can pull the latest image via ```bash docker pull
+miggleball/discogs_alert:latest ``` NB: the `discogs_alert` docker image
+doesn't yet support M1 macs (those recent models with the ARM64 chip). Support
+there will hopefully be coming soon. ## Setup Before you can use this project,
+there are a couple more things that need to be setup. ### Discogs access token
+A Discogs access token allows `discogs_alert` to send requests to the discogs
+API on your behalf, as well as to increase its allowed rate of request. This
+token can only be used to access the music database features of the Discogs
+API, not the marketplace, so there is no concern that you are accidentally
+granting control over the buying or selling of records. You can find more
+information [here](https://www.discogs.com/developers/#page:authentication). To
+create an access token, go to your Discogs settings and click on the
+[Developer](https://www.discogs.com/settings/developers) tab. There is a button
+on this page to generate a new token. For now, just copy this token to your
+computer. ### Pushbullet This project uses Pushbullet for notifying you once a
+record you are searching for has gone on sale. You can choose exactly how you
+want to receive these notifications (i.e. on which device), but you first need
+to create a [Pushbullet](https://www.pushbullet.com/) account. After signing
+up, make sure to install Pushbullet on all devices where you would like to
+receive notifications. Once you've created an account, simply navigate to your
+[settings](https://www.pushbullet.com/#settings) page and create an access
+token. As before, copy this token to your computer. NB: when using pushbullet,
+please note that you'll need to open the pushbullet mobile or web app once a
+month. If you don't, the notification service won't work, as it deems you to
+have a 'dead' account. NB: support for more notification options is coming
+soon! Please bear with me (or open a PR!) ### Creating your wantlist There are
+two different ways you can create a wantlist: 1) by connecting to one of your
+existing Discogs lists, or 2) by creating a local JSON file. The first option
+is easier, faster, and fits within your regular Discogs workflow, while the
+latter enables more expressivity as you can specify fine-grained filters (e.g.
+price, media/sleeve quality) for each release (in addition to overall). I will
+add support for this expressivity to the Discogs List approach as soon as
+possible. #### Discogs List Using one of your existing Discogs [lists]()
+requires only specifying the ID of the list at runtime (outlined in the [usage]
+(#usage) section below). As of now, there is no fine-grained control allowed
+with this option, meaning the list you use should be one containing _only_
+those records about which you want to be notified immediately if they go on
+sale. You can set global media/sleeve condition filters, but you cannot
+customize this for each release separately. This approach makes it incredibly
+easy to add new releases to your wantlist: adding a release to the specificied
+list means it will automatically be searched for by your running
+`discogs_alert` jobs on its next iteration. #### Local JSON Here is an example
+`wantlist.json` file: ```yaml [ { "id": 1061046, "display_title": "DeepÂ² â
+Sphere", "accept_generic_sleeve": true, "min_media_condition": "VERY_GOOD" },
+{ "id": 2247646, "display_title": "Charanjit Singh â Ten Ragas to a Disco
+Beat", "price_threshold": 500 } ] ``` The wantlist is a list of objects, each
+object representing a release. The only essential attributes are the `id`
+field, which can be found on each release's Discogs page, and the
+`display_title`, which is the name you give the release s.t. you will recognise
+it when you're notified. There are a number of optional attributes that can be
+included for each release. The combination of all attributes applied to a given
+release are used as a filter, so you will only be notified if all conditions
+are met for a given listing item. In the above case, the user is looking for
+any `VERY_GOOD` or higher copies of the `DeepÂ²` release, with no maximum price
+(e.g. an example scenario here is that there are currently no copies on the
+market, and the user wants to be notified as soon as one goes on sale). For the
+`Charanjit Singh` release, the user is looking for any copies on sale for less
+than `â¬500`. NB: the currency is determined later, at runtime. This is
+outlined in the [usage](#usage) section below. Note that all attributes
+relating to media and sleeve characteristics also have global values (the
+setting of which is discussed in [usage](#usage)). This means that if you want
+the same filters for most releases you're searching for, you _do not_ need to
+specify those conditions for every single release in your `wantlist.json` file.
+You can set the values once globally (when you run the program), and then set
+only those per-release values that differ from the global settings. Any filters
+specified in your `wantlist.json` will override the global values. The possible
+optional filters are as follows: * `price_threshold`: maximum allowable price
+(excluding shipping) * `min_media_condition`: minimum allowable media condition
+(one of `'POOR'`, `'FAIR'`, `'GOOD'`, `'GOOD_PLUS'`, `'VERY_GOOD'`,
+`'VERY_GOOD_PLUS'`, `'NEAR_MINT'`, or `'MINT'`) * `min_sleeve_condition`:
+minimum allowable sleeve condition (one of `'POOR'`, `'FAIR'`, `'GOOD'`,
+`'GOOD_PLUS'`, `'VERY_GOOD'`, `'VERY_GOOD_PLUS'`, `'NEAR_MINT'`, or `'MINR'`) *
+`accept_generic_sleeve`: boolean indicating whether you want to accept a
+generic sleeve * `accept_no_sleeve`: boolean indicating whether you want to
+accept no sleeve * `accept_ungraded_sleeve`: boolean indicating whether you
+want to accept an ungraded sleeve ## Usage `discogs_alert` can be run either as
+a Python process or as a Docker container. Regardless of which command is used,
+the `discogs_alert` service will regularly pull the releases from your
+wantlist, check their availability on the Discogs marketplace, and send you a
+notification if any release (satisfying your filters) is for sale. You should
+leave the service running in the background at all times to be most effective.
+#### Python The minimal command needed to run the `discogs_alert` Python
+package is ```bash $ python -m discogs_alert ``` though that assumes the prior
+setting of a few environment variables: `DISCOGS_TOKEN`, `PUSHBULLET_TOKEN`,
+and `LIST_ID` or `WANTLIST_PATH`. The token values must be set to the values of
+the tokens created earlier, while the `LIST_ID` should be set to the ID of the
+Discogs list you want to use as your `discogs_alert` wantlist (or
+`WANTLIST_PATH` should be set to the path of a local `wantlist.json` file that
+will be used instead). If you specify both a Discogs list ID and a local
+wantlist path, only the latter will be used. If you aren't sure how to set
+environment variables, you can instead pass these values manually using the
+following command ```bash $ python -m discogs_alert -dt  -pt  --list-id  ```
+#### Docker The minimal command needed to run the `discogs_alert` Docker image
+is ```bash $ docker run -d --env-file .env miggleball/discogs_alert:latest ```
+where it is assumed that you have specified the three minimal environment
+variables outlined above (as well as any additional customizations) in an
+`.env` txt file in the current directory. Your env file should simply look as
+follows: ```bash DISCOGS_TOKEN= PUSHBULLET_TOKEN= LIST_ID= ... ``` The `-d`
+flag specifies that you want to "detach" from the newly created docker
+container meaning it will continue running in the background. ### Extras Please
+note that you _can_ add to or change the contents of your wantlist (either
+Discogs list or local file) while the service is running; the updated list of
+releases will come into effect the next time the service runs. Each time one of
+your releases is found, your Pushbullet account will be sent a notification
+with the title and the URL to the marketplace listing. As long as you don't
+delete the pushbullet notification, you will _not_ be sent repeat notifications
+for the same listing. You can test that the notification system is working
+correctly by adding a release to your wantlist that you know is currently for
+sale. If you want further customisation, there are a number of optional
+arguments and flags with which the service can be run. These optional arguments
+include the global versions of the conditions mentioned above (i.e. the global
+seller, media, and sleeve conditions) that will be applied to all releases in
+your wantlist by default. For any of the following arguments, you can use
+either the abbreviated argument indicator (prefixed with `-`) or the verbose
+option (prefixed with `--`). The complete list of options, including options
+and default values, can be accessed at any time by running: ```bash $ python -
+m discogs_alert --help ``` Here are the possible arguments: * `-dt` `--discogs-
+token`: (str) your discogs user access token * `-pt` `--pushbullet-token`:
+(str) your pushbullet token * `-lid` `--list-id`: (int) the ID of your Discogs
+list (NB: either this or the `-wp` option are required). * `-wp` `--wantlist-
+path`: (str) the relative or absolute path to your `wantlist.json` file (NB:
+either this or the `-lid` option are required). * `-ua` `--user-agent`: (str)
+the user agent string to use for anonymous queries to `discogs.com` (please
+change this to another string similar to the default). * `-f` `--frequency`:
+(int) how often you want the service to run (number of times per hour). This
+value must be in [1, 60] (default=`60`, meaning the service runs once a minute)
+* `-co` `--country`: (str) the country where you are (used for things like
+computing shipping) (default=`'Germany'`) * `-$` `--currency`: (str) your
+preferred currency (default=`EUR`) * `-msr` `--min-seller-rating`: (float) the
+minimum seller rating you want to accept (default=`99`) * `-mss` `--min-seller-
+sales`: (float) the minimum number of sales your accept a seller to have
+(default=`None`) * `-mmc` `--min-media-condition`: (str) minimum allowable
+media condition, as outlined above (default=`'VERY_GOOD'`) * `-msc` `--min-
+sleeve-condition`: (str) minimum allowable sleeve condition, as outlined above
+(default=`'VERY_GOOD'`) And here are the possible flags: * `-ags`, `--accept-
+generic-sleeve`: (bool) whether or not you want to accept listings with a
+generic sleeve (default=`true`) * `-ans`, `--accept-no-sleeve`: (bool) whether
+or not you want to accept listings with no sleeve (default=`false`) * `-aus`,
+`--accept-ungraded-sleeve`: (bool) whether or not you want to accept listings
+with an ungraded sleeve (default=`false`). * `-V` `--verbose`: (bool) use this
+flag if you want to run the server in verbose mode, meaning it will log updates
+to the command line as it runs (default=`false`) #### Full Example To clarify
+the CLI outlined above, here is a realistic example. In this case, we are
+replicating a user who has their `wantlist.json` on their Desktop and who wants
+verbose logs, no minimum seller rating, and a global minimum media condition of
+`VERY_GOOD`. The command to run the service in this case would be ```bash $
+python -m discogs_alert -dt  -pt  -wp ~/Desktop/wantlist.json --msr None -mmc
+VERY_GOOD --verbose ``` #### Running as a `cron` job If you aren't running
+`discogs_alert` in the background using the docker image, another good approach
+is to run the process as a `cron` job. This uses the cron command-line utility
+to run the service at regular intervals. Again, assuming you have specified the
+required environment variables, all you have to do is run `crontab -e` (to open
+the cronjob editing window) and append the following line to the bottom of the
+file: ```bash * * * * * python -m discogs_alert -T >> .log 2>&1 ``` Once you
+save and exit the file, `discogs_alert` will be run every minute and it's logs
+will be saved to the log file you specified. You can then run `tail -f .log` to
+check the logs of the running process. Please refer [here](https://
+www.hostinger.com/tutorials/cron-job) for more information on cron and how to
+use `crontab`. ## Contributing 1. Fork (https://github.com/michaelhball/
 discogs_alert/fork) 2. Create your feature branch (git checkout -b feature/
 fooBar) 3. Commit your changes (git commit -am 'Add some fooBar') 4. Push to
 the branch (git push origin feature/fooBar) 5. Create a new Pull Request ###
 Setting up the dev environment Ideally, you should work inside a virtual
 environment set up for this project. Once that's the case, simply run the
 following two commands to install all dependencies: * `$ pip install --user
 poetry` * `$ poetry install` And that's it! Until you want to push your changes
```

