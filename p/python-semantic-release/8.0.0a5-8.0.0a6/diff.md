# Comparing `tmp/python-semantic-release-8.0.0a5.tar.gz` & `tmp/python-semantic-release-8.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-semantic-release-8.0.0a5.tar", last modified: Mon Apr 17 20:00:17 2023, max compression
+gzip compressed data, was "python-semantic-release-8.0.0a6.tar", last modified: Sun Jun  4 17:38:36 2023, max compression
```

## Comparing `python-semantic-release-8.0.0a5.tar` & `python-semantic-release-8.0.0a6.tar`

### file list

```diff
@@ -1,126 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.356697 python-semantic-release-8.0.0a5/
--rw-r--r--   0 root         (0) root         (0)      230 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/AUTHORS.rst
--rw-r--r--   0 root         (0) root         (0)     1084 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      153 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2696 2023-04-17 20:00:17.356697 python-semantic-release-8.0.0a5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1858 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/README.rst
--rw-r--r--   0 root         (0) root         (0)     5340 2023-04-17 19:59:59.000000 python-semantic-release-8.0.0a5/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2696 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4022 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      520 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2023-04-17 20:00:17.000000 python-semantic-release-8.0.0a5/python_semantic_release.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/
--rw-r--r--   0 root         (0) root         (0)     1093 2023-04-17 19:59:59.000000 python-semantic-release-8.0.0a5/semantic_release/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)      361 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/changelog/context.py
--rw-r--r--   0 root         (0) root         (0)     6470 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/changelog/release_history.py
--rw-r--r--   0 root         (0) root         (0)     4328 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/changelog/template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)      451 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/changelog.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/generate_config.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/main.py
--rw-r--r--   0 root         (0) root         (0)     2954 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/publish.py
--rw-r--r--   0 root         (0) root         (0)    16552 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/commands/version.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/common.py
--rw-r--r--   0 root         (0) root         (0)    17524 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/config.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/const.py
--rw-r--r--   0 root         (0) root         (0)     2875 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      935 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/cli/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)      884 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2569 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/_base.py
--rw-r--r--   0 root         (0) root         (0)     4364 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/angular.py
--rw-r--r--   0 root         (0) root         (0)     3288 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/emoji.py
--rw-r--r--   0 root         (0) root         (0)     5713 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/scipy.py
--rw-r--r--   0 root         (0) root         (0)     3193 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/tag.py
--rw-r--r--   0 root         (0) root         (0)      846 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/token.py
--rw-r--r--   0 root         (0) root         (0)      529 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/commit_parser/util.py
--rw-r--r--   0 root         (0) root         (0)      615 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.344697 python-semantic-release-8.0.0a5/semantic_release/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/data/templates/
--rw-r--r--   0 root         (0) root         (0)     1143 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/data/templates/CHANGELOG.md.j2
--rw-r--r--   0 root         (0) root         (0)      507 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/data/templates/release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)     1020 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/enums.py
--rw-r--r--   0 root         (0) root         (0)      674 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/errors.py
--rw-r--r--   0 root         (0) root         (0)     4088 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.348697 python-semantic-release-8.0.0a5/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)      300 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/_base.py
--rw-r--r--   0 root         (0) root         (0)     9035 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/gitea.py
--rw-r--r--   0 root         (0) root         (0)    10675 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/github.py
--rw-r--r--   0 root         (0) root         (0)     6016 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/gitlab.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/token_auth.py
--rw-r--r--   0 root         (0) root         (0)     2708 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/hvcs/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)      339 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14177 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/algorithm.py
--rw-r--r--   0 root         (0) root         (0)     7267 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/declaration.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/translator.py
--rw-r--r--   0 root         (0) root         (0)    14060 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/semantic_release/version/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 20:00:17.356697 python-semantic-release-8.0.0a5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      466 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.344697 python-semantic-release-8.0.0a5/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/command_line/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/__init__.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/conftest.py
--rw-r--r--   0 root         (0) root         (0)     5707 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_generate_config.py
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_help.py
--rw-r--r--   0 root         (0) root         (0)      501 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_main.py
--rw-r--r--   0 root         (0) root         (0)    23514 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/command_line/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/fixtures/
--rw-r--r--   0 root         (0) root         (0)      106 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/__init__.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/commit_parsers.py
--rw-r--r--   0 root         (0) root         (0)     2235 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/example_project.py
--rw-r--r--   0 root         (0) root         (0)    45283 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/git_repo.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/fixtures/scipy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/scenario/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/scenario/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46838 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/scenario/test_next_version.py
--rw-r--r--   0 root         (0) root         (0)    12186 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/scenario/test_release_history.py
--rw-r--r--   0 root         (0) root         (0)     3513 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/scenario/test_template_render.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5089 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_changelog_context.py
--rw-r--r--   0 root         (0) root         (0)     2540 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_default_changelog.py
--rw-r--r--   0 root         (0) root         (0)     1747 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_release_notes.py
--rw-r--r--   0 root         (0) root         (0)     2102 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1730 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_config.py
--rw-r--r--   0 root         (0) root         (0)     5768 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_masking_filter.py
--rw-r--r--   0 root         (0) root         (0)      799 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/helper.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_angular.py
--rw-r--r--   0 root         (0) root         (0)     2487 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_emoji.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_scipy.py
--rw-r--r--   0 root         (0) root         (0)     2173 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.352697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test__base.py
--rw-r--r--   0 root         (0) root         (0)    24084 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_gitea.py
--rw-r--r--   0 root         (0) root         (0)    25564 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_github.py
--rw-r--r--   0 root         (0) root         (0)    10376 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_gitlab.py
--rw-r--r--   0 root         (0) root         (0)      965 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_token_auth.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 20:00:17.356697 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7319 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_declaration.py
--rw-r--r--   0 root         (0) root         (0)     2996 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_translator.py
--rw-r--r--   0 root         (0) root         (0)     9640 2023-04-17 19:59:07.000000 python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/AUTHORS.rst
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      153 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2272 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/README.rst
+-rw-r--r--   0 root         (0) root         (0)     4632 2023-06-04 17:38:28.000000 python-semantic-release-8.0.0a6/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.161791 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4186 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-06-04 17:38:36.000000 python-semantic-release-8.0.0a6/python_semantic_release.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.161791 python-semantic-release-8.0.0a6/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-06-04 17:38:28.000000 python-semantic-release-8.0.0a6/semantic_release/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.161791 python-semantic-release-8.0.0a6/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)      361 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/changelog/context.py
+-rw-r--r--   0 root         (0) root         (0)     6470 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/changelog/release_history.py
+-rw-r--r--   0 root         (0) root         (0)     4328 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/changelog/template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/generate_config.py
+-rw-r--r--   0 root         (0) root         (0)     4451 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/main.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/publish.py
+-rw-r--r--   0 root         (0) root         (0)    18060 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/commands/version.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/common.py
+-rw-r--r--   0 root         (0) root         (0)    13693 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/const.py
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     2875 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/cli/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)      884 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2569 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/_base.py
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/angular.py
+-rw-r--r--   0 root         (0) root         (0)     3288 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/emoji.py
+-rw-r--r--   0 root         (0) root         (0)     5713 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/scipy.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/token.py
+-rw-r--r--   0 root         (0) root         (0)      529 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/commit_parser/util.py
+-rw-r--r--   0 root         (0) root         (0)      831 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.157791 python-semantic-release-8.0.0a6/semantic_release/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/data/templates/
+-rw-r--r--   0 root         (0) root         (0)     1059 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/data/templates/CHANGELOG.md.j2
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/data/templates/release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/enums.py
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/errors.py
+-rw-r--r--   0 root         (0) root         (0)     4088 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)      300 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/_base.py
+-rw-r--r--   0 root         (0) root         (0)     8285 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/gitea.py
+-rw-r--r--   0 root         (0) root         (0)    10154 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/github.py
+-rw-r--r--   0 root         (0) root         (0)     5029 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/token_auth.py
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/hvcs/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.165791 python-semantic-release-8.0.0a6/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14177 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     7267 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/declaration.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/translator.py
+-rw-r--r--   0 root         (0) root         (0)    14060 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/semantic_release/version/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      466 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.161791 python-semantic-release-8.0.0a6/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/command_line/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     5707 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_generate_config.py
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_help.py
+-rw-r--r--   0 root         (0) root         (0)      501 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_main.py
+-rw-r--r--   0 root         (0) root         (0)    25217 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/command_line/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/fixtures/
+-rw-r--r--   0 root         (0) root         (0)      106 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/commit_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/example_project.py
+-rw-r--r--   0 root         (0) root         (0)    45283 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/git_repo.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/fixtures/scipy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/scenario/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/scenario/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46838 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/scenario/test_next_version.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/scenario/test_release_history.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/scenario/test_template_render.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5005 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_changelog_context.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_default_changelog.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_release_notes.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_config.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_github_actions_output.py
+-rw-r--r--   0 root         (0) root         (0)     5768 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_masking_filter.py
+-rw-r--r--   0 root         (0) root         (0)      799 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.169791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/helper.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_angular.py
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_emoji.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_scipy.py
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      648 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_token.py
+-rw-r--r--   0 root         (0) root         (0)      442 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test__base.py
+-rw-r--r--   0 root         (0) root         (0)    22874 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_gitea.py
+-rw-r--r--   0 root         (0) root         (0)    24334 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_github.py
+-rw-r--r--   0 root         (0) root         (0)    10021 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_gitlab.py
+-rw-r--r--   0 root         (0) root         (0)      965 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_token_auth.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-04 17:38:36.173791 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7319 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_declaration.py
+-rw-r--r--   0 root         (0) root         (0)     2996 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_translator.py
+-rw-r--r--   0 root         (0) root         (0)     9640 2023-06-04 17:37:58.000000 python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_version.py
```

### Comparing `python-semantic-release-8.0.0a5/LICENSE` & `python-semantic-release-8.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/PKG-INFO` & `python-semantic-release-8.0.0a6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0a5
+Version: 8.0.0a6
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -49,11 +49,19 @@
 
 .. _semantic-release: https://github.com/semantic-release/semantic-release
 .. _talk from JSConf Budapest: https://www.youtube.com/watch?v=tc2UgG5L7WM
 .. _getting started guide: https://python-semantic-release.readthedocs.io/en/latest/#getting-started
 .. _GitHub Action: https://python-semantic-release.readthedocs.io/en/latest/automatic-releases/github-actions.html
 .. _conda-forge: https://anaconda.org/conda-forge/python-semantic-release
 
