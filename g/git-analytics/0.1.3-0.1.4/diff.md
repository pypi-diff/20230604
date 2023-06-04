# Comparing `tmp/git_analytics-0.1.3.tar.gz` & `tmp/git_analytics-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_analytics-0.1.3.tar", max compression
+gzip compressed data, was "git_analytics-0.1.4.tar", max compression
```

## Comparing `git_analytics-0.1.3.tar` & `git_analytics-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1062 2021-11-16 13:27:56.856247 git_analytics-0.1.3/LICENSE
--rw-r--r--   0        0        0      585 2023-02-12 05:20:23.882354 git_analytics-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-02-11 06:31:39.349864 git_analytics-0.1.3/git_analytics/__init__.py
--rw-r--r--   0        0        0     2961 2023-02-12 11:53:43.260213 git_analytics-0.1.3/git_analytics/main.py
--rw-r--r--   0        0        0   163873 2023-02-11 12:10:27.332506 git_analytics-0.1.3/git_analytics/static/css/bootstrap.min.css
--rw-r--r--   0        0        0    10283 2023-02-11 12:18:20.194469 git_analytics-0.1.3/git_analytics/static/index.html
--rw-r--r--   0        0        0    78129 2023-02-11 12:11:11.541079 git_analytics-0.1.3/git_analytics/static/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   192461 2023-02-11 12:11:29.002424 git_analytics-0.1.3/git_analytics/static/js/chart.min.js
--rw-r--r--   0        0        0      472 2023-02-12 11:53:54.279456 git_analytics-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1435 1970-01-01 00:00:00.000000 git_analytics-0.1.3/setup.py
--rw-r--r--   0        0        0     1241 1970-01-01 00:00:00.000000 git_analytics-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1062 2021-11-16 13:27:56.856247 git_analytics-0.1.4/LICENSE
+-rw-r--r--   0        0        0      585 2023-02-12 05:20:23.882354 git_analytics-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-02-11 06:31:39.349864 git_analytics-0.1.4/git_analytics/__init__.py
+-rw-r--r--   0        0        0     4180 2023-06-04 19:14:35.710003 git_analytics-0.1.4/git_analytics/main.py
+-rw-r--r--   0        0        0   163873 2023-02-11 12:10:27.332506 git_analytics-0.1.4/git_analytics/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0    11730 2023-06-04 19:32:20.872837 git_analytics-0.1.4/git_analytics/static/index.html
+-rw-r--r--   0        0        0    78129 2023-02-11 12:11:11.541079 git_analytics-0.1.4/git_analytics/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   192461 2023-02-11 12:11:29.002424 git_analytics-0.1.4/git_analytics/static/js/chart.min.js
+-rw-r--r--   0        0        0      472 2023-06-04 19:14:50.658666 git_analytics-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1442 1970-01-01 00:00:00.000000 git_analytics-0.1.4/setup.py
+-rw-r--r--   0        0        0     1248 1970-01-01 00:00:00.000000 git_analytics-0.1.4/PKG-INFO
```

### Comparing `git_analytics-0.1.3/LICENSE` & `git_analytics-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `git_analytics-0.1.3/README.md` & `git_analytics-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `git_analytics-0.1.3/git_analytics/main.py` & `git_analytics-0.1.4/git_analytics/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,68 @@
 import os
+from dataclasses import dataclass, asdict
 from collections import Counter, defaultdict
 from wsgiref.simple_server import make_server
 
 import falcon
 from git import Repo
 
 
+@dataclass
+class Author:
+    commits: int = 0
+    insertions: int = 0
+    deletions: int = 0
+    maximum_change: int = 0
+
+
 repo: Repo = Repo()
 
-dict_authors = Counter()
+dict_authors = defaultdict(Author)
 dict_day_of_week = defaultdict(Counter)
 dict_hour_of_day = defaultdict(Counter)
 dict_day_of_month = defaultdict(Counter)
 
 dict_tags = Counter()
 dict_tags_of_author = defaultdict(Counter)