-.. |Test Status| image:: https://img.shields.io/github/workflow/status/relekang/python-semantic-release/Test%20%26%20Release?label=Tests&logo=github
+.. |Test Status| image:: https://img.shields.io/github/actions/workflow/status/python-semantic-release/python-semantic-release/main.yml?branch=master&label=Test%20Status&logo=github
+   :target: https://github.com/python-semantic-release/python-semantic-release/actions/workflows/main.yml
+   :alt: test-status
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/python-semantic-release?label=PyPI&logo=pypi
+   :target: https://pypi.org/project/python-semantic-release/
+   :alt: pypi
 .. |conda-forge Version| image:: https://img.shields.io/conda/vn/conda-forge/python-semantic-release?logo=anaconda
-.. |Read the Docs Status| image:: https://img.shields.io/readthedocs/python-semantic-release?label=Read%20the%20Docs&logo=read-the-docs
+   :target: https://anaconda.org/conda-forge/python-semantic-release
+   :alt: conda-forge
+.. |Read the Docs Status| image:: https://img.shields.io/readthedocs/python-semantic-release?label=Read%20the%20Docs&logo=Read%20the%20Docs
+   :target: https://python-semantic-release.readthedocs.io/en/latest/
+   :alt: docs
```

### Comparing `python-semantic-release-8.0.0a5/README.rst` & `python-semantic-release-8.0.0a6/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -26,11 +26,19 @@
 
 .. _semantic-release: https://github.com/semantic-release/semantic-release
 .. _talk from JSConf Budapest: https://www.youtube.com/watch?v=tc2UgG5L7WM
 .. _getting started guide: https://python-semantic-release.readthedocs.io/en/latest/#getting-started
 .. _GitHub Action: https://python-semantic-release.readthedocs.io/en/latest/automatic-releases/github-actions.html
 .. _conda-forge: https://anaconda.org/conda-forge/python-semantic-release
 
-.. |Test Status| image:: https://img.shields.io/github/workflow/status/relekang/python-semantic-release/Test%20%26%20Release?label=Tests&logo=github
+.. |Test Status| image:: https://img.shields.io/github/actions/workflow/status/python-semantic-release/python-semantic-release/main.yml?branch=master&label=Test%20Status&logo=github
+   :target: https://github.com/python-semantic-release/python-semantic-release/actions/workflows/main.yml
+   :alt: test-status
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/python-semantic-release?label=PyPI&logo=pypi
+   :target: https://pypi.org/project/python-semantic-release/
+   :alt: pypi
 .. |conda-forge Version| image:: https://img.shields.io/conda/vn/conda-forge/python-semantic-release?logo=anaconda
-.. |Read the Docs Status| image:: https://img.shields.io/readthedocs/python-semantic-release?label=Read%20the%20Docs&logo=read-the-docs
+   :target: https://anaconda.org/conda-forge/python-semantic-release
+   :alt: conda-forge
+.. |Read the Docs Status| image:: https://img.shields.io/readthedocs/python-semantic-release?label=Read%20the%20Docs&logo=Read%20the%20Docs
+   :target: https://python-semantic-release.readthedocs.io/en/latest/
+   :alt: docs
```

### Comparing `python-semantic-release-8.0.0a5/pyproject.toml` & `python-semantic-release-8.0.0a6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # and https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-semantic-release"
-version = "8.0.0-alpha.5"
+version = "8.0.0-alpha.6"
 description = "Automatic Semantic Versioning for Python projects"
 requires-python = ">=3.7"
 license = { text = "MIT" }
 classifiers = [
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
   "Programming Language :: Python :: 3.7",
@@ -19,47 +19,49 @@
   "Programming Language :: Python :: 3.10",
 ]
 readme = "README.rst"
 authors = [{ name = "Rolf Erik Lekang", email = "me@rolflekang.com" }]
 dependencies = [
   "click>=7,<9",
   "gitpython>=3.0.8,<4",
-  "twine>=4,<5",
   "requests>=2.25,<3",
   "jinja2>=3.1.2,<4",
   "python-gitlab>=2,<4",
   "tomlkit~=0.10",
   "dotty-dict>=1.3.0,<2",
   "dataclasses==0.8; python_version < '3.7.0'",
   "importlib-resources==5.7",
   "pydantic>=1.10.2,<2",
+  "rich>=12.5.1",
+  "shellingham>=1.5.0.post1",
 ]
 
 [project.scripts]
 semantic-release = "semantic_release.cli:main"
 
 [project.urls]
 "Project Url" = "http://github.com/python-semantic-release/python-semantic-release"
 Homepage = "https://python-semantic-release.readthedocs.io"
 
 [project.optional-dependencies]
 docs = [
   "Sphinx==5.2.3",
   "sphinxcontrib-apidoc==0.3.0",
-  "sphinx-autobuild==2021.3.14",
+  "sphinx-autobuild==2021.03.14",
 ]
 test = [
   "coverage[toml]>=6,<7",
   "pytest>=7,<8",
   "pytest-xdist>=2,<3",
   "pytest-mock>=3,<4",
   "pytest-lazy-fixture~=0.6.3",
   "pytest-cov>=4,<5",
   "responses==0.21.0",
   "requests-mock>=1.10.0,<2",
+  "types-pytest-lazy-fixture>=0.6.3.3",
 ]
 dev = ["tox", "isort", "black"]
 mypy = ["mypy", "types-requests"]
 
 [tool.pytest.ini_options]
 addopts = [
   "-nauto",
@@ -132,15 +134,18 @@
 
 [tool.semantic_release]
 logging_use_named_masks = true
 tag_format = "v{version}"
 commit_parser = "angular"
 commit_author = "semantic-release <semantic-release>"
 commit_message = "{version}\n\nAutomatically generated by python-semantic-release"
-build_command = "python setup.py sdist bdist_wheel"
+build_command = """
+    python -m pip install build~=0.10.0
+    python -m build .
+"""
 major_on_zero = true
 assets = []
 version_variables = ["semantic_release/__init__.py:__version__"]
 version_toml = ["pyproject.toml:project.version"]
 
 [tool.semantic_release.commit_parser_options]
 allowed_tags = [
@@ -186,48 +191,13 @@
 match = "8.0.x"
 prerelease = true
 prerelease_token = "alpha"
 
 [tool.semantic_release.remote]
 name = "origin"
 type = "github"
-ignore_token_for_push = true
+ignore_token_for_push = false
 token = { env = "GH_TOKEN" }
 
-[tool.semantic_release.upload]
+[tool.semantic_release.publish]
 dist_glob_patterns = ["dist/*"]
-upload_to_repository = true
 upload_to_vcs_release = true
-sign = false
-sign_with = "gpg"
-config_file = "~/.pypirc"
-skip_existing = false
-repository_name = "pypi"
-disable_progress_bar = false
-
-[tool.semantic_release.upload.pypi_token]
-env = "PYPI_TOKEN"
-
-[tool.semantic_release.upload.identity]
-env = "GPG_IDENTITIY"
-
-[tool.semantic_release.upload.username]
-env = "REPOSITORY_USERNAME"
-default_env = "TWINE_USERNAME"
-
-[tool.semantic_release.upload.password]
-env = "REPOSITORY_PASSWORD"
-default_env = "TWINE_PASSWORD"
-
-[tool.semantic_release.upload.non_interactive]
-env = "TWINE_NON_INTERACTIVE"
-default = "true"
-
-[tool.semantic_release.upload.cacert]
-env = "TWINE_CERT"
-
-[tool.semantic_release.upload.client_cert]
-env = "TWINE_CLIENT_CERT"
-
-[tool.semantic_release.upload.repository_url]
-env = "REPOSITORY_URL"
-default_env = "TWINE_REPOSITORY_URL"
```

### Comparing `python-semantic-release-8.0.0a5/python_semantic_release.egg-info/PKG-INFO` & `python-semantic-release-8.0.0a6/python_semantic_release.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-semantic-release
-Version: 8.0.0a5
+Version: 8.0.0a6
 Summary: Automatic Semantic Versioning for Python projects
 Author-email: Rolf Erik Lekang <me@rolflekang.com>
 License: MIT
 Project-URL: Project Url, http://github.com/python-semantic-release/python-semantic-release
 Project-URL: Homepage, https://python-semantic-release.readthedocs.io
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -49,11 +49,19 @@
 
 .. _semantic-release: https://github.com/semantic-release/semantic-release
 .. _talk from JSConf Budapest: https://www.youtube.com/watch?v=tc2UgG5L7WM
 .. _getting started guide: https://python-semantic-release.readthedocs.io/en/latest/#getting-started
 .. _GitHub Action: https://python-semantic-release.readthedocs.io/en/latest/automatic-releases/github-actions.html
 .. _conda-forge: https://anaconda.org/conda-forge/python-semantic-release
 
-.. |Test Status| image:: https://img.shields.io/github/workflow/status/relekang/python-semantic-release/Test%20%26%20Release?label=Tests&logo=github
+.. |Test Status| image:: https://img.shields.io/github/actions/workflow/status/python-semantic-release/python-semantic-release/main.yml?branch=master&label=Test%20Status&logo=github
+   :target: https://github.com/python-semantic-release/python-semantic-release/actions/workflows/main.yml
+   :alt: test-status
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/python-semantic-release?label=PyPI&logo=pypi
+   :target: https://pypi.org/project/python-semantic-release/
+   :alt: pypi
 .. |conda-forge Version| image:: https://img.shields.io/conda/vn/conda-forge/python-semantic-release?logo=anaconda
-.. |Read the Docs Status| image:: https://img.shields.io/readthedocs/python-semantic-release?label=Read%20the%20Docs&logo=read-the-docs
+   :target: https://anaconda.org/conda-forge/python-semantic-release
+   :alt: conda-forge
+.. |Read the Docs Status| image:: https://img.shields.io/readthedocs/python-semantic-release?label=Read%20the%20Docs&logo=Read%20the%20Docs
+   :target: https://python-semantic-release.readthedocs.io/en/latest/
+   :alt: docs
```

### Comparing `python-semantic-release-8.0.0a5/python_semantic_release.egg-info/SOURCES.txt` & `python-semantic-release-8.0.0a6/python_semantic_release.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 semantic_release/changelog/context.py
 semantic_release/changelog/release_history.py
 semantic_release/changelog/template.py
 semantic_release/cli/__init__.py
 semantic_release/cli/common.py
 semantic_release/cli/config.py
 semantic_release/cli/const.py
+semantic_release/cli/github_actions_output.py
 semantic_release/cli/masking_filter.py
 semantic_release/cli/util.py
 semantic_release/cli/commands/__init__.py
 semantic_release/cli/commands/changelog.py
 semantic_release/cli/commands/generate_config.py
 semantic_release/cli/commands/main.py
 semantic_release/cli/commands/publish.py
@@ -75,22 +76,24 @@
 tests/unit/semantic_release/changelog/__init__.py
 tests/unit/semantic_release/changelog/test_changelog_context.py
 tests/unit/semantic_release/changelog/test_default_changelog.py
 tests/unit/semantic_release/changelog/test_release_notes.py
 tests/unit/semantic_release/changelog/test_template.py
 tests/unit/semantic_release/cli/__init__.py
 tests/unit/semantic_release/cli/test_config.py
+tests/unit/semantic_release/cli/test_github_actions_output.py
 tests/unit/semantic_release/cli/test_masking_filter.py
 tests/unit/semantic_release/cli/test_version.py
 tests/unit/semantic_release/commit_parser/__init__.py
 tests/unit/semantic_release/commit_parser/helper.py
 tests/unit/semantic_release/commit_parser/test_angular.py
 tests/unit/semantic_release/commit_parser/test_emoji.py
 tests/unit/semantic_release/commit_parser/test_scipy.py
 tests/unit/semantic_release/commit_parser/test_tag.py
+tests/unit/semantic_release/commit_parser/test_token.py
 tests/unit/semantic_release/commit_parser/test_util.py
 tests/unit/semantic_release/hvcs/__init__.py
 tests/unit/semantic_release/hvcs/test__base.py
 tests/unit/semantic_release/hvcs/test_gitea.py
 tests/unit/semantic_release/hvcs/test_github.py
 tests/unit/semantic_release/hvcs/test_gitlab.py
 tests/unit/semantic_release/hvcs/test_token_auth.py
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/__init__.py` & `python-semantic-release-8.0.0a6/semantic_release/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from semantic_release.version import (
     Version as Version,
     VersionTranslator as VersionTranslator,
     next_version as next_version,
     tags_and_versions as tags_and_versions,
 )
 
-__version__ = "8.0.0-alpha.5"
+__version__ = "8.0.0-alpha.6"
 
 
 def setup_hook(argv: list[str]) -> None:
     """
     A hook to be used in setup.py to enable `python setup.py publish`.
 
     :param argv: sys.argv
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/changelog/context.py` & `python-semantic-release-8.0.0a6/semantic_release/changelog/context.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/changelog/release_history.py` & `python-semantic-release-8.0.0a6/semantic_release/changelog/release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/changelog/template.py` & `python-semantic-release-8.0.0a6/semantic_release/changelog/template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/cli/commands/changelog.py` & `python-semantic-release-8.0.0a6/semantic_release/cli/commands/changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/cli/commands/generate_config.py` & `python-semantic-release-8.0.0a6/semantic_release/cli/commands/generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/cli/commands/main.py` & `python-semantic-release-8.0.0a6/semantic_release/cli/commands/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     RuntimeContext,
     read_toml,
 )
 from semantic_release.cli.const import DEFAULT_CONFIG_FILE
 from semantic_release.cli.util import rprint
 from semantic_release.errors import InvalidConfiguration, NotAReleaseBranch
 
-FORMAT = "[%(name)s] %(module)s:%(funcName)s: %(message)s"
+FORMAT = "[%(name)s] %(levelname)s %(module)s.%(funcName)s: %(message)s"
 
 
 @click.group(
     context_settings={
         "help_option_names": ["-h", "--help"],
     },
 )
@@ -66,17 +66,14 @@
 
     Automated Semantic Versioning based on version 2.0.0 of the Semantic Versioning
     specification, which can be found at https://semver.org/spec/v2.0.0.html.
 
     Detect the next semantically correct version for a project based on the Git
     history, create and publish a changelog to a remote VCS, build a project.
 
-    If the project is written in Python, distributions can also be
-    uploaded to a remote Python package repository using twine.
-
     For more information, visit https://python-semantic-release.readthedocs.io/
     """
 
     console = Console(stderr=True)
 
     log_level = [logging.WARNING, logging.INFO, logging.DEBUG][verbosity]
     logging.basicConfig(
@@ -110,22 +107,22 @@
             "'--noop' flag was supplied"
         )
     cli_options = GlobalCommandLineOptions(
         noop=noop, verbosity=verbosity, config_file=config_file
     )
 
     try:
-        if config_file and config_file.endswith(".toml"):
+        if config_file.endswith(".toml"):
             log.info(f"Loading TOML configuration from {config_file}")
             config_text = read_toml(config_file)
-        elif config_file and config_file.endswith(".json"):
+        elif config_file.endswith(".json"):
             log.info(f"Loading JSON configuration from {config_file}")
             raw_text = (Path() / config_file).resolve().read_text(encoding="utf-8")
             config_text = json.loads(raw_text)["semantic_release"]
-        elif config_file:
+        else:
             *_, suffix = config_file.split(".")
             ctx.fail(f"{suffix!r} is not a supported configuration format")
     except (FileNotFoundError, InvalidConfiguration) as exc:
         ctx.fail(str(exc))
 
     raw_config = RawConfig.parse_obj(config_text)
     try:
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/cli/commands/version.py` & `python-semantic-release-8.0.0a6/semantic_release/cli/commands/version.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from __future__ import annotations
 
 import logging
 import os
+import subprocess
 from contextlib import nullcontext
 from datetime import datetime
 from typing import TYPE_CHECKING, ContextManager
 
 import click
+import shellingham  # type: ignore[import]
 
 from semantic_release.changelog import ReleaseHistory, environment, recursive_render
 from semantic_release.changelog.context import make_changelog_context
 from semantic_release.cli.common import (
     render_default_changelog_file,
     render_release_notes,
 )
+from semantic_release.cli.github_actions_output import VersionGitHubActionsOutput
 from semantic_release.cli.util import indented, noop_report, rprint
-from semantic_release.const import DEFAULT_VERSION
+from semantic_release.const import DEFAULT_SHELL, DEFAULT_VERSION
 from semantic_release.enums import LevelBump
 from semantic_release.version import (
     Version,
     VersionTranslator,
     next_version,
     tags_and_versions,
 )
@@ -81,14 +84,29 @@
         for declaration in version_declarations:
             new_content = declaration.replace(new_version=version)
             declaration.path.write_text(new_content)
 
     return paths
 
 
+def shell(cmd: str, *, check: bool = True) -> subprocess.CompletedProcess:
+    shell: str | None
+    try:
+        shell, _ = shellingham.detect_shell()
+    except shellingham.ShellDetectionFailure:
+        log.warning("failed to detect shell, using default shell: %s", DEFAULT_SHELL)
+        log.debug("stack trace", exc_info=True)
+        shell = DEFAULT_SHELL
+
+    if not shell:
+        raise TypeError("'shell' is None")
+
+    return subprocess.run([shell, "-c", cmd], check=check)
+
+
 @click.command(
     short_help="Detect and apply a new version",
     context_settings={
         "help_option_names": ["-h", "--help"],
     },
 )
 @click.option(
@@ -148,15 +166,15 @@
     default=True,
     help="Whether or not to create a release in the remote VCS, if supported",
 )
 @click.option(
     "--build-metadata",
     "build_metadata",
     default=os.getenv("PSR_BUILD_METADATA"),
-    help="Build metadata to append to the latest version",
+    help="Build metadata to append to the new version",
 )
 @click.pass_context
 def version(
     ctx: click.Context,
     print_only: bool = False,
     force_prerelease: bool = False,
     prerelease_token: str | None = None,
@@ -196,15 +214,19 @@
     changelog_excluded_commit_patterns = runtime.changelog_excluded_commit_patterns
     env = runtime.template_environment
     template_dir = runtime.template_dir
     assets = runtime.assets
     commit_author = runtime.commit_author
     commit_message = runtime.commit_message
     major_on_zero = runtime.major_on_zero
+    build_command = runtime.build_command
     opts = runtime.global_cli_options
+    gha_output = VersionGitHubActionsOutput()
+
+    ctx.call_on_close(gha_output.write_if_possible)
 
     if prerelease_token:
         log.info("Forcing use of %s as the prerelease token", prerelease_token)
         translator.prerelease_token = prerelease_token
 
     # Only push if we're committing changes
     if push_changes and not commit_changes:
@@ -250,14 +272,16 @@
             prerelease=prerelease,
             major_on_zero=major_on_zero,
         )
 
     if build_metadata:
         new_version.build_metadata = build_metadata
 
+    gha_output.released = False
+    gha_output.version = new_version
     # If the new version has already been released, we fail and abort
     if new_version in {v for _, v in tags_and_versions(repo.tags, translator)}:
         ctx.fail(
             f"No release will be made, {str(new_version)} has already been released!"
         )
 
     if print_only:
@@ -272,14 +296,30 @@
         repo=repo,
         version_declarations=runtime.version_declarations,
         version=new_version,
         noop=opts.noop,
     )
     all_paths_to_add = files_with_new_version_written + (assets or [])
 
+    # Build distributions before committing any changes - this way if the
+    # build fails, modifications to the source code won't be committed
+    if not build_command:
+        rprint("[green]No build command specified, skipping")
+    if runtime.global_cli_options.noop:
+        noop_report(f"would have run the build_command {build_command}")
+    else:
+        try:
+            log.info("Running build command %s", build_command)
+            rprint(
+                f"[bold green]:hammer_and_wrench: Running build command: {build_command}"
+            )
+            shell(build_command, check=True)
+        except subprocess.CalledProcessError as exc:
+            ctx.fail(str(exc))
+
     # Commit changes
     if commit_changes and opts.noop:
         # Indents the newlines so that terminal formatting is happy - note the
         # git commit line of the output is 24 spaces indented too
         # Only this message needs such special handling because of the newlines
         # that might be in a commit message between the subject and body
         indented_commit_message = commit_message.format(version=new_version).replace(
@@ -446,18 +486,19 @@
                     would have run:
                         git push {runtime.masker.mask(remote_url)} {active_branch}
                         git push --tags {runtime.masker.mask(remote_url)} {active_branch}
                     """
                 )
             )
         else:
-            # Wrap in GitCommandError handling - remove token
             repo.git.push(remote_url, active_branch)
             repo.git.push("--tags", remote_url, active_branch)
 
+    gha_output.released = True
+
     if make_vcs_release and opts.noop:
         noop_report(
             f"would have created a release for the tag {new_version.as_tag()!r}"
         )
         noop_report(f"would have uploaded the following assets: {runtime.assets}")
     elif make_vcs_release:
         release = rh.released[new_version]
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/cli/common.py` & `python-semantic-release-8.0.0a6/semantic_release/cli/common.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/cli/config.py` & `python-semantic-release-8.0.0a6/semantic_release/cli/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from __future__ import annotations
 
 import logging
 import os
-import platform
 import re
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Any, ClassVar, Dict, List, Optional, Tuple, Union
 
 import tomlkit
-import twine.utils
 from git import Actor
 from git.repo.base import Repo
 from jinja2 import Environment
 from pydantic import BaseModel
-from twine.exceptions import TwineException
-from twine.settings import Settings as TwineSettings
 from typing_extensions import Literal
 
 from semantic_release.changelog import environment
 from semantic_release.cli.const import DEFAULT_CONFIG_FILE
 from semantic_release.cli.masking_filter import MaskingFilter
 from semantic_release.commit_parser import (
     AngularCommitParser,
@@ -120,55 +116,23 @@
     url: Optional[MaybeFromEnv] = None
     type: HvcsClient = HvcsClient.GITHUB
     domain: Optional[str] = None
     api_domain: Optional[str] = None
     ignore_token_for_push: bool = False
 
 
-class UploadConfig(BaseModel):
+class PublishConfig(BaseModel):
     dist_glob_patterns: Tuple[str, ...] = ("dist/*",)
-    pypi_token: MaybeFromEnv = EnvConfigVar(env="PYPI_TOKEN")
-    upload_to_repository: bool = True
     upload_to_vcs_release: bool = True
-    # https://twine.readthedocs.io/en/stable/
-    sign: bool = False
-    sign_with: str = "gpg"
-    identity: MaybeFromEnv = EnvConfigVar(env="GPG_IDENTITIY")
-    # https://twine.readthedocs.io/en/stable/#environment-variables
-    # NOTE: this is breaking, as it will no longer check PYPI_USERNAME
-    username: MaybeFromEnv = EnvConfigVar(
-        env="REPOSITORY_USERNAME", default_env="TWINE_USERNAME"
-    )
-    # NOTE: this is breaking, as it will no longer check PYPI_PASSWORD or PYPI_TOKEN
-    password: MaybeFromEnv = EnvConfigVar(
-        env="REPOSITORY_PASSWORD", default_env="TWINE_PASSWORD"
-    )
-    non_interactive: MaybeFromEnv = EnvConfigVar(
-        env="TWINE_NON_INTERACTIVE", default="true"
-    )
-    comment: Optional[str] = None
-    config_file: str = twine.utils.DEFAULT_CONFIG_FILE
-    skip_existing: bool = False
-    cacert: MaybeFromEnv = EnvConfigVar(env="TWINE_CERT")
-    client_cert: MaybeFromEnv = EnvConfigVar(env="TWINE_CLIENT_CERT")
-    repository_name: str = "pypi"
-    repository_url: MaybeFromEnv = EnvConfigVar(
-        env="REPOSITORY_URL", default_env="TWINE_REPOSITORY_URL"
-    )
-    verbose: bool = False
-    disable_progress_bar: bool = False
-
-
-_PY = "py" if platform.system() == "Windows" else "python"
 
 
 class RawConfig(BaseModel):
     assets: Tuple[str, ...] = ()
     branches: Dict[str, BranchConfig] = {"main": BranchConfig()}
-    build_command: str = f"{_PY} setup.py sdist bdist_wheel"
+    build_command: Optional[str] = None
     changelog: ChangelogConfig = ChangelogConfig()
     commit_author: MaybeFromEnv = EnvConfigVar(
         env="GIT_COMMIT_AUTHOR", default=DEFAULT_COMMIT_AUTHOR
     )
     commit_message: str = COMMIT_MESSAGE
     commit_parser: str = "angular"
     # It's up to the parser_options() method to validate these
@@ -188,15 +152,15 @@
         "minor_tags": ["feat"],
         "patch_tags": ["fix", "perf"],
     }
     logging_use_named_masks: bool = False
     major_on_zero: bool = True
     remote: RemoteConfig = RemoteConfig()
     tag_format: str = "v{version}"
-    upload: UploadConfig = UploadConfig()
+    publish: PublishConfig = PublishConfig()
     version_toml: Optional[Tuple[str, ...]] = None
     version_variables: Optional[Tuple[str, ...]] = None
 
 
 @dataclass
 class GlobalCommandLineOptions:
     """
@@ -241,20 +205,15 @@
     HvcsClient.GITLAB: Gitlab,
     HvcsClient.GITEA: Gitea,
 }
 
 
 @dataclass
 class RuntimeContext:
-    _mask_attrs_: ClassVar[List[str]] = [
-        "hvcs_client.token",
-        "twine_settings.password",
-        "twine_settings.cacert",
-        "twine_settings.client_cert",
-    ]
+    _mask_attrs_: ClassVar[List[str]] = ["hvcs_client.token"]
 
     repo: Repo
     commit_parser: CommitParser[ParseResult, ParserOptions]
     version_translator: VersionTranslator
     major_on_zero: bool
     prerelease: bool
     assets: Tuple[str, ...]
@@ -263,18 +222,16 @@
     changelog_excluded_commit_patterns: Tuple[re.Pattern[str], ...]
     version_declarations: Tuple[VersionDeclarationABC, ...]
     hvcs_client: HvcsBase
     changelog_file: Path
     ignore_token_for_push: bool
     template_environment: Environment
     template_dir: str
-    build_command: str
-    twine_settings: Optional[TwineSettings]
+    build_command: Optional[str]
     dist_glob_patterns: Tuple[str, ...]
-    upload_to_repository: bool
     upload_to_vcs_release: bool
     global_cli_options: GlobalCommandLineOptions
     # This way the filter can be passed around if needed, so that another function
     # can accept the filter as an argument and call
     masker: MaskingFilter
 
     @staticmethod
@@ -303,59 +260,14 @@
                 active_branch,
             )
         else:
             raise NotAReleaseBranch(
                 f"branch {active_branch!r} isn't in any release groups; no release will be made"
             )
 