-
+dict_number_lines = defaultdict(int)
 
 TYPE_LIST = ['feature', 'fix', 'docs', 'style', 'refactor', 'test', 'chore', 'merge', 'wip',]
 def _get_type_list(commit_message: str):
     part_commit_message = commit_message.split(':')[0]
     return [tag for tag in TYPE_LIST if tag in part_commit_message]
 
-
+lines_in_day = {}
 for c in repo.iter_commits():
-    dict_authors[c.author.name] += 1
+
+    dict_authors[c.author.name].commits += 1
+    dict_authors[c.author.name].insertions += c.stats.total['insertions']
+    dict_authors[c.author.name].deletions += c.stats.total['deletions']
+    if c.stats.total['lines'] > dict_authors[c.author.name].maximum_change:
+        dict_authors[c.author.name].maximum_change = c.stats.total['lines']
+
     dict_day_of_week[c.committed_datetime.weekday()][c.author.name] +=1
     dict_hour_of_day[c.committed_datetime.hour][c.author.name] +=1
     dict_day_of_month[c.committed_datetime.day][c.author.name] +=1
 
+    lines_in_day[c.committed_date] = c.stats.total['insertions'] - c.stats.total['deletions']
+    
     tags = _get_type_list(c.message)
     for tag in tags:
         dict_tags[tag] += 1
         dict_tags_of_author[c.author.name][tag] += 1
 
+old_rows = 0
+sort_day = list(lines_in_day.keys())
+sort_day.sort()
+for day in sort_day:
+    number_rows = lines_in_day[day]
+    dict_number_lines[day] = old_rows + number_rows
+    old_rows = old_rows + number_rows
+
 
 class GitAnaliticsResource:
 
     def on_get_index(self, req, resp):
         raise falcon.HTTPMovedPermanently('index.html')
         
     def on_get_about(self, req, resp):
@@ -47,15 +72,17 @@
             "branch_name": repo.active_branch.name,
             "date_first_commit": str(l[-1].committed_datetime),
             "date_last_commit": str(l[0].committed_datetime),
             "total_number_commit": len(l),
         }
     
     def on_get_authors(self, req, resp):
-        resp.media = dict_authors
+        resp.media = {
+            author: asdict(achievements)
+        for author, achievements in dict_authors.items()}
         
     def on_get_month(self, req, resp):
         resp.media = { day:dict_day_of_month[day] for day in range(1,32)}
 
     def on_get_week(self, req, resp):
         resp.media = {
             'Monday': dict_day_of_week[0],
@@ -65,26 +92,33 @@
             'Friday': dict_day_of_week[4],
             'Saturday': dict_day_of_week[5],
             'Sunday': dict_day_of_week[6],
         }
 
     def on_get_day(self, req, resp):
         resp.media = { hour:dict_hour_of_day[hour] for hour in range(0,24)}
-
+    
+    def on_get_number_lines(self, req, resp):
+        result = [{'date': date, 'value': value} for date, value in dict_number_lines.items()]
+        resp.media = result
 
 app = falcon.App()
 analitics_resource = GitAnaliticsResource()
 
 static_path= os.path.dirname(os.path.abspath(__file__)) + '/static/'
 app.add_static_route('/', static_path)
 app.add_route('/', analitics_resource, suffix='index')
 app.add_route('/api/about', analitics_resource, suffix='about')
 app.add_route('/api/authors', analitics_resource, suffix='authors')
 app.add_route('/api/month', analitics_resource, suffix='month')
 app.add_route('/api/week', analitics_resource, suffix='week')
 app.add_route('/api/day', analitics_resource, suffix='day')
+app.add_route('/api/lines', analitics_resource, suffix='number_lines')
 
 
 def run():
     with make_server('', 8000, app) as httpd:
         print('Service started at http://localhost:8000/')
         httpd.serve_forever()