-    @classmethod
-    def make_twine_settings(
-        cls, upload_config: UploadConfig
-    ) -> Optional[TwineSettings]:
-        settings = TwineSettings(
-            sign=upload_config.sign,
-            sign_with=upload_config.sign_with,
-            identity=cls.resolve_from_env(upload_config.identity),
-            username=cls.resolve_from_env(upload_config.username),
-            password=cls.resolve_from_env(upload_config.password),
-            non_interactive=(
-                False
-                if cls.resolve_from_env(upload_config.non_interactive)
-                in ("false", "0", 0)
-                else True
-            ),
-            comment=upload_config.comment,
-            config_file=upload_config.config_file,
-            skip_existing=upload_config.skip_existing,
-            cacert=cls.resolve_from_env(upload_config.cacert),
-            client_cert=cls.resolve_from_env(upload_config.client_cert),
-            repository_name=upload_config.repository_name,
-            repository_url=cls.resolve_from_env(upload_config.repository_url),
-            verbose=(
-                upload_config.verbose
-                or logging.getLogger("semantic_release").getEffectiveLevel()
-                <= logging.INFO
-            ),
-            disable_progress_bar=upload_config.disable_progress_bar,
-        )
-        try:
-            # Twine settings are lazy, so we trigger validation errors now if there
-            # are any
-            settings.username
-            settings.password
-            settings.config_file
-        except TwineException as err:
-            log.warning(
-                "TwineException: uploading to repositories will be unavailable (message: %r)",
-                str(err),
-            )
-            return None
-        else:
-            return settings
-
     def apply_log_masking(self, masker: MaskingFilter) -> MaskingFilter:
         for attr in self._mask_attrs_:
             masker.add_mask_for(str(_recursive_getattr(self, attr)), f"context.{attr}")
             masker.add_mask_for(repr(_recursive_getattr(self, attr)), f"context.{attr}")
         return masker
 
     @classmethod
@@ -459,20 +371,14 @@
         )
 
         # version_translator
         version_translator = VersionTranslator(
             tag_format=raw.tag_format, prerelease_token=branch_config.prerelease_token
         )
 
-        try:
-            twine_settings = cls.make_twine_settings(raw.upload)
-        except TwineException as err:
-            log.warning(str(err))
-            log.warning("uploading to repositories will be unavailable", exc_info=True)
-
         self = cls(
             repo=repo,
             commit_parser=commit_parser,
             version_translator=version_translator,
             major_on_zero=raw.major_on_zero,
             build_command=raw.build_command,
             version_declarations=tuple(version_declarations),
@@ -482,18 +388,16 @@
             commit_author=commit_author,
             commit_message=raw.commit_message,
             changelog_excluded_commit_patterns=changelog_excluded_commit_patterns,
             prerelease=branch_config.prerelease,
             ignore_token_for_push=raw.remote.ignore_token_for_push,
             template_dir=raw.changelog.template_dir,
             template_environment=template_environment,
-            twine_settings=twine_settings,
-            dist_glob_patterns=raw.upload.dist_glob_patterns,
-            upload_to_repository=raw.upload.upload_to_repository,
-            upload_to_vcs_release=raw.upload.upload_to_vcs_release,
+            dist_glob_patterns=raw.publish.dist_glob_patterns,
+            upload_to_vcs_release=raw.publish.upload_to_vcs_release,
             global_cli_options=global_cli_options,
             masker=masker,
         )
         # credential masker
         self.apply_log_masking(self.masker)
 
         return self
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/cli/masking_filter.py` & `python-semantic-release-8.0.0a6/semantic_release/cli/masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/cli/util.py` & `python-semantic-release-8.0.0a6/semantic_release/cli/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/commit_parser/__init__.py` & `python-semantic-release-8.0.0a6/semantic_release/commit_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/commit_parser/_base.py` & `python-semantic-release-8.0.0a6/semantic_release/commit_parser/_base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/commit_parser/angular.py` & `python-semantic-release-8.0.0a6/semantic_release/commit_parser/angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/commit_parser/emoji.py` & `python-semantic-release-8.0.0a6/semantic_release/commit_parser/emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/commit_parser/scipy.py` & `python-semantic-release-8.0.0a6/semantic_release/commit_parser/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/commit_parser/tag.py` & `python-semantic-release-8.0.0a6/semantic_release/commit_parser/tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/commit_parser/util.py` & `python-semantic-release-8.0.0a6/semantic_release/commit_parser/util.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/enums.py` & `python-semantic-release-8.0.0a6/semantic_release/enums.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/errors.py` & `python-semantic-release-8.0.0a6/semantic_release/errors.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/helpers.py` & `python-semantic-release-8.0.0a6/semantic_release/helpers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/hvcs/_base.py` & `python-semantic-release-8.0.0a6/semantic_release/hvcs/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Common functionality and interface for interacting with Git remote VCS
 """
 from __future__ import annotations
 
 import logging
-import os
 import warnings
+from functools import lru_cache
 
 from semantic_release.helpers import parse_git_url
 from semantic_release.hvcs.token_auth import TokenAuth
 from semantic_release.hvcs.util import build_requests_session
 
 logger = logging.getLogger(__name__)
 
@@ -46,14 +46,15 @@
         self.hvcs_domain = hvcs_domain
         self.hvcs_api_domain = hvcs_api_domain
         self.token = token
         auth = None if not self.token else TokenAuth(self.token)
         self._remote_url = remote_url
         self.session = build_requests_session(auth=auth)
 
+    @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         """
         Parse the repository's remote url to identify the repository
         owner and name
         """
         parsed_git_url = parse_git_url(self._remote_url)
         return parsed_git_url.namespace, parsed_git_url.repo_name
@@ -74,22 +75,14 @@
         :param from_rev: The older version to compare. Can be a commit sha, tag or branch name.
         :param to_rev: The newer version to compare. Can be a commit sha, tag or branch name.
         :return: Link to view a comparison between the two versions.
         """
         _not_supported(self, "compare_url")
         return ""
 