+
+if __name__ == '__main__':
+    run()
```

### Comparing `git_analytics-0.1.3/git_analytics/static/css/bootstrap.min.css` & `git_analytics-0.1.4/git_analytics/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `git_analytics-0.1.3/git_analytics/static/index.html` & `git_analytics-0.1.4/git_analytics/static/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -5,30 +5,34 @@
     <meta charset="utf-8" />
     <title>Git Analytics</title>
     <link href="css/bootstrap.min.css" rel="stylesheet"
         integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
     <script src="js/bootstrap.bundle.min.js"
         integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p"
         crossorigin="anonymous"></script>
-    <script src="js/chart.min.js" integrity="sha256-7lWo7cjrrponRJcS6bc8isfsPDwSKoaYfGIHgSheQkk="
-        crossorigin="anonymous"></script>
+    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
+
+    <script src="https://cdn.jsdelivr.net/npm/chart.js/dist/chart.min.js"></script>
+    <script
+        src="https://cdn.jsdelivr.net/npm/chartjs-adapter-date-fns/dist/chartjs-adapter-date-fns.bundle.min.js"></script>
+
 </head>
 
 <body>
     <main>
         <div class="container py-4">
             <header class="pb-3 mb-4 border-bottom">
                 <a href="/" class="d-flex align-items-center text-dark text-decoration-none">
                     <span class="fs-4" id="title-branch"></span>
                 </a>
             </header>
 
             <div class="p-5 mb-4 bg-light rounded-3">
                 <div class="container-fluid py-5">
-                    <h1 class="display-5 fw-bold">Сommits by day of the week. </h1>
+                    <h1 class="display-5 fw-bold">Сommits by day of the week</h1>
                     <canvas id="chartWeek" width="400" height="150"></canvas>
                 </div>
             </div>
 
             <div class="row align-items-md-stretch">
                 <div class="col-md-6">
                     <div class="h-100 p-5 text-white bg-dark rounded-3">
@@ -45,27 +49,35 @@
                         <canvas id="chartAuthors" width="150" height="150"></canvas>
                     </div>
                 </div>
             </div>
 
             <div class="p-5 mb-4 bg-light rounded-3">
                 <div class="container-fluid py-5">
-                    <h1 class="display-5 fw-bold">Сommits by hour of the day. </h1>
+                    <h1 class="display-5 fw-bold">Сommits by hour of the day</h1>
                     <canvas id="chartDay" width="400" height="150"></canvas>
                 </div>
             </div>
 
             <div class="p-5 mb-4 bg-light rounded-3">
                 <div class="container-fluid py-5">
-                    <h1 class="display-5 fw-bold">Сommits by day of the month. </h1>
+                    <h1 class="display-5 fw-bold">Сommits by day of the month</h1>
                     <canvas id="chartMonth" width="400" height="150"></canvas>
                 </div>
             </div>
+
+            <div class="p-5 mb-4 bg-light rounded-3">
+                <div class="container-fluid py-5">
+                    <h1 class="display-5 fw-bold">Number of lines of code</h1>
+                    <canvas id="chartLines" width="400" height="150"></canvas>
+                </div>
+            </div>
+
             <footer class="pt-3 mt-4 text-muted border-top">
-                &copy; 2021
+                &copy; 2023
             </footer>
         </div>
     </main>
     <script>
         const COLORS = [
             '#4dc9f6',
             '#f67019',
@@ -78,14 +90,25 @@
             '#8549ba'
         ];
 
         function getColor(index) {
             return COLORS[index % COLORS.length];
         }
 
+        fetch('api/lines')
+            .then((response) => { return response.json() })
+            .then((data) => {
+                values = [];
+                values = []
+                for (let d of data) {
+                    values.push({ x: d.date * 1000, y: d.value })
+                };
+                buildChartLines(values);
+            })
+
         fetch('api/about')
             .then((response) => { return response.json() })
             .then((data) => {
                 document.getElementById('title-branch').innerText = data.branch_name;
                 document.getElementById('text-total').innerText = "Total number of comments: " + data['total_number_commit'];
                 document.getElementById('text-first').innerText = "Date of the first comment: " + data['date_first_commit'];
                 document.getElementById('text-last').innerText = "Date of the last comment: " + data['date_last_commit']
@@ -97,21 +120,17 @@
                 labels = [];
                 dataValues = [];
                 backgroundColor = [];
                 let number_author = 0
                 for (var d in data) {
                     number_author = number_author + 1;
                     labels.push(d);
-                    dataValues.push(data[d]);
+                    dataValues.push(data[d].commits);
                     backgroundColor.push(getColor(number_author));
                 }
-                console.log(labels);
-                console.log(dataValues);
-                console.log(backgroundColor);
-
                 buildChartAuthors(labels, dataValues, backgroundColor);
             })
 
         fetch('api/week')
             .then((response) => { return response.json() })
             .then((data) => {
                 let list_authors = new Set();
@@ -213,14 +232,39 @@
                         'data': dataAuthor,
                         'backgroundColor': getColor(number_author)
                     });
                 }
                 buildChartMonth(list_days_of_month, values);
             })
 
+        function buildChartLines(values) {
+            const ctx = document.getElementById('chartLines');
+            const myChart = new Chart(ctx, {
+                type: 'line',
+                data: {
+                    datasets: [{ data: values }]
+                },
+                options: {
+                    plugins: {
+                        legend: {
+                            display: false,
+                        }
+                    },
+                    scales: {
+                        x: {
+                            type: 'time',
+                            time: {
+                                unit: 'day',
+                            }
+                        }
+                    }
+                }
+            });
+        }
+
         function buildChartAuthors(labels, dataValues, backgroundColor) {
             const ctx = document.getElementById('chartAuthors');
             const myChart = new Chart(ctx, {
                 type: 'pie',
                 data: {
                     labels: labels,
                     datasets: [
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 
-****** Ð¡ommits by day of the week. ******
+****** Ð¡ommits by day of the week ******
 ***** Git analytics *****
 Go_GitHub
 ***** Number of commits by repository authors *****
-****** Ð¡ommits by hour of the day. ******
-****** Ð¡ommits by day of the month. ******
- © 2021
+****** Ð¡ommits by hour of the day ******
+****** Ð¡ommits by day of the month ******
+****** Number of lines of code ******
+ © 2023
```