-    def check_build_status(self, ref: str) -> bool:
-        """
-        Check the status of a build at `ref` in a remote VCS that reports build
-        statuses, such as GitHub Actions or GitLab CI
-        """
-        _not_supported(self, "check_build_status")
-        return True
-
     def upload_dists(self, tag: str, dist_glob: str) -> int:
         """
         Upload built distributions to a release on a remote VCS that
         supports such uploads
         """
         _not_supported(self, "upload_dists")
         return 0
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/hvcs/gitea.py` & `python-semantic-release-8.0.0a6/semantic_release/hvcs/gitea.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,33 +60,14 @@
         self.api_url = f"https://{self.hvcs_api_domain}"
 
         self.token = token
         auth = None if not self.token else TokenAuth(self.token)
         self.session = build_requests_session(auth=auth)
 
     @logged_function(log)
-    def check_build_status(self, ref: str) -> bool:
-        """Check build status
-        https://gitea.com/api/swagger#/repository/repoCreateStatus
-        :param ref: The sha1 hash of the commit ref
-        :return: Was the build status success?
-        """
-        url = f"{self.api_url}/repos/{self.owner}/{self.repo_name}/statuses/{ref}"
-        try:
-            response = self.session.get(url)
-        except HTTPError as err:
-            log.warning("error checking build status: %s", err)
-            return False
-
-        data = response.json()
-        if isinstance(data, list):
-            return data[0].get("status") == "success"  # type: ignore
-        return data.get("status") == "success"  # type: ignore
-
-    @logged_function(log)
     def create_release(
         self, tag: str, release_notes: str, prerelease: bool = False
     ) -> int:
         """Create a new release
         https://gitea.com/api/swagger#/repository/repoCreateRelease
         :param tag: Tag to create release for
         :param release_notes: The release notes for this version
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/hvcs/github.py` & `python-semantic-release-8.0.0a6/semantic_release/hvcs/github.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from __future__ import annotations
 
 import glob
 import logging
 import mimetypes
 import os
+from functools import lru_cache
 
 from requests import HTTPError
 
 from semantic_release.helpers import logged_function
 from semantic_release.hvcs._base import HvcsBase
 from semantic_release.hvcs.token_auth import TokenAuth
 from semantic_release.hvcs.util import build_requests_session, suppress_not_found
@@ -63,14 +64,15 @@
 
         self.api_url = f"https://{self.hvcs_api_domain}"
 
         self.token = token
         auth = None if not self.token else TokenAuth(self.token)
         self.session = build_requests_session(auth=auth)
 
+    @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         # Github actions context
         if "GITHUB_REPOSITORY" in os.environ:
             log.debug("getting repository owner and name from environment variables")
             owner, name = os.environ["GITHUB_REPOSITORY"].rsplit("/", 1)
             return owner, name
         return super()._get_repository_owner_and_name()
@@ -88,30 +90,14 @@
         """
         return (
             f"https://{self.hvcs_domain}/{self.owner}/{self.repo_name}/compare/"
             f"{from_rev}...{to_rev}"
         )
 
     @logged_function(log)
-    def check_build_status(self, ref: str) -> bool:
-        """Check build status
-        https://docs.github.com/rest/reference/repos#get-the-combined-status-for-a-specific-reference
-        :param ref: The sha1 hash of the commit ref
-        :return: Was the build status success?
-        """
-        url = f"{self.api_url}/repos/{self.owner}/{self.repo_name}/commits/{ref}/status"
-        try:
-            response = self.session.get(url)
-        except HTTPError as err:
-            log.warning("error checking build status: %s", err)
-            return False
-
-        return response.json().get("state") == "success"  # type: ignore
-
-    @logged_function(log)
     def create_release(
         self, tag: str, release_notes: str, prerelease: bool = False
     ) -> int:
         """Create a new release
         https://docs.github.com/rest/reference/repos#create-a-release
         :param tag: Tag to create release for
         :param release_notes: The release notes for this version
@@ -262,14 +248,15 @@
             except HTTPError:
                 log.error("error uploading asset %s", file_path, exc_info=True)
 
         return n_succeeded
 
     def remote_url(self, use_token: bool = True) -> str:
         if not (self.token and use_token):
+            log.info("requested to use token for push but no token set, ignoring...")
             return self._remote_url
         actor = os.getenv("GITHUB_ACTOR")
         return (
             f"https://{actor}:{self.token}@{self.hvcs_domain}/{self.owner}/{self.repo_name}.git"
             if actor
             else f"https://{self.token}@{self.hvcs_domain}/{self.owner}/{self.repo_name}.git"
         )
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/hvcs/gitlab.py` & `python-semantic-release-8.0.0a6/semantic_release/hvcs/gitlab.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Helper code for interacting with a Gitlab remote VCS
 """
 from __future__ import annotations
 
 import logging
 import mimetypes
 import os
+from functools import lru_cache
 from urllib.parse import urlsplit
 
 import gitlab
 
 from semantic_release.helpers import logged_function
 from semantic_release.hvcs._base import HvcsBase
 from semantic_release.hvcs.token_auth import TokenAuth
@@ -68,51 +69,26 @@
         Use Gitlab-CI environment varable to get the server domain, if available
         """
         if "CI_SERVER_URL" in os.environ:
             url = urlsplit(os.environ["CI_SERVER_URL"])
             return f"{url.netloc}{url.path}".rstrip("/")
         return os.getenv("CI_SERVER_HOST")
 
+    @lru_cache(maxsize=1)
     def _get_repository_owner_and_name(self) -> tuple[str, str]:
         """
         Get the repository owner and name from GitLab CI environment variables, if
         available, otherwise from parsing the remote url
         """
         if "CI_PROJECT_NAMESPACE" in os.environ and "CI_PROJECT_NAME" in os.environ:
             log.debug("getting repository owner and name from environment variables")
             return os.environ["CI_PROJECT_NAMESPACE"], os.environ["CI_PROJECT_NAME"]
         return super()._get_repository_owner_and_name()
 
     @logged_function(log)
-    def check_build_status(self, ref: str) -> bool:
-        """Check last build status
-        :param ref: The sha1 hash of the commit ref
-        :return: the status of the pipeline (False if a job failed)
-        """
-        client = gitlab.Gitlab(self.api_url, private_token=self.token)
-        client.auth()
-        jobs = (
-            client.projects.get(f"{self.owner}/{self.repo_name}")
-            .commits.get(ref)
-            .statuses.list()
-        )
-        for job in jobs:
-            # "success" and "skipped" aren't considered
-            if job["status"] == "pending":  # type: ignore[index]
-                log.info(
-                    "Job %s is still in pending status",
-                    job["name"],  # type: ignore[index]
-                )
-                return False
-            if job["status"] == "failed" and not job["allow_failure"]:  # type: ignore[index]
-                log.info("Job %s failed", job["name"])  # type: ignore[index]
-                return False
-        return True
-
-    @logged_function(log)
     def create_release(
         self, tag: str, release_notes: str, prerelease: bool = False
     ) -> bool:
         """Post release changelog
         :param tag: Tag to create release for
         :param release_notes: The release notes for this version
         :param prerelease: This parameter has no effect
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/hvcs/token_auth.py` & `python-semantic-release-8.0.0a6/semantic_release/hvcs/token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/hvcs/util.py` & `python-semantic-release-8.0.0a6/semantic_release/hvcs/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         elif not isinstance(retry, Retry):
             raise ValueError("retry should be a bool, int or Retry instance.")
         adapter = HTTPAdapter(max_retries=retry)
         session.mount("http://", adapter)
         session.mount("https://", adapter)
 
     if auth:
+        logger.debug("setting up default session authentication")
         session.auth = auth
 
     return session
 
 
 _R = TypeVar("_R")
```

### Comparing `python-semantic-release-8.0.0a5/semantic_release/version/algorithm.py` & `python-semantic-release-8.0.0a6/semantic_release/version/algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/version/declaration.py` & `python-semantic-release-8.0.0a6/semantic_release/version/declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/version/translator.py` & `python-semantic-release-8.0.0a6/semantic_release/version/translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/semantic_release/version/version.py` & `python-semantic-release-8.0.0a6/semantic_release/version/version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/command_line/test_changelog.py` & `python-semantic-release-8.0.0a6/tests/command_line/test_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/command_line/test_generate_config.py` & `python-semantic-release-8.0.0a6/tests/command_line/test_generate_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/command_line/test_help.py` & `python-semantic-release-8.0.0a6/tests/command_line/test_help.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/command_line/test_version.py` & `python-semantic-release-8.0.0a6/tests/command_line/test_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from __future__ import annotations
 
 import difflib
 import filecmp
 import re
+import shlex
 import shutil
+from subprocess import CompletedProcess
+from unittest import mock
 
 import pytest
 import tomlkit
 from pytest_lazyfixture import lazy_fixture
 
 from semantic_release.cli import main, version
 
 from tests.const import EXAMPLE_PROJECT_NAME