### Comparing `git_analytics-0.1.3/git_analytics/static/js/bootstrap.bundle.min.js` & `git_analytics-0.1.4/git_analytics/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `git_analytics-0.1.3/git_analytics/static/js/chart.min.js` & `git_analytics-0.1.4/git_analytics/static/js/chart.min.js`

 * *Files identical despite different names*

### Comparing `git_analytics-0.1.3/setup.py` & `git_analytics-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 packages = \
 ['git_analytics']
 
 package_data = \
 {'': ['*'], 'git_analytics': ['static/*', 'static/css/*', 'static/js/*']}
 
 install_requires = \
-['GitPython>=3.1.0', 'falcon>=3.1.0']
+['GitPython>=3.1.0', 'falcon>=3.0.0,<3.1.0']
 
 entry_points = \
 {'console_scripts': ['git-analytics = git_analytics.main:run']}
 
 setup_kwargs = {
     'name': 'git-analytics',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'The detailed analysis tool for git repositories.',
     'long_description': '# Git-Analytics\n\nThe detailed analysis tool for git repositories.\n\n## Installation\n\nThe latest stable version can be installed directly from PyPI:\n\n```sh\npip install git-analytics\n```\n\n## Usage\n\nTo run, enter the command and open the browser at [http://localhost:8000/](http://localhost:8000/).\n\n```sh\ngit-analytics\n```\n\n## Screenshots\n\n![screenshot 1](https://live.staticflickr.com/65535/52679528807_48caac329f_k.jpg)\n\n![screenshot 2](https://live.staticflickr.com/65535/52680543193_c676158df2_k.jpg)\n\n![screenshot 3](https://live.staticflickr.com/65535/52679528732_1f7b9351cd_k.jpg)\n',
     'author': 'n0rfas',
     'author_email': 'antsa@yandex.ru',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `git_analytics-0.1.3/PKG-INFO` & `git_analytics-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: git-analytics
-Version: 0.1.3
+Version: 0.1.4
 Summary: The detailed analysis tool for git repositories.
 License: MIT
 Author: n0rfas
 Author-email: antsa@yandex.ru
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.0)
-Requires-Dist: falcon (>=3.1.0)
+Requires-Dist: falcon (>=3.0.0,<3.1.0)
 Description-Content-Type: text/markdown
 
 # Git-Analytics
 
 The detailed analysis tool for git repositories.
 
 ## Installation
```