-from tests.util import flatten_dircmp
+from tests.util import actions_output_to_dict, flatten_dircmp
 
 
 @pytest.mark.parametrize(
     "repo",
     [
         lazy_fixture("repo_with_no_tags_angular_commits"),
         lazy_fixture("repo_with_single_branch_angular_commits"),
@@ -617,7 +620,48 @@
 
     metadata_suffix = "build.abc-12345"
     result = cli_runner.invoke(
         main, [version.name, "--no-push", "--build-metadata", metadata_suffix]
     )
     assert result.exit_code == 0
     assert repo.git.tag(l=f"*{metadata_suffix}")
+
+
+@pytest.mark.parametrize("shell", ("/usr/bin/bash", "/usr/bin/zsh", "powershell"))
+def test_version_runs_build_command(
+    repo_with_git_flow_angular_commits, cli_runner, example_pyproject_toml, shell
+):
+    config = tomlkit.loads(example_pyproject_toml.read_text(encoding="utf-8"))
+    build_command = config["tool"]["semantic_release"]["build_command"]
+    exe = shell.split("/")[-1]
+    with mock.patch(
+        "subprocess.run", return_value=CompletedProcess(args=(), returncode=0)
+    ) as patched_subprocess_run, mock.patch(
+        "shellingham.detect_shell", return_value=(exe, shell)
+    ):
+        result = cli_runner.invoke(
+            main, [version.name, "--patch", "--no-push"]
+        )  # force a new version
+        assert result.exit_code == 0
+
+        patched_subprocess_run.assert_called_once_with(
+            [exe, "-c", build_command], check=True
+        )
+
+
+def test_version_writes_github_actions_output(
+    repo_with_git_flow_angular_commits, cli_runner, monkeypatch, tmp_path
+):
+    mock_output_file = tmp_path / "action.out"
+    monkeypatch.setenv("GITHUB_OUTPUT", str(mock_output_file.resolve()))
+    result = cli_runner.invoke(main, [version.name, "--patch", "--no-push"])
+    assert result.exit_code == 0
+
+    action_outputs = actions_output_to_dict(
+        mock_output_file.read_text(encoding="utf-8")
+    )
+    assert "released" in action_outputs
+    assert action_outputs["released"] == "true"
+    assert "version" in action_outputs
+    assert action_outputs["version"] == "1.2.1"
+    assert "tag" in action_outputs
+    assert action_outputs["tag"] == "v1.2.1"
```

### Comparing `python-semantic-release-8.0.0a5/tests/fixtures/commit_parsers.py` & `python-semantic-release-8.0.0a6/tests/fixtures/commit_parsers.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/fixtures/example_project.py` & `python-semantic-release-8.0.0a6/tests/fixtures/example_project.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/fixtures/git_repo.py` & `python-semantic-release-8.0.0a6/tests/fixtures/git_repo.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/fixtures/scipy.py` & `python-semantic-release-8.0.0a6/tests/fixtures/scipy.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/scenario/test_next_version.py` & `python-semantic-release-8.0.0a6/tests/scenario/test_next_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/scenario/test_release_history.py` & `python-semantic-release-8.0.0a6/tests/scenario/test_release_history.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/scenario/test_template_render.py` & `python-semantic-release-8.0.0a6/tests/scenario/test_template_render.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_changelog_context.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_changelog_context.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 CHANGELOG_TEMPLATE = r"""
 # CHANGELOG
 {% if context.history.unreleased | length > 0 %}
 ## Unreleased
 {% for type_, commits in context.history.unreleased.items() %}
 ### {{ type_ | capitalize }}
 {% for commit in commits %}{% if type_ != "unknown" %}
-* {{ commit.commit.message.rstrip() }} ([`{{ commit.commit.hexsha[:7] }}`]({{ commit.commit.hexsha | commit_hash_url }}))
+* {{ commit.message.rstrip() }} ([`{{ commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
 {% else %}
-* {{ commit.commit.message.rstrip() }} ([`{{ commit.commit.hexsha[:7] }}`]({{ commit.commit.hexsha | commit_hash_url }}))
+* {{ commit.message.rstrip() }} ([`{{ commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
 {% endif %}{% endfor %}{% endfor %}{% endif %}
 {% for version, release in context.history.released.items() %}
 ## {{ version.as_tag() }} ({{ release.tagged_date.strftime("%Y-%m-%d") }})
 {% for type_, commits in release["elements"].items() %}
 ### {{ type_ | capitalize }}
 {% for commit in commits %}{% if type_ != "unknown" %}
-* {{ commit.commit.message.rstrip() }} ([`{{ commit.commit.hexsha[:7] }}`]({{ commit.commit.hexsha | commit_hash_url }}))
+* {{ commit.message.rstrip() }} ([`{{ commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
 {% else %}
-* {{ commit.commit.message.rstrip() }} ([`{{ commit.commit.hexsha[:7] }}`]({{ commit.commit.hexsha | commit_hash_url }}))
+* {{ commit.message.rstrip() }} ([`{{ commit.short_hash }}`]({{ commit.hexsha | commit_hash_url }}))
 {% endif %}{% endfor %}{% endfor %}{% endfor %}
 """
 
 EXPECTED_CHANGELOG_CONTENT_ANGULAR = r"""
 # CHANGELOG
 ## v0.2.0
 ### Feature
```

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_default_changelog.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_default_changelog.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_release_notes.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/changelog/test_template.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/changelog/test_template.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_config.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_masking_filter.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_masking_filter.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/cli/test_version.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/cli/test_version.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_angular.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_angular.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_emoji.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_emoji.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/commit_parser/test_tag.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/commit_parser/test_tag.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test__base.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test__base.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_gitea.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_gitea.py`

 * *Files 6% similar despite different names*

```diff
@@ -188,47 +188,14 @@
 ############
 
 
 gitea_matcher = re.compile(rf"^https://{Gitea.DEFAULT_DOMAIN}")
 gitea_api_matcher = re.compile(rf"^https://{Gitea.DEFAULT_API_DOMAIN}")
 
 
-@pytest.mark.parametrize(
-    "resp_payload, status_code, expected",
-    [
-        ({"status": "success"}, 200, True),
-        ({"status": "pending"}, 200, False),
-        ({"status": "failed"}, 200, False),
-        ([{"status": "success"}] * 2, 200, True),
-        ([{"status": "pending"}] * 2, 200, False),
-        ([{"status": "failed"}] * 2, 200, False),
-        ({}, 404, False),
-    ],
-)
-def test_check_build_status(default_gitea_client, resp_payload, status_code, expected):
-    ref = "refA"
-    with requests_mock.Mocker(session=default_gitea_client.session) as m:
-        m.register_uri(
-            "GET", gitea_api_matcher, json=resp_payload, status_code=status_code
-        )
-        assert default_gitea_client.check_build_status(ref) == expected
-        assert m.called
-        assert len(m.request_history) == 1
-        assert m.last_request.method == "GET"
-        assert (
-            m.last_request.url
-            == "{api_url}/repos/{owner}/{repo_name}/statuses/{ref}".format(
-                api_url=default_gitea_client.api_url,
-                owner=default_gitea_client.owner,
-                repo_name=default_gitea_client.repo_name,
-                ref=ref,
-            )
-        )
-
-
 @pytest.mark.parametrize("status_code", (201,))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_release_succeeds(
     default_gitea_client, status_code, prerelease, mock_release_id
 ):
     tag = "v1.0.0"
```

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_github.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_github.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,47 +229,14 @@
 ############
 
 
 github_matcher = re.compile(rf"^https://{Github.DEFAULT_DOMAIN}")
 github_api_matcher = re.compile(rf"^https://{Github.DEFAULT_API_DOMAIN}")
 
 
-@pytest.mark.parametrize(
-    "resp_payload, status_code, expected",
-    [
-        ({"state": "success"}, 200, True),
-        ({"state": "pending"}, 200, False),
-        ({"state": "failed"}, 200, False),
-        ({"error": "not found"}, 404, False),
-        ({"error": "too many requests"}, 429, False),
-        ({"error": "internal error"}, 500, False),
-        ({"error": "temporarily unavailable"}, 503, False),
-    ],
-)
-def test_check_build_status(default_gh_client, resp_payload, status_code, expected):
-    ref = "refA"
-    with requests_mock.Mocker(session=default_gh_client.session) as m:
-        m.register_uri(
-            "GET", github_api_matcher, json=resp_payload, status_code=status_code
-        )
-        assert default_gh_client.check_build_status(ref) == expected
-        assert m.called
-        assert len(m.request_history) == 1
-        assert m.last_request.method == "GET"
-        assert (
-            m.last_request.url
-            == "{api_url}/repos/{owner}/{repo_name}/commits/{ref}/status".format(
-                api_url=default_gh_client.api_url,
-                owner=default_gh_client.owner,
-                repo_name=default_gh_client.repo_name,
-                ref=ref,
-            )
-        )
-
-
 @pytest.mark.parametrize("status_code", (200, 201))
 @pytest.mark.parametrize("mock_release_id", range(3))
 @pytest.mark.parametrize("prerelease", (True, False))
 def test_create_release_succeeds(
     default_gh_client, status_code, prerelease, mock_release_id
 ):
     tag = "v1.0.0"
```

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_gitlab.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_gitlab.py`

 * *Files 3% similar despite different names*

```diff
@@ -311,28 +311,14 @@
         owner=default_gl_client.owner,
         repo=default_gl_client.repo_name,
         pr_number=pr_number,
     )
 
 
 @pytest.mark.parametrize(
-    "status, expected",
-    [
-        ("pending", False),
-        ("failure", False),
-        ("allow_failure", True),
-        ("success", True),
-    ],
-)
-def test_check_build_status(default_gl_client, status, expected):
-    with mock_gitlab(status=status):
-        assert default_gl_client.check_build_status(REF) == expected
-
-
-@pytest.mark.parametrize(
     "tag, expected",
     [
         (A_GOOD_TAG, True),
         (A_LOCKED_TAG, True),
         (A_BAD_TAG, False),
     ],
 )
```

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/hvcs/test_token_auth.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/hvcs/test_token_auth.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_algorithm.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_algorithm.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_declaration.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_declaration.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_translator.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_translator.py`

 * *Files identical despite different names*

### Comparing `python-semantic-release-8.0.0a5/tests/unit/semantic_release/version/test_version.py` & `python-semantic-release-8.0.0a6/tests/unit/semantic_release/version/test_version.py`

 * *Files identical despite different names*

